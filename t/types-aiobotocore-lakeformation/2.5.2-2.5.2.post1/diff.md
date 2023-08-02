# Comparing `tmp/types-aiobotocore-lakeformation-2.5.2.tar.gz` & `tmp/types-aiobotocore-lakeformation-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lakeformation-2.5.2.tar", last modified: Sat Jul  8 01:43:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-lakeformation-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
```

## Comparing `types-aiobotocore-lakeformation-2.5.2.tar` & `types-aiobotocore-lakeformation-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:52.998421 types-aiobotocore-lakeformation-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19139 2023-07-08 01:43:52.998421 types-aiobotocore-lakeformation-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17550 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:52.998421 types-aiobotocore-lakeformation-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:52.998421 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39391 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39330 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48272 2023-07-08 01:33:37.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48187 2023-07-08 01:33:37.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:36.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:52.998421 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19139 2023-07-08 01:43:52.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-08 01:43:52.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:52.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:52.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:52.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:43:52.000000 types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.249544 types-aiobotocore-lakeformation-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-08-02 14:52:33.249544 types-aiobotocore-lakeformation-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18225 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.249544 types-aiobotocore-lakeformation-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.249544 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39583 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39522 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    55269 2023-08-02 14:41:44.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55171 2023-08-02 14:41:44.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:43.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.249544 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19767 2023-08-02 14:52:33.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:33.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:33.000000 types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lakeformation-2.5.2/LICENSE` & `types-aiobotocore-lakeformation-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2/PKG-INFO` & `types-aiobotocore-lakeformation-2.5.2.post1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lakeformation
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LakeFormation 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LakeFormation 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lakeformation type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore lakeformation type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lakeformation"></a>
 
 # types-aiobotocore-lakeformation
 
 [![PyPI - types-aiobotocore-lakeformation](https://img.shields.io/pypi/v/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lakeformation?color=blue)](https://pypistats.org/packages/types-aiobotocore-lakeformation)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lakeformation)](https://pepy.tech/project/types-aiobotocore-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LakeFormation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
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
 [types-aiobotocore-lakeformation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/).
 
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
@@ -337,35 +336,36 @@
 )
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lakeformation.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lakeformation.type_defs import (
-    LFTagPairTypeDef,
+    ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
-    AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
+    LFTagPairOutputTypeDef,
+    ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
-    CommitTransactionResponseTypeDef,
     CreateLFTagRequestRequestTypeDef,
+    RowFilterOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
     DataLocationResourceTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
@@ -379,111 +379,131 @@
     ExecutionStatisticsTypeDef,
     ExtendTransactionRequestRequestTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
-    GetLFTagResponseTypeDef,
     GetQueryStateRequestRequestTypeDef,
-    GetQueryStateResponseTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
-    GetTableObjectsRequestRequestTypeDef,
+    TimestampTypeDef,
     PartitionValueListTypeDef,
-    GetTemporaryGluePartitionCredentialsResponseTypeDef,
-    GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
-    GetWorkUnitResultsResponseTypeDef,
-    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
+    LFTagKeyResourceOutputTypeDef,
     LFTagKeyResourceTypeDef,
+    LFTagOutputTypeDef,
+    LFTagPairTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
-    ListLFTagsRequestListLFTagsPaginateTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     TableObjectTypeDef,
-    QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartQueryPlanningResponseTypeDef,
+    TableResourceOutputTypeDef,
     StartTransactionRequestRequestTypeDef,
-    StartTransactionResponseTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
+    AssumeDecoratedRoleWithSAMLResponseTypeDef,
+    CommitTransactionResponseTypeDef,
+    GetLFTagResponseTypeDef,
+    GetQueryStateResponseTypeDef,
+    GetTemporaryGluePartitionCredentialsResponseTypeDef,
+    GetTemporaryGlueTableCredentialsResponseTypeDef,
+    GetWorkUnitResultsResponseTypeDef,
+    StartQueryPlanningResponseTypeDef,
+    StartTransactionResponseTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
-    ColumnLFTagTypeDef,
-    ListLFTagsResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
-    LFTagErrorTypeDef,
+    PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
+    ColumnLFTagTypeDef,
+    LFTagErrorTypeDef,
+    ListLFTagsResponseTypeDef,
+    TableWithColumnsResourceOutputTypeDef,
     TableWithColumnsResourceTypeDef,
+    DataCellsFilterOutputTypeDef,
     DataCellsFilterTypeDef,
     TaggedDatabaseTypeDef,
     WriteOperationTypeDef,
     DeleteObjectsOnCancelRequestRequestTypeDef,
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
+    GetTableObjectsRequestRequestTypeDef,
+    QueryPlanningContextTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
+    LFTagPolicyResourceOutputTypeDef,
+    LFTagPairUnionTypeDef,
     LFTagPolicyResourceTypeDef,
-    SearchDatabasesByLFTagsRequestRequestTypeDef,
-    SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-    SearchTablesByLFTagsRequestRequestTypeDef,
-    SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+    LFTagUnionTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
     ListDataCellsFilterRequestRequestTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     PartitionObjectsTypeDef,
-    StartQueryPlanningRequestRequestTypeDef,
+    TableResourceUnionTypeDef,
+    DataLakeSettingsOutputTypeDef,
+    DataLakeSettingsTypeDef,
     GetResourceLFTagsResponseTypeDef,
     TaggedTableTypeDef,
     AddLFTagsToResourceResponseTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    DataLakeSettingsTypeDef,
-    CreateDataCellsFilterRequestRequestTypeDef,
     GetDataCellsFilterResponseTypeDef,
     ListDataCellsFilterResponseTypeDef,
+    CreateDataCellsFilterRequestRequestTypeDef,
+    DataCellsFilterUnionTypeDef,
     UpdateDataCellsFilterRequestRequestTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     UpdateTableObjectsRequestRequestTypeDef,
+    StartQueryPlanningRequestRequestTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
+    SearchDatabasesByLFTagsRequestRequestTypeDef,
+    SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+    SearchTablesByLFTagsRequestRequestTypeDef,
+    SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     GetTableObjectsResponseTypeDef,
-    SearchTablesByLFTagsResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
+    DataLakeSettingsUnionTypeDef,
     PutDataLakeSettingsRequestRequestTypeDef,
+    SearchTablesByLFTagsResponseTypeDef,
+    BatchPermissionsRequestEntryOutputTypeDef,
+    PrincipalResourcePermissionsTypeDef,
     AddLFTagsToResourceRequestRequestTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     GetResourceLFTagsRequestRequestTypeDef,
     GrantPermissionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
-    PrincipalResourcePermissionsTypeDef,
     RemoveLFTagsFromResourceRequestRequestTypeDef,
+    ResourceUnionTypeDef,
     RevokePermissionsRequestRequestTypeDef,
-    BatchGrantPermissionsRequestRequestTypeDef,
     BatchPermissionsFailureEntryTypeDef,
-    BatchRevokePermissionsRequestRequestTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     ListPermissionsResponseTypeDef,
+    BatchPermissionsRequestEntryUnionTypeDef,
     BatchGrantPermissionsResponseTypeDef,
     BatchRevokePermissionsResponseTypeDef,
+    BatchGrantPermissionsRequestRequestTypeDef,
+    BatchRevokePermissionsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> LFTagPairTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lakeformation-2.5.2/README.md` & `types-aiobotocore-lakeformation-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-lakeformation"></a>
 
 # types-aiobotocore-lakeformation
 
 [![PyPI - types-aiobotocore-lakeformation](https://img.shields.io/pypi/v/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lakeformation?color=blue)](https://pypistats.org/packages/types-aiobotocore-lakeformation)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lakeformation)](https://pepy.tech/project/types-aiobotocore-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LakeFormation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
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
 [types-aiobotocore-lakeformation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/).
 
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
@@ -304,35 +304,36 @@
 )
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lakeformation.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lakeformation.type_defs import (
-    LFTagPairTypeDef,
+    ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
-    AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
+    LFTagPairOutputTypeDef,
+    ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
-    CommitTransactionResponseTypeDef,
     CreateLFTagRequestRequestTypeDef,
+    RowFilterOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
     DataLocationResourceTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
@@ -346,111 +347,131 @@
     ExecutionStatisticsTypeDef,
     ExtendTransactionRequestRequestTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
-    GetLFTagResponseTypeDef,
     GetQueryStateRequestRequestTypeDef,
-    GetQueryStateResponseTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
-    GetTableObjectsRequestRequestTypeDef,
+    TimestampTypeDef,
     PartitionValueListTypeDef,
-    GetTemporaryGluePartitionCredentialsResponseTypeDef,
-    GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
-    GetWorkUnitResultsResponseTypeDef,
-    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
+    LFTagKeyResourceOutputTypeDef,
     LFTagKeyResourceTypeDef,
+    LFTagOutputTypeDef,
+    LFTagPairTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
-    ListLFTagsRequestListLFTagsPaginateTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     TableObjectTypeDef,
-    QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartQueryPlanningResponseTypeDef,
+    TableResourceOutputTypeDef,
     StartTransactionRequestRequestTypeDef,
-    StartTransactionResponseTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
+    AssumeDecoratedRoleWithSAMLResponseTypeDef,
+    CommitTransactionResponseTypeDef,
+    GetLFTagResponseTypeDef,
+    GetQueryStateResponseTypeDef,
+    GetTemporaryGluePartitionCredentialsResponseTypeDef,
+    GetTemporaryGlueTableCredentialsResponseTypeDef,
+    GetWorkUnitResultsResponseTypeDef,
+    StartQueryPlanningResponseTypeDef,
+    StartTransactionResponseTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
-    ColumnLFTagTypeDef,
-    ListLFTagsResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
-    LFTagErrorTypeDef,
+    PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
+    ColumnLFTagTypeDef,
+    LFTagErrorTypeDef,
+    ListLFTagsResponseTypeDef,
+    TableWithColumnsResourceOutputTypeDef,
     TableWithColumnsResourceTypeDef,
+    DataCellsFilterOutputTypeDef,
     DataCellsFilterTypeDef,
     TaggedDatabaseTypeDef,
     WriteOperationTypeDef,
     DeleteObjectsOnCancelRequestRequestTypeDef,
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
+    GetTableObjectsRequestRequestTypeDef,
+    QueryPlanningContextTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
+    LFTagPolicyResourceOutputTypeDef,
+    LFTagPairUnionTypeDef,
     LFTagPolicyResourceTypeDef,
-    SearchDatabasesByLFTagsRequestRequestTypeDef,
-    SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-    SearchTablesByLFTagsRequestRequestTypeDef,
-    SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+    LFTagUnionTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
     ListDataCellsFilterRequestRequestTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     PartitionObjectsTypeDef,
-    StartQueryPlanningRequestRequestTypeDef,
+    TableResourceUnionTypeDef,
+    DataLakeSettingsOutputTypeDef,
+    DataLakeSettingsTypeDef,
     GetResourceLFTagsResponseTypeDef,
     TaggedTableTypeDef,
     AddLFTagsToResourceResponseTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    DataLakeSettingsTypeDef,
-    CreateDataCellsFilterRequestRequestTypeDef,
     GetDataCellsFilterResponseTypeDef,
     ListDataCellsFilterResponseTypeDef,
+    CreateDataCellsFilterRequestRequestTypeDef,
+    DataCellsFilterUnionTypeDef,
     UpdateDataCellsFilterRequestRequestTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     UpdateTableObjectsRequestRequestTypeDef,
+    StartQueryPlanningRequestRequestTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
+    SearchDatabasesByLFTagsRequestRequestTypeDef,
+    SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+    SearchTablesByLFTagsRequestRequestTypeDef,
+    SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     GetTableObjectsResponseTypeDef,
-    SearchTablesByLFTagsResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
+    DataLakeSettingsUnionTypeDef,
     PutDataLakeSettingsRequestRequestTypeDef,
+    SearchTablesByLFTagsResponseTypeDef,
+    BatchPermissionsRequestEntryOutputTypeDef,
+    PrincipalResourcePermissionsTypeDef,
     AddLFTagsToResourceRequestRequestTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     GetResourceLFTagsRequestRequestTypeDef,
     GrantPermissionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
-    PrincipalResourcePermissionsTypeDef,
     RemoveLFTagsFromResourceRequestRequestTypeDef,
+    ResourceUnionTypeDef,
     RevokePermissionsRequestRequestTypeDef,
-    BatchGrantPermissionsRequestRequestTypeDef,
     BatchPermissionsFailureEntryTypeDef,
-    BatchRevokePermissionsRequestRequestTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     ListPermissionsResponseTypeDef,
+    BatchPermissionsRequestEntryUnionTypeDef,
     BatchGrantPermissionsResponseTypeDef,
     BatchRevokePermissionsResponseTypeDef,
+    BatchGrantPermissionsRequestRequestTypeDef,
+    BatchRevokePermissionsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> LFTagPairTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lakeformation-2.5.2/setup.py` & `types-aiobotocore-lakeformation-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lakeformation",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_lakeformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LakeFormation 2.5.2 service generated with"
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
-    keywords="aiobotocore lakeformation type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore lakeformation type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lakeformation": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/"
```

### Comparing `types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/__init__.py` & `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/__init__.pyi` & `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/client.py` & `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("lakeformation") as client:
         client: LakeFormationClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     DataLakeResourceTypeType,
     OptimizerTypeType,
@@ -38,20 +37,20 @@
     SearchTablesByLFTagsPaginator,
 )
 from .type_defs import (
     AddLFTagsToResourceResponseTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     BatchGrantPermissionsResponseTypeDef,
-    BatchPermissionsRequestEntryTypeDef,
+    BatchPermissionsRequestEntryUnionTypeDef,
     BatchRevokePermissionsResponseTypeDef,
     CommitTransactionResponseTypeDef,
-    DataCellsFilterTypeDef,
+    DataCellsFilterUnionTypeDef,
     DataLakePrincipalTypeDef,
-    DataLakeSettingsTypeDef,
+    DataLakeSettingsUnionTypeDef,
     DescribeResourceResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     GetLFTagResponseTypeDef,
@@ -59,31 +58,32 @@
     GetQueryStatisticsResponseTypeDef,
     GetResourceLFTagsResponseTypeDef,
     GetTableObjectsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsResponseTypeDef,
     GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsResponseTypeDef,
     GetWorkUnitsResponseTypeDef,
-    LFTagPairTypeDef,
-    LFTagTypeDef,
+    LFTagPairUnionTypeDef,
+    LFTagUnionTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     ListTransactionsResponseTypeDef,
     PartitionValueListTypeDef,
     QueryPlanningContextTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    ResourceTypeDef,
+    ResourceUnionTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
     StartQueryPlanningResponseTypeDef,
     StartTransactionResponseTypeDef,
-    TableResourceTypeDef,
+    TableResourceUnionTypeDef,
+    TimestampTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     VirtualObjectTypeDef,
     WriteOperationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -138,15 +138,19 @@
         LakeFormationClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#exceptions)
         """
 
     async def add_lf_tags_to_resource(
-        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
+        self,
+        *,
+        Resource: ResourceUnionTypeDef,
+        LFTags: Sequence[LFTagPairUnionTypeDef],
+        CatalogId: str = ...
     ) -> AddLFTagsToResourceResponseTypeDef:
         """
         Attaches one or more LF-tags to an existing resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.add_lf_tags_to_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#add_lf_tags_to_resource)
         """
@@ -159,25 +163,25 @@
         the SAML assertion included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.assume_decorated_role_with_saml)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#assume_decorated_role_with_saml)
         """
 
     async def batch_grant_permissions(
-        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef], CatalogId: str = ...
     ) -> BatchGrantPermissionsResponseTypeDef:
         """
         Batch operation to grant permissions to the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_grant_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#batch_grant_permissions)
         """
 
     async def batch_revoke_permissions(
-        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef], CatalogId: str = ...
     ) -> BatchRevokePermissionsResponseTypeDef:
         """
         Batch operation to revoke permissions from the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_revoke_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#batch_revoke_permissions)
         """
@@ -211,15 +215,15 @@
         Attempts to commit the specified transaction.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.commit_transaction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#commit_transaction)
         """
 
     async def create_data_cells_filter(
-        self, *, TableData: DataCellsFilterTypeDef
+        self, *, TableData: DataCellsFilterUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a data cell filter to allow one to grant access to certain columns on
         certain rows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#create_data_cells_filter)
@@ -379,15 +383,19 @@
         Retrieves statistics on the planning and execution of a query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_query_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_query_statistics)
         """
 
     async def get_resource_lf_tags(
-        self, *, Resource: ResourceTypeDef, CatalogId: str = ..., ShowAssignedLFTags: bool = ...
+        self,
+        *,
+        Resource: ResourceUnionTypeDef,
+        CatalogId: str = ...,
+        ShowAssignedLFTags: bool = ...
     ) -> GetResourceLFTagsResponseTypeDef:
         """
         Returns the LF-tags applied to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_resource_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_resource_lf_tags)
         """
@@ -395,15 +403,15 @@
     async def get_table_objects(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         TransactionId: str = ...,
-        QueryAsOfTime: Union[datetime, str] = ...,
+        QueryAsOfTime: TimestampTypeDef = ...,
         PartitionPredicate: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> GetTableObjectsResponseTypeDef:
         """
         Returns the set of Amazon S3 objects that make up the specified governed table.
 
@@ -466,29 +474,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_work_units)
         """
 
     async def grant_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: ResourceTypeDef,
+        Resource: ResourceUnionTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Grants permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.grant_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#grant_permissions)
         """
 
     async def list_data_cells_filter(
-        self, *, Table: TableResourceTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
+        self, *, Table: TableResourceUnionTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataCellsFilterResponseTypeDef:
         """
         Lists all the data cell filters on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_data_cells_filter)
         """
@@ -510,15 +518,15 @@
 
     async def list_permissions(
         self,
         *,
         CatalogId: str = ...,
         Principal: DataLakePrincipalTypeDef = ...,
         ResourceType: DataLakeResourceTypeType = ...,
-        Resource: ResourceTypeDef = ...,
+        Resource: ResourceUnionTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncludeRelated: str = ...
     ) -> ListPermissionsResponseTypeDef:
         """
         Returns a list of the principal permissions on the resource, filtered by the
         permissions of the caller.
@@ -571,15 +579,15 @@
         Returns metadata about transactions and their status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_transactions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_transactions)
         """
 
     async def put_data_lake_settings(
-        self, *, DataLakeSettings: DataLakeSettingsTypeDef, CatalogId: str = ...
+        self, *, DataLakeSettings: DataLakeSettingsUnionTypeDef, CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Sets the list of data lake administrators who have admin privileges on all
         resources managed by Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.put_data_lake_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#put_data_lake_settings)
@@ -597,28 +605,32 @@
         Registers the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.register_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#register_resource)
         """
 
     async def remove_lf_tags_from_resource(
-        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
+        self,
+        *,
+        Resource: ResourceUnionTypeDef,
+        LFTags: Sequence[LFTagPairUnionTypeDef],
+        CatalogId: str = ...
     ) -> RemoveLFTagsFromResourceResponseTypeDef:
         """
         Removes an LF-tag from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.remove_lf_tags_from_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#remove_lf_tags_from_resource)
         """
 
     async def revoke_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: ResourceTypeDef,
+        Resource: ResourceUnionTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Revokes permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
@@ -626,30 +638,30 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.revoke_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#revoke_permissions)
         """
 
     async def search_databases_by_lf_tags(
         self,
         *,
-        Expression: Sequence[LFTagTypeDef],
+        Expression: Sequence[LFTagUnionTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchDatabasesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `DATABASE` resources by `TagCondition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_databases_by_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#search_databases_by_lf_tags)
         """
 
     async def search_tables_by_lf_tags(
         self,
         *,
-        Expression: Sequence[LFTagTypeDef],
+        Expression: Sequence[LFTagUnionTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchTablesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `TABLE` resources by `LFTag`s.
 
@@ -674,15 +686,15 @@
         Starts a new transaction and returns its transaction ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.start_transaction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#start_transaction)
         """
 
     async def update_data_cells_filter(
-        self, *, TableData: DataCellsFilterTypeDef
+        self, *, TableData: DataCellsFilterUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates a data cell filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#update_data_cells_filter)
         """
```

### Comparing `types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/client.pyi` & `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("lakeformation") as client:
         client: LakeFormationClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     DataLakeResourceTypeType,
     OptimizerTypeType,
@@ -38,20 +37,20 @@
     SearchTablesByLFTagsPaginator,
 )
 from .type_defs import (
     AddLFTagsToResourceResponseTypeDef,
     AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     BatchGrantPermissionsResponseTypeDef,
-    BatchPermissionsRequestEntryTypeDef,
+    BatchPermissionsRequestEntryUnionTypeDef,
     BatchRevokePermissionsResponseTypeDef,
     CommitTransactionResponseTypeDef,
-    DataCellsFilterTypeDef,
+    DataCellsFilterUnionTypeDef,
     DataLakePrincipalTypeDef,
-    DataLakeSettingsTypeDef,
+    DataLakeSettingsUnionTypeDef,
     DescribeResourceResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     GetLFTagResponseTypeDef,
@@ -59,31 +58,32 @@
     GetQueryStatisticsResponseTypeDef,
     GetResourceLFTagsResponseTypeDef,
     GetTableObjectsResponseTypeDef,
     GetTemporaryGluePartitionCredentialsResponseTypeDef,
     GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsResponseTypeDef,
     GetWorkUnitsResponseTypeDef,
-    LFTagPairTypeDef,
-    LFTagTypeDef,
+    LFTagPairUnionTypeDef,
+    LFTagUnionTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     ListPermissionsResponseTypeDef,
     ListResourcesResponseTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     ListTransactionsResponseTypeDef,
     PartitionValueListTypeDef,
     QueryPlanningContextTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    ResourceTypeDef,
+    ResourceUnionTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
     StartQueryPlanningResponseTypeDef,
     StartTransactionResponseTypeDef,
-    TableResourceTypeDef,
+    TableResourceUnionTypeDef,
+    TimestampTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
     VirtualObjectTypeDef,
     WriteOperationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -133,15 +133,19 @@
         """
         LakeFormationClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#exceptions)
         """
     async def add_lf_tags_to_resource(
-        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
+        self,
+        *,
+        Resource: ResourceUnionTypeDef,
+        LFTags: Sequence[LFTagPairUnionTypeDef],
+        CatalogId: str = ...
     ) -> AddLFTagsToResourceResponseTypeDef:
         """
         Attaches one or more LF-tags to an existing resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.add_lf_tags_to_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#add_lf_tags_to_resource)
         """
@@ -152,24 +156,24 @@
         Allows a caller to assume an IAM role decorated as the SAML user specified in
         the SAML assertion included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.assume_decorated_role_with_saml)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#assume_decorated_role_with_saml)
         """
     async def batch_grant_permissions(
-        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef], CatalogId: str = ...
     ) -> BatchGrantPermissionsResponseTypeDef:
         """
         Batch operation to grant permissions to the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_grant_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#batch_grant_permissions)
         """
     async def batch_revoke_permissions(
-        self, *, Entries: Sequence[BatchPermissionsRequestEntryTypeDef], CatalogId: str = ...
+        self, *, Entries: Sequence[BatchPermissionsRequestEntryUnionTypeDef], CatalogId: str = ...
     ) -> BatchRevokePermissionsResponseTypeDef:
         """
         Batch operation to revoke permissions from the principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.batch_revoke_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#batch_revoke_permissions)
         """
@@ -198,15 +202,15 @@
         """
         Attempts to commit the specified transaction.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.commit_transaction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#commit_transaction)
         """
     async def create_data_cells_filter(
-        self, *, TableData: DataCellsFilterTypeDef
+        self, *, TableData: DataCellsFilterUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a data cell filter to allow one to grant access to certain columns on
         certain rows.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.create_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#create_data_cells_filter)
@@ -350,30 +354,34 @@
         """
         Retrieves statistics on the planning and execution of a query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_query_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_query_statistics)
         """
     async def get_resource_lf_tags(
-        self, *, Resource: ResourceTypeDef, CatalogId: str = ..., ShowAssignedLFTags: bool = ...
+        self,
+        *,
+        Resource: ResourceUnionTypeDef,
+        CatalogId: str = ...,
+        ShowAssignedLFTags: bool = ...
     ) -> GetResourceLFTagsResponseTypeDef:
         """
         Returns the LF-tags applied to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_resource_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_resource_lf_tags)
         """
     async def get_table_objects(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         CatalogId: str = ...,
         TransactionId: str = ...,
-        QueryAsOfTime: Union[datetime, str] = ...,
+        QueryAsOfTime: TimestampTypeDef = ...,
         PartitionPredicate: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> GetTableObjectsResponseTypeDef:
         """
         Returns the set of Amazon S3 objects that make up the specified governed table.
 
@@ -431,28 +439,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.get_work_units)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#get_work_units)
         """
     async def grant_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: ResourceTypeDef,
+        Resource: ResourceUnionTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Grants permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.grant_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#grant_permissions)
         """
     async def list_data_cells_filter(
-        self, *, Table: TableResourceTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
+        self, *, Table: TableResourceUnionTypeDef = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListDataCellsFilterResponseTypeDef:
         """
         Lists all the data cell filters on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_data_cells_filter)
         """
@@ -472,15 +480,15 @@
         """
     async def list_permissions(
         self,
         *,
         CatalogId: str = ...,
         Principal: DataLakePrincipalTypeDef = ...,
         ResourceType: DataLakeResourceTypeType = ...,
-        Resource: ResourceTypeDef = ...,
+        Resource: ResourceUnionTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         IncludeRelated: str = ...
     ) -> ListPermissionsResponseTypeDef:
         """
         Returns a list of the principal permissions on the resource, filtered by the
         permissions of the caller.
@@ -529,15 +537,15 @@
         """
         Returns metadata about transactions and their status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.list_transactions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#list_transactions)
         """
     async def put_data_lake_settings(
-        self, *, DataLakeSettings: DataLakeSettingsTypeDef, CatalogId: str = ...
+        self, *, DataLakeSettings: DataLakeSettingsUnionTypeDef, CatalogId: str = ...
     ) -> Dict[str, Any]:
         """
         Sets the list of data lake administrators who have admin privileges on all
         resources managed by Lake Formation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.put_data_lake_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#put_data_lake_settings)
@@ -553,56 +561,60 @@
         """
         Registers the resource as managed by the Data Catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.register_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#register_resource)
         """
     async def remove_lf_tags_from_resource(
-        self, *, Resource: ResourceTypeDef, LFTags: Sequence[LFTagPairTypeDef], CatalogId: str = ...
+        self,
+        *,
+        Resource: ResourceUnionTypeDef,
+        LFTags: Sequence[LFTagPairUnionTypeDef],
+        CatalogId: str = ...
     ) -> RemoveLFTagsFromResourceResponseTypeDef:
         """
         Removes an LF-tag from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.remove_lf_tags_from_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#remove_lf_tags_from_resource)
         """
     async def revoke_permissions(
         self,
         *,
         Principal: DataLakePrincipalTypeDef,
-        Resource: ResourceTypeDef,
+        Resource: ResourceUnionTypeDef,
         Permissions: Sequence[PermissionType],
         CatalogId: str = ...,
         PermissionsWithGrantOption: Sequence[PermissionType] = ...
     ) -> Dict[str, Any]:
         """
         Revokes permissions to the principal to access metadata in the Data Catalog and
         data organized in underlying data storage such as Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.revoke_permissions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#revoke_permissions)
         """
     async def search_databases_by_lf_tags(
         self,
         *,
-        Expression: Sequence[LFTagTypeDef],
+        Expression: Sequence[LFTagUnionTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchDatabasesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `DATABASE` resources by `TagCondition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.search_databases_by_lf_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#search_databases_by_lf_tags)
         """
     async def search_tables_by_lf_tags(
         self,
         *,
-        Expression: Sequence[LFTagTypeDef],
+        Expression: Sequence[LFTagUnionTypeDef],
         NextToken: str = ...,
         MaxResults: int = ...,
         CatalogId: str = ...
     ) -> SearchTablesByLFTagsResponseTypeDef:
         """
         This operation allows a search on `TABLE` resources by `LFTag`s.
 
@@ -624,15 +636,15 @@
         """
         Starts a new transaction and returns its transaction ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.start_transaction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#start_transaction)
         """
     async def update_data_cells_filter(
-        self, *, TableData: DataCellsFilterTypeDef
+        self, *, TableData: DataCellsFilterUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates a data cell filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Client.update_data_cells_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/client/#update_data_cells_filter)
         """
```

### Comparing `types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/literals.py` & `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/literals.pyi` & `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/paginator.py` & `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,21 @@
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import ResourceShareTypeType
 from .type_defs import (
     GetWorkUnitsResponseTypeDef,
-    LFTagTypeDef,
+    LFTagUnionTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     PaginatorConfigTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
-    TableResourceTypeDef,
+    TableResourceUnionTypeDef,
 )
 
 __all__ = (
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
@@ -67,30 +67,33 @@
 class GetWorkUnitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#getworkunitspaginator)
     """
 
     def paginate(
-        self, *, QueryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetWorkUnitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#getworkunitspaginator)
         """
 
 
 class ListDataCellsFilterPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self,
+        *,
+        Table: TableResourceUnionTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
 
@@ -101,15 +104,15 @@
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#listlftagspaginator)
         """
 
 
@@ -118,17 +121,17 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[LFTagTypeDef],
+        Expression: Sequence[LFTagUnionTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
 
 
@@ -137,15 +140,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[LFTagTypeDef],
+        Expression: Sequence[LFTagUnionTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/paginator.pyi` & `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -32,21 +32,21 @@
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import ResourceShareTypeType
 from .type_defs import (
     GetWorkUnitsResponseTypeDef,
-    LFTagTypeDef,
+    LFTagUnionTypeDef,
     ListDataCellsFilterResponseTypeDef,
     ListLFTagsResponseTypeDef,
     PaginatorConfigTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     SearchTablesByLFTagsResponseTypeDef,
-    TableResourceTypeDef,
+    TableResourceUnionTypeDef,
 )
 
 __all__ = (
     "GetWorkUnitsPaginator",
     "ListDataCellsFilterPaginator",
     "ListLFTagsPaginator",
     "SearchDatabasesByLFTagsPaginator",
@@ -64,29 +64,32 @@
 class GetWorkUnitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#getworkunitspaginator)
     """
 
     def paginate(
-        self, *, QueryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetWorkUnitsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#getworkunitspaginator)
         """
 
 class ListDataCellsFilterPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#listdatacellsfilterpaginator)
     """
 
     def paginate(
-        self, *, Table: TableResourceTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self,
+        *,
+        Table: TableResourceUnionTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataCellsFilterResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#listdatacellsfilterpaginator)
         """
 
 class ListLFTagsPaginator(AioPaginator):
@@ -96,15 +99,15 @@
     """
 
     def paginate(
         self,
         *,
         CatalogId: str = ...,
         ResourceShareType: ResourceShareTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#listlftagspaginator)
         """
 
 class SearchDatabasesByLFTagsPaginator(AioPaginator):
@@ -112,17 +115,17 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchdatabasesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[LFTagTypeDef],
+        Expression: Sequence[LFTagUnionTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchDatabasesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchdatabasesbylftagspaginator)
         """
 
 class SearchTablesByLFTagsPaginator(AioPaginator):
@@ -130,15 +133,15 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchtablesbylftagspaginator)
     """
 
     def paginate(
         self,
         *,
-        Expression: Sequence[LFTagTypeDef],
+        Expression: Sequence[LFTagUnionTypeDef],
         CatalogId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchTablesByLFTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/paginators/#searchtablesbylftagspaginator)
         """
```

### Comparing `types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/type_defs.py` & `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lakeformation service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_lakeformation.type_defs import LFTagPairTypeDef
+    from types_aiobotocore_lakeformation.type_defs import ResponseMetadataTypeDef
 
-    data: LFTagPairTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -35,26 +35,27 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "LFTagPairTypeDef",
+    "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
+    "LFTagPairOutputTypeDef",
+    "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
-    "CommitTransactionResponseTypeDef",
     "CreateLFTagRequestRequestTypeDef",
+    "RowFilterOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
     "DataLocationResourceTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
     "DeleteObjectInputTypeDef",
@@ -68,129 +69,140 @@
     "ExecutionStatisticsTypeDef",
     "ExtendTransactionRequestRequestTypeDef",
     "FilterConditionTypeDef",
     "GetDataCellsFilterRequestRequestTypeDef",
     "GetDataLakeSettingsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathRequestRequestTypeDef",
     "GetLFTagRequestRequestTypeDef",
-    "GetLFTagResponseTypeDef",
     "GetQueryStateRequestRequestTypeDef",
-    "GetQueryStateResponseTypeDef",
     "GetQueryStatisticsRequestRequestTypeDef",
     "PlanningStatisticsTypeDef",
-    "GetTableObjectsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "PartitionValueListTypeDef",
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
     "GetWorkUnitResultsRequestRequestTypeDef",
-    "GetWorkUnitResultsResponseTypeDef",
-    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetWorkUnitsRequestRequestTypeDef",
     "WorkUnitRangeTypeDef",
+    "LFTagKeyResourceOutputTypeDef",
     "LFTagKeyResourceTypeDef",
+    "LFTagOutputTypeDef",
+    "LFTagPairTypeDef",
     "LFTagTypeDef",
     "TableResourceTypeDef",
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "ListLFTagsRequestRequestTypeDef",
     "ListTableStorageOptimizersRequestRequestTypeDef",
     "StorageOptimizerTypeDef",
     "ListTransactionsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "TableObjectTypeDef",
-    "QueryPlanningContextTypeDef",
     "RegisterResourceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartQueryPlanningResponseTypeDef",
+    "TableResourceOutputTypeDef",
     "StartTransactionRequestRequestTypeDef",
-    "StartTransactionResponseTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
+    "CommitTransactionResponseTypeDef",
+    "GetLFTagResponseTypeDef",
+    "GetQueryStateResponseTypeDef",
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    "GetWorkUnitResultsResponseTypeDef",
+    "StartQueryPlanningResponseTypeDef",
+    "StartTransactionResponseTypeDef",
     "UpdateTableStorageOptimizerResponseTypeDef",
-    "ColumnLFTagTypeDef",
-    "ListLFTagsResponseTypeDef",
     "GetTemporaryGlueTableCredentialsRequestRequestTypeDef",
-    "LFTagErrorTypeDef",
+    "PrincipalPermissionsOutputTypeDef",
     "PrincipalPermissionsTypeDef",
+    "ColumnLFTagTypeDef",
+    "LFTagErrorTypeDef",
+    "ListLFTagsResponseTypeDef",
+    "TableWithColumnsResourceOutputTypeDef",
     "TableWithColumnsResourceTypeDef",
+    "DataCellsFilterOutputTypeDef",
     "DataCellsFilterTypeDef",
     "TaggedDatabaseTypeDef",
     "WriteOperationTypeDef",
     "DeleteObjectsOnCancelRequestRequestTypeDef",
     "DescribeResourceResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "DescribeTransactionResponseTypeDef",
     "ListTransactionsResponseTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "GetQueryStatisticsResponseTypeDef",
+    "GetTableObjectsRequestRequestTypeDef",
+    "QueryPlanningContextTypeDef",
     "GetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
+    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "GetWorkUnitsResponseTypeDef",
+    "LFTagPolicyResourceOutputTypeDef",
+    "LFTagPairUnionTypeDef",
     "LFTagPolicyResourceTypeDef",
-    "SearchDatabasesByLFTagsRequestRequestTypeDef",
-    "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    "SearchTablesByLFTagsRequestRequestTypeDef",
-    "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    "LFTagUnionTypeDef",
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     "ListDataCellsFilterRequestRequestTypeDef",
     "ListTableStorageOptimizersResponseTypeDef",
     "PartitionObjectsTypeDef",
-    "StartQueryPlanningRequestRequestTypeDef",
+    "TableResourceUnionTypeDef",
+    "DataLakeSettingsOutputTypeDef",
+    "DataLakeSettingsTypeDef",
     "GetResourceLFTagsResponseTypeDef",
     "TaggedTableTypeDef",
     "AddLFTagsToResourceResponseTypeDef",
     "RemoveLFTagsFromResourceResponseTypeDef",
-    "DataLakeSettingsTypeDef",
-    "CreateDataCellsFilterRequestRequestTypeDef",
     "GetDataCellsFilterResponseTypeDef",
     "ListDataCellsFilterResponseTypeDef",
+    "CreateDataCellsFilterRequestRequestTypeDef",
+    "DataCellsFilterUnionTypeDef",
     "UpdateDataCellsFilterRequestRequestTypeDef",
     "SearchDatabasesByLFTagsResponseTypeDef",
     "UpdateTableObjectsRequestRequestTypeDef",
+    "StartQueryPlanningRequestRequestTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
+    "SearchDatabasesByLFTagsRequestRequestTypeDef",
+    "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    "SearchTablesByLFTagsRequestRequestTypeDef",
+    "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "GetTableObjectsResponseTypeDef",
-    "SearchTablesByLFTagsResponseTypeDef",
     "GetDataLakeSettingsResponseTypeDef",
+    "DataLakeSettingsUnionTypeDef",
     "PutDataLakeSettingsRequestRequestTypeDef",
+    "SearchTablesByLFTagsResponseTypeDef",
+    "BatchPermissionsRequestEntryOutputTypeDef",
+    "PrincipalResourcePermissionsTypeDef",
     "AddLFTagsToResourceRequestRequestTypeDef",
     "BatchPermissionsRequestEntryTypeDef",
     "GetResourceLFTagsRequestRequestTypeDef",
     "GrantPermissionsRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
-    "PrincipalResourcePermissionsTypeDef",
     "RemoveLFTagsFromResourceRequestRequestTypeDef",
+    "ResourceUnionTypeDef",
     "RevokePermissionsRequestRequestTypeDef",
-    "BatchGrantPermissionsRequestRequestTypeDef",
     "BatchPermissionsFailureEntryTypeDef",
-    "BatchRevokePermissionsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathResponseTypeDef",
     "ListPermissionsResponseTypeDef",
+    "BatchPermissionsRequestEntryUnionTypeDef",
     "BatchGrantPermissionsResponseTypeDef",
     "BatchRevokePermissionsResponseTypeDef",
+    "BatchGrantPermissionsRequestRequestTypeDef",
+    "BatchRevokePermissionsRequestRequestTypeDef",
 )
 
-_RequiredLFTagPairTypeDef = TypedDict(
-    "_RequiredLFTagPairTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": Sequence[str],
-    },
-)
-_OptionalLFTagPairTypeDef = TypedDict(
-    "_OptionalLFTagPairTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CatalogId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
-    pass
-
-
 _RequiredAddObjectInputTypeDef = TypedDict(
     "_RequiredAddObjectInputTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
@@ -228,25 +240,14 @@
 class AssumeDecoratedRoleWithSAMLRequestRequestTypeDef(
     _RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     _OptionalAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
 ):
     pass
 
 
-AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
     },
     total=False,
 )
@@ -271,14 +272,42 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
+_RequiredLFTagPairOutputTypeDef = TypedDict(
+    "_RequiredLFTagPairOutputTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+_OptionalLFTagPairOutputTypeDef = TypedDict(
+    "_OptionalLFTagPairOutputTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class LFTagPairOutputTypeDef(_RequiredLFTagPairOutputTypeDef, _OptionalLFTagPairOutputTypeDef):
+    pass
+
+
+ColumnWildcardOutputTypeDef = TypedDict(
+    "ColumnWildcardOutputTypeDef",
+    {
+        "ExcludedColumnNames": List[str],
+    },
+    total=False,
+)
+
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
     total=False,
 )
@@ -286,22 +315,14 @@
 CommitTransactionRequestRequestTypeDef = TypedDict(
     "CommitTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-CommitTransactionResponseTypeDef = TypedDict(
-    "CommitTransactionResponseTypeDef",
-    {
-        "TransactionStatus": TransactionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -316,14 +337,23 @@
 
 class CreateLFTagRequestRequestTypeDef(
     _RequiredCreateLFTagRequestRequestTypeDef, _OptionalCreateLFTagRequestRequestTypeDef
 ):
     pass
 
 
+RowFilterOutputTypeDef = TypedDict(
+    "RowFilterOutputTypeDef",
+    {
+        "FilterExpression": str,
+        "AllRowsWildcard": Dict[str, Any],
+    },
+    total=False,
+)
+
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -591,40 +621,21 @@
 
 class GetLFTagRequestRequestTypeDef(
     _RequiredGetLFTagRequestRequestTypeDef, _OptionalGetLFTagRequestRequestTypeDef
 ):
     pass
 
 
-GetLFTagResponseTypeDef = TypedDict(
-    "GetLFTagResponseTypeDef",
-    {
-        "CatalogId": str,
-        "TagKey": str,
-        "TagValues": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetQueryStateRequestRequestTypeDef = TypedDict(
     "GetQueryStateRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
-GetQueryStateResponseTypeDef = TypedDict(
-    "GetQueryStateResponseTypeDef",
-    {
-        "Error": str,
-        "State": QueryStateStringType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetQueryStatisticsRequestRequestTypeDef = TypedDict(
     "GetQueryStatisticsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
@@ -635,109 +646,41 @@
         "PlanningTimeMillis": int,
         "QueueTimeMillis": int,
         "WorkUnitsGeneratedCount": int,
     },
     total=False,
 )
 
-_RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTableObjectsRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-    },
-)
-_OptionalGetTableObjectsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTableObjectsRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-        "TransactionId": str,
-        "QueryAsOfTime": Union[datetime, str],
-        "PartitionPredicate": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class GetTableObjectsRequestRequestTypeDef(
-    _RequiredGetTableObjectsRequestRequestTypeDef, _OptionalGetTableObjectsRequestRequestTypeDef
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 PartitionValueListTypeDef = TypedDict(
     "PartitionValueListTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
-GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkUnitResultsRequestRequestTypeDef = TypedDict(
     "GetWorkUnitResultsRequestRequestTypeDef",
     {
         "QueryId": str,
         "WorkUnitId": int,
         "WorkUnitToken": str,
     },
 )
 
-GetWorkUnitResultsResponseTypeDef = TypedDict(
-    "GetWorkUnitResultsResponseTypeDef",
-    {
-        "ResultStream": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
-    {
-        "QueryId": str,
-    },
-)
-_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
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
-class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
-    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetWorkUnitsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkUnitsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 _OptionalGetWorkUnitsRequestRequestTypeDef = TypedDict(
@@ -761,14 +704,36 @@
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
+_RequiredLFTagKeyResourceOutputTypeDef = TypedDict(
+    "_RequiredLFTagKeyResourceOutputTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+_OptionalLFTagKeyResourceOutputTypeDef = TypedDict(
+    "_OptionalLFTagKeyResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class LFTagKeyResourceOutputTypeDef(
+    _RequiredLFTagKeyResourceOutputTypeDef, _OptionalLFTagKeyResourceOutputTypeDef
+):
+    pass
+
+
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -781,14 +746,42 @@
 )
 
 
 class LFTagKeyResourceTypeDef(_RequiredLFTagKeyResourceTypeDef, _OptionalLFTagKeyResourceTypeDef):
     pass
 
 
+LFTagOutputTypeDef = TypedDict(
+    "LFTagOutputTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+
+_RequiredLFTagPairTypeDef = TypedDict(
+    "_RequiredLFTagPairTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": Sequence[str],
+    },
+)
+_OptionalLFTagPairTypeDef = TypedDict(
+    "_OptionalLFTagPairTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
+    pass
+
+
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -810,24 +803,14 @@
 )
 
 
 class TableResourceTypeDef(_RequiredTableResourceTypeDef, _OptionalTableResourceTypeDef):
     pass
 
 
-ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "ResourceShareType": ResourceShareTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLFTagsRequestRequestTypeDef = TypedDict(
     "ListLFTagsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "ResourceShareType": ResourceShareTypeType,
         "MaxResults": int,
         "NextToken": str,
@@ -880,58 +863,24 @@
         "StatusFilter": TransactionStatusFilterType,
         "MaxResults": int,
         "NextToken": str,
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
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
     total=False,
 )
 
-_RequiredQueryPlanningContextTypeDef = TypedDict(
-    "_RequiredQueryPlanningContextTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalQueryPlanningContextTypeDef = TypedDict(
-    "_OptionalQueryPlanningContextTypeDef",
-    {
-        "CatalogId": str,
-        "QueryAsOfTime": Union[datetime, str],
-        "QueryParameters": Mapping[str, str],
-        "TransactionId": str,
-    },
-    total=False,
-)
-
-
-class QueryPlanningContextTypeDef(
-    _RequiredQueryPlanningContextTypeDef, _OptionalQueryPlanningContextTypeDef
-):
-    pass
-
-
 _RequiredRegisterResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalRegisterResourceRequestRequestTypeDef = TypedDict(
@@ -947,49 +896,45 @@
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredTableResourceOutputTypeDef = TypedDict(
+    "_RequiredTableResourceOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DatabaseName": str,
     },
 )
-
-StartQueryPlanningResponseTypeDef = TypedDict(
-    "StartQueryPlanningResponseTypeDef",
+_OptionalTableResourceOutputTypeDef = TypedDict(
+    "_OptionalTableResourceOutputTypeDef",
     {
-        "QueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CatalogId": str,
+        "Name": str,
+        "TableWildcard": Dict[str, Any],
     },
+    total=False,
 )
 
+
+class TableResourceOutputTypeDef(
+    _RequiredTableResourceOutputTypeDef, _OptionalTableResourceOutputTypeDef
+):
+    pass
+
+
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
 
-StartTransactionResponseTypeDef = TypedDict(
-    "StartTransactionResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
     },
 )
 _OptionalUpdateLFTagRequestRequestTypeDef = TypedDict(
@@ -1051,37 +996,103 @@
 class UpdateTableStorageOptimizerRequestRequestTypeDef(
     _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef,
     _OptionalUpdateTableStorageOptimizerRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
-    "UpdateTableStorageOptimizerResponseTypeDef",
+AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     {
-        "Result": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ColumnLFTagTypeDef = TypedDict(
-    "ColumnLFTagTypeDef",
+CommitTransactionResponseTypeDef = TypedDict(
+    "CommitTransactionResponseTypeDef",
     {
-        "Name": str,
-        "LFTags": List[LFTagPairTypeDef],
+        "TransactionStatus": TransactionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListLFTagsResponseTypeDef = TypedDict(
-    "ListLFTagsResponseTypeDef",
+GetLFTagResponseTypeDef = TypedDict(
+    "GetLFTagResponseTypeDef",
     {
-        "LFTags": List[LFTagPairTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueryStateResponseTypeDef = TypedDict(
+    "GetQueryStateResponseTypeDef",
+    {
+        "Error": str,
+        "State": QueryStateStringType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkUnitResultsResponseTypeDef = TypedDict(
+    "GetWorkUnitResultsResponseTypeDef",
+    {
+        "ResultStream": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryPlanningResponseTypeDef = TypedDict(
+    "StartQueryPlanningResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartTransactionResponseTypeDef = TypedDict(
+    "StartTransactionResponseTypeDef",
+    {
+        "TransactionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
+    "UpdateTableStorageOptimizerResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
@@ -1102,32 +1113,83 @@
 class GetTemporaryGlueTableCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
 ):
     pass
 
 
-LFTagErrorTypeDef = TypedDict(
-    "LFTagErrorTypeDef",
+PrincipalPermissionsOutputTypeDef = TypedDict(
+    "PrincipalPermissionsOutputTypeDef",
     {
-        "LFTag": LFTagPairTypeDef,
-        "Error": ErrorDetailTypeDef,
+        "Principal": DataLakePrincipalTypeDef,
+        "Permissions": List[PermissionType],
     },
     total=False,
 )
 
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
-        "Permissions": List[PermissionType],
+        "Permissions": Sequence[PermissionType],
     },
     total=False,
 )
 
+ColumnLFTagTypeDef = TypedDict(
+    "ColumnLFTagTypeDef",
+    {
+        "Name": str,
+        "LFTags": List[LFTagPairOutputTypeDef],
+    },
+    total=False,
+)
+
+LFTagErrorTypeDef = TypedDict(
+    "LFTagErrorTypeDef",
+    {
+        "LFTag": LFTagPairOutputTypeDef,
+        "Error": ErrorDetailTypeDef,
+    },
+    total=False,
+)
+
+ListLFTagsResponseTypeDef = TypedDict(
+    "ListLFTagsResponseTypeDef",
+    {
+        "LFTags": List[LFTagPairOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredTableWithColumnsResourceOutputTypeDef = TypedDict(
+    "_RequiredTableWithColumnsResourceOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "Name": str,
+    },
+)
+_OptionalTableWithColumnsResourceOutputTypeDef = TypedDict(
+    "_OptionalTableWithColumnsResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ColumnNames": List[str],
+        "ColumnWildcard": ColumnWildcardOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class TableWithColumnsResourceOutputTypeDef(
+    _RequiredTableWithColumnsResourceOutputTypeDef, _OptionalTableWithColumnsResourceOutputTypeDef
+):
+    pass
+
+
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1144,14 +1206,41 @@
 
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
 
+_RequiredDataCellsFilterOutputTypeDef = TypedDict(
+    "_RequiredDataCellsFilterOutputTypeDef",
+    {
+        "TableCatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Name": str,
+    },
+)
+_OptionalDataCellsFilterOutputTypeDef = TypedDict(
+    "_OptionalDataCellsFilterOutputTypeDef",
+    {
+        "RowFilter": RowFilterOutputTypeDef,
+        "ColumnNames": List[str],
+        "ColumnWildcard": ColumnWildcardOutputTypeDef,
+        "VersionId": str,
+    },
+    total=False,
+)
+
+
+class DataCellsFilterOutputTypeDef(
+    _RequiredDataCellsFilterOutputTypeDef, _OptionalDataCellsFilterOutputTypeDef
+):
+    pass
+
+
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1173,15 +1262,15 @@
     pass
 
 
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
         "Database": DatabaseResourceTypeDef,
-        "LFTags": List[LFTagPairTypeDef],
+        "LFTags": List[LFTagPairOutputTypeDef],
     },
     total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
@@ -1216,41 +1305,41 @@
     pass
 
 
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceInfo": ResourceInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "ResourceInfoList": List[ResourceInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTransactionResponseTypeDef = TypedDict(
     "DescribeTransactionResponseTypeDef",
     {
         "TransactionDescription": TransactionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTransactionsResponseTypeDef = TypedDict(
     "ListTransactionsResponseTypeDef",
     {
         "Transactions": List[TransactionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesRequestRequestTypeDef = TypedDict(
     "ListResourcesRequestRequestTypeDef",
     {
         "FilterConditionList": Sequence[FilterConditionTypeDef],
@@ -1262,175 +1351,188 @@
 
 GetQueryStatisticsResponseTypeDef = TypedDict(
     "GetQueryStatisticsResponseTypeDef",
     {
         "ExecutionStatistics": ExecutionStatisticsTypeDef,
         "PlanningStatistics": PlanningStatisticsTypeDef,
         "QuerySubmissionTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
+_RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTableObjectsRequestRequestTypeDef",
     {
-        "TableArn": str,
-        "Partition": PartitionValueListTypeDef,
-        "SupportedPermissionTypes": Sequence[PermissionTypeType],
+        "DatabaseName": str,
+        "TableName": str,
     },
 )
-_OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
+_OptionalGetTableObjectsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTableObjectsRequestRequestTypeDef",
     {
-        "Permissions": Sequence[PermissionType],
-        "DurationSeconds": int,
-        "AuditContext": AuditContextTypeDef,
+        "CatalogId": str,
+        "TransactionId": str,
+        "QueryAsOfTime": TimestampTypeDef,
+        "PartitionPredicate": str,
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
 
-class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(
-    _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
-    _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+class GetTableObjectsRequestRequestTypeDef(
+    _RequiredGetTableObjectsRequestRequestTypeDef, _OptionalGetTableObjectsRequestRequestTypeDef
 ):
     pass
 
 
-GetWorkUnitsResponseTypeDef = TypedDict(
-    "GetWorkUnitsResponseTypeDef",
-    {
-        "NextToken": str,
-        "QueryId": str,
-        "WorkUnitRanges": List[WorkUnitRangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredLFTagPolicyResourceTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceTypeDef",
+_RequiredQueryPlanningContextTypeDef = TypedDict(
+    "_RequiredQueryPlanningContextTypeDef",
     {
-        "ResourceType": ResourceTypeType,
-        "Expression": Sequence[LFTagTypeDef],
+        "DatabaseName": str,
     },
 )
-_OptionalLFTagPolicyResourceTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceTypeDef",
+_OptionalQueryPlanningContextTypeDef = TypedDict(
+    "_OptionalQueryPlanningContextTypeDef",
     {
         "CatalogId": str,
+        "QueryAsOfTime": TimestampTypeDef,
+        "QueryParameters": Mapping[str, str],
+        "TransactionId": str,
     },
     total=False,
 )
 
 
-class LFTagPolicyResourceTypeDef(
-    _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
+class QueryPlanningContextTypeDef(
+    _RequiredQueryPlanningContextTypeDef, _OptionalQueryPlanningContextTypeDef
 ):
     pass
 
 
-_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
+_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
-        "Expression": Sequence[LFTagTypeDef],
+        "TableArn": str,
+        "Partition": PartitionValueListTypeDef,
+        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
 )
-_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
+_OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "CatalogId": str,
+        "Permissions": Sequence[PermissionType],
+        "DurationSeconds": int,
+        "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
 
-class SearchDatabasesByLFTagsRequestRequestTypeDef(
-    _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef,
-    _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
+class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(
+    _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+    _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
-    "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     {
-        "Expression": Sequence[LFTagTypeDef],
+        "QueryId": str,
     },
 )
-_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
-    "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     {
-        "CatalogId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
-    _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-    _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
+    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
+ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     {
-        "Expression": Sequence[LFTagTypeDef],
+        "CatalogId": str,
+        "ResourceShareType": ResourceShareTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
+
+GetWorkUnitsResponseTypeDef = TypedDict(
+    "GetWorkUnitsResponseTypeDef",
     {
         "NextToken": str,
-        "MaxResults": int,
+        "QueryId": str,
+        "WorkUnitRanges": List[WorkUnitRangeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredLFTagPolicyResourceOutputTypeDef = TypedDict(
+    "_RequiredLFTagPolicyResourceOutputTypeDef",
+    {
+        "ResourceType": ResourceTypeType,
+        "Expression": List[LFTagOutputTypeDef],
+    },
+)
+_OptionalLFTagPolicyResourceOutputTypeDef = TypedDict(
+    "_OptionalLFTagPolicyResourceOutputTypeDef",
+    {
         "CatalogId": str,
     },
     total=False,
 )
 
 
-class SearchTablesByLFTagsRequestRequestTypeDef(
-    _RequiredSearchTablesByLFTagsRequestRequestTypeDef,
-    _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
+class LFTagPolicyResourceOutputTypeDef(
+    _RequiredLFTagPolicyResourceOutputTypeDef, _OptionalLFTagPolicyResourceOutputTypeDef
 ):
     pass
 
 
-_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
-    "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+LFTagPairUnionTypeDef = Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]
+_RequiredLFTagPolicyResourceTypeDef = TypedDict(
+    "_RequiredLFTagPolicyResourceTypeDef",
     {
+        "ResourceType": ResourceTypeType,
         "Expression": Sequence[LFTagTypeDef],
     },
 )
-_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
-    "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+_OptionalLFTagPolicyResourceTypeDef = TypedDict(
+    "_OptionalLFTagPolicyResourceTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
-    _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
-    _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+class LFTagPolicyResourceTypeDef(
+    _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
 ):
     pass
 
 
+LFTagUnionTypeDef = Union[LFTagTypeDef, LFTagOutputTypeDef]
 ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = TypedDict(
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     {
         "Table": TableResourceTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDataCellsFilterRequestRequestTypeDef = TypedDict(
     "ListDataCellsFilterRequestRequestTypeDef",
     {
@@ -1442,124 +1544,133 @@
 )
 
 ListTableStorageOptimizersResponseTypeDef = TypedDict(
     "ListTableStorageOptimizersResponseTypeDef",
     {
         "StorageOptimizerList": List[StorageOptimizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
     total=False,
 )
 
-StartQueryPlanningRequestRequestTypeDef = TypedDict(
-    "StartQueryPlanningRequestRequestTypeDef",
+TableResourceUnionTypeDef = Union[TableResourceTypeDef, TableResourceOutputTypeDef]
+DataLakeSettingsOutputTypeDef = TypedDict(
+    "DataLakeSettingsOutputTypeDef",
     {
-        "QueryPlanningContext": QueryPlanningContextTypeDef,
-        "QueryString": str,
+        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
+        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "Parameters": Dict[str, str],
+        "TrustedResourceOwners": List[str],
+        "AllowExternalDataFiltering": bool,
+        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
+        "AuthorizedSessionTagValueList": List[str],
+    },
+    total=False,
+)
+
+DataLakeSettingsTypeDef = TypedDict(
+    "DataLakeSettingsTypeDef",
+    {
+        "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
+        "CreateDatabaseDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "Parameters": Mapping[str, str],
+        "TrustedResourceOwners": Sequence[str],
+        "AllowExternalDataFiltering": bool,
+        "ExternalDataFilteringAllowList": Sequence[DataLakePrincipalTypeDef],
+        "AuthorizedSessionTagValueList": Sequence[str],
     },
+    total=False,
 )
 
 GetResourceLFTagsResponseTypeDef = TypedDict(
     "GetResourceLFTagsResponseTypeDef",
     {
-        "LFTagOnDatabase": List[LFTagPairTypeDef],
-        "LFTagsOnTable": List[LFTagPairTypeDef],
+        "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
+        "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaggedTableTypeDef = TypedDict(
     "TaggedTableTypeDef",
     {
-        "Table": TableResourceTypeDef,
-        "LFTagOnDatabase": List[LFTagPairTypeDef],
-        "LFTagsOnTable": List[LFTagPairTypeDef],
+        "Table": TableResourceOutputTypeDef,
+        "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
+        "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
     total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveLFTagsFromResourceResponseTypeDef = TypedDict(
     "RemoveLFTagsFromResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DataLakeSettingsTypeDef = TypedDict(
-    "DataLakeSettingsTypeDef",
-    {
-        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
-        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsTypeDef],
-        "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
-        "Parameters": Dict[str, str],
-        "TrustedResourceOwners": List[str],
-        "AllowExternalDataFiltering": bool,
-        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
-        "AuthorizedSessionTagValueList": List[str],
-    },
-    total=False,
-)
-
-CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
-    "CreateDataCellsFilterRequestRequestTypeDef",
-    {
-        "TableData": DataCellsFilterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataCellsFilterResponseTypeDef = TypedDict(
     "GetDataCellsFilterResponseTypeDef",
     {
-        "DataCellsFilter": DataCellsFilterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataCellsFilter": DataCellsFilterOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataCellsFilterResponseTypeDef = TypedDict(
     "ListDataCellsFilterResponseTypeDef",
     {
-        "DataCellsFilters": List[DataCellsFilterTypeDef],
+        "DataCellsFilters": List[DataCellsFilterOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
+    "CreateDataCellsFilterRequestRequestTypeDef",
+    {
+        "TableData": DataCellsFilterTypeDef,
     },
 )
 
+DataCellsFilterUnionTypeDef = Union[DataCellsFilterTypeDef, DataCellsFilterOutputTypeDef]
 UpdateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "UpdateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
     },
 )
 
 SearchDatabasesByLFTagsResponseTypeDef = TypedDict(
     "SearchDatabasesByLFTagsResponseTypeDef",
     {
         "NextToken": str,
         "DatabaseList": List[TaggedDatabaseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -1580,14 +1691,37 @@
 class UpdateTableObjectsRequestRequestTypeDef(
     _RequiredUpdateTableObjectsRequestRequestTypeDef,
     _OptionalUpdateTableObjectsRequestRequestTypeDef,
 ):
     pass
 
 
+StartQueryPlanningRequestRequestTypeDef = TypedDict(
+    "StartQueryPlanningRequestRequestTypeDef",
+    {
+        "QueryPlanningContext": QueryPlanningContextTypeDef,
+        "QueryString": str,
+    },
+)
+
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
+    {
+        "Catalog": Dict[str, Any],
+        "Database": DatabaseResourceTypeDef,
+        "Table": TableResourceOutputTypeDef,
+        "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
+        "DataLocation": DataLocationResourceTypeDef,
+        "DataCellsFilter": DataCellsFilterResourceTypeDef,
+        "LFTag": LFTagKeyResourceOutputTypeDef,
+        "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
+    },
+    total=False,
+)
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
         "Table": TableResourceTypeDef,
         "TableWithColumns": TableWithColumnsResourceTypeDef,
@@ -1595,40 +1729,126 @@
         "DataCellsFilter": DataCellsFilterResourceTypeDef,
         "LFTag": LFTagKeyResourceTypeDef,
         "LFTagPolicy": LFTagPolicyResourceTypeDef,
     },
     total=False,
 )
 
-GetTableObjectsResponseTypeDef = TypedDict(
-    "GetTableObjectsResponseTypeDef",
+_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
+    {
+        "Expression": Sequence[LFTagUnionTypeDef],
+    },
+)
+_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
     {
-        "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxResults": int,
+        "CatalogId": str,
     },
+    total=False,
 )
 
-SearchTablesByLFTagsResponseTypeDef = TypedDict(
-    "SearchTablesByLFTagsResponseTypeDef",
+
+class SearchDatabasesByLFTagsRequestRequestTypeDef(
+    _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef,
+    _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
+    "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    {
+        "Expression": Sequence[LFTagUnionTypeDef],
+    },
+)
+_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
+    "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
+    _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+    _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
+    {
+        "Expression": Sequence[LFTagUnionTypeDef],
+    },
+)
+_OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
     {
         "NextToken": str,
-        "TableList": List[TaggedTableTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxResults": int,
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+
+class SearchTablesByLFTagsRequestRequestTypeDef(
+    _RequiredSearchTablesByLFTagsRequestRequestTypeDef,
+    _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
+    "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    {
+        "Expression": Sequence[LFTagUnionTypeDef],
+    },
+)
+_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
+    "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
+    _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+    _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+):
+    pass
+
+
+GetTableObjectsResponseTypeDef = TypedDict(
+    "GetTableObjectsResponseTypeDef",
+    {
+        "Objects": List[PartitionObjectsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataLakeSettingsResponseTypeDef = TypedDict(
     "GetDataLakeSettingsResponseTypeDef",
     {
-        "DataLakeSettings": DataLakeSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataLakeSettings": DataLakeSettingsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataLakeSettingsUnionTypeDef = Union[DataLakeSettingsTypeDef, DataLakeSettingsOutputTypeDef]
 _RequiredPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataLakeSettingsRequestRequestTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
     },
 )
 _OptionalPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
@@ -1643,19 +1863,65 @@
 class PutDataLakeSettingsRequestRequestTypeDef(
     _RequiredPutDataLakeSettingsRequestRequestTypeDef,
     _OptionalPutDataLakeSettingsRequestRequestTypeDef,
 ):
     pass
 
 
+SearchTablesByLFTagsResponseTypeDef = TypedDict(
+    "SearchTablesByLFTagsResponseTypeDef",
+    {
+        "NextToken": str,
+        "TableList": List[TaggedTableTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "_RequiredBatchPermissionsRequestEntryOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "_OptionalBatchPermissionsRequestEntryOutputTypeDef",
+    {
+        "Principal": DataLakePrincipalTypeDef,
+        "Resource": ResourceOutputTypeDef,
+        "Permissions": List[PermissionType],
+        "PermissionsWithGrantOption": List[PermissionType],
+    },
+    total=False,
+)
+
+
+class BatchPermissionsRequestEntryOutputTypeDef(
+    _RequiredBatchPermissionsRequestEntryOutputTypeDef,
+    _OptionalBatchPermissionsRequestEntryOutputTypeDef,
+):
+    pass
+
+
+PrincipalResourcePermissionsTypeDef = TypedDict(
+    "PrincipalResourcePermissionsTypeDef",
+    {
+        "Principal": DataLakePrincipalTypeDef,
+        "Resource": ResourceOutputTypeDef,
+        "Permissions": List[PermissionType],
+        "PermissionsWithGrantOption": List[PermissionType],
+        "AdditionalDetails": DetailsMapTypeDef,
+    },
+    total=False,
+)
+
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[LFTagPairTypeDef],
+        "LFTags": Sequence[LFTagPairUnionTypeDef],
     },
 )
 _OptionalAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_OptionalAddLFTagsToResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -1750,31 +2016,19 @@
         "NextToken": str,
         "MaxResults": int,
         "IncludeRelated": str,
     },
     total=False,
 )
 
-PrincipalResourcePermissionsTypeDef = TypedDict(
-    "PrincipalResourcePermissionsTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
-        "Resource": ResourceTypeDef,
-        "Permissions": List[PermissionType],
-        "PermissionsWithGrantOption": List[PermissionType],
-        "AdditionalDetails": DetailsMapTypeDef,
-    },
-    total=False,
-)
-
 _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[LFTagPairTypeDef],
+        "LFTags": Sequence[LFTagPairUnionTypeDef],
     },
 )
 _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_OptionalRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -1785,14 +2039,15 @@
 class RemoveLFTagsFromResourceRequestRequestTypeDef(
     _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef,
     _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef,
 ):
     pass
 
 
+ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
 _RequiredRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredRevokePermissionsRequestRequestTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Resource": ResourceTypeDef,
         "Permissions": Sequence[PermissionType],
     },
@@ -1809,18 +2064,64 @@
 
 class RevokePermissionsRequestRequestTypeDef(
     _RequiredRevokePermissionsRequestRequestTypeDef, _OptionalRevokePermissionsRequestRequestTypeDef
 ):
     pass
 
 
+BatchPermissionsFailureEntryTypeDef = TypedDict(
+    "BatchPermissionsFailureEntryTypeDef",
+    {
+        "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
+        "Error": ErrorDetailTypeDef,
+    },
+    total=False,
+)
+
+GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
+    "GetEffectivePermissionsForPathResponseTypeDef",
+    {
+        "Permissions": List[PrincipalResourcePermissionsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPermissionsResponseTypeDef = TypedDict(
+    "ListPermissionsResponseTypeDef",
+    {
+        "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchPermissionsRequestEntryUnionTypeDef = Union[
+    BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef
+]
+BatchGrantPermissionsResponseTypeDef = TypedDict(
+    "BatchGrantPermissionsResponseTypeDef",
+    {
+        "Failures": List[BatchPermissionsFailureEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchRevokePermissionsResponseTypeDef = TypedDict(
+    "BatchRevokePermissionsResponseTypeDef",
+    {
+        "Failures": List[BatchPermissionsFailureEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
     {
-        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
+        "Entries": Sequence[BatchPermissionsRequestEntryUnionTypeDef],
     },
 )
 _OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalBatchGrantPermissionsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -1831,27 +2132,18 @@
 class BatchGrantPermissionsRequestRequestTypeDef(
     _RequiredBatchGrantPermissionsRequestRequestTypeDef,
     _OptionalBatchGrantPermissionsRequestRequestTypeDef,
 ):
     pass
 
 
-BatchPermissionsFailureEntryTypeDef = TypedDict(
-    "BatchPermissionsFailureEntryTypeDef",
-    {
-        "RequestEntry": BatchPermissionsRequestEntryTypeDef,
-        "Error": ErrorDetailTypeDef,
-    },
-    total=False,
-)
-
 _RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
     {
-        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
+        "Entries": Sequence[BatchPermissionsRequestEntryUnionTypeDef],
     },
 )
 _OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_OptionalBatchRevokePermissionsRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -1860,42 +2152,7 @@
 
 
 class BatchRevokePermissionsRequestRequestTypeDef(
     _RequiredBatchRevokePermissionsRequestRequestTypeDef,
     _OptionalBatchRevokePermissionsRequestRequestTypeDef,
 ):
     pass
-
-
-GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
-    "GetEffectivePermissionsForPathResponseTypeDef",
-    {
-        "Permissions": List[PrincipalResourcePermissionsTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPermissionsResponseTypeDef = TypedDict(
-    "ListPermissionsResponseTypeDef",
-    {
-        "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchGrantPermissionsResponseTypeDef = TypedDict(
-    "BatchGrantPermissionsResponseTypeDef",
-    {
-        "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchRevokePermissionsResponseTypeDef = TypedDict(
-    "BatchRevokePermissionsResponseTypeDef",
-    {
-        "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation/type_defs.pyi` & `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lakeformation service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_lakeformation.type_defs import LFTagPairTypeDef
+    from types_aiobotocore_lakeformation.type_defs import ResponseMetadataTypeDef
 
-    data: LFTagPairTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -34,26 +34,27 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "LFTagPairTypeDef",
+    "ResponseMetadataTypeDef",
     "AddObjectInputTypeDef",
     "AssumeDecoratedRoleWithSAMLRequestRequestTypeDef",
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     "AuditContextTypeDef",
     "ErrorDetailTypeDef",
     "DataLakePrincipalTypeDef",
     "CancelTransactionRequestRequestTypeDef",
+    "LFTagPairOutputTypeDef",
+    "ColumnWildcardOutputTypeDef",
     "ColumnWildcardTypeDef",
     "CommitTransactionRequestRequestTypeDef",
-    "CommitTransactionResponseTypeDef",
     "CreateLFTagRequestRequestTypeDef",
+    "RowFilterOutputTypeDef",
     "DataCellsFilterResourceTypeDef",
     "RowFilterTypeDef",
     "DataLocationResourceTypeDef",
     "DatabaseResourceTypeDef",
     "DeleteDataCellsFilterRequestRequestTypeDef",
     "DeleteLFTagRequestRequestTypeDef",
     "DeleteObjectInputTypeDef",
@@ -67,127 +68,140 @@
     "ExecutionStatisticsTypeDef",
     "ExtendTransactionRequestRequestTypeDef",
     "FilterConditionTypeDef",
     "GetDataCellsFilterRequestRequestTypeDef",
     "GetDataLakeSettingsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathRequestRequestTypeDef",
     "GetLFTagRequestRequestTypeDef",
-    "GetLFTagResponseTypeDef",
     "GetQueryStateRequestRequestTypeDef",
-    "GetQueryStateResponseTypeDef",
     "GetQueryStatisticsRequestRequestTypeDef",
     "PlanningStatisticsTypeDef",
-    "GetTableObjectsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "PartitionValueListTypeDef",
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
     "GetWorkUnitResultsRequestRequestTypeDef",
-    "GetWorkUnitResultsResponseTypeDef",
-    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetWorkUnitsRequestRequestTypeDef",
     "WorkUnitRangeTypeDef",
+    "LFTagKeyResourceOutputTypeDef",
     "LFTagKeyResourceTypeDef",
+    "LFTagOutputTypeDef",
+    "LFTagPairTypeDef",
     "LFTagTypeDef",
     "TableResourceTypeDef",
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "ListLFTagsRequestRequestTypeDef",
     "ListTableStorageOptimizersRequestRequestTypeDef",
     "StorageOptimizerTypeDef",
     "ListTransactionsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "TableObjectTypeDef",
-    "QueryPlanningContextTypeDef",
     "RegisterResourceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartQueryPlanningResponseTypeDef",
+    "TableResourceOutputTypeDef",
     "StartTransactionRequestRequestTypeDef",
-    "StartTransactionResponseTypeDef",
     "UpdateLFTagRequestRequestTypeDef",
     "UpdateResourceRequestRequestTypeDef",
     "UpdateTableStorageOptimizerRequestRequestTypeDef",
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
+    "CommitTransactionResponseTypeDef",
+    "GetLFTagResponseTypeDef",
+    "GetQueryStateResponseTypeDef",
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    "GetWorkUnitResultsResponseTypeDef",
+    "StartQueryPlanningResponseTypeDef",
+    "StartTransactionResponseTypeDef",
     "UpdateTableStorageOptimizerResponseTypeDef",
-    "ColumnLFTagTypeDef",
-    "ListLFTagsResponseTypeDef",
     "GetTemporaryGlueTableCredentialsRequestRequestTypeDef",
-    "LFTagErrorTypeDef",
+    "PrincipalPermissionsOutputTypeDef",
     "PrincipalPermissionsTypeDef",
+    "ColumnLFTagTypeDef",
+    "LFTagErrorTypeDef",
+    "ListLFTagsResponseTypeDef",
+    "TableWithColumnsResourceOutputTypeDef",
     "TableWithColumnsResourceTypeDef",
+    "DataCellsFilterOutputTypeDef",
     "DataCellsFilterTypeDef",
     "TaggedDatabaseTypeDef",
     "WriteOperationTypeDef",
     "DeleteObjectsOnCancelRequestRequestTypeDef",
     "DescribeResourceResponseTypeDef",
     "ListResourcesResponseTypeDef",
     "DescribeTransactionResponseTypeDef",
     "ListTransactionsResponseTypeDef",
     "ListResourcesRequestRequestTypeDef",
     "GetQueryStatisticsResponseTypeDef",
+    "GetTableObjectsRequestRequestTypeDef",
+    "QueryPlanningContextTypeDef",
     "GetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
+    "GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     "GetWorkUnitsResponseTypeDef",
+    "LFTagPolicyResourceOutputTypeDef",
+    "LFTagPairUnionTypeDef",
     "LFTagPolicyResourceTypeDef",
-    "SearchDatabasesByLFTagsRequestRequestTypeDef",
-    "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
-    "SearchTablesByLFTagsRequestRequestTypeDef",
-    "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    "LFTagUnionTypeDef",
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     "ListDataCellsFilterRequestRequestTypeDef",
     "ListTableStorageOptimizersResponseTypeDef",
     "PartitionObjectsTypeDef",
-    "StartQueryPlanningRequestRequestTypeDef",
+    "TableResourceUnionTypeDef",
+    "DataLakeSettingsOutputTypeDef",
+    "DataLakeSettingsTypeDef",
     "GetResourceLFTagsResponseTypeDef",
     "TaggedTableTypeDef",
     "AddLFTagsToResourceResponseTypeDef",
     "RemoveLFTagsFromResourceResponseTypeDef",
-    "DataLakeSettingsTypeDef",
-    "CreateDataCellsFilterRequestRequestTypeDef",
     "GetDataCellsFilterResponseTypeDef",
     "ListDataCellsFilterResponseTypeDef",
+    "CreateDataCellsFilterRequestRequestTypeDef",
+    "DataCellsFilterUnionTypeDef",
     "UpdateDataCellsFilterRequestRequestTypeDef",
     "SearchDatabasesByLFTagsResponseTypeDef",
     "UpdateTableObjectsRequestRequestTypeDef",
+    "StartQueryPlanningRequestRequestTypeDef",
+    "ResourceOutputTypeDef",
     "ResourceTypeDef",
+    "SearchDatabasesByLFTagsRequestRequestTypeDef",
+    "SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    "SearchTablesByLFTagsRequestRequestTypeDef",
+    "SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
     "GetTableObjectsResponseTypeDef",
-    "SearchTablesByLFTagsResponseTypeDef",
     "GetDataLakeSettingsResponseTypeDef",
+    "DataLakeSettingsUnionTypeDef",
     "PutDataLakeSettingsRequestRequestTypeDef",
+    "SearchTablesByLFTagsResponseTypeDef",
+    "BatchPermissionsRequestEntryOutputTypeDef",
+    "PrincipalResourcePermissionsTypeDef",
     "AddLFTagsToResourceRequestRequestTypeDef",
     "BatchPermissionsRequestEntryTypeDef",
     "GetResourceLFTagsRequestRequestTypeDef",
     "GrantPermissionsRequestRequestTypeDef",
     "ListPermissionsRequestRequestTypeDef",
-    "PrincipalResourcePermissionsTypeDef",
     "RemoveLFTagsFromResourceRequestRequestTypeDef",
+    "ResourceUnionTypeDef",
     "RevokePermissionsRequestRequestTypeDef",
-    "BatchGrantPermissionsRequestRequestTypeDef",
     "BatchPermissionsFailureEntryTypeDef",
-    "BatchRevokePermissionsRequestRequestTypeDef",
     "GetEffectivePermissionsForPathResponseTypeDef",
     "ListPermissionsResponseTypeDef",
+    "BatchPermissionsRequestEntryUnionTypeDef",
     "BatchGrantPermissionsResponseTypeDef",
     "BatchRevokePermissionsResponseTypeDef",
+    "BatchGrantPermissionsRequestRequestTypeDef",
+    "BatchRevokePermissionsRequestRequestTypeDef",
 )
 
-_RequiredLFTagPairTypeDef = TypedDict(
-    "_RequiredLFTagPairTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": Sequence[str],
-    },
-)
-_OptionalLFTagPairTypeDef = TypedDict(
-    "_OptionalLFTagPairTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CatalogId": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
-    pass
-
 _RequiredAddObjectInputTypeDef = TypedDict(
     "_RequiredAddObjectInputTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
@@ -221,25 +235,14 @@
 
 class AssumeDecoratedRoleWithSAMLRequestRequestTypeDef(
     _RequiredAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
     _OptionalAssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
 ):
     pass
 
-AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
-    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AuditContextTypeDef = TypedDict(
     "AuditContextTypeDef",
     {
         "AdditionalAuditContext": str,
     },
     total=False,
 )
@@ -264,14 +267,40 @@
 CancelTransactionRequestRequestTypeDef = TypedDict(
     "CancelTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
+_RequiredLFTagPairOutputTypeDef = TypedDict(
+    "_RequiredLFTagPairOutputTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+_OptionalLFTagPairOutputTypeDef = TypedDict(
+    "_OptionalLFTagPairOutputTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class LFTagPairOutputTypeDef(_RequiredLFTagPairOutputTypeDef, _OptionalLFTagPairOutputTypeDef):
+    pass
+
+ColumnWildcardOutputTypeDef = TypedDict(
+    "ColumnWildcardOutputTypeDef",
+    {
+        "ExcludedColumnNames": List[str],
+    },
+    total=False,
+)
+
 ColumnWildcardTypeDef = TypedDict(
     "ColumnWildcardTypeDef",
     {
         "ExcludedColumnNames": Sequence[str],
     },
     total=False,
 )
@@ -279,22 +308,14 @@
 CommitTransactionRequestRequestTypeDef = TypedDict(
     "CommitTransactionRequestRequestTypeDef",
     {
         "TransactionId": str,
     },
 )
 
-CommitTransactionResponseTypeDef = TypedDict(
-    "CommitTransactionResponseTypeDef",
-    {
-        "TransactionStatus": TransactionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -307,14 +328,23 @@
 )
 
 class CreateLFTagRequestRequestTypeDef(
     _RequiredCreateLFTagRequestRequestTypeDef, _OptionalCreateLFTagRequestRequestTypeDef
 ):
     pass
 
+RowFilterOutputTypeDef = TypedDict(
+    "RowFilterOutputTypeDef",
+    {
+        "FilterExpression": str,
+        "AllRowsWildcard": Dict[str, Any],
+    },
+    total=False,
+)
+
 DataCellsFilterResourceTypeDef = TypedDict(
     "DataCellsFilterResourceTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -568,40 +598,21 @@
 )
 
 class GetLFTagRequestRequestTypeDef(
     _RequiredGetLFTagRequestRequestTypeDef, _OptionalGetLFTagRequestRequestTypeDef
 ):
     pass
 
-GetLFTagResponseTypeDef = TypedDict(
-    "GetLFTagResponseTypeDef",
-    {
-        "CatalogId": str,
-        "TagKey": str,
-        "TagValues": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetQueryStateRequestRequestTypeDef = TypedDict(
     "GetQueryStateRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
-GetQueryStateResponseTypeDef = TypedDict(
-    "GetQueryStateResponseTypeDef",
-    {
-        "Error": str,
-        "State": QueryStateStringType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetQueryStatisticsRequestRequestTypeDef = TypedDict(
     "GetQueryStatisticsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
@@ -612,105 +623,41 @@
         "PlanningTimeMillis": int,
         "QueueTimeMillis": int,
         "WorkUnitsGeneratedCount": int,
     },
     total=False,
 )
 
-_RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTableObjectsRequestRequestTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-    },
-)
-_OptionalGetTableObjectsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTableObjectsRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-        "TransactionId": str,
-        "QueryAsOfTime": Union[datetime, str],
-        "PartitionPredicate": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class GetTableObjectsRequestRequestTypeDef(
-    _RequiredGetTableObjectsRequestRequestTypeDef, _OptionalGetTableObjectsRequestRequestTypeDef
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 PartitionValueListTypeDef = TypedDict(
     "PartitionValueListTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
-GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
-    "GetTemporaryGlueTableCredentialsResponseTypeDef",
-    {
-        "AccessKeyId": str,
-        "SecretAccessKey": str,
-        "SessionToken": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkUnitResultsRequestRequestTypeDef = TypedDict(
     "GetWorkUnitResultsRequestRequestTypeDef",
     {
         "QueryId": str,
         "WorkUnitId": int,
         "WorkUnitToken": str,
     },
 )
 
-GetWorkUnitResultsResponseTypeDef = TypedDict(
-    "GetWorkUnitResultsResponseTypeDef",
-    {
-        "ResultStream": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
-    {
-        "QueryId": str,
-    },
-)
-_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
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
 
-class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
-    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetWorkUnitsRequestRequestTypeDef = TypedDict(
     "_RequiredGetWorkUnitsRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 _OptionalGetWorkUnitsRequestRequestTypeDef = TypedDict(
@@ -732,14 +679,34 @@
     {
         "WorkUnitIdMax": int,
         "WorkUnitIdMin": int,
         "WorkUnitToken": str,
     },
 )
 
+_RequiredLFTagKeyResourceOutputTypeDef = TypedDict(
+    "_RequiredLFTagKeyResourceOutputTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+_OptionalLFTagKeyResourceOutputTypeDef = TypedDict(
+    "_OptionalLFTagKeyResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class LFTagKeyResourceOutputTypeDef(
+    _RequiredLFTagKeyResourceOutputTypeDef, _OptionalLFTagKeyResourceOutputTypeDef
+):
+    pass
+
 _RequiredLFTagKeyResourceTypeDef = TypedDict(
     "_RequiredLFTagKeyResourceTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -750,14 +717,40 @@
     },
     total=False,
 )
 
 class LFTagKeyResourceTypeDef(_RequiredLFTagKeyResourceTypeDef, _OptionalLFTagKeyResourceTypeDef):
     pass
 
+LFTagOutputTypeDef = TypedDict(
+    "LFTagOutputTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": List[str],
+    },
+)
+
+_RequiredLFTagPairTypeDef = TypedDict(
+    "_RequiredLFTagPairTypeDef",
+    {
+        "TagKey": str,
+        "TagValues": Sequence[str],
+    },
+)
+_OptionalLFTagPairTypeDef = TypedDict(
+    "_OptionalLFTagPairTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class LFTagPairTypeDef(_RequiredLFTagPairTypeDef, _OptionalLFTagPairTypeDef):
+    pass
+
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -777,24 +770,14 @@
     },
     total=False,
 )
 
 class TableResourceTypeDef(_RequiredTableResourceTypeDef, _OptionalTableResourceTypeDef):
     pass
 
-ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
-    "ListLFTagsRequestListLFTagsPaginateTypeDef",
-    {
-        "CatalogId": str,
-        "ResourceShareType": ResourceShareTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLFTagsRequestRequestTypeDef = TypedDict(
     "ListLFTagsRequestRequestTypeDef",
     {
         "CatalogId": str,
         "ResourceShareType": ResourceShareTypeType,
         "MaxResults": int,
         "NextToken": str,
@@ -845,56 +828,24 @@
         "StatusFilter": TransactionStatusFilterType,
         "MaxResults": int,
         "NextToken": str,
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
 TableObjectTypeDef = TypedDict(
     "TableObjectTypeDef",
     {
         "Uri": str,
         "ETag": str,
         "Size": int,
     },
     total=False,
 )
 
-_RequiredQueryPlanningContextTypeDef = TypedDict(
-    "_RequiredQueryPlanningContextTypeDef",
-    {
-        "DatabaseName": str,
-    },
-)
-_OptionalQueryPlanningContextTypeDef = TypedDict(
-    "_OptionalQueryPlanningContextTypeDef",
-    {
-        "CatalogId": str,
-        "QueryAsOfTime": Union[datetime, str],
-        "QueryParameters": Mapping[str, str],
-        "TransactionId": str,
-    },
-    total=False,
-)
-
-class QueryPlanningContextTypeDef(
-    _RequiredQueryPlanningContextTypeDef, _OptionalQueryPlanningContextTypeDef
-):
-    pass
-
 _RequiredRegisterResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalRegisterResourceRequestRequestTypeDef = TypedDict(
@@ -908,49 +859,43 @@
 )
 
 class RegisterResourceRequestRequestTypeDef(
     _RequiredRegisterResourceRequestRequestTypeDef, _OptionalRegisterResourceRequestRequestTypeDef
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredTableResourceOutputTypeDef = TypedDict(
+    "_RequiredTableResourceOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "DatabaseName": str,
     },
 )
-
-StartQueryPlanningResponseTypeDef = TypedDict(
-    "StartQueryPlanningResponseTypeDef",
+_OptionalTableResourceOutputTypeDef = TypedDict(
+    "_OptionalTableResourceOutputTypeDef",
     {
-        "QueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CatalogId": str,
+        "Name": str,
+        "TableWildcard": Dict[str, Any],
     },
+    total=False,
 )
 
+class TableResourceOutputTypeDef(
+    _RequiredTableResourceOutputTypeDef, _OptionalTableResourceOutputTypeDef
+):
+    pass
+
 StartTransactionRequestRequestTypeDef = TypedDict(
     "StartTransactionRequestRequestTypeDef",
     {
         "TransactionType": TransactionTypeType,
     },
     total=False,
 )
 
-StartTransactionResponseTypeDef = TypedDict(
-    "StartTransactionResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLFTagRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLFTagRequestRequestTypeDef",
     {
         "TagKey": str,
     },
 )
 _OptionalUpdateLFTagRequestRequestTypeDef = TypedDict(
@@ -1006,37 +951,103 @@
 
 class UpdateTableStorageOptimizerRequestRequestTypeDef(
     _RequiredUpdateTableStorageOptimizerRequestRequestTypeDef,
     _OptionalUpdateTableStorageOptimizerRequestRequestTypeDef,
 ):
     pass
 
-UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
-    "UpdateTableStorageOptimizerResponseTypeDef",
+AssumeDecoratedRoleWithSAMLResponseTypeDef = TypedDict(
+    "AssumeDecoratedRoleWithSAMLResponseTypeDef",
     {
-        "Result": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ColumnLFTagTypeDef = TypedDict(
-    "ColumnLFTagTypeDef",
+CommitTransactionResponseTypeDef = TypedDict(
+    "CommitTransactionResponseTypeDef",
     {
-        "Name": str,
-        "LFTags": List[LFTagPairTypeDef],
+        "TransactionStatus": TransactionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListLFTagsResponseTypeDef = TypedDict(
-    "ListLFTagsResponseTypeDef",
+GetLFTagResponseTypeDef = TypedDict(
+    "GetLFTagResponseTypeDef",
     {
-        "LFTags": List[LFTagPairTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CatalogId": str,
+        "TagKey": str,
+        "TagValues": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQueryStateResponseTypeDef = TypedDict(
+    "GetQueryStateResponseTypeDef",
+    {
+        "Error": str,
+        "State": QueryStateStringType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemporaryGluePartitionCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGluePartitionCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemporaryGlueTableCredentialsResponseTypeDef = TypedDict(
+    "GetTemporaryGlueTableCredentialsResponseTypeDef",
+    {
+        "AccessKeyId": str,
+        "SecretAccessKey": str,
+        "SessionToken": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkUnitResultsResponseTypeDef = TypedDict(
+    "GetWorkUnitResultsResponseTypeDef",
+    {
+        "ResultStream": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryPlanningResponseTypeDef = TypedDict(
+    "StartQueryPlanningResponseTypeDef",
+    {
+        "QueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartTransactionResponseTypeDef = TypedDict(
+    "StartTransactionResponseTypeDef",
+    {
+        "TransactionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTableStorageOptimizerResponseTypeDef = TypedDict(
+    "UpdateTableStorageOptimizerResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef",
     {
         "TableArn": str,
@@ -1055,32 +1066,81 @@
 
 class GetTemporaryGlueTableCredentialsRequestRequestTypeDef(
     _RequiredGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
     _OptionalGetTemporaryGlueTableCredentialsRequestRequestTypeDef,
 ):
     pass
 
-LFTagErrorTypeDef = TypedDict(
-    "LFTagErrorTypeDef",
+PrincipalPermissionsOutputTypeDef = TypedDict(
+    "PrincipalPermissionsOutputTypeDef",
     {
-        "LFTag": LFTagPairTypeDef,
-        "Error": ErrorDetailTypeDef,
+        "Principal": DataLakePrincipalTypeDef,
+        "Permissions": List[PermissionType],
     },
     total=False,
 )
 
 PrincipalPermissionsTypeDef = TypedDict(
     "PrincipalPermissionsTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
-        "Permissions": List[PermissionType],
+        "Permissions": Sequence[PermissionType],
+    },
+    total=False,
+)
+
+ColumnLFTagTypeDef = TypedDict(
+    "ColumnLFTagTypeDef",
+    {
+        "Name": str,
+        "LFTags": List[LFTagPairOutputTypeDef],
+    },
+    total=False,
+)
+
+LFTagErrorTypeDef = TypedDict(
+    "LFTagErrorTypeDef",
+    {
+        "LFTag": LFTagPairOutputTypeDef,
+        "Error": ErrorDetailTypeDef,
+    },
+    total=False,
+)
+
+ListLFTagsResponseTypeDef = TypedDict(
+    "ListLFTagsResponseTypeDef",
+    {
+        "LFTags": List[LFTagPairOutputTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredTableWithColumnsResourceOutputTypeDef = TypedDict(
+    "_RequiredTableWithColumnsResourceOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "Name": str,
+    },
+)
+_OptionalTableWithColumnsResourceOutputTypeDef = TypedDict(
+    "_OptionalTableWithColumnsResourceOutputTypeDef",
+    {
+        "CatalogId": str,
+        "ColumnNames": List[str],
+        "ColumnWildcard": ColumnWildcardOutputTypeDef,
     },
     total=False,
 )
 
+class TableWithColumnsResourceOutputTypeDef(
+    _RequiredTableWithColumnsResourceOutputTypeDef, _OptionalTableWithColumnsResourceOutputTypeDef
+):
+    pass
+
 _RequiredTableWithColumnsResourceTypeDef = TypedDict(
     "_RequiredTableWithColumnsResourceTypeDef",
     {
         "DatabaseName": str,
         "Name": str,
     },
 )
@@ -1095,14 +1155,39 @@
 )
 
 class TableWithColumnsResourceTypeDef(
     _RequiredTableWithColumnsResourceTypeDef, _OptionalTableWithColumnsResourceTypeDef
 ):
     pass
 
+_RequiredDataCellsFilterOutputTypeDef = TypedDict(
+    "_RequiredDataCellsFilterOutputTypeDef",
+    {
+        "TableCatalogId": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "Name": str,
+    },
+)
+_OptionalDataCellsFilterOutputTypeDef = TypedDict(
+    "_OptionalDataCellsFilterOutputTypeDef",
+    {
+        "RowFilter": RowFilterOutputTypeDef,
+        "ColumnNames": List[str],
+        "ColumnWildcard": ColumnWildcardOutputTypeDef,
+        "VersionId": str,
+    },
+    total=False,
+)
+
+class DataCellsFilterOutputTypeDef(
+    _RequiredDataCellsFilterOutputTypeDef, _OptionalDataCellsFilterOutputTypeDef
+):
+    pass
+
 _RequiredDataCellsFilterTypeDef = TypedDict(
     "_RequiredDataCellsFilterTypeDef",
     {
         "TableCatalogId": str,
         "DatabaseName": str,
         "TableName": str,
         "Name": str,
@@ -1122,15 +1207,15 @@
 class DataCellsFilterTypeDef(_RequiredDataCellsFilterTypeDef, _OptionalDataCellsFilterTypeDef):
     pass
 
 TaggedDatabaseTypeDef = TypedDict(
     "TaggedDatabaseTypeDef",
     {
         "Database": DatabaseResourceTypeDef,
-        "LFTags": List[LFTagPairTypeDef],
+        "LFTags": List[LFTagPairOutputTypeDef],
     },
     total=False,
 )
 
 WriteOperationTypeDef = TypedDict(
     "WriteOperationTypeDef",
     {
@@ -1163,41 +1248,41 @@
 ):
     pass
 
 DescribeResourceResponseTypeDef = TypedDict(
     "DescribeResourceResponseTypeDef",
     {
         "ResourceInfo": ResourceInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesResponseTypeDef = TypedDict(
     "ListResourcesResponseTypeDef",
     {
         "ResourceInfoList": List[ResourceInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTransactionResponseTypeDef = TypedDict(
     "DescribeTransactionResponseTypeDef",
     {
         "TransactionDescription": TransactionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTransactionsResponseTypeDef = TypedDict(
     "ListTransactionsResponseTypeDef",
     {
         "Transactions": List[TransactionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesRequestRequestTypeDef = TypedDict(
     "ListResourcesRequestRequestTypeDef",
     {
         "FilterConditionList": Sequence[FilterConditionTypeDef],
@@ -1209,163 +1294,176 @@
 
 GetQueryStatisticsResponseTypeDef = TypedDict(
     "GetQueryStatisticsResponseTypeDef",
     {
         "ExecutionStatistics": ExecutionStatisticsTypeDef,
         "PlanningStatistics": PlanningStatisticsTypeDef,
         "QuerySubmissionTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
+_RequiredGetTableObjectsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTableObjectsRequestRequestTypeDef",
     {
-        "TableArn": str,
-        "Partition": PartitionValueListTypeDef,
-        "SupportedPermissionTypes": Sequence[PermissionTypeType],
+        "DatabaseName": str,
+        "TableName": str,
     },
 )
-_OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
+_OptionalGetTableObjectsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTableObjectsRequestRequestTypeDef",
     {
-        "Permissions": Sequence[PermissionType],
-        "DurationSeconds": int,
-        "AuditContext": AuditContextTypeDef,
+        "CatalogId": str,
+        "TransactionId": str,
+        "QueryAsOfTime": TimestampTypeDef,
+        "PartitionPredicate": str,
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(
-    _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
-    _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+class GetTableObjectsRequestRequestTypeDef(
+    _RequiredGetTableObjectsRequestRequestTypeDef, _OptionalGetTableObjectsRequestRequestTypeDef
 ):
     pass
 
-GetWorkUnitsResponseTypeDef = TypedDict(
-    "GetWorkUnitsResponseTypeDef",
-    {
-        "NextToken": str,
-        "QueryId": str,
-        "WorkUnitRanges": List[WorkUnitRangeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredLFTagPolicyResourceTypeDef = TypedDict(
-    "_RequiredLFTagPolicyResourceTypeDef",
+_RequiredQueryPlanningContextTypeDef = TypedDict(
+    "_RequiredQueryPlanningContextTypeDef",
     {
-        "ResourceType": ResourceTypeType,
-        "Expression": Sequence[LFTagTypeDef],
+        "DatabaseName": str,
     },
 )
-_OptionalLFTagPolicyResourceTypeDef = TypedDict(
-    "_OptionalLFTagPolicyResourceTypeDef",
+_OptionalQueryPlanningContextTypeDef = TypedDict(
+    "_OptionalQueryPlanningContextTypeDef",
     {
         "CatalogId": str,
+        "QueryAsOfTime": TimestampTypeDef,
+        "QueryParameters": Mapping[str, str],
+        "TransactionId": str,
     },
     total=False,
 )
 
-class LFTagPolicyResourceTypeDef(
-    _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
+class QueryPlanningContextTypeDef(
+    _RequiredQueryPlanningContextTypeDef, _OptionalQueryPlanningContextTypeDef
 ):
     pass
 
-_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
+_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
-        "Expression": Sequence[LFTagTypeDef],
+        "TableArn": str,
+        "Partition": PartitionValueListTypeDef,
+        "SupportedPermissionTypes": Sequence[PermissionTypeType],
     },
 )
-_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
+_OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "CatalogId": str,
+        "Permissions": Sequence[PermissionType],
+        "DurationSeconds": int,
+        "AuditContext": AuditContextTypeDef,
     },
     total=False,
 )
 
-class SearchDatabasesByLFTagsRequestRequestTypeDef(
-    _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef,
-    _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
+class GetTemporaryGluePartitionCredentialsRequestRequestTypeDef(
+    _RequiredGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+    _OptionalGetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
-    "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     {
-        "Expression": Sequence[LFTagTypeDef],
+        "QueryId": str,
     },
 )
-_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
-    "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef",
     {
-        "CatalogId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
-    _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-    _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+class GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef(
+    _RequiredGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    _OptionalGetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
 ):
     pass
 
-_RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
+ListLFTagsRequestListLFTagsPaginateTypeDef = TypedDict(
+    "ListLFTagsRequestListLFTagsPaginateTypeDef",
     {
-        "Expression": Sequence[LFTagTypeDef],
+        "CatalogId": str,
+        "ResourceShareType": ResourceShareTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
+
+GetWorkUnitsResponseTypeDef = TypedDict(
+    "GetWorkUnitsResponseTypeDef",
     {
         "NextToken": str,
-        "MaxResults": int,
+        "QueryId": str,
+        "WorkUnitRanges": List[WorkUnitRangeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredLFTagPolicyResourceOutputTypeDef = TypedDict(
+    "_RequiredLFTagPolicyResourceOutputTypeDef",
+    {
+        "ResourceType": ResourceTypeType,
+        "Expression": List[LFTagOutputTypeDef],
+    },
+)
+_OptionalLFTagPolicyResourceOutputTypeDef = TypedDict(
+    "_OptionalLFTagPolicyResourceOutputTypeDef",
+    {
         "CatalogId": str,
     },
     total=False,
 )
 
-class SearchTablesByLFTagsRequestRequestTypeDef(
-    _RequiredSearchTablesByLFTagsRequestRequestTypeDef,
-    _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
+class LFTagPolicyResourceOutputTypeDef(
+    _RequiredLFTagPolicyResourceOutputTypeDef, _OptionalLFTagPolicyResourceOutputTypeDef
 ):
     pass
 
-_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
-    "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+LFTagPairUnionTypeDef = Union[LFTagPairTypeDef, LFTagPairOutputTypeDef]
+_RequiredLFTagPolicyResourceTypeDef = TypedDict(
+    "_RequiredLFTagPolicyResourceTypeDef",
     {
+        "ResourceType": ResourceTypeType,
         "Expression": Sequence[LFTagTypeDef],
     },
 )
-_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
-    "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+_OptionalLFTagPolicyResourceTypeDef = TypedDict(
+    "_OptionalLFTagPolicyResourceTypeDef",
     {
         "CatalogId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
-    _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
-    _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+class LFTagPolicyResourceTypeDef(
+    _RequiredLFTagPolicyResourceTypeDef, _OptionalLFTagPolicyResourceTypeDef
 ):
     pass
 
+LFTagUnionTypeDef = Union[LFTagTypeDef, LFTagOutputTypeDef]
 ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = TypedDict(
     "ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef",
     {
         "Table": TableResourceTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListDataCellsFilterRequestRequestTypeDef = TypedDict(
     "ListDataCellsFilterRequestRequestTypeDef",
     {
@@ -1377,124 +1475,133 @@
 )
 
 ListTableStorageOptimizersResponseTypeDef = TypedDict(
     "ListTableStorageOptimizersResponseTypeDef",
     {
         "StorageOptimizerList": List[StorageOptimizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PartitionObjectsTypeDef = TypedDict(
     "PartitionObjectsTypeDef",
     {
         "PartitionValues": List[str],
         "Objects": List[TableObjectTypeDef],
     },
     total=False,
 )
 
-StartQueryPlanningRequestRequestTypeDef = TypedDict(
-    "StartQueryPlanningRequestRequestTypeDef",
+TableResourceUnionTypeDef = Union[TableResourceTypeDef, TableResourceOutputTypeDef]
+DataLakeSettingsOutputTypeDef = TypedDict(
+    "DataLakeSettingsOutputTypeDef",
     {
-        "QueryPlanningContext": QueryPlanningContextTypeDef,
-        "QueryString": str,
+        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
+        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "CreateTableDefaultPermissions": List[PrincipalPermissionsOutputTypeDef],
+        "Parameters": Dict[str, str],
+        "TrustedResourceOwners": List[str],
+        "AllowExternalDataFiltering": bool,
+        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
+        "AuthorizedSessionTagValueList": List[str],
     },
+    total=False,
+)
+
+DataLakeSettingsTypeDef = TypedDict(
+    "DataLakeSettingsTypeDef",
+    {
+        "DataLakeAdmins": Sequence[DataLakePrincipalTypeDef],
+        "CreateDatabaseDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "CreateTableDefaultPermissions": Sequence[PrincipalPermissionsTypeDef],
+        "Parameters": Mapping[str, str],
+        "TrustedResourceOwners": Sequence[str],
+        "AllowExternalDataFiltering": bool,
+        "ExternalDataFilteringAllowList": Sequence[DataLakePrincipalTypeDef],
+        "AuthorizedSessionTagValueList": Sequence[str],
+    },
+    total=False,
 )
 
 GetResourceLFTagsResponseTypeDef = TypedDict(
     "GetResourceLFTagsResponseTypeDef",
     {
-        "LFTagOnDatabase": List[LFTagPairTypeDef],
-        "LFTagsOnTable": List[LFTagPairTypeDef],
+        "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
+        "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaggedTableTypeDef = TypedDict(
     "TaggedTableTypeDef",
     {
-        "Table": TableResourceTypeDef,
-        "LFTagOnDatabase": List[LFTagPairTypeDef],
-        "LFTagsOnTable": List[LFTagPairTypeDef],
+        "Table": TableResourceOutputTypeDef,
+        "LFTagOnDatabase": List[LFTagPairOutputTypeDef],
+        "LFTagsOnTable": List[LFTagPairOutputTypeDef],
         "LFTagsOnColumns": List[ColumnLFTagTypeDef],
     },
     total=False,
 )
 
 AddLFTagsToResourceResponseTypeDef = TypedDict(
     "AddLFTagsToResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveLFTagsFromResourceResponseTypeDef = TypedDict(
     "RemoveLFTagsFromResourceResponseTypeDef",
     {
         "Failures": List[LFTagErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DataLakeSettingsTypeDef = TypedDict(
-    "DataLakeSettingsTypeDef",
-    {
-        "DataLakeAdmins": List[DataLakePrincipalTypeDef],
-        "CreateDatabaseDefaultPermissions": List[PrincipalPermissionsTypeDef],
-        "CreateTableDefaultPermissions": List[PrincipalPermissionsTypeDef],
-        "Parameters": Dict[str, str],
-        "TrustedResourceOwners": List[str],
-        "AllowExternalDataFiltering": bool,
-        "ExternalDataFilteringAllowList": List[DataLakePrincipalTypeDef],
-        "AuthorizedSessionTagValueList": List[str],
-    },
-    total=False,
-)
-
-CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
-    "CreateDataCellsFilterRequestRequestTypeDef",
-    {
-        "TableData": DataCellsFilterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataCellsFilterResponseTypeDef = TypedDict(
     "GetDataCellsFilterResponseTypeDef",
     {
-        "DataCellsFilter": DataCellsFilterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataCellsFilter": DataCellsFilterOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataCellsFilterResponseTypeDef = TypedDict(
     "ListDataCellsFilterResponseTypeDef",
     {
-        "DataCellsFilters": List[DataCellsFilterTypeDef],
+        "DataCellsFilters": List[DataCellsFilterOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataCellsFilterRequestRequestTypeDef = TypedDict(
+    "CreateDataCellsFilterRequestRequestTypeDef",
+    {
+        "TableData": DataCellsFilterTypeDef,
     },
 )
 
+DataCellsFilterUnionTypeDef = Union[DataCellsFilterTypeDef, DataCellsFilterOutputTypeDef]
 UpdateDataCellsFilterRequestRequestTypeDef = TypedDict(
     "UpdateDataCellsFilterRequestRequestTypeDef",
     {
         "TableData": DataCellsFilterTypeDef,
     },
 )
 
 SearchDatabasesByLFTagsResponseTypeDef = TypedDict(
     "SearchDatabasesByLFTagsResponseTypeDef",
     {
         "NextToken": str,
         "DatabaseList": List[TaggedDatabaseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTableObjectsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableObjectsRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -1513,14 +1620,37 @@
 
 class UpdateTableObjectsRequestRequestTypeDef(
     _RequiredUpdateTableObjectsRequestRequestTypeDef,
     _OptionalUpdateTableObjectsRequestRequestTypeDef,
 ):
     pass
 
+StartQueryPlanningRequestRequestTypeDef = TypedDict(
+    "StartQueryPlanningRequestRequestTypeDef",
+    {
+        "QueryPlanningContext": QueryPlanningContextTypeDef,
+        "QueryString": str,
+    },
+)
+
+ResourceOutputTypeDef = TypedDict(
+    "ResourceOutputTypeDef",
+    {
+        "Catalog": Dict[str, Any],
+        "Database": DatabaseResourceTypeDef,
+        "Table": TableResourceOutputTypeDef,
+        "TableWithColumns": TableWithColumnsResourceOutputTypeDef,
+        "DataLocation": DataLocationResourceTypeDef,
+        "DataCellsFilter": DataCellsFilterResourceTypeDef,
+        "LFTag": LFTagKeyResourceOutputTypeDef,
+        "LFTagPolicy": LFTagPolicyResourceOutputTypeDef,
+    },
+    total=False,
+)
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Catalog": Mapping[str, Any],
         "Database": DatabaseResourceTypeDef,
         "Table": TableResourceTypeDef,
         "TableWithColumns": TableWithColumnsResourceTypeDef,
@@ -1528,40 +1658,118 @@
         "DataCellsFilter": DataCellsFilterResourceTypeDef,
         "LFTag": LFTagKeyResourceTypeDef,
         "LFTagPolicy": LFTagPolicyResourceTypeDef,
     },
     total=False,
 )
 
-GetTableObjectsResponseTypeDef = TypedDict(
-    "GetTableObjectsResponseTypeDef",
+_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchDatabasesByLFTagsRequestRequestTypeDef",
+    {
+        "Expression": Sequence[LFTagUnionTypeDef],
+    },
+)
+_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchDatabasesByLFTagsRequestRequestTypeDef",
     {
-        "Objects": List[PartitionObjectsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxResults": int,
+        "CatalogId": str,
     },
+    total=False,
 )
 
-SearchTablesByLFTagsResponseTypeDef = TypedDict(
-    "SearchTablesByLFTagsResponseTypeDef",
+class SearchDatabasesByLFTagsRequestRequestTypeDef(
+    _RequiredSearchDatabasesByLFTagsRequestRequestTypeDef,
+    _OptionalSearchDatabasesByLFTagsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
+    "_RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    {
+        "Expression": Sequence[LFTagUnionTypeDef],
+    },
+)
+_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = TypedDict(
+    "_OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef(
+    _RequiredSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+    _OptionalSearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+):
+    pass
+
+_RequiredSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchTablesByLFTagsRequestRequestTypeDef",
+    {
+        "Expression": Sequence[LFTagUnionTypeDef],
+    },
+)
+_OptionalSearchTablesByLFTagsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchTablesByLFTagsRequestRequestTypeDef",
     {
         "NextToken": str,
-        "TableList": List[TaggedTableTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxResults": int,
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class SearchTablesByLFTagsRequestRequestTypeDef(
+    _RequiredSearchTablesByLFTagsRequestRequestTypeDef,
+    _OptionalSearchTablesByLFTagsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
+    "_RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    {
+        "Expression": Sequence[LFTagUnionTypeDef],
+    },
+)
+_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = TypedDict(
+    "_OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef",
+    {
+        "CatalogId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef(
+    _RequiredSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+    _OptionalSearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+):
+    pass
+
+GetTableObjectsResponseTypeDef = TypedDict(
+    "GetTableObjectsResponseTypeDef",
+    {
+        "Objects": List[PartitionObjectsTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataLakeSettingsResponseTypeDef = TypedDict(
     "GetDataLakeSettingsResponseTypeDef",
     {
-        "DataLakeSettings": DataLakeSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DataLakeSettings": DataLakeSettingsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DataLakeSettingsUnionTypeDef = Union[DataLakeSettingsTypeDef, DataLakeSettingsOutputTypeDef]
 _RequiredPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredPutDataLakeSettingsRequestRequestTypeDef",
     {
         "DataLakeSettings": DataLakeSettingsTypeDef,
     },
 )
 _OptionalPutDataLakeSettingsRequestRequestTypeDef = TypedDict(
@@ -1574,19 +1782,63 @@
 
 class PutDataLakeSettingsRequestRequestTypeDef(
     _RequiredPutDataLakeSettingsRequestRequestTypeDef,
     _OptionalPutDataLakeSettingsRequestRequestTypeDef,
 ):
     pass
 
+SearchTablesByLFTagsResponseTypeDef = TypedDict(
+    "SearchTablesByLFTagsResponseTypeDef",
+    {
+        "NextToken": str,
+        "TableList": List[TaggedTableTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "_RequiredBatchPermissionsRequestEntryOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalBatchPermissionsRequestEntryOutputTypeDef = TypedDict(
+    "_OptionalBatchPermissionsRequestEntryOutputTypeDef",
+    {
+        "Principal": DataLakePrincipalTypeDef,
+        "Resource": ResourceOutputTypeDef,
+        "Permissions": List[PermissionType],
+        "PermissionsWithGrantOption": List[PermissionType],
+    },
+    total=False,
+)
+
+class BatchPermissionsRequestEntryOutputTypeDef(
+    _RequiredBatchPermissionsRequestEntryOutputTypeDef,
+    _OptionalBatchPermissionsRequestEntryOutputTypeDef,
+):
+    pass
+
+PrincipalResourcePermissionsTypeDef = TypedDict(
+    "PrincipalResourcePermissionsTypeDef",
+    {
+        "Principal": DataLakePrincipalTypeDef,
+        "Resource": ResourceOutputTypeDef,
+        "Permissions": List[PermissionType],
+        "PermissionsWithGrantOption": List[PermissionType],
+        "AdditionalDetails": DetailsMapTypeDef,
+    },
+    total=False,
+)
+
 _RequiredAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_RequiredAddLFTagsToResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[LFTagPairTypeDef],
+        "LFTags": Sequence[LFTagPairUnionTypeDef],
     },
 )
 _OptionalAddLFTagsToResourceRequestRequestTypeDef = TypedDict(
     "_OptionalAddLFTagsToResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -1673,31 +1925,19 @@
         "NextToken": str,
         "MaxResults": int,
         "IncludeRelated": str,
     },
     total=False,
 )
 
-PrincipalResourcePermissionsTypeDef = TypedDict(
-    "PrincipalResourcePermissionsTypeDef",
-    {
-        "Principal": DataLakePrincipalTypeDef,
-        "Resource": ResourceTypeDef,
-        "Permissions": List[PermissionType],
-        "PermissionsWithGrantOption": List[PermissionType],
-        "AdditionalDetails": DetailsMapTypeDef,
-    },
-    total=False,
-)
-
 _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "Resource": ResourceTypeDef,
-        "LFTags": Sequence[LFTagPairTypeDef],
+        "LFTags": Sequence[LFTagPairUnionTypeDef],
     },
 )
 _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef = TypedDict(
     "_OptionalRemoveLFTagsFromResourceRequestRequestTypeDef",
     {
         "CatalogId": str,
     },
@@ -1706,14 +1946,15 @@
 
 class RemoveLFTagsFromResourceRequestRequestTypeDef(
     _RequiredRemoveLFTagsFromResourceRequestRequestTypeDef,
     _OptionalRemoveLFTagsFromResourceRequestRequestTypeDef,
 ):
     pass
 
+ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
 _RequiredRevokePermissionsRequestRequestTypeDef = TypedDict(
     "_RequiredRevokePermissionsRequestRequestTypeDef",
     {
         "Principal": DataLakePrincipalTypeDef,
         "Resource": ResourceTypeDef,
         "Permissions": Sequence[PermissionType],
     },
@@ -1728,89 +1969,92 @@
 )
 
 class RevokePermissionsRequestRequestTypeDef(
     _RequiredRevokePermissionsRequestRequestTypeDef, _OptionalRevokePermissionsRequestRequestTypeDef
 ):
     pass
 
-_RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
-    {
-        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
-    },
-)
-_OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGrantPermissionsRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class BatchGrantPermissionsRequestRequestTypeDef(
-    _RequiredBatchGrantPermissionsRequestRequestTypeDef,
-    _OptionalBatchGrantPermissionsRequestRequestTypeDef,
-):
-    pass
-
 BatchPermissionsFailureEntryTypeDef = TypedDict(
     "BatchPermissionsFailureEntryTypeDef",
     {
-        "RequestEntry": BatchPermissionsRequestEntryTypeDef,
+        "RequestEntry": BatchPermissionsRequestEntryOutputTypeDef,
         "Error": ErrorDetailTypeDef,
     },
     total=False,
 )
 
-_RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
-    {
-        "Entries": Sequence[BatchPermissionsRequestEntryTypeDef],
-    },
-)
-_OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchRevokePermissionsRequestRequestTypeDef",
-    {
-        "CatalogId": str,
-    },
-    total=False,
-)
-
-class BatchRevokePermissionsRequestRequestTypeDef(
-    _RequiredBatchRevokePermissionsRequestRequestTypeDef,
-    _OptionalBatchRevokePermissionsRequestRequestTypeDef,
-):
-    pass
-
 GetEffectivePermissionsForPathResponseTypeDef = TypedDict(
     "GetEffectivePermissionsForPathResponseTypeDef",
     {
         "Permissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "PrincipalResourcePermissions": List[PrincipalResourcePermissionsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchPermissionsRequestEntryUnionTypeDef = Union[
+    BatchPermissionsRequestEntryTypeDef, BatchPermissionsRequestEntryOutputTypeDef
+]
 BatchGrantPermissionsResponseTypeDef = TypedDict(
     "BatchGrantPermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchRevokePermissionsResponseTypeDef = TypedDict(
     "BatchRevokePermissionsResponseTypeDef",
     {
         "Failures": List[BatchPermissionsFailureEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGrantPermissionsRequestRequestTypeDef",
+    {
+        "Entries": Sequence[BatchPermissionsRequestEntryUnionTypeDef],
     },
 )
+_OptionalBatchGrantPermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGrantPermissionsRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class BatchGrantPermissionsRequestRequestTypeDef(
+    _RequiredBatchGrantPermissionsRequestRequestTypeDef,
+    _OptionalBatchGrantPermissionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchRevokePermissionsRequestRequestTypeDef",
+    {
+        "Entries": Sequence[BatchPermissionsRequestEntryUnionTypeDef],
+    },
+)
+_OptionalBatchRevokePermissionsRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchRevokePermissionsRequestRequestTypeDef",
+    {
+        "CatalogId": str,
+    },
+    total=False,
+)
+
+class BatchRevokePermissionsRequestRequestTypeDef(
+    _RequiredBatchRevokePermissionsRequestRequestTypeDef,
+    _OptionalBatchRevokePermissionsRequestRequestTypeDef,
+):
+    pass
```

### Comparing `types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation.egg-info/PKG-INFO` & `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lakeformation
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LakeFormation 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LakeFormation 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lakeformation type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore lakeformation type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lakeformation"></a>
 
 # types-aiobotocore-lakeformation
 
 [![PyPI - types-aiobotocore-lakeformation](https://img.shields.io/pypi/v/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lakeformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lakeformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lakeformation?color=blue)](https://pypistats.org/packages/types-aiobotocore-lakeformation)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lakeformation)](https://pepy.tech/project/types-aiobotocore-lakeformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LakeFormation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
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
 [types-aiobotocore-lakeformation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lakeformation/).
 
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
@@ -337,35 +336,36 @@
 )
 
 
 def check_value(value: ComparisonOperatorType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lakeformation.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lakeformation.type_defs import (
-    LFTagPairTypeDef,
+    ResponseMetadataTypeDef,
     AddObjectInputTypeDef,
     AssumeDecoratedRoleWithSAMLRequestRequestTypeDef,
-    AssumeDecoratedRoleWithSAMLResponseTypeDef,
     AuditContextTypeDef,
     ErrorDetailTypeDef,
     DataLakePrincipalTypeDef,
     CancelTransactionRequestRequestTypeDef,
+    LFTagPairOutputTypeDef,
+    ColumnWildcardOutputTypeDef,
     ColumnWildcardTypeDef,
     CommitTransactionRequestRequestTypeDef,
-    CommitTransactionResponseTypeDef,
     CreateLFTagRequestRequestTypeDef,
+    RowFilterOutputTypeDef,
     DataCellsFilterResourceTypeDef,
     RowFilterTypeDef,
     DataLocationResourceTypeDef,
     DatabaseResourceTypeDef,
     DeleteDataCellsFilterRequestRequestTypeDef,
     DeleteLFTagRequestRequestTypeDef,
     DeleteObjectInputTypeDef,
@@ -379,111 +379,131 @@
     ExecutionStatisticsTypeDef,
     ExtendTransactionRequestRequestTypeDef,
     FilterConditionTypeDef,
     GetDataCellsFilterRequestRequestTypeDef,
     GetDataLakeSettingsRequestRequestTypeDef,
     GetEffectivePermissionsForPathRequestRequestTypeDef,
     GetLFTagRequestRequestTypeDef,
-    GetLFTagResponseTypeDef,
     GetQueryStateRequestRequestTypeDef,
-    GetQueryStateResponseTypeDef,
     GetQueryStatisticsRequestRequestTypeDef,
     PlanningStatisticsTypeDef,
-    GetTableObjectsRequestRequestTypeDef,
+    TimestampTypeDef,
     PartitionValueListTypeDef,
-    GetTemporaryGluePartitionCredentialsResponseTypeDef,
-    GetTemporaryGlueTableCredentialsResponseTypeDef,
     GetWorkUnitResultsRequestRequestTypeDef,
-    GetWorkUnitResultsResponseTypeDef,
-    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetWorkUnitsRequestRequestTypeDef,
     WorkUnitRangeTypeDef,
+    LFTagKeyResourceOutputTypeDef,
     LFTagKeyResourceTypeDef,
+    LFTagOutputTypeDef,
+    LFTagPairTypeDef,
     LFTagTypeDef,
     TableResourceTypeDef,
-    ListLFTagsRequestListLFTagsPaginateTypeDef,
     ListLFTagsRequestRequestTypeDef,
     ListTableStorageOptimizersRequestRequestTypeDef,
     StorageOptimizerTypeDef,
     ListTransactionsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     TableObjectTypeDef,
-    QueryPlanningContextTypeDef,
     RegisterResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartQueryPlanningResponseTypeDef,
+    TableResourceOutputTypeDef,
     StartTransactionRequestRequestTypeDef,
-    StartTransactionResponseTypeDef,
     UpdateLFTagRequestRequestTypeDef,
     UpdateResourceRequestRequestTypeDef,
     UpdateTableStorageOptimizerRequestRequestTypeDef,
+    AssumeDecoratedRoleWithSAMLResponseTypeDef,
+    CommitTransactionResponseTypeDef,
+    GetLFTagResponseTypeDef,
+    GetQueryStateResponseTypeDef,
+    GetTemporaryGluePartitionCredentialsResponseTypeDef,
+    GetTemporaryGlueTableCredentialsResponseTypeDef,
+    GetWorkUnitResultsResponseTypeDef,
+    StartQueryPlanningResponseTypeDef,
+    StartTransactionResponseTypeDef,
     UpdateTableStorageOptimizerResponseTypeDef,
-    ColumnLFTagTypeDef,
-    ListLFTagsResponseTypeDef,
     GetTemporaryGlueTableCredentialsRequestRequestTypeDef,
-    LFTagErrorTypeDef,
+    PrincipalPermissionsOutputTypeDef,
     PrincipalPermissionsTypeDef,
+    ColumnLFTagTypeDef,
+    LFTagErrorTypeDef,
+    ListLFTagsResponseTypeDef,
+    TableWithColumnsResourceOutputTypeDef,
     TableWithColumnsResourceTypeDef,
+    DataCellsFilterOutputTypeDef,
     DataCellsFilterTypeDef,
     TaggedDatabaseTypeDef,
     WriteOperationTypeDef,
     DeleteObjectsOnCancelRequestRequestTypeDef,
     DescribeResourceResponseTypeDef,
     ListResourcesResponseTypeDef,
     DescribeTransactionResponseTypeDef,
     ListTransactionsResponseTypeDef,
     ListResourcesRequestRequestTypeDef,
     GetQueryStatisticsResponseTypeDef,
+    GetTableObjectsRequestRequestTypeDef,
+    QueryPlanningContextTypeDef,
     GetTemporaryGluePartitionCredentialsRequestRequestTypeDef,
+    GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef,
+    ListLFTagsRequestListLFTagsPaginateTypeDef,
     GetWorkUnitsResponseTypeDef,
+    LFTagPolicyResourceOutputTypeDef,
+    LFTagPairUnionTypeDef,
     LFTagPolicyResourceTypeDef,
-    SearchDatabasesByLFTagsRequestRequestTypeDef,
-    SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
-    SearchTablesByLFTagsRequestRequestTypeDef,
-    SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
+    LFTagUnionTypeDef,
     ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef,
     ListDataCellsFilterRequestRequestTypeDef,
     ListTableStorageOptimizersResponseTypeDef,
     PartitionObjectsTypeDef,
-    StartQueryPlanningRequestRequestTypeDef,
+    TableResourceUnionTypeDef,
+    DataLakeSettingsOutputTypeDef,
+    DataLakeSettingsTypeDef,
     GetResourceLFTagsResponseTypeDef,
     TaggedTableTypeDef,
     AddLFTagsToResourceResponseTypeDef,
     RemoveLFTagsFromResourceResponseTypeDef,
-    DataLakeSettingsTypeDef,
-    CreateDataCellsFilterRequestRequestTypeDef,
     GetDataCellsFilterResponseTypeDef,
     ListDataCellsFilterResponseTypeDef,
+    CreateDataCellsFilterRequestRequestTypeDef,
+    DataCellsFilterUnionTypeDef,
     UpdateDataCellsFilterRequestRequestTypeDef,
     SearchDatabasesByLFTagsResponseTypeDef,
     UpdateTableObjectsRequestRequestTypeDef,
+    StartQueryPlanningRequestRequestTypeDef,
+    ResourceOutputTypeDef,
     ResourceTypeDef,
+    SearchDatabasesByLFTagsRequestRequestTypeDef,
+    SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef,
+    SearchTablesByLFTagsRequestRequestTypeDef,
+    SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef,
     GetTableObjectsResponseTypeDef,
-    SearchTablesByLFTagsResponseTypeDef,
     GetDataLakeSettingsResponseTypeDef,
+    DataLakeSettingsUnionTypeDef,
     PutDataLakeSettingsRequestRequestTypeDef,
+    SearchTablesByLFTagsResponseTypeDef,
+    BatchPermissionsRequestEntryOutputTypeDef,
+    PrincipalResourcePermissionsTypeDef,
     AddLFTagsToResourceRequestRequestTypeDef,
     BatchPermissionsRequestEntryTypeDef,
     GetResourceLFTagsRequestRequestTypeDef,
     GrantPermissionsRequestRequestTypeDef,
     ListPermissionsRequestRequestTypeDef,
-    PrincipalResourcePermissionsTypeDef,
     RemoveLFTagsFromResourceRequestRequestTypeDef,
+    ResourceUnionTypeDef,
     RevokePermissionsRequestRequestTypeDef,
-    BatchGrantPermissionsRequestRequestTypeDef,
     BatchPermissionsFailureEntryTypeDef,
-    BatchRevokePermissionsRequestRequestTypeDef,
     GetEffectivePermissionsForPathResponseTypeDef,
     ListPermissionsResponseTypeDef,
+    BatchPermissionsRequestEntryUnionTypeDef,
     BatchGrantPermissionsResponseTypeDef,
     BatchRevokePermissionsResponseTypeDef,
+    BatchGrantPermissionsRequestRequestTypeDef,
+    BatchRevokePermissionsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> LFTagPairTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lakeformation-2.5.2/types_aiobotocore_lakeformation.egg-info/SOURCES.txt` & `types-aiobotocore-lakeformation-2.5.2.post1/types_aiobotocore_lakeformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*


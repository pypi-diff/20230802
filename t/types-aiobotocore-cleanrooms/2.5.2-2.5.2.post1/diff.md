# Comparing `tmp/types-aiobotocore-cleanrooms-2.5.2.tar.gz` & `tmp/types-aiobotocore-cleanrooms-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cleanrooms-2.5.2.tar", last modified: Sat Jul  8 01:43:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-cleanrooms-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:59 2023, max compression
```

## Comparing `types-aiobotocore-cleanrooms-2.5.2.tar` & `types-aiobotocore-cleanrooms-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:20.549807 types-aiobotocore-cleanrooms-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-07-08 01:43:20.549807 types-aiobotocore-cleanrooms-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17696 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:20.549807 types-aiobotocore-cleanrooms-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:20.549807 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31966 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31913 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-07-08 01:26:48.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41309 2023-07-08 01:26:49.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41256 2023-07-08 01:26:49.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:47.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:20.549807 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19280 2023-07-08 01:43:20.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:20.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:20.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:20.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:20.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:20.000000 types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.853637 types-aiobotocore-cleanrooms-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-08-02 14:51:59.849637 types-aiobotocore-cleanrooms-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:59.853637 types-aiobotocore-cleanrooms-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.849637 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31981 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31928 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-08-02 14:34:17.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43244 2023-08-02 14:34:18.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43189 2023-08-02 14:34:18.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.849637 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-08-02 14:51:59.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:51:59.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:51:59.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2/LICENSE` & `types-aiobotocore-cleanrooms-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2/PKG-INFO` & `types-aiobotocore-cleanrooms-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cleanrooms
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CleanRoomsService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CleanRoomsService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cleanrooms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cleanrooms type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cleanrooms"></a>
 
 # types-aiobotocore-cleanrooms
 
 [![PyPI - types-aiobotocore-cleanrooms](https://img.shields.io/pypi/v/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cleanrooms?color=blue)](https://pypistats.org/packages/types-aiobotocore-cleanrooms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cleanrooms)](https://pepy.tech/project/types-aiobotocore-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CleanRoomsService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [types-aiobotocore-cleanrooms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/).
 
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
@@ -351,28 +350,31 @@
 )
 
 
 def check_value(value: AggregateFunctionNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cleanrooms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cleanrooms.type_defs import (
+    AggregateColumnOutputTypeDef,
     AggregateColumnTypeDef,
     AggregationConstraintTypeDef,
+    AnalysisRuleListOutputTypeDef,
     AnalysisRuleListTypeDef,
     BatchGetSchemaErrorTypeDef,
     BatchGetSchemaInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     CollaborationSummaryTypeDef,
     DataEncryptionMetadataTypeDef,
     ColumnTypeDef,
     ConfiguredTableAssociationSummaryTypeDef,
     ConfiguredTableAssociationTypeDef,
     ConfiguredTableSummaryTypeDef,
     MemberSpecificationTypeDef,
@@ -390,101 +392,104 @@
     GetConfiguredTableAssociationInputRequestTypeDef,
     GetConfiguredTableInputRequestTypeDef,
     GetMembershipInputRequestTypeDef,
     GetProtectedQueryInputRequestTypeDef,
     GetSchemaAnalysisRuleInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     GlueTableReferenceTypeDef,
-    ListCollaborationsInputListCollaborationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCollaborationsInputRequestTypeDef,
-    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
     ListConfiguredTableAssociationsInputRequestTypeDef,
-    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
     ListConfiguredTablesInputRequestTypeDef,
-    ListMembersInputListMembersPaginateTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
-    ListMembershipsInputListMembershipsPaginateTypeDef,
     ListMembershipsInputRequestTypeDef,
     MembershipSummaryTypeDef,
-    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
     ListProtectedQueriesInputRequestTypeDef,
     ProtectedQuerySummaryTypeDef,
-    ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
     ProtectedQueryErrorTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
+    AnalysisRuleAggregationOutputTypeDef,
     AnalysisRuleAggregationTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     CreateCollaborationInputRequestTypeDef,
     CreateMembershipOutputTypeDef,
     GetMembershipOutputTypeDef,
     UpdateMembershipOutputTypeDef,
     TableReferenceTypeDef,
+    ListCollaborationsInputListCollaborationsPaginateTypeDef,
+    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
+    ListMembersInputListMembersPaginateTypeDef,
+    ListMembershipsInputListMembershipsPaginateTypeDef,
+    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+    ListSchemasInputListSchemasPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
     ProtectedQueryOutputConfigurationTypeDef,
     ProtectedQueryOutputTypeDef,
     AnalysisRulePolicyV1TypeDef,
+    ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
     ConfiguredTableAnalysisRulePolicyV1TypeDef,
     CreateCollaborationOutputTypeDef,
     GetCollaborationOutputTypeDef,
     UpdateCollaborationOutputTypeDef,
     BatchGetSchemaOutputTypeDef,
     GetSchemaOutputTypeDef,
     ConfiguredTableTypeDef,
     CreateConfiguredTableInputRequestTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQueryResultTypeDef,
     AnalysisRulePolicyTypeDef,
+    ConfiguredTableAnalysisRulePolicyOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateConfiguredTableOutputTypeDef,
     GetConfiguredTableOutputTypeDef,
     UpdateConfiguredTableOutputTypeDef,
     StartProtectedQueryInputRequestTypeDef,
     ProtectedQueryTypeDef,
     AnalysisRuleTypeDef,
     ConfiguredTableAnalysisRuleTypeDef,
+    ConfiguredTableAnalysisRulePolicyUnionTypeDef,
     CreateConfiguredTableAnalysisRuleInputRequestTypeDef,
     UpdateConfiguredTableAnalysisRuleInputRequestTypeDef,
     GetProtectedQueryOutputTypeDef,
     StartProtectedQueryOutputTypeDef,
     UpdateProtectedQueryOutputTypeDef,
     GetSchemaAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     GetConfiguredTableAnalysisRuleOutputTypeDef,
     UpdateConfiguredTableAnalysisRuleOutputTypeDef,
 )
 
 
-def get_structure() -> AggregateColumnTypeDef:
+def get_value() -> AggregateColumnOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2/README.md` & `types-aiobotocore-cleanrooms-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cleanrooms"></a>
 
 # types-aiobotocore-cleanrooms
 
 [![PyPI - types-aiobotocore-cleanrooms](https://img.shields.io/pypi/v/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cleanrooms?color=blue)](https://pypistats.org/packages/types-aiobotocore-cleanrooms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cleanrooms)](https://pepy.tech/project/types-aiobotocore-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CleanRoomsService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [types-aiobotocore-cleanrooms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/).
 
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
@@ -318,28 +318,31 @@
 )
 
 
 def check_value(value: AggregateFunctionNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cleanrooms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cleanrooms.type_defs import (
+    AggregateColumnOutputTypeDef,
     AggregateColumnTypeDef,
     AggregationConstraintTypeDef,
+    AnalysisRuleListOutputTypeDef,
     AnalysisRuleListTypeDef,
     BatchGetSchemaErrorTypeDef,
     BatchGetSchemaInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     CollaborationSummaryTypeDef,
     DataEncryptionMetadataTypeDef,
     ColumnTypeDef,
     ConfiguredTableAssociationSummaryTypeDef,
     ConfiguredTableAssociationTypeDef,
     ConfiguredTableSummaryTypeDef,
     MemberSpecificationTypeDef,
@@ -357,101 +360,104 @@
     GetConfiguredTableAssociationInputRequestTypeDef,
     GetConfiguredTableInputRequestTypeDef,
     GetMembershipInputRequestTypeDef,
     GetProtectedQueryInputRequestTypeDef,
     GetSchemaAnalysisRuleInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     GlueTableReferenceTypeDef,
-    ListCollaborationsInputListCollaborationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCollaborationsInputRequestTypeDef,
-    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
     ListConfiguredTableAssociationsInputRequestTypeDef,
-    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
     ListConfiguredTablesInputRequestTypeDef,
-    ListMembersInputListMembersPaginateTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
-    ListMembershipsInputListMembershipsPaginateTypeDef,
     ListMembershipsInputRequestTypeDef,
     MembershipSummaryTypeDef,
-    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
     ListProtectedQueriesInputRequestTypeDef,
     ProtectedQuerySummaryTypeDef,
-    ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
     ProtectedQueryErrorTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
+    AnalysisRuleAggregationOutputTypeDef,
     AnalysisRuleAggregationTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     CreateCollaborationInputRequestTypeDef,
     CreateMembershipOutputTypeDef,
     GetMembershipOutputTypeDef,
     UpdateMembershipOutputTypeDef,
     TableReferenceTypeDef,
+    ListCollaborationsInputListCollaborationsPaginateTypeDef,
+    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
+    ListMembersInputListMembersPaginateTypeDef,
+    ListMembershipsInputListMembershipsPaginateTypeDef,
+    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+    ListSchemasInputListSchemasPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
     ProtectedQueryOutputConfigurationTypeDef,
     ProtectedQueryOutputTypeDef,
     AnalysisRulePolicyV1TypeDef,
+    ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
     ConfiguredTableAnalysisRulePolicyV1TypeDef,
     CreateCollaborationOutputTypeDef,
     GetCollaborationOutputTypeDef,
     UpdateCollaborationOutputTypeDef,
     BatchGetSchemaOutputTypeDef,
     GetSchemaOutputTypeDef,
     ConfiguredTableTypeDef,
     CreateConfiguredTableInputRequestTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQueryResultTypeDef,
     AnalysisRulePolicyTypeDef,
+    ConfiguredTableAnalysisRulePolicyOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateConfiguredTableOutputTypeDef,
     GetConfiguredTableOutputTypeDef,
     UpdateConfiguredTableOutputTypeDef,
     StartProtectedQueryInputRequestTypeDef,
     ProtectedQueryTypeDef,
     AnalysisRuleTypeDef,
     ConfiguredTableAnalysisRuleTypeDef,
+    ConfiguredTableAnalysisRulePolicyUnionTypeDef,
     CreateConfiguredTableAnalysisRuleInputRequestTypeDef,
     UpdateConfiguredTableAnalysisRuleInputRequestTypeDef,
     GetProtectedQueryOutputTypeDef,
     StartProtectedQueryOutputTypeDef,
     UpdateProtectedQueryOutputTypeDef,
     GetSchemaAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     GetConfiguredTableAnalysisRuleOutputTypeDef,
     UpdateConfiguredTableAnalysisRuleOutputTypeDef,
 )
 
 
-def get_structure() -> AggregateColumnTypeDef:
+def get_value() -> AggregateColumnOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2/setup.py` & `types-aiobotocore-cleanrooms-2.5.2.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cleanrooms",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cleanrooms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CleanRoomsService 2.5.2 service generated with"
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
-    keywords="aiobotocore cleanrooms type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cleanrooms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cleanrooms": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/"
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/__init__.py` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/__init__.pyi` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/__main__.py` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CleanRoomsService 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CleanRoomsService 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService\nOther"
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

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/client.py` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ListMembershipsPaginator,
     ListMembersPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
 )
 from .type_defs import (
     BatchGetSchemaOutputTypeDef,
-    ConfiguredTableAnalysisRulePolicyTypeDef,
+    ConfiguredTableAnalysisRulePolicyUnionTypeDef,
     CreateCollaborationOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     CreateConfiguredTableOutputTypeDef,
     CreateMembershipOutputTypeDef,
     DataEncryptionMetadataTypeDef,
     GetCollaborationOutputTypeDef,
@@ -185,15 +185,15 @@
         """
 
     async def create_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
+        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyUnionTypeDef
     ) -> CreateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Creates a new analysis rule for a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table_analysis_rule)
         """
@@ -527,15 +527,15 @@
         """
 
     async def update_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
+        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyUnionTypeDef
     ) -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Updates a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table_analysis_rule)
         """
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/client.pyi` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ListMembershipsPaginator,
     ListMembersPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
 )
 from .type_defs import (
     BatchGetSchemaOutputTypeDef,
-    ConfiguredTableAnalysisRulePolicyTypeDef,
+    ConfiguredTableAnalysisRulePolicyUnionTypeDef,
     CreateCollaborationOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     CreateConfiguredTableOutputTypeDef,
     CreateMembershipOutputTypeDef,
     DataEncryptionMetadataTypeDef,
     GetCollaborationOutputTypeDef,
@@ -175,15 +175,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table)
         """
     async def create_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
+        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyUnionTypeDef
     ) -> CreateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Creates a new analysis rule for a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table_analysis_rule)
         """
@@ -486,15 +486,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table)
         """
     async def update_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
+        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyUnionTypeDef
     ) -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Updates a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table_analysis_rule)
         """
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/literals.py` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/literals.pyi` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/paginator.py` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,78 +83,75 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationspaginator)
     """
 
     def paginate(
         self,
         *,
         memberStatus: FilterableMemberStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCollaborationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationspaginator)
         """
 
 
 class ListConfiguredTableAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
     """
 
     def paginate(
-        self, *, membershipIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, membershipIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConfiguredTableAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
         """
 
 
 class ListConfiguredTablesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConfiguredTablesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtablespaginator)
         """
 
 
 class ListMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, collaborationIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, collaborationIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmemberspaginator)
         """
 
 
 class ListMembershipsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmembershipspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        status: MembershipStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: MembershipStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembershipsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmembershipspaginator)
         """
 
 
@@ -165,15 +162,15 @@
     """
 
     def paginate(
         self,
         *,
         membershipIdentifier: str,
         status: ProtectedQueryStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProtectedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listprotectedqueriespaginator)
         """
 
 
@@ -184,13 +181,13 @@
     """
 
     def paginate(
         self,
         *,
         collaborationIdentifier: str,
         schemaType: Literal["TABLE"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSchemasOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listschemaspaginator)
         """
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/paginator.pyi` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -79,74 +79,71 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationspaginator)
     """
 
     def paginate(
         self,
         *,
         memberStatus: FilterableMemberStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCollaborationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationspaginator)
         """
 
 class ListConfiguredTableAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
     """
 
     def paginate(
-        self, *, membershipIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, membershipIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConfiguredTableAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTableAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtableassociationspaginator)
         """
 
 class ListConfiguredTablesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtablespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConfiguredTablesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListConfiguredTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listconfiguredtablespaginator)
         """
 
 class ListMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, collaborationIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, collaborationIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmemberspaginator)
         """
 
 class ListMembershipsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmembershipspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        status: MembershipStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: MembershipStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembershipsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listmembershipspaginator)
         """
 
 class ListProtectedQueriesPaginator(AioPaginator):
@@ -156,15 +153,15 @@
     """
 
     def paginate(
         self,
         *,
         membershipIdentifier: str,
         status: ProtectedQueryStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProtectedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listprotectedqueriespaginator)
         """
 
 class ListSchemasPaginator(AioPaginator):
@@ -174,13 +171,13 @@
     """
 
     def paginate(
         self,
         *,
         collaborationIdentifier: str,
         schemaType: Literal["TABLE"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSchemasOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listschemaspaginator)
         """
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/type_defs.py` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for cleanrooms service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_cleanrooms.type_defs import AggregateColumnTypeDef
+    from types_aiobotocore_cleanrooms.type_defs import AggregateColumnOutputTypeDef
 
-    data: AggregateColumnTypeDef = {...}
+    data: AggregateColumnOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggregateFunctionNameType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
@@ -35,21 +35,23 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AggregateColumnOutputTypeDef",
     "AggregateColumnTypeDef",
     "AggregationConstraintTypeDef",
+    "AnalysisRuleListOutputTypeDef",
     "AnalysisRuleListTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CollaborationSummaryTypeDef",
     "DataEncryptionMetadataTypeDef",
     "ColumnTypeDef",
     "ConfiguredTableAssociationSummaryTypeDef",
     "ConfiguredTableAssociationTypeDef",
     "ConfiguredTableSummaryTypeDef",
     "MemberSpecificationTypeDef",
@@ -67,99 +69,110 @@
     "GetConfiguredTableAssociationInputRequestTypeDef",
     "GetConfiguredTableInputRequestTypeDef",
     "GetMembershipInputRequestTypeDef",
     "GetProtectedQueryInputRequestTypeDef",
     "GetSchemaAnalysisRuleInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "GlueTableReferenceTypeDef",
-    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListCollaborationsInputRequestTypeDef",
-    "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
     "ListConfiguredTableAssociationsInputRequestTypeDef",
-    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
     "ListConfiguredTablesInputRequestTypeDef",
-    "ListMembersInputListMembersPaginateTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
-    "ListMembershipsInputListMembershipsPaginateTypeDef",
     "ListMembershipsInputRequestTypeDef",
     "MembershipSummaryTypeDef",
-    "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
     "ListProtectedQueriesInputRequestTypeDef",
     "ProtectedQuerySummaryTypeDef",
-    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListSchemasInputRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ProtectedQueryErrorTypeDef",
     "ProtectedQueryS3OutputConfigurationTypeDef",
     "ProtectedQueryS3OutputTypeDef",
     "ProtectedQuerySQLParametersTypeDef",
     "ProtectedQueryStatisticsTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
+    "AnalysisRuleAggregationOutputTypeDef",
     "AnalysisRuleAggregationTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
     "GetConfiguredTableAssociationOutputTypeDef",
     "UpdateConfiguredTableAssociationOutputTypeDef",
     "ListConfiguredTablesOutputTypeDef",
     "CreateCollaborationInputRequestTypeDef",
     "CreateMembershipOutputTypeDef",
     "GetMembershipOutputTypeDef",
     "UpdateMembershipOutputTypeDef",
     "TableReferenceTypeDef",
+    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+    "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
+    "ListMembersInputListMembersPaginateTypeDef",
+    "ListMembershipsInputListMembershipsPaginateTypeDef",
+    "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListMembersOutputTypeDef",
     "ListMembershipsOutputTypeDef",
     "ListProtectedQueriesOutputTypeDef",
     "ListSchemasOutputTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
+    "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     "CreateCollaborationOutputTypeDef",
     "GetCollaborationOutputTypeDef",
     "UpdateCollaborationOutputTypeDef",
     "BatchGetSchemaOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "ConfiguredTableTypeDef",
     "CreateConfiguredTableInputRequestTypeDef",
     "ProtectedQueryResultConfigurationTypeDef",
     "ProtectedQueryResultTypeDef",
     "AnalysisRulePolicyTypeDef",
+    "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     "CreateConfiguredTableOutputTypeDef",
     "GetConfiguredTableOutputTypeDef",
     "UpdateConfiguredTableOutputTypeDef",
     "StartProtectedQueryInputRequestTypeDef",
     "ProtectedQueryTypeDef",
     "AnalysisRuleTypeDef",
     "ConfiguredTableAnalysisRuleTypeDef",
+    "ConfiguredTableAnalysisRulePolicyUnionTypeDef",
     "CreateConfiguredTableAnalysisRuleInputRequestTypeDef",
     "UpdateConfiguredTableAnalysisRuleInputRequestTypeDef",
     "GetProtectedQueryOutputTypeDef",
     "StartProtectedQueryOutputTypeDef",
     "UpdateProtectedQueryOutputTypeDef",
     "GetSchemaAnalysisRuleOutputTypeDef",
     "CreateConfiguredTableAnalysisRuleOutputTypeDef",
     "GetConfiguredTableAnalysisRuleOutputTypeDef",
     "UpdateConfiguredTableAnalysisRuleOutputTypeDef",
 )
 
+AggregateColumnOutputTypeDef = TypedDict(
+    "AggregateColumnOutputTypeDef",
+    {
+        "columnNames": List[str],
+        "function": AggregateFunctionNameType,
+    },
+)
+
 AggregateColumnTypeDef = TypedDict(
     "AggregateColumnTypeDef",
     {
         "columnNames": Sequence[str],
         "function": AggregateFunctionNameType,
     },
 )
@@ -169,14 +182,22 @@
     {
         "columnName": str,
         "minimum": int,
         "type": Literal["COUNT_DISTINCT"],
     },
 )
 
+AnalysisRuleListOutputTypeDef = TypedDict(
+    "AnalysisRuleListOutputTypeDef",
+    {
+        "joinColumns": List[str],
+        "listColumns": List[str],
+    },
+)
+
 AnalysisRuleListTypeDef = TypedDict(
     "AnalysisRuleListTypeDef",
     {
         "joinColumns": Sequence[str],
         "listColumns": Sequence[str],
     },
 )
@@ -194,14 +215,25 @@
     "BatchGetSchemaInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "names": Sequence[str],
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
 _RequiredCollaborationSummaryTypeDef = TypedDict(
     "_RequiredCollaborationSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "creatorAccountId": str,
@@ -216,21 +248,19 @@
     {
         "membershipId": str,
         "membershipArn": str,
     },
     total=False,
 )
 
-
 class CollaborationSummaryTypeDef(
     _RequiredCollaborationSummaryTypeDef, _OptionalCollaborationSummaryTypeDef
 ):
     pass
 
-
 DataEncryptionMetadataTypeDef = TypedDict(
     "DataEncryptionMetadataTypeDef",
     {
         "allowCleartext": bool,
         "allowDuplicates": bool,
         "allowJoinsOnColumnsWithDifferentNames": bool,
         "preserveNulls": bool,
@@ -278,21 +308,19 @@
     "_OptionalConfiguredTableAssociationTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class ConfiguredTableAssociationTypeDef(
     _RequiredConfiguredTableAssociationTypeDef, _OptionalConfiguredTableAssociationTypeDef
 ):
     pass
 
-
 ConfiguredTableSummaryTypeDef = TypedDict(
     "ConfiguredTableSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "createTime": datetime,
@@ -325,22 +353,20 @@
     {
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateConfiguredTableAssociationInputRequestTypeDef(
     _RequiredCreateConfiguredTableAssociationInputRequestTypeDef,
     _OptionalCreateConfiguredTableAssociationInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateMembershipInputRequestTypeDef = TypedDict(
     "_RequiredCreateMembershipInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "queryLogStatus": MembershipQueryLogStatusType,
     },
 )
@@ -348,21 +374,19 @@
     "_OptionalCreateMembershipInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateMembershipInputRequestTypeDef(
     _RequiredCreateMembershipInputRequestTypeDef, _OptionalCreateMembershipInputRequestTypeDef
 ):
     pass
 
-
 MembershipTypeDef = TypedDict(
     "MembershipTypeDef",
     {
         "id": str,
         "arn": str,
         "collaborationArn": str,
         "collaborationId": str,
@@ -488,55 +512,34 @@
     "GlueTableReferenceTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
 
-ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
-    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "memberStatus": FilterableMemberStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListCollaborationsInputRequestTypeDef = TypedDict(
     "ListCollaborationsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "memberStatus": FilterableMemberStatusType,
     },
     total=False,
 )
 
-_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    {
-        "membershipIdentifier": str,
-    },
-)
-_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(
-    _RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-    _OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListConfiguredTableAssociationsInputRequestTypeDef = TypedDict(
     "_RequiredListConfiguredTableAssociationsInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalListConfiguredTableAssociationsInputRequestTypeDef = TypedDict(
@@ -544,61 +547,29 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListConfiguredTableAssociationsInputRequestTypeDef(
     _RequiredListConfiguredTableAssociationsInputRequestTypeDef,
     _OptionalListConfiguredTableAssociationsInputRequestTypeDef,
 ):
     pass
 
-
-ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef = TypedDict(
-    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListConfiguredTablesInputRequestTypeDef = TypedDict(
     "ListConfiguredTablesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListMembersInputListMembersPaginateTypeDef = TypedDict(
-    "_RequiredListMembersInputListMembersPaginateTypeDef",
-    {
-        "collaborationIdentifier": str,
-    },
-)
-_OptionalListMembersInputListMembersPaginateTypeDef = TypedDict(
-    "_OptionalListMembersInputListMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMembersInputListMembersPaginateTypeDef(
-    _RequiredListMembersInputListMembersPaginateTypeDef,
-    _OptionalListMembersInputListMembersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMembersInputRequestTypeDef = TypedDict(
     "_RequiredListMembersInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalListMembersInputRequestTypeDef = TypedDict(
@@ -606,21 +577,19 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListMembersInputRequestTypeDef(
     _RequiredListMembersInputRequestTypeDef, _OptionalListMembersInputRequestTypeDef
 ):
     pass
 
-
 _RequiredMemberSummaryTypeDef = TypedDict(
     "_RequiredMemberSummaryTypeDef",
     {
         "accountId": str,
         "status": MemberStatusType,
         "displayName": str,
         "abilities": List[MemberAbilityType],
@@ -633,28 +602,17 @@
     {
         "membershipId": str,
         "membershipArn": str,
     },
     total=False,
 )
 
-
 class MemberSummaryTypeDef(_RequiredMemberSummaryTypeDef, _OptionalMemberSummaryTypeDef):
     pass
 
-
-ListMembershipsInputListMembershipsPaginateTypeDef = TypedDict(
-    "ListMembershipsInputListMembershipsPaginateTypeDef",
-    {
-        "status": MembershipStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMembershipsInputRequestTypeDef = TypedDict(
     "ListMembershipsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": MembershipStatusType,
     },
@@ -674,37 +632,14 @@
         "createTime": datetime,
         "updateTime": datetime,
         "status": MembershipStatusType,
         "memberAbilities": List[MemberAbilityType],
     },
 )
 
-_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
-    "_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    {
-        "membershipIdentifier": str,
-    },
-)
-_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
-    "_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    {
-        "status": ProtectedQueryStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(
-    _RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-    _OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListProtectedQueriesInputRequestTypeDef = TypedDict(
     "_RequiredListProtectedQueriesInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalListProtectedQueriesInputRequestTypeDef = TypedDict(
@@ -713,56 +648,31 @@
         "status": ProtectedQueryStatusType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListProtectedQueriesInputRequestTypeDef(
     _RequiredListProtectedQueriesInputRequestTypeDef,
     _OptionalListProtectedQueriesInputRequestTypeDef,
 ):
     pass
 
-
 ProtectedQuerySummaryTypeDef = TypedDict(
     "ProtectedQuerySummaryTypeDef",
     {
         "id": str,
         "membershipId": str,
         "membershipArn": str,
         "createTime": datetime,
         "status": ProtectedQueryStatusType,
     },
 )
 
-_RequiredListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "collaborationIdentifier": str,
-    },
-)
-_OptionalListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "schemaType": Literal["TABLE"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSchemasInputListSchemasPaginateTypeDef(
-    _RequiredListSchemasInputListSchemasPaginateTypeDef,
-    _OptionalListSchemasInputListSchemasPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSchemasInputRequestTypeDef = TypedDict(
     "_RequiredListSchemasInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalListSchemasInputRequestTypeDef = TypedDict(
@@ -771,21 +681,19 @@
         "schemaType": Literal["TABLE"],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListSchemasInputRequestTypeDef(
     _RequiredListSchemasInputRequestTypeDef, _OptionalListSchemasInputRequestTypeDef
 ):
     pass
 
-
 _RequiredSchemaSummaryTypeDef = TypedDict(
     "_RequiredSchemaSummaryTypeDef",
     {
         "name": str,
         "type": Literal["TABLE"],
         "creatorAccountId": str,
         "createTime": datetime,
@@ -799,44 +707,24 @@
     "_OptionalSchemaSummaryTypeDef",
     {
         "analysisMethod": Literal["DIRECT_QUERY"],
     },
     total=False,
 )
 
-
 class SchemaSummaryTypeDef(_RequiredSchemaSummaryTypeDef, _OptionalSchemaSummaryTypeDef):
     pass
 
-
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
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
 ProtectedQueryErrorTypeDef = TypedDict(
     "ProtectedQueryErrorTypeDef",
     {
         "message": str,
         "code": str,
     },
 )
@@ -852,22 +740,20 @@
     "_OptionalProtectedQueryS3OutputConfigurationTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
-
 class ProtectedQueryS3OutputConfigurationTypeDef(
     _RequiredProtectedQueryS3OutputConfigurationTypeDef,
     _OptionalProtectedQueryS3OutputConfigurationTypeDef,
 ):
     pass
 
-
 ProtectedQueryS3OutputTypeDef = TypedDict(
     "ProtectedQueryS3OutputTypeDef",
     {
         "location": str,
     },
 )
 
@@ -882,25 +768,14 @@
     "ProtectedQueryStatisticsTypeDef",
     {
         "totalDurationInMillis": int,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -924,21 +799,19 @@
     {
         "name": str,
         "description": str,
     },
     total=False,
 )
 
-
 class UpdateCollaborationInputRequestTypeDef(
     _RequiredUpdateCollaborationInputRequestTypeDef, _OptionalUpdateCollaborationInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateConfiguredTableAssociationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateConfiguredTableAssociationInputRequestTypeDef",
     {
         "configuredTableAssociationIdentifier": str,
         "membershipIdentifier": str,
     },
 )
@@ -947,22 +820,20 @@
     {
         "description": str,
         "roleArn": str,
     },
     total=False,
 )
 
-
 class UpdateConfiguredTableAssociationInputRequestTypeDef(
     _RequiredUpdateConfiguredTableAssociationInputRequestTypeDef,
     _OptionalUpdateConfiguredTableAssociationInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateConfiguredTableInputRequestTypeDef = TypedDict(
     "_RequiredUpdateConfiguredTableInputRequestTypeDef",
     {
         "configuredTableIdentifier": str,
     },
 )
 _OptionalUpdateConfiguredTableInputRequestTypeDef = TypedDict(
@@ -970,52 +841,71 @@
     {
         "name": str,
         "description": str,
     },
     total=False,
 )
 
-
 class UpdateConfiguredTableInputRequestTypeDef(
     _RequiredUpdateConfiguredTableInputRequestTypeDef,
     _OptionalUpdateConfiguredTableInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateMembershipInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMembershipInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalUpdateMembershipInputRequestTypeDef = TypedDict(
     "_OptionalUpdateMembershipInputRequestTypeDef",
     {
         "queryLogStatus": MembershipQueryLogStatusType,
     },
     total=False,
 )
 
-
 class UpdateMembershipInputRequestTypeDef(
     _RequiredUpdateMembershipInputRequestTypeDef, _OptionalUpdateMembershipInputRequestTypeDef
 ):
     pass
 
-
 UpdateProtectedQueryInputRequestTypeDef = TypedDict(
     "UpdateProtectedQueryInputRequestTypeDef",
     {
         "membershipIdentifier": str,
         "protectedQueryIdentifier": str,
         "targetStatus": Literal["CANCELLED"],
     },
 )
 
+_RequiredAnalysisRuleAggregationOutputTypeDef = TypedDict(
+    "_RequiredAnalysisRuleAggregationOutputTypeDef",
+    {
+        "aggregateColumns": List[AggregateColumnOutputTypeDef],
+        "joinColumns": List[str],
+        "dimensionColumns": List[str],
+        "scalarFunctions": List[ScalarFunctionsType],
+        "outputConstraints": List[AggregationConstraintTypeDef],
+    },
+)
+_OptionalAnalysisRuleAggregationOutputTypeDef = TypedDict(
+    "_OptionalAnalysisRuleAggregationOutputTypeDef",
+    {
+        "joinRequired": Literal["QUERY_RUNNER"],
+    },
+    total=False,
+)
+
+class AnalysisRuleAggregationOutputTypeDef(
+    _RequiredAnalysisRuleAggregationOutputTypeDef, _OptionalAnalysisRuleAggregationOutputTypeDef
+):
+    pass
+
 _RequiredAnalysisRuleAggregationTypeDef = TypedDict(
     "_RequiredAnalysisRuleAggregationTypeDef",
     {
         "aggregateColumns": Sequence[AggregateColumnTypeDef],
         "joinColumns": Sequence[str],
         "dimensionColumns": Sequence[str],
         "scalarFunctions": Sequence[ScalarFunctionsType],
@@ -1026,27 +916,33 @@
     "_OptionalAnalysisRuleAggregationTypeDef",
     {
         "joinRequired": Literal["QUERY_RUNNER"],
     },
     total=False,
 )
 
-
 class AnalysisRuleAggregationTypeDef(
     _RequiredAnalysisRuleAggregationTypeDef, _OptionalAnalysisRuleAggregationTypeDef
 ):
     pass
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListCollaborationsOutputTypeDef = TypedDict(
     "ListCollaborationsOutputTypeDef",
     {
         "nextToken": str,
         "collaborationList": List[CollaborationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCollaborationTypeDef = TypedDict(
     "_RequiredCollaborationTypeDef",
     {
         "id": str,
@@ -1067,19 +963,17 @@
         "membershipId": str,
         "membershipArn": str,
         "dataEncryptionMetadata": DataEncryptionMetadataTypeDef,
     },
     total=False,
 )
 
-
 class CollaborationTypeDef(_RequiredCollaborationTypeDef, _OptionalCollaborationTypeDef):
     pass
 
-
 _RequiredSchemaTypeDef = TypedDict(
     "_RequiredSchemaTypeDef",
     {
         "columns": List[ColumnTypeDef],
         "partitionKeys": List[ColumnTypeDef],
         "analysisRuleTypes": List[AnalysisRuleTypeType],
         "creatorAccountId": str,
@@ -1096,58 +990,56 @@
     "_OptionalSchemaTypeDef",
     {
         "analysisMethod": Literal["DIRECT_QUERY"],
     },
     total=False,
 )
 
-
 class SchemaTypeDef(_RequiredSchemaTypeDef, _OptionalSchemaTypeDef):
     pass
 
-
 ListConfiguredTableAssociationsOutputTypeDef = TypedDict(
     "ListConfiguredTableAssociationsOutputTypeDef",
     {
         "configuredTableAssociationSummaries": List[ConfiguredTableAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConfiguredTableAssociationOutputTypeDef = TypedDict(
     "CreateConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConfiguredTableAssociationOutputTypeDef = TypedDict(
     "GetConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfiguredTableAssociationOutputTypeDef = TypedDict(
     "UpdateConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfiguredTablesOutputTypeDef = TypedDict(
     "ListConfiguredTablesOutputTypeDef",
     {
         "configuredTableSummaries": List[ConfiguredTableSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCollaborationInputRequestTypeDef = TypedDict(
     "_RequiredCreateCollaborationInputRequestTypeDef",
     {
         "members": Sequence[MemberSpecificationTypeDef],
@@ -1163,86 +1055,192 @@
     {
         "dataEncryptionMetadata": DataEncryptionMetadataTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateCollaborationInputRequestTypeDef(
     _RequiredCreateCollaborationInputRequestTypeDef, _OptionalCreateCollaborationInputRequestTypeDef
 ):
     pass
 
-
 CreateMembershipOutputTypeDef = TypedDict(
     "CreateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMembershipOutputTypeDef = TypedDict(
     "GetMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMembershipOutputTypeDef = TypedDict(
     "UpdateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TableReferenceTypeDef = TypedDict(
     "TableReferenceTypeDef",
     {
         "glue": GlueTableReferenceTypeDef,
     },
     total=False,
 )
 
+ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
+    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+    {
+        "memberStatus": FilterableMemberStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(
+    _RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+    _OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+):
+    pass
+
+ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef = TypedDict(
+    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMembersInputListMembersPaginateTypeDef = TypedDict(
+    "_RequiredListMembersInputListMembersPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListMembersInputListMembersPaginateTypeDef = TypedDict(
+    "_OptionalListMembersInputListMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMembersInputListMembersPaginateTypeDef(
+    _RequiredListMembersInputListMembersPaginateTypeDef,
+    _OptionalListMembersInputListMembersPaginateTypeDef,
+):
+    pass
+
+ListMembershipsInputListMembershipsPaginateTypeDef = TypedDict(
+    "ListMembershipsInputListMembershipsPaginateTypeDef",
+    {
+        "status": MembershipStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
+    "_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
+    "_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    {
+        "status": ProtectedQueryStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(
+    _RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+    _OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+):
+    pass
+
+_RequiredListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "schemaType": Literal["TABLE"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSchemasInputListSchemasPaginateTypeDef(
+    _RequiredListSchemasInputListSchemasPaginateTypeDef,
+    _OptionalListSchemasInputListSchemasPaginateTypeDef,
+):
+    pass
+
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "nextToken": str,
         "memberSummaries": List[MemberSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembershipsOutputTypeDef = TypedDict(
     "ListMembershipsOutputTypeDef",
     {
         "nextToken": str,
         "membershipSummaries": List[MembershipSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtectedQueriesOutputTypeDef = TypedDict(
     "ListProtectedQueriesOutputTypeDef",
     {
         "nextToken": str,
         "protectedQueries": List[ProtectedQuerySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemasOutputTypeDef = TypedDict(
     "ListSchemasOutputTypeDef",
     {
         "schemaSummaries": List[SchemaSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProtectedQueryOutputConfigurationTypeDef = TypedDict(
     "ProtectedQueryOutputConfigurationTypeDef",
     {
         "s3": ProtectedQueryS3OutputConfigurationTypeDef,
@@ -1257,16 +1255,25 @@
     },
     total=False,
 )
 
 AnalysisRulePolicyV1TypeDef = TypedDict(
     "AnalysisRulePolicyV1TypeDef",
     {
-        "list": AnalysisRuleListTypeDef,
-        "aggregation": AnalysisRuleAggregationTypeDef,
+        "list": AnalysisRuleListOutputTypeDef,
+        "aggregation": AnalysisRuleAggregationOutputTypeDef,
+    },
+    total=False,
+)
+
+ConfiguredTableAnalysisRulePolicyV1OutputTypeDef = TypedDict(
+    "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
+    {
+        "list": AnalysisRuleListOutputTypeDef,
+        "aggregation": AnalysisRuleAggregationOutputTypeDef,
     },
     total=False,
 )
 
 ConfiguredTableAnalysisRulePolicyV1TypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     {
@@ -1276,48 +1283,48 @@
     total=False,
 )
 
 CreateCollaborationOutputTypeDef = TypedDict(
     "CreateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCollaborationOutputTypeDef = TypedDict(
     "GetCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCollaborationOutputTypeDef = TypedDict(
     "UpdateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetSchemaOutputTypeDef = TypedDict(
     "BatchGetSchemaOutputTypeDef",
     {
         "schemas": List[SchemaTypeDef],
         "errors": List[BatchGetSchemaErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSchemaOutputTypeDef = TypedDict(
     "GetSchemaOutputTypeDef",
     {
         "schema": SchemaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConfiguredTableTypeDef = TypedDict(
     "_RequiredConfiguredTableTypeDef",
     {
         "id": str,
@@ -1335,19 +1342,17 @@
     "_OptionalConfiguredTableTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class ConfiguredTableTypeDef(_RequiredConfiguredTableTypeDef, _OptionalConfiguredTableTypeDef):
     pass
 
-
 _RequiredCreateConfiguredTableInputRequestTypeDef = TypedDict(
     "_RequiredCreateConfiguredTableInputRequestTypeDef",
     {
         "name": str,
         "tableReference": TableReferenceTypeDef,
         "allowedColumns": Sequence[str],
         "analysisMethod": Literal["DIRECT_QUERY"],
@@ -1358,22 +1363,20 @@
     {
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateConfiguredTableInputRequestTypeDef(
     _RequiredCreateConfiguredTableInputRequestTypeDef,
     _OptionalCreateConfiguredTableInputRequestTypeDef,
 ):
     pass
 
-
 ProtectedQueryResultConfigurationTypeDef = TypedDict(
     "ProtectedQueryResultConfigurationTypeDef",
     {
         "outputConfiguration": ProtectedQueryOutputConfigurationTypeDef,
     },
 )
 
@@ -1388,43 +1391,51 @@
     "AnalysisRulePolicyTypeDef",
     {
         "v1": AnalysisRulePolicyV1TypeDef,
     },
     total=False,
 )
 
+ConfiguredTableAnalysisRulePolicyOutputTypeDef = TypedDict(
+    "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
+    {
+        "v1": ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
+    },
+    total=False,
+)
+
 ConfiguredTableAnalysisRulePolicyTypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     {
         "v1": ConfiguredTableAnalysisRulePolicyV1TypeDef,
     },
     total=False,
 )
 
 CreateConfiguredTableOutputTypeDef = TypedDict(
     "CreateConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConfiguredTableOutputTypeDef = TypedDict(
     "GetConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfiguredTableOutputTypeDef = TypedDict(
     "UpdateConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartProtectedQueryInputRequestTypeDef = TypedDict(
     "StartProtectedQueryInputRequestTypeDef",
     {
         "type": Literal["SQL"],
@@ -1452,19 +1463,17 @@
         "statistics": ProtectedQueryStatisticsTypeDef,
         "result": ProtectedQueryResultTypeDef,
         "error": ProtectedQueryErrorTypeDef,
     },
     total=False,
 )
 
-
 class ProtectedQueryTypeDef(_RequiredProtectedQueryTypeDef, _OptionalProtectedQueryTypeDef):
     pass
 
-
 AnalysisRuleTypeDef = TypedDict(
     "AnalysisRuleTypeDef",
     {
         "collaborationId": str,
         "type": AnalysisRuleTypeType,
         "name": str,
         "createTime": datetime,
@@ -1474,21 +1483,24 @@
 )
 
 ConfiguredTableAnalysisRuleTypeDef = TypedDict(
     "ConfiguredTableAnalysisRuleTypeDef",
     {
         "configuredTableId": str,
         "configuredTableArn": str,
-        "policy": ConfiguredTableAnalysisRulePolicyTypeDef,
+        "policy": ConfiguredTableAnalysisRulePolicyOutputTypeDef,
         "type": ConfiguredTableAnalysisRuleTypeType,
         "createTime": datetime,
         "updateTime": datetime,
     },
 )
 
+ConfiguredTableAnalysisRulePolicyUnionTypeDef = Union[
+    ConfiguredTableAnalysisRulePolicyTypeDef, ConfiguredTableAnalysisRulePolicyOutputTypeDef
+]
 CreateConfiguredTableAnalysisRuleInputRequestTypeDef = TypedDict(
     "CreateConfiguredTableAnalysisRuleInputRequestTypeDef",
     {
         "configuredTableIdentifier": str,
         "analysisRuleType": ConfiguredTableAnalysisRuleTypeType,
         "analysisRulePolicy": ConfiguredTableAnalysisRulePolicyTypeDef,
     },
@@ -1503,58 +1515,58 @@
     },
 )
 
 GetProtectedQueryOutputTypeDef = TypedDict(
     "GetProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartProtectedQueryOutputTypeDef = TypedDict(
     "StartProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProtectedQueryOutputTypeDef = TypedDict(
     "UpdateProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSchemaAnalysisRuleOutputTypeDef = TypedDict(
     "GetSchemaAnalysisRuleOutputTypeDef",
     {
         "analysisRule": AnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "CreateConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "GetConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "UpdateConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms/type_defs.pyi` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for cleanrooms service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_cleanrooms.type_defs import AggregateColumnTypeDef
+    from types_aiobotocore_cleanrooms.type_defs import AggregateColumnOutputTypeDef
 
-    data: AggregateColumnTypeDef = {...}
+    data: AggregateColumnOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggregateFunctionNameType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
@@ -35,20 +35,24 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AggregateColumnOutputTypeDef",
     "AggregateColumnTypeDef",
     "AggregationConstraintTypeDef",
+    "AnalysisRuleListOutputTypeDef",
     "AnalysisRuleListTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CollaborationSummaryTypeDef",
     "DataEncryptionMetadataTypeDef",
     "ColumnTypeDef",
     "ConfiguredTableAssociationSummaryTypeDef",
     "ConfiguredTableAssociationTypeDef",
     "ConfiguredTableSummaryTypeDef",
     "MemberSpecificationTypeDef",
@@ -66,99 +70,110 @@
     "GetConfiguredTableAssociationInputRequestTypeDef",
     "GetConfiguredTableInputRequestTypeDef",
     "GetMembershipInputRequestTypeDef",
     "GetProtectedQueryInputRequestTypeDef",
     "GetSchemaAnalysisRuleInputRequestTypeDef",
     "GetSchemaInputRequestTypeDef",
     "GlueTableReferenceTypeDef",
-    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListCollaborationsInputRequestTypeDef",
-    "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
     "ListConfiguredTableAssociationsInputRequestTypeDef",
-    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
     "ListConfiguredTablesInputRequestTypeDef",
-    "ListMembersInputListMembersPaginateTypeDef",
     "ListMembersInputRequestTypeDef",
     "MemberSummaryTypeDef",
-    "ListMembershipsInputListMembershipsPaginateTypeDef",
     "ListMembershipsInputRequestTypeDef",
     "MembershipSummaryTypeDef",
-    "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
     "ListProtectedQueriesInputRequestTypeDef",
     "ProtectedQuerySummaryTypeDef",
-    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListSchemasInputRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ProtectedQueryErrorTypeDef",
     "ProtectedQueryS3OutputConfigurationTypeDef",
     "ProtectedQueryS3OutputTypeDef",
     "ProtectedQuerySQLParametersTypeDef",
     "ProtectedQueryStatisticsTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
+    "AnalysisRuleAggregationOutputTypeDef",
     "AnalysisRuleAggregationTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
     "GetConfiguredTableAssociationOutputTypeDef",
     "UpdateConfiguredTableAssociationOutputTypeDef",
     "ListConfiguredTablesOutputTypeDef",
     "CreateCollaborationInputRequestTypeDef",
     "CreateMembershipOutputTypeDef",
     "GetMembershipOutputTypeDef",
     "UpdateMembershipOutputTypeDef",
     "TableReferenceTypeDef",
+    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+    "ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
+    "ListMembersInputListMembersPaginateTypeDef",
+    "ListMembershipsInputListMembershipsPaginateTypeDef",
+    "ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    "ListSchemasInputListSchemasPaginateTypeDef",
     "ListMembersOutputTypeDef",
     "ListMembershipsOutputTypeDef",
     "ListProtectedQueriesOutputTypeDef",
     "ListSchemasOutputTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
+    "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     "CreateCollaborationOutputTypeDef",
     "GetCollaborationOutputTypeDef",
     "UpdateCollaborationOutputTypeDef",
     "BatchGetSchemaOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "ConfiguredTableTypeDef",
     "CreateConfiguredTableInputRequestTypeDef",
     "ProtectedQueryResultConfigurationTypeDef",
     "ProtectedQueryResultTypeDef",
     "AnalysisRulePolicyTypeDef",
+    "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     "CreateConfiguredTableOutputTypeDef",
     "GetConfiguredTableOutputTypeDef",
     "UpdateConfiguredTableOutputTypeDef",
     "StartProtectedQueryInputRequestTypeDef",
     "ProtectedQueryTypeDef",
     "AnalysisRuleTypeDef",
     "ConfiguredTableAnalysisRuleTypeDef",
+    "ConfiguredTableAnalysisRulePolicyUnionTypeDef",
     "CreateConfiguredTableAnalysisRuleInputRequestTypeDef",
     "UpdateConfiguredTableAnalysisRuleInputRequestTypeDef",
     "GetProtectedQueryOutputTypeDef",
     "StartProtectedQueryOutputTypeDef",
     "UpdateProtectedQueryOutputTypeDef",
     "GetSchemaAnalysisRuleOutputTypeDef",
     "CreateConfiguredTableAnalysisRuleOutputTypeDef",
     "GetConfiguredTableAnalysisRuleOutputTypeDef",
     "UpdateConfiguredTableAnalysisRuleOutputTypeDef",
 )
 
+AggregateColumnOutputTypeDef = TypedDict(
+    "AggregateColumnOutputTypeDef",
+    {
+        "columnNames": List[str],
+        "function": AggregateFunctionNameType,
+    },
+)
+
 AggregateColumnTypeDef = TypedDict(
     "AggregateColumnTypeDef",
     {
         "columnNames": Sequence[str],
         "function": AggregateFunctionNameType,
     },
 )
@@ -168,14 +183,22 @@
     {
         "columnName": str,
         "minimum": int,
         "type": Literal["COUNT_DISTINCT"],
     },
 )
 
+AnalysisRuleListOutputTypeDef = TypedDict(
+    "AnalysisRuleListOutputTypeDef",
+    {
+        "joinColumns": List[str],
+        "listColumns": List[str],
+    },
+)
+
 AnalysisRuleListTypeDef = TypedDict(
     "AnalysisRuleListTypeDef",
     {
         "joinColumns": Sequence[str],
         "listColumns": Sequence[str],
     },
 )
@@ -193,14 +216,25 @@
     "BatchGetSchemaInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "names": Sequence[str],
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
 _RequiredCollaborationSummaryTypeDef = TypedDict(
     "_RequiredCollaborationSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "creatorAccountId": str,
@@ -215,19 +249,21 @@
     {
         "membershipId": str,
         "membershipArn": str,
     },
     total=False,
 )
 
+
 class CollaborationSummaryTypeDef(
     _RequiredCollaborationSummaryTypeDef, _OptionalCollaborationSummaryTypeDef
 ):
     pass
 
+
 DataEncryptionMetadataTypeDef = TypedDict(
     "DataEncryptionMetadataTypeDef",
     {
         "allowCleartext": bool,
         "allowDuplicates": bool,
         "allowJoinsOnColumnsWithDifferentNames": bool,
         "preserveNulls": bool,
@@ -275,19 +311,21 @@
     "_OptionalConfiguredTableAssociationTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class ConfiguredTableAssociationTypeDef(
     _RequiredConfiguredTableAssociationTypeDef, _OptionalConfiguredTableAssociationTypeDef
 ):
     pass
 
+
 ConfiguredTableSummaryTypeDef = TypedDict(
     "ConfiguredTableSummaryTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "createTime": datetime,
@@ -320,20 +358,22 @@
     {
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateConfiguredTableAssociationInputRequestTypeDef(
     _RequiredCreateConfiguredTableAssociationInputRequestTypeDef,
     _OptionalCreateConfiguredTableAssociationInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateMembershipInputRequestTypeDef = TypedDict(
     "_RequiredCreateMembershipInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
         "queryLogStatus": MembershipQueryLogStatusType,
     },
 )
@@ -341,19 +381,21 @@
     "_OptionalCreateMembershipInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateMembershipInputRequestTypeDef(
     _RequiredCreateMembershipInputRequestTypeDef, _OptionalCreateMembershipInputRequestTypeDef
 ):
     pass
 
+
 MembershipTypeDef = TypedDict(
     "MembershipTypeDef",
     {
         "id": str,
         "arn": str,
         "collaborationArn": str,
         "collaborationId": str,
@@ -479,53 +521,34 @@
     "GlueTableReferenceTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
 
-ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
-    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "memberStatus": FilterableMemberStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListCollaborationsInputRequestTypeDef = TypedDict(
     "ListCollaborationsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "memberStatus": FilterableMemberStatusType,
     },
     total=False,
 )
 
-_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    {
-        "membershipIdentifier": str,
-    },
-)
-_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(
-    _RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-    _OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListConfiguredTableAssociationsInputRequestTypeDef = TypedDict(
     "_RequiredListConfiguredTableAssociationsInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalListConfiguredTableAssociationsInputRequestTypeDef = TypedDict(
@@ -533,57 +556,31 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListConfiguredTableAssociationsInputRequestTypeDef(
     _RequiredListConfiguredTableAssociationsInputRequestTypeDef,
     _OptionalListConfiguredTableAssociationsInputRequestTypeDef,
 ):
     pass
 
-ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef = TypedDict(
-    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListConfiguredTablesInputRequestTypeDef = TypedDict(
     "ListConfiguredTablesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListMembersInputListMembersPaginateTypeDef = TypedDict(
-    "_RequiredListMembersInputListMembersPaginateTypeDef",
-    {
-        "collaborationIdentifier": str,
-    },
-)
-_OptionalListMembersInputListMembersPaginateTypeDef = TypedDict(
-    "_OptionalListMembersInputListMembersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMembersInputListMembersPaginateTypeDef(
-    _RequiredListMembersInputListMembersPaginateTypeDef,
-    _OptionalListMembersInputListMembersPaginateTypeDef,
-):
-    pass
-
 _RequiredListMembersInputRequestTypeDef = TypedDict(
     "_RequiredListMembersInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalListMembersInputRequestTypeDef = TypedDict(
@@ -591,19 +588,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListMembersInputRequestTypeDef(
     _RequiredListMembersInputRequestTypeDef, _OptionalListMembersInputRequestTypeDef
 ):
     pass
 
+
 _RequiredMemberSummaryTypeDef = TypedDict(
     "_RequiredMemberSummaryTypeDef",
     {
         "accountId": str,
         "status": MemberStatusType,
         "displayName": str,
         "abilities": List[MemberAbilityType],
@@ -616,25 +615,18 @@
     {
         "membershipId": str,
         "membershipArn": str,
     },
     total=False,
 )
 
+
 class MemberSummaryTypeDef(_RequiredMemberSummaryTypeDef, _OptionalMemberSummaryTypeDef):
     pass
 
-ListMembershipsInputListMembershipsPaginateTypeDef = TypedDict(
-    "ListMembershipsInputListMembershipsPaginateTypeDef",
-    {
-        "status": MembershipStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListMembershipsInputRequestTypeDef = TypedDict(
     "ListMembershipsInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": MembershipStatusType,
@@ -655,35 +647,14 @@
         "createTime": datetime,
         "updateTime": datetime,
         "status": MembershipStatusType,
         "memberAbilities": List[MemberAbilityType],
     },
 )
 
-_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
-    "_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    {
-        "membershipIdentifier": str,
-    },
-)
-_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
-    "_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
-    {
-        "status": ProtectedQueryStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(
-    _RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-    _OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
-):
-    pass
-
 _RequiredListProtectedQueriesInputRequestTypeDef = TypedDict(
     "_RequiredListProtectedQueriesInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalListProtectedQueriesInputRequestTypeDef = TypedDict(
@@ -692,52 +663,33 @@
         "status": ProtectedQueryStatusType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListProtectedQueriesInputRequestTypeDef(
     _RequiredListProtectedQueriesInputRequestTypeDef,
     _OptionalListProtectedQueriesInputRequestTypeDef,
 ):
     pass
 
+
 ProtectedQuerySummaryTypeDef = TypedDict(
     "ProtectedQuerySummaryTypeDef",
     {
         "id": str,
         "membershipId": str,
         "membershipArn": str,
         "createTime": datetime,
         "status": ProtectedQueryStatusType,
     },
 )
 
-_RequiredListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "collaborationIdentifier": str,
-    },
-)
-_OptionalListSchemasInputListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasInputListSchemasPaginateTypeDef",
-    {
-        "schemaType": Literal["TABLE"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSchemasInputListSchemasPaginateTypeDef(
-    _RequiredListSchemasInputListSchemasPaginateTypeDef,
-    _OptionalListSchemasInputListSchemasPaginateTypeDef,
-):
-    pass
-
 _RequiredListSchemasInputRequestTypeDef = TypedDict(
     "_RequiredListSchemasInputRequestTypeDef",
     {
         "collaborationIdentifier": str,
     },
 )
 _OptionalListSchemasInputRequestTypeDef = TypedDict(
@@ -746,19 +698,21 @@
         "schemaType": Literal["TABLE"],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListSchemasInputRequestTypeDef(
     _RequiredListSchemasInputRequestTypeDef, _OptionalListSchemasInputRequestTypeDef
 ):
     pass
 
+
 _RequiredSchemaSummaryTypeDef = TypedDict(
     "_RequiredSchemaSummaryTypeDef",
     {
         "name": str,
         "type": Literal["TABLE"],
         "creatorAccountId": str,
         "createTime": datetime,
@@ -772,42 +726,26 @@
     "_OptionalSchemaSummaryTypeDef",
     {
         "analysisMethod": Literal["DIRECT_QUERY"],
     },
     total=False,
 )
 
+
 class SchemaSummaryTypeDef(_RequiredSchemaSummaryTypeDef, _OptionalSchemaSummaryTypeDef):
     pass
 
+
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
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
 ProtectedQueryErrorTypeDef = TypedDict(
     "ProtectedQueryErrorTypeDef",
     {
         "message": str,
         "code": str,
     },
 )
@@ -823,20 +761,22 @@
     "_OptionalProtectedQueryS3OutputConfigurationTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
+
 class ProtectedQueryS3OutputConfigurationTypeDef(
     _RequiredProtectedQueryS3OutputConfigurationTypeDef,
     _OptionalProtectedQueryS3OutputConfigurationTypeDef,
 ):
     pass
 
+
 ProtectedQueryS3OutputTypeDef = TypedDict(
     "ProtectedQueryS3OutputTypeDef",
     {
         "location": str,
     },
 )
 
@@ -851,25 +791,14 @@
     "ProtectedQueryStatisticsTypeDef",
     {
         "totalDurationInMillis": int,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -893,19 +822,21 @@
     {
         "name": str,
         "description": str,
     },
     total=False,
 )
 
+
 class UpdateCollaborationInputRequestTypeDef(
     _RequiredUpdateCollaborationInputRequestTypeDef, _OptionalUpdateCollaborationInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateConfiguredTableAssociationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateConfiguredTableAssociationInputRequestTypeDef",
     {
         "configuredTableAssociationIdentifier": str,
         "membershipIdentifier": str,
     },
 )
@@ -914,20 +845,22 @@
     {
         "description": str,
         "roleArn": str,
     },
     total=False,
 )
 
+
 class UpdateConfiguredTableAssociationInputRequestTypeDef(
     _RequiredUpdateConfiguredTableAssociationInputRequestTypeDef,
     _OptionalUpdateConfiguredTableAssociationInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateConfiguredTableInputRequestTypeDef = TypedDict(
     "_RequiredUpdateConfiguredTableInputRequestTypeDef",
     {
         "configuredTableIdentifier": str,
     },
 )
 _OptionalUpdateConfiguredTableInputRequestTypeDef = TypedDict(
@@ -935,48 +868,77 @@
     {
         "name": str,
         "description": str,
     },
     total=False,
 )
 
+
 class UpdateConfiguredTableInputRequestTypeDef(
     _RequiredUpdateConfiguredTableInputRequestTypeDef,
     _OptionalUpdateConfiguredTableInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateMembershipInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMembershipInputRequestTypeDef",
     {
         "membershipIdentifier": str,
     },
 )
 _OptionalUpdateMembershipInputRequestTypeDef = TypedDict(
     "_OptionalUpdateMembershipInputRequestTypeDef",
     {
         "queryLogStatus": MembershipQueryLogStatusType,
     },
     total=False,
 )
 
+
 class UpdateMembershipInputRequestTypeDef(
     _RequiredUpdateMembershipInputRequestTypeDef, _OptionalUpdateMembershipInputRequestTypeDef
 ):
     pass
 
+
 UpdateProtectedQueryInputRequestTypeDef = TypedDict(
     "UpdateProtectedQueryInputRequestTypeDef",
     {
         "membershipIdentifier": str,
         "protectedQueryIdentifier": str,
         "targetStatus": Literal["CANCELLED"],
     },
 )
 
+_RequiredAnalysisRuleAggregationOutputTypeDef = TypedDict(
+    "_RequiredAnalysisRuleAggregationOutputTypeDef",
+    {
+        "aggregateColumns": List[AggregateColumnOutputTypeDef],
+        "joinColumns": List[str],
+        "dimensionColumns": List[str],
+        "scalarFunctions": List[ScalarFunctionsType],
+        "outputConstraints": List[AggregationConstraintTypeDef],
+    },
+)
+_OptionalAnalysisRuleAggregationOutputTypeDef = TypedDict(
+    "_OptionalAnalysisRuleAggregationOutputTypeDef",
+    {
+        "joinRequired": Literal["QUERY_RUNNER"],
+    },
+    total=False,
+)
+
+
+class AnalysisRuleAggregationOutputTypeDef(
+    _RequiredAnalysisRuleAggregationOutputTypeDef, _OptionalAnalysisRuleAggregationOutputTypeDef
+):
+    pass
+
+
 _RequiredAnalysisRuleAggregationTypeDef = TypedDict(
     "_RequiredAnalysisRuleAggregationTypeDef",
     {
         "aggregateColumns": Sequence[AggregateColumnTypeDef],
         "joinColumns": Sequence[str],
         "dimensionColumns": Sequence[str],
         "scalarFunctions": Sequence[ScalarFunctionsType],
@@ -987,25 +949,35 @@
     "_OptionalAnalysisRuleAggregationTypeDef",
     {
         "joinRequired": Literal["QUERY_RUNNER"],
     },
     total=False,
 )
 
+
 class AnalysisRuleAggregationTypeDef(
     _RequiredAnalysisRuleAggregationTypeDef, _OptionalAnalysisRuleAggregationTypeDef
 ):
     pass
 
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCollaborationsOutputTypeDef = TypedDict(
     "ListCollaborationsOutputTypeDef",
     {
         "nextToken": str,
         "collaborationList": List[CollaborationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCollaborationTypeDef = TypedDict(
     "_RequiredCollaborationTypeDef",
     {
         "id": str,
@@ -1026,17 +998,19 @@
         "membershipId": str,
         "membershipArn": str,
         "dataEncryptionMetadata": DataEncryptionMetadataTypeDef,
     },
     total=False,
 )
 
+
 class CollaborationTypeDef(_RequiredCollaborationTypeDef, _OptionalCollaborationTypeDef):
     pass
 
+
 _RequiredSchemaTypeDef = TypedDict(
     "_RequiredSchemaTypeDef",
     {
         "columns": List[ColumnTypeDef],
         "partitionKeys": List[ColumnTypeDef],
         "analysisRuleTypes": List[AnalysisRuleTypeType],
         "creatorAccountId": str,
@@ -1053,56 +1027,58 @@
     "_OptionalSchemaTypeDef",
     {
         "analysisMethod": Literal["DIRECT_QUERY"],
     },
     total=False,
 )
 
+
 class SchemaTypeDef(_RequiredSchemaTypeDef, _OptionalSchemaTypeDef):
     pass
 
+
 ListConfiguredTableAssociationsOutputTypeDef = TypedDict(
     "ListConfiguredTableAssociationsOutputTypeDef",
     {
         "configuredTableAssociationSummaries": List[ConfiguredTableAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConfiguredTableAssociationOutputTypeDef = TypedDict(
     "CreateConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConfiguredTableAssociationOutputTypeDef = TypedDict(
     "GetConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfiguredTableAssociationOutputTypeDef = TypedDict(
     "UpdateConfiguredTableAssociationOutputTypeDef",
     {
         "configuredTableAssociation": ConfiguredTableAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfiguredTablesOutputTypeDef = TypedDict(
     "ListConfiguredTablesOutputTypeDef",
     {
         "configuredTableSummaries": List[ConfiguredTableSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCollaborationInputRequestTypeDef = TypedDict(
     "_RequiredCreateCollaborationInputRequestTypeDef",
     {
         "members": Sequence[MemberSpecificationTypeDef],
@@ -1118,84 +1094,202 @@
     {
         "dataEncryptionMetadata": DataEncryptionMetadataTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateCollaborationInputRequestTypeDef(
     _RequiredCreateCollaborationInputRequestTypeDef, _OptionalCreateCollaborationInputRequestTypeDef
 ):
     pass
 
+
 CreateMembershipOutputTypeDef = TypedDict(
     "CreateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMembershipOutputTypeDef = TypedDict(
     "GetMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMembershipOutputTypeDef = TypedDict(
     "UpdateMembershipOutputTypeDef",
     {
         "membership": MembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TableReferenceTypeDef = TypedDict(
     "TableReferenceTypeDef",
     {
         "glue": GlueTableReferenceTypeDef,
     },
     total=False,
 )
 
+ListCollaborationsInputListCollaborationsPaginateTypeDef = TypedDict(
+    "ListCollaborationsInputListCollaborationsPaginateTypeDef",
+    {
+        "memberStatus": FilterableMemberStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef(
+    _RequiredListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+    _OptionalListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+):
+    pass
+
+
+ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef = TypedDict(
+    "ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMembersInputListMembersPaginateTypeDef = TypedDict(
+    "_RequiredListMembersInputListMembersPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListMembersInputListMembersPaginateTypeDef = TypedDict(
+    "_OptionalListMembersInputListMembersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMembersInputListMembersPaginateTypeDef(
+    _RequiredListMembersInputListMembersPaginateTypeDef,
+    _OptionalListMembersInputListMembersPaginateTypeDef,
+):
+    pass
+
+
+ListMembershipsInputListMembershipsPaginateTypeDef = TypedDict(
+    "ListMembershipsInputListMembershipsPaginateTypeDef",
+    {
+        "status": MembershipStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
+    "_RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    {
+        "membershipIdentifier": str,
+    },
+)
+_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef = TypedDict(
+    "_OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef",
+    {
+        "status": ProtectedQueryStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef(
+    _RequiredListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+    _OptionalListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "collaborationIdentifier": str,
+    },
+)
+_OptionalListSchemasInputListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasInputListSchemasPaginateTypeDef",
+    {
+        "schemaType": Literal["TABLE"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSchemasInputListSchemasPaginateTypeDef(
+    _RequiredListSchemasInputListSchemasPaginateTypeDef,
+    _OptionalListSchemasInputListSchemasPaginateTypeDef,
+):
+    pass
+
+
 ListMembersOutputTypeDef = TypedDict(
     "ListMembersOutputTypeDef",
     {
         "nextToken": str,
         "memberSummaries": List[MemberSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembershipsOutputTypeDef = TypedDict(
     "ListMembershipsOutputTypeDef",
     {
         "nextToken": str,
         "membershipSummaries": List[MembershipSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtectedQueriesOutputTypeDef = TypedDict(
     "ListProtectedQueriesOutputTypeDef",
     {
         "nextToken": str,
         "protectedQueries": List[ProtectedQuerySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemasOutputTypeDef = TypedDict(
     "ListSchemasOutputTypeDef",
     {
         "schemaSummaries": List[SchemaSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProtectedQueryOutputConfigurationTypeDef = TypedDict(
     "ProtectedQueryOutputConfigurationTypeDef",
     {
         "s3": ProtectedQueryS3OutputConfigurationTypeDef,
@@ -1210,16 +1304,25 @@
     },
     total=False,
 )
 
 AnalysisRulePolicyV1TypeDef = TypedDict(
     "AnalysisRulePolicyV1TypeDef",
     {
-        "list": AnalysisRuleListTypeDef,
-        "aggregation": AnalysisRuleAggregationTypeDef,
+        "list": AnalysisRuleListOutputTypeDef,
+        "aggregation": AnalysisRuleAggregationOutputTypeDef,
+    },
+    total=False,
+)
+
+ConfiguredTableAnalysisRulePolicyV1OutputTypeDef = TypedDict(
+    "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
+    {
+        "list": AnalysisRuleListOutputTypeDef,
+        "aggregation": AnalysisRuleAggregationOutputTypeDef,
     },
     total=False,
 )
 
 ConfiguredTableAnalysisRulePolicyV1TypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     {
@@ -1229,48 +1332,48 @@
     total=False,
 )
 
 CreateCollaborationOutputTypeDef = TypedDict(
     "CreateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCollaborationOutputTypeDef = TypedDict(
     "GetCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCollaborationOutputTypeDef = TypedDict(
     "UpdateCollaborationOutputTypeDef",
     {
         "collaboration": CollaborationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetSchemaOutputTypeDef = TypedDict(
     "BatchGetSchemaOutputTypeDef",
     {
         "schemas": List[SchemaTypeDef],
         "errors": List[BatchGetSchemaErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSchemaOutputTypeDef = TypedDict(
     "GetSchemaOutputTypeDef",
     {
         "schema": SchemaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConfiguredTableTypeDef = TypedDict(
     "_RequiredConfiguredTableTypeDef",
     {
         "id": str,
@@ -1288,17 +1391,19 @@
     "_OptionalConfiguredTableTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class ConfiguredTableTypeDef(_RequiredConfiguredTableTypeDef, _OptionalConfiguredTableTypeDef):
     pass
 
+
 _RequiredCreateConfiguredTableInputRequestTypeDef = TypedDict(
     "_RequiredCreateConfiguredTableInputRequestTypeDef",
     {
         "name": str,
         "tableReference": TableReferenceTypeDef,
         "allowedColumns": Sequence[str],
         "analysisMethod": Literal["DIRECT_QUERY"],
@@ -1309,20 +1414,22 @@
     {
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateConfiguredTableInputRequestTypeDef(
     _RequiredCreateConfiguredTableInputRequestTypeDef,
     _OptionalCreateConfiguredTableInputRequestTypeDef,
 ):
     pass
 
+
 ProtectedQueryResultConfigurationTypeDef = TypedDict(
     "ProtectedQueryResultConfigurationTypeDef",
     {
         "outputConfiguration": ProtectedQueryOutputConfigurationTypeDef,
     },
 )
 
@@ -1337,43 +1444,51 @@
     "AnalysisRulePolicyTypeDef",
     {
         "v1": AnalysisRulePolicyV1TypeDef,
     },
     total=False,
 )
 
+ConfiguredTableAnalysisRulePolicyOutputTypeDef = TypedDict(
+    "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
+    {
+        "v1": ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
+    },
+    total=False,
+)
+
 ConfiguredTableAnalysisRulePolicyTypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     {
         "v1": ConfiguredTableAnalysisRulePolicyV1TypeDef,
     },
     total=False,
 )
 
 CreateConfiguredTableOutputTypeDef = TypedDict(
     "CreateConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConfiguredTableOutputTypeDef = TypedDict(
     "GetConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfiguredTableOutputTypeDef = TypedDict(
     "UpdateConfiguredTableOutputTypeDef",
     {
         "configuredTable": ConfiguredTableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartProtectedQueryInputRequestTypeDef = TypedDict(
     "StartProtectedQueryInputRequestTypeDef",
     {
         "type": Literal["SQL"],
@@ -1401,17 +1516,19 @@
         "statistics": ProtectedQueryStatisticsTypeDef,
         "result": ProtectedQueryResultTypeDef,
         "error": ProtectedQueryErrorTypeDef,
     },
     total=False,
 )
 
+
 class ProtectedQueryTypeDef(_RequiredProtectedQueryTypeDef, _OptionalProtectedQueryTypeDef):
     pass
 
+
 AnalysisRuleTypeDef = TypedDict(
     "AnalysisRuleTypeDef",
     {
         "collaborationId": str,
         "type": AnalysisRuleTypeType,
         "name": str,
         "createTime": datetime,
@@ -1421,21 +1538,24 @@
 )
 
 ConfiguredTableAnalysisRuleTypeDef = TypedDict(
     "ConfiguredTableAnalysisRuleTypeDef",
     {
         "configuredTableId": str,
         "configuredTableArn": str,
-        "policy": ConfiguredTableAnalysisRulePolicyTypeDef,
+        "policy": ConfiguredTableAnalysisRulePolicyOutputTypeDef,
         "type": ConfiguredTableAnalysisRuleTypeType,
         "createTime": datetime,
         "updateTime": datetime,
     },
 )
 
+ConfiguredTableAnalysisRulePolicyUnionTypeDef = Union[
+    ConfiguredTableAnalysisRulePolicyTypeDef, ConfiguredTableAnalysisRulePolicyOutputTypeDef
+]
 CreateConfiguredTableAnalysisRuleInputRequestTypeDef = TypedDict(
     "CreateConfiguredTableAnalysisRuleInputRequestTypeDef",
     {
         "configuredTableIdentifier": str,
         "analysisRuleType": ConfiguredTableAnalysisRuleTypeType,
         "analysisRulePolicy": ConfiguredTableAnalysisRulePolicyTypeDef,
     },
@@ -1450,58 +1570,58 @@
     },
 )
 
 GetProtectedQueryOutputTypeDef = TypedDict(
     "GetProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartProtectedQueryOutputTypeDef = TypedDict(
     "StartProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProtectedQueryOutputTypeDef = TypedDict(
     "UpdateProtectedQueryOutputTypeDef",
     {
         "protectedQuery": ProtectedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSchemaAnalysisRuleOutputTypeDef = TypedDict(
     "GetSchemaAnalysisRuleOutputTypeDef",
     {
         "analysisRule": AnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "CreateConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "GetConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConfiguredTableAnalysisRuleOutputTypeDef = TypedDict(
     "UpdateConfiguredTableAnalysisRuleOutputTypeDef",
     {
         "analysisRule": ConfiguredTableAnalysisRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms.egg-info/PKG-INFO` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cleanrooms
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CleanRoomsService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CleanRoomsService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cleanrooms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cleanrooms type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cleanrooms"></a>
 
 # types-aiobotocore-cleanrooms
 
 [![PyPI - types-aiobotocore-cleanrooms](https://img.shields.io/pypi/v/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cleanrooms?color=blue)](https://pypistats.org/packages/types-aiobotocore-cleanrooms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cleanrooms)](https://pepy.tech/project/types-aiobotocore-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CleanRoomsService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [types-aiobotocore-cleanrooms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/).
 
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
@@ -351,28 +350,31 @@
 )
 
 
 def check_value(value: AggregateFunctionNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cleanrooms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cleanrooms.type_defs import (
+    AggregateColumnOutputTypeDef,
     AggregateColumnTypeDef,
     AggregationConstraintTypeDef,
+    AnalysisRuleListOutputTypeDef,
     AnalysisRuleListTypeDef,
     BatchGetSchemaErrorTypeDef,
     BatchGetSchemaInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     CollaborationSummaryTypeDef,
     DataEncryptionMetadataTypeDef,
     ColumnTypeDef,
     ConfiguredTableAssociationSummaryTypeDef,
     ConfiguredTableAssociationTypeDef,
     ConfiguredTableSummaryTypeDef,
     MemberSpecificationTypeDef,
@@ -390,101 +392,104 @@
     GetConfiguredTableAssociationInputRequestTypeDef,
     GetConfiguredTableInputRequestTypeDef,
     GetMembershipInputRequestTypeDef,
     GetProtectedQueryInputRequestTypeDef,
     GetSchemaAnalysisRuleInputRequestTypeDef,
     GetSchemaInputRequestTypeDef,
     GlueTableReferenceTypeDef,
-    ListCollaborationsInputListCollaborationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCollaborationsInputRequestTypeDef,
-    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
     ListConfiguredTableAssociationsInputRequestTypeDef,
-    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
     ListConfiguredTablesInputRequestTypeDef,
-    ListMembersInputListMembersPaginateTypeDef,
     ListMembersInputRequestTypeDef,
     MemberSummaryTypeDef,
-    ListMembershipsInputListMembershipsPaginateTypeDef,
     ListMembershipsInputRequestTypeDef,
     MembershipSummaryTypeDef,
-    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
     ListProtectedQueriesInputRequestTypeDef,
     ProtectedQuerySummaryTypeDef,
-    ListSchemasInputListSchemasPaginateTypeDef,
     ListSchemasInputRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
     ProtectedQueryErrorTypeDef,
     ProtectedQueryS3OutputConfigurationTypeDef,
     ProtectedQueryS3OutputTypeDef,
     ProtectedQuerySQLParametersTypeDef,
     ProtectedQueryStatisticsTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCollaborationInputRequestTypeDef,
     UpdateConfiguredTableAssociationInputRequestTypeDef,
     UpdateConfiguredTableInputRequestTypeDef,
     UpdateMembershipInputRequestTypeDef,
     UpdateProtectedQueryInputRequestTypeDef,
+    AnalysisRuleAggregationOutputTypeDef,
     AnalysisRuleAggregationTypeDef,
+    ListTagsForResourceOutputTypeDef,
     ListCollaborationsOutputTypeDef,
     CollaborationTypeDef,
     SchemaTypeDef,
     ListConfiguredTableAssociationsOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     GetConfiguredTableAssociationOutputTypeDef,
     UpdateConfiguredTableAssociationOutputTypeDef,
     ListConfiguredTablesOutputTypeDef,
     CreateCollaborationInputRequestTypeDef,
     CreateMembershipOutputTypeDef,
     GetMembershipOutputTypeDef,
     UpdateMembershipOutputTypeDef,
     TableReferenceTypeDef,
+    ListCollaborationsInputListCollaborationsPaginateTypeDef,
+    ListConfiguredTableAssociationsInputListConfiguredTableAssociationsPaginateTypeDef,
+    ListConfiguredTablesInputListConfiguredTablesPaginateTypeDef,
+    ListMembersInputListMembersPaginateTypeDef,
+    ListMembershipsInputListMembershipsPaginateTypeDef,
+    ListProtectedQueriesInputListProtectedQueriesPaginateTypeDef,
+    ListSchemasInputListSchemasPaginateTypeDef,
     ListMembersOutputTypeDef,
     ListMembershipsOutputTypeDef,
     ListProtectedQueriesOutputTypeDef,
     ListSchemasOutputTypeDef,
     ProtectedQueryOutputConfigurationTypeDef,
     ProtectedQueryOutputTypeDef,
     AnalysisRulePolicyV1TypeDef,
+    ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
     ConfiguredTableAnalysisRulePolicyV1TypeDef,
     CreateCollaborationOutputTypeDef,
     GetCollaborationOutputTypeDef,
     UpdateCollaborationOutputTypeDef,
     BatchGetSchemaOutputTypeDef,
     GetSchemaOutputTypeDef,
     ConfiguredTableTypeDef,
     CreateConfiguredTableInputRequestTypeDef,
     ProtectedQueryResultConfigurationTypeDef,
     ProtectedQueryResultTypeDef,
     AnalysisRulePolicyTypeDef,
+    ConfiguredTableAnalysisRulePolicyOutputTypeDef,
     ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateConfiguredTableOutputTypeDef,
     GetConfiguredTableOutputTypeDef,
     UpdateConfiguredTableOutputTypeDef,
     StartProtectedQueryInputRequestTypeDef,
     ProtectedQueryTypeDef,
     AnalysisRuleTypeDef,
     ConfiguredTableAnalysisRuleTypeDef,
+    ConfiguredTableAnalysisRulePolicyUnionTypeDef,
     CreateConfiguredTableAnalysisRuleInputRequestTypeDef,
     UpdateConfiguredTableAnalysisRuleInputRequestTypeDef,
     GetProtectedQueryOutputTypeDef,
     StartProtectedQueryOutputTypeDef,
     UpdateProtectedQueryOutputTypeDef,
     GetSchemaAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     GetConfiguredTableAnalysisRuleOutputTypeDef,
     UpdateConfiguredTableAnalysisRuleOutputTypeDef,
 )
 
 
-def get_structure() -> AggregateColumnTypeDef:
+def get_value() -> AggregateColumnOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt` & `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt`

 * *Files identical despite different names*


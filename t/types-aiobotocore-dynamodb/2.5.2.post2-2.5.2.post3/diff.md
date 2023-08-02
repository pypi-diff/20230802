# Comparing `tmp/types-aiobotocore-dynamodb-2.5.2.post2.tar.gz` & `tmp/types-aiobotocore-dynamodb-2.5.2.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dynamodb-2.5.2.post2.tar", last modified: Sun Jul 16 12:49:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-dynamodb-2.5.2.post3.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
```

## Comparing `types-aiobotocore-dynamodb-2.5.2.post2.tar` & `types-aiobotocore-dynamodb-2.5.2.post3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-16 12:49:57.917694 types-aiobotocore-dynamodb-2.5.2.post2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-07-16 12:47:33.000000 types-aiobotocore-dynamodb-2.5.2.post2/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29495 2023-07-16 12:49:57.917694 types-aiobotocore-dynamodb-2.5.2.post2/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)    27920 2023-07-16 12:49:24.000000 types-aiobotocore-dynamodb-2.5.2.post2/README.md
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-07-16 12:49:57.917694 types-aiobotocore-dynamodb-2.5.2.post2/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2131 2023-07-16 12:49:24.000000 types-aiobotocore-dynamodb-2.5.2.post2/setup.py
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-16 12:49:57.917694 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1813 2023-07-16 12:47:33.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1812 2023-07-16 12:47:33.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-07-16 12:49:24.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    56380 2023-07-16 12:49:25.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    56311 2023-07-16 12:49:25.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12866 2023-07-16 12:49:26.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    12864 2023-07-16 12:49:26.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8705 2023-07-16 12:47:34.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     8698 2023-07-16 12:47:34.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-07-16 12:47:33.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29455 2023-07-16 12:49:25.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/service_resource.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29426 2023-07-16 12:49:25.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/service_resource.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)   151607 2023-07-16 12:49:30.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   151470 2023-07-16 12:49:28.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-07-16 12:49:24.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2442 2023-07-16 12:47:35.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     2440 2023-07-16 12:47:34.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-16 12:49:57.917694 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    29495 2023-07-16 12:49:57.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1002 2023-07-16 12:49:57.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-16 12:49:57.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-07-16 12:49:57.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-07-16 12:49:57.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-07-16 12:49:57.000000 types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.249600 types-aiobotocore-dynamodb-2.5.2.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26301 2023-08-02 14:52:12.241600 types-aiobotocore-dynamodb-2.5.2.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24779 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.249600 types-aiobotocore-dynamodb-2.5.2.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.237600 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50026 2023-08-02 14:36:50.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49957 2023-08-02 14:36:50.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-08-02 14:36:51.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-08-02 14:36:51.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-08-02 14:36:51.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-08-02 14:36:51.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23950 2023-08-02 14:36:50.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23921 2023-08-02 14:36:50.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   104451 2023-08-02 14:36:53.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104312 2023-08-02 14:36:52.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:49.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-02 14:36:51.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-08-02 14:36:51.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.241600 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26301 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/LICENSE` & `types-aiobotocore-dynamodb-2.5.2.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/PKG-INFO` & `types-aiobotocore-dynamodb-2.5.2.post3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-dynamodb
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.15.0
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore dynamodb type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-dynamodb"></a>
 
 # types-aiobotocore-dynamodb
 
 [![PyPI - types-aiobotocore-dynamodb](https://img.shields.io/pypi/v/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dynamodb?color=blue)](https://pypistats.org/packages/types-aiobotocore-dynamodb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodb)](https://pepy.tech/project/types-aiobotocore-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DynamoDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-dynamodb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +45,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -448,83 +415,54 @@
 )
 
 
 def check_value(value: AttributeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_dynamodb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_dynamodb.type_defs import (
     ResponseMetadataTypeDef,
-    ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
-    AttributeDefinitionOutputTypeDef,
-    AttributeDefinitionServiceResourceTypeDef,
-    AttributeDefinitionTableOutputTypeDef,
-    AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
-    AttributeValueServiceResourceTypeDef,
-    AttributeValueTableTypeDef,
     AttributeValueTypeDef,
-    AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
-    BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
-    KeysAndAttributesServiceResourceTypeDef,
-    KeysAndAttributesServiceResourceOutputTypeDef,
+    TableAttributeValueTypeDef,
     BatchStatementErrorTypeDef,
-    ItemCollectionMetricsServiceResourceTypeDef,
-    BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
-    CapacityServiceResourceTypeDef,
-    CapacityTableTypeDef,
     CapacityTypeDef,
-    ConditionTableTypeDef,
+    ConditionBaseImportTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
     ContributorInsightsSummaryTypeDef,
     CreateBackupInputRequestTypeDef,
-    KeySchemaElementTableTypeDef,
-    ProjectionTableTypeDef,
-    ProvisionedThroughputTableTypeDef,
     KeySchemaElementTypeDef,
     ProjectionTypeDef,
     ProvisionedThroughputTypeDef,
     ReplicaTypeDef,
     CreateReplicaActionTypeDef,
-    ProvisionedThroughputOverrideTableTypeDef,
     ProvisionedThroughputOverrideTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationTypeDef,
     TagTypeDef,
-    KeySchemaElementServiceResourceTypeDef,
-    ProvisionedThroughputServiceResourceTypeDef,
-    SSESpecificationServiceResourceTypeDef,
-    StreamSpecificationServiceResourceTypeDef,
-    TagServiceResourceTypeDef,
     CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
     DeleteBackupInputRequestTypeDef,
-    DeleteGlobalSecondaryIndexActionTableTypeDef,
     DeleteGlobalSecondaryIndexActionTypeDef,
-    ExpectedAttributeValueTableTypeDef,
-    ItemCollectionMetricsTableTypeDef,
     DeleteReplicaActionTypeDef,
-    DeleteReplicationGroupMemberActionTableTypeDef,
     DeleteReplicationGroupMemberActionTypeDef,
-    DeleteRequestServiceResourceOutputTypeDef,
-    DeleteRequestServiceResourceTypeDef,
     DeleteTableInputRequestTypeDef,
     DescribeBackupInputRequestTypeDef,
     DescribeContinuousBackupsInputRequestTypeDef,
     DescribeContributorInsightsInputRequestTypeDef,
     FailureExceptionTypeDef,
     EndpointTypeDef,
     DescribeExportInputRequestTypeDef,
@@ -536,261 +474,215 @@
     KinesisDataStreamDestinationTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
     ExportSummaryTypeDef,
-    ExportTableToPointInTimeInputRequestTypeDef,
-    GetItemInputTableGetItemTypeDef,
-    KeySchemaElementTableOutputTypeDef,
-    ProjectionTableOutputTypeDef,
-    ProvisionedThroughputDescriptionTableTypeDef,
-    KeySchemaElementOutputTypeDef,
+    TimestampTypeDef,
     ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
-    ProvisionedThroughputOutputTypeDef,
-    ProjectionServiceResourceTypeDef,
-    ReplicaOutputTypeDef,
-    S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
     ListTablesInputRequestTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
-    TagTableTypeDef,
-    TagOutputTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
-    ProvisionedThroughputOverrideOutputTypeDef,
-    ProvisionedThroughputOverrideTableOutputTypeDef,
-    PutRequestServiceResourceOutputTypeDef,
-    PutRequestServiceResourceTypeDef,
-    TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
-    RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
-    SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
-    SSESpecificationOutputTypeDef,
-    SSESpecificationTableTypeDef,
-    StreamSpecificationOutputTypeDef,
-    StreamSpecificationTableOutputTypeDef,
-    StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
-    TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
-    ArchivalSummaryTableResponseMetadataTypeDef,
-    BillingModeSummaryTableResponseMetadataTypeDef,
+    ArchivalSummaryResponseTypeDef,
+    BillingModeSummaryResponseTypeDef,
     DescribeLimitsOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     KinesisStreamingDestinationOutputTypeDef,
-    ListTablesOutputTableTypeDef,
     ListTablesOutputTypeDef,
-    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
-    RestoreSummaryTableResponseMetadataTypeDef,
-    SSEDescriptionTableResponseMetadataTypeDef,
-    StreamSpecificationTableResponseMetadataTypeDef,
-    TableClassSummaryTableResponseMetadataTypeDef,
+    ProvisionedThroughputDescriptionResponseTypeDef,
+    RestoreSummaryResponseTypeDef,
+    SSEDescriptionResponseTypeDef,
+    StreamSpecificationResponseTypeDef,
+    TableClassSummaryResponseTypeDef,
     UpdateContributorInsightsOutputTypeDef,
-    AttributeValueUpdateTypeDef,
-    BatchStatementRequestTypeDef,
-    ConditionCheckTypeDef,
-    ConditionTypeDef,
+    UniversalAttributeValueTypeDef,
+    AutoScalingPolicyDescriptionTypeDef,
+    AutoScalingPolicyUpdateTypeDef,
+    CreateBackupOutputTypeDef,
+    ListBackupsOutputTypeDef,
     DeleteRequestOutputTypeDef,
-    DeleteRequestTypeDef,
-    DeleteTypeDef,
-    ExecuteStatementInputRequestTypeDef,
-    ExpectedAttributeValueTypeDef,
-    GetItemInputRequestTypeDef,
-    GetTypeDef,
+    GetItemInputTableGetItemTypeDef,
     ItemCollectionMetricsTypeDef,
     ItemResponseTypeDef,
     KeysAndAttributesOutputTypeDef,
-    KeysAndAttributesTypeDef,
-    ParameterizedStatementTypeDef,
     PutRequestOutputTypeDef,
-    PutRequestTypeDef,
-    PutTypeDef,
-    UpdateTypeDef,
-    AutoScalingPolicyDescriptionTypeDef,
-    AutoScalingPolicyUpdateTypeDef,
-    CreateBackupOutputTypeDef,
-    ListBackupsOutputTableTypeDef,
-    ListBackupsOutputTypeDef,
-    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     BatchStatementResponseTypeDef,
-    ConsumedCapacityServiceResourceTypeDef,
-    ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
-    QueryInputTableQueryTypeDef,
-    ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
-    CreateGlobalSecondaryIndexActionTableTypeDef,
-    UpdateGlobalSecondaryIndexActionTableTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
     GlobalSecondaryIndexTypeDef,
+    SourceTableDetailsTypeDef,
     UpdateGlobalSecondaryIndexActionTypeDef,
     CreateGlobalTableInputRequestTypeDef,
-    ReplicaGlobalSecondaryIndexTableTypeDef,
+    GlobalTableTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     InputFormatOptionsOutputTypeDef,
     InputFormatOptionsTypeDef,
-    DeleteItemInputTableDeleteItemTypeDef,
-    PutItemInputTablePutItemTypeDef,
-    UpdateItemInputTableUpdateItemTypeDef,
     ReplicaUpdateTypeDef,
     DescribeContributorInsightsOutputTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
-    GlobalSecondaryIndexDescriptionTableTypeDef,
+    ExportTableToPointInTimeInputRequestTypeDef,
+    ListBackupsInputRequestTypeDef,
+    GlobalSecondaryIndexInfoTypeDef,
+    GlobalSecondaryIndexOutputTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
     LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
-    GlobalSecondaryIndexInfoTypeDef,
-    GlobalSecondaryIndexOutputTypeDef,
-    SourceTableDetailsTypeDef,
-    GlobalSecondaryIndexServiceResourceTypeDef,
-    LocalSecondaryIndexServiceResourceTypeDef,
-    GlobalTableTypeDef,
     ImportSummaryTypeDef,
     ListBackupsInputListBackupsPaginateTypeDef,
     ListTablesInputListTablesPaginateTypeDef,
     ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    ScanInputScanPaginateTypeDef,
-    ListTagsOfResourceOutputTableTypeDef,
-    ListTagsOfResourceOutputTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
-    WriteRequestServiceResourceOutputTypeDef,
-    WriteRequestServiceResourceTypeDef,
-    UpdateTimeToLiveOutputTypeDef,
     UpdateTimeToLiveInputRequestTypeDef,
-    BatchExecuteStatementInputRequestTypeDef,
-    QueryInputRequestTypeDef,
-    ScanInputRequestTypeDef,
-    DeleteItemInputRequestTypeDef,
-    PutItemInputRequestTypeDef,
-    UpdateItemInputRequestTypeDef,
-    TransactGetItemTypeDef,
-    BatchGetItemInputRequestTypeDef,
-    ExecuteTransactionInputRequestTypeDef,
-    WriteRequestOutputTypeDef,
-    WriteRequestTypeDef,
-    TransactWriteItemTypeDef,
+    UpdateTimeToLiveOutputTypeDef,
+    AttributeValueUpdateTypeDef,
+    BatchStatementRequestTypeDef,
+    ConditionCheckTypeDef,
+    ConditionTypeDef,
+    DeleteRequestTypeDef,
+    DeleteTypeDef,
+    ExecuteStatementInputRequestTypeDef,
+    ExpectedAttributeValueTypeDef,
+    GetItemInputRequestTypeDef,
+    GetTypeDef,
+    KeysAndAttributesTypeDef,
+    ParameterizedStatementTypeDef,
+    PutRequestTypeDef,
+    PutTypeDef,
+    UpdateTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
-    BatchGetItemOutputServiceResourceTypeDef,
-    DeleteItemOutputTableTypeDef,
-    GetItemOutputTableTypeDef,
-    PutItemOutputTableTypeDef,
-    QueryOutputTableTypeDef,
-    ScanOutputTableTypeDef,
-    UpdateItemOutputTableTypeDef,
+    WriteRequestOutputTypeDef,
     BatchExecuteStatementOutputTypeDef,
     BatchGetItemOutputTypeDef,
     DeleteItemOutputTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     GetItemOutputTypeDef,
     PutItemOutputTypeDef,
     QueryOutputTypeDef,
     ScanOutputTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactWriteItemsOutputTypeDef,
     UpdateItemOutputTypeDef,
     DescribeContinuousBackupsOutputTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
-    GlobalSecondaryIndexUpdateTableTypeDef,
-    CreateTableInputRequestTypeDef,
-    RestoreTableFromBackupInputRequestTypeDef,
-    RestoreTableToPointInTimeInputRequestTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
-    CreateReplicationGroupMemberActionTableTypeDef,
-    UpdateReplicationGroupMemberActionTableTypeDef,
+    ListGlobalTablesOutputTypeDef,
+    ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
+    InputFormatOptionsUnionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
-    SourceTableFeatureDetailsTypeDef,
+    GlobalSecondaryIndexUnionTypeDef,
     TableCreationParametersOutputTypeDef,
-    CreateTableInputServiceResourceCreateTableTypeDef,
-    ListGlobalTablesOutputTypeDef,
+    SourceTableFeatureDetailsTypeDef,
     ListImportsOutputTypeDef,
-    ReplicaDescriptionTypeDef,
-    ReplicaDescriptionTableTypeDef,
-    BatchWriteItemOutputServiceResourceTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-    TransactGetItemsInputRequestTypeDef,
-    BatchWriteItemOutputTypeDef,
-    BatchWriteItemInputRequestTypeDef,
-    TransactWriteItemsInputRequestTypeDef,
+    BatchExecuteStatementInputRequestTypeDef,
+    QueryInputQueryPaginateTypeDef,
+    QueryInputRequestTypeDef,
+    QueryInputTableQueryTypeDef,
+    ScanInputRequestTypeDef,
+    ScanInputScanPaginateTypeDef,
+    ScanInputTableScanTypeDef,
+    DeleteItemInputRequestTypeDef,
+    DeleteItemInputTableDeleteItemTypeDef,
+    PutItemInputRequestTypeDef,
+    PutItemInputTablePutItemTypeDef,
+    UpdateItemInputRequestTypeDef,
+    UpdateItemInputTableUpdateItemTypeDef,
+    TransactGetItemTypeDef,
+    KeysAndAttributesUnionTypeDef,
+    ExecuteTransactionInputRequestTypeDef,
+    WriteRequestTypeDef,
+    TransactWriteItemTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
+    BatchWriteItemOutputTypeDef,
     ImportTableInputRequestTypeDef,
-    ReplicationGroupUpdateTableTypeDef,
-    ReplicationGroupUpdateTypeDef,
-    BackupDescriptionTypeDef,
-    ImportTableDescriptionTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
-    TableDescriptionTableTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    CreateTableInputRequestTypeDef,
+    CreateTableInputServiceResourceCreateTableTypeDef,
+    RestoreTableFromBackupInputRequestTypeDef,
+    RestoreTableToPointInTimeInputRequestTypeDef,
+    ImportTableDescriptionTypeDef,
+    TableCreationParametersUnionTypeDef,
+    BackupDescriptionTypeDef,
+    TransactGetItemsInputRequestTypeDef,
+    BatchGetItemInputRequestTypeDef,
+    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
+    WriteRequestUnionTypeDef,
+    TransactWriteItemsInputRequestTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
-    UpdateTableInputTableUpdateTypeDef,
-    UpdateTableInputRequestTypeDef,
-    DeleteBackupOutputTypeDef,
-    DescribeBackupOutputTypeDef,
-    DescribeImportOutputTypeDef,
-    ImportTableOutputTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     CreateTableOutputTypeDef,
     DeleteTableOutputTypeDef,
     DescribeTableOutputTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     UpdateTableOutputTypeDef,
-    DeleteTableOutputTableTypeDef,
+    UpdateTableInputRequestTypeDef,
+    UpdateTableInputTableUpdateTypeDef,
+    DescribeImportOutputTypeDef,
+    ImportTableOutputTypeDef,
+    DeleteBackupOutputTypeDef,
+    DescribeBackupOutputTypeDef,
+    BatchWriteItemInputRequestTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/README.md` & `types-aiobotocore-dynamodb-2.5.2.post3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-dynamodb
+Version: 2.5.2.post3
+Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore dynamodb type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-dynamodb"></a>
 
 # types-aiobotocore-dynamodb
 
 [![PyPI - types-aiobotocore-dynamodb](https://img.shields.io/pypi/v/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dynamodb?color=blue)](https://pypistats.org/packages/types-aiobotocore-dynamodb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodb)](https://pepy.tech/project/types-aiobotocore-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DynamoDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-dynamodb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -45,15 +77,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -415,83 +447,54 @@
 )
 
 
 def check_value(value: AttributeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_dynamodb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_dynamodb.type_defs import (
     ResponseMetadataTypeDef,
-    ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
-    AttributeDefinitionOutputTypeDef,
-    AttributeDefinitionServiceResourceTypeDef,
-    AttributeDefinitionTableOutputTypeDef,
-    AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
-    AttributeValueServiceResourceTypeDef,
-    AttributeValueTableTypeDef,
     AttributeValueTypeDef,
-    AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
-    BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
-    KeysAndAttributesServiceResourceTypeDef,
-    KeysAndAttributesServiceResourceOutputTypeDef,
+    TableAttributeValueTypeDef,
     BatchStatementErrorTypeDef,
-    ItemCollectionMetricsServiceResourceTypeDef,
-    BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
-    CapacityServiceResourceTypeDef,
-    CapacityTableTypeDef,
     CapacityTypeDef,
-    ConditionTableTypeDef,
+    ConditionBaseImportTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
     ContributorInsightsSummaryTypeDef,
     CreateBackupInputRequestTypeDef,
-    KeySchemaElementTableTypeDef,
-    ProjectionTableTypeDef,
-    ProvisionedThroughputTableTypeDef,
     KeySchemaElementTypeDef,
     ProjectionTypeDef,
     ProvisionedThroughputTypeDef,
     ReplicaTypeDef,
     CreateReplicaActionTypeDef,
-    ProvisionedThroughputOverrideTableTypeDef,
     ProvisionedThroughputOverrideTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationTypeDef,
     TagTypeDef,
-    KeySchemaElementServiceResourceTypeDef,
-    ProvisionedThroughputServiceResourceTypeDef,
-    SSESpecificationServiceResourceTypeDef,
-    StreamSpecificationServiceResourceTypeDef,
-    TagServiceResourceTypeDef,
     CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
     DeleteBackupInputRequestTypeDef,
-    DeleteGlobalSecondaryIndexActionTableTypeDef,
     DeleteGlobalSecondaryIndexActionTypeDef,
-    ExpectedAttributeValueTableTypeDef,
-    ItemCollectionMetricsTableTypeDef,
     DeleteReplicaActionTypeDef,
-    DeleteReplicationGroupMemberActionTableTypeDef,
     DeleteReplicationGroupMemberActionTypeDef,
-    DeleteRequestServiceResourceOutputTypeDef,
-    DeleteRequestServiceResourceTypeDef,
     DeleteTableInputRequestTypeDef,
     DescribeBackupInputRequestTypeDef,
     DescribeContinuousBackupsInputRequestTypeDef,
     DescribeContributorInsightsInputRequestTypeDef,
     FailureExceptionTypeDef,
     EndpointTypeDef,
     DescribeExportInputRequestTypeDef,
@@ -503,261 +506,215 @@
     KinesisDataStreamDestinationTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
     ExportSummaryTypeDef,
-    ExportTableToPointInTimeInputRequestTypeDef,
-    GetItemInputTableGetItemTypeDef,
-    KeySchemaElementTableOutputTypeDef,
-    ProjectionTableOutputTypeDef,
-    ProvisionedThroughputDescriptionTableTypeDef,
-    KeySchemaElementOutputTypeDef,
+    TimestampTypeDef,
     ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
-    ProvisionedThroughputOutputTypeDef,
-    ProjectionServiceResourceTypeDef,
-    ReplicaOutputTypeDef,
-    S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
     ListTablesInputRequestTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
-    TagTableTypeDef,
-    TagOutputTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
-    ProvisionedThroughputOverrideOutputTypeDef,
-    ProvisionedThroughputOverrideTableOutputTypeDef,
-    PutRequestServiceResourceOutputTypeDef,
-    PutRequestServiceResourceTypeDef,
-    TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
-    RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
-    SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
-    SSESpecificationOutputTypeDef,
-    SSESpecificationTableTypeDef,
-    StreamSpecificationOutputTypeDef,
-    StreamSpecificationTableOutputTypeDef,
-    StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
-    TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
-    ArchivalSummaryTableResponseMetadataTypeDef,
-    BillingModeSummaryTableResponseMetadataTypeDef,
+    ArchivalSummaryResponseTypeDef,
+    BillingModeSummaryResponseTypeDef,
     DescribeLimitsOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     KinesisStreamingDestinationOutputTypeDef,
-    ListTablesOutputTableTypeDef,
     ListTablesOutputTypeDef,
-    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
-    RestoreSummaryTableResponseMetadataTypeDef,
-    SSEDescriptionTableResponseMetadataTypeDef,
-    StreamSpecificationTableResponseMetadataTypeDef,
-    TableClassSummaryTableResponseMetadataTypeDef,
+    ProvisionedThroughputDescriptionResponseTypeDef,
+    RestoreSummaryResponseTypeDef,
+    SSEDescriptionResponseTypeDef,
+    StreamSpecificationResponseTypeDef,
+    TableClassSummaryResponseTypeDef,
     UpdateContributorInsightsOutputTypeDef,
-    AttributeValueUpdateTypeDef,
-    BatchStatementRequestTypeDef,
-    ConditionCheckTypeDef,
-    ConditionTypeDef,
+    UniversalAttributeValueTypeDef,
+    AutoScalingPolicyDescriptionTypeDef,
+    AutoScalingPolicyUpdateTypeDef,
+    CreateBackupOutputTypeDef,
+    ListBackupsOutputTypeDef,
     DeleteRequestOutputTypeDef,
-    DeleteRequestTypeDef,
-    DeleteTypeDef,
-    ExecuteStatementInputRequestTypeDef,
-    ExpectedAttributeValueTypeDef,
-    GetItemInputRequestTypeDef,
-    GetTypeDef,
+    GetItemInputTableGetItemTypeDef,
     ItemCollectionMetricsTypeDef,
     ItemResponseTypeDef,
     KeysAndAttributesOutputTypeDef,
-    KeysAndAttributesTypeDef,
-    ParameterizedStatementTypeDef,
     PutRequestOutputTypeDef,
-    PutRequestTypeDef,
-    PutTypeDef,
-    UpdateTypeDef,
-    AutoScalingPolicyDescriptionTypeDef,
-    AutoScalingPolicyUpdateTypeDef,
-    CreateBackupOutputTypeDef,
-    ListBackupsOutputTableTypeDef,
-    ListBackupsOutputTypeDef,
-    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     BatchStatementResponseTypeDef,
-    ConsumedCapacityServiceResourceTypeDef,
-    ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
-    QueryInputTableQueryTypeDef,
-    ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
-    CreateGlobalSecondaryIndexActionTableTypeDef,
-    UpdateGlobalSecondaryIndexActionTableTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
     GlobalSecondaryIndexTypeDef,
+    SourceTableDetailsTypeDef,
     UpdateGlobalSecondaryIndexActionTypeDef,
     CreateGlobalTableInputRequestTypeDef,
-    ReplicaGlobalSecondaryIndexTableTypeDef,
+    GlobalTableTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     InputFormatOptionsOutputTypeDef,
     InputFormatOptionsTypeDef,
-    DeleteItemInputTableDeleteItemTypeDef,
-    PutItemInputTablePutItemTypeDef,
-    UpdateItemInputTableUpdateItemTypeDef,
     ReplicaUpdateTypeDef,
     DescribeContributorInsightsOutputTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
-    GlobalSecondaryIndexDescriptionTableTypeDef,
+    ExportTableToPointInTimeInputRequestTypeDef,
+    ListBackupsInputRequestTypeDef,
+    GlobalSecondaryIndexInfoTypeDef,
+    GlobalSecondaryIndexOutputTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
     LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
-    GlobalSecondaryIndexInfoTypeDef,
-    GlobalSecondaryIndexOutputTypeDef,
-    SourceTableDetailsTypeDef,
-    GlobalSecondaryIndexServiceResourceTypeDef,
-    LocalSecondaryIndexServiceResourceTypeDef,
-    GlobalTableTypeDef,
     ImportSummaryTypeDef,
     ListBackupsInputListBackupsPaginateTypeDef,
     ListTablesInputListTablesPaginateTypeDef,
     ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    ScanInputScanPaginateTypeDef,
-    ListTagsOfResourceOutputTableTypeDef,
-    ListTagsOfResourceOutputTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
-    WriteRequestServiceResourceOutputTypeDef,
-    WriteRequestServiceResourceTypeDef,
-    UpdateTimeToLiveOutputTypeDef,
     UpdateTimeToLiveInputRequestTypeDef,
-    BatchExecuteStatementInputRequestTypeDef,
-    QueryInputRequestTypeDef,
-    ScanInputRequestTypeDef,
-    DeleteItemInputRequestTypeDef,
-    PutItemInputRequestTypeDef,
-    UpdateItemInputRequestTypeDef,
-    TransactGetItemTypeDef,
-    BatchGetItemInputRequestTypeDef,
-    ExecuteTransactionInputRequestTypeDef,
-    WriteRequestOutputTypeDef,
-    WriteRequestTypeDef,
-    TransactWriteItemTypeDef,
+    UpdateTimeToLiveOutputTypeDef,
+    AttributeValueUpdateTypeDef,
+    BatchStatementRequestTypeDef,
+    ConditionCheckTypeDef,
+    ConditionTypeDef,
+    DeleteRequestTypeDef,
+    DeleteTypeDef,
+    ExecuteStatementInputRequestTypeDef,
+    ExpectedAttributeValueTypeDef,
+    GetItemInputRequestTypeDef,
+    GetTypeDef,
+    KeysAndAttributesTypeDef,
+    ParameterizedStatementTypeDef,
+    PutRequestTypeDef,
+    PutTypeDef,
+    UpdateTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
-    BatchGetItemOutputServiceResourceTypeDef,
-    DeleteItemOutputTableTypeDef,
-    GetItemOutputTableTypeDef,
-    PutItemOutputTableTypeDef,
-    QueryOutputTableTypeDef,
-    ScanOutputTableTypeDef,
-    UpdateItemOutputTableTypeDef,
+    WriteRequestOutputTypeDef,
     BatchExecuteStatementOutputTypeDef,
     BatchGetItemOutputTypeDef,
     DeleteItemOutputTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     GetItemOutputTypeDef,
     PutItemOutputTypeDef,
     QueryOutputTypeDef,
     ScanOutputTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactWriteItemsOutputTypeDef,
     UpdateItemOutputTypeDef,
     DescribeContinuousBackupsOutputTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
-    GlobalSecondaryIndexUpdateTableTypeDef,
-    CreateTableInputRequestTypeDef,
-    RestoreTableFromBackupInputRequestTypeDef,
-    RestoreTableToPointInTimeInputRequestTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
-    CreateReplicationGroupMemberActionTableTypeDef,
-    UpdateReplicationGroupMemberActionTableTypeDef,
+    ListGlobalTablesOutputTypeDef,
+    ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
+    InputFormatOptionsUnionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
-    SourceTableFeatureDetailsTypeDef,
+    GlobalSecondaryIndexUnionTypeDef,
     TableCreationParametersOutputTypeDef,
-    CreateTableInputServiceResourceCreateTableTypeDef,
-    ListGlobalTablesOutputTypeDef,
+    SourceTableFeatureDetailsTypeDef,
     ListImportsOutputTypeDef,
-    ReplicaDescriptionTypeDef,
-    ReplicaDescriptionTableTypeDef,
-    BatchWriteItemOutputServiceResourceTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-    TransactGetItemsInputRequestTypeDef,
-    BatchWriteItemOutputTypeDef,
-    BatchWriteItemInputRequestTypeDef,
-    TransactWriteItemsInputRequestTypeDef,
+    BatchExecuteStatementInputRequestTypeDef,
+    QueryInputQueryPaginateTypeDef,
+    QueryInputRequestTypeDef,
+    QueryInputTableQueryTypeDef,
+    ScanInputRequestTypeDef,
+    ScanInputScanPaginateTypeDef,
+    ScanInputTableScanTypeDef,
+    DeleteItemInputRequestTypeDef,
+    DeleteItemInputTableDeleteItemTypeDef,
+    PutItemInputRequestTypeDef,
+    PutItemInputTablePutItemTypeDef,
+    UpdateItemInputRequestTypeDef,
+    UpdateItemInputTableUpdateItemTypeDef,
+    TransactGetItemTypeDef,
+    KeysAndAttributesUnionTypeDef,
+    ExecuteTransactionInputRequestTypeDef,
+    WriteRequestTypeDef,
+    TransactWriteItemTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
+    BatchWriteItemOutputTypeDef,
     ImportTableInputRequestTypeDef,
-    ReplicationGroupUpdateTableTypeDef,
-    ReplicationGroupUpdateTypeDef,
-    BackupDescriptionTypeDef,
-    ImportTableDescriptionTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
-    TableDescriptionTableTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    CreateTableInputRequestTypeDef,
+    CreateTableInputServiceResourceCreateTableTypeDef,
+    RestoreTableFromBackupInputRequestTypeDef,
+    RestoreTableToPointInTimeInputRequestTypeDef,
+    ImportTableDescriptionTypeDef,
+    TableCreationParametersUnionTypeDef,
+    BackupDescriptionTypeDef,
+    TransactGetItemsInputRequestTypeDef,
+    BatchGetItemInputRequestTypeDef,
+    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
+    WriteRequestUnionTypeDef,
+    TransactWriteItemsInputRequestTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
-    UpdateTableInputTableUpdateTypeDef,
-    UpdateTableInputRequestTypeDef,
-    DeleteBackupOutputTypeDef,
-    DescribeBackupOutputTypeDef,
-    DescribeImportOutputTypeDef,
-    ImportTableOutputTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     CreateTableOutputTypeDef,
     DeleteTableOutputTypeDef,
     DescribeTableOutputTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     UpdateTableOutputTypeDef,
-    DeleteTableOutputTableTypeDef,
+    UpdateTableInputRequestTypeDef,
+    UpdateTableInputTableUpdateTypeDef,
+    DescribeImportOutputTypeDef,
+    ImportTableOutputTypeDef,
+    DeleteBackupOutputTypeDef,
+    DescribeBackupOutputTypeDef,
+    BatchWriteItemInputRequestTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/setup.py` & `types-aiobotocore-dynamodb-2.5.2.post3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dynamodb",
-    version="2.5.2.post2",
+    version="2.5.2.post3",
     packages=["types_aiobotocore_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder"
-        " 7.15.0"
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
-    keywords="aiobotocore dynamodb type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore dynamodb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_dynamodb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/"
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/__init__.py` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     ScanPaginator,
 )
 from .service_resource import DynamoDBServiceResource
 from .waiter import TableExistsWaiter, TableNotExistsWaiter
 
 Client = DynamoDBClient
 
+ServiceResource = DynamoDBServiceResource
 
 __all__ = (
     "Client",
     "DynamoDBClient",
     "DynamoDBServiceResource",
     "ListBackupsPaginator",
     "ListTablesPaginator",
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/__init__.pyi` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,18 @@
     ScanPaginator,
 )
 from .service_resource import DynamoDBServiceResource
 from .waiter import TableExistsWaiter, TableNotExistsWaiter
 
 Client = DynamoDBClient
 
+
+ServiceResource = DynamoDBServiceResource
+
+
 __all__ = (
     "Client",
     "DynamoDBClient",
     "DynamoDBServiceResource",
     "ListBackupsPaginator",
     "ListTablesPaginator",
     "ListTagsOfResourcePaginator",
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/__main__.py` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DynamoDB 2.5.2\nVersion:         2.5.2.post2\nBuilder"
-        " version: 7.15.0\nDocs:           "
+        "Type annotations for aiobotocore.DynamoDB 2.5.2\nVersion:         2.5.2.post3\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post2")
+    print("2.5.2.post3")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/client.py` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/client.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 
     session = get_session()
     async with session.create_client("dynamodb") as client:
         client: DynamoDBClient
     ```
 """
 import sys
-from datetime import datetime
-from decimal import Decimal
-from typing import Any, Dict, Mapping, Sequence, Set, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     BackupTypeFilterType,
     BillingModeType,
@@ -42,15 +40,14 @@
     ListTablesPaginator,
     ListTagsOfResourcePaginator,
     QueryPaginator,
     ScanPaginator,
 )
 from .type_defs import (
     AttributeDefinitionTypeDef,
-    AttributeValueTypeDef,
     AttributeValueUpdateTypeDef,
     AutoScalingSettingsUpdateTypeDef,
     BatchExecuteStatementOutputTypeDef,
     BatchGetItemOutputTypeDef,
     BatchStatementRequestTypeDef,
     BatchWriteItemOutputTypeDef,
     ConditionTypeDef,
@@ -76,20 +73,20 @@
     EmptyResponseMetadataTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     ExpectedAttributeValueTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     GetItemOutputTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
-    GlobalSecondaryIndexTypeDef,
+    GlobalSecondaryIndexUnionTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ImportTableOutputTypeDef,
-    InputFormatOptionsTypeDef,
-    KeysAndAttributesTypeDef,
+    InputFormatOptionsUnionTypeDef,
+    KeysAndAttributesUnionTypeDef,
     KeySchemaElementTypeDef,
     KinesisStreamingDestinationOutputTypeDef,
     ListBackupsOutputTypeDef,
     ListContributorInsightsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
@@ -108,50 +105,49 @@
     ReplicaUpdateTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     S3BucketSourceTypeDef,
     ScanOutputTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationTypeDef,
-    TableCreationParametersTypeDef,
+    TableCreationParametersUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TimeToLiveSpecificationTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactGetItemTypeDef,
     TransactWriteItemsOutputTypeDef,
     TransactWriteItemTypeDef,
+    UniversalAttributeValueTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateItemOutputTypeDef,
     UpdateTableOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
     UpdateTimeToLiveOutputTypeDef,
-    WriteRequestTypeDef,
+    WriteRequestUnionTypeDef,
 )
 from .waiter import TableExistsWaiter, TableNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DynamoDBClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BackupInUseException: Type[BotocoreClientError]
     BackupNotFoundException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConditionalCheckFailedException: Type[BotocoreClientError]
     ContinuousBackupsUnavailableException: Type[BotocoreClientError]
     DuplicateItemException: Type[BotocoreClientError]
@@ -178,15 +174,14 @@
     TableAlreadyExistsException: Type[BotocoreClientError]
     TableInUseException: Type[BotocoreClientError]
     TableNotFoundException: Type[BotocoreClientError]
     TransactionCanceledException: Type[BotocoreClientError]
     TransactionConflictException: Type[BotocoreClientError]
     TransactionInProgressException: Type[BotocoreClientError]
 
-
 class DynamoDBClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/)
     """
 
     meta: ClientMeta
@@ -195,828 +190,572 @@
     def exceptions(self) -> Exceptions:
         """
         DynamoDBClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#exceptions)
         """
-
     async def batch_execute_statement(
         self,
         *,
         Statements: Sequence[BatchStatementRequestTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
     ) -> BatchExecuteStatementOutputTypeDef:
         """
         This operation allows you to perform batch reads or writes on data stored in
         DynamoDB, using PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_execute_statement)
         """
-
     async def batch_get_item(
         self,
         *,
-        RequestItems: Mapping[str, KeysAndAttributesTypeDef],
+        RequestItems: Mapping[str, KeysAndAttributesUnionTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
     ) -> BatchGetItemOutputTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_get_item)
         """
-
     async def batch_write_item(
         self,
         *,
-        RequestItems: Mapping[str, Sequence[WriteRequestTypeDef]],
+        RequestItems: Mapping[str, Sequence[WriteRequestUnionTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
     ) -> BatchWriteItemOutputTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_write_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_write_item)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#close)
         """
-
     async def create_backup(self, *, TableName: str, BackupName: str) -> CreateBackupOutputTypeDef:
         """
         Creates a backup for an existing table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.create_backup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#create_backup)
         """
-
     async def create_global_table(
         self, *, GlobalTableName: str, ReplicationGroup: Sequence[ReplicaTypeDef]
     ) -> CreateGlobalTableOutputTypeDef:
         """
         Creates a global table from an existing table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.create_global_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#create_global_table)
         """
-
     async def create_table(
         self,
         *,
         AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],
         TableName: str,
         KeySchema: Sequence[KeySchemaElementTypeDef],
         LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,
-        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexTypeDef] = ...,
+        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
     ) -> CreateTableOutputTypeDef:
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#create_table)
         """
-
     async def delete_backup(self, *, BackupArn: str) -> DeleteBackupOutputTypeDef:
         """
         Deletes an existing backup of a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_backup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#delete_backup)
         """
-
     async def delete_item(
         self,
         *,
         TableName: str,
-        Key: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        Key: Mapping[str, UniversalAttributeValueTypeDef],
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
     ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#delete_item)
         """
-
     async def delete_table(self, *, TableName: str) -> DeleteTableOutputTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#delete_table)
         """
-
     async def describe_backup(self, *, BackupArn: str) -> DescribeBackupOutputTypeDef:
         """
         Describes an existing backup of a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_backup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_backup)
         """
-
     async def describe_continuous_backups(
         self, *, TableName: str
     ) -> DescribeContinuousBackupsOutputTypeDef:
         """
         Checks the status of continuous backups and point in time recovery on the
         specified table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_continuous_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_continuous_backups)
         """
-
     async def describe_contributor_insights(
         self, *, TableName: str, IndexName: str = ...
     ) -> DescribeContributorInsightsOutputTypeDef:
         """
         Returns information about contributor insights for a given table or global
         secondary index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_contributor_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_contributor_insights)
         """
-
     async def describe_endpoints(self) -> DescribeEndpointsResponseTypeDef:
         """
         Returns the regional endpoint information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_endpoints)
         """
-
     async def describe_export(self, *, ExportArn: str) -> DescribeExportOutputTypeDef:
         """
         Describes an existing table export.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_export)
         """
-
     async def describe_global_table(
         self, *, GlobalTableName: str
     ) -> DescribeGlobalTableOutputTypeDef:
         """
         Returns information about the specified global table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_global_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_global_table)
         """
-
     async def describe_global_table_settings(
         self, *, GlobalTableName: str
     ) -> DescribeGlobalTableSettingsOutputTypeDef:
         """
         Describes Region-specific settings for a global table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_global_table_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_global_table_settings)
         """
-
     async def describe_import(self, *, ImportArn: str) -> DescribeImportOutputTypeDef:
         """
         Represents the properties of the import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_import)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_import)
         """
-
     async def describe_kinesis_streaming_destination(
         self, *, TableName: str
     ) -> DescribeKinesisStreamingDestinationOutputTypeDef:
         """
         Returns information about the status of Kinesis streaming.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_kinesis_streaming_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_kinesis_streaming_destination)
         """
-
     async def describe_limits(self) -> DescribeLimitsOutputTypeDef:
         """
         Returns the current provisioned-capacity quotas for your Amazon Web Services
         account in a Region, both for the Region as a whole and for any one DynamoDB
         table that you create there.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_limits)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_limits)
         """
-
     async def describe_table(self, *, TableName: str) -> DescribeTableOutputTypeDef:
         """
         Returns information about the table, including the current status of the table,
         when it was created, the primary key schema, and any indexes on the table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_table)
         """
-
     async def describe_table_replica_auto_scaling(
         self, *, TableName: str
     ) -> DescribeTableReplicaAutoScalingOutputTypeDef:
         """
         Describes auto scaling settings across replicas of the global table at once.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_table_replica_auto_scaling)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_table_replica_auto_scaling)
         """
-
     async def describe_time_to_live(self, *, TableName: str) -> DescribeTimeToLiveOutputTypeDef:
         """
         Gives a description of the Time to Live (TTL) status on the specified table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_time_to_live)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_time_to_live)
         """
-
     async def disable_kinesis_streaming_destination(
         self, *, TableName: str, StreamArn: str
     ) -> KinesisStreamingDestinationOutputTypeDef:
         """
         Stops replication from the DynamoDB table to the Kinesis data stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.disable_kinesis_streaming_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#disable_kinesis_streaming_destination)
         """
-
     async def enable_kinesis_streaming_destination(
         self, *, TableName: str, StreamArn: str
     ) -> KinesisStreamingDestinationOutputTypeDef:
         """
         Starts table data replication to the specified Kinesis data stream at a
         timestamp chosen during the enable workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.enable_kinesis_streaming_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#enable_kinesis_streaming_destination)
         """
-
     async def execute_statement(
         self,
         *,
         Statement: str,
-        Parameters: Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ] = ...,
+        Parameters: Sequence[UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         NextToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         Limit: int = ...
     ) -> ExecuteStatementOutputTypeDef:
         """
         This operation allows you to perform reads and singleton writes on data stored
         in DynamoDB, using PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#execute_statement)
         """
-
     async def execute_transaction(
         self,
         *,
         TransactStatements: Sequence[ParameterizedStatementTypeDef],
         ClientRequestToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
     ) -> ExecuteTransactionOutputTypeDef:
         """
         This operation allows you to perform transactional reads or writes on data
         stored in DynamoDB, using PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.execute_transaction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#execute_transaction)
         """
-
     async def export_table_to_point_in_time(
         self,
         *,
         TableArn: str,
         S3Bucket: str,
-        ExportTime: Union[datetime, str] = ...,
+        ExportTime: TimestampTypeDef = ...,
         ClientToken: str = ...,
         S3BucketOwner: str = ...,
         S3Prefix: str = ...,
         S3SseAlgorithm: S3SseAlgorithmType = ...,
         S3SseKmsKeyId: str = ...,
         ExportFormat: ExportFormatType = ...
     ) -> ExportTableToPointInTimeOutputTypeDef:
         """
         Exports table data to an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.export_table_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#export_table_to_point_in_time)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#generate_presigned_url)
         """
-
     async def get_item(
         self,
         *,
         TableName: str,
-        Key: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        Key: Mapping[str, UniversalAttributeValueTypeDef],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...
     ) -> GetItemOutputTypeDef:
         """
         The `GetItem` operation returns a set of attributes for the item with the given
         primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_item)
         """
-
     async def import_table(
         self,
         *,
         S3BucketSource: S3BucketSourceTypeDef,
         InputFormat: InputFormatType,
-        TableCreationParameters: TableCreationParametersTypeDef,
+        TableCreationParameters: TableCreationParametersUnionTypeDef,
         ClientToken: str = ...,
-        InputFormatOptions: InputFormatOptionsTypeDef = ...,
+        InputFormatOptions: InputFormatOptionsUnionTypeDef = ...,
         InputCompressionType: InputCompressionTypeType = ...
     ) -> ImportTableOutputTypeDef:
         """
         Imports table data from an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.import_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#import_table)
         """
-
     async def list_backups(
         self,
         *,
         TableName: str = ...,
         Limit: int = ...,
-        TimeRangeLowerBound: Union[datetime, str] = ...,
-        TimeRangeUpperBound: Union[datetime, str] = ...,
+        TimeRangeLowerBound: TimestampTypeDef = ...,
+        TimeRangeUpperBound: TimestampTypeDef = ...,
         ExclusiveStartBackupArn: str = ...,
         BackupType: BackupTypeFilterType = ...
     ) -> ListBackupsOutputTypeDef:
         """
         List backups associated with an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_backups)
         """
-
     async def list_contributor_insights(
         self, *, TableName: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListContributorInsightsOutputTypeDef:
         """
         Returns a list of ContributorInsightsSummary for a table and all its global
         secondary indexes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_contributor_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_contributor_insights)
         """
-
     async def list_exports(
         self, *, TableArn: str = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> ListExportsOutputTypeDef:
         """
         Lists completed exports within the past 90 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_exports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_exports)
         """
-
     async def list_global_tables(
         self, *, ExclusiveStartGlobalTableName: str = ..., Limit: int = ..., RegionName: str = ...
     ) -> ListGlobalTablesOutputTypeDef:
         """
         Lists all global tables that have a replica in the specified Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_global_tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_global_tables)
         """
-
     async def list_imports(
         self, *, TableArn: str = ..., PageSize: int = ..., NextToken: str = ...
     ) -> ListImportsOutputTypeDef:
         """
         Lists completed imports within the past 90 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_imports)
         """
-
     async def list_tables(
         self, *, ExclusiveStartTableName: str = ..., Limit: int = ...
     ) -> ListTablesOutputTypeDef:
         """
         Returns an array of table names associated with the current account and
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_tables)
         """
-
     async def list_tags_of_resource(
         self, *, ResourceArn: str, NextToken: str = ...
     ) -> ListTagsOfResourceOutputTypeDef:
         """
         List all tags on an Amazon DynamoDB resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_tags_of_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_tags_of_resource)
         """
-
     async def put_item(
         self,
         *,
         TableName: str,
-        Item: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        Item: Mapping[str, UniversalAttributeValueTypeDef],
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
     ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#put_item)
         """
-
     async def query(
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         ConsistentRead: bool = ...,
         KeyConditions: Mapping[str, ConditionTypeDef] = ...,
         QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
-        ExclusiveStartKey: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...,
+        ExclusiveStartKey: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
     ) -> QueryOutputTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#query)
         """
-
     async def restore_table_from_backup(
         self,
         *,
         TargetTableName: str,
         BackupArn: str,
         BillingModeOverride: BillingModeType = ...,
-        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexTypeDef] = ...,
+        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...
     ) -> RestoreTableFromBackupOutputTypeDef:
         """
         Creates a new table from an existing backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.restore_table_from_backup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#restore_table_from_backup)
         """
-
     async def restore_table_to_point_in_time(
         self,
         *,
         TargetTableName: str,
         SourceTableArn: str = ...,
         SourceTableName: str = ...,
         UseLatestRestorableTime: bool = ...,
-        RestoreDateTime: Union[datetime, str] = ...,
+        RestoreDateTime: TimestampTypeDef = ...,
         BillingModeOverride: BillingModeType = ...,
-        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexTypeDef] = ...,
+        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...
     ) -> RestoreTableToPointInTimeOutputTypeDef:
         """
         Restores the specified table to the specified point in time within
         `EarliestRestorableDateTime` and `LatestRestorableDateTime`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.restore_table_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#restore_table_to_point_in_time)
         """
-
     async def scan(
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         Select: SelectType = ...,
         ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
-        ExclusiveStartKey: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...,
+        ExclusiveStartKey: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...
     ) -> ScanOutputTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.scan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#scan)
         """
-
     async def tag_resource(
         self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associate a set of tags with an Amazon DynamoDB resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#tag_resource)
         """
-
     async def transact_get_items(
         self,
         *,
         TransactItems: Sequence[TransactGetItemTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
     ) -> TransactGetItemsOutputTypeDef:
         """
         `TransactGetItems` is a synchronous operation that atomically retrieves multiple
         items from one or more tables (but not from indexes) in a single account and
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.transact_get_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#transact_get_items)
         """
-
     async def transact_write_items(
         self,
         *,
         TransactItems: Sequence[TransactWriteItemTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ClientRequestToken: str = ...
@@ -1024,63 +763,58 @@
         """
         `TransactWriteItems` is a synchronous write operation that groups up to 100
         action requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.transact_write_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#transact_write_items)
         """
-
     async def untag_resource(
         self, *, ResourceArn: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes the association of tags from an Amazon DynamoDB resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#untag_resource)
         """
-
     async def update_continuous_backups(
         self,
         *,
         TableName: str,
         PointInTimeRecoverySpecification: PointInTimeRecoverySpecificationTypeDef
     ) -> UpdateContinuousBackupsOutputTypeDef:
         """
         `UpdateContinuousBackups` enables or disables point in time recovery for the
         specified table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_continuous_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_continuous_backups)
         """
-
     async def update_contributor_insights(
         self,
         *,
         TableName: str,
         ContributorInsightsAction: ContributorInsightsActionType,
         IndexName: str = ...
     ) -> UpdateContributorInsightsOutputTypeDef:
         """
         Updates the status for contributor insights for a specific table or index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_contributor_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_contributor_insights)
         """
-
     async def update_global_table(
         self, *, GlobalTableName: str, ReplicaUpdates: Sequence[ReplicaUpdateTypeDef]
     ) -> UpdateGlobalTableOutputTypeDef:
         """
         Adds or removes replicas in the specified global table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_global_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_global_table)
         """
-
     async def update_global_table_settings(
         self,
         *,
         GlobalTableName: str,
         GlobalTableBillingMode: BillingModeType = ...,
         GlobalTableProvisionedWriteCapacityUnits: int = ...,
         GlobalTableProvisionedWriteCapacityAutoScalingSettingsUpdate: AutoScalingSettingsUpdateTypeDef = ...,
@@ -1091,81 +825,37 @@
     ) -> UpdateGlobalTableSettingsOutputTypeDef:
         """
         Updates settings for a global table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_global_table_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_global_table_settings)
         """
-
     async def update_item(
         self,
         *,
         TableName: str,
-        Key: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        Key: Mapping[str, UniversalAttributeValueTypeDef],
         AttributeUpdates: Mapping[str, AttributeValueUpdateTypeDef] = ...,
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
     ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_item)
         """
-
     async def update_table(
         self,
         *,
         TableName: str,
         AttributeDefinitions: Sequence[AttributeDefinitionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
@@ -1179,96 +869,85 @@
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_table)
         """
-
     async def update_table_replica_auto_scaling(
         self,
         *,
         TableName: str,
         GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef] = ...,
         ProvisionedWriteCapacityAutoScalingUpdate: AutoScalingSettingsUpdateTypeDef = ...,
         ReplicaUpdates: Sequence[ReplicaAutoScalingUpdateTypeDef] = ...
     ) -> UpdateTableReplicaAutoScalingOutputTypeDef:
         """
         Updates auto scaling settings on your global tables at once.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_table_replica_auto_scaling)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_table_replica_auto_scaling)
         """
-
     async def update_time_to_live(
         self, *, TableName: str, TimeToLiveSpecification: TimeToLiveSpecificationTypeDef
     ) -> UpdateTimeToLiveOutputTypeDef:
         """
         The `UpdateTimeToLive` method enables or disables Time to Live (TTL) for the
         specified table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_time_to_live)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_time_to_live)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_backups"]) -> ListBackupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_tables"]) -> ListTablesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_of_resource"]
     ) -> ListTagsOfResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["query"]) -> QueryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["scan"]) -> ScanPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_paginator)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["table_exists"]) -> TableExistsWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["table_not_exists"]) -> TableNotExistsWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_waiter)
         """
-
     async def __aenter__(self) -> "DynamoDBClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/client.pyi` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 
     session = get_session()
     async with session.create_client("dynamodb") as client:
         client: DynamoDBClient
     ```
 """
 import sys
-from datetime import datetime
-from decimal import Decimal
-from typing import Any, Dict, Mapping, Sequence, Set, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     BackupTypeFilterType,
     BillingModeType,
@@ -42,15 +40,14 @@
     ListTablesPaginator,
     ListTagsOfResourcePaginator,
     QueryPaginator,
     ScanPaginator,
 )
 from .type_defs import (
     AttributeDefinitionTypeDef,
-    AttributeValueTypeDef,
     AttributeValueUpdateTypeDef,
     AutoScalingSettingsUpdateTypeDef,
     BatchExecuteStatementOutputTypeDef,
     BatchGetItemOutputTypeDef,
     BatchStatementRequestTypeDef,
     BatchWriteItemOutputTypeDef,
     ConditionTypeDef,
@@ -76,20 +73,20 @@
     EmptyResponseMetadataTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     ExpectedAttributeValueTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     GetItemOutputTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
-    GlobalSecondaryIndexTypeDef,
+    GlobalSecondaryIndexUnionTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ImportTableOutputTypeDef,
-    InputFormatOptionsTypeDef,
-    KeysAndAttributesTypeDef,
+    InputFormatOptionsUnionTypeDef,
+    KeysAndAttributesUnionTypeDef,
     KeySchemaElementTypeDef,
     KinesisStreamingDestinationOutputTypeDef,
     ListBackupsOutputTypeDef,
     ListContributorInsightsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListGlobalTablesOutputTypeDef,
     ListImportsOutputTypeDef,
@@ -108,47 +105,52 @@
     ReplicaUpdateTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     S3BucketSourceTypeDef,
     ScanOutputTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationTypeDef,
-    TableCreationParametersTypeDef,
+    TableCreationParametersUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TimeToLiveSpecificationTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactGetItemTypeDef,
     TransactWriteItemsOutputTypeDef,
     TransactWriteItemTypeDef,
+    UniversalAttributeValueTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
     UpdateContributorInsightsOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateItemOutputTypeDef,
     UpdateTableOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
     UpdateTimeToLiveOutputTypeDef,
-    WriteRequestTypeDef,
+    WriteRequestUnionTypeDef,
 )
 from .waiter import TableExistsWaiter, TableNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("DynamoDBClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BackupInUseException: Type[BotocoreClientError]
     BackupNotFoundException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConditionalCheckFailedException: Type[BotocoreClientError]
     ContinuousBackupsUnavailableException: Type[BotocoreClientError]
     DuplicateItemException: Type[BotocoreClientError]
@@ -175,14 +177,15 @@
     TableAlreadyExistsException: Type[BotocoreClientError]
     TableInUseException: Type[BotocoreClientError]
     TableNotFoundException: Type[BotocoreClientError]
     TransactionCanceledException: Type[BotocoreClientError]
     TransactionConflictException: Type[BotocoreClientError]
     TransactionInProgressException: Type[BotocoreClientError]
 
+
 class DynamoDBClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/)
     """
 
     meta: ClientMeta
@@ -191,781 +194,619 @@
     def exceptions(self) -> Exceptions:
         """
         DynamoDBClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#exceptions)
         """
+
     async def batch_execute_statement(
         self,
         *,
         Statements: Sequence[BatchStatementRequestTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
     ) -> BatchExecuteStatementOutputTypeDef:
         """
         This operation allows you to perform batch reads or writes on data stored in
         DynamoDB, using PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_execute_statement)
         """
+
     async def batch_get_item(
         self,
         *,
-        RequestItems: Mapping[str, KeysAndAttributesTypeDef],
+        RequestItems: Mapping[str, KeysAndAttributesUnionTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
     ) -> BatchGetItemOutputTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_get_item)
         """
+
     async def batch_write_item(
         self,
         *,
-        RequestItems: Mapping[str, Sequence[WriteRequestTypeDef]],
+        RequestItems: Mapping[str, Sequence[WriteRequestUnionTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
     ) -> BatchWriteItemOutputTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.batch_write_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#batch_write_item)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#close)
         """
+
     async def create_backup(self, *, TableName: str, BackupName: str) -> CreateBackupOutputTypeDef:
         """
         Creates a backup for an existing table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.create_backup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#create_backup)
         """
+
     async def create_global_table(
         self, *, GlobalTableName: str, ReplicationGroup: Sequence[ReplicaTypeDef]
     ) -> CreateGlobalTableOutputTypeDef:
         """
         Creates a global table from an existing table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.create_global_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#create_global_table)
         """
+
     async def create_table(
         self,
         *,
         AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],
         TableName: str,
         KeySchema: Sequence[KeySchemaElementTypeDef],
         LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,
-        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexTypeDef] = ...,
+        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
         StreamSpecification: StreamSpecificationTypeDef = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
     ) -> CreateTableOutputTypeDef:
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#create_table)
         """
+
     async def delete_backup(self, *, BackupArn: str) -> DeleteBackupOutputTypeDef:
         """
         Deletes an existing backup of a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_backup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#delete_backup)
         """
+
     async def delete_item(
         self,
         *,
         TableName: str,
-        Key: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        Key: Mapping[str, UniversalAttributeValueTypeDef],
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
     ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#delete_item)
         """
+
     async def delete_table(self, *, TableName: str) -> DeleteTableOutputTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.delete_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#delete_table)
         """
+
     async def describe_backup(self, *, BackupArn: str) -> DescribeBackupOutputTypeDef:
         """
         Describes an existing backup of a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_backup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_backup)
         """
+
     async def describe_continuous_backups(
         self, *, TableName: str
     ) -> DescribeContinuousBackupsOutputTypeDef:
         """
         Checks the status of continuous backups and point in time recovery on the
         specified table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_continuous_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_continuous_backups)
         """
+
     async def describe_contributor_insights(
         self, *, TableName: str, IndexName: str = ...
     ) -> DescribeContributorInsightsOutputTypeDef:
         """
         Returns information about contributor insights for a given table or global
         secondary index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_contributor_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_contributor_insights)
         """
+
     async def describe_endpoints(self) -> DescribeEndpointsResponseTypeDef:
         """
         Returns the regional endpoint information.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_endpoints)
         """
+
     async def describe_export(self, *, ExportArn: str) -> DescribeExportOutputTypeDef:
         """
         Describes an existing table export.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_export)
         """
+
     async def describe_global_table(
         self, *, GlobalTableName: str
     ) -> DescribeGlobalTableOutputTypeDef:
         """
         Returns information about the specified global table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_global_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_global_table)
         """
+
     async def describe_global_table_settings(
         self, *, GlobalTableName: str
     ) -> DescribeGlobalTableSettingsOutputTypeDef:
         """
         Describes Region-specific settings for a global table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_global_table_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_global_table_settings)
         """
+
     async def describe_import(self, *, ImportArn: str) -> DescribeImportOutputTypeDef:
         """
         Represents the properties of the import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_import)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_import)
         """
+
     async def describe_kinesis_streaming_destination(
         self, *, TableName: str
     ) -> DescribeKinesisStreamingDestinationOutputTypeDef:
         """
         Returns information about the status of Kinesis streaming.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_kinesis_streaming_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_kinesis_streaming_destination)
         """
+
     async def describe_limits(self) -> DescribeLimitsOutputTypeDef:
         """
         Returns the current provisioned-capacity quotas for your Amazon Web Services
         account in a Region, both for the Region as a whole and for any one DynamoDB
         table that you create there.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_limits)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_limits)
         """
+
     async def describe_table(self, *, TableName: str) -> DescribeTableOutputTypeDef:
         """
         Returns information about the table, including the current status of the table,
         when it was created, the primary key schema, and any indexes on the table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_table)
         """
+
     async def describe_table_replica_auto_scaling(
         self, *, TableName: str
     ) -> DescribeTableReplicaAutoScalingOutputTypeDef:
         """
         Describes auto scaling settings across replicas of the global table at once.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_table_replica_auto_scaling)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_table_replica_auto_scaling)
         """
+
     async def describe_time_to_live(self, *, TableName: str) -> DescribeTimeToLiveOutputTypeDef:
         """
         Gives a description of the Time to Live (TTL) status on the specified table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.describe_time_to_live)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#describe_time_to_live)
         """
+
     async def disable_kinesis_streaming_destination(
         self, *, TableName: str, StreamArn: str
     ) -> KinesisStreamingDestinationOutputTypeDef:
         """
         Stops replication from the DynamoDB table to the Kinesis data stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.disable_kinesis_streaming_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#disable_kinesis_streaming_destination)
         """
+
     async def enable_kinesis_streaming_destination(
         self, *, TableName: str, StreamArn: str
     ) -> KinesisStreamingDestinationOutputTypeDef:
         """
         Starts table data replication to the specified Kinesis data stream at a
         timestamp chosen during the enable workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.enable_kinesis_streaming_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#enable_kinesis_streaming_destination)
         """
+
     async def execute_statement(
         self,
         *,
         Statement: str,
-        Parameters: Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ] = ...,
+        Parameters: Sequence[UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         NextToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         Limit: int = ...
     ) -> ExecuteStatementOutputTypeDef:
         """
         This operation allows you to perform reads and singleton writes on data stored
         in DynamoDB, using PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.execute_statement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#execute_statement)
         """
+
     async def execute_transaction(
         self,
         *,
         TransactStatements: Sequence[ParameterizedStatementTypeDef],
         ClientRequestToken: str = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
     ) -> ExecuteTransactionOutputTypeDef:
         """
         This operation allows you to perform transactional reads or writes on data
         stored in DynamoDB, using PartiQL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.execute_transaction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#execute_transaction)
         """
+
     async def export_table_to_point_in_time(
         self,
         *,
         TableArn: str,
         S3Bucket: str,
-        ExportTime: Union[datetime, str] = ...,
+        ExportTime: TimestampTypeDef = ...,
         ClientToken: str = ...,
         S3BucketOwner: str = ...,
         S3Prefix: str = ...,
         S3SseAlgorithm: S3SseAlgorithmType = ...,
         S3SseKmsKeyId: str = ...,
         ExportFormat: ExportFormatType = ...
     ) -> ExportTableToPointInTimeOutputTypeDef:
         """
         Exports table data to an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.export_table_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#export_table_to_point_in_time)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#generate_presigned_url)
         """
+
     async def get_item(
         self,
         *,
         TableName: str,
-        Key: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        Key: Mapping[str, UniversalAttributeValueTypeDef],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...
     ) -> GetItemOutputTypeDef:
         """
         The `GetItem` operation returns a set of attributes for the item with the given
         primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_item)
         """
+
     async def import_table(
         self,
         *,
         S3BucketSource: S3BucketSourceTypeDef,
         InputFormat: InputFormatType,
-        TableCreationParameters: TableCreationParametersTypeDef,
+        TableCreationParameters: TableCreationParametersUnionTypeDef,
         ClientToken: str = ...,
-        InputFormatOptions: InputFormatOptionsTypeDef = ...,
+        InputFormatOptions: InputFormatOptionsUnionTypeDef = ...,
         InputCompressionType: InputCompressionTypeType = ...
     ) -> ImportTableOutputTypeDef:
         """
         Imports table data from an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.import_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#import_table)
         """
+
     async def list_backups(
         self,
         *,
         TableName: str = ...,
         Limit: int = ...,
-        TimeRangeLowerBound: Union[datetime, str] = ...,
-        TimeRangeUpperBound: Union[datetime, str] = ...,
+        TimeRangeLowerBound: TimestampTypeDef = ...,
+        TimeRangeUpperBound: TimestampTypeDef = ...,
         ExclusiveStartBackupArn: str = ...,
         BackupType: BackupTypeFilterType = ...
     ) -> ListBackupsOutputTypeDef:
         """
         List backups associated with an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_backups)
         """
+
     async def list_contributor_insights(
         self, *, TableName: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListContributorInsightsOutputTypeDef:
         """
         Returns a list of ContributorInsightsSummary for a table and all its global
         secondary indexes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_contributor_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_contributor_insights)
         """
+
     async def list_exports(
         self, *, TableArn: str = ..., MaxResults: int = ..., NextToken: str = ...
     ) -> ListExportsOutputTypeDef:
         """
         Lists completed exports within the past 90 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_exports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_exports)
         """
+
     async def list_global_tables(
         self, *, ExclusiveStartGlobalTableName: str = ..., Limit: int = ..., RegionName: str = ...
     ) -> ListGlobalTablesOutputTypeDef:
         """
         Lists all global tables that have a replica in the specified Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_global_tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_global_tables)
         """
+
     async def list_imports(
         self, *, TableArn: str = ..., PageSize: int = ..., NextToken: str = ...
     ) -> ListImportsOutputTypeDef:
         """
         Lists completed imports within the past 90 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_imports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_imports)
         """
+
     async def list_tables(
         self, *, ExclusiveStartTableName: str = ..., Limit: int = ...
     ) -> ListTablesOutputTypeDef:
         """
         Returns an array of table names associated with the current account and
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_tables)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_tables)
         """
+
     async def list_tags_of_resource(
         self, *, ResourceArn: str, NextToken: str = ...
     ) -> ListTagsOfResourceOutputTypeDef:
         """
         List all tags on an Amazon DynamoDB resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.list_tags_of_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#list_tags_of_resource)
         """
+
     async def put_item(
         self,
         *,
         TableName: str,
-        Item: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        Item: Mapping[str, UniversalAttributeValueTypeDef],
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
     ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#put_item)
         """
+
     async def query(
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         ConsistentRead: bool = ...,
         KeyConditions: Mapping[str, ConditionTypeDef] = ...,
         QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
-        ExclusiveStartKey: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...,
+        ExclusiveStartKey: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
     ) -> QueryOutputTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#query)
         """
+
     async def restore_table_from_backup(
         self,
         *,
         TargetTableName: str,
         BackupArn: str,
         BillingModeOverride: BillingModeType = ...,
-        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexTypeDef] = ...,
+        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...
     ) -> RestoreTableFromBackupOutputTypeDef:
         """
         Creates a new table from an existing backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.restore_table_from_backup)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#restore_table_from_backup)
         """
+
     async def restore_table_to_point_in_time(
         self,
         *,
         TargetTableName: str,
         SourceTableArn: str = ...,
         SourceTableName: str = ...,
         UseLatestRestorableTime: bool = ...,
-        RestoreDateTime: Union[datetime, str] = ...,
+        RestoreDateTime: TimestampTypeDef = ...,
         BillingModeOverride: BillingModeType = ...,
-        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexTypeDef] = ...,
+        GlobalSecondaryIndexOverride: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         LocalSecondaryIndexOverride: Sequence[LocalSecondaryIndexTypeDef] = ...,
         ProvisionedThroughputOverride: ProvisionedThroughputTypeDef = ...,
         SSESpecificationOverride: SSESpecificationTypeDef = ...
     ) -> RestoreTableToPointInTimeOutputTypeDef:
         """
         Restores the specified table to the specified point in time within
         `EarliestRestorableDateTime` and `LatestRestorableDateTime`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.restore_table_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#restore_table_to_point_in_time)
         """
+
     async def scan(
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         Select: SelectType = ...,
         ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
-        ExclusiveStartKey: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...,
+        ExclusiveStartKey: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...
     ) -> ScanOutputTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.scan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#scan)
         """
+
     async def tag_resource(
         self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associate a set of tags with an Amazon DynamoDB resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#tag_resource)
         """
+
     async def transact_get_items(
         self,
         *,
         TransactItems: Sequence[TransactGetItemTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
     ) -> TransactGetItemsOutputTypeDef:
         """
         `TransactGetItems` is a synchronous operation that atomically retrieves multiple
         items from one or more tables (but not from indexes) in a single account and
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.transact_get_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#transact_get_items)
         """
+
     async def transact_write_items(
         self,
         *,
         TransactItems: Sequence[TransactWriteItemTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ClientRequestToken: str = ...
@@ -973,58 +814,63 @@
         """
         `TransactWriteItems` is a synchronous write operation that groups up to 100
         action requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.transact_write_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#transact_write_items)
         """
+
     async def untag_resource(
         self, *, ResourceArn: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Removes the association of tags from an Amazon DynamoDB resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#untag_resource)
         """
+
     async def update_continuous_backups(
         self,
         *,
         TableName: str,
         PointInTimeRecoverySpecification: PointInTimeRecoverySpecificationTypeDef
     ) -> UpdateContinuousBackupsOutputTypeDef:
         """
         `UpdateContinuousBackups` enables or disables point in time recovery for the
         specified table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_continuous_backups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_continuous_backups)
         """
+
     async def update_contributor_insights(
         self,
         *,
         TableName: str,
         ContributorInsightsAction: ContributorInsightsActionType,
         IndexName: str = ...
     ) -> UpdateContributorInsightsOutputTypeDef:
         """
         Updates the status for contributor insights for a specific table or index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_contributor_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_contributor_insights)
         """
+
     async def update_global_table(
         self, *, GlobalTableName: str, ReplicaUpdates: Sequence[ReplicaUpdateTypeDef]
     ) -> UpdateGlobalTableOutputTypeDef:
         """
         Adds or removes replicas in the specified global table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_global_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_global_table)
         """
+
     async def update_global_table_settings(
         self,
         *,
         GlobalTableName: str,
         GlobalTableBillingMode: BillingModeType = ...,
         GlobalTableProvisionedWriteCapacityUnits: int = ...,
         GlobalTableProvisionedWriteCapacityAutoScalingSettingsUpdate: AutoScalingSettingsUpdateTypeDef = ...,
@@ -1035,79 +881,39 @@
     ) -> UpdateGlobalTableSettingsOutputTypeDef:
         """
         Updates settings for a global table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_global_table_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_global_table_settings)
         """
+
     async def update_item(
         self,
         *,
         TableName: str,
-        Key: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        Key: Mapping[str, UniversalAttributeValueTypeDef],
         AttributeUpdates: Mapping[str, AttributeValueUpdateTypeDef] = ...,
         Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
         ConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ] = ...
+        ExpressionAttributeValues: Mapping[str, UniversalAttributeValueTypeDef] = ...
     ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_item)
         """
+
     async def update_table(
         self,
         *,
         TableName: str,
         AttributeDefinitions: Sequence[AttributeDefinitionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
         ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
@@ -1121,85 +927,96 @@
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_table)
         """
+
     async def update_table_replica_auto_scaling(
         self,
         *,
         TableName: str,
         GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef] = ...,
         ProvisionedWriteCapacityAutoScalingUpdate: AutoScalingSettingsUpdateTypeDef = ...,
         ReplicaUpdates: Sequence[ReplicaAutoScalingUpdateTypeDef] = ...
     ) -> UpdateTableReplicaAutoScalingOutputTypeDef:
         """
         Updates auto scaling settings on your global tables at once.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_table_replica_auto_scaling)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_table_replica_auto_scaling)
         """
+
     async def update_time_to_live(
         self, *, TableName: str, TimeToLiveSpecification: TimeToLiveSpecificationTypeDef
     ) -> UpdateTimeToLiveOutputTypeDef:
         """
         The `UpdateTimeToLive` method enables or disables Time to Live (TTL) for the
         specified table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.update_time_to_live)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#update_time_to_live)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_backups"]) -> ListBackupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_tables"]) -> ListTablesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_of_resource"]
     ) -> ListTagsOfResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["query"]) -> QueryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["scan"]) -> ScanPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_paginator)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["table_exists"]) -> TableExistsWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["table_not_exists"]) -> TableNotExistsWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/#get_waiter)
         """
+
     async def __aenter__(self) -> "DynamoDBClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/client/)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/literals.py` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/literals.pyi` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/paginator.py` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/paginator.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,35 +24,35 @@
         list_backups_paginator: ListBackupsPaginator = client.get_paginator("list_backups")
         list_tables_paginator: ListTablesPaginator = client.get_paginator("list_tables")
         list_tags_of_resource_paginator: ListTagsOfResourcePaginator = client.get_paginator("list_tags_of_resource")
         query_paginator: QueryPaginator = client.get_paginator("query")
         scan_paginator: ScanPaginator = client.get_paginator("scan")
     ```
 """
-from datetime import datetime
-from decimal import Decimal
-from typing import Any, AsyncIterator, Generic, Iterator, Mapping, Sequence, Set, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Mapping, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import (
     BackupTypeFilterType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     SelectType,
 )
 from .type_defs import (
-    ConditionTableTypeDef,
-    ListBackupsOutputTableTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTagsOfResourceOutputTableTypeDef,
+    ConditionTypeDef,
+    ListBackupsOutputTypeDef,
+    ListTablesOutputTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     PaginatorConfigTypeDef,
-    QueryOutputTableTypeDef,
-    ScanOutputTableTypeDef,
+    QueryOutputTypeDef,
+    ScanOutputTypeDef,
+    TableAttributeValueTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListBackupsPaginator",
     "ListTablesPaginator",
     "ListTagsOfResourcePaginator",
     "QueryPaginator",
@@ -76,49 +76,49 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listbackupspaginator)
     """
 
     def paginate(
         self,
         *,
         TableName: str = ...,
-        TimeRangeLowerBound: Union[datetime, str] = ...,
-        TimeRangeUpperBound: Union[datetime, str] = ...,
+        TimeRangeLowerBound: TimestampTypeDef = ...,
+        TimeRangeUpperBound: TimestampTypeDef = ...,
         BackupType: BackupTypeFilterType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[ListBackupsOutputTableTypeDef]:
+    ) -> AsyncIterator[ListBackupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listbackupspaginator)
         """
 
 
 class ListTablesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtablespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[ListTablesOutputTableTypeDef]:
+    ) -> AsyncIterator[ListTablesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtablespaginator)
         """
 
 
 class ListTagsOfResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtagsofresourcepaginator)
     """
 
     def paginate(
         self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[ListTagsOfResourceOutputTableTypeDef]:
+    ) -> AsyncIterator[ListTagsOfResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtagsofresourcepaginator)
         """
 
 
 class QueryPaginator(AioPaginator):
@@ -131,44 +131,26 @@
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
-        KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,
-        QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        KeyConditions: Mapping[str, ConditionTypeDef] = ...,
+        QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[QueryOutputTableTypeDef]:
+    ) -> AsyncIterator[QueryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#querypaginator)
         """
 
 
 class ScanPaginator(AioPaginator):
@@ -180,41 +162,23 @@
     def paginate(
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Select: SelectType = ...,
-        ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[ScanOutputTableTypeDef]:
+    ) -> AsyncIterator[ScanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/paginator.pyi` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/paginator.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -24,35 +24,35 @@
         list_backups_paginator: ListBackupsPaginator = client.get_paginator("list_backups")
         list_tables_paginator: ListTablesPaginator = client.get_paginator("list_tables")
         list_tags_of_resource_paginator: ListTagsOfResourcePaginator = client.get_paginator("list_tags_of_resource")
         query_paginator: QueryPaginator = client.get_paginator("query")
         scan_paginator: ScanPaginator = client.get_paginator("scan")
     ```
 """
-from datetime import datetime
-from decimal import Decimal
-from typing import Any, AsyncIterator, Generic, Iterator, Mapping, Sequence, Set, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Mapping, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import (
     BackupTypeFilterType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     SelectType,
 )
 from .type_defs import (
-    ConditionTableTypeDef,
-    ListBackupsOutputTableTypeDef,
-    ListTablesOutputTableTypeDef,
-    ListTagsOfResourceOutputTableTypeDef,
+    ConditionTypeDef,
+    ListBackupsOutputTypeDef,
+    ListTablesOutputTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     PaginatorConfigTypeDef,
-    QueryOutputTableTypeDef,
-    ScanOutputTableTypeDef,
+    QueryOutputTypeDef,
+    ScanOutputTypeDef,
+    TableAttributeValueTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListBackupsPaginator",
     "ListTablesPaginator",
     "ListTagsOfResourcePaginator",
     "QueryPaginator",
@@ -73,47 +73,47 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listbackupspaginator)
     """
 
     def paginate(
         self,
         *,
         TableName: str = ...,
-        TimeRangeLowerBound: Union[datetime, str] = ...,
-        TimeRangeUpperBound: Union[datetime, str] = ...,
+        TimeRangeLowerBound: TimestampTypeDef = ...,
+        TimeRangeUpperBound: TimestampTypeDef = ...,
         BackupType: BackupTypeFilterType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[ListBackupsOutputTableTypeDef]:
+    ) -> AsyncIterator[ListBackupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listbackupspaginator)
         """
 
 class ListTablesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtablespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[ListTablesOutputTableTypeDef]:
+    ) -> AsyncIterator[ListTablesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtablespaginator)
         """
 
 class ListTagsOfResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtagsofresourcepaginator)
     """
 
     def paginate(
         self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[ListTagsOfResourceOutputTableTypeDef]:
+    ) -> AsyncIterator[ListTagsOfResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#listtagsofresourcepaginator)
         """
 
 class QueryPaginator(AioPaginator):
     """
@@ -125,44 +125,26 @@
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
-        KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,
-        QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        KeyConditions: Mapping[str, ConditionTypeDef] = ...,
+        QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         KeyConditionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[QueryOutputTableTypeDef]:
+    ) -> AsyncIterator[QueryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#querypaginator)
         """
 
 class ScanPaginator(AioPaginator):
     """
@@ -173,41 +155,23 @@
     def paginate(
         self,
         *,
         TableName: str,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Select: SelectType = ...,
-        ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
         FilterExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[ScanOutputTableTypeDef]:
+    ) -> AsyncIterator[ScanOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/paginators/#scanpaginator)
         """
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/service_resource.py` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/service_resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,80 +15,64 @@
     async with session.resource("dynamodb") as resource:
         resource: DynamoDBServiceResource
 
         my_table: dynamodb_resources.Table = resource.Table(...)
 ```
 """
 from datetime import datetime
-from decimal import Decimal
-from typing import (
-    Any,
-    AsyncIterator,
-    Awaitable,
-    List,
-    Mapping,
-    NoReturn,
-    Optional,
-    Sequence,
-    Set,
-    Union,
-)
+from typing import AsyncIterator, Awaitable, List, Mapping, NoReturn, Optional, Sequence
 
 from .client import DynamoDBClient
 from .literals import (
     BillingModeType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     ReturnItemCollectionMetricsType,
     ReturnValueType,
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
-    ArchivalSummaryTableResponseMetadataTypeDef,
-    AttributeDefinitionServiceResourceTypeDef,
-    AttributeDefinitionTableOutputTypeDef,
-    AttributeDefinitionTableTypeDef,
-    AttributeValueUpdateTableTypeDef,
-    BatchGetItemOutputServiceResourceTypeDef,
-    BatchWriteItemOutputServiceResourceTypeDef,
-    BillingModeSummaryTableResponseMetadataTypeDef,
-    ConditionTableTypeDef,
-    DeleteItemOutputTableTypeDef,
-    DeleteTableOutputTableTypeDef,
-    ExpectedAttributeValueTableTypeDef,
-    GetItemOutputTableTypeDef,
-    GlobalSecondaryIndexDescriptionTableTypeDef,
-    GlobalSecondaryIndexServiceResourceTypeDef,
-    GlobalSecondaryIndexUpdateTableTypeDef,
-    KeysAndAttributesServiceResourceTypeDef,
-    KeySchemaElementServiceResourceTypeDef,
-    KeySchemaElementTableOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
-    LocalSecondaryIndexServiceResourceTypeDef,
-    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
-    ProvisionedThroughputServiceResourceTypeDef,
-    ProvisionedThroughputTableTypeDef,
-    PutItemOutputTableTypeDef,
-    QueryOutputTableTypeDef,
-    ReplicaDescriptionTableTypeDef,
-    ReplicationGroupUpdateTableTypeDef,
-    RestoreSummaryTableResponseMetadataTypeDef,
-    ScanOutputTableTypeDef,
-    SSEDescriptionTableResponseMetadataTypeDef,
-    SSESpecificationServiceResourceTypeDef,
-    SSESpecificationTableTypeDef,
-    StreamSpecificationServiceResourceTypeDef,
-    StreamSpecificationTableResponseMetadataTypeDef,
-    StreamSpecificationTableTypeDef,
-    TableClassSummaryTableResponseMetadataTypeDef,
-    TagServiceResourceTypeDef,
-    UpdateItemOutputTableTypeDef,
-    WriteRequestServiceResourceTypeDef,
+    ArchivalSummaryResponseTypeDef,
+    AttributeDefinitionTypeDef,
+    AttributeValueUpdateTypeDef,
+    BatchGetItemOutputTypeDef,
+    BatchWriteItemOutputTypeDef,
+    BillingModeSummaryResponseTypeDef,
+    ConditionBaseImportTypeDef,
+    ConditionTypeDef,
+    DeleteItemOutputTypeDef,
+    DeleteTableOutputTypeDef,
+    ExpectedAttributeValueTypeDef,
+    GetItemOutputTypeDef,
+    GlobalSecondaryIndexDescriptionTypeDef,
+    GlobalSecondaryIndexUnionTypeDef,
+    GlobalSecondaryIndexUpdateTypeDef,
+    KeysAndAttributesUnionTypeDef,
+    KeySchemaElementTypeDef,
+    LocalSecondaryIndexDescriptionTypeDef,
+    LocalSecondaryIndexTypeDef,
+    ProvisionedThroughputDescriptionResponseTypeDef,
+    ProvisionedThroughputTypeDef,
+    PutItemOutputTypeDef,
+    QueryOutputTypeDef,
+    ReplicaDescriptionTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    RestoreSummaryResponseTypeDef,
+    ScanOutputTypeDef,
+    SSEDescriptionResponseTypeDef,
+    SSESpecificationTypeDef,
+    StreamSpecificationResponseTypeDef,
+    StreamSpecificationTypeDef,
+    TableAttributeValueTypeDef,
+    TableClassSummaryResponseTypeDef,
+    TagTypeDef,
+    UpdateItemOutputTypeDef,
+    WriteRequestUnionTypeDef,
 )
 
 try:
     from aioboto3.dynamodb.table import BatchWriter
 except (ModuleNotFoundError, ImportError):
     from builtins import object as BatchWriter
 try:
@@ -96,18 +80,14 @@
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOBoto3ServiceResource
 try:
     from aioboto3.resources.collection import AIOResourceCollection
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOResourceCollection
 try:
-    from boto3.dynamodb.conditions import ConditionBase
-except (ModuleNotFoundError, ImportError):
-    from builtins import object as ConditionBase
-try:
     from boto3.resources.base import ResourceMeta
 except (ModuleNotFoundError, ImportError):
     from builtins import object as ResourceMeta
 
 
 __all__ = ("DynamoDBServiceResource", "Table", "ServiceResourceTablesCollection")
 
@@ -179,36 +159,36 @@
 
 class Table(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#table)
     """
 
-    attribute_definitions: Awaitable[List[AttributeDefinitionTableOutputTypeDef]]
+    attribute_definitions: Awaitable[List[AttributeDefinitionTypeDef]]
     table_name: Awaitable[str]
-    key_schema: Awaitable[List[KeySchemaElementTableOutputTypeDef]]
+    key_schema: Awaitable[List[KeySchemaElementTypeDef]]
     table_status: Awaitable[TableStatusType]
     creation_date_time: Awaitable[datetime]
-    provisioned_throughput: Awaitable[ProvisionedThroughputDescriptionTableResponseMetadataTypeDef]
+    provisioned_throughput: Awaitable[ProvisionedThroughputDescriptionResponseTypeDef]
     table_size_bytes: Awaitable[int]
     item_count: Awaitable[int]
     table_arn: Awaitable[str]
     table_id: Awaitable[str]
-    billing_mode_summary: Awaitable[BillingModeSummaryTableResponseMetadataTypeDef]
-    local_secondary_indexes: Awaitable[List[LocalSecondaryIndexDescriptionTableTypeDef]]
-    global_secondary_indexes: Awaitable[List[GlobalSecondaryIndexDescriptionTableTypeDef]]
-    stream_specification: Awaitable[StreamSpecificationTableResponseMetadataTypeDef]
+    billing_mode_summary: Awaitable[BillingModeSummaryResponseTypeDef]
+    local_secondary_indexes: Awaitable[List[LocalSecondaryIndexDescriptionTypeDef]]
+    global_secondary_indexes: Awaitable[List[GlobalSecondaryIndexDescriptionTypeDef]]
+    stream_specification: Awaitable[StreamSpecificationResponseTypeDef]
     latest_stream_label: Awaitable[str]
     latest_stream_arn: Awaitable[str]
     global_table_version: Awaitable[str]
-    replicas: Awaitable[List[ReplicaDescriptionTableTypeDef]]
-    restore_summary: Awaitable[RestoreSummaryTableResponseMetadataTypeDef]
-    sse_description: Awaitable[SSEDescriptionTableResponseMetadataTypeDef]
-    archival_summary: Awaitable[ArchivalSummaryTableResponseMetadataTypeDef]
-    table_class_summary: Awaitable[TableClassSummaryTableResponseMetadataTypeDef]
+    replicas: Awaitable[List[ReplicaDescriptionTypeDef]]
+    restore_summary: Awaitable[RestoreSummaryResponseTypeDef]
+    sse_description: Awaitable[SSEDescriptionResponseTypeDef]
+    archival_summary: Awaitable[ArchivalSummaryResponseTypeDef]
+    table_class_summary: Awaitable[TableClassSummaryResponseTypeDef]
     deletion_protection_enabled: Awaitable[bool]
     name: str
 
     def batch_writer(
         self,
         overwrite_by_pkeys: Optional[List[str]] = ...,
         flush_amount: int = ...,
@@ -217,71 +197,35 @@
         """
         Create a batch writer object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablebatch_writer-method)
         """
 
-    async def delete(self) -> DeleteTableOutputTableTypeDef:
+    async def delete(self) -> DeleteTableOutputTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete-method)
         """
 
     async def delete_item(
         self,
         *,
-        Key: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
+        Key: Mapping[str, TableAttributeValueTypeDef],
+        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
-        ConditionExpression: Union[str, ConditionBase] = ...,
+        ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...
-    ) -> DeleteItemOutputTableTypeDef:
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+    ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete_item-method)
         """
 
@@ -292,39 +236,21 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableget_available_subresources-method)
         """
 
     async def get_item(
         self,
         *,
-        Key: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        Key: Mapping[str, TableAttributeValueTypeDef],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...
-    ) -> GetItemOutputTableTypeDef:
+    ) -> GetItemOutputTypeDef:
         """
         The `GetItem` operation returns a set of attributes for the item with the given
         primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableget_item-method)
         """
@@ -337,60 +263,24 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableload-method)
         """
 
     async def put_item(
         self,
         *,
-        Item: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
+        Item: Mapping[str, TableAttributeValueTypeDef],
+        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
-        ConditionExpression: Union[str, ConditionBase] = ...,
+        ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...
-    ) -> PutItemOutputTableTypeDef:
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+    ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableput_item-method)
         """
 
@@ -398,62 +288,26 @@
         self,
         *,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         ConsistentRead: bool = ...,
-        KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,
-        QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        KeyConditions: Mapping[str, ConditionTypeDef] = ...,
+        QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
-        ExclusiveStartKey: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExclusiveStartKey: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
-        FilterExpression: Union[str, ConditionBase] = ...,
-        KeyConditionExpression: Union[str, ConditionBase] = ...,
+        FilterExpression: ConditionBaseImportTypeDef = ...,
+        KeyConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...
-    ) -> QueryOutputTableTypeDef:
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+    ) -> QueryOutputTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablequery-method)
         """
@@ -470,142 +324,70 @@
     async def scan(
         self,
         *,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         Select: SelectType = ...,
-        ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
-        ExclusiveStartKey: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExclusiveStartKey: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
-        FilterExpression: Union[str, ConditionBase] = ...,
+        FilterExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...
-    ) -> ScanOutputTableTypeDef:
+    ) -> ScanOutputTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablescan-method)
         """
 
     async def update(
         self,
         *,
-        AttributeDefinitions: Sequence[AttributeDefinitionTableTypeDef] = ...,
+        AttributeDefinitions: Sequence[AttributeDefinitionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
-        ProvisionedThroughput: ProvisionedThroughputTableTypeDef = ...,
-        GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTableTypeDef] = ...,
-        StreamSpecification: StreamSpecificationTableTypeDef = ...,
-        SSESpecification: SSESpecificationTableTypeDef = ...,
-        ReplicaUpdates: Sequence[ReplicationGroupUpdateTableTypeDef] = ...,
+        ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
+        GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,
+        StreamSpecification: StreamSpecificationTypeDef = ...,
+        SSESpecification: SSESpecificationTypeDef = ...,
+        ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
     ) -> "_Table":
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableupdate-method)
         """
 
     async def update_item(
         self,
         *,
-        Key: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        AttributeUpdates: Mapping[str, AttributeValueUpdateTableTypeDef] = ...,
-        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
+        Key: Mapping[str, TableAttributeValueTypeDef],
+        AttributeUpdates: Mapping[str, AttributeValueUpdateTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
-        ConditionExpression: Union[str, ConditionBase] = ...,
+        ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...
-    ) -> UpdateItemOutputTableTypeDef:
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+    ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableupdate_item-method)
         """
@@ -650,53 +432,53 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcetable-method)
         """
 
     async def batch_get_item(
         self,
         *,
-        RequestItems: Mapping[str, KeysAndAttributesServiceResourceTypeDef],
+        RequestItems: Mapping[str, KeysAndAttributesUnionTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
-    ) -> BatchGetItemOutputServiceResourceTypeDef:
+    ) -> BatchGetItemOutputTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcebatch_get_item-method)
         """
 
     async def batch_write_item(
         self,
         *,
-        RequestItems: Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
+        RequestItems: Mapping[str, Sequence[WriteRequestUnionTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
-    ) -> BatchWriteItemOutputServiceResourceTypeDef:
+    ) -> BatchWriteItemOutputTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_write_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcebatch_write_item-method)
         """
 
     async def create_table(
         self,
         *,
-        AttributeDefinitions: Sequence[AttributeDefinitionServiceResourceTypeDef],
+        AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],
         TableName: str,
-        KeySchema: Sequence[KeySchemaElementServiceResourceTypeDef],
-        LocalSecondaryIndexes: Sequence[LocalSecondaryIndexServiceResourceTypeDef] = ...,
-        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexServiceResourceTypeDef] = ...,
+        KeySchema: Sequence[KeySchemaElementTypeDef],
+        LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,
+        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
-        ProvisionedThroughput: ProvisionedThroughputServiceResourceTypeDef = ...,
-        StreamSpecification: StreamSpecificationServiceResourceTypeDef = ...,
-        SSESpecification: SSESpecificationServiceResourceTypeDef = ...,
-        Tags: Sequence[TagServiceResourceTypeDef] = ...,
+        ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
+        StreamSpecification: StreamSpecificationTypeDef = ...,
+        SSESpecification: SSESpecificationTypeDef = ...,
+        Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
     ) -> _Table:
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.create_table)
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/service_resource.pyi` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/service_resource.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -15,80 +15,64 @@
     async with session.resource("dynamodb") as resource:
         resource: DynamoDBServiceResource
 
         my_table: dynamodb_resources.Table = resource.Table(...)
 ```
 """
 from datetime import datetime
-from decimal import Decimal
-from typing import (
-    Any,
-    AsyncIterator,
-    Awaitable,
-    List,
-    Mapping,
-    NoReturn,
-    Optional,
-    Sequence,
-    Set,
-    Union,
-)
+from typing import AsyncIterator, Awaitable, List, Mapping, NoReturn, Optional, Sequence
 
 from .client import DynamoDBClient
 from .literals import (
     BillingModeType,
     ConditionalOperatorType,
     ReturnConsumedCapacityType,
     ReturnItemCollectionMetricsType,
     ReturnValueType,
     SelectType,
     TableClassType,
     TableStatusType,
 )
 from .type_defs import (
-    ArchivalSummaryTableResponseMetadataTypeDef,
-    AttributeDefinitionServiceResourceTypeDef,
-    AttributeDefinitionTableOutputTypeDef,
-    AttributeDefinitionTableTypeDef,
-    AttributeValueUpdateTableTypeDef,
-    BatchGetItemOutputServiceResourceTypeDef,
-    BatchWriteItemOutputServiceResourceTypeDef,
-    BillingModeSummaryTableResponseMetadataTypeDef,
-    ConditionTableTypeDef,
-    DeleteItemOutputTableTypeDef,
-    DeleteTableOutputTableTypeDef,
-    ExpectedAttributeValueTableTypeDef,
-    GetItemOutputTableTypeDef,
-    GlobalSecondaryIndexDescriptionTableTypeDef,
-    GlobalSecondaryIndexServiceResourceTypeDef,
-    GlobalSecondaryIndexUpdateTableTypeDef,
-    KeysAndAttributesServiceResourceTypeDef,
-    KeySchemaElementServiceResourceTypeDef,
-    KeySchemaElementTableOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
-    LocalSecondaryIndexServiceResourceTypeDef,
-    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
-    ProvisionedThroughputServiceResourceTypeDef,
-    ProvisionedThroughputTableTypeDef,
-    PutItemOutputTableTypeDef,
-    QueryOutputTableTypeDef,
-    ReplicaDescriptionTableTypeDef,
-    ReplicationGroupUpdateTableTypeDef,
-    RestoreSummaryTableResponseMetadataTypeDef,
-    ScanOutputTableTypeDef,
-    SSEDescriptionTableResponseMetadataTypeDef,
-    SSESpecificationServiceResourceTypeDef,
-    SSESpecificationTableTypeDef,
-    StreamSpecificationServiceResourceTypeDef,
-    StreamSpecificationTableResponseMetadataTypeDef,
-    StreamSpecificationTableTypeDef,
-    TableClassSummaryTableResponseMetadataTypeDef,
-    TagServiceResourceTypeDef,
-    UpdateItemOutputTableTypeDef,
-    WriteRequestServiceResourceTypeDef,
+    ArchivalSummaryResponseTypeDef,
+    AttributeDefinitionTypeDef,
+    AttributeValueUpdateTypeDef,
+    BatchGetItemOutputTypeDef,
+    BatchWriteItemOutputTypeDef,
+    BillingModeSummaryResponseTypeDef,
+    ConditionBaseImportTypeDef,
+    ConditionTypeDef,
+    DeleteItemOutputTypeDef,
+    DeleteTableOutputTypeDef,
+    ExpectedAttributeValueTypeDef,
+    GetItemOutputTypeDef,
+    GlobalSecondaryIndexDescriptionTypeDef,
+    GlobalSecondaryIndexUnionTypeDef,
+    GlobalSecondaryIndexUpdateTypeDef,
+    KeysAndAttributesUnionTypeDef,
+    KeySchemaElementTypeDef,
+    LocalSecondaryIndexDescriptionTypeDef,
+    LocalSecondaryIndexTypeDef,
+    ProvisionedThroughputDescriptionResponseTypeDef,
+    ProvisionedThroughputTypeDef,
+    PutItemOutputTypeDef,
+    QueryOutputTypeDef,
+    ReplicaDescriptionTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    RestoreSummaryResponseTypeDef,
+    ScanOutputTypeDef,
+    SSEDescriptionResponseTypeDef,
+    SSESpecificationTypeDef,
+    StreamSpecificationResponseTypeDef,
+    StreamSpecificationTypeDef,
+    TableAttributeValueTypeDef,
+    TableClassSummaryResponseTypeDef,
+    TagTypeDef,
+    UpdateItemOutputTypeDef,
+    WriteRequestUnionTypeDef,
 )
 
 try:
     from aioboto3.dynamodb.table import BatchWriter
 except (ModuleNotFoundError, ImportError):
     from builtins import object as BatchWriter
 try:
@@ -96,18 +80,14 @@
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOBoto3ServiceResource
 try:
     from aioboto3.resources.collection import AIOResourceCollection
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOResourceCollection
 try:
-    from boto3.dynamodb.conditions import ConditionBase
-except (ModuleNotFoundError, ImportError):
-    from builtins import object as ConditionBase
-try:
     from boto3.resources.base import ResourceMeta
 except (ModuleNotFoundError, ImportError):
     from builtins import object as ResourceMeta
 
 __all__ = ("DynamoDBServiceResource", "Table", "ServiceResourceTablesCollection")
 
 class ServiceResourceTablesCollection(AIOResourceCollection):
@@ -170,36 +150,36 @@
 
 class Table(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#table)
     """
 
-    attribute_definitions: Awaitable[List[AttributeDefinitionTableOutputTypeDef]]
+    attribute_definitions: Awaitable[List[AttributeDefinitionTypeDef]]
     table_name: Awaitable[str]
-    key_schema: Awaitable[List[KeySchemaElementTableOutputTypeDef]]
+    key_schema: Awaitable[List[KeySchemaElementTypeDef]]
     table_status: Awaitable[TableStatusType]
     creation_date_time: Awaitable[datetime]
-    provisioned_throughput: Awaitable[ProvisionedThroughputDescriptionTableResponseMetadataTypeDef]
+    provisioned_throughput: Awaitable[ProvisionedThroughputDescriptionResponseTypeDef]
     table_size_bytes: Awaitable[int]
     item_count: Awaitable[int]
     table_arn: Awaitable[str]
     table_id: Awaitable[str]
-    billing_mode_summary: Awaitable[BillingModeSummaryTableResponseMetadataTypeDef]
-    local_secondary_indexes: Awaitable[List[LocalSecondaryIndexDescriptionTableTypeDef]]
-    global_secondary_indexes: Awaitable[List[GlobalSecondaryIndexDescriptionTableTypeDef]]
-    stream_specification: Awaitable[StreamSpecificationTableResponseMetadataTypeDef]
+    billing_mode_summary: Awaitable[BillingModeSummaryResponseTypeDef]
+    local_secondary_indexes: Awaitable[List[LocalSecondaryIndexDescriptionTypeDef]]
+    global_secondary_indexes: Awaitable[List[GlobalSecondaryIndexDescriptionTypeDef]]
+    stream_specification: Awaitable[StreamSpecificationResponseTypeDef]
     latest_stream_label: Awaitable[str]
     latest_stream_arn: Awaitable[str]
     global_table_version: Awaitable[str]
-    replicas: Awaitable[List[ReplicaDescriptionTableTypeDef]]
-    restore_summary: Awaitable[RestoreSummaryTableResponseMetadataTypeDef]
-    sse_description: Awaitable[SSEDescriptionTableResponseMetadataTypeDef]
-    archival_summary: Awaitable[ArchivalSummaryTableResponseMetadataTypeDef]
-    table_class_summary: Awaitable[TableClassSummaryTableResponseMetadataTypeDef]
+    replicas: Awaitable[List[ReplicaDescriptionTypeDef]]
+    restore_summary: Awaitable[RestoreSummaryResponseTypeDef]
+    sse_description: Awaitable[SSEDescriptionResponseTypeDef]
+    archival_summary: Awaitable[ArchivalSummaryResponseTypeDef]
+    table_class_summary: Awaitable[TableClassSummaryResponseTypeDef]
     deletion_protection_enabled: Awaitable[bool]
     name: str
 
     def batch_writer(
         self,
         overwrite_by_pkeys: Optional[List[str]] = ...,
         flush_amount: int = ...,
@@ -207,70 +187,34 @@
     ) -> BatchWriter:
         """
         Create a batch writer object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.batch_writer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablebatch_writer-method)
         """
-    async def delete(self) -> DeleteTableOutputTableTypeDef:
+    async def delete(self) -> DeleteTableOutputTypeDef:
         """
         The `DeleteTable` operation deletes a table and all of its items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete-method)
         """
     async def delete_item(
         self,
         *,
-        Key: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
+        Key: Mapping[str, TableAttributeValueTypeDef],
+        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
-        ConditionExpression: Union[str, ConditionBase] = ...,
+        ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...
-    ) -> DeleteItemOutputTableTypeDef:
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+    ) -> DeleteItemOutputTypeDef:
         """
         Deletes a single item in a table by primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.delete_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tabledelete_item-method)
         """
     async def get_available_subresources(self) -> Sequence[str]:
@@ -279,39 +223,21 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableget_available_subresources-method)
         """
     async def get_item(
         self,
         *,
-        Key: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        Key: Mapping[str, TableAttributeValueTypeDef],
         AttributesToGet: Sequence[str] = ...,
         ConsistentRead: bool = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...
-    ) -> GetItemOutputTableTypeDef:
+    ) -> GetItemOutputTypeDef:
         """
         The `GetItem` operation returns a set of attributes for the item with the given
         primary key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableget_item-method)
         """
@@ -322,122 +248,50 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.load)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableload-method)
         """
     async def put_item(
         self,
         *,
-        Item: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
+        Item: Mapping[str, TableAttributeValueTypeDef],
+        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
-        ConditionExpression: Union[str, ConditionBase] = ...,
+        ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...
-    ) -> PutItemOutputTableTypeDef:
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+    ) -> PutItemOutputTypeDef:
         """
         Creates a new item, or replaces an old item with a new item.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.put_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableput_item-method)
         """
     async def query(
         self,
         *,
         IndexName: str = ...,
         Select: SelectType = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         ConsistentRead: bool = ...,
-        KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,
-        QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        KeyConditions: Mapping[str, ConditionTypeDef] = ...,
+        QueryFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ScanIndexForward: bool = ...,
-        ExclusiveStartKey: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExclusiveStartKey: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ProjectionExpression: str = ...,
-        FilterExpression: Union[str, ConditionBase] = ...,
-        KeyConditionExpression: Union[str, ConditionBase] = ...,
+        FilterExpression: ConditionBaseImportTypeDef = ...,
+        KeyConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...
-    ) -> QueryOutputTableTypeDef:
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+    ) -> QueryOutputTypeDef:
         """
         You must provide the name of the partition key attribute and a single value for
         that attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablequery-method)
         """
@@ -452,140 +306,68 @@
     async def scan(
         self,
         *,
         IndexName: str = ...,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         Select: SelectType = ...,
-        ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,
+        ScanFilter: Mapping[str, ConditionTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
-        ExclusiveStartKey: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExclusiveStartKey: Mapping[str, TableAttributeValueTypeDef] = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         TotalSegments: int = ...,
         Segment: int = ...,
         ProjectionExpression: str = ...,
-        FilterExpression: Union[str, ConditionBase] = ...,
+        FilterExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...,
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
         ConsistentRead: bool = ...
-    ) -> ScanOutputTableTypeDef:
+    ) -> ScanOutputTypeDef:
         """
         The `Scan` operation returns one or more items and item attributes by accessing
         every item in a table or a secondary index.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.scan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tablescan-method)
         """
     async def update(
         self,
         *,
-        AttributeDefinitions: Sequence[AttributeDefinitionTableTypeDef] = ...,
+        AttributeDefinitions: Sequence[AttributeDefinitionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
-        ProvisionedThroughput: ProvisionedThroughputTableTypeDef = ...,
-        GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTableTypeDef] = ...,
-        StreamSpecification: StreamSpecificationTableTypeDef = ...,
-        SSESpecification: SSESpecificationTableTypeDef = ...,
-        ReplicaUpdates: Sequence[ReplicationGroupUpdateTableTypeDef] = ...,
+        ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
+        GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,
+        StreamSpecification: StreamSpecificationTypeDef = ...,
+        SSESpecification: SSESpecificationTypeDef = ...,
+        ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
     ) -> "_Table":
         """
         Modifies the provisioned throughput settings, global secondary indexes, or
         DynamoDB Streams settings for a given table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableupdate-method)
         """
     async def update_item(
         self,
         *,
-        Key: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        AttributeUpdates: Mapping[str, AttributeValueUpdateTableTypeDef] = ...,
-        Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,
+        Key: Mapping[str, TableAttributeValueTypeDef],
+        AttributeUpdates: Mapping[str, AttributeValueUpdateTypeDef] = ...,
+        Expected: Mapping[str, ExpectedAttributeValueTypeDef] = ...,
         ConditionalOperator: ConditionalOperatorType = ...,
         ReturnValues: ReturnValueType = ...,
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,
         UpdateExpression: str = ...,
-        ConditionExpression: Union[str, ConditionBase] = ...,
+        ConditionExpression: ConditionBaseImportTypeDef = ...,
         ExpressionAttributeNames: Mapping[str, str] = ...,
-        ExpressionAttributeValues: Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ] = ...
-    ) -> UpdateItemOutputTableTypeDef:
+        ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...
+    ) -> UpdateItemOutputTypeDef:
         """
         Edits an existing item's attributes, or adds a new item to the table if it does
         not already exist.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Table.update_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#tableupdate_item-method)
         """
@@ -624,51 +406,51 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.Table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcetable-method)
         """
     async def batch_get_item(
         self,
         *,
-        RequestItems: Mapping[str, KeysAndAttributesServiceResourceTypeDef],
+        RequestItems: Mapping[str, KeysAndAttributesUnionTypeDef],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...
-    ) -> BatchGetItemOutputServiceResourceTypeDef:
+    ) -> BatchGetItemOutputTypeDef:
         """
         The `BatchGetItem` operation returns the attributes of one or more items from
         one or more tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_get_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcebatch_get_item-method)
         """
     async def batch_write_item(
         self,
         *,
-        RequestItems: Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
+        RequestItems: Mapping[str, Sequence[WriteRequestUnionTypeDef]],
         ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,
         ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...
-    ) -> BatchWriteItemOutputServiceResourceTypeDef:
+    ) -> BatchWriteItemOutputTypeDef:
         """
         The `BatchWriteItem` operation puts or deletes multiple items in one or more
         tables.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.batch_write_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/service_resource/#dynamodbserviceresourcebatch_write_item-method)
         """
     async def create_table(
         self,
         *,
-        AttributeDefinitions: Sequence[AttributeDefinitionServiceResourceTypeDef],
+        AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],
         TableName: str,
-        KeySchema: Sequence[KeySchemaElementServiceResourceTypeDef],
-        LocalSecondaryIndexes: Sequence[LocalSecondaryIndexServiceResourceTypeDef] = ...,
-        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexServiceResourceTypeDef] = ...,
+        KeySchema: Sequence[KeySchemaElementTypeDef],
+        LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,
+        GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,
         BillingMode: BillingModeType = ...,
-        ProvisionedThroughput: ProvisionedThroughputServiceResourceTypeDef = ...,
-        StreamSpecification: StreamSpecificationServiceResourceTypeDef = ...,
-        SSESpecification: SSESpecificationServiceResourceTypeDef = ...,
-        Tags: Sequence[TagServiceResourceTypeDef] = ...,
+        ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,
+        StreamSpecification: StreamSpecificationTypeDef = ...,
+        SSESpecification: SSESpecificationTypeDef = ...,
+        Tags: Sequence[TagTypeDef] = ...,
         TableClass: TableClassType = ...,
         DeletionProtectionEnabled: bool = ...
     ) -> _Table:
         """
         The `CreateTable` operation adds a new table to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.ServiceResource.create_table)
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/type_defs.py` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/type_defs.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_dynamodb.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
@@ -63,73 +63,44 @@
     from boto3.dynamodb.conditions import ConditionBase
 except (ModuleNotFoundError, ImportError):
     from builtins import object as ConditionBase
 
 
 __all__ = (
     "ResponseMetadataTypeDef",
-    "ArchivalSummaryTableTypeDef",
     "ArchivalSummaryTypeDef",
-    "AttributeDefinitionOutputTypeDef",
-    "AttributeDefinitionServiceResourceTypeDef",
-    "AttributeDefinitionTableOutputTypeDef",
-    "AttributeDefinitionTableTypeDef",
     "AttributeDefinitionTypeDef",
-    "AttributeValueServiceResourceTypeDef",
-    "AttributeValueTableTypeDef",
     "AttributeValueTypeDef",
-    "AttributeValueUpdateTableTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
-    "BackupSummaryTableTypeDef",
     "BackupSummaryTypeDef",
-    "KeysAndAttributesServiceResourceTypeDef",
-    "KeysAndAttributesServiceResourceOutputTypeDef",
+    "TableAttributeValueTypeDef",
     "BatchStatementErrorTypeDef",
-    "ItemCollectionMetricsServiceResourceTypeDef",
-    "BillingModeSummaryTableTypeDef",
     "BillingModeSummaryTypeDef",
-    "CapacityServiceResourceTypeDef",
-    "CapacityTableTypeDef",
     "CapacityTypeDef",
-    "ConditionTableTypeDef",
+    "ConditionBaseImportTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
     "ContributorInsightsSummaryTypeDef",
     "CreateBackupInputRequestTypeDef",
-    "KeySchemaElementTableTypeDef",
-    "ProjectionTableTypeDef",
-    "ProvisionedThroughputTableTypeDef",
     "KeySchemaElementTypeDef",
     "ProjectionTypeDef",
     "ProvisionedThroughputTypeDef",
     "ReplicaTypeDef",
     "CreateReplicaActionTypeDef",
-    "ProvisionedThroughputOverrideTableTypeDef",
     "ProvisionedThroughputOverrideTypeDef",
     "SSESpecificationTypeDef",
     "StreamSpecificationTypeDef",
     "TagTypeDef",
-    "KeySchemaElementServiceResourceTypeDef",
-    "ProvisionedThroughputServiceResourceTypeDef",
-    "SSESpecificationServiceResourceTypeDef",
-    "StreamSpecificationServiceResourceTypeDef",
-    "TagServiceResourceTypeDef",
     "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
     "DeleteBackupInputRequestTypeDef",
-    "DeleteGlobalSecondaryIndexActionTableTypeDef",
     "DeleteGlobalSecondaryIndexActionTypeDef",
-    "ExpectedAttributeValueTableTypeDef",
-    "ItemCollectionMetricsTableTypeDef",
     "DeleteReplicaActionTypeDef",
-    "DeleteReplicationGroupMemberActionTableTypeDef",
     "DeleteReplicationGroupMemberActionTypeDef",
-    "DeleteRequestServiceResourceOutputTypeDef",
-    "DeleteRequestServiceResourceTypeDef",
     "DeleteTableInputRequestTypeDef",
     "DescribeBackupInputRequestTypeDef",
     "DescribeContinuousBackupsInputRequestTypeDef",
     "DescribeContributorInsightsInputRequestTypeDef",
     "FailureExceptionTypeDef",
     "EndpointTypeDef",
     "DescribeExportInputRequestTypeDef",
@@ -141,250 +112,204 @@
     "KinesisDataStreamDestinationTypeDef",
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
     "ExportSummaryTypeDef",
-    "ExportTableToPointInTimeInputRequestTypeDef",
-    "GetItemInputTableGetItemTypeDef",
-    "KeySchemaElementTableOutputTypeDef",
-    "ProjectionTableOutputTypeDef",
-    "ProvisionedThroughputDescriptionTableTypeDef",
-    "KeySchemaElementOutputTypeDef",
+    "TimestampTypeDef",
     "ProjectionOutputTypeDef",
     "ProvisionedThroughputDescriptionTypeDef",
-    "ProvisionedThroughputOutputTypeDef",
-    "ProjectionServiceResourceTypeDef",
-    "ReplicaOutputTypeDef",
-    "S3BucketSourceOutputTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ListBackupsInputRequestTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
     "ListTablesInputRequestTypeDef",
     "ListTagsOfResourceInputRequestTypeDef",
-    "TagTableTypeDef",
-    "TagOutputTypeDef",
     "PointInTimeRecoverySpecificationTypeDef",
-    "ProvisionedThroughputOverrideOutputTypeDef",
-    "ProvisionedThroughputOverrideTableOutputTypeDef",
-    "PutRequestServiceResourceOutputTypeDef",
-    "PutRequestServiceResourceTypeDef",
-    "TableClassSummaryTableTypeDef",
     "TableClassSummaryTypeDef",
-    "RestoreSummaryTableTypeDef",
     "RestoreSummaryTypeDef",
-    "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
-    "SSESpecificationOutputTypeDef",
-    "SSESpecificationTableTypeDef",
-    "StreamSpecificationOutputTypeDef",
-    "StreamSpecificationTableOutputTypeDef",
-    "StreamSpecificationTableTypeDef",
     "TableBatchWriterRequestTypeDef",
-    "TimeToLiveSpecificationOutputTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
-    "ArchivalSummaryTableResponseMetadataTypeDef",
-    "BillingModeSummaryTableResponseMetadataTypeDef",
+    "ArchivalSummaryResponseTypeDef",
+    "BillingModeSummaryResponseTypeDef",
     "DescribeLimitsOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "KinesisStreamingDestinationOutputTypeDef",
-    "ListTablesOutputTableTypeDef",
     "ListTablesOutputTypeDef",
-    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
-    "RestoreSummaryTableResponseMetadataTypeDef",
-    "SSEDescriptionTableResponseMetadataTypeDef",
-    "StreamSpecificationTableResponseMetadataTypeDef",
-    "TableClassSummaryTableResponseMetadataTypeDef",
+    "ProvisionedThroughputDescriptionResponseTypeDef",
+    "RestoreSummaryResponseTypeDef",
+    "SSEDescriptionResponseTypeDef",
+    "StreamSpecificationResponseTypeDef",
+    "TableClassSummaryResponseTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
-    "AttributeValueUpdateTypeDef",
-    "BatchStatementRequestTypeDef",
-    "ConditionCheckTypeDef",
-    "ConditionTypeDef",
+    "UniversalAttributeValueTypeDef",
+    "AutoScalingPolicyDescriptionTypeDef",
+    "AutoScalingPolicyUpdateTypeDef",
+    "CreateBackupOutputTypeDef",
+    "ListBackupsOutputTypeDef",
     "DeleteRequestOutputTypeDef",
-    "DeleteRequestTypeDef",
-    "DeleteTypeDef",
-    "ExecuteStatementInputRequestTypeDef",
-    "ExpectedAttributeValueTypeDef",
-    "GetItemInputRequestTypeDef",
-    "GetTypeDef",
+    "GetItemInputTableGetItemTypeDef",
     "ItemCollectionMetricsTypeDef",
     "ItemResponseTypeDef",
     "KeysAndAttributesOutputTypeDef",
-    "KeysAndAttributesTypeDef",
-    "ParameterizedStatementTypeDef",
     "PutRequestOutputTypeDef",
-    "PutRequestTypeDef",
-    "PutTypeDef",
-    "UpdateTypeDef",
-    "AutoScalingPolicyDescriptionTypeDef",
-    "AutoScalingPolicyUpdateTypeDef",
-    "CreateBackupOutputTypeDef",
-    "ListBackupsOutputTableTypeDef",
-    "ListBackupsOutputTypeDef",
-    "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
     "BatchStatementResponseTypeDef",
-    "ConsumedCapacityServiceResourceTypeDef",
-    "ConsumedCapacityTableTypeDef",
     "ConsumedCapacityTypeDef",
-    "QueryInputTableQueryTypeDef",
-    "ScanInputTableScanTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
-    "CreateGlobalSecondaryIndexActionTableTypeDef",
-    "UpdateGlobalSecondaryIndexActionTableTypeDef",
     "LocalSecondaryIndexTypeDef",
     "CreateGlobalSecondaryIndexActionTypeDef",
     "GlobalSecondaryIndexTypeDef",
+    "SourceTableDetailsTypeDef",
     "UpdateGlobalSecondaryIndexActionTypeDef",
     "CreateGlobalTableInputRequestTypeDef",
-    "ReplicaGlobalSecondaryIndexTableTypeDef",
+    "GlobalTableTypeDef",
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexTypeDef",
+    "ListTagsOfResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "InputFormatOptionsOutputTypeDef",
     "InputFormatOptionsTypeDef",
-    "DeleteItemInputTableDeleteItemTypeDef",
-    "PutItemInputTablePutItemTypeDef",
-    "UpdateItemInputTableUpdateItemTypeDef",
     "ReplicaUpdateTypeDef",
     "DescribeContributorInsightsOutputTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DescribeExportOutputTypeDef",
     "ExportTableToPointInTimeOutputTypeDef",
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     "DescribeTableInputTableExistsWaitTypeDef",
     "DescribeTableInputTableNotExistsWaitTypeDef",
     "DescribeTimeToLiveOutputTypeDef",
     "ListExportsOutputTypeDef",
-    "LocalSecondaryIndexDescriptionTableTypeDef",
-    "GlobalSecondaryIndexDescriptionTableTypeDef",
+    "ExportTableToPointInTimeInputRequestTypeDef",
+    "ListBackupsInputRequestTypeDef",
+    "GlobalSecondaryIndexInfoTypeDef",
+    "GlobalSecondaryIndexOutputTypeDef",
     "LocalSecondaryIndexDescriptionTypeDef",
     "LocalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexDescriptionTypeDef",
-    "GlobalSecondaryIndexInfoTypeDef",
-    "GlobalSecondaryIndexOutputTypeDef",
-    "SourceTableDetailsTypeDef",
-    "GlobalSecondaryIndexServiceResourceTypeDef",
-    "LocalSecondaryIndexServiceResourceTypeDef",
-    "GlobalTableTypeDef",
     "ImportSummaryTypeDef",
     "ListBackupsInputListBackupsPaginateTypeDef",
     "ListTablesInputListTablesPaginateTypeDef",
     "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    "QueryInputQueryPaginateTypeDef",
-    "ScanInputScanPaginateTypeDef",
-    "ListTagsOfResourceOutputTableTypeDef",
-    "ListTagsOfResourceOutputTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
-    "WriteRequestServiceResourceOutputTypeDef",
-    "WriteRequestServiceResourceTypeDef",
-    "UpdateTimeToLiveOutputTypeDef",
     "UpdateTimeToLiveInputRequestTypeDef",
-    "BatchExecuteStatementInputRequestTypeDef",
-    "QueryInputRequestTypeDef",
-    "ScanInputRequestTypeDef",
-    "DeleteItemInputRequestTypeDef",
-    "PutItemInputRequestTypeDef",
-    "UpdateItemInputRequestTypeDef",
-    "TransactGetItemTypeDef",
-    "BatchGetItemInputRequestTypeDef",
-    "ExecuteTransactionInputRequestTypeDef",
-    "WriteRequestOutputTypeDef",
-    "WriteRequestTypeDef",
-    "TransactWriteItemTypeDef",
+    "UpdateTimeToLiveOutputTypeDef",
+    "AttributeValueUpdateTypeDef",
+    "BatchStatementRequestTypeDef",
+    "ConditionCheckTypeDef",
+    "ConditionTypeDef",
+    "DeleteRequestTypeDef",
+    "DeleteTypeDef",
+    "ExecuteStatementInputRequestTypeDef",
+    "ExpectedAttributeValueTypeDef",
+    "GetItemInputRequestTypeDef",
+    "GetTypeDef",
+    "KeysAndAttributesTypeDef",
+    "ParameterizedStatementTypeDef",
+    "PutRequestTypeDef",
+    "PutTypeDef",
+    "UpdateTypeDef",
     "AutoScalingSettingsDescriptionTypeDef",
     "AutoScalingSettingsUpdateTypeDef",
-    "BatchGetItemOutputServiceResourceTypeDef",
-    "DeleteItemOutputTableTypeDef",
-    "GetItemOutputTableTypeDef",
-    "PutItemOutputTableTypeDef",
-    "QueryOutputTableTypeDef",
-    "ScanOutputTableTypeDef",
-    "UpdateItemOutputTableTypeDef",
+    "WriteRequestOutputTypeDef",
     "BatchExecuteStatementOutputTypeDef",
     "BatchGetItemOutputTypeDef",
     "DeleteItemOutputTypeDef",
     "ExecuteStatementOutputTypeDef",
     "ExecuteTransactionOutputTypeDef",
     "GetItemOutputTypeDef",
     "PutItemOutputTypeDef",
     "QueryOutputTypeDef",
     "ScanOutputTypeDef",
     "TransactGetItemsOutputTypeDef",
     "TransactWriteItemsOutputTypeDef",
     "UpdateItemOutputTypeDef",
     "DescribeContinuousBackupsOutputTypeDef",
     "UpdateContinuousBackupsOutputTypeDef",
-    "GlobalSecondaryIndexUpdateTableTypeDef",
-    "CreateTableInputRequestTypeDef",
-    "RestoreTableFromBackupInputRequestTypeDef",
-    "RestoreTableToPointInTimeInputRequestTypeDef",
     "TableCreationParametersTypeDef",
     "GlobalSecondaryIndexUpdateTypeDef",
-    "CreateReplicationGroupMemberActionTableTypeDef",
-    "UpdateReplicationGroupMemberActionTableTypeDef",
+    "ListGlobalTablesOutputTypeDef",
+    "ReplicaDescriptionTypeDef",
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
+    "InputFormatOptionsUnionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
-    "SourceTableFeatureDetailsTypeDef",
+    "GlobalSecondaryIndexUnionTypeDef",
     "TableCreationParametersOutputTypeDef",
-    "CreateTableInputServiceResourceCreateTableTypeDef",
-    "ListGlobalTablesOutputTypeDef",
+    "SourceTableFeatureDetailsTypeDef",
     "ListImportsOutputTypeDef",
-    "ReplicaDescriptionTypeDef",
-    "ReplicaDescriptionTableTypeDef",
-    "BatchWriteItemOutputServiceResourceTypeDef",
-    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
-    "TransactGetItemsInputRequestTypeDef",
-    "BatchWriteItemOutputTypeDef",
-    "BatchWriteItemInputRequestTypeDef",
-    "TransactWriteItemsInputRequestTypeDef",
+    "BatchExecuteStatementInputRequestTypeDef",
+    "QueryInputQueryPaginateTypeDef",
+    "QueryInputRequestTypeDef",
+    "QueryInputTableQueryTypeDef",
+    "ScanInputRequestTypeDef",
+    "ScanInputScanPaginateTypeDef",
+    "ScanInputTableScanTypeDef",
+    "DeleteItemInputRequestTypeDef",
+    "DeleteItemInputTableDeleteItemTypeDef",
+    "PutItemInputRequestTypeDef",
+    "PutItemInputTablePutItemTypeDef",
+    "UpdateItemInputRequestTypeDef",
+    "UpdateItemInputTableUpdateItemTypeDef",
+    "TransactGetItemTypeDef",
+    "KeysAndAttributesUnionTypeDef",
+    "ExecuteTransactionInputRequestTypeDef",
+    "WriteRequestTypeDef",
+    "TransactWriteItemTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef",
+    "BatchWriteItemOutputTypeDef",
     "ImportTableInputRequestTypeDef",
-    "ReplicationGroupUpdateTableTypeDef",
-    "ReplicationGroupUpdateTypeDef",
-    "BackupDescriptionTypeDef",
-    "ImportTableDescriptionTypeDef",
     "GlobalTableDescriptionTypeDef",
     "TableDescriptionTypeDef",
-    "TableDescriptionTableTypeDef",
+    "ReplicationGroupUpdateTypeDef",
+    "CreateTableInputRequestTypeDef",
+    "CreateTableInputServiceResourceCreateTableTypeDef",
+    "RestoreTableFromBackupInputRequestTypeDef",
+    "RestoreTableToPointInTimeInputRequestTypeDef",
+    "ImportTableDescriptionTypeDef",
+    "TableCreationParametersUnionTypeDef",
+    "BackupDescriptionTypeDef",
+    "TransactGetItemsInputRequestTypeDef",
+    "BatchGetItemInputRequestTypeDef",
+    "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    "WriteRequestUnionTypeDef",
+    "TransactWriteItemsInputRequestTypeDef",
     "ReplicaAutoScalingDescriptionTypeDef",
     "ReplicaSettingsDescriptionTypeDef",
     "ReplicaAutoScalingUpdateTypeDef",
     "ReplicaSettingsUpdateTypeDef",
-    "UpdateTableInputTableUpdateTypeDef",
-    "UpdateTableInputRequestTypeDef",
-    "DeleteBackupOutputTypeDef",
-    "DescribeBackupOutputTypeDef",
-    "DescribeImportOutputTypeDef",
-    "ImportTableOutputTypeDef",
     "CreateGlobalTableOutputTypeDef",
     "DescribeGlobalTableOutputTypeDef",
     "UpdateGlobalTableOutputTypeDef",
     "CreateTableOutputTypeDef",
     "DeleteTableOutputTypeDef",
     "DescribeTableOutputTypeDef",
     "RestoreTableFromBackupOutputTypeDef",
     "RestoreTableToPointInTimeOutputTypeDef",
     "UpdateTableOutputTypeDef",
-    "DeleteTableOutputTableTypeDef",
+    "UpdateTableInputRequestTypeDef",
+    "UpdateTableInputTableUpdateTypeDef",
+    "DescribeImportOutputTypeDef",
+    "ImportTableOutputTypeDef",
+    "DeleteBackupOutputTypeDef",
+    "DescribeBackupOutputTypeDef",
+    "BatchWriteItemInputRequestTypeDef",
+    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "TableAutoScalingDescriptionTypeDef",
     "DescribeGlobalTableSettingsOutputTypeDef",
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
@@ -397,104 +322,32 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-ArchivalSummaryTableTypeDef = TypedDict(
-    "ArchivalSummaryTableTypeDef",
-    {
-        "ArchivalDateTime": datetime,
-        "ArchivalReason": str,
-        "ArchivalBackupArn": str,
-    },
-)
-
 ArchivalSummaryTypeDef = TypedDict(
     "ArchivalSummaryTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
-)
-
-AttributeDefinitionOutputTypeDef = TypedDict(
-    "AttributeDefinitionOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": ScalarAttributeTypeType,
-    },
-)
-
-AttributeDefinitionServiceResourceTypeDef = TypedDict(
-    "AttributeDefinitionServiceResourceTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": ScalarAttributeTypeType,
-    },
-)
-
-AttributeDefinitionTableOutputTypeDef = TypedDict(
-    "AttributeDefinitionTableOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": ScalarAttributeTypeType,
-    },
-)
-
-AttributeDefinitionTableTypeDef = TypedDict(
-    "AttributeDefinitionTableTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": ScalarAttributeTypeType,
-    },
+    total=False,
 )
 
 AttributeDefinitionTypeDef = TypedDict(
     "AttributeDefinitionTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
 
-AttributeValueServiceResourceTypeDef = TypedDict(
-    "AttributeValueServiceResourceTypeDef",
-    {
-        "S": str,
-        "N": str,
-        "B": bytes,
-        "SS": List[str],
-        "NS": List[str],
-        "BS": List[bytes],
-        "M": Dict[str, Dict[str, Any]],
-        "L": List[Dict[str, Any]],
-        "NULL": bool,
-        "BOOL": bool,
-    },
-)
-
-AttributeValueTableTypeDef = TypedDict(
-    "AttributeValueTableTypeDef",
-    {
-        "S": str,
-        "N": str,
-        "B": bytes,
-        "SS": List[str],
-        "NS": List[str],
-        "BS": List[bytes],
-        "M": Dict[str, Dict[str, Any]],
-        "L": List[Dict[str, Any]],
-        "NULL": bool,
-        "BOOL": bool,
-    },
-)
-
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "S": str,
         "N": str,
         "B": bytes,
         "SS": Sequence[str],
@@ -504,48 +357,38 @@
         "L": Sequence[Any],
         "NULL": bool,
         "BOOL": bool,
     },
     total=False,
 )
 
-AttributeValueUpdateTableTypeDef = TypedDict(
-    "AttributeValueUpdateTableTypeDef",
+_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
+    "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
-        "Value": Union[
-            bytes,
-            bytearray,
-            str,
-            int,
-            Decimal,
-            bool,
-            Set[int],
-            Set[Decimal],
-            Set[str],
-            Set[bytes],
-            Set[bytearray],
-            Sequence[Any],
-            Mapping[str, Any],
-            None,
-        ],
-        "Action": AttributeActionType,
+        "TargetValue": float,
     },
-    total=False,
 )
-
-AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
-    "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
+_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
+    "_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
-        "TargetValue": float,
     },
+    total=False,
 )
 
+
+class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(
+    _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
+    _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
+):
+    pass
+
+
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
@@ -562,261 +405,128 @@
 class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(
     _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
 ):
     pass
 
 
-BackupDetailsTypeDef = TypedDict(
-    "BackupDetailsTypeDef",
+_RequiredBackupDetailsTypeDef = TypedDict(
+    "_RequiredBackupDetailsTypeDef",
     {
         "BackupArn": str,
         "BackupName": str,
-        "BackupSizeBytes": int,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupCreationDateTime": datetime,
-        "BackupExpiryDateTime": datetime,
     },
 )
-
-BackupSummaryTableTypeDef = TypedDict(
-    "BackupSummaryTableTypeDef",
+_OptionalBackupDetailsTypeDef = TypedDict(
+    "_OptionalBackupDetailsTypeDef",
     {
-        "TableName": str,
-        "TableId": str,
-        "TableArn": str,
-        "BackupArn": str,
-        "BackupName": str,
-        "BackupCreationDateTime": datetime,
-        "BackupExpiryDateTime": datetime,
-        "BackupStatus": BackupStatusType,
-        "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
+        "BackupExpiryDateTime": datetime,
     },
+    total=False,
 )
 
+
+class BackupDetailsTypeDef(_RequiredBackupDetailsTypeDef, _OptionalBackupDetailsTypeDef):
+    pass
+
+
 BackupSummaryTypeDef = TypedDict(
     "BackupSummaryTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "TableArn": str,
         "BackupArn": str,
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
-)
-
-_RequiredKeysAndAttributesServiceResourceTypeDef = TypedDict(
-    "_RequiredKeysAndAttributesServiceResourceTypeDef",
-    {
-        "Keys": Sequence[
-            Mapping[
-                str,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
-    },
-)
-_OptionalKeysAndAttributesServiceResourceTypeDef = TypedDict(
-    "_OptionalKeysAndAttributesServiceResourceTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-    },
     total=False,
 )
 
-
-class KeysAndAttributesServiceResourceTypeDef(
-    _RequiredKeysAndAttributesServiceResourceTypeDef,
-    _OptionalKeysAndAttributesServiceResourceTypeDef,
-):
-    pass
-
-
-KeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
-    "KeysAndAttributesServiceResourceOutputTypeDef",
-    {
-        "Keys": List[Dict[str, "AttributeValueServiceResourceTypeDef"]],
-        "AttributesToGet": List[str],
-        "ConsistentRead": bool,
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Dict[str, str],
-    },
-)
-
+TableAttributeValueTypeDef = Union[
+    bytes,
+    bytearray,
+    str,
+    int,
+    Decimal,
+    bool,
+    Set[int],
+    Set[Decimal],
+    Set[str],
+    Set[bytes],
+    Set[bytearray],
+    Sequence[Any],
+    Mapping[str, Any],
+    None,
+]
 BatchStatementErrorTypeDef = TypedDict(
     "BatchStatementErrorTypeDef",
     {
         "Code": BatchStatementErrorCodeEnumType,
         "Message": str,
     },
-)
-
-ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
-    "ItemCollectionMetricsServiceResourceTypeDef",
-    {
-        "ItemCollectionKey": Dict[str, "AttributeValueServiceResourceTypeDef"],
-        "SizeEstimateRangeGB": List[float],
-    },
-)
-
-BillingModeSummaryTableTypeDef = TypedDict(
-    "BillingModeSummaryTableTypeDef",
-    {
-        "BillingMode": BillingModeType,
-        "LastUpdateToPayPerRequestDateTime": datetime,
-    },
+    total=False,
 )
 
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
-)
-
-CapacityServiceResourceTypeDef = TypedDict(
-    "CapacityServiceResourceTypeDef",
-    {
-        "ReadCapacityUnits": float,
-        "WriteCapacityUnits": float,
-        "CapacityUnits": float,
-    },
-)
-
-CapacityTableTypeDef = TypedDict(
-    "CapacityTableTypeDef",
-    {
-        "ReadCapacityUnits": float,
-        "WriteCapacityUnits": float,
-        "CapacityUnits": float,
-    },
+    total=False,
 )
 
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-)
-
-_RequiredConditionTableTypeDef = TypedDict(
-    "_RequiredConditionTableTypeDef",
-    {
-        "ComparisonOperator": ComparisonOperatorType,
-    },
-)
-_OptionalConditionTableTypeDef = TypedDict(
-    "_OptionalConditionTableTypeDef",
-    {
-        "AttributeValueList": Sequence[
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ],
-    },
     total=False,
 )
 
-
-class ConditionTableTypeDef(_RequiredConditionTableTypeDef, _OptionalConditionTableTypeDef):
-    pass
-
-
+ConditionBaseImportTypeDef = Union[str, ConditionBase]
 PointInTimeRecoveryDescriptionTypeDef = TypedDict(
     "PointInTimeRecoveryDescriptionTypeDef",
     {
         "PointInTimeRecoveryStatus": PointInTimeRecoveryStatusType,
         "EarliestRestorableDateTime": datetime,
         "LatestRestorableDateTime": datetime,
     },
+    total=False,
 )
 
 ContributorInsightsSummaryTypeDef = TypedDict(
     "ContributorInsightsSummaryTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
     },
+    total=False,
 )
 
 CreateBackupInputRequestTypeDef = TypedDict(
     "CreateBackupInputRequestTypeDef",
     {
         "TableName": str,
         "BackupName": str,
     },
 )
 
-KeySchemaElementTableTypeDef = TypedDict(
-    "KeySchemaElementTableTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": KeyTypeType,
-    },
-)
-
-ProjectionTableTypeDef = TypedDict(
-    "ProjectionTableTypeDef",
-    {
-        "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": Sequence[str],
-    },
-    total=False,
-)
-
-ProvisionedThroughputTableTypeDef = TypedDict(
-    "ProvisionedThroughputTableTypeDef",
-    {
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-)
-
 KeySchemaElementTypeDef = TypedDict(
     "KeySchemaElementTypeDef",
     {
         "AttributeName": str,
         "KeyType": KeyTypeType,
     },
 )
@@ -849,22 +559,14 @@
 CreateReplicaActionTypeDef = TypedDict(
     "CreateReplicaActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
-ProvisionedThroughputOverrideTableTypeDef = TypedDict(
-    "ProvisionedThroughputOverrideTableTypeDef",
-    {
-        "ReadCapacityUnits": int,
-    },
-    total=False,
-)
-
 ProvisionedThroughputOverrideTypeDef = TypedDict(
     "ProvisionedThroughputOverrideTypeDef",
     {
         "ReadCapacityUnits": int,
     },
     total=False,
 )
@@ -904,76 +606,21 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-KeySchemaElementServiceResourceTypeDef = TypedDict(
-    "KeySchemaElementServiceResourceTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": KeyTypeType,
-    },
-)
-
-ProvisionedThroughputServiceResourceTypeDef = TypedDict(
-    "ProvisionedThroughputServiceResourceTypeDef",
-    {
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-)
-
-SSESpecificationServiceResourceTypeDef = TypedDict(
-    "SSESpecificationServiceResourceTypeDef",
-    {
-        "Enabled": bool,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyId": str,
-    },
-    total=False,
-)
-
-_RequiredStreamSpecificationServiceResourceTypeDef = TypedDict(
-    "_RequiredStreamSpecificationServiceResourceTypeDef",
-    {
-        "StreamEnabled": bool,
-    },
-)
-_OptionalStreamSpecificationServiceResourceTypeDef = TypedDict(
-    "_OptionalStreamSpecificationServiceResourceTypeDef",
-    {
-        "StreamViewType": StreamViewTypeType,
-    },
-    total=False,
-)
-
-
-class StreamSpecificationServiceResourceTypeDef(
-    _RequiredStreamSpecificationServiceResourceTypeDef,
-    _OptionalStreamSpecificationServiceResourceTypeDef,
-):
-    pass
-
-
-TagServiceResourceTypeDef = TypedDict(
-    "TagServiceResourceTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 CsvOptionsOutputTypeDef = TypedDict(
     "CsvOptionsOutputTypeDef",
     {
         "Delimiter": str,
         "HeaderList": List[str],
     },
+    total=False,
 )
 
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderList": Sequence[str],
@@ -984,132 +631,35 @@
 DeleteBackupInputRequestTypeDef = TypedDict(
     "DeleteBackupInputRequestTypeDef",
     {
         "BackupArn": str,
     },
 )
 
-DeleteGlobalSecondaryIndexActionTableTypeDef = TypedDict(
-    "DeleteGlobalSecondaryIndexActionTableTypeDef",
-    {
-        "IndexName": str,
-    },
-)
-
 DeleteGlobalSecondaryIndexActionTypeDef = TypedDict(
     "DeleteGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
     },
 )
 
-ExpectedAttributeValueTableTypeDef = TypedDict(
-    "ExpectedAttributeValueTableTypeDef",
-    {
-        "Value": Union[
-            bytes,
-            bytearray,
-            str,
-            int,
-            Decimal,
-            bool,
-            Set[int],
-            Set[Decimal],
-            Set[str],
-            Set[bytes],
-            Set[bytearray],
-            Sequence[Any],
-            Mapping[str, Any],
-            None,
-        ],
-        "Exists": bool,
-        "ComparisonOperator": ComparisonOperatorType,
-        "AttributeValueList": Sequence[
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ],
-    },
-    total=False,
-)
-
-ItemCollectionMetricsTableTypeDef = TypedDict(
-    "ItemCollectionMetricsTableTypeDef",
-    {
-        "ItemCollectionKey": Dict[str, "AttributeValueTableTypeDef"],
-        "SizeEstimateRangeGB": List[float],
-    },
-)
-
 DeleteReplicaActionTypeDef = TypedDict(
     "DeleteReplicaActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
-DeleteReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "DeleteReplicationGroupMemberActionTableTypeDef",
-    {
-        "RegionName": str,
-    },
-)
-
 DeleteReplicationGroupMemberActionTypeDef = TypedDict(
     "DeleteReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
-DeleteRequestServiceResourceOutputTypeDef = TypedDict(
-    "DeleteRequestServiceResourceOutputTypeDef",
-    {
-        "Key": Dict[str, "AttributeValueServiceResourceTypeDef"],
-    },
-)
-
-DeleteRequestServiceResourceTypeDef = TypedDict(
-    "DeleteRequestServiceResourceTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-
 DeleteTableInputRequestTypeDef = TypedDict(
     "DeleteTableInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 
@@ -1151,14 +701,15 @@
 
 FailureExceptionTypeDef = TypedDict(
     "FailureExceptionTypeDef",
     {
         "ExceptionName": str,
         "ExceptionDescription": str,
     },
+    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "CachePeriodInMinutes": int,
@@ -1191,14 +742,15 @@
         "S3SseKmsKeyId": str,
         "FailureCode": str,
         "FailureMessage": str,
         "ExportFormat": ExportFormatType,
         "BilledSizeBytes": int,
         "ItemCount": int,
     },
+    total=False,
 )
 
 DescribeGlobalTableInputRequestTypeDef = TypedDict(
     "DescribeGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
@@ -1228,14 +780,15 @@
 KinesisDataStreamDestinationTypeDef = TypedDict(
     "KinesisDataStreamDestinationTypeDef",
     {
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "DestinationStatusDescription": str,
     },
+    total=False,
 )
 
 DescribeTableInputRequestTypeDef = TypedDict(
     "DescribeTableInputRequestTypeDef",
     {
         "TableName": str,
     },
@@ -1266,183 +819,48 @@
 
 TimeToLiveDescriptionTypeDef = TypedDict(
     "TimeToLiveDescriptionTypeDef",
     {
         "TimeToLiveStatus": TimeToLiveStatusType,
         "AttributeName": str,
     },
+    total=False,
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
-)
-
-_RequiredExportTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_RequiredExportTableToPointInTimeInputRequestTypeDef",
-    {
-        "TableArn": str,
-        "S3Bucket": str,
-    },
-)
-_OptionalExportTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_OptionalExportTableToPointInTimeInputRequestTypeDef",
-    {
-        "ExportTime": Union[datetime, str],
-        "ClientToken": str,
-        "S3BucketOwner": str,
-        "S3Prefix": str,
-        "S3SseAlgorithm": S3SseAlgorithmType,
-        "S3SseKmsKeyId": str,
-        "ExportFormat": ExportFormatType,
-    },
-    total=False,
-)
-
-
-class ExportTableToPointInTimeInputRequestTypeDef(
-    _RequiredExportTableToPointInTimeInputRequestTypeDef,
-    _OptionalExportTableToPointInTimeInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredGetItemInputTableGetItemTypeDef = TypedDict(
-    "_RequiredGetItemInputTableGetItemTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalGetItemInputTableGetItemTypeDef = TypedDict(
-    "_OptionalGetItemInputTableGetItemTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-    },
     total=False,
 )
 
-
-class GetItemInputTableGetItemTypeDef(
-    _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
-):
-    pass
-
-
-KeySchemaElementTableOutputTypeDef = TypedDict(
-    "KeySchemaElementTableOutputTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": KeyTypeType,
-    },
-)
-
-ProjectionTableOutputTypeDef = TypedDict(
-    "ProjectionTableOutputTypeDef",
-    {
-        "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": List[str],
-    },
-)
-
-ProvisionedThroughputDescriptionTableTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionTableTypeDef",
-    {
-        "LastIncreaseDateTime": datetime,
-        "LastDecreaseDateTime": datetime,
-        "NumberOfDecreasesToday": int,
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-)
-
-KeySchemaElementOutputTypeDef = TypedDict(
-    "KeySchemaElementOutputTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": KeyTypeType,
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ProjectionOutputTypeDef = TypedDict(
     "ProjectionOutputTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
         "NonKeyAttributes": List[str],
     },
+    total=False,
 )
 
 ProvisionedThroughputDescriptionTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
-)
-
-ProvisionedThroughputOutputTypeDef = TypedDict(
-    "ProvisionedThroughputOutputTypeDef",
-    {
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-)
-
-ProjectionServiceResourceTypeDef = TypedDict(
-    "ProjectionServiceResourceTypeDef",
-    {
-        "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": Sequence[str],
-    },
     total=False,
 )
 
-ReplicaOutputTypeDef = TypedDict(
-    "ReplicaOutputTypeDef",
-    {
-        "RegionName": str,
-    },
-)
-
-S3BucketSourceOutputTypeDef = TypedDict(
-    "S3BucketSourceOutputTypeDef",
-    {
-        "S3BucketOwner": str,
-        "S3Bucket": str,
-        "S3KeyPrefix": str,
-    },
-)
-
 _RequiredS3BucketSourceTypeDef = TypedDict(
     "_RequiredS3BucketSourceTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalS3BucketSourceTypeDef = TypedDict(
@@ -1473,27 +891,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ListBackupsInputRequestTypeDef = TypedDict(
-    "ListBackupsInputRequestTypeDef",
-    {
-        "TableName": str,
-        "Limit": int,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
-        "ExclusiveStartBackupArn": str,
-        "BackupType": BackupTypeFilterType,
-    },
-    total=False,
-)
-
 ListContributorInsightsInputRequestTypeDef = TypedDict(
     "ListContributorInsightsInputRequestTypeDef",
     {
         "TableName": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1556,211 +961,70 @@
 
 class ListTagsOfResourceInputRequestTypeDef(
     _RequiredListTagsOfResourceInputRequestTypeDef, _OptionalListTagsOfResourceInputRequestTypeDef
 ):
     pass
 
 
-TagTableTypeDef = TypedDict(
-    "TagTableTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
-ProvisionedThroughputOverrideOutputTypeDef = TypedDict(
-    "ProvisionedThroughputOverrideOutputTypeDef",
-    {
-        "ReadCapacityUnits": int,
-    },
-)
-
-ProvisionedThroughputOverrideTableOutputTypeDef = TypedDict(
-    "ProvisionedThroughputOverrideTableOutputTypeDef",
-    {
-        "ReadCapacityUnits": int,
-    },
-)
-
-PutRequestServiceResourceOutputTypeDef = TypedDict(
-    "PutRequestServiceResourceOutputTypeDef",
-    {
-        "Item": Dict[str, "AttributeValueServiceResourceTypeDef"],
-    },
-)
-
-PutRequestServiceResourceTypeDef = TypedDict(
-    "PutRequestServiceResourceTypeDef",
-    {
-        "Item": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-
-TableClassSummaryTableTypeDef = TypedDict(
-    "TableClassSummaryTableTypeDef",
-    {
-        "TableClass": TableClassType,
-        "LastUpdateDateTime": datetime,
-    },
-)
-
 TableClassSummaryTypeDef = TypedDict(
     "TableClassSummaryTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
+    total=False,
 )
 
-RestoreSummaryTableTypeDef = TypedDict(
-    "RestoreSummaryTableTypeDef",
+_RequiredRestoreSummaryTypeDef = TypedDict(
+    "_RequiredRestoreSummaryTypeDef",
     {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
     },
 )
-
-RestoreSummaryTypeDef = TypedDict(
-    "RestoreSummaryTypeDef",
+_OptionalRestoreSummaryTypeDef = TypedDict(
+    "_OptionalRestoreSummaryTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
-        "RestoreDateTime": datetime,
-        "RestoreInProgress": bool,
     },
+    total=False,
 )
 
-SSEDescriptionTableTypeDef = TypedDict(
-    "SSEDescriptionTableTypeDef",
-    {
-        "Status": SSEStatusType,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyArn": str,
-        "InaccessibleEncryptionDateTime": datetime,
-    },
-)
+
+class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
+    pass
+
 
 SSEDescriptionTypeDef = TypedDict(
     "SSEDescriptionTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
     },
-)
-
-SSESpecificationOutputTypeDef = TypedDict(
-    "SSESpecificationOutputTypeDef",
-    {
-        "Enabled": bool,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyId": str,
-    },
-)
-
-SSESpecificationTableTypeDef = TypedDict(
-    "SSESpecificationTableTypeDef",
-    {
-        "Enabled": bool,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyId": str,
-    },
     total=False,
 )
 
-StreamSpecificationOutputTypeDef = TypedDict(
-    "StreamSpecificationOutputTypeDef",
-    {
-        "StreamEnabled": bool,
-        "StreamViewType": StreamViewTypeType,
-    },
-)
-
-StreamSpecificationTableOutputTypeDef = TypedDict(
-    "StreamSpecificationTableOutputTypeDef",
-    {
-        "StreamEnabled": bool,
-        "StreamViewType": StreamViewTypeType,
-    },
-)
-
-_RequiredStreamSpecificationTableTypeDef = TypedDict(
-    "_RequiredStreamSpecificationTableTypeDef",
-    {
-        "StreamEnabled": bool,
-    },
-)
-_OptionalStreamSpecificationTableTypeDef = TypedDict(
-    "_OptionalStreamSpecificationTableTypeDef",
-    {
-        "StreamViewType": StreamViewTypeType,
-    },
-    total=False,
-)
-
-
-class StreamSpecificationTableTypeDef(
-    _RequiredStreamSpecificationTableTypeDef, _OptionalStreamSpecificationTableTypeDef
-):
-    pass
-
-
 TableBatchWriterRequestTypeDef = TypedDict(
     "TableBatchWriterRequestTypeDef",
     {
         "overwrite_by_pkeys": List[str],
     },
     total=False,
 )
 
-TimeToLiveSpecificationOutputTypeDef = TypedDict(
-    "TimeToLiveSpecificationOutputTypeDef",
-    {
-        "Enabled": bool,
-        "AttributeName": str,
-    },
-)
-
 TimeToLiveSpecificationTypeDef = TypedDict(
     "TimeToLiveSpecificationTypeDef",
     {
         "Enabled": bool,
         "AttributeName": str,
     },
 )
@@ -1792,26 +1056,26 @@
 class UpdateContributorInsightsInputRequestTypeDef(
     _RequiredUpdateContributorInsightsInputRequestTypeDef,
     _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
 
-ArchivalSummaryTableResponseMetadataTypeDef = TypedDict(
-    "ArchivalSummaryTableResponseMetadataTypeDef",
+ArchivalSummaryResponseTypeDef = TypedDict(
+    "ArchivalSummaryResponseTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BillingModeSummaryTableResponseMetadataTypeDef = TypedDict(
-    "BillingModeSummaryTableResponseMetadataTypeDef",
+BillingModeSummaryResponseTypeDef = TypedDict(
+    "BillingModeSummaryResponseTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1839,77 +1103,68 @@
         "TableName": str,
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTablesOutputTableTypeDef = TypedDict(
-    "ListTablesOutputTableTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTablesOutputTypeDef = TypedDict(
     "ListTablesOutputTypeDef",
     {
         "TableNames": List[str],
         "LastEvaluatedTableName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProvisionedThroughputDescriptionTableResponseMetadataTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
+ProvisionedThroughputDescriptionResponseTypeDef = TypedDict(
+    "ProvisionedThroughputDescriptionResponseTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RestoreSummaryTableResponseMetadataTypeDef = TypedDict(
-    "RestoreSummaryTableResponseMetadataTypeDef",
+RestoreSummaryResponseTypeDef = TypedDict(
+    "RestoreSummaryResponseTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SSEDescriptionTableResponseMetadataTypeDef = TypedDict(
-    "SSEDescriptionTableResponseMetadataTypeDef",
+SSEDescriptionResponseTypeDef = TypedDict(
+    "SSEDescriptionResponseTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StreamSpecificationTableResponseMetadataTypeDef = TypedDict(
-    "StreamSpecificationTableResponseMetadataTypeDef",
+StreamSpecificationResponseTypeDef = TypedDict(
+    "StreamSpecificationResponseTypeDef",
     {
         "StreamEnabled": bool,
         "StreamViewType": StreamViewTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TableClassSummaryTableResponseMetadataTypeDef = TypedDict(
-    "TableClassSummaryTableResponseMetadataTypeDef",
+TableClassSummaryResponseTypeDef = TypedDict(
+    "TableClassSummaryResponseTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1919,1042 +1174,213 @@
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttributeValueUpdateTypeDef = TypedDict(
-    "AttributeValueUpdateTypeDef",
+UniversalAttributeValueTypeDef = Union[
+    AttributeValueTypeDef,
+    bytes,
+    bytearray,
+    str,
+    int,
+    Decimal,
+    bool,
+    Set[int],
+    Set[Decimal],
+    Set[str],
+    Set[bytes],
+    Set[bytearray],
+    Sequence[Any],
+    Mapping[str, Any],
+    None,
+]
+AutoScalingPolicyDescriptionTypeDef = TypedDict(
+    "AutoScalingPolicyDescriptionTypeDef",
     {
-        "Value": Union[
-            AttributeValueTypeDef,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "Action": AttributeActionType,
+        "PolicyName": str,
+        "TargetTrackingScalingPolicyConfiguration": (
+            AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
+        ),
     },
     total=False,
 )
 
-_RequiredBatchStatementRequestTypeDef = TypedDict(
-    "_RequiredBatchStatementRequestTypeDef",
+_RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
+    "_RequiredAutoScalingPolicyUpdateTypeDef",
     {
-        "Statement": str,
+        "TargetTrackingScalingPolicyConfiguration": (
+            AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
+        ),
     },
 )
-_OptionalBatchStatementRequestTypeDef = TypedDict(
-    "_OptionalBatchStatementRequestTypeDef",
+_OptionalAutoScalingPolicyUpdateTypeDef = TypedDict(
+    "_OptionalAutoScalingPolicyUpdateTypeDef",
     {
-        "Parameters": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
-        "ConsistentRead": bool,
+        "PolicyName": str,
     },
     total=False,
 )
 
 
-class BatchStatementRequestTypeDef(
-    _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
+class AutoScalingPolicyUpdateTypeDef(
+    _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
 ):
     pass
 
 
-_RequiredConditionCheckTypeDef = TypedDict(
-    "_RequiredConditionCheckTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "TableName": str,
-        "ConditionExpression": str,
-    },
-)
-_OptionalConditionCheckTypeDef = TypedDict(
-    "_OptionalConditionCheckTypeDef",
+CreateBackupOutputTypeDef = TypedDict(
+    "CreateBackupOutputTypeDef",
     {
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
+        "BackupDetails": BackupDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class ConditionCheckTypeDef(_RequiredConditionCheckTypeDef, _OptionalConditionCheckTypeDef):
-    pass
-
-
-_RequiredConditionTypeDef = TypedDict(
-    "_RequiredConditionTypeDef",
-    {
-        "ComparisonOperator": ComparisonOperatorType,
-    },
-)
-_OptionalConditionTypeDef = TypedDict(
-    "_OptionalConditionTypeDef",
+ListBackupsOutputTypeDef = TypedDict(
+    "ListBackupsOutputTypeDef",
     {
-        "AttributeValueList": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "BackupSummaries": List[BackupSummaryTypeDef],
+        "LastEvaluatedBackupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class ConditionTypeDef(_RequiredConditionTypeDef, _OptionalConditionTypeDef):
-    pass
-
-
 DeleteRequestOutputTypeDef = TypedDict(
     "DeleteRequestOutputTypeDef",
     {
-        "Key": Dict[str, AttributeValueTypeDef],
-    },
-)
-
-DeleteRequestTypeDef = TypedDict(
-    "DeleteRequestTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-    },
-)
-
-_RequiredDeleteTypeDef = TypedDict(
-    "_RequiredDeleteTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "TableName": str,
-    },
-)
-_OptionalDeleteTypeDef = TypedDict(
-    "_OptionalDeleteTypeDef",
-    {
-        "ConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-
-class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
-    pass
-
-
-_RequiredExecuteStatementInputRequestTypeDef = TypedDict(
-    "_RequiredExecuteStatementInputRequestTypeDef",
-    {
-        "Statement": str,
-    },
-)
-_OptionalExecuteStatementInputRequestTypeDef = TypedDict(
-    "_OptionalExecuteStatementInputRequestTypeDef",
-    {
-        "Parameters": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
-        "ConsistentRead": bool,
-        "NextToken": str,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "Limit": int,
-    },
-    total=False,
-)
-
-
-class ExecuteStatementInputRequestTypeDef(
-    _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
-):
-    pass
-
-
-ExpectedAttributeValueTypeDef = TypedDict(
-    "ExpectedAttributeValueTypeDef",
-    {
-        "Value": Union[
-            AttributeValueTypeDef,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "Exists": bool,
-        "ComparisonOperator": ComparisonOperatorType,
-        "AttributeValueList": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "Key": Dict[str, TableAttributeValueTypeDef],
     },
-    total=False,
 )
 
-_RequiredGetItemInputRequestTypeDef = TypedDict(
-    "_RequiredGetItemInputRequestTypeDef",
+_RequiredGetItemInputTableGetItemTypeDef = TypedDict(
+    "_RequiredGetItemInputTableGetItemTypeDef",
     {
-        "TableName": str,
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
-_OptionalGetItemInputRequestTypeDef = TypedDict(
-    "_OptionalGetItemInputRequestTypeDef",
+_OptionalGetItemInputTableGetItemTypeDef = TypedDict(
+    "_OptionalGetItemInputTableGetItemTypeDef",
     {
         "AttributesToGet": Sequence[str],
         "ConsistentRead": bool,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
 
-class GetItemInputRequestTypeDef(
-    _RequiredGetItemInputRequestTypeDef, _OptionalGetItemInputRequestTypeDef
+class GetItemInputTableGetItemTypeDef(
+    _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
 ):
     pass
 
 
-_RequiredGetTypeDef = TypedDict(
-    "_RequiredGetTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "TableName": str,
-    },
-)
-_OptionalGetTypeDef = TypedDict(
-    "_OptionalGetTypeDef",
-    {
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class GetTypeDef(_RequiredGetTypeDef, _OptionalGetTypeDef):
-    pass
-
-
 ItemCollectionMetricsTypeDef = TypedDict(
     "ItemCollectionMetricsTypeDef",
     {
-        "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
+        "ItemCollectionKey": Dict[str, TableAttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
+    total=False,
 )
 
 ItemResponseTypeDef = TypedDict(
     "ItemResponseTypeDef",
     {
-        "Item": Dict[str, AttributeValueTypeDef],
-    },
-)
-
-KeysAndAttributesOutputTypeDef = TypedDict(
-    "KeysAndAttributesOutputTypeDef",
-    {
-        "Keys": List[Dict[str, AttributeValueTypeDef]],
-        "AttributesToGet": List[str],
-        "ConsistentRead": bool,
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Dict[str, str],
+        "Item": Dict[str, TableAttributeValueTypeDef],
     },
+    total=False,
 )
 
-_RequiredKeysAndAttributesTypeDef = TypedDict(
-    "_RequiredKeysAndAttributesTypeDef",
+_RequiredKeysAndAttributesOutputTypeDef = TypedDict(
+    "_RequiredKeysAndAttributesOutputTypeDef",
     {
-        "Keys": Sequence[
-            Mapping[
-                str,
-                Union[
-                    AttributeValueTypeDef,
-                    Union[
-                        bytes,
-                        bytearray,
-                        str,
-                        int,
-                        Decimal,
-                        bool,
-                        Set[int],
-                        Set[Decimal],
-                        Set[str],
-                        Set[bytes],
-                        Set[bytearray],
-                        Sequence[Any],
-                        Mapping[str, Any],
-                        None,
-                    ],
-                ],
-            ]
-        ],
+        "Keys": List[Dict[str, TableAttributeValueTypeDef]],
     },
 )
-_OptionalKeysAndAttributesTypeDef = TypedDict(
-    "_OptionalKeysAndAttributesTypeDef",
+_OptionalKeysAndAttributesOutputTypeDef = TypedDict(
+    "_OptionalKeysAndAttributesOutputTypeDef",
     {
-        "AttributesToGet": Sequence[str],
+        "AttributesToGet": List[str],
         "ConsistentRead": bool,
         "ProjectionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class KeysAndAttributesTypeDef(
-    _RequiredKeysAndAttributesTypeDef, _OptionalKeysAndAttributesTypeDef
-):
-    pass
-
-
-_RequiredParameterizedStatementTypeDef = TypedDict(
-    "_RequiredParameterizedStatementTypeDef",
-    {
-        "Statement": str,
-    },
-)
-_OptionalParameterizedStatementTypeDef = TypedDict(
-    "_OptionalParameterizedStatementTypeDef",
-    {
-        "Parameters": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "ExpressionAttributeNames": Dict[str, str],
     },
     total=False,
 )
 
 
-class ParameterizedStatementTypeDef(
-    _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
+class KeysAndAttributesOutputTypeDef(
+    _RequiredKeysAndAttributesOutputTypeDef, _OptionalKeysAndAttributesOutputTypeDef
 ):
     pass
 
 
 PutRequestOutputTypeDef = TypedDict(
     "PutRequestOutputTypeDef",
     {
-        "Item": Dict[str, AttributeValueTypeDef],
-    },
-)
-
-PutRequestTypeDef = TypedDict(
-    "PutRequestTypeDef",
-    {
-        "Item": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-    },
-)
-
-_RequiredPutTypeDef = TypedDict(
-    "_RequiredPutTypeDef",
-    {
-        "Item": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "TableName": str,
-    },
-)
-_OptionalPutTypeDef = TypedDict(
-    "_OptionalPutTypeDef",
-    {
-        "ConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-
-class PutTypeDef(_RequiredPutTypeDef, _OptionalPutTypeDef):
-    pass
-
-
-_RequiredUpdateTypeDef = TypedDict(
-    "_RequiredUpdateTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "UpdateExpression": str,
-        "TableName": str,
-    },
-)
-_OptionalUpdateTypeDef = TypedDict(
-    "_OptionalUpdateTypeDef",
-    {
-        "ConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-
-class UpdateTypeDef(_RequiredUpdateTypeDef, _OptionalUpdateTypeDef):
-    pass
-
-
-AutoScalingPolicyDescriptionTypeDef = TypedDict(
-    "AutoScalingPolicyDescriptionTypeDef",
-    {
-        "PolicyName": str,
-        "TargetTrackingScalingPolicyConfiguration": (
-            AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
-        ),
-    },
-)
-
-_RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
-    "_RequiredAutoScalingPolicyUpdateTypeDef",
-    {
-        "TargetTrackingScalingPolicyConfiguration": (
-            AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
-        ),
-    },
-)
-_OptionalAutoScalingPolicyUpdateTypeDef = TypedDict(
-    "_OptionalAutoScalingPolicyUpdateTypeDef",
-    {
-        "PolicyName": str,
-    },
-    total=False,
-)
-
-
-class AutoScalingPolicyUpdateTypeDef(
-    _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
-):
-    pass
-
-
-CreateBackupOutputTypeDef = TypedDict(
-    "CreateBackupOutputTypeDef",
-    {
-        "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupsOutputTableTypeDef = TypedDict(
-    "ListBackupsOutputTableTypeDef",
-    {
-        "BackupSummaries": List[BackupSummaryTableTypeDef],
-        "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupsOutputTypeDef = TypedDict(
-    "ListBackupsOutputTypeDef",
-    {
-        "BackupSummaries": List[BackupSummaryTypeDef],
-        "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
-    "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    {
-        "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
+        "Item": Dict[str, TableAttributeValueTypeDef],
     },
 )
-_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
-    "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-    },
-    total=False,
-)
-
-
-class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
-    _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
-):
-    pass
-
 
 BatchStatementResponseTypeDef = TypedDict(
     "BatchStatementResponseTypeDef",
     {
         "Error": BatchStatementErrorTypeDef,
         "TableName": str,
-        "Item": Dict[str, AttributeValueTypeDef],
-    },
-)
-
-ConsumedCapacityServiceResourceTypeDef = TypedDict(
-    "ConsumedCapacityServiceResourceTypeDef",
-    {
-        "TableName": str,
-        "CapacityUnits": float,
-        "ReadCapacityUnits": float,
-        "WriteCapacityUnits": float,
-        "Table": CapacityServiceResourceTypeDef,
-        "LocalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
-        "GlobalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
-    },
-)
-
-ConsumedCapacityTableTypeDef = TypedDict(
-    "ConsumedCapacityTableTypeDef",
-    {
-        "TableName": str,
-        "CapacityUnits": float,
-        "ReadCapacityUnits": float,
-        "WriteCapacityUnits": float,
-        "Table": CapacityTableTypeDef,
-        "LocalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
-        "GlobalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
+        "Item": Dict[str, TableAttributeValueTypeDef],
     },
+    total=False,
 )
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTypeDef],
     },
-)
-
-QueryInputTableQueryTypeDef = TypedDict(
-    "QueryInputTableQueryTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": Union[str, ConditionBase],
-        "KeyConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
     total=False,
 )
 
-ScanInputTableScanTypeDef = TypedDict(
-    "ScanInputTableScanTypeDef",
-    {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-    },
-    total=False,
-)
-
-ContinuousBackupsDescriptionTypeDef = TypedDict(
-    "ContinuousBackupsDescriptionTypeDef",
+_RequiredContinuousBackupsDescriptionTypeDef = TypedDict(
+    "_RequiredContinuousBackupsDescriptionTypeDef",
     {
         "ContinuousBackupsStatus": ContinuousBackupsStatusType,
-        "PointInTimeRecoveryDescription": PointInTimeRecoveryDescriptionTypeDef,
-    },
-)
-
-ListContributorInsightsOutputTypeDef = TypedDict(
-    "ListContributorInsightsOutputTypeDef",
-    {
-        "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
-    "_RequiredCreateGlobalSecondaryIndexActionTableTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": Sequence[KeySchemaElementTableTypeDef],
-        "Projection": ProjectionTableTypeDef,
-    },
-)
-_OptionalCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
-    "_OptionalCreateGlobalSecondaryIndexActionTableTypeDef",
+_OptionalContinuousBackupsDescriptionTypeDef = TypedDict(
+    "_OptionalContinuousBackupsDescriptionTypeDef",
     {
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
+        "PointInTimeRecoveryDescription": PointInTimeRecoveryDescriptionTypeDef,
     },
     total=False,
 )
 
 
-class CreateGlobalSecondaryIndexActionTableTypeDef(
-    _RequiredCreateGlobalSecondaryIndexActionTableTypeDef,
-    _OptionalCreateGlobalSecondaryIndexActionTableTypeDef,
+class ContinuousBackupsDescriptionTypeDef(
+    _RequiredContinuousBackupsDescriptionTypeDef, _OptionalContinuousBackupsDescriptionTypeDef
 ):
     pass
 
 
-UpdateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
-    "UpdateGlobalSecondaryIndexActionTableTypeDef",
+ListContributorInsightsOutputTypeDef = TypedDict(
+    "ListContributorInsightsOutputTypeDef",
     {
-        "IndexName": str,
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
+        "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LocalSecondaryIndexTypeDef = TypedDict(
     "LocalSecondaryIndexTypeDef",
     {
         "IndexName": str,
@@ -3006,14 +1432,42 @@
 
 class GlobalSecondaryIndexTypeDef(
     _RequiredGlobalSecondaryIndexTypeDef, _OptionalGlobalSecondaryIndexTypeDef
 ):
     pass
 
 
+_RequiredSourceTableDetailsTypeDef = TypedDict(
+    "_RequiredSourceTableDetailsTypeDef",
+    {
+        "TableName": str,
+        "TableId": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "TableCreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+    },
+)
+_OptionalSourceTableDetailsTypeDef = TypedDict(
+    "_OptionalSourceTableDetailsTypeDef",
+    {
+        "TableArn": str,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "BillingMode": BillingModeType,
+    },
+    total=False,
+)
+
+
+class SourceTableDetailsTypeDef(
+    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
+):
+    pass
+
+
 UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
 )
@@ -3022,36 +1476,32 @@
     "CreateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicationGroup": Sequence[ReplicaTypeDef],
     },
 )
 
-_RequiredReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
-    "_RequiredReplicaGlobalSecondaryIndexTableTypeDef",
+GlobalTableTypeDef = TypedDict(
+    "GlobalTableTypeDef",
     {
-        "IndexName": str,
+        "GlobalTableName": str,
+        "ReplicationGroup": List[ReplicaTypeDef],
     },
+    total=False,
 )
-_OptionalReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
-    "_OptionalReplicaGlobalSecondaryIndexTableTypeDef",
+
+ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     {
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
+        "IndexName": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
     },
     total=False,
 )
 
-
-class ReplicaGlobalSecondaryIndexTableTypeDef(
-    _RequiredReplicaGlobalSecondaryIndexTableTypeDef,
-    _OptionalReplicaGlobalSecondaryIndexTableTypeDef,
-):
-    pass
-
-
 _RequiredReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalReplicaGlobalSecondaryIndexTypeDef = TypedDict(
@@ -3065,231 +1515,47 @@
 
 class ReplicaGlobalSecondaryIndexTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTypeDef, _OptionalReplicaGlobalSecondaryIndexTypeDef
 ):
     pass
 
 
+ListTagsOfResourceOutputTypeDef = TypedDict(
+    "ListTagsOfResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 InputFormatOptionsOutputTypeDef = TypedDict(
     "InputFormatOptionsOutputTypeDef",
     {
         "Csv": CsvOptionsOutputTypeDef,
     },
+    total=False,
 )
 
 InputFormatOptionsTypeDef = TypedDict(
     "InputFormatOptionsTypeDef",
     {
         "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredDeleteItemInputTableDeleteItemTypeDef = TypedDict(
-    "_RequiredDeleteItemInputTableDeleteItemTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalDeleteItemInputTableDeleteItemTypeDef = TypedDict(
-    "_OptionalDeleteItemInputTableDeleteItemTypeDef",
-    {
-        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-    total=False,
-)
-
-
-class DeleteItemInputTableDeleteItemTypeDef(
-    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
-):
-    pass
-
-
-_RequiredPutItemInputTablePutItemTypeDef = TypedDict(
-    "_RequiredPutItemInputTablePutItemTypeDef",
-    {
-        "Item": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalPutItemInputTablePutItemTypeDef = TypedDict(
-    "_OptionalPutItemInputTablePutItemTypeDef",
-    {
-        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionalOperator": ConditionalOperatorType,
-        "ConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-    total=False,
-)
-
-
-class PutItemInputTablePutItemTypeDef(
-    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
-):
-    pass
-
-
-_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_OptionalUpdateItemInputTableUpdateItemTypeDef",
-    {
-        "AttributeUpdates": Mapping[str, AttributeValueUpdateTableTypeDef],
-        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "UpdateExpression": str,
-        "ConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateItemInputTableUpdateItemTypeDef(
-    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
-):
-    pass
-
-
 ReplicaUpdateTypeDef = TypedDict(
     "ReplicaUpdateTypeDef",
     {
         "Create": CreateReplicaActionTypeDef,
         "Delete": DeleteReplicaActionTypeDef,
     },
     total=False,
@@ -3398,173 +1664,150 @@
     {
         "ExportSummaries": List[ExportSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTableTypeDef",
+_RequiredExportTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_RequiredExportTableToPointInTimeInputRequestTypeDef",
     {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
-        "Projection": ProjectionTableOutputTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
+        "TableArn": str,
+        "S3Bucket": str,
     },
 )
-
-GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "GlobalSecondaryIndexDescriptionTableTypeDef",
+_OptionalExportTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_OptionalExportTableToPointInTimeInputRequestTypeDef",
     {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
-        "Projection": ProjectionTableOutputTypeDef,
-        "IndexStatus": IndexStatusType,
-        "Backfilling": bool,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
+        "ExportTime": TimestampTypeDef,
+        "ClientToken": str,
+        "S3BucketOwner": str,
+        "S3Prefix": str,
+        "S3SseAlgorithm": S3SseAlgorithmType,
+        "S3SseKmsKeyId": str,
+        "ExportFormat": ExportFormatType,
     },
+    total=False,
 )
 
-LocalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
-    },
-)
 
-LocalSecondaryIndexInfoTypeDef = TypedDict(
-    "LocalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-    },
-)
+class ExportTableToPointInTimeInputRequestTypeDef(
+    _RequiredExportTableToPointInTimeInputRequestTypeDef,
+    _OptionalExportTableToPointInTimeInputRequestTypeDef,
+):
+    pass
 
-GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "GlobalSecondaryIndexDescriptionTypeDef",
+
+ListBackupsInputRequestTypeDef = TypedDict(
+    "ListBackupsInputRequestTypeDef",
     {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-        "IndexStatus": IndexStatusType,
-        "Backfilling": bool,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
+        "TableName": str,
+        "Limit": int,
+        "TimeRangeLowerBound": TimestampTypeDef,
+        "TimeRangeUpperBound": TimestampTypeDef,
+        "ExclusiveStartBackupArn": str,
+        "BackupType": BackupTypeFilterType,
     },
+    total=False,
 )
 
 GlobalSecondaryIndexInfoTypeDef = TypedDict(
     "GlobalSecondaryIndexInfoTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
         "Projection": ProjectionOutputTypeDef,
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
+    total=False,
 )
 
-GlobalSecondaryIndexOutputTypeDef = TypedDict(
-    "GlobalSecondaryIndexOutputTypeDef",
+_RequiredGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "_RequiredGlobalSecondaryIndexOutputTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
         "Projection": ProjectionOutputTypeDef,
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
-    },
-)
-
-SourceTableDetailsTypeDef = TypedDict(
-    "SourceTableDetailsTypeDef",
-    {
-        "TableName": str,
-        "TableId": str,
-        "TableArn": str,
-        "TableSizeBytes": int,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "TableCreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
-        "ItemCount": int,
-        "BillingMode": BillingModeType,
     },
 )
-
-_RequiredGlobalSecondaryIndexServiceResourceTypeDef = TypedDict(
-    "_RequiredGlobalSecondaryIndexServiceResourceTypeDef",
+_OptionalGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "_OptionalGlobalSecondaryIndexOutputTypeDef",
     {
-        "IndexName": str,
-        "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
-        "Projection": ProjectionServiceResourceTypeDef,
-    },
-)
-_OptionalGlobalSecondaryIndexServiceResourceTypeDef = TypedDict(
-    "_OptionalGlobalSecondaryIndexServiceResourceTypeDef",
-    {
-        "ProvisionedThroughput": ProvisionedThroughputServiceResourceTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
 
-class GlobalSecondaryIndexServiceResourceTypeDef(
-    _RequiredGlobalSecondaryIndexServiceResourceTypeDef,
-    _OptionalGlobalSecondaryIndexServiceResourceTypeDef,
+class GlobalSecondaryIndexOutputTypeDef(
+    _RequiredGlobalSecondaryIndexOutputTypeDef, _OptionalGlobalSecondaryIndexOutputTypeDef
 ):
     pass
 
 
-LocalSecondaryIndexServiceResourceTypeDef = TypedDict(
-    "LocalSecondaryIndexServiceResourceTypeDef",
+LocalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
-        "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
-        "Projection": ProjectionServiceResourceTypeDef,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
     },
+    total=False,
 )
 
-GlobalTableTypeDef = TypedDict(
-    "GlobalTableTypeDef",
+LocalSecondaryIndexInfoTypeDef = TypedDict(
+    "LocalSecondaryIndexInfoTypeDef",
     {
-        "GlobalTableName": str,
-        "ReplicationGroup": List[ReplicaOutputTypeDef],
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionOutputTypeDef,
     },
+    total=False,
+)
+
+GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "GlobalSecondaryIndexDescriptionTypeDef",
+    {
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "IndexStatus": IndexStatusType,
+        "Backfilling": bool,
+        "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
+    },
+    total=False,
 )
 
 ImportSummaryTypeDef = TypedDict(
     "ImportSummaryTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
         "TableArn": str,
-        "S3BucketSource": S3BucketSourceOutputTypeDef,
+        "S3BucketSource": S3BucketSourceTypeDef,
         "CloudWatchLogGroupArn": str,
         "InputFormat": InputFormatType,
         "StartTime": datetime,
         "EndTime": datetime,
     },
+    total=False,
 )
 
 ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
     "ListBackupsInputListBackupsPaginateTypeDef",
     {
         "TableName": str,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
+        "TimeRangeLowerBound": TimestampTypeDef,
+        "TimeRangeUpperBound": TimestampTypeDef,
         "BackupType": BackupTypeFilterType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTablesInputListTablesPaginateTypeDef = TypedDict(
@@ -3593,794 +1836,392 @@
 class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
     _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
 ):
     pass
 
 
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
+UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
+    "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
+        "PointInTimeRecoverySpecification": PointInTimeRecoverySpecificationTypeDef,
     },
 )
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
+
+UpdateTimeToLiveInputRequestTypeDef = TypedDict(
+    "UpdateTimeToLiveInputRequestTypeDef",
     {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "TableName": str,
+        "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
     },
-    total=False,
 )
 
+UpdateTimeToLiveOutputTypeDef = TypedDict(
+    "UpdateTimeToLiveOutputTypeDef",
+    {
+        "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
-
+AttributeValueUpdateTypeDef = TypedDict(
+    "AttributeValueUpdateTypeDef",
+    {
+        "Value": UniversalAttributeValueTypeDef,
+        "Action": AttributeActionType,
+    },
+    total=False,
+)
 
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
+_RequiredBatchStatementRequestTypeDef = TypedDict(
+    "_RequiredBatchStatementRequestTypeDef",
     {
-        "TableName": str,
+        "Statement": str,
     },
 )
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
+_OptionalBatchStatementRequestTypeDef = TypedDict(
+    "_OptionalBatchStatementRequestTypeDef",
     {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
+        "Parameters": Sequence[UniversalAttributeValueTypeDef],
         "ConsistentRead": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+class BatchStatementRequestTypeDef(
+    _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
 ):
     pass
 
 
-ListTagsOfResourceOutputTableTypeDef = TypedDict(
-    "ListTagsOfResourceOutputTableTypeDef",
+_RequiredConditionCheckTypeDef = TypedDict(
+    "_RequiredConditionCheckTypeDef",
     {
-        "Tags": List[TagTableTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
+        "TableName": str,
+        "ConditionExpression": str,
     },
 )
-
-ListTagsOfResourceOutputTypeDef = TypedDict(
-    "ListTagsOfResourceOutputTypeDef",
+_OptionalConditionCheckTypeDef = TypedDict(
+    "_OptionalConditionCheckTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
+    total=False,
 )
 
-UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
-    "UpdateContinuousBackupsInputRequestTypeDef",
-    {
-        "TableName": str,
-        "PointInTimeRecoverySpecification": PointInTimeRecoverySpecificationTypeDef,
-    },
-)
 
-ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
-    },
-)
+class ConditionCheckTypeDef(_RequiredConditionCheckTypeDef, _OptionalConditionCheckTypeDef):
+    pass
 
-ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
-    },
-)
 
-WriteRequestServiceResourceOutputTypeDef = TypedDict(
-    "WriteRequestServiceResourceOutputTypeDef",
+_RequiredConditionTypeDef = TypedDict(
+    "_RequiredConditionTypeDef",
     {
-        "PutRequest": PutRequestServiceResourceOutputTypeDef,
-        "DeleteRequest": DeleteRequestServiceResourceOutputTypeDef,
+        "ComparisonOperator": ComparisonOperatorType,
     },
 )
-
-WriteRequestServiceResourceTypeDef = TypedDict(
-    "WriteRequestServiceResourceTypeDef",
+_OptionalConditionTypeDef = TypedDict(
+    "_OptionalConditionTypeDef",
     {
-        "PutRequest": PutRequestServiceResourceTypeDef,
-        "DeleteRequest": DeleteRequestServiceResourceTypeDef,
+        "AttributeValueList": Sequence[UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-UpdateTimeToLiveOutputTypeDef = TypedDict(
-    "UpdateTimeToLiveOutputTypeDef",
-    {
-        "TimeToLiveSpecification": TimeToLiveSpecificationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-UpdateTimeToLiveInputRequestTypeDef = TypedDict(
-    "UpdateTimeToLiveInputRequestTypeDef",
+class ConditionTypeDef(_RequiredConditionTypeDef, _OptionalConditionTypeDef):
+    pass
+
+
+DeleteRequestTypeDef = TypedDict(
+    "DeleteRequestTypeDef",
     {
-        "TableName": str,
-        "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
 
-_RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
-    "_RequiredBatchExecuteStatementInputRequestTypeDef",
+_RequiredDeleteTypeDef = TypedDict(
+    "_RequiredDeleteTypeDef",
     {
-        "Statements": Sequence[BatchStatementRequestTypeDef],
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
+        "TableName": str,
     },
 )
-_OptionalBatchExecuteStatementInputRequestTypeDef = TypedDict(
-    "_OptionalBatchExecuteStatementInputRequestTypeDef",
+_OptionalDeleteTypeDef = TypedDict(
+    "_OptionalDeleteTypeDef",
     {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class BatchExecuteStatementInputRequestTypeDef(
-    _RequiredBatchExecuteStatementInputRequestTypeDef,
-    _OptionalBatchExecuteStatementInputRequestTypeDef,
-):
+class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
 
-_RequiredQueryInputRequestTypeDef = TypedDict(
-    "_RequiredQueryInputRequestTypeDef",
+_RequiredExecuteStatementInputRequestTypeDef = TypedDict(
+    "_RequiredExecuteStatementInputRequestTypeDef",
     {
-        "TableName": str,
+        "Statement": str,
     },
 )
-_OptionalQueryInputRequestTypeDef = TypedDict(
-    "_OptionalQueryInputRequestTypeDef",
+_OptionalExecuteStatementInputRequestTypeDef = TypedDict(
+    "_OptionalExecuteStatementInputRequestTypeDef",
     {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
+        "Parameters": Sequence[UniversalAttributeValueTypeDef],
         "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTypeDef],
-        "QueryFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "NextToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "Limit": int,
     },
     total=False,
 )
 
 
-class QueryInputRequestTypeDef(
-    _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
+class ExecuteStatementInputRequestTypeDef(
+    _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
 ):
     pass
 
 
-_RequiredScanInputRequestTypeDef = TypedDict(
-    "_RequiredScanInputRequestTypeDef",
+ExpectedAttributeValueTypeDef = TypedDict(
+    "ExpectedAttributeValueTypeDef",
+    {
+        "Value": UniversalAttributeValueTypeDef,
+        "Exists": bool,
+        "ComparisonOperator": ComparisonOperatorType,
+        "AttributeValueList": Sequence[UniversalAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+_RequiredGetItemInputRequestTypeDef = TypedDict(
+    "_RequiredGetItemInputRequestTypeDef",
     {
         "TableName": str,
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
-_OptionalScanInputRequestTypeDef = TypedDict(
-    "_OptionalScanInputRequestTypeDef",
+_OptionalGetItemInputRequestTypeDef = TypedDict(
+    "_OptionalGetItemInputRequestTypeDef",
     {
-        "IndexName": str,
         "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "ConsistentRead": bool,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
         "ProjectionExpression": str,
-        "FilterExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "ConsistentRead": bool,
     },
     total=False,
 )
 
 
-class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
+class GetItemInputRequestTypeDef(
+    _RequiredGetItemInputRequestTypeDef, _OptionalGetItemInputRequestTypeDef
+):
     pass
 
 
-_RequiredDeleteItemInputRequestTypeDef = TypedDict(
-    "_RequiredDeleteItemInputRequestTypeDef",
+_RequiredGetTypeDef = TypedDict(
+    "_RequiredGetTypeDef",
     {
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
         "TableName": str,
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
     },
 )
-_OptionalDeleteItemInputRequestTypeDef = TypedDict(
-    "_OptionalDeleteItemInputRequestTypeDef",
+_OptionalGetTypeDef = TypedDict(
+    "_OptionalGetTypeDef",
     {
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionExpression": str,
+        "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
     },
     total=False,
 )
 
 
-class DeleteItemInputRequestTypeDef(
-    _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
-):
+class GetTypeDef(_RequiredGetTypeDef, _OptionalGetTypeDef):
     pass
 
 
-_RequiredPutItemInputRequestTypeDef = TypedDict(
-    "_RequiredPutItemInputRequestTypeDef",
+_RequiredKeysAndAttributesTypeDef = TypedDict(
+    "_RequiredKeysAndAttributesTypeDef",
     {
-        "TableName": str,
-        "Item": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "Keys": Sequence[Mapping[str, UniversalAttributeValueTypeDef]],
     },
 )
-_OptionalPutItemInputRequestTypeDef = TypedDict(
-    "_OptionalPutItemInputRequestTypeDef",
+_OptionalKeysAndAttributesTypeDef = TypedDict(
+    "_OptionalKeysAndAttributesTypeDef",
     {
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionalOperator": ConditionalOperatorType,
-        "ConditionExpression": str,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
     },
     total=False,
 )
 
 
-class PutItemInputRequestTypeDef(
-    _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
+class KeysAndAttributesTypeDef(
+    _RequiredKeysAndAttributesTypeDef, _OptionalKeysAndAttributesTypeDef
 ):
     pass
 
 
-_RequiredUpdateItemInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateItemInputRequestTypeDef",
+_RequiredParameterizedStatementTypeDef = TypedDict(
+    "_RequiredParameterizedStatementTypeDef",
     {
-        "TableName": str,
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "Statement": str,
     },
 )
-_OptionalUpdateItemInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateItemInputRequestTypeDef",
+_OptionalParameterizedStatementTypeDef = TypedDict(
+    "_OptionalParameterizedStatementTypeDef",
     {
-        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "UpdateExpression": str,
-        "ConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "Parameters": Sequence[UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
 
-class UpdateItemInputRequestTypeDef(
-    _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
+class ParameterizedStatementTypeDef(
+    _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
 ):
     pass
 
 
-TransactGetItemTypeDef = TypedDict(
-    "TransactGetItemTypeDef",
+PutRequestTypeDef = TypedDict(
+    "PutRequestTypeDef",
     {
-        "Get": GetTypeDef,
+        "Item": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
 
-_RequiredBatchGetItemInputRequestTypeDef = TypedDict(
-    "_RequiredBatchGetItemInputRequestTypeDef",
+_RequiredPutTypeDef = TypedDict(
+    "_RequiredPutTypeDef",
     {
-        "RequestItems": Mapping[str, KeysAndAttributesTypeDef],
+        "Item": Mapping[str, UniversalAttributeValueTypeDef],
+        "TableName": str,
     },
 )
-_OptionalBatchGetItemInputRequestTypeDef = TypedDict(
-    "_OptionalBatchGetItemInputRequestTypeDef",
+_OptionalPutTypeDef = TypedDict(
+    "_OptionalPutTypeDef",
     {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class BatchGetItemInputRequestTypeDef(
-    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
-):
+class PutTypeDef(_RequiredPutTypeDef, _OptionalPutTypeDef):
     pass
 
 
-_RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
-    "_RequiredExecuteTransactionInputRequestTypeDef",
+_RequiredUpdateTypeDef = TypedDict(
+    "_RequiredUpdateTypeDef",
     {
-        "TransactStatements": Sequence[ParameterizedStatementTypeDef],
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
+        "UpdateExpression": str,
+        "TableName": str,
     },
 )
-_OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
-    "_OptionalExecuteTransactionInputRequestTypeDef",
+_OptionalUpdateTypeDef = TypedDict(
+    "_OptionalUpdateTypeDef",
     {
-        "ClientRequestToken": str,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
 
-class ExecuteTransactionInputRequestTypeDef(
-    _RequiredExecuteTransactionInputRequestTypeDef, _OptionalExecuteTransactionInputRequestTypeDef
-):
+class UpdateTypeDef(_RequiredUpdateTypeDef, _OptionalUpdateTypeDef):
     pass
 
 
-WriteRequestOutputTypeDef = TypedDict(
-    "WriteRequestOutputTypeDef",
-    {
-        "PutRequest": PutRequestOutputTypeDef,
-        "DeleteRequest": DeleteRequestOutputTypeDef,
-    },
-)
-
-WriteRequestTypeDef = TypedDict(
-    "WriteRequestTypeDef",
-    {
-        "PutRequest": PutRequestTypeDef,
-        "DeleteRequest": DeleteRequestTypeDef,
-    },
-    total=False,
-)
-
-TransactWriteItemTypeDef = TypedDict(
-    "TransactWriteItemTypeDef",
-    {
-        "ConditionCheck": ConditionCheckTypeDef,
-        "Put": PutTypeDef,
-        "Delete": DeleteTypeDef,
-        "Update": UpdateTypeDef,
-    },
-    total=False,
-)
-
 AutoScalingSettingsDescriptionTypeDef = TypedDict(
     "AutoScalingSettingsDescriptionTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicies": List[AutoScalingPolicyDescriptionTypeDef],
     },
+    total=False,
 )
 
 AutoScalingSettingsUpdateTypeDef = TypedDict(
     "AutoScalingSettingsUpdateTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicyUpdate": AutoScalingPolicyUpdateTypeDef,
     },
     total=False,
 )
 
-BatchGetItemOutputServiceResourceTypeDef = TypedDict(
-    "BatchGetItemOutputServiceResourceTypeDef",
-    {
-        "Responses": Dict[str, List[Dict[str, "AttributeValueServiceResourceTypeDef"]]],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceOutputTypeDef],
-        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteItemOutputTableTypeDef = TypedDict(
-    "DeleteItemOutputTableTypeDef",
-    {
-        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetItemOutputTableTypeDef = TypedDict(
-    "GetItemOutputTableTypeDef",
-    {
-        "Item": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutItemOutputTableTypeDef = TypedDict(
-    "PutItemOutputTableTypeDef",
-    {
-        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-QueryOutputTableTypeDef = TypedDict(
-    "QueryOutputTableTypeDef",
-    {
-        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
-        "Count": int,
-        "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ScanOutputTableTypeDef = TypedDict(
-    "ScanOutputTableTypeDef",
-    {
-        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
-        "Count": int,
-        "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateItemOutputTableTypeDef = TypedDict(
-    "UpdateItemOutputTableTypeDef",
+WriteRequestOutputTypeDef = TypedDict(
+    "WriteRequestOutputTypeDef",
     {
-        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PutRequest": PutRequestOutputTypeDef,
+        "DeleteRequest": DeleteRequestOutputTypeDef,
     },
+    total=False,
 )
 
 BatchExecuteStatementOutputTypeDef = TypedDict(
     "BatchExecuteStatementOutputTypeDef",
     {
         "Responses": List[BatchStatementResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetItemOutputTypeDef = TypedDict(
     "BatchGetItemOutputTypeDef",
     {
-        "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
+        "Responses": Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
         "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
-        "Attributes": Dict[str, AttributeValueTypeDef],
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
-        "Items": List[Dict[str, AttributeValueTypeDef]],
+        "Items": List[Dict[str, TableAttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
@@ -4389,49 +2230,49 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
-        "Item": Dict[str, AttributeValueTypeDef],
+        "Item": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
-        "Attributes": Dict[str, AttributeValueTypeDef],
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
-        "Items": List[Dict[str, AttributeValueTypeDef]],
+        "Items": List[Dict[str, TableAttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
-        "Items": List[Dict[str, AttributeValueTypeDef]],
+        "Items": List[Dict[str, TableAttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
@@ -4450,15 +2291,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
-        "Attributes": Dict[str, AttributeValueTypeDef],
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
@@ -4473,112 +2314,14 @@
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
-    "GlobalSecondaryIndexUpdateTableTypeDef",
-    {
-        "Update": UpdateGlobalSecondaryIndexActionTableTypeDef,
-        "Create": CreateGlobalSecondaryIndexActionTableTypeDef,
-        "Delete": DeleteGlobalSecondaryIndexActionTableTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateTableInputRequestTypeDef = TypedDict(
-    "_RequiredCreateTableInputRequestTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "TableName": str,
-        "KeySchema": Sequence[KeySchemaElementTypeDef],
-    },
-)
-_OptionalCreateTableInputRequestTypeDef = TypedDict(
-    "_OptionalCreateTableInputRequestTypeDef",
-    {
-        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
-        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
-
-class CreateTableInputRequestTypeDef(
-    _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
-):
-    pass
-
-
-_RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
-    "_RequiredRestoreTableFromBackupInputRequestTypeDef",
-    {
-        "TargetTableName": str,
-        "BackupArn": str,
-    },
-)
-_OptionalRestoreTableFromBackupInputRequestTypeDef = TypedDict(
-    "_OptionalRestoreTableFromBackupInputRequestTypeDef",
-    {
-        "BillingModeOverride": BillingModeType,
-        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexTypeDef],
-        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
-        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
-        "SSESpecificationOverride": SSESpecificationTypeDef,
-    },
-    total=False,
-)
-
-
-class RestoreTableFromBackupInputRequestTypeDef(
-    _RequiredRestoreTableFromBackupInputRequestTypeDef,
-    _OptionalRestoreTableFromBackupInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
-    {
-        "TargetTableName": str,
-    },
-)
-_OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_OptionalRestoreTableToPointInTimeInputRequestTypeDef",
-    {
-        "SourceTableArn": str,
-        "SourceTableName": str,
-        "UseLatestRestorableTime": bool,
-        "RestoreDateTime": Union[datetime, str],
-        "BillingModeOverride": BillingModeType,
-        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexTypeDef],
-        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
-        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
-        "SSESpecificationOverride": SSESpecificationTypeDef,
-    },
-    total=False,
-)
-
-
-class RestoreTableToPointInTimeInputRequestTypeDef(
-    _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
-    _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
-):
-    pass
-
-
 _RequiredTableCreationParametersTypeDef = TypedDict(
     "_RequiredTableCreationParametersTypeDef",
     {
         "TableName": str,
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "KeySchema": Sequence[KeySchemaElementTypeDef],
     },
@@ -4607,64 +2350,39 @@
         "Update": UpdateGlobalSecondaryIndexActionTypeDef,
         "Create": CreateGlobalSecondaryIndexActionTypeDef,
         "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "_RequiredCreateReplicationGroupMemberActionTableTypeDef",
+ListGlobalTablesOutputTypeDef = TypedDict(
+    "ListGlobalTablesOutputTypeDef",
     {
-        "RegionName": str,
+        "GlobalTables": List[GlobalTableTypeDef],
+        "LastEvaluatedGlobalTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "_OptionalCreateReplicationGroupMemberActionTableTypeDef",
-    {
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-        "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
-        "TableClassOverride": TableClassType,
-    },
-    total=False,
-)
-
-
-class CreateReplicationGroupMemberActionTableTypeDef(
-    _RequiredCreateReplicationGroupMemberActionTableTypeDef,
-    _OptionalCreateReplicationGroupMemberActionTableTypeDef,
-):
-    pass
 
-
-_RequiredUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "_RequiredUpdateReplicationGroupMemberActionTableTypeDef",
+ReplicaDescriptionTypeDef = TypedDict(
+    "ReplicaDescriptionTypeDef",
     {
         "RegionName": str,
-    },
-)
-_OptionalUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "_OptionalUpdateReplicationGroupMemberActionTableTypeDef",
-    {
+        "ReplicaStatus": ReplicaStatusType,
+        "ReplicaStatusDescription": str,
+        "ReplicaStatusPercentProgress": str,
         "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-        "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
-        "TableClassOverride": TableClassType,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
+        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
+        "ReplicaInaccessibleDateTime": datetime,
+        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
     total=False,
 )
 
-
-class UpdateReplicationGroupMemberActionTableTypeDef(
-    _RequiredUpdateReplicationGroupMemberActionTableTypeDef,
-    _OptionalUpdateReplicationGroupMemberActionTableTypeDef,
-):
-    pass
-
-
 _RequiredCreateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalCreateReplicationGroupMemberActionTypeDef = TypedDict(
@@ -4707,257 +2425,540 @@
 class UpdateReplicationGroupMemberActionTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
 
+InputFormatOptionsUnionTypeDef = Union[InputFormatOptionsTypeDef, InputFormatOptionsOutputTypeDef]
 UpdateGlobalTableInputRequestTypeDef = TypedDict(
     "UpdateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaUpdates": Sequence[ReplicaUpdateTypeDef],
     },
 )
 
+GlobalSecondaryIndexUnionTypeDef = Union[
+    GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef
+]
+_RequiredTableCreationParametersOutputTypeDef = TypedDict(
+    "_RequiredTableCreationParametersOutputTypeDef",
+    {
+        "TableName": str,
+        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
+    },
+)
+_OptionalTableCreationParametersOutputTypeDef = TypedDict(
+    "_OptionalTableCreationParametersOutputTypeDef",
+    {
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class TableCreationParametersOutputTypeDef(
+    _RequiredTableCreationParametersOutputTypeDef, _OptionalTableCreationParametersOutputTypeDef
+):
+    pass
+
+
 SourceTableFeatureDetailsTypeDef = TypedDict(
     "SourceTableFeatureDetailsTypeDef",
     {
         "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
         "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
-        "StreamDescription": StreamSpecificationOutputTypeDef,
+        "StreamDescription": StreamSpecificationTypeDef,
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
         "SSEDescription": SSEDescriptionTypeDef,
     },
+    total=False,
 )
 
-TableCreationParametersOutputTypeDef = TypedDict(
-    "TableCreationParametersOutputTypeDef",
+ListImportsOutputTypeDef = TypedDict(
+    "ListImportsOutputTypeDef",
+    {
+        "ImportSummaryList": List[ImportSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
+    "_RequiredBatchExecuteStatementInputRequestTypeDef",
+    {
+        "Statements": Sequence[BatchStatementRequestTypeDef],
+    },
+)
+_OptionalBatchExecuteStatementInputRequestTypeDef = TypedDict(
+    "_OptionalBatchExecuteStatementInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+    },
+    total=False,
+)
+
+
+class BatchExecuteStatementInputRequestTypeDef(
+    _RequiredBatchExecuteStatementInputRequestTypeDef,
+    _OptionalBatchExecuteStatementInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
     {
         "TableName": str,
-        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
-        "SSESpecification": SSESpecificationOutputTypeDef,
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
     },
 )
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTypeDef],
+        "QueryFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-_RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
-    "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
+
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
+
+_RequiredQueryInputRequestTypeDef = TypedDict(
+    "_RequiredQueryInputRequestTypeDef",
     {
-        "AttributeDefinitions": Sequence[AttributeDefinitionServiceResourceTypeDef],
         "TableName": str,
-        "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
     },
 )
-_OptionalCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
-    "_OptionalCreateTableInputServiceResourceCreateTableTypeDef",
+_OptionalQueryInputRequestTypeDef = TypedDict(
+    "_OptionalQueryInputRequestTypeDef",
     {
-        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexServiceResourceTypeDef],
-        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexServiceResourceTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputServiceResourceTypeDef,
-        "StreamSpecification": StreamSpecificationServiceResourceTypeDef,
-        "SSESpecification": SSESpecificationServiceResourceTypeDef,
-        "Tags": Sequence[TagServiceResourceTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTypeDef],
+        "QueryFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ExclusiveStartKey": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
 
-class CreateTableInputServiceResourceCreateTableTypeDef(
-    _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
-    _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
+class QueryInputRequestTypeDef(
+    _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
 ):
     pass
 
 
-ListGlobalTablesOutputTypeDef = TypedDict(
-    "ListGlobalTablesOutputTypeDef",
+QueryInputTableQueryTypeDef = TypedDict(
+    "QueryInputTableQueryTypeDef",
     {
-        "GlobalTables": List[GlobalTableTypeDef],
-        "LastEvaluatedGlobalTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTypeDef],
+        "QueryFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": ConditionBaseImportTypeDef,
+        "KeyConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
     },
+    total=False,
 )
 
-ListImportsOutputTypeDef = TypedDict(
-    "ListImportsOutputTypeDef",
+_RequiredScanInputRequestTypeDef = TypedDict(
+    "_RequiredScanInputRequestTypeDef",
     {
-        "ImportSummaryList": List[ImportSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TableName": str,
+    },
+)
+_OptionalScanInputRequestTypeDef = TypedDict(
+    "_OptionalScanInputRequestTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ExclusiveStartKey": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ConsistentRead": bool,
     },
+    total=False,
 )
 
-ReplicaDescriptionTypeDef = TypedDict(
-    "ReplicaDescriptionTypeDef",
+
+class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
+    pass
+
+
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
     {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
+        "TableName": str,
     },
 )
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-ReplicaDescriptionTableTypeDef = TypedDict(
-    "ReplicaDescriptionTableTypeDef",
+
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
+
+ScanInputTableScanTypeDef = TypedDict(
+    "ScanInputTableScanTypeDef",
     {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ConsistentRead": bool,
     },
+    total=False,
 )
 
-BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
-    "BatchWriteItemOutputServiceResourceTypeDef",
+_RequiredDeleteItemInputRequestTypeDef = TypedDict(
+    "_RequiredDeleteItemInputRequestTypeDef",
     {
-        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceOutputTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TableName": str,
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
+    },
+)
+_OptionalDeleteItemInputRequestTypeDef = TypedDict(
+    "_OptionalDeleteItemInputRequestTypeDef",
+    {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
+    total=False,
 )
 
-_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
-    "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+
+class DeleteItemInputRequestTypeDef(
+    _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
+):
+    pass
+
+
+_RequiredDeleteItemInputTableDeleteItemTypeDef = TypedDict(
+    "_RequiredDeleteItemInputTableDeleteItemTypeDef",
     {
-        "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
+        "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
-_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
-    "_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+_OptionalDeleteItemInputTableDeleteItemTypeDef = TypedDict(
+    "_OptionalDeleteItemInputTableDeleteItemTypeDef",
     {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
     },
     total=False,
 )
 
 
-class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
-    _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-    _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+class DeleteItemInputTableDeleteItemTypeDef(
+    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
 ):
     pass
 
 
-_RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
-    "_RequiredTransactGetItemsInputRequestTypeDef",
+_RequiredPutItemInputRequestTypeDef = TypedDict(
+    "_RequiredPutItemInputRequestTypeDef",
     {
-        "TransactItems": Sequence[TransactGetItemTypeDef],
+        "TableName": str,
+        "Item": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
-_OptionalTransactGetItemsInputRequestTypeDef = TypedDict(
-    "_OptionalTransactGetItemsInputRequestTypeDef",
+_OptionalPutItemInputRequestTypeDef = TypedDict(
+    "_OptionalPutItemInputRequestTypeDef",
     {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionalOperator": ConditionalOperatorType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
 
-class TransactGetItemsInputRequestTypeDef(
-    _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
+class PutItemInputRequestTypeDef(
+    _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
 ):
     pass
 
 
-BatchWriteItemOutputTypeDef = TypedDict(
-    "BatchWriteItemOutputTypeDef",
+_RequiredPutItemInputTablePutItemTypeDef = TypedDict(
+    "_RequiredPutItemInputTablePutItemTypeDef",
     {
-        "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Item": Mapping[str, TableAttributeValueTypeDef],
+    },
+)
+_OptionalPutItemInputTablePutItemTypeDef = TypedDict(
+    "_OptionalPutItemInputTablePutItemTypeDef",
+    {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionalOperator": ConditionalOperatorType,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
     },
+    total=False,
 )
 
-_RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
-    "_RequiredBatchWriteItemInputRequestTypeDef",
+
+class PutItemInputTablePutItemTypeDef(
+    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
+):
+    pass
+
+
+_RequiredUpdateItemInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateItemInputRequestTypeDef",
     {
-        "RequestItems": Mapping[str, Sequence[WriteRequestTypeDef]],
+        "TableName": str,
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
-_OptionalBatchWriteItemInputRequestTypeDef = TypedDict(
-    "_OptionalBatchWriteItemInputRequestTypeDef",
+_OptionalUpdateItemInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateItemInputRequestTypeDef",
     {
+        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "UpdateExpression": str,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
 
-class BatchWriteItemInputRequestTypeDef(
-    _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
+class UpdateItemInputRequestTypeDef(
+    _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
     pass
 
 
-_RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
-    "_RequiredTransactWriteItemsInputRequestTypeDef",
+_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
+    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
     {
-        "TransactItems": Sequence[TransactWriteItemTypeDef],
+        "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
-_OptionalTransactWriteItemsInputRequestTypeDef = TypedDict(
-    "_OptionalTransactWriteItemsInputRequestTypeDef",
+_OptionalUpdateItemInputTableUpdateItemTypeDef = TypedDict(
+    "_OptionalUpdateItemInputTableUpdateItemTypeDef",
     {
+        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "UpdateExpression": str,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateItemInputTableUpdateItemTypeDef(
+    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
+):
+    pass
+
+
+TransactGetItemTypeDef = TypedDict(
+    "TransactGetItemTypeDef",
+    {
+        "Get": GetTypeDef,
+    },
+)
+
+KeysAndAttributesUnionTypeDef = Union[KeysAndAttributesTypeDef, KeysAndAttributesOutputTypeDef]
+_RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
+    "_RequiredExecuteTransactionInputRequestTypeDef",
+    {
+        "TransactStatements": Sequence[ParameterizedStatementTypeDef],
+    },
+)
+_OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
+    "_OptionalExecuteTransactionInputRequestTypeDef",
+    {
         "ClientRequestToken": str,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
 
-class TransactWriteItemsInputRequestTypeDef(
-    _RequiredTransactWriteItemsInputRequestTypeDef, _OptionalTransactWriteItemsInputRequestTypeDef
+class ExecuteTransactionInputRequestTypeDef(
+    _RequiredExecuteTransactionInputRequestTypeDef, _OptionalExecuteTransactionInputRequestTypeDef
 ):
     pass
 
 
+WriteRequestTypeDef = TypedDict(
+    "WriteRequestTypeDef",
+    {
+        "PutRequest": PutRequestTypeDef,
+        "DeleteRequest": DeleteRequestTypeDef,
+    },
+    total=False,
+)
+
+TransactWriteItemTypeDef = TypedDict(
+    "TransactWriteItemTypeDef",
+    {
+        "ConditionCheck": ConditionCheckTypeDef,
+        "Put": PutTypeDef,
+        "Delete": DeleteTypeDef,
+        "Update": UpdateTypeDef,
+    },
+    total=False,
+)
+
 ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     {
         "IndexName": str,
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
+    total=False,
 )
 
-ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
+_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
+    "_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     {
         "IndexName": str,
+    },
+)
+_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
+    "_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
+    {
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
+    total=False,
 )
 
+
+class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(
+    _RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
+    _OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
+):
+    pass
+
+
 GlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -5014,14 +3015,24 @@
 class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
 
+BatchWriteItemOutputTypeDef = TypedDict(
+    "BatchWriteItemOutputTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredImportTableInputRequestTypeDef = TypedDict(
     "_RequiredImportTableInputRequestTypeDef",
     {
         "S3BucketSource": S3BucketSourceTypeDef,
         "InputFormat": InputFormatType,
         "TableCreationParameters": TableCreationParametersTypeDef,
     },
@@ -5039,165 +3050,355 @@
 
 class ImportTableInputRequestTypeDef(
     _RequiredImportTableInputRequestTypeDef, _OptionalImportTableInputRequestTypeDef
 ):
     pass
 
 
-ReplicationGroupUpdateTableTypeDef = TypedDict(
-    "ReplicationGroupUpdateTableTypeDef",
+GlobalTableDescriptionTypeDef = TypedDict(
+    "GlobalTableDescriptionTypeDef",
+    {
+        "ReplicationGroup": List[ReplicaDescriptionTypeDef],
+        "GlobalTableArn": str,
+        "CreationDateTime": datetime,
+        "GlobalTableStatus": GlobalTableStatusType,
+        "GlobalTableName": str,
+    },
+    total=False,
+)
+
+TableDescriptionTypeDef = TypedDict(
+    "TableDescriptionTypeDef",
     {
-        "Create": CreateReplicationGroupMemberActionTableTypeDef,
-        "Update": UpdateReplicationGroupMemberActionTableTypeDef,
-        "Delete": DeleteReplicationGroupMemberActionTableTypeDef,
+        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "TableStatus": TableStatusType,
+        "CreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "TableArn": str,
+        "TableId": str,
+        "BillingModeSummary": BillingModeSummaryTypeDef,
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "LatestStreamLabel": str,
+        "LatestStreamArn": str,
+        "GlobalTableVersion": str,
+        "Replicas": List[ReplicaDescriptionTypeDef],
+        "RestoreSummary": RestoreSummaryTypeDef,
+        "SSEDescription": SSEDescriptionTypeDef,
+        "ArchivalSummary": ArchivalSummaryTypeDef,
+        "TableClassSummary": TableClassSummaryTypeDef,
+        "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
 ReplicationGroupUpdateTypeDef = TypedDict(
     "ReplicationGroupUpdateTypeDef",
     {
         "Create": CreateReplicationGroupMemberActionTypeDef,
         "Update": UpdateReplicationGroupMemberActionTypeDef,
         "Delete": DeleteReplicationGroupMemberActionTypeDef,
     },
     total=False,
 )
 
-BackupDescriptionTypeDef = TypedDict(
-    "BackupDescriptionTypeDef",
+_RequiredCreateTableInputRequestTypeDef = TypedDict(
+    "_RequiredCreateTableInputRequestTypeDef",
     {
-        "BackupDetails": BackupDetailsTypeDef,
-        "SourceTableDetails": SourceTableDetailsTypeDef,
-        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+    },
+)
+_OptionalCreateTableInputRequestTypeDef = TypedDict(
+    "_OptionalCreateTableInputRequestTypeDef",
+    {
+        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexUnionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+
+class CreateTableInputRequestTypeDef(
+    _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
+    "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+    },
+)
+_OptionalCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
+    "_OptionalCreateTableInputServiceResourceCreateTableTypeDef",
+    {
+        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexUnionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+
+class CreateTableInputServiceResourceCreateTableTypeDef(
+    _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
+    _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
+):
+    pass
+
+
+_RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
+    "_RequiredRestoreTableFromBackupInputRequestTypeDef",
+    {
+        "TargetTableName": str,
+        "BackupArn": str,
+    },
+)
+_OptionalRestoreTableFromBackupInputRequestTypeDef = TypedDict(
+    "_OptionalRestoreTableFromBackupInputRequestTypeDef",
+    {
+        "BillingModeOverride": BillingModeType,
+        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexUnionTypeDef],
+        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
+        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
+        "SSESpecificationOverride": SSESpecificationTypeDef,
+    },
+    total=False,
+)
+
+
+class RestoreTableFromBackupInputRequestTypeDef(
+    _RequiredRestoreTableFromBackupInputRequestTypeDef,
+    _OptionalRestoreTableFromBackupInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
+    {
+        "TargetTableName": str,
+    },
+)
+_OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_OptionalRestoreTableToPointInTimeInputRequestTypeDef",
+    {
+        "SourceTableArn": str,
+        "SourceTableName": str,
+        "UseLatestRestorableTime": bool,
+        "RestoreDateTime": TimestampTypeDef,
+        "BillingModeOverride": BillingModeType,
+        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexUnionTypeDef],
+        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
+        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
+        "SSESpecificationOverride": SSESpecificationTypeDef,
     },
+    total=False,
 )
 
+
+class RestoreTableToPointInTimeInputRequestTypeDef(
+    _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
+    _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
+):
+    pass
+
+
 ImportTableDescriptionTypeDef = TypedDict(
     "ImportTableDescriptionTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
         "TableArn": str,
         "TableId": str,
         "ClientToken": str,
-        "S3BucketSource": S3BucketSourceOutputTypeDef,
+        "S3BucketSource": S3BucketSourceTypeDef,
         "ErrorCount": int,
         "CloudWatchLogGroupArn": str,
         "InputFormat": InputFormatType,
         "InputFormatOptions": InputFormatOptionsOutputTypeDef,
         "InputCompressionType": InputCompressionTypeType,
         "TableCreationParameters": TableCreationParametersOutputTypeDef,
         "StartTime": datetime,
         "EndTime": datetime,
         "ProcessedSizeBytes": int,
         "ProcessedItemCount": int,
         "ImportedItemCount": int,
         "FailureCode": str,
         "FailureMessage": str,
     },
+    total=False,
 )
 
-GlobalTableDescriptionTypeDef = TypedDict(
-    "GlobalTableDescriptionTypeDef",
+TableCreationParametersUnionTypeDef = Union[
+    TableCreationParametersTypeDef, TableCreationParametersOutputTypeDef
+]
+BackupDescriptionTypeDef = TypedDict(
+    "BackupDescriptionTypeDef",
     {
-        "ReplicationGroup": List[ReplicaDescriptionTypeDef],
-        "GlobalTableArn": str,
-        "CreationDateTime": datetime,
-        "GlobalTableStatus": GlobalTableStatusType,
-        "GlobalTableName": str,
+        "BackupDetails": BackupDetailsTypeDef,
+        "SourceTableDetails": SourceTableDetailsTypeDef,
+        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
     },
+    total=False,
 )
 
-TableDescriptionTypeDef = TypedDict(
-    "TableDescriptionTypeDef",
+_RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
+    "_RequiredTransactGetItemsInputRequestTypeDef",
     {
-        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
-        "TableName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "TableStatus": TableStatusType,
-        "CreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "TableArn": str,
-        "TableId": str,
-        "BillingModeSummary": BillingModeSummaryTypeDef,
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTypeDef],
-        "StreamSpecification": StreamSpecificationOutputTypeDef,
-        "LatestStreamLabel": str,
-        "LatestStreamArn": str,
-        "GlobalTableVersion": str,
-        "Replicas": List[ReplicaDescriptionTypeDef],
-        "RestoreSummary": RestoreSummaryTypeDef,
-        "SSEDescription": SSEDescriptionTypeDef,
-        "ArchivalSummary": ArchivalSummaryTypeDef,
-        "TableClassSummary": TableClassSummaryTypeDef,
-        "DeletionProtectionEnabled": bool,
+        "TransactItems": Sequence[TransactGetItemTypeDef],
+    },
+)
+_OptionalTransactGetItemsInputRequestTypeDef = TypedDict(
+    "_OptionalTransactGetItemsInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
+    total=False,
 )
 
-TableDescriptionTableTypeDef = TypedDict(
-    "TableDescriptionTableTypeDef",
+
+class TransactGetItemsInputRequestTypeDef(
+    _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
+):
+    pass
+
+
+_RequiredBatchGetItemInputRequestTypeDef = TypedDict(
+    "_RequiredBatchGetItemInputRequestTypeDef",
     {
-        "AttributeDefinitions": List[AttributeDefinitionTableOutputTypeDef],
-        "TableName": str,
-        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
-        "TableStatus": TableStatusType,
-        "CreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "TableArn": str,
-        "TableId": str,
-        "BillingModeSummary": BillingModeSummaryTableTypeDef,
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableOutputTypeDef,
-        "LatestStreamLabel": str,
-        "LatestStreamArn": str,
-        "GlobalTableVersion": str,
-        "Replicas": List[ReplicaDescriptionTableTypeDef],
-        "RestoreSummary": RestoreSummaryTableTypeDef,
-        "SSEDescription": SSEDescriptionTableTypeDef,
-        "ArchivalSummary": ArchivalSummaryTableTypeDef,
-        "TableClassSummary": TableClassSummaryTableTypeDef,
-        "DeletionProtectionEnabled": bool,
+        "RequestItems": Mapping[str, KeysAndAttributesUnionTypeDef],
+    },
+)
+_OptionalBatchGetItemInputRequestTypeDef = TypedDict(
+    "_OptionalBatchGetItemInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+    },
+    total=False,
+)
+
+
+class BatchGetItemInputRequestTypeDef(
+    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
+):
+    pass
+
+
+_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
+    "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    {
+        "RequestItems": Mapping[str, KeysAndAttributesUnionTypeDef],
+    },
+)
+_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
+    "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+    },
+    total=False,
+)
+
+
+class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
+    _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
+    _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
+):
+    pass
+
+
+WriteRequestUnionTypeDef = Union[WriteRequestTypeDef, WriteRequestOutputTypeDef]
+_RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
+    "_RequiredTransactWriteItemsInputRequestTypeDef",
+    {
+        "TransactItems": Sequence[TransactWriteItemTypeDef],
     },
 )
+_OptionalTransactWriteItemsInputRequestTypeDef = TypedDict(
+    "_OptionalTransactWriteItemsInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class TransactWriteItemsInputRequestTypeDef(
+    _RequiredTransactWriteItemsInputRequestTypeDef, _OptionalTransactWriteItemsInputRequestTypeDef
+):
+    pass
+
 
 ReplicaAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaAutoScalingDescriptionTypeDef",
     {
         "RegionName": str,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef],
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaStatus": ReplicaStatusType,
     },
+    total=False,
 )
 
-ReplicaSettingsDescriptionTypeDef = TypedDict(
-    "ReplicaSettingsDescriptionTypeDef",
+_RequiredReplicaSettingsDescriptionTypeDef = TypedDict(
+    "_RequiredReplicaSettingsDescriptionTypeDef",
     {
         "RegionName": str,
+    },
+)
+_OptionalReplicaSettingsDescriptionTypeDef = TypedDict(
+    "_OptionalReplicaSettingsDescriptionTypeDef",
+    {
         "ReplicaStatus": ReplicaStatusType,
         "ReplicaBillingModeSummary": BillingModeSummaryTypeDef,
         "ReplicaProvisionedReadCapacityUnits": int,
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityUnits": int,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaGlobalSecondaryIndexSettings": List[
             ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef
         ],
         "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
+    total=False,
 )
 
+
+class ReplicaSettingsDescriptionTypeDef(
+    _RequiredReplicaSettingsDescriptionTypeDef, _OptionalReplicaSettingsDescriptionTypeDef
+):
+    pass
+
+
 _RequiredReplicaAutoScalingUpdateTypeDef = TypedDict(
     "_RequiredReplicaAutoScalingUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaAutoScalingUpdateTypeDef = TypedDict(
@@ -5240,28 +3441,84 @@
 
 class ReplicaSettingsUpdateTypeDef(
     _RequiredReplicaSettingsUpdateTypeDef, _OptionalReplicaSettingsUpdateTypeDef
 ):
     pass
 
 
-UpdateTableInputTableUpdateTypeDef = TypedDict(
-    "UpdateTableInputTableUpdateTypeDef",
+CreateGlobalTableOutputTypeDef = TypedDict(
+    "CreateGlobalTableOutputTypeDef",
     {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableTypeDef,
-        "SSESpecification": SSESpecificationTableTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTableTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
+        "GlobalTableDescription": GlobalTableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGlobalTableOutputTypeDef = TypedDict(
+    "DescribeGlobalTableOutputTypeDef",
+    {
+        "GlobalTableDescription": GlobalTableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGlobalTableOutputTypeDef = TypedDict(
+    "UpdateGlobalTableOutputTypeDef",
+    {
+        "GlobalTableDescription": GlobalTableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTableOutputTypeDef = TypedDict(
+    "CreateTableOutputTypeDef",
+    {
+        "TableDescription": TableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTableOutputTypeDef = TypedDict(
+    "DeleteTableOutputTypeDef",
+    {
+        "TableDescription": TableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTableOutputTypeDef = TypedDict(
+    "DescribeTableOutputTypeDef",
+    {
+        "Table": TableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreTableFromBackupOutputTypeDef = TypedDict(
+    "RestoreTableFromBackupOutputTypeDef",
+    {
+        "TableDescription": TableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreTableToPointInTimeOutputTypeDef = TypedDict(
+    "RestoreTableToPointInTimeOutputTypeDef",
+    {
+        "TableDescription": TableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTableOutputTypeDef = TypedDict(
+    "UpdateTableOutputTypeDef",
+    {
+        "TableDescription": TableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredUpdateTableInputRequestTypeDef = TypedDict(
     "_RequiredUpdateTableInputRequestTypeDef",
     {
         "TableName": str,
     },
@@ -5285,28 +3542,28 @@
 
 class UpdateTableInputRequestTypeDef(
     _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
 ):
     pass
 
 
-DeleteBackupOutputTypeDef = TypedDict(
-    "DeleteBackupOutputTypeDef",
-    {
-        "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBackupOutputTypeDef = TypedDict(
-    "DescribeBackupOutputTypeDef",
+UpdateTableInputTableUpdateTypeDef = TypedDict(
+    "UpdateTableInputTableUpdateTypeDef",
     {
-        "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
     },
+    total=False,
 )
 
 DescribeImportOutputTypeDef = TypedDict(
     "DescribeImportOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -5317,101 +3574,83 @@
     "ImportTableOutputTypeDef",
     {
         "ImportTableDescription": ImportTableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateGlobalTableOutputTypeDef = TypedDict(
-    "CreateGlobalTableOutputTypeDef",
+DeleteBackupOutputTypeDef = TypedDict(
+    "DeleteBackupOutputTypeDef",
     {
-        "GlobalTableDescription": GlobalTableDescriptionTypeDef,
+        "BackupDescription": BackupDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeGlobalTableOutputTypeDef = TypedDict(
-    "DescribeGlobalTableOutputTypeDef",
+DescribeBackupOutputTypeDef = TypedDict(
+    "DescribeBackupOutputTypeDef",
     {
-        "GlobalTableDescription": GlobalTableDescriptionTypeDef,
+        "BackupDescription": BackupDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateGlobalTableOutputTypeDef = TypedDict(
-    "UpdateGlobalTableOutputTypeDef",
+_RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
+    "_RequiredBatchWriteItemInputRequestTypeDef",
     {
-        "GlobalTableDescription": GlobalTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestItems": Mapping[str, Sequence[WriteRequestUnionTypeDef]],
     },
 )
-
-CreateTableOutputTypeDef = TypedDict(
-    "CreateTableOutputTypeDef",
+_OptionalBatchWriteItemInputRequestTypeDef = TypedDict(
+    "_OptionalBatchWriteItemInputRequestTypeDef",
     {
-        "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
     },
+    total=False,
 )
 
-DeleteTableOutputTypeDef = TypedDict(
-    "DeleteTableOutputTypeDef",
-    {
-        "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-DescribeTableOutputTypeDef = TypedDict(
-    "DescribeTableOutputTypeDef",
-    {
-        "Table": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class BatchWriteItemInputRequestTypeDef(
+    _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
+):
+    pass
 
-RestoreTableFromBackupOutputTypeDef = TypedDict(
-    "RestoreTableFromBackupOutputTypeDef",
-    {
-        "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-RestoreTableToPointInTimeOutputTypeDef = TypedDict(
-    "RestoreTableToPointInTimeOutputTypeDef",
+_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
+    "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     {
-        "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "RequestItems": Mapping[str, Sequence[WriteRequestUnionTypeDef]],
     },
 )
-
-UpdateTableOutputTypeDef = TypedDict(
-    "UpdateTableOutputTypeDef",
+_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
+    "_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     {
-        "TableDescription": TableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
     },
+    total=False,
 )
 
-DeleteTableOutputTableTypeDef = TypedDict(
-    "DeleteTableOutputTableTypeDef",
-    {
-        "TableDescription": TableDescriptionTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+
+class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
+    _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+    _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+):
+    pass
+
 
 TableAutoScalingDescriptionTypeDef = TypedDict(
     "TableAutoScalingDescriptionTypeDef",
     {
         "TableName": str,
         "TableStatus": TableStatusType,
         "Replicas": List[ReplicaAutoScalingDescriptionTypeDef],
     },
+    total=False,
 )
 
 DescribeGlobalTableSettingsOutputTypeDef = TypedDict(
     "DescribeGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/type_defs.pyi` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/type_defs.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_dynamodb.type_defs import ResponseMetadataTypeDef
 
-    data: ResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from decimal import Decimal
 from typing import Any, Dict, List, Mapping, Sequence, Set, Union
 
@@ -62,73 +62,44 @@
 try:
     from boto3.dynamodb.conditions import ConditionBase
 except (ModuleNotFoundError, ImportError):
     from builtins import object as ConditionBase
 
 __all__ = (
     "ResponseMetadataTypeDef",
-    "ArchivalSummaryTableTypeDef",
     "ArchivalSummaryTypeDef",
-    "AttributeDefinitionOutputTypeDef",
-    "AttributeDefinitionServiceResourceTypeDef",
-    "AttributeDefinitionTableOutputTypeDef",
-    "AttributeDefinitionTableTypeDef",
     "AttributeDefinitionTypeDef",
-    "AttributeValueServiceResourceTypeDef",
-    "AttributeValueTableTypeDef",
     "AttributeValueTypeDef",
-    "AttributeValueUpdateTableTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     "AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     "BackupDetailsTypeDef",
-    "BackupSummaryTableTypeDef",
     "BackupSummaryTypeDef",
-    "KeysAndAttributesServiceResourceTypeDef",
-    "KeysAndAttributesServiceResourceOutputTypeDef",
+    "TableAttributeValueTypeDef",
     "BatchStatementErrorTypeDef",
-    "ItemCollectionMetricsServiceResourceTypeDef",
-    "BillingModeSummaryTableTypeDef",
     "BillingModeSummaryTypeDef",
-    "CapacityServiceResourceTypeDef",
-    "CapacityTableTypeDef",
     "CapacityTypeDef",
-    "ConditionTableTypeDef",
+    "ConditionBaseImportTypeDef",
     "PointInTimeRecoveryDescriptionTypeDef",
     "ContributorInsightsSummaryTypeDef",
     "CreateBackupInputRequestTypeDef",
-    "KeySchemaElementTableTypeDef",
-    "ProjectionTableTypeDef",
-    "ProvisionedThroughputTableTypeDef",
     "KeySchemaElementTypeDef",
     "ProjectionTypeDef",
     "ProvisionedThroughputTypeDef",
     "ReplicaTypeDef",
     "CreateReplicaActionTypeDef",
-    "ProvisionedThroughputOverrideTableTypeDef",
     "ProvisionedThroughputOverrideTypeDef",
     "SSESpecificationTypeDef",
     "StreamSpecificationTypeDef",
     "TagTypeDef",
-    "KeySchemaElementServiceResourceTypeDef",
-    "ProvisionedThroughputServiceResourceTypeDef",
-    "SSESpecificationServiceResourceTypeDef",
-    "StreamSpecificationServiceResourceTypeDef",
-    "TagServiceResourceTypeDef",
     "CsvOptionsOutputTypeDef",
     "CsvOptionsTypeDef",
     "DeleteBackupInputRequestTypeDef",
-    "DeleteGlobalSecondaryIndexActionTableTypeDef",
     "DeleteGlobalSecondaryIndexActionTypeDef",
-    "ExpectedAttributeValueTableTypeDef",
-    "ItemCollectionMetricsTableTypeDef",
     "DeleteReplicaActionTypeDef",
-    "DeleteReplicationGroupMemberActionTableTypeDef",
     "DeleteReplicationGroupMemberActionTypeDef",
-    "DeleteRequestServiceResourceOutputTypeDef",
-    "DeleteRequestServiceResourceTypeDef",
     "DeleteTableInputRequestTypeDef",
     "DescribeBackupInputRequestTypeDef",
     "DescribeContinuousBackupsInputRequestTypeDef",
     "DescribeContributorInsightsInputRequestTypeDef",
     "FailureExceptionTypeDef",
     "EndpointTypeDef",
     "DescribeExportInputRequestTypeDef",
@@ -140,250 +111,204 @@
     "KinesisDataStreamDestinationTypeDef",
     "DescribeTableInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTableReplicaAutoScalingInputRequestTypeDef",
     "DescribeTimeToLiveInputRequestTypeDef",
     "TimeToLiveDescriptionTypeDef",
     "ExportSummaryTypeDef",
-    "ExportTableToPointInTimeInputRequestTypeDef",
-    "GetItemInputTableGetItemTypeDef",
-    "KeySchemaElementTableOutputTypeDef",
-    "ProjectionTableOutputTypeDef",
-    "ProvisionedThroughputDescriptionTableTypeDef",
-    "KeySchemaElementOutputTypeDef",
+    "TimestampTypeDef",
     "ProjectionOutputTypeDef",
     "ProvisionedThroughputDescriptionTypeDef",
-    "ProvisionedThroughputOutputTypeDef",
-    "ProjectionServiceResourceTypeDef",
-    "ReplicaOutputTypeDef",
-    "S3BucketSourceOutputTypeDef",
     "S3BucketSourceTypeDef",
     "KinesisStreamingDestinationInputRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ListBackupsInputRequestTypeDef",
     "ListContributorInsightsInputRequestTypeDef",
     "ListExportsInputRequestTypeDef",
     "ListGlobalTablesInputRequestTypeDef",
     "ListImportsInputRequestTypeDef",
     "ListTablesInputRequestTypeDef",
     "ListTagsOfResourceInputRequestTypeDef",
-    "TagTableTypeDef",
-    "TagOutputTypeDef",
     "PointInTimeRecoverySpecificationTypeDef",
-    "ProvisionedThroughputOverrideOutputTypeDef",
-    "ProvisionedThroughputOverrideTableOutputTypeDef",
-    "PutRequestServiceResourceOutputTypeDef",
-    "PutRequestServiceResourceTypeDef",
-    "TableClassSummaryTableTypeDef",
     "TableClassSummaryTypeDef",
-    "RestoreSummaryTableTypeDef",
     "RestoreSummaryTypeDef",
-    "SSEDescriptionTableTypeDef",
     "SSEDescriptionTypeDef",
-    "SSESpecificationOutputTypeDef",
-    "SSESpecificationTableTypeDef",
-    "StreamSpecificationOutputTypeDef",
-    "StreamSpecificationTableOutputTypeDef",
-    "StreamSpecificationTableTypeDef",
     "TableBatchWriterRequestTypeDef",
-    "TimeToLiveSpecificationOutputTypeDef",
     "TimeToLiveSpecificationTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateContributorInsightsInputRequestTypeDef",
-    "ArchivalSummaryTableResponseMetadataTypeDef",
-    "BillingModeSummaryTableResponseMetadataTypeDef",
+    "ArchivalSummaryResponseTypeDef",
+    "BillingModeSummaryResponseTypeDef",
     "DescribeLimitsOutputTypeDef",
     "EmptyResponseMetadataTypeDef",
     "KinesisStreamingDestinationOutputTypeDef",
-    "ListTablesOutputTableTypeDef",
     "ListTablesOutputTypeDef",
-    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
-    "RestoreSummaryTableResponseMetadataTypeDef",
-    "SSEDescriptionTableResponseMetadataTypeDef",
-    "StreamSpecificationTableResponseMetadataTypeDef",
-    "TableClassSummaryTableResponseMetadataTypeDef",
+    "ProvisionedThroughputDescriptionResponseTypeDef",
+    "RestoreSummaryResponseTypeDef",
+    "SSEDescriptionResponseTypeDef",
+    "StreamSpecificationResponseTypeDef",
+    "TableClassSummaryResponseTypeDef",
     "UpdateContributorInsightsOutputTypeDef",
-    "AttributeValueUpdateTypeDef",
-    "BatchStatementRequestTypeDef",
-    "ConditionCheckTypeDef",
-    "ConditionTypeDef",
+    "UniversalAttributeValueTypeDef",
+    "AutoScalingPolicyDescriptionTypeDef",
+    "AutoScalingPolicyUpdateTypeDef",
+    "CreateBackupOutputTypeDef",
+    "ListBackupsOutputTypeDef",
     "DeleteRequestOutputTypeDef",
-    "DeleteRequestTypeDef",
-    "DeleteTypeDef",
-    "ExecuteStatementInputRequestTypeDef",
-    "ExpectedAttributeValueTypeDef",
-    "GetItemInputRequestTypeDef",
-    "GetTypeDef",
+    "GetItemInputTableGetItemTypeDef",
     "ItemCollectionMetricsTypeDef",
     "ItemResponseTypeDef",
     "KeysAndAttributesOutputTypeDef",
-    "KeysAndAttributesTypeDef",
-    "ParameterizedStatementTypeDef",
     "PutRequestOutputTypeDef",
-    "PutRequestTypeDef",
-    "PutTypeDef",
-    "UpdateTypeDef",
-    "AutoScalingPolicyDescriptionTypeDef",
-    "AutoScalingPolicyUpdateTypeDef",
-    "CreateBackupOutputTypeDef",
-    "ListBackupsOutputTableTypeDef",
-    "ListBackupsOutputTypeDef",
-    "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
     "BatchStatementResponseTypeDef",
-    "ConsumedCapacityServiceResourceTypeDef",
-    "ConsumedCapacityTableTypeDef",
     "ConsumedCapacityTypeDef",
-    "QueryInputTableQueryTypeDef",
-    "ScanInputTableScanTypeDef",
     "ContinuousBackupsDescriptionTypeDef",
     "ListContributorInsightsOutputTypeDef",
-    "CreateGlobalSecondaryIndexActionTableTypeDef",
-    "UpdateGlobalSecondaryIndexActionTableTypeDef",
     "LocalSecondaryIndexTypeDef",
     "CreateGlobalSecondaryIndexActionTypeDef",
     "GlobalSecondaryIndexTypeDef",
+    "SourceTableDetailsTypeDef",
     "UpdateGlobalSecondaryIndexActionTypeDef",
     "CreateGlobalTableInputRequestTypeDef",
-    "ReplicaGlobalSecondaryIndexTableTypeDef",
+    "GlobalTableTypeDef",
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexTypeDef",
+    "ListTagsOfResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "InputFormatOptionsOutputTypeDef",
     "InputFormatOptionsTypeDef",
-    "DeleteItemInputTableDeleteItemTypeDef",
-    "PutItemInputTablePutItemTypeDef",
-    "UpdateItemInputTableUpdateItemTypeDef",
     "ReplicaUpdateTypeDef",
     "DescribeContributorInsightsOutputTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "DescribeExportOutputTypeDef",
     "ExportTableToPointInTimeOutputTypeDef",
     "DescribeKinesisStreamingDestinationOutputTypeDef",
     "DescribeTableInputTableExistsWaitTypeDef",
     "DescribeTableInputTableNotExistsWaitTypeDef",
     "DescribeTimeToLiveOutputTypeDef",
     "ListExportsOutputTypeDef",
-    "LocalSecondaryIndexDescriptionTableTypeDef",
-    "GlobalSecondaryIndexDescriptionTableTypeDef",
+    "ExportTableToPointInTimeInputRequestTypeDef",
+    "ListBackupsInputRequestTypeDef",
+    "GlobalSecondaryIndexInfoTypeDef",
+    "GlobalSecondaryIndexOutputTypeDef",
     "LocalSecondaryIndexDescriptionTypeDef",
     "LocalSecondaryIndexInfoTypeDef",
     "GlobalSecondaryIndexDescriptionTypeDef",
-    "GlobalSecondaryIndexInfoTypeDef",
-    "GlobalSecondaryIndexOutputTypeDef",
-    "SourceTableDetailsTypeDef",
-    "GlobalSecondaryIndexServiceResourceTypeDef",
-    "LocalSecondaryIndexServiceResourceTypeDef",
-    "GlobalTableTypeDef",
     "ImportSummaryTypeDef",
     "ListBackupsInputListBackupsPaginateTypeDef",
     "ListTablesInputListTablesPaginateTypeDef",
     "ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef",
-    "QueryInputQueryPaginateTypeDef",
-    "ScanInputScanPaginateTypeDef",
-    "ListTagsOfResourceOutputTableTypeDef",
-    "ListTagsOfResourceOutputTypeDef",
     "UpdateContinuousBackupsInputRequestTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
-    "WriteRequestServiceResourceOutputTypeDef",
-    "WriteRequestServiceResourceTypeDef",
-    "UpdateTimeToLiveOutputTypeDef",
     "UpdateTimeToLiveInputRequestTypeDef",
-    "BatchExecuteStatementInputRequestTypeDef",
-    "QueryInputRequestTypeDef",
-    "ScanInputRequestTypeDef",
-    "DeleteItemInputRequestTypeDef",
-    "PutItemInputRequestTypeDef",
-    "UpdateItemInputRequestTypeDef",
-    "TransactGetItemTypeDef",
-    "BatchGetItemInputRequestTypeDef",
-    "ExecuteTransactionInputRequestTypeDef",
-    "WriteRequestOutputTypeDef",
-    "WriteRequestTypeDef",
-    "TransactWriteItemTypeDef",
+    "UpdateTimeToLiveOutputTypeDef",
+    "AttributeValueUpdateTypeDef",
+    "BatchStatementRequestTypeDef",
+    "ConditionCheckTypeDef",
+    "ConditionTypeDef",
+    "DeleteRequestTypeDef",
+    "DeleteTypeDef",
+    "ExecuteStatementInputRequestTypeDef",
+    "ExpectedAttributeValueTypeDef",
+    "GetItemInputRequestTypeDef",
+    "GetTypeDef",
+    "KeysAndAttributesTypeDef",
+    "ParameterizedStatementTypeDef",
+    "PutRequestTypeDef",
+    "PutTypeDef",
+    "UpdateTypeDef",
     "AutoScalingSettingsDescriptionTypeDef",
     "AutoScalingSettingsUpdateTypeDef",
-    "BatchGetItemOutputServiceResourceTypeDef",
-    "DeleteItemOutputTableTypeDef",
-    "GetItemOutputTableTypeDef",
-    "PutItemOutputTableTypeDef",
-    "QueryOutputTableTypeDef",
-    "ScanOutputTableTypeDef",
-    "UpdateItemOutputTableTypeDef",
+    "WriteRequestOutputTypeDef",
     "BatchExecuteStatementOutputTypeDef",
     "BatchGetItemOutputTypeDef",
     "DeleteItemOutputTypeDef",
     "ExecuteStatementOutputTypeDef",
     "ExecuteTransactionOutputTypeDef",
     "GetItemOutputTypeDef",
     "PutItemOutputTypeDef",
     "QueryOutputTypeDef",
     "ScanOutputTypeDef",
     "TransactGetItemsOutputTypeDef",
     "TransactWriteItemsOutputTypeDef",
     "UpdateItemOutputTypeDef",
     "DescribeContinuousBackupsOutputTypeDef",
     "UpdateContinuousBackupsOutputTypeDef",
-    "GlobalSecondaryIndexUpdateTableTypeDef",
-    "CreateTableInputRequestTypeDef",
-    "RestoreTableFromBackupInputRequestTypeDef",
-    "RestoreTableToPointInTimeInputRequestTypeDef",
     "TableCreationParametersTypeDef",
     "GlobalSecondaryIndexUpdateTypeDef",
-    "CreateReplicationGroupMemberActionTableTypeDef",
-    "UpdateReplicationGroupMemberActionTableTypeDef",
+    "ListGlobalTablesOutputTypeDef",
+    "ReplicaDescriptionTypeDef",
     "CreateReplicationGroupMemberActionTypeDef",
     "UpdateReplicationGroupMemberActionTypeDef",
+    "InputFormatOptionsUnionTypeDef",
     "UpdateGlobalTableInputRequestTypeDef",
-    "SourceTableFeatureDetailsTypeDef",
+    "GlobalSecondaryIndexUnionTypeDef",
     "TableCreationParametersOutputTypeDef",
-    "CreateTableInputServiceResourceCreateTableTypeDef",
-    "ListGlobalTablesOutputTypeDef",
+    "SourceTableFeatureDetailsTypeDef",
     "ListImportsOutputTypeDef",
-    "ReplicaDescriptionTypeDef",
-    "ReplicaDescriptionTableTypeDef",
-    "BatchWriteItemOutputServiceResourceTypeDef",
-    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
-    "TransactGetItemsInputRequestTypeDef",
-    "BatchWriteItemOutputTypeDef",
-    "BatchWriteItemInputRequestTypeDef",
-    "TransactWriteItemsInputRequestTypeDef",
+    "BatchExecuteStatementInputRequestTypeDef",
+    "QueryInputQueryPaginateTypeDef",
+    "QueryInputRequestTypeDef",
+    "QueryInputTableQueryTypeDef",
+    "ScanInputRequestTypeDef",
+    "ScanInputScanPaginateTypeDef",
+    "ScanInputTableScanTypeDef",
+    "DeleteItemInputRequestTypeDef",
+    "DeleteItemInputTableDeleteItemTypeDef",
+    "PutItemInputRequestTypeDef",
+    "PutItemInputTablePutItemTypeDef",
+    "UpdateItemInputRequestTypeDef",
+    "UpdateItemInputTableUpdateItemTypeDef",
+    "TransactGetItemTypeDef",
+    "KeysAndAttributesUnionTypeDef",
+    "ExecuteTransactionInputRequestTypeDef",
+    "WriteRequestTypeDef",
+    "TransactWriteItemTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef",
     "ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef",
+    "BatchWriteItemOutputTypeDef",
     "ImportTableInputRequestTypeDef",
-    "ReplicationGroupUpdateTableTypeDef",
-    "ReplicationGroupUpdateTypeDef",
-    "BackupDescriptionTypeDef",
-    "ImportTableDescriptionTypeDef",
     "GlobalTableDescriptionTypeDef",
     "TableDescriptionTypeDef",
-    "TableDescriptionTableTypeDef",
+    "ReplicationGroupUpdateTypeDef",
+    "CreateTableInputRequestTypeDef",
+    "CreateTableInputServiceResourceCreateTableTypeDef",
+    "RestoreTableFromBackupInputRequestTypeDef",
+    "RestoreTableToPointInTimeInputRequestTypeDef",
+    "ImportTableDescriptionTypeDef",
+    "TableCreationParametersUnionTypeDef",
+    "BackupDescriptionTypeDef",
+    "TransactGetItemsInputRequestTypeDef",
+    "BatchGetItemInputRequestTypeDef",
+    "BatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    "WriteRequestUnionTypeDef",
+    "TransactWriteItemsInputRequestTypeDef",
     "ReplicaAutoScalingDescriptionTypeDef",
     "ReplicaSettingsDescriptionTypeDef",
     "ReplicaAutoScalingUpdateTypeDef",
     "ReplicaSettingsUpdateTypeDef",
-    "UpdateTableInputTableUpdateTypeDef",
-    "UpdateTableInputRequestTypeDef",
-    "DeleteBackupOutputTypeDef",
-    "DescribeBackupOutputTypeDef",
-    "DescribeImportOutputTypeDef",
-    "ImportTableOutputTypeDef",
     "CreateGlobalTableOutputTypeDef",
     "DescribeGlobalTableOutputTypeDef",
     "UpdateGlobalTableOutputTypeDef",
     "CreateTableOutputTypeDef",
     "DeleteTableOutputTypeDef",
     "DescribeTableOutputTypeDef",
     "RestoreTableFromBackupOutputTypeDef",
     "RestoreTableToPointInTimeOutputTypeDef",
     "UpdateTableOutputTypeDef",
-    "DeleteTableOutputTableTypeDef",
+    "UpdateTableInputRequestTypeDef",
+    "UpdateTableInputTableUpdateTypeDef",
+    "DescribeImportOutputTypeDef",
+    "ImportTableOutputTypeDef",
+    "DeleteBackupOutputTypeDef",
+    "DescribeBackupOutputTypeDef",
+    "BatchWriteItemInputRequestTypeDef",
+    "BatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
     "TableAutoScalingDescriptionTypeDef",
     "DescribeGlobalTableSettingsOutputTypeDef",
     "UpdateGlobalTableSettingsOutputTypeDef",
     "UpdateTableReplicaAutoScalingInputRequestTypeDef",
     "UpdateGlobalTableSettingsInputRequestTypeDef",
     "DescribeTableReplicaAutoScalingOutputTypeDef",
     "UpdateTableReplicaAutoScalingOutputTypeDef",
@@ -396,104 +321,32 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-ArchivalSummaryTableTypeDef = TypedDict(
-    "ArchivalSummaryTableTypeDef",
-    {
-        "ArchivalDateTime": datetime,
-        "ArchivalReason": str,
-        "ArchivalBackupArn": str,
-    },
-)
-
 ArchivalSummaryTypeDef = TypedDict(
     "ArchivalSummaryTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
     },
-)
-
-AttributeDefinitionOutputTypeDef = TypedDict(
-    "AttributeDefinitionOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": ScalarAttributeTypeType,
-    },
-)
-
-AttributeDefinitionServiceResourceTypeDef = TypedDict(
-    "AttributeDefinitionServiceResourceTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": ScalarAttributeTypeType,
-    },
-)
-
-AttributeDefinitionTableOutputTypeDef = TypedDict(
-    "AttributeDefinitionTableOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": ScalarAttributeTypeType,
-    },
-)
-
-AttributeDefinitionTableTypeDef = TypedDict(
-    "AttributeDefinitionTableTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": ScalarAttributeTypeType,
-    },
+    total=False,
 )
 
 AttributeDefinitionTypeDef = TypedDict(
     "AttributeDefinitionTypeDef",
     {
         "AttributeName": str,
         "AttributeType": ScalarAttributeTypeType,
     },
 )
 
-AttributeValueServiceResourceTypeDef = TypedDict(
-    "AttributeValueServiceResourceTypeDef",
-    {
-        "S": str,
-        "N": str,
-        "B": bytes,
-        "SS": List[str],
-        "NS": List[str],
-        "BS": List[bytes],
-        "M": Dict[str, Dict[str, Any]],
-        "L": List[Dict[str, Any]],
-        "NULL": bool,
-        "BOOL": bool,
-    },
-)
-
-AttributeValueTableTypeDef = TypedDict(
-    "AttributeValueTableTypeDef",
-    {
-        "S": str,
-        "N": str,
-        "B": bytes,
-        "SS": List[str],
-        "NS": List[str],
-        "BS": List[bytes],
-        "M": Dict[str, Dict[str, Any]],
-        "L": List[Dict[str, Any]],
-        "NULL": bool,
-        "BOOL": bool,
-    },
-)
-
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "S": str,
         "N": str,
         "B": bytes,
         "SS": Sequence[str],
@@ -503,48 +356,36 @@
         "L": Sequence[Any],
         "NULL": bool,
         "BOOL": bool,
     },
     total=False,
 )
 
-AttributeValueUpdateTableTypeDef = TypedDict(
-    "AttributeValueUpdateTableTypeDef",
+_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
+    "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
-        "Value": Union[
-            bytes,
-            bytearray,
-            str,
-            int,
-            Decimal,
-            bool,
-            Set[int],
-            Set[Decimal],
-            Set[str],
-            Set[bytes],
-            Set[bytearray],
-            Sequence[Any],
-            Mapping[str, Any],
-            None,
-        ],
-        "Action": AttributeActionType,
+        "TargetValue": float,
     },
-    total=False,
 )
-
-AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
-    "AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
+_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef = TypedDict(
+    "_OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef",
     {
         "DisableScaleIn": bool,
         "ScaleInCooldown": int,
         "ScaleOutCooldown": int,
-        "TargetValue": float,
     },
+    total=False,
 )
 
+class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(
+    _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
+    _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
+):
+    pass
+
 _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
     "_RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef = TypedDict(
@@ -559,257 +400,126 @@
 
 class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(
     _RequiredAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     _OptionalAutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
 ):
     pass
 
-BackupDetailsTypeDef = TypedDict(
-    "BackupDetailsTypeDef",
+_RequiredBackupDetailsTypeDef = TypedDict(
+    "_RequiredBackupDetailsTypeDef",
     {
         "BackupArn": str,
         "BackupName": str,
-        "BackupSizeBytes": int,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupCreationDateTime": datetime,
-        "BackupExpiryDateTime": datetime,
     },
 )
-
-BackupSummaryTableTypeDef = TypedDict(
-    "BackupSummaryTableTypeDef",
+_OptionalBackupDetailsTypeDef = TypedDict(
+    "_OptionalBackupDetailsTypeDef",
     {
-        "TableName": str,
-        "TableId": str,
-        "TableArn": str,
-        "BackupArn": str,
-        "BackupName": str,
-        "BackupCreationDateTime": datetime,
-        "BackupExpiryDateTime": datetime,
-        "BackupStatus": BackupStatusType,
-        "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
+        "BackupExpiryDateTime": datetime,
     },
+    total=False,
 )
 
+class BackupDetailsTypeDef(_RequiredBackupDetailsTypeDef, _OptionalBackupDetailsTypeDef):
+    pass
+
 BackupSummaryTypeDef = TypedDict(
     "BackupSummaryTypeDef",
     {
         "TableName": str,
         "TableId": str,
         "TableArn": str,
         "BackupArn": str,
         "BackupName": str,
         "BackupCreationDateTime": datetime,
         "BackupExpiryDateTime": datetime,
         "BackupStatus": BackupStatusType,
         "BackupType": BackupTypeType,
         "BackupSizeBytes": int,
     },
-)
-
-_RequiredKeysAndAttributesServiceResourceTypeDef = TypedDict(
-    "_RequiredKeysAndAttributesServiceResourceTypeDef",
-    {
-        "Keys": Sequence[
-            Mapping[
-                str,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
-    },
-)
-_OptionalKeysAndAttributesServiceResourceTypeDef = TypedDict(
-    "_OptionalKeysAndAttributesServiceResourceTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-    },
     total=False,
 )
 
-class KeysAndAttributesServiceResourceTypeDef(
-    _RequiredKeysAndAttributesServiceResourceTypeDef,
-    _OptionalKeysAndAttributesServiceResourceTypeDef,
-):
-    pass
-
-KeysAndAttributesServiceResourceOutputTypeDef = TypedDict(
-    "KeysAndAttributesServiceResourceOutputTypeDef",
-    {
-        "Keys": List[Dict[str, "AttributeValueServiceResourceTypeDef"]],
-        "AttributesToGet": List[str],
-        "ConsistentRead": bool,
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Dict[str, str],
-    },
-)
-
+TableAttributeValueTypeDef = Union[
+    bytes,
+    bytearray,
+    str,
+    int,
+    Decimal,
+    bool,
+    Set[int],
+    Set[Decimal],
+    Set[str],
+    Set[bytes],
+    Set[bytearray],
+    Sequence[Any],
+    Mapping[str, Any],
+    None,
+]
 BatchStatementErrorTypeDef = TypedDict(
     "BatchStatementErrorTypeDef",
     {
         "Code": BatchStatementErrorCodeEnumType,
         "Message": str,
     },
-)
-
-ItemCollectionMetricsServiceResourceTypeDef = TypedDict(
-    "ItemCollectionMetricsServiceResourceTypeDef",
-    {
-        "ItemCollectionKey": Dict[str, "AttributeValueServiceResourceTypeDef"],
-        "SizeEstimateRangeGB": List[float],
-    },
-)
-
-BillingModeSummaryTableTypeDef = TypedDict(
-    "BillingModeSummaryTableTypeDef",
-    {
-        "BillingMode": BillingModeType,
-        "LastUpdateToPayPerRequestDateTime": datetime,
-    },
+    total=False,
 )
 
 BillingModeSummaryTypeDef = TypedDict(
     "BillingModeSummaryTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
     },
-)
-
-CapacityServiceResourceTypeDef = TypedDict(
-    "CapacityServiceResourceTypeDef",
-    {
-        "ReadCapacityUnits": float,
-        "WriteCapacityUnits": float,
-        "CapacityUnits": float,
-    },
-)
-
-CapacityTableTypeDef = TypedDict(
-    "CapacityTableTypeDef",
-    {
-        "ReadCapacityUnits": float,
-        "WriteCapacityUnits": float,
-        "CapacityUnits": float,
-    },
+    total=False,
 )
 
 CapacityTypeDef = TypedDict(
     "CapacityTypeDef",
     {
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "CapacityUnits": float,
     },
-)
-
-_RequiredConditionTableTypeDef = TypedDict(
-    "_RequiredConditionTableTypeDef",
-    {
-        "ComparisonOperator": ComparisonOperatorType,
-    },
-)
-_OptionalConditionTableTypeDef = TypedDict(
-    "_OptionalConditionTableTypeDef",
-    {
-        "AttributeValueList": Sequence[
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ],
-    },
     total=False,
 )
 
-class ConditionTableTypeDef(_RequiredConditionTableTypeDef, _OptionalConditionTableTypeDef):
-    pass
-
+ConditionBaseImportTypeDef = Union[str, ConditionBase]
 PointInTimeRecoveryDescriptionTypeDef = TypedDict(
     "PointInTimeRecoveryDescriptionTypeDef",
     {
         "PointInTimeRecoveryStatus": PointInTimeRecoveryStatusType,
         "EarliestRestorableDateTime": datetime,
         "LatestRestorableDateTime": datetime,
     },
+    total=False,
 )
 
 ContributorInsightsSummaryTypeDef = TypedDict(
     "ContributorInsightsSummaryTypeDef",
     {
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
     },
+    total=False,
 )
 
 CreateBackupInputRequestTypeDef = TypedDict(
     "CreateBackupInputRequestTypeDef",
     {
         "TableName": str,
         "BackupName": str,
     },
 )
 
-KeySchemaElementTableTypeDef = TypedDict(
-    "KeySchemaElementTableTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": KeyTypeType,
-    },
-)
-
-ProjectionTableTypeDef = TypedDict(
-    "ProjectionTableTypeDef",
-    {
-        "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": Sequence[str],
-    },
-    total=False,
-)
-
-ProvisionedThroughputTableTypeDef = TypedDict(
-    "ProvisionedThroughputTableTypeDef",
-    {
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-)
-
 KeySchemaElementTypeDef = TypedDict(
     "KeySchemaElementTypeDef",
     {
         "AttributeName": str,
         "KeyType": KeyTypeType,
     },
 )
@@ -842,22 +552,14 @@
 CreateReplicaActionTypeDef = TypedDict(
     "CreateReplicaActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
-ProvisionedThroughputOverrideTableTypeDef = TypedDict(
-    "ProvisionedThroughputOverrideTableTypeDef",
-    {
-        "ReadCapacityUnits": int,
-    },
-    total=False,
-)
-
 ProvisionedThroughputOverrideTypeDef = TypedDict(
     "ProvisionedThroughputOverrideTypeDef",
     {
         "ReadCapacityUnits": int,
     },
     total=False,
 )
@@ -895,74 +597,21 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-KeySchemaElementServiceResourceTypeDef = TypedDict(
-    "KeySchemaElementServiceResourceTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": KeyTypeType,
-    },
-)
-
-ProvisionedThroughputServiceResourceTypeDef = TypedDict(
-    "ProvisionedThroughputServiceResourceTypeDef",
-    {
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-)
-
-SSESpecificationServiceResourceTypeDef = TypedDict(
-    "SSESpecificationServiceResourceTypeDef",
-    {
-        "Enabled": bool,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyId": str,
-    },
-    total=False,
-)
-
-_RequiredStreamSpecificationServiceResourceTypeDef = TypedDict(
-    "_RequiredStreamSpecificationServiceResourceTypeDef",
-    {
-        "StreamEnabled": bool,
-    },
-)
-_OptionalStreamSpecificationServiceResourceTypeDef = TypedDict(
-    "_OptionalStreamSpecificationServiceResourceTypeDef",
-    {
-        "StreamViewType": StreamViewTypeType,
-    },
-    total=False,
-)
-
-class StreamSpecificationServiceResourceTypeDef(
-    _RequiredStreamSpecificationServiceResourceTypeDef,
-    _OptionalStreamSpecificationServiceResourceTypeDef,
-):
-    pass
-
-TagServiceResourceTypeDef = TypedDict(
-    "TagServiceResourceTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 CsvOptionsOutputTypeDef = TypedDict(
     "CsvOptionsOutputTypeDef",
     {
         "Delimiter": str,
         "HeaderList": List[str],
     },
+    total=False,
 )
 
 CsvOptionsTypeDef = TypedDict(
     "CsvOptionsTypeDef",
     {
         "Delimiter": str,
         "HeaderList": Sequence[str],
@@ -973,132 +622,35 @@
 DeleteBackupInputRequestTypeDef = TypedDict(
     "DeleteBackupInputRequestTypeDef",
     {
         "BackupArn": str,
     },
 )
 
-DeleteGlobalSecondaryIndexActionTableTypeDef = TypedDict(
-    "DeleteGlobalSecondaryIndexActionTableTypeDef",
-    {
-        "IndexName": str,
-    },
-)
-
 DeleteGlobalSecondaryIndexActionTypeDef = TypedDict(
     "DeleteGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
     },
 )
 
-ExpectedAttributeValueTableTypeDef = TypedDict(
-    "ExpectedAttributeValueTableTypeDef",
-    {
-        "Value": Union[
-            bytes,
-            bytearray,
-            str,
-            int,
-            Decimal,
-            bool,
-            Set[int],
-            Set[Decimal],
-            Set[str],
-            Set[bytes],
-            Set[bytearray],
-            Sequence[Any],
-            Mapping[str, Any],
-            None,
-        ],
-        "Exists": bool,
-        "ComparisonOperator": ComparisonOperatorType,
-        "AttributeValueList": Sequence[
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ]
-        ],
-    },
-    total=False,
-)
-
-ItemCollectionMetricsTableTypeDef = TypedDict(
-    "ItemCollectionMetricsTableTypeDef",
-    {
-        "ItemCollectionKey": Dict[str, "AttributeValueTableTypeDef"],
-        "SizeEstimateRangeGB": List[float],
-    },
-)
-
 DeleteReplicaActionTypeDef = TypedDict(
     "DeleteReplicaActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
-DeleteReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "DeleteReplicationGroupMemberActionTableTypeDef",
-    {
-        "RegionName": str,
-    },
-)
-
 DeleteReplicationGroupMemberActionTypeDef = TypedDict(
     "DeleteReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 
-DeleteRequestServiceResourceOutputTypeDef = TypedDict(
-    "DeleteRequestServiceResourceOutputTypeDef",
-    {
-        "Key": Dict[str, "AttributeValueServiceResourceTypeDef"],
-    },
-)
-
-DeleteRequestServiceResourceTypeDef = TypedDict(
-    "DeleteRequestServiceResourceTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-
 DeleteTableInputRequestTypeDef = TypedDict(
     "DeleteTableInputRequestTypeDef",
     {
         "TableName": str,
     },
 )
 
@@ -1138,14 +690,15 @@
 
 FailureExceptionTypeDef = TypedDict(
     "FailureExceptionTypeDef",
     {
         "ExceptionName": str,
         "ExceptionDescription": str,
     },
+    total=False,
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Address": str,
         "CachePeriodInMinutes": int,
@@ -1178,14 +731,15 @@
         "S3SseKmsKeyId": str,
         "FailureCode": str,
         "FailureMessage": str,
         "ExportFormat": ExportFormatType,
         "BilledSizeBytes": int,
         "ItemCount": int,
     },
+    total=False,
 )
 
 DescribeGlobalTableInputRequestTypeDef = TypedDict(
     "DescribeGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
     },
@@ -1215,14 +769,15 @@
 KinesisDataStreamDestinationTypeDef = TypedDict(
     "KinesisDataStreamDestinationTypeDef",
     {
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "DestinationStatusDescription": str,
     },
+    total=False,
 )
 
 DescribeTableInputRequestTypeDef = TypedDict(
     "DescribeTableInputRequestTypeDef",
     {
         "TableName": str,
     },
@@ -1253,179 +808,48 @@
 
 TimeToLiveDescriptionTypeDef = TypedDict(
     "TimeToLiveDescriptionTypeDef",
     {
         "TimeToLiveStatus": TimeToLiveStatusType,
         "AttributeName": str,
     },
+    total=False,
 )
 
 ExportSummaryTypeDef = TypedDict(
     "ExportSummaryTypeDef",
     {
         "ExportArn": str,
         "ExportStatus": ExportStatusType,
     },
-)
-
-_RequiredExportTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_RequiredExportTableToPointInTimeInputRequestTypeDef",
-    {
-        "TableArn": str,
-        "S3Bucket": str,
-    },
-)
-_OptionalExportTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_OptionalExportTableToPointInTimeInputRequestTypeDef",
-    {
-        "ExportTime": Union[datetime, str],
-        "ClientToken": str,
-        "S3BucketOwner": str,
-        "S3Prefix": str,
-        "S3SseAlgorithm": S3SseAlgorithmType,
-        "S3SseKmsKeyId": str,
-        "ExportFormat": ExportFormatType,
-    },
     total=False,
 )
 
-class ExportTableToPointInTimeInputRequestTypeDef(
-    _RequiredExportTableToPointInTimeInputRequestTypeDef,
-    _OptionalExportTableToPointInTimeInputRequestTypeDef,
-):
-    pass
-
-_RequiredGetItemInputTableGetItemTypeDef = TypedDict(
-    "_RequiredGetItemInputTableGetItemTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalGetItemInputTableGetItemTypeDef = TypedDict(
-    "_OptionalGetItemInputTableGetItemTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-    },
-    total=False,
-)
-
-class GetItemInputTableGetItemTypeDef(
-    _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
-):
-    pass
-
-KeySchemaElementTableOutputTypeDef = TypedDict(
-    "KeySchemaElementTableOutputTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": KeyTypeType,
-    },
-)
-
-ProjectionTableOutputTypeDef = TypedDict(
-    "ProjectionTableOutputTypeDef",
-    {
-        "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": List[str],
-    },
-)
-
-ProvisionedThroughputDescriptionTableTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionTableTypeDef",
-    {
-        "LastIncreaseDateTime": datetime,
-        "LastDecreaseDateTime": datetime,
-        "NumberOfDecreasesToday": int,
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-)
-
-KeySchemaElementOutputTypeDef = TypedDict(
-    "KeySchemaElementOutputTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": KeyTypeType,
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ProjectionOutputTypeDef = TypedDict(
     "ProjectionOutputTypeDef",
     {
         "ProjectionType": ProjectionTypeType,
         "NonKeyAttributes": List[str],
     },
+    total=False,
 )
 
 ProvisionedThroughputDescriptionTypeDef = TypedDict(
     "ProvisionedThroughputDescriptionTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
     },
-)
-
-ProvisionedThroughputOutputTypeDef = TypedDict(
-    "ProvisionedThroughputOutputTypeDef",
-    {
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-)
-
-ProjectionServiceResourceTypeDef = TypedDict(
-    "ProjectionServiceResourceTypeDef",
-    {
-        "ProjectionType": ProjectionTypeType,
-        "NonKeyAttributes": Sequence[str],
-    },
     total=False,
 )
 
-ReplicaOutputTypeDef = TypedDict(
-    "ReplicaOutputTypeDef",
-    {
-        "RegionName": str,
-    },
-)
-
-S3BucketSourceOutputTypeDef = TypedDict(
-    "S3BucketSourceOutputTypeDef",
-    {
-        "S3BucketOwner": str,
-        "S3Bucket": str,
-        "S3KeyPrefix": str,
-    },
-)
-
 _RequiredS3BucketSourceTypeDef = TypedDict(
     "_RequiredS3BucketSourceTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalS3BucketSourceTypeDef = TypedDict(
@@ -1454,27 +878,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-ListBackupsInputRequestTypeDef = TypedDict(
-    "ListBackupsInputRequestTypeDef",
-    {
-        "TableName": str,
-        "Limit": int,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
-        "ExclusiveStartBackupArn": str,
-        "BackupType": BackupTypeFilterType,
-    },
-    total=False,
-)
-
 ListContributorInsightsInputRequestTypeDef = TypedDict(
     "ListContributorInsightsInputRequestTypeDef",
     {
         "TableName": str,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -1535,209 +946,68 @@
 )
 
 class ListTagsOfResourceInputRequestTypeDef(
     _RequiredListTagsOfResourceInputRequestTypeDef, _OptionalListTagsOfResourceInputRequestTypeDef
 ):
     pass
 
-TagTableTypeDef = TypedDict(
-    "TagTableTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 PointInTimeRecoverySpecificationTypeDef = TypedDict(
     "PointInTimeRecoverySpecificationTypeDef",
     {
         "PointInTimeRecoveryEnabled": bool,
     },
 )
 
-ProvisionedThroughputOverrideOutputTypeDef = TypedDict(
-    "ProvisionedThroughputOverrideOutputTypeDef",
-    {
-        "ReadCapacityUnits": int,
-    },
-)
-
-ProvisionedThroughputOverrideTableOutputTypeDef = TypedDict(
-    "ProvisionedThroughputOverrideTableOutputTypeDef",
-    {
-        "ReadCapacityUnits": int,
-    },
-)
-
-PutRequestServiceResourceOutputTypeDef = TypedDict(
-    "PutRequestServiceResourceOutputTypeDef",
-    {
-        "Item": Dict[str, "AttributeValueServiceResourceTypeDef"],
-    },
-)
-
-PutRequestServiceResourceTypeDef = TypedDict(
-    "PutRequestServiceResourceTypeDef",
-    {
-        "Item": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-
-TableClassSummaryTableTypeDef = TypedDict(
-    "TableClassSummaryTableTypeDef",
-    {
-        "TableClass": TableClassType,
-        "LastUpdateDateTime": datetime,
-    },
-)
-
 TableClassSummaryTypeDef = TypedDict(
     "TableClassSummaryTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
     },
+    total=False,
 )
 
-RestoreSummaryTableTypeDef = TypedDict(
-    "RestoreSummaryTableTypeDef",
+_RequiredRestoreSummaryTypeDef = TypedDict(
+    "_RequiredRestoreSummaryTypeDef",
     {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
     },
 )
-
-RestoreSummaryTypeDef = TypedDict(
-    "RestoreSummaryTypeDef",
+_OptionalRestoreSummaryTypeDef = TypedDict(
+    "_OptionalRestoreSummaryTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
-        "RestoreDateTime": datetime,
-        "RestoreInProgress": bool,
     },
+    total=False,
 )
 
-SSEDescriptionTableTypeDef = TypedDict(
-    "SSEDescriptionTableTypeDef",
-    {
-        "Status": SSEStatusType,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyArn": str,
-        "InaccessibleEncryptionDateTime": datetime,
-    },
-)
+class RestoreSummaryTypeDef(_RequiredRestoreSummaryTypeDef, _OptionalRestoreSummaryTypeDef):
+    pass
 
 SSEDescriptionTypeDef = TypedDict(
     "SSEDescriptionTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
     },
-)
-
-SSESpecificationOutputTypeDef = TypedDict(
-    "SSESpecificationOutputTypeDef",
-    {
-        "Enabled": bool,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyId": str,
-    },
-)
-
-SSESpecificationTableTypeDef = TypedDict(
-    "SSESpecificationTableTypeDef",
-    {
-        "Enabled": bool,
-        "SSEType": SSETypeType,
-        "KMSMasterKeyId": str,
-    },
     total=False,
 )
 
-StreamSpecificationOutputTypeDef = TypedDict(
-    "StreamSpecificationOutputTypeDef",
-    {
-        "StreamEnabled": bool,
-        "StreamViewType": StreamViewTypeType,
-    },
-)
-
-StreamSpecificationTableOutputTypeDef = TypedDict(
-    "StreamSpecificationTableOutputTypeDef",
-    {
-        "StreamEnabled": bool,
-        "StreamViewType": StreamViewTypeType,
-    },
-)
-
-_RequiredStreamSpecificationTableTypeDef = TypedDict(
-    "_RequiredStreamSpecificationTableTypeDef",
-    {
-        "StreamEnabled": bool,
-    },
-)
-_OptionalStreamSpecificationTableTypeDef = TypedDict(
-    "_OptionalStreamSpecificationTableTypeDef",
-    {
-        "StreamViewType": StreamViewTypeType,
-    },
-    total=False,
-)
-
-class StreamSpecificationTableTypeDef(
-    _RequiredStreamSpecificationTableTypeDef, _OptionalStreamSpecificationTableTypeDef
-):
-    pass
-
 TableBatchWriterRequestTypeDef = TypedDict(
     "TableBatchWriterRequestTypeDef",
     {
         "overwrite_by_pkeys": List[str],
     },
     total=False,
 )
 
-TimeToLiveSpecificationOutputTypeDef = TypedDict(
-    "TimeToLiveSpecificationOutputTypeDef",
-    {
-        "Enabled": bool,
-        "AttributeName": str,
-    },
-)
-
 TimeToLiveSpecificationTypeDef = TypedDict(
     "TimeToLiveSpecificationTypeDef",
     {
         "Enabled": bool,
         "AttributeName": str,
     },
 )
@@ -1767,26 +1037,26 @@
 
 class UpdateContributorInsightsInputRequestTypeDef(
     _RequiredUpdateContributorInsightsInputRequestTypeDef,
     _OptionalUpdateContributorInsightsInputRequestTypeDef,
 ):
     pass
 
-ArchivalSummaryTableResponseMetadataTypeDef = TypedDict(
-    "ArchivalSummaryTableResponseMetadataTypeDef",
+ArchivalSummaryResponseTypeDef = TypedDict(
+    "ArchivalSummaryResponseTypeDef",
     {
         "ArchivalDateTime": datetime,
         "ArchivalReason": str,
         "ArchivalBackupArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BillingModeSummaryTableResponseMetadataTypeDef = TypedDict(
-    "BillingModeSummaryTableResponseMetadataTypeDef",
+BillingModeSummaryResponseTypeDef = TypedDict(
+    "BillingModeSummaryResponseTypeDef",
     {
         "BillingMode": BillingModeType,
         "LastUpdateToPayPerRequestDateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1814,77 +1084,68 @@
         "TableName": str,
         "StreamArn": str,
         "DestinationStatus": DestinationStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTablesOutputTableTypeDef = TypedDict(
-    "ListTablesOutputTableTypeDef",
-    {
-        "TableNames": List[str],
-        "LastEvaluatedTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListTablesOutputTypeDef = TypedDict(
     "ListTablesOutputTypeDef",
     {
         "TableNames": List[str],
         "LastEvaluatedTableName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProvisionedThroughputDescriptionTableResponseMetadataTypeDef = TypedDict(
-    "ProvisionedThroughputDescriptionTableResponseMetadataTypeDef",
+ProvisionedThroughputDescriptionResponseTypeDef = TypedDict(
+    "ProvisionedThroughputDescriptionResponseTypeDef",
     {
         "LastIncreaseDateTime": datetime,
         "LastDecreaseDateTime": datetime,
         "NumberOfDecreasesToday": int,
         "ReadCapacityUnits": int,
         "WriteCapacityUnits": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RestoreSummaryTableResponseMetadataTypeDef = TypedDict(
-    "RestoreSummaryTableResponseMetadataTypeDef",
+RestoreSummaryResponseTypeDef = TypedDict(
+    "RestoreSummaryResponseTypeDef",
     {
         "SourceBackupArn": str,
         "SourceTableArn": str,
         "RestoreDateTime": datetime,
         "RestoreInProgress": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SSEDescriptionTableResponseMetadataTypeDef = TypedDict(
-    "SSEDescriptionTableResponseMetadataTypeDef",
+SSEDescriptionResponseTypeDef = TypedDict(
+    "SSEDescriptionResponseTypeDef",
     {
         "Status": SSEStatusType,
         "SSEType": SSETypeType,
         "KMSMasterKeyArn": str,
         "InaccessibleEncryptionDateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StreamSpecificationTableResponseMetadataTypeDef = TypedDict(
-    "StreamSpecificationTableResponseMetadataTypeDef",
+StreamSpecificationResponseTypeDef = TypedDict(
+    "StreamSpecificationResponseTypeDef",
     {
         "StreamEnabled": bool,
         "StreamViewType": StreamViewTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TableClassSummaryTableResponseMetadataTypeDef = TypedDict(
-    "TableClassSummaryTableResponseMetadataTypeDef",
+TableClassSummaryResponseTypeDef = TypedDict(
+    "TableClassSummaryResponseTypeDef",
     {
         "TableClass": TableClassType,
         "LastUpdateDateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1894,1017 +1155,208 @@
         "TableName": str,
         "IndexName": str,
         "ContributorInsightsStatus": ContributorInsightsStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttributeValueUpdateTypeDef = TypedDict(
-    "AttributeValueUpdateTypeDef",
+UniversalAttributeValueTypeDef = Union[
+    AttributeValueTypeDef,
+    bytes,
+    bytearray,
+    str,
+    int,
+    Decimal,
+    bool,
+    Set[int],
+    Set[Decimal],
+    Set[str],
+    Set[bytes],
+    Set[bytearray],
+    Sequence[Any],
+    Mapping[str, Any],
+    None,
+]
+AutoScalingPolicyDescriptionTypeDef = TypedDict(
+    "AutoScalingPolicyDescriptionTypeDef",
     {
-        "Value": Union[
-            AttributeValueTypeDef,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "Action": AttributeActionType,
+        "PolicyName": str,
+        "TargetTrackingScalingPolicyConfiguration": (
+            AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
+        ),
     },
     total=False,
 )
 
-_RequiredBatchStatementRequestTypeDef = TypedDict(
-    "_RequiredBatchStatementRequestTypeDef",
+_RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
+    "_RequiredAutoScalingPolicyUpdateTypeDef",
     {
-        "Statement": str,
+        "TargetTrackingScalingPolicyConfiguration": (
+            AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
+        ),
     },
 )
-_OptionalBatchStatementRequestTypeDef = TypedDict(
-    "_OptionalBatchStatementRequestTypeDef",
+_OptionalAutoScalingPolicyUpdateTypeDef = TypedDict(
+    "_OptionalAutoScalingPolicyUpdateTypeDef",
     {
-        "Parameters": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
-        "ConsistentRead": bool,
+        "PolicyName": str,
     },
     total=False,
 )
 
-class BatchStatementRequestTypeDef(
-    _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
+class AutoScalingPolicyUpdateTypeDef(
+    _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
 ):
     pass
 
-_RequiredConditionCheckTypeDef = TypedDict(
-    "_RequiredConditionCheckTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "TableName": str,
-        "ConditionExpression": str,
-    },
-)
-_OptionalConditionCheckTypeDef = TypedDict(
-    "_OptionalConditionCheckTypeDef",
+CreateBackupOutputTypeDef = TypedDict(
+    "CreateBackupOutputTypeDef",
     {
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
+        "BackupDetails": BackupDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ConditionCheckTypeDef(_RequiredConditionCheckTypeDef, _OptionalConditionCheckTypeDef):
-    pass
-
-_RequiredConditionTypeDef = TypedDict(
-    "_RequiredConditionTypeDef",
-    {
-        "ComparisonOperator": ComparisonOperatorType,
-    },
-)
-_OptionalConditionTypeDef = TypedDict(
-    "_OptionalConditionTypeDef",
+ListBackupsOutputTypeDef = TypedDict(
+    "ListBackupsOutputTypeDef",
     {
-        "AttributeValueList": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "BackupSummaries": List[BackupSummaryTypeDef],
+        "LastEvaluatedBackupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ConditionTypeDef(_RequiredConditionTypeDef, _OptionalConditionTypeDef):
-    pass
-
 DeleteRequestOutputTypeDef = TypedDict(
     "DeleteRequestOutputTypeDef",
     {
-        "Key": Dict[str, AttributeValueTypeDef],
+        "Key": Dict[str, TableAttributeValueTypeDef],
     },
 )
 
-DeleteRequestTypeDef = TypedDict(
-    "DeleteRequestTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-    },
-)
-
-_RequiredDeleteTypeDef = TypedDict(
-    "_RequiredDeleteTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "TableName": str,
-    },
-)
-_OptionalDeleteTypeDef = TypedDict(
-    "_OptionalDeleteTypeDef",
-    {
-        "ConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
-    pass
-
-_RequiredExecuteStatementInputRequestTypeDef = TypedDict(
-    "_RequiredExecuteStatementInputRequestTypeDef",
-    {
-        "Statement": str,
-    },
-)
-_OptionalExecuteStatementInputRequestTypeDef = TypedDict(
-    "_OptionalExecuteStatementInputRequestTypeDef",
-    {
-        "Parameters": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
-        "ConsistentRead": bool,
-        "NextToken": str,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "Limit": int,
-    },
-    total=False,
-)
-
-class ExecuteStatementInputRequestTypeDef(
-    _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
-):
-    pass
-
-ExpectedAttributeValueTypeDef = TypedDict(
-    "ExpectedAttributeValueTypeDef",
-    {
-        "Value": Union[
-            AttributeValueTypeDef,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "Exists": bool,
-        "ComparisonOperator": ComparisonOperatorType,
-        "AttributeValueList": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
-    },
-    total=False,
-)
-
-_RequiredGetItemInputRequestTypeDef = TypedDict(
-    "_RequiredGetItemInputRequestTypeDef",
+_RequiredGetItemInputTableGetItemTypeDef = TypedDict(
+    "_RequiredGetItemInputTableGetItemTypeDef",
     {
-        "TableName": str,
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
-_OptionalGetItemInputRequestTypeDef = TypedDict(
-    "_OptionalGetItemInputRequestTypeDef",
+_OptionalGetItemInputTableGetItemTypeDef = TypedDict(
+    "_OptionalGetItemInputTableGetItemTypeDef",
     {
         "AttributesToGet": Sequence[str],
         "ConsistentRead": bool,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
     },
     total=False,
 )
 
-class GetItemInputRequestTypeDef(
-    _RequiredGetItemInputRequestTypeDef, _OptionalGetItemInputRequestTypeDef
+class GetItemInputTableGetItemTypeDef(
+    _RequiredGetItemInputTableGetItemTypeDef, _OptionalGetItemInputTableGetItemTypeDef
 ):
     pass
 
-_RequiredGetTypeDef = TypedDict(
-    "_RequiredGetTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "TableName": str,
-    },
-)
-_OptionalGetTypeDef = TypedDict(
-    "_OptionalGetTypeDef",
-    {
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-    },
-    total=False,
-)
-
-class GetTypeDef(_RequiredGetTypeDef, _OptionalGetTypeDef):
-    pass
-
 ItemCollectionMetricsTypeDef = TypedDict(
     "ItemCollectionMetricsTypeDef",
     {
-        "ItemCollectionKey": Dict[str, AttributeValueTypeDef],
+        "ItemCollectionKey": Dict[str, TableAttributeValueTypeDef],
         "SizeEstimateRangeGB": List[float],
     },
+    total=False,
 )
 
 ItemResponseTypeDef = TypedDict(
     "ItemResponseTypeDef",
     {
-        "Item": Dict[str, AttributeValueTypeDef],
-    },
-)
-
-KeysAndAttributesOutputTypeDef = TypedDict(
-    "KeysAndAttributesOutputTypeDef",
-    {
-        "Keys": List[Dict[str, AttributeValueTypeDef]],
-        "AttributesToGet": List[str],
-        "ConsistentRead": bool,
-        "ProjectionExpression": str,
-        "ExpressionAttributeNames": Dict[str, str],
+        "Item": Dict[str, TableAttributeValueTypeDef],
     },
+    total=False,
 )
 
-_RequiredKeysAndAttributesTypeDef = TypedDict(
-    "_RequiredKeysAndAttributesTypeDef",
+_RequiredKeysAndAttributesOutputTypeDef = TypedDict(
+    "_RequiredKeysAndAttributesOutputTypeDef",
     {
-        "Keys": Sequence[
-            Mapping[
-                str,
-                Union[
-                    AttributeValueTypeDef,
-                    Union[
-                        bytes,
-                        bytearray,
-                        str,
-                        int,
-                        Decimal,
-                        bool,
-                        Set[int],
-                        Set[Decimal],
-                        Set[str],
-                        Set[bytes],
-                        Set[bytearray],
-                        Sequence[Any],
-                        Mapping[str, Any],
-                        None,
-                    ],
-                ],
-            ]
-        ],
+        "Keys": List[Dict[str, TableAttributeValueTypeDef]],
     },
 )
-_OptionalKeysAndAttributesTypeDef = TypedDict(
-    "_OptionalKeysAndAttributesTypeDef",
+_OptionalKeysAndAttributesOutputTypeDef = TypedDict(
+    "_OptionalKeysAndAttributesOutputTypeDef",
     {
-        "AttributesToGet": Sequence[str],
+        "AttributesToGet": List[str],
         "ConsistentRead": bool,
         "ProjectionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-    },
-    total=False,
-)
-
-class KeysAndAttributesTypeDef(
-    _RequiredKeysAndAttributesTypeDef, _OptionalKeysAndAttributesTypeDef
-):
-    pass
-
-_RequiredParameterizedStatementTypeDef = TypedDict(
-    "_RequiredParameterizedStatementTypeDef",
-    {
-        "Statement": str,
-    },
-)
-_OptionalParameterizedStatementTypeDef = TypedDict(
-    "_OptionalParameterizedStatementTypeDef",
-    {
-        "Parameters": Sequence[
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ]
-        ],
+        "ExpressionAttributeNames": Dict[str, str],
     },
     total=False,
 )
 
-class ParameterizedStatementTypeDef(
-    _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
+class KeysAndAttributesOutputTypeDef(
+    _RequiredKeysAndAttributesOutputTypeDef, _OptionalKeysAndAttributesOutputTypeDef
 ):
     pass
 
 PutRequestOutputTypeDef = TypedDict(
     "PutRequestOutputTypeDef",
     {
-        "Item": Dict[str, AttributeValueTypeDef],
-    },
-)
-
-PutRequestTypeDef = TypedDict(
-    "PutRequestTypeDef",
-    {
-        "Item": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "Item": Dict[str, TableAttributeValueTypeDef],
     },
 )
 
-_RequiredPutTypeDef = TypedDict(
-    "_RequiredPutTypeDef",
-    {
-        "Item": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "TableName": str,
-    },
-)
-_OptionalPutTypeDef = TypedDict(
-    "_OptionalPutTypeDef",
-    {
-        "ConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-class PutTypeDef(_RequiredPutTypeDef, _OptionalPutTypeDef):
-    pass
-
-_RequiredUpdateTypeDef = TypedDict(
-    "_RequiredUpdateTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "UpdateExpression": str,
-        "TableName": str,
-    },
-)
-_OptionalUpdateTypeDef = TypedDict(
-    "_OptionalUpdateTypeDef",
-    {
-        "ConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
-    },
-    total=False,
-)
-
-class UpdateTypeDef(_RequiredUpdateTypeDef, _OptionalUpdateTypeDef):
-    pass
-
-AutoScalingPolicyDescriptionTypeDef = TypedDict(
-    "AutoScalingPolicyDescriptionTypeDef",
-    {
-        "PolicyName": str,
-        "TargetTrackingScalingPolicyConfiguration": (
-            AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef
-        ),
-    },
-)
-
-_RequiredAutoScalingPolicyUpdateTypeDef = TypedDict(
-    "_RequiredAutoScalingPolicyUpdateTypeDef",
-    {
-        "TargetTrackingScalingPolicyConfiguration": (
-            AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef
-        ),
-    },
-)
-_OptionalAutoScalingPolicyUpdateTypeDef = TypedDict(
-    "_OptionalAutoScalingPolicyUpdateTypeDef",
-    {
-        "PolicyName": str,
-    },
-    total=False,
-)
-
-class AutoScalingPolicyUpdateTypeDef(
-    _RequiredAutoScalingPolicyUpdateTypeDef, _OptionalAutoScalingPolicyUpdateTypeDef
-):
-    pass
-
-CreateBackupOutputTypeDef = TypedDict(
-    "CreateBackupOutputTypeDef",
-    {
-        "BackupDetails": BackupDetailsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupsOutputTableTypeDef = TypedDict(
-    "ListBackupsOutputTableTypeDef",
-    {
-        "BackupSummaries": List[BackupSummaryTableTypeDef],
-        "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListBackupsOutputTypeDef = TypedDict(
-    "ListBackupsOutputTypeDef",
-    {
-        "BackupSummaries": List[BackupSummaryTypeDef],
-        "LastEvaluatedBackupArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
-    "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    {
-        "RequestItems": Mapping[str, KeysAndAttributesServiceResourceTypeDef],
-    },
-)
-_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
-    "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
-    {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-    },
-    total=False,
-)
-
-class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
-    _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
-    _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
-):
-    pass
-
 BatchStatementResponseTypeDef = TypedDict(
     "BatchStatementResponseTypeDef",
     {
         "Error": BatchStatementErrorTypeDef,
         "TableName": str,
-        "Item": Dict[str, AttributeValueTypeDef],
-    },
-)
-
-ConsumedCapacityServiceResourceTypeDef = TypedDict(
-    "ConsumedCapacityServiceResourceTypeDef",
-    {
-        "TableName": str,
-        "CapacityUnits": float,
-        "ReadCapacityUnits": float,
-        "WriteCapacityUnits": float,
-        "Table": CapacityServiceResourceTypeDef,
-        "LocalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
-        "GlobalSecondaryIndexes": Dict[str, CapacityServiceResourceTypeDef],
-    },
-)
-
-ConsumedCapacityTableTypeDef = TypedDict(
-    "ConsumedCapacityTableTypeDef",
-    {
-        "TableName": str,
-        "CapacityUnits": float,
-        "ReadCapacityUnits": float,
-        "WriteCapacityUnits": float,
-        "Table": CapacityTableTypeDef,
-        "LocalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
-        "GlobalSecondaryIndexes": Dict[str, CapacityTableTypeDef],
+        "Item": Dict[str, TableAttributeValueTypeDef],
     },
+    total=False,
 )
 
 ConsumedCapacityTypeDef = TypedDict(
     "ConsumedCapacityTypeDef",
     {
         "TableName": str,
         "CapacityUnits": float,
         "ReadCapacityUnits": float,
         "WriteCapacityUnits": float,
         "Table": CapacityTypeDef,
         "LocalSecondaryIndexes": Dict[str, CapacityTypeDef],
         "GlobalSecondaryIndexes": Dict[str, CapacityTypeDef],
     },
-)
-
-QueryInputTableQueryTypeDef = TypedDict(
-    "QueryInputTableQueryTypeDef",
-    {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": Union[str, ConditionBase],
-        "KeyConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
     total=False,
 )
 
-ScanInputTableScanTypeDef = TypedDict(
-    "ScanInputTableScanTypeDef",
+_RequiredContinuousBackupsDescriptionTypeDef = TypedDict(
+    "_RequiredContinuousBackupsDescriptionTypeDef",
     {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
+        "ContinuousBackupsStatus": ContinuousBackupsStatusType,
     },
-    total=False,
 )
-
-ContinuousBackupsDescriptionTypeDef = TypedDict(
-    "ContinuousBackupsDescriptionTypeDef",
+_OptionalContinuousBackupsDescriptionTypeDef = TypedDict(
+    "_OptionalContinuousBackupsDescriptionTypeDef",
     {
-        "ContinuousBackupsStatus": ContinuousBackupsStatusType,
         "PointInTimeRecoveryDescription": PointInTimeRecoveryDescriptionTypeDef,
     },
+    total=False,
 )
 
+class ContinuousBackupsDescriptionTypeDef(
+    _RequiredContinuousBackupsDescriptionTypeDef, _OptionalContinuousBackupsDescriptionTypeDef
+):
+    pass
+
 ListContributorInsightsOutputTypeDef = TypedDict(
     "ListContributorInsightsOutputTypeDef",
     {
         "ContributorInsightsSummaries": List[ContributorInsightsSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
-    "_RequiredCreateGlobalSecondaryIndexActionTableTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": Sequence[KeySchemaElementTableTypeDef],
-        "Projection": ProjectionTableTypeDef,
-    },
-)
-_OptionalCreateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
-    "_OptionalCreateGlobalSecondaryIndexActionTableTypeDef",
-    {
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
-    },
-    total=False,
-)
-
-class CreateGlobalSecondaryIndexActionTableTypeDef(
-    _RequiredCreateGlobalSecondaryIndexActionTableTypeDef,
-    _OptionalCreateGlobalSecondaryIndexActionTableTypeDef,
-):
-    pass
-
-UpdateGlobalSecondaryIndexActionTableTypeDef = TypedDict(
-    "UpdateGlobalSecondaryIndexActionTableTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
-    },
-)
-
 LocalSecondaryIndexTypeDef = TypedDict(
     "LocalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "KeySchema": Sequence[KeySchemaElementTypeDef],
         "Projection": ProjectionTypeDef,
     },
@@ -2949,14 +1401,40 @@
 )
 
 class GlobalSecondaryIndexTypeDef(
     _RequiredGlobalSecondaryIndexTypeDef, _OptionalGlobalSecondaryIndexTypeDef
 ):
     pass
 
+_RequiredSourceTableDetailsTypeDef = TypedDict(
+    "_RequiredSourceTableDetailsTypeDef",
+    {
+        "TableName": str,
+        "TableId": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "TableCreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+    },
+)
+_OptionalSourceTableDetailsTypeDef = TypedDict(
+    "_OptionalSourceTableDetailsTypeDef",
+    {
+        "TableArn": str,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "BillingMode": BillingModeType,
+    },
+    total=False,
+)
+
+class SourceTableDetailsTypeDef(
+    _RequiredSourceTableDetailsTypeDef, _OptionalSourceTableDetailsTypeDef
+):
+    pass
+
 UpdateGlobalSecondaryIndexActionTypeDef = TypedDict(
     "UpdateGlobalSecondaryIndexActionTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
 )
@@ -2965,34 +1443,32 @@
     "CreateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicationGroup": Sequence[ReplicaTypeDef],
     },
 )
 
-_RequiredReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
-    "_RequiredReplicaGlobalSecondaryIndexTableTypeDef",
+GlobalTableTypeDef = TypedDict(
+    "GlobalTableTypeDef",
     {
-        "IndexName": str,
+        "GlobalTableName": str,
+        "ReplicationGroup": List[ReplicaTypeDef],
     },
+    total=False,
 )
-_OptionalReplicaGlobalSecondaryIndexTableTypeDef = TypedDict(
-    "_OptionalReplicaGlobalSecondaryIndexTableTypeDef",
+
+ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
     {
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
+        "IndexName": str,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
     },
     total=False,
 )
 
-class ReplicaGlobalSecondaryIndexTableTypeDef(
-    _RequiredReplicaGlobalSecondaryIndexTableTypeDef,
-    _OptionalReplicaGlobalSecondaryIndexTableTypeDef,
-):
-    pass
-
 _RequiredReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "_RequiredReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
     },
 )
 _OptionalReplicaGlobalSecondaryIndexTypeDef = TypedDict(
@@ -3004,225 +1480,47 @@
 )
 
 class ReplicaGlobalSecondaryIndexTypeDef(
     _RequiredReplicaGlobalSecondaryIndexTypeDef, _OptionalReplicaGlobalSecondaryIndexTypeDef
 ):
     pass
 
+ListTagsOfResourceOutputTypeDef = TypedDict(
+    "ListTagsOfResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 InputFormatOptionsOutputTypeDef = TypedDict(
     "InputFormatOptionsOutputTypeDef",
     {
         "Csv": CsvOptionsOutputTypeDef,
     },
+    total=False,
 )
 
 InputFormatOptionsTypeDef = TypedDict(
     "InputFormatOptionsTypeDef",
     {
         "Csv": CsvOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredDeleteItemInputTableDeleteItemTypeDef = TypedDict(
-    "_RequiredDeleteItemInputTableDeleteItemTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalDeleteItemInputTableDeleteItemTypeDef = TypedDict(
-    "_OptionalDeleteItemInputTableDeleteItemTypeDef",
-    {
-        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-    total=False,
-)
-
-class DeleteItemInputTableDeleteItemTypeDef(
-    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
-):
-    pass
-
-_RequiredPutItemInputTablePutItemTypeDef = TypedDict(
-    "_RequiredPutItemInputTablePutItemTypeDef",
-    {
-        "Item": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalPutItemInputTablePutItemTypeDef = TypedDict(
-    "_OptionalPutItemInputTablePutItemTypeDef",
-    {
-        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionalOperator": ConditionalOperatorType,
-        "ConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-    total=False,
-)
-
-class PutItemInputTablePutItemTypeDef(
-    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
-):
-    pass
-
-_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
-    {
-        "Key": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-)
-_OptionalUpdateItemInputTableUpdateItemTypeDef = TypedDict(
-    "_OptionalUpdateItemInputTableUpdateItemTypeDef",
-    {
-        "AttributeUpdates": Mapping[str, AttributeValueUpdateTableTypeDef],
-        "Expected": Mapping[str, ExpectedAttributeValueTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "UpdateExpression": str,
-        "ConditionExpression": Union[str, ConditionBase],
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-    },
-    total=False,
-)
-
-class UpdateItemInputTableUpdateItemTypeDef(
-    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
-):
-    pass
-
 ReplicaUpdateTypeDef = TypedDict(
     "ReplicaUpdateTypeDef",
     {
         "Create": CreateReplicaActionTypeDef,
         "Delete": DeleteReplicaActionTypeDef,
     },
     total=False,
@@ -3327,171 +1625,146 @@
     {
         "ExportSummaries": List[ExportSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LocalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTableTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
-        "Projection": ProjectionTableOutputTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
-    },
-)
-
-GlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "GlobalSecondaryIndexDescriptionTableTypeDef",
+_RequiredExportTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_RequiredExportTableToPointInTimeInputRequestTypeDef",
     {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
-        "Projection": ProjectionTableOutputTypeDef,
-        "IndexStatus": IndexStatusType,
-        "Backfilling": bool,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
+        "TableArn": str,
+        "S3Bucket": str,
     },
 )
-
-LocalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "LocalSecondaryIndexDescriptionTypeDef",
+_OptionalExportTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_OptionalExportTableToPointInTimeInputRequestTypeDef",
     {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
+        "ExportTime": TimestampTypeDef,
+        "ClientToken": str,
+        "S3BucketOwner": str,
+        "S3Prefix": str,
+        "S3SseAlgorithm": S3SseAlgorithmType,
+        "S3SseKmsKeyId": str,
+        "ExportFormat": ExportFormatType,
     },
+    total=False,
 )
 
-LocalSecondaryIndexInfoTypeDef = TypedDict(
-    "LocalSecondaryIndexInfoTypeDef",
-    {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-    },
-)
+class ExportTableToPointInTimeInputRequestTypeDef(
+    _RequiredExportTableToPointInTimeInputRequestTypeDef,
+    _OptionalExportTableToPointInTimeInputRequestTypeDef,
+):
+    pass
 
-GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "GlobalSecondaryIndexDescriptionTypeDef",
+ListBackupsInputRequestTypeDef = TypedDict(
+    "ListBackupsInputRequestTypeDef",
     {
-        "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "Projection": ProjectionOutputTypeDef,
-        "IndexStatus": IndexStatusType,
-        "Backfilling": bool,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
-        "IndexSizeBytes": int,
-        "ItemCount": int,
-        "IndexArn": str,
+        "TableName": str,
+        "Limit": int,
+        "TimeRangeLowerBound": TimestampTypeDef,
+        "TimeRangeUpperBound": TimestampTypeDef,
+        "ExclusiveStartBackupArn": str,
+        "BackupType": BackupTypeFilterType,
     },
+    total=False,
 )
 
 GlobalSecondaryIndexInfoTypeDef = TypedDict(
     "GlobalSecondaryIndexInfoTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
         "Projection": ProjectionOutputTypeDef,
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
+    total=False,
 )
 
-GlobalSecondaryIndexOutputTypeDef = TypedDict(
-    "GlobalSecondaryIndexOutputTypeDef",
+_RequiredGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "_RequiredGlobalSecondaryIndexOutputTypeDef",
     {
         "IndexName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
         "Projection": ProjectionOutputTypeDef,
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
     },
 )
-
-SourceTableDetailsTypeDef = TypedDict(
-    "SourceTableDetailsTypeDef",
+_OptionalGlobalSecondaryIndexOutputTypeDef = TypedDict(
+    "_OptionalGlobalSecondaryIndexOutputTypeDef",
     {
-        "TableName": str,
-        "TableId": str,
-        "TableArn": str,
-        "TableSizeBytes": int,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "TableCreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
-        "ItemCount": int,
-        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
     },
+    total=False,
 )
 
-_RequiredGlobalSecondaryIndexServiceResourceTypeDef = TypedDict(
-    "_RequiredGlobalSecondaryIndexServiceResourceTypeDef",
+class GlobalSecondaryIndexOutputTypeDef(
+    _RequiredGlobalSecondaryIndexOutputTypeDef, _OptionalGlobalSecondaryIndexOutputTypeDef
+):
+    pass
+
+LocalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "LocalSecondaryIndexDescriptionTypeDef",
     {
         "IndexName": str,
-        "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
-        "Projection": ProjectionServiceResourceTypeDef,
-    },
-)
-_OptionalGlobalSecondaryIndexServiceResourceTypeDef = TypedDict(
-    "_OptionalGlobalSecondaryIndexServiceResourceTypeDef",
-    {
-        "ProvisionedThroughput": ProvisionedThroughputServiceResourceTypeDef,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
     },
     total=False,
 )
 
-class GlobalSecondaryIndexServiceResourceTypeDef(
-    _RequiredGlobalSecondaryIndexServiceResourceTypeDef,
-    _OptionalGlobalSecondaryIndexServiceResourceTypeDef,
-):
-    pass
-
-LocalSecondaryIndexServiceResourceTypeDef = TypedDict(
-    "LocalSecondaryIndexServiceResourceTypeDef",
+LocalSecondaryIndexInfoTypeDef = TypedDict(
+    "LocalSecondaryIndexInfoTypeDef",
     {
         "IndexName": str,
-        "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
-        "Projection": ProjectionServiceResourceTypeDef,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionOutputTypeDef,
     },
+    total=False,
 )
 
-GlobalTableTypeDef = TypedDict(
-    "GlobalTableTypeDef",
+GlobalSecondaryIndexDescriptionTypeDef = TypedDict(
+    "GlobalSecondaryIndexDescriptionTypeDef",
     {
-        "GlobalTableName": str,
-        "ReplicationGroup": List[ReplicaOutputTypeDef],
+        "IndexName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "Projection": ProjectionOutputTypeDef,
+        "IndexStatus": IndexStatusType,
+        "Backfilling": bool,
+        "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
+        "IndexSizeBytes": int,
+        "ItemCount": int,
+        "IndexArn": str,
     },
+    total=False,
 )
 
 ImportSummaryTypeDef = TypedDict(
     "ImportSummaryTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
         "TableArn": str,
-        "S3BucketSource": S3BucketSourceOutputTypeDef,
+        "S3BucketSource": S3BucketSourceTypeDef,
         "CloudWatchLogGroupArn": str,
         "InputFormat": InputFormatType,
         "StartTime": datetime,
         "EndTime": datetime,
     },
+    total=False,
 )
 
 ListBackupsInputListBackupsPaginateTypeDef = TypedDict(
     "ListBackupsInputListBackupsPaginateTypeDef",
     {
         "TableName": str,
-        "TimeRangeLowerBound": Union[datetime, str],
-        "TimeRangeUpperBound": Union[datetime, str],
+        "TimeRangeLowerBound": TimestampTypeDef,
+        "TimeRangeUpperBound": TimestampTypeDef,
         "BackupType": BackupTypeFilterType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTablesInputListTablesPaginateTypeDef = TypedDict(
@@ -3518,774 +1791,370 @@
 
 class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(
     _RequiredListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
     _OptionalListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
 ):
     pass
 
-_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryInputQueryPaginateTypeDef",
+UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
+    "UpdateContinuousBackupsInputRequestTypeDef",
     {
         "TableName": str,
+        "PointInTimeRecoverySpecification": PointInTimeRecoverySpecificationTypeDef,
     },
 )
-_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryInputQueryPaginateTypeDef",
+
+UpdateTimeToLiveInputRequestTypeDef = TypedDict(
+    "UpdateTimeToLiveInputRequestTypeDef",
     {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTableTypeDef],
-        "QueryFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "TableName": str,
+        "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
     },
-    total=False,
 )
 
-class QueryInputQueryPaginateTypeDef(
-    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
-):
-    pass
-
-_RequiredScanInputScanPaginateTypeDef = TypedDict(
-    "_RequiredScanInputScanPaginateTypeDef",
+UpdateTimeToLiveOutputTypeDef = TypedDict(
+    "UpdateTimeToLiveOutputTypeDef",
     {
-        "TableName": str,
+        "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalScanInputScanPaginateTypeDef = TypedDict(
-    "_OptionalScanInputScanPaginateTypeDef",
+
+AttributeValueUpdateTypeDef = TypedDict(
+    "AttributeValueUpdateTypeDef",
     {
-        "IndexName": str,
-        "AttributesToGet": Sequence[str],
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTableTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                bytes,
-                bytearray,
-                str,
-                int,
-                Decimal,
-                bool,
-                Set[int],
-                Set[Decimal],
-                Set[str],
-                Set[bytes],
-                Set[bytearray],
-                Sequence[Any],
-                Mapping[str, Any],
-                None,
-            ],
-        ],
-        "ConsistentRead": bool,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Value": UniversalAttributeValueTypeDef,
+        "Action": AttributeActionType,
     },
     total=False,
 )
 
-class ScanInputScanPaginateTypeDef(
-    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
-):
-    pass
-
-ListTagsOfResourceOutputTableTypeDef = TypedDict(
-    "ListTagsOfResourceOutputTableTypeDef",
+_RequiredBatchStatementRequestTypeDef = TypedDict(
+    "_RequiredBatchStatementRequestTypeDef",
     {
-        "Tags": List[TagTableTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Statement": str,
     },
 )
-
-ListTagsOfResourceOutputTypeDef = TypedDict(
-    "ListTagsOfResourceOutputTypeDef",
+_OptionalBatchStatementRequestTypeDef = TypedDict(
+    "_OptionalBatchStatementRequestTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Parameters": Sequence[UniversalAttributeValueTypeDef],
+        "ConsistentRead": bool,
     },
+    total=False,
 )
 
-UpdateContinuousBackupsInputRequestTypeDef = TypedDict(
-    "UpdateContinuousBackupsInputRequestTypeDef",
+class BatchStatementRequestTypeDef(
+    _RequiredBatchStatementRequestTypeDef, _OptionalBatchStatementRequestTypeDef
+):
+    pass
+
+_RequiredConditionCheckTypeDef = TypedDict(
+    "_RequiredConditionCheckTypeDef",
     {
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
         "TableName": str,
-        "PointInTimeRecoverySpecification": PointInTimeRecoverySpecificationTypeDef,
+        "ConditionExpression": str,
     },
 )
-
-ReplicaGlobalSecondaryIndexDescriptionTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTypeDef",
+_OptionalConditionCheckTypeDef = TypedDict(
+    "_OptionalConditionCheckTypeDef",
     {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
+    total=False,
 )
 
-ReplicaGlobalSecondaryIndexDescriptionTableTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexDescriptionTableTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
-    },
-)
+class ConditionCheckTypeDef(_RequiredConditionCheckTypeDef, _OptionalConditionCheckTypeDef):
+    pass
 
-WriteRequestServiceResourceOutputTypeDef = TypedDict(
-    "WriteRequestServiceResourceOutputTypeDef",
+_RequiredConditionTypeDef = TypedDict(
+    "_RequiredConditionTypeDef",
     {
-        "PutRequest": PutRequestServiceResourceOutputTypeDef,
-        "DeleteRequest": DeleteRequestServiceResourceOutputTypeDef,
+        "ComparisonOperator": ComparisonOperatorType,
     },
 )
-
-WriteRequestServiceResourceTypeDef = TypedDict(
-    "WriteRequestServiceResourceTypeDef",
+_OptionalConditionTypeDef = TypedDict(
+    "_OptionalConditionTypeDef",
     {
-        "PutRequest": PutRequestServiceResourceTypeDef,
-        "DeleteRequest": DeleteRequestServiceResourceTypeDef,
+        "AttributeValueList": Sequence[UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-UpdateTimeToLiveOutputTypeDef = TypedDict(
-    "UpdateTimeToLiveOutputTypeDef",
-    {
-        "TimeToLiveSpecification": TimeToLiveSpecificationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class ConditionTypeDef(_RequiredConditionTypeDef, _OptionalConditionTypeDef):
+    pass
 
-UpdateTimeToLiveInputRequestTypeDef = TypedDict(
-    "UpdateTimeToLiveInputRequestTypeDef",
+DeleteRequestTypeDef = TypedDict(
+    "DeleteRequestTypeDef",
     {
-        "TableName": str,
-        "TimeToLiveSpecification": TimeToLiveSpecificationTypeDef,
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
 
-_RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
-    "_RequiredBatchExecuteStatementInputRequestTypeDef",
+_RequiredDeleteTypeDef = TypedDict(
+    "_RequiredDeleteTypeDef",
     {
-        "Statements": Sequence[BatchStatementRequestTypeDef],
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
+        "TableName": str,
     },
 )
-_OptionalBatchExecuteStatementInputRequestTypeDef = TypedDict(
-    "_OptionalBatchExecuteStatementInputRequestTypeDef",
+_OptionalDeleteTypeDef = TypedDict(
+    "_OptionalDeleteTypeDef",
     {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-class BatchExecuteStatementInputRequestTypeDef(
-    _RequiredBatchExecuteStatementInputRequestTypeDef,
-    _OptionalBatchExecuteStatementInputRequestTypeDef,
-):
+class DeleteTypeDef(_RequiredDeleteTypeDef, _OptionalDeleteTypeDef):
     pass
 
-_RequiredQueryInputRequestTypeDef = TypedDict(
-    "_RequiredQueryInputRequestTypeDef",
+_RequiredExecuteStatementInputRequestTypeDef = TypedDict(
+    "_RequiredExecuteStatementInputRequestTypeDef",
     {
-        "TableName": str,
+        "Statement": str,
     },
 )
-_OptionalQueryInputRequestTypeDef = TypedDict(
-    "_OptionalQueryInputRequestTypeDef",
+_OptionalExecuteStatementInputRequestTypeDef = TypedDict(
+    "_OptionalExecuteStatementInputRequestTypeDef",
     {
-        "IndexName": str,
-        "Select": SelectType,
-        "AttributesToGet": Sequence[str],
-        "Limit": int,
+        "Parameters": Sequence[UniversalAttributeValueTypeDef],
         "ConsistentRead": bool,
-        "KeyConditions": Mapping[str, ConditionTypeDef],
-        "QueryFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ScanIndexForward": bool,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "NextToken": str,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ProjectionExpression": str,
-        "FilterExpression": str,
-        "KeyConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "Limit": int,
     },
     total=False,
 )
 
-class QueryInputRequestTypeDef(
-    _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
+class ExecuteStatementInputRequestTypeDef(
+    _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
 ):
     pass
 
-_RequiredScanInputRequestTypeDef = TypedDict(
-    "_RequiredScanInputRequestTypeDef",
+ExpectedAttributeValueTypeDef = TypedDict(
+    "ExpectedAttributeValueTypeDef",
+    {
+        "Value": UniversalAttributeValueTypeDef,
+        "Exists": bool,
+        "ComparisonOperator": ComparisonOperatorType,
+        "AttributeValueList": Sequence[UniversalAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+_RequiredGetItemInputRequestTypeDef = TypedDict(
+    "_RequiredGetItemInputRequestTypeDef",
     {
         "TableName": str,
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
-_OptionalScanInputRequestTypeDef = TypedDict(
-    "_OptionalScanInputRequestTypeDef",
+_OptionalGetItemInputRequestTypeDef = TypedDict(
+    "_OptionalGetItemInputRequestTypeDef",
     {
-        "IndexName": str,
         "AttributesToGet": Sequence[str],
-        "Limit": int,
-        "Select": SelectType,
-        "ScanFilter": Mapping[str, ConditionTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ExclusiveStartKey": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "ConsistentRead": bool,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "TotalSegments": int,
-        "Segment": int,
         "ProjectionExpression": str,
-        "FilterExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
-        "ConsistentRead": bool,
     },
     total=False,
 )
 
-class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
+class GetItemInputRequestTypeDef(
+    _RequiredGetItemInputRequestTypeDef, _OptionalGetItemInputRequestTypeDef
+):
     pass
 
-_RequiredDeleteItemInputRequestTypeDef = TypedDict(
-    "_RequiredDeleteItemInputRequestTypeDef",
+_RequiredGetTypeDef = TypedDict(
+    "_RequiredGetTypeDef",
     {
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
         "TableName": str,
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
     },
 )
-_OptionalDeleteItemInputRequestTypeDef = TypedDict(
-    "_OptionalDeleteItemInputRequestTypeDef",
+_OptionalGetTypeDef = TypedDict(
+    "_OptionalGetTypeDef",
     {
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionExpression": str,
+        "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
     },
     total=False,
 )
 
-class DeleteItemInputRequestTypeDef(
-    _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
-):
+class GetTypeDef(_RequiredGetTypeDef, _OptionalGetTypeDef):
     pass
 
-_RequiredPutItemInputRequestTypeDef = TypedDict(
-    "_RequiredPutItemInputRequestTypeDef",
+_RequiredKeysAndAttributesTypeDef = TypedDict(
+    "_RequiredKeysAndAttributesTypeDef",
     {
-        "TableName": str,
-        "Item": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "Keys": Sequence[Mapping[str, UniversalAttributeValueTypeDef]],
     },
 )
-_OptionalPutItemInputRequestTypeDef = TypedDict(
-    "_OptionalPutItemInputRequestTypeDef",
+_OptionalKeysAndAttributesTypeDef = TypedDict(
+    "_OptionalKeysAndAttributesTypeDef",
     {
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "ConditionalOperator": ConditionalOperatorType,
-        "ConditionExpression": str,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "ProjectionExpression": str,
         "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
     },
     total=False,
 )
 
-class PutItemInputRequestTypeDef(
-    _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
+class KeysAndAttributesTypeDef(
+    _RequiredKeysAndAttributesTypeDef, _OptionalKeysAndAttributesTypeDef
 ):
     pass
 
-_RequiredUpdateItemInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateItemInputRequestTypeDef",
+_RequiredParameterizedStatementTypeDef = TypedDict(
+    "_RequiredParameterizedStatementTypeDef",
     {
-        "TableName": str,
-        "Key": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "Statement": str,
     },
 )
-_OptionalUpdateItemInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateItemInputRequestTypeDef",
+_OptionalParameterizedStatementTypeDef = TypedDict(
+    "_OptionalParameterizedStatementTypeDef",
     {
-        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
-        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
-        "ConditionalOperator": ConditionalOperatorType,
-        "ReturnValues": ReturnValueType,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
-        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
-        "UpdateExpression": str,
-        "ConditionExpression": str,
-        "ExpressionAttributeNames": Mapping[str, str],
-        "ExpressionAttributeValues": Mapping[
-            str,
-            Union[
-                AttributeValueTypeDef,
-                Union[
-                    bytes,
-                    bytearray,
-                    str,
-                    int,
-                    Decimal,
-                    bool,
-                    Set[int],
-                    Set[Decimal],
-                    Set[str],
-                    Set[bytes],
-                    Set[bytearray],
-                    Sequence[Any],
-                    Mapping[str, Any],
-                    None,
-                ],
-            ],
-        ],
+        "Parameters": Sequence[UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-class UpdateItemInputRequestTypeDef(
-    _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
+class ParameterizedStatementTypeDef(
+    _RequiredParameterizedStatementTypeDef, _OptionalParameterizedStatementTypeDef
 ):
     pass
 
-TransactGetItemTypeDef = TypedDict(
-    "TransactGetItemTypeDef",
+PutRequestTypeDef = TypedDict(
+    "PutRequestTypeDef",
     {
-        "Get": GetTypeDef,
+        "Item": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
 
-_RequiredBatchGetItemInputRequestTypeDef = TypedDict(
-    "_RequiredBatchGetItemInputRequestTypeDef",
+_RequiredPutTypeDef = TypedDict(
+    "_RequiredPutTypeDef",
     {
-        "RequestItems": Mapping[str, KeysAndAttributesTypeDef],
+        "Item": Mapping[str, UniversalAttributeValueTypeDef],
+        "TableName": str,
     },
 )
-_OptionalBatchGetItemInputRequestTypeDef = TypedDict(
-    "_OptionalBatchGetItemInputRequestTypeDef",
+_OptionalPutTypeDef = TypedDict(
+    "_OptionalPutTypeDef",
     {
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-class BatchGetItemInputRequestTypeDef(
-    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
-):
+class PutTypeDef(_RequiredPutTypeDef, _OptionalPutTypeDef):
     pass
 
-_RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
-    "_RequiredExecuteTransactionInputRequestTypeDef",
+_RequiredUpdateTypeDef = TypedDict(
+    "_RequiredUpdateTypeDef",
     {
-        "TransactStatements": Sequence[ParameterizedStatementTypeDef],
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
+        "UpdateExpression": str,
+        "TableName": str,
     },
 )
-_OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
-    "_OptionalExecuteTransactionInputRequestTypeDef",
+_OptionalUpdateTypeDef = TypedDict(
+    "_OptionalUpdateTypeDef",
     {
-        "ClientRequestToken": str,
-        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnValuesOnConditionCheckFailure": ReturnValuesOnConditionCheckFailureType,
     },
     total=False,
 )
 
-class ExecuteTransactionInputRequestTypeDef(
-    _RequiredExecuteTransactionInputRequestTypeDef, _OptionalExecuteTransactionInputRequestTypeDef
-):
+class UpdateTypeDef(_RequiredUpdateTypeDef, _OptionalUpdateTypeDef):
     pass
 
-WriteRequestOutputTypeDef = TypedDict(
-    "WriteRequestOutputTypeDef",
-    {
-        "PutRequest": PutRequestOutputTypeDef,
-        "DeleteRequest": DeleteRequestOutputTypeDef,
-    },
-)
-
-WriteRequestTypeDef = TypedDict(
-    "WriteRequestTypeDef",
-    {
-        "PutRequest": PutRequestTypeDef,
-        "DeleteRequest": DeleteRequestTypeDef,
-    },
-    total=False,
-)
-
-TransactWriteItemTypeDef = TypedDict(
-    "TransactWriteItemTypeDef",
-    {
-        "ConditionCheck": ConditionCheckTypeDef,
-        "Put": PutTypeDef,
-        "Delete": DeleteTypeDef,
-        "Update": UpdateTypeDef,
-    },
-    total=False,
-)
-
 AutoScalingSettingsDescriptionTypeDef = TypedDict(
     "AutoScalingSettingsDescriptionTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicies": List[AutoScalingPolicyDescriptionTypeDef],
     },
+    total=False,
 )
 
 AutoScalingSettingsUpdateTypeDef = TypedDict(
     "AutoScalingSettingsUpdateTypeDef",
     {
         "MinimumUnits": int,
         "MaximumUnits": int,
         "AutoScalingDisabled": bool,
         "AutoScalingRoleArn": str,
         "ScalingPolicyUpdate": AutoScalingPolicyUpdateTypeDef,
     },
     total=False,
 )
 
-BatchGetItemOutputServiceResourceTypeDef = TypedDict(
-    "BatchGetItemOutputServiceResourceTypeDef",
-    {
-        "Responses": Dict[str, List[Dict[str, "AttributeValueServiceResourceTypeDef"]]],
-        "UnprocessedKeys": Dict[str, KeysAndAttributesServiceResourceOutputTypeDef],
-        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteItemOutputTableTypeDef = TypedDict(
-    "DeleteItemOutputTableTypeDef",
-    {
-        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetItemOutputTableTypeDef = TypedDict(
-    "GetItemOutputTableTypeDef",
-    {
-        "Item": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutItemOutputTableTypeDef = TypedDict(
-    "PutItemOutputTableTypeDef",
-    {
-        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-QueryOutputTableTypeDef = TypedDict(
-    "QueryOutputTableTypeDef",
-    {
-        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
-        "Count": int,
-        "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ScanOutputTableTypeDef = TypedDict(
-    "ScanOutputTableTypeDef",
-    {
-        "Items": List[Dict[str, "AttributeValueTableTypeDef"]],
-        "Count": int,
-        "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdateItemOutputTableTypeDef = TypedDict(
-    "UpdateItemOutputTableTypeDef",
+WriteRequestOutputTypeDef = TypedDict(
+    "WriteRequestOutputTypeDef",
     {
-        "Attributes": Dict[str, "AttributeValueTableTypeDef"],
-        "ConsumedCapacity": ConsumedCapacityTableTypeDef,
-        "ItemCollectionMetrics": ItemCollectionMetricsTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "PutRequest": PutRequestOutputTypeDef,
+        "DeleteRequest": DeleteRequestOutputTypeDef,
     },
+    total=False,
 )
 
 BatchExecuteStatementOutputTypeDef = TypedDict(
     "BatchExecuteStatementOutputTypeDef",
     {
         "Responses": List[BatchStatementResponseTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetItemOutputTypeDef = TypedDict(
     "BatchGetItemOutputTypeDef",
     {
-        "Responses": Dict[str, List[Dict[str, AttributeValueTypeDef]]],
+        "Responses": Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
         "UnprocessedKeys": Dict[str, KeysAndAttributesOutputTypeDef],
         "ConsumedCapacity": List[ConsumedCapacityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteItemOutputTypeDef = TypedDict(
     "DeleteItemOutputTypeDef",
     {
-        "Attributes": Dict[str, AttributeValueTypeDef],
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteStatementOutputTypeDef = TypedDict(
     "ExecuteStatementOutputTypeDef",
     {
-        "Items": List[Dict[str, AttributeValueTypeDef]],
+        "Items": List[Dict[str, TableAttributeValueTypeDef]],
         "NextToken": str,
         "ConsumedCapacity": ConsumedCapacityTypeDef,
-        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExecuteTransactionOutputTypeDef = TypedDict(
     "ExecuteTransactionOutputTypeDef",
     {
@@ -4294,49 +2163,49 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetItemOutputTypeDef = TypedDict(
     "GetItemOutputTypeDef",
     {
-        "Item": Dict[str, AttributeValueTypeDef],
+        "Item": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutItemOutputTypeDef = TypedDict(
     "PutItemOutputTypeDef",
     {
-        "Attributes": Dict[str, AttributeValueTypeDef],
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryOutputTypeDef = TypedDict(
     "QueryOutputTypeDef",
     {
-        "Items": List[Dict[str, AttributeValueTypeDef]],
+        "Items": List[Dict[str, TableAttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScanOutputTypeDef = TypedDict(
     "ScanOutputTypeDef",
     {
-        "Items": List[Dict[str, AttributeValueTypeDef]],
+        "Items": List[Dict[str, TableAttributeValueTypeDef]],
         "Count": int,
         "ScannedCount": int,
-        "LastEvaluatedKey": Dict[str, AttributeValueTypeDef],
+        "LastEvaluatedKey": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransactGetItemsOutputTypeDef = TypedDict(
     "TransactGetItemsOutputTypeDef",
@@ -4355,15 +2224,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateItemOutputTypeDef = TypedDict(
     "UpdateItemOutputTypeDef",
     {
-        "Attributes": Dict[str, AttributeValueTypeDef],
+        "Attributes": Dict[str, TableAttributeValueTypeDef],
         "ConsumedCapacity": ConsumedCapacityTypeDef,
         "ItemCollectionMetrics": ItemCollectionMetricsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousBackupsOutputTypeDef = TypedDict(
@@ -4378,106 +2247,14 @@
     "UpdateContinuousBackupsOutputTypeDef",
     {
         "ContinuousBackupsDescription": ContinuousBackupsDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GlobalSecondaryIndexUpdateTableTypeDef = TypedDict(
-    "GlobalSecondaryIndexUpdateTableTypeDef",
-    {
-        "Update": UpdateGlobalSecondaryIndexActionTableTypeDef,
-        "Create": CreateGlobalSecondaryIndexActionTableTypeDef,
-        "Delete": DeleteGlobalSecondaryIndexActionTableTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateTableInputRequestTypeDef = TypedDict(
-    "_RequiredCreateTableInputRequestTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "TableName": str,
-        "KeySchema": Sequence[KeySchemaElementTypeDef],
-    },
-)
-_OptionalCreateTableInputRequestTypeDef = TypedDict(
-    "_OptionalCreateTableInputRequestTypeDef",
-    {
-        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
-        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
-class CreateTableInputRequestTypeDef(
-    _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
-):
-    pass
-
-_RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
-    "_RequiredRestoreTableFromBackupInputRequestTypeDef",
-    {
-        "TargetTableName": str,
-        "BackupArn": str,
-    },
-)
-_OptionalRestoreTableFromBackupInputRequestTypeDef = TypedDict(
-    "_OptionalRestoreTableFromBackupInputRequestTypeDef",
-    {
-        "BillingModeOverride": BillingModeType,
-        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexTypeDef],
-        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
-        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
-        "SSESpecificationOverride": SSESpecificationTypeDef,
-    },
-    total=False,
-)
-
-class RestoreTableFromBackupInputRequestTypeDef(
-    _RequiredRestoreTableFromBackupInputRequestTypeDef,
-    _OptionalRestoreTableFromBackupInputRequestTypeDef,
-):
-    pass
-
-_RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
-    {
-        "TargetTableName": str,
-    },
-)
-_OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
-    "_OptionalRestoreTableToPointInTimeInputRequestTypeDef",
-    {
-        "SourceTableArn": str,
-        "SourceTableName": str,
-        "UseLatestRestorableTime": bool,
-        "RestoreDateTime": Union[datetime, str],
-        "BillingModeOverride": BillingModeType,
-        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexTypeDef],
-        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
-        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
-        "SSESpecificationOverride": SSESpecificationTypeDef,
-    },
-    total=False,
-)
-
-class RestoreTableToPointInTimeInputRequestTypeDef(
-    _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
-    _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
-):
-    pass
-
 _RequiredTableCreationParametersTypeDef = TypedDict(
     "_RequiredTableCreationParametersTypeDef",
     {
         "TableName": str,
         "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
         "KeySchema": Sequence[KeySchemaElementTypeDef],
     },
@@ -4504,60 +2281,39 @@
         "Update": UpdateGlobalSecondaryIndexActionTypeDef,
         "Create": CreateGlobalSecondaryIndexActionTypeDef,
         "Delete": DeleteGlobalSecondaryIndexActionTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "_RequiredCreateReplicationGroupMemberActionTableTypeDef",
-    {
-        "RegionName": str,
-    },
-)
-_OptionalCreateReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "_OptionalCreateReplicationGroupMemberActionTableTypeDef",
+ListGlobalTablesOutputTypeDef = TypedDict(
+    "ListGlobalTablesOutputTypeDef",
     {
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-        "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
-        "TableClassOverride": TableClassType,
+        "GlobalTables": List[GlobalTableTypeDef],
+        "LastEvaluatedGlobalTableName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateReplicationGroupMemberActionTableTypeDef(
-    _RequiredCreateReplicationGroupMemberActionTableTypeDef,
-    _OptionalCreateReplicationGroupMemberActionTableTypeDef,
-):
-    pass
-
-_RequiredUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "_RequiredUpdateReplicationGroupMemberActionTableTypeDef",
+ReplicaDescriptionTypeDef = TypedDict(
+    "ReplicaDescriptionTypeDef",
     {
         "RegionName": str,
-    },
-)
-_OptionalUpdateReplicationGroupMemberActionTableTypeDef = TypedDict(
-    "_OptionalUpdateReplicationGroupMemberActionTableTypeDef",
-    {
+        "ReplicaStatus": ReplicaStatusType,
+        "ReplicaStatusDescription": str,
+        "ReplicaStatusPercentProgress": str,
         "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableTypeDef,
-        "GlobalSecondaryIndexes": Sequence[ReplicaGlobalSecondaryIndexTableTypeDef],
-        "TableClassOverride": TableClassType,
+        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTypeDef,
+        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
+        "ReplicaInaccessibleDateTime": datetime,
+        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
     total=False,
 )
 
-class UpdateReplicationGroupMemberActionTableTypeDef(
-    _RequiredUpdateReplicationGroupMemberActionTableTypeDef,
-    _OptionalUpdateReplicationGroupMemberActionTableTypeDef,
-):
-    pass
-
 _RequiredCreateReplicationGroupMemberActionTypeDef = TypedDict(
     "_RequiredCreateReplicationGroupMemberActionTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalCreateReplicationGroupMemberActionTypeDef = TypedDict(
@@ -4596,247 +2352,512 @@
 
 class UpdateReplicationGroupMemberActionTypeDef(
     _RequiredUpdateReplicationGroupMemberActionTypeDef,
     _OptionalUpdateReplicationGroupMemberActionTypeDef,
 ):
     pass
 
+InputFormatOptionsUnionTypeDef = Union[InputFormatOptionsTypeDef, InputFormatOptionsOutputTypeDef]
 UpdateGlobalTableInputRequestTypeDef = TypedDict(
     "UpdateGlobalTableInputRequestTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaUpdates": Sequence[ReplicaUpdateTypeDef],
     },
 )
 
+GlobalSecondaryIndexUnionTypeDef = Union[
+    GlobalSecondaryIndexTypeDef, GlobalSecondaryIndexOutputTypeDef
+]
+_RequiredTableCreationParametersOutputTypeDef = TypedDict(
+    "_RequiredTableCreationParametersOutputTypeDef",
+    {
+        "TableName": str,
+        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "KeySchema": List[KeySchemaElementTypeDef],
+    },
+)
+_OptionalTableCreationParametersOutputTypeDef = TypedDict(
+    "_OptionalTableCreationParametersOutputTypeDef",
+    {
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
+    },
+    total=False,
+)
+
+class TableCreationParametersOutputTypeDef(
+    _RequiredTableCreationParametersOutputTypeDef, _OptionalTableCreationParametersOutputTypeDef
+):
+    pass
+
 SourceTableFeatureDetailsTypeDef = TypedDict(
     "SourceTableFeatureDetailsTypeDef",
     {
         "LocalSecondaryIndexes": List[LocalSecondaryIndexInfoTypeDef],
         "GlobalSecondaryIndexes": List[GlobalSecondaryIndexInfoTypeDef],
-        "StreamDescription": StreamSpecificationOutputTypeDef,
+        "StreamDescription": StreamSpecificationTypeDef,
         "TimeToLiveDescription": TimeToLiveDescriptionTypeDef,
         "SSEDescription": SSEDescriptionTypeDef,
     },
+    total=False,
 )
 
-TableCreationParametersOutputTypeDef = TypedDict(
-    "TableCreationParametersOutputTypeDef",
+ListImportsOutputTypeDef = TypedDict(
+    "ListImportsOutputTypeDef",
+    {
+        "ImportSummaryList": List[ImportSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
+    "_RequiredBatchExecuteStatementInputRequestTypeDef",
+    {
+        "Statements": Sequence[BatchStatementRequestTypeDef],
+    },
+)
+_OptionalBatchExecuteStatementInputRequestTypeDef = TypedDict(
+    "_OptionalBatchExecuteStatementInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+    },
+    total=False,
+)
+
+class BatchExecuteStatementInputRequestTypeDef(
+    _RequiredBatchExecuteStatementInputRequestTypeDef,
+    _OptionalBatchExecuteStatementInputRequestTypeDef,
+):
+    pass
+
+_RequiredQueryInputQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryInputQueryPaginateTypeDef",
     {
         "TableName": str,
-        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputOutputTypeDef,
-        "SSESpecification": SSESpecificationOutputTypeDef,
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexOutputTypeDef],
     },
 )
+_OptionalQueryInputQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryInputQueryPaginateTypeDef",
+    {
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTypeDef],
+        "QueryFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-_RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
-    "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
+class QueryInputQueryPaginateTypeDef(
+    _RequiredQueryInputQueryPaginateTypeDef, _OptionalQueryInputQueryPaginateTypeDef
+):
+    pass
+
+_RequiredQueryInputRequestTypeDef = TypedDict(
+    "_RequiredQueryInputRequestTypeDef",
     {
-        "AttributeDefinitions": Sequence[AttributeDefinitionServiceResourceTypeDef],
         "TableName": str,
-        "KeySchema": Sequence[KeySchemaElementServiceResourceTypeDef],
     },
 )
-_OptionalCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
-    "_OptionalCreateTableInputServiceResourceCreateTableTypeDef",
+_OptionalQueryInputRequestTypeDef = TypedDict(
+    "_OptionalQueryInputRequestTypeDef",
     {
-        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexServiceResourceTypeDef],
-        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexServiceResourceTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputServiceResourceTypeDef,
-        "StreamSpecification": StreamSpecificationServiceResourceTypeDef,
-        "SSESpecification": SSESpecificationServiceResourceTypeDef,
-        "Tags": Sequence[TagServiceResourceTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTypeDef],
+        "QueryFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ExclusiveStartKey": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "KeyConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-class CreateTableInputServiceResourceCreateTableTypeDef(
-    _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
-    _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
+class QueryInputRequestTypeDef(
+    _RequiredQueryInputRequestTypeDef, _OptionalQueryInputRequestTypeDef
 ):
     pass
 
-ListGlobalTablesOutputTypeDef = TypedDict(
-    "ListGlobalTablesOutputTypeDef",
+QueryInputTableQueryTypeDef = TypedDict(
+    "QueryInputTableQueryTypeDef",
     {
-        "GlobalTables": List[GlobalTableTypeDef],
-        "LastEvaluatedGlobalTableName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "IndexName": str,
+        "Select": SelectType,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "ConsistentRead": bool,
+        "KeyConditions": Mapping[str, ConditionTypeDef],
+        "QueryFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ScanIndexForward": bool,
+        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ProjectionExpression": str,
+        "FilterExpression": ConditionBaseImportTypeDef,
+        "KeyConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
     },
+    total=False,
 )
 
-ListImportsOutputTypeDef = TypedDict(
-    "ListImportsOutputTypeDef",
+_RequiredScanInputRequestTypeDef = TypedDict(
+    "_RequiredScanInputRequestTypeDef",
     {
-        "ImportSummaryList": List[ImportSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TableName": str,
+    },
+)
+_OptionalScanInputRequestTypeDef = TypedDict(
+    "_OptionalScanInputRequestTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ExclusiveStartKey": Mapping[str, UniversalAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+        "ConsistentRead": bool,
     },
+    total=False,
 )
 
-ReplicaDescriptionTypeDef = TypedDict(
-    "ReplicaDescriptionTypeDef",
+class ScanInputRequestTypeDef(_RequiredScanInputRequestTypeDef, _OptionalScanInputRequestTypeDef):
+    pass
+
+_RequiredScanInputScanPaginateTypeDef = TypedDict(
+    "_RequiredScanInputScanPaginateTypeDef",
     {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideOutputTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTypeDef,
+        "TableName": str,
+    },
+)
+_OptionalScanInputScanPaginateTypeDef = TypedDict(
+    "_OptionalScanInputScanPaginateTypeDef",
+    {
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ReplicaDescriptionTableTypeDef = TypedDict(
-    "ReplicaDescriptionTableTypeDef",
+class ScanInputScanPaginateTypeDef(
+    _RequiredScanInputScanPaginateTypeDef, _OptionalScanInputScanPaginateTypeDef
+):
+    pass
+
+ScanInputTableScanTypeDef = TypedDict(
+    "ScanInputTableScanTypeDef",
     {
-        "RegionName": str,
-        "ReplicaStatus": ReplicaStatusType,
-        "ReplicaStatusDescription": str,
-        "ReplicaStatusPercentProgress": str,
-        "KMSMasterKeyId": str,
-        "ProvisionedThroughputOverride": ProvisionedThroughputOverrideTableOutputTypeDef,
-        "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexDescriptionTableTypeDef],
-        "ReplicaInaccessibleDateTime": datetime,
-        "ReplicaTableClassSummary": TableClassSummaryTableTypeDef,
+        "IndexName": str,
+        "AttributesToGet": Sequence[str],
+        "Limit": int,
+        "Select": SelectType,
+        "ScanFilter": Mapping[str, ConditionTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ExclusiveStartKey": Mapping[str, TableAttributeValueTypeDef],
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "TotalSegments": int,
+        "Segment": int,
+        "ProjectionExpression": str,
+        "FilterExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+        "ConsistentRead": bool,
     },
+    total=False,
 )
 
-BatchWriteItemOutputServiceResourceTypeDef = TypedDict(
-    "BatchWriteItemOutputServiceResourceTypeDef",
+_RequiredDeleteItemInputRequestTypeDef = TypedDict(
+    "_RequiredDeleteItemInputRequestTypeDef",
     {
-        "UnprocessedItems": Dict[str, List[WriteRequestServiceResourceOutputTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityServiceResourceTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "TableName": str,
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
+_OptionalDeleteItemInputRequestTypeDef = TypedDict(
+    "_OptionalDeleteItemInputRequestTypeDef",
+    {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
+    },
+    total=False,
+)
 
-_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
-    "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+class DeleteItemInputRequestTypeDef(
+    _RequiredDeleteItemInputRequestTypeDef, _OptionalDeleteItemInputRequestTypeDef
+):
+    pass
+
+_RequiredDeleteItemInputTableDeleteItemTypeDef = TypedDict(
+    "_RequiredDeleteItemInputTableDeleteItemTypeDef",
     {
-        "RequestItems": Mapping[str, Sequence[WriteRequestServiceResourceTypeDef]],
+        "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
-_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
-    "_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+_OptionalDeleteItemInputTableDeleteItemTypeDef = TypedDict(
+    "_OptionalDeleteItemInputTableDeleteItemTypeDef",
     {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
     },
     total=False,
 )
 
-class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
-    _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-    _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+class DeleteItemInputTableDeleteItemTypeDef(
+    _RequiredDeleteItemInputTableDeleteItemTypeDef, _OptionalDeleteItemInputTableDeleteItemTypeDef
 ):
     pass
 
-_RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
-    "_RequiredTransactGetItemsInputRequestTypeDef",
+_RequiredPutItemInputRequestTypeDef = TypedDict(
+    "_RequiredPutItemInputRequestTypeDef",
     {
-        "TransactItems": Sequence[TransactGetItemTypeDef],
+        "TableName": str,
+        "Item": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
-_OptionalTransactGetItemsInputRequestTypeDef = TypedDict(
-    "_OptionalTransactGetItemsInputRequestTypeDef",
+_OptionalPutItemInputRequestTypeDef = TypedDict(
+    "_OptionalPutItemInputRequestTypeDef",
     {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionalOperator": ConditionalOperatorType,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-class TransactGetItemsInputRequestTypeDef(
-    _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
+class PutItemInputRequestTypeDef(
+    _RequiredPutItemInputRequestTypeDef, _OptionalPutItemInputRequestTypeDef
 ):
     pass
 
-BatchWriteItemOutputTypeDef = TypedDict(
-    "BatchWriteItemOutputTypeDef",
+_RequiredPutItemInputTablePutItemTypeDef = TypedDict(
+    "_RequiredPutItemInputTablePutItemTypeDef",
     {
-        "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
-        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
-        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Item": Mapping[str, TableAttributeValueTypeDef],
     },
 )
+_OptionalPutItemInputTablePutItemTypeDef = TypedDict(
+    "_OptionalPutItemInputTablePutItemTypeDef",
+    {
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ReturnValues": ReturnValueType,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ConditionalOperator": ConditionalOperatorType,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
 
-_RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
-    "_RequiredBatchWriteItemInputRequestTypeDef",
+class PutItemInputTablePutItemTypeDef(
+    _RequiredPutItemInputTablePutItemTypeDef, _OptionalPutItemInputTablePutItemTypeDef
+):
+    pass
+
+_RequiredUpdateItemInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateItemInputRequestTypeDef",
     {
-        "RequestItems": Mapping[str, Sequence[WriteRequestTypeDef]],
+        "TableName": str,
+        "Key": Mapping[str, UniversalAttributeValueTypeDef],
     },
 )
-_OptionalBatchWriteItemInputRequestTypeDef = TypedDict(
-    "_OptionalBatchWriteItemInputRequestTypeDef",
+_OptionalUpdateItemInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateItemInputRequestTypeDef",
     {
+        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "UpdateExpression": str,
+        "ConditionExpression": str,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, UniversalAttributeValueTypeDef],
     },
     total=False,
 )
 
-class BatchWriteItemInputRequestTypeDef(
-    _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
+class UpdateItemInputRequestTypeDef(
+    _RequiredUpdateItemInputRequestTypeDef, _OptionalUpdateItemInputRequestTypeDef
 ):
     pass
 
-_RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
-    "_RequiredTransactWriteItemsInputRequestTypeDef",
+_RequiredUpdateItemInputTableUpdateItemTypeDef = TypedDict(
+    "_RequiredUpdateItemInputTableUpdateItemTypeDef",
     {
-        "TransactItems": Sequence[TransactWriteItemTypeDef],
+        "Key": Mapping[str, TableAttributeValueTypeDef],
     },
 )
-_OptionalTransactWriteItemsInputRequestTypeDef = TypedDict(
-    "_OptionalTransactWriteItemsInputRequestTypeDef",
+_OptionalUpdateItemInputTableUpdateItemTypeDef = TypedDict(
+    "_OptionalUpdateItemInputTableUpdateItemTypeDef",
     {
+        "AttributeUpdates": Mapping[str, AttributeValueUpdateTypeDef],
+        "Expected": Mapping[str, ExpectedAttributeValueTypeDef],
+        "ConditionalOperator": ConditionalOperatorType,
+        "ReturnValues": ReturnValueType,
         "ReturnConsumedCapacity": ReturnConsumedCapacityType,
         "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "UpdateExpression": str,
+        "ConditionExpression": ConditionBaseImportTypeDef,
+        "ExpressionAttributeNames": Mapping[str, str],
+        "ExpressionAttributeValues": Mapping[str, TableAttributeValueTypeDef],
+    },
+    total=False,
+)
+
+class UpdateItemInputTableUpdateItemTypeDef(
+    _RequiredUpdateItemInputTableUpdateItemTypeDef, _OptionalUpdateItemInputTableUpdateItemTypeDef
+):
+    pass
+
+TransactGetItemTypeDef = TypedDict(
+    "TransactGetItemTypeDef",
+    {
+        "Get": GetTypeDef,
+    },
+)
+
+KeysAndAttributesUnionTypeDef = Union[KeysAndAttributesTypeDef, KeysAndAttributesOutputTypeDef]
+_RequiredExecuteTransactionInputRequestTypeDef = TypedDict(
+    "_RequiredExecuteTransactionInputRequestTypeDef",
+    {
+        "TransactStatements": Sequence[ParameterizedStatementTypeDef],
+    },
+)
+_OptionalExecuteTransactionInputRequestTypeDef = TypedDict(
+    "_OptionalExecuteTransactionInputRequestTypeDef",
+    {
         "ClientRequestToken": str,
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
     total=False,
 )
 
-class TransactWriteItemsInputRequestTypeDef(
-    _RequiredTransactWriteItemsInputRequestTypeDef, _OptionalTransactWriteItemsInputRequestTypeDef
+class ExecuteTransactionInputRequestTypeDef(
+    _RequiredExecuteTransactionInputRequestTypeDef, _OptionalExecuteTransactionInputRequestTypeDef
 ):
     pass
 
+WriteRequestTypeDef = TypedDict(
+    "WriteRequestTypeDef",
+    {
+        "PutRequest": PutRequestTypeDef,
+        "DeleteRequest": DeleteRequestTypeDef,
+    },
+    total=False,
+)
+
+TransactWriteItemTypeDef = TypedDict(
+    "TransactWriteItemTypeDef",
+    {
+        "ConditionCheck": ConditionCheckTypeDef,
+        "Put": PutTypeDef,
+        "Delete": DeleteTypeDef,
+        "Update": UpdateTypeDef,
+    },
+    total=False,
+)
+
 ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef",
     {
         "IndexName": str,
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
+    total=False,
 )
 
-ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
-    "ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
+_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
+    "_RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
     {
         "IndexName": str,
+    },
+)
+_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef = TypedDict(
+    "_OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef",
+    {
         "IndexStatus": IndexStatusType,
         "ProvisionedReadCapacityUnits": int,
         "ProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ProvisionedWriteCapacityUnits": int,
         "ProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
     },
+    total=False,
 )
 
+class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(
+    _RequiredReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
+    _OptionalReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
+):
+    pass
+
 GlobalSecondaryIndexAutoScalingUpdateTypeDef = TypedDict(
     "GlobalSecondaryIndexAutoScalingUpdateTypeDef",
     {
         "IndexName": str,
         "ProvisionedWriteCapacityAutoScalingUpdate": AutoScalingSettingsUpdateTypeDef,
     },
     total=False,
@@ -4889,14 +2910,24 @@
 
 class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(
     _RequiredReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
     _OptionalReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
 ):
     pass
 
+BatchWriteItemOutputTypeDef = TypedDict(
+    "BatchWriteItemOutputTypeDef",
+    {
+        "UnprocessedItems": Dict[str, List[WriteRequestOutputTypeDef]],
+        "ItemCollectionMetrics": Dict[str, List[ItemCollectionMetricsTypeDef]],
+        "ConsumedCapacity": List[ConsumedCapacityTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredImportTableInputRequestTypeDef = TypedDict(
     "_RequiredImportTableInputRequestTypeDef",
     {
         "S3BucketSource": S3BucketSourceTypeDef,
         "InputFormat": InputFormatType,
         "TableCreationParameters": TableCreationParametersTypeDef,
     },
@@ -4912,165 +2943,337 @@
 )
 
 class ImportTableInputRequestTypeDef(
     _RequiredImportTableInputRequestTypeDef, _OptionalImportTableInputRequestTypeDef
 ):
     pass
 
-ReplicationGroupUpdateTableTypeDef = TypedDict(
-    "ReplicationGroupUpdateTableTypeDef",
+GlobalTableDescriptionTypeDef = TypedDict(
+    "GlobalTableDescriptionTypeDef",
     {
-        "Create": CreateReplicationGroupMemberActionTableTypeDef,
-        "Update": UpdateReplicationGroupMemberActionTableTypeDef,
-        "Delete": DeleteReplicationGroupMemberActionTableTypeDef,
+        "ReplicationGroup": List[ReplicaDescriptionTypeDef],
+        "GlobalTableArn": str,
+        "CreationDateTime": datetime,
+        "GlobalTableStatus": GlobalTableStatusType,
+        "GlobalTableName": str,
+    },
+    total=False,
+)
+
+TableDescriptionTypeDef = TypedDict(
+    "TableDescriptionTypeDef",
+    {
+        "AttributeDefinitions": List[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": List[KeySchemaElementTypeDef],
+        "TableStatus": TableStatusType,
+        "CreationDateTime": datetime,
+        "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
+        "TableSizeBytes": int,
+        "ItemCount": int,
+        "TableArn": str,
+        "TableId": str,
+        "BillingModeSummary": BillingModeSummaryTypeDef,
+        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTypeDef],
+        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "LatestStreamLabel": str,
+        "LatestStreamArn": str,
+        "GlobalTableVersion": str,
+        "Replicas": List[ReplicaDescriptionTypeDef],
+        "RestoreSummary": RestoreSummaryTypeDef,
+        "SSEDescription": SSEDescriptionTypeDef,
+        "ArchivalSummary": ArchivalSummaryTypeDef,
+        "TableClassSummary": TableClassSummaryTypeDef,
+        "DeletionProtectionEnabled": bool,
     },
     total=False,
 )
 
 ReplicationGroupUpdateTypeDef = TypedDict(
     "ReplicationGroupUpdateTypeDef",
     {
         "Create": CreateReplicationGroupMemberActionTypeDef,
         "Update": UpdateReplicationGroupMemberActionTypeDef,
         "Delete": DeleteReplicationGroupMemberActionTypeDef,
     },
     total=False,
 )
 
-BackupDescriptionTypeDef = TypedDict(
-    "BackupDescriptionTypeDef",
+_RequiredCreateTableInputRequestTypeDef = TypedDict(
+    "_RequiredCreateTableInputRequestTypeDef",
     {
-        "BackupDetails": BackupDetailsTypeDef,
-        "SourceTableDetails": SourceTableDetailsTypeDef,
-        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+    },
+)
+_OptionalCreateTableInputRequestTypeDef = TypedDict(
+    "_OptionalCreateTableInputRequestTypeDef",
+    {
+        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexUnionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+class CreateTableInputRequestTypeDef(
+    _RequiredCreateTableInputRequestTypeDef, _OptionalCreateTableInputRequestTypeDef
+):
+    pass
+
+_RequiredCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
+    "_RequiredCreateTableInputServiceResourceCreateTableTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "TableName": str,
+        "KeySchema": Sequence[KeySchemaElementTypeDef],
+    },
+)
+_OptionalCreateTableInputServiceResourceCreateTableTypeDef = TypedDict(
+    "_OptionalCreateTableInputServiceResourceCreateTableTypeDef",
+    {
+        "LocalSecondaryIndexes": Sequence[LocalSecondaryIndexTypeDef],
+        "GlobalSecondaryIndexes": Sequence[GlobalSecondaryIndexUnionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+class CreateTableInputServiceResourceCreateTableTypeDef(
+    _RequiredCreateTableInputServiceResourceCreateTableTypeDef,
+    _OptionalCreateTableInputServiceResourceCreateTableTypeDef,
+):
+    pass
+
+_RequiredRestoreTableFromBackupInputRequestTypeDef = TypedDict(
+    "_RequiredRestoreTableFromBackupInputRequestTypeDef",
+    {
+        "TargetTableName": str,
+        "BackupArn": str,
+    },
+)
+_OptionalRestoreTableFromBackupInputRequestTypeDef = TypedDict(
+    "_OptionalRestoreTableFromBackupInputRequestTypeDef",
+    {
+        "BillingModeOverride": BillingModeType,
+        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexUnionTypeDef],
+        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
+        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
+        "SSESpecificationOverride": SSESpecificationTypeDef,
+    },
+    total=False,
+)
+
+class RestoreTableFromBackupInputRequestTypeDef(
+    _RequiredRestoreTableFromBackupInputRequestTypeDef,
+    _OptionalRestoreTableFromBackupInputRequestTypeDef,
+):
+    pass
+
+_RequiredRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_RequiredRestoreTableToPointInTimeInputRequestTypeDef",
+    {
+        "TargetTableName": str,
+    },
+)
+_OptionalRestoreTableToPointInTimeInputRequestTypeDef = TypedDict(
+    "_OptionalRestoreTableToPointInTimeInputRequestTypeDef",
+    {
+        "SourceTableArn": str,
+        "SourceTableName": str,
+        "UseLatestRestorableTime": bool,
+        "RestoreDateTime": TimestampTypeDef,
+        "BillingModeOverride": BillingModeType,
+        "GlobalSecondaryIndexOverride": Sequence[GlobalSecondaryIndexUnionTypeDef],
+        "LocalSecondaryIndexOverride": Sequence[LocalSecondaryIndexTypeDef],
+        "ProvisionedThroughputOverride": ProvisionedThroughputTypeDef,
+        "SSESpecificationOverride": SSESpecificationTypeDef,
     },
+    total=False,
 )
 
+class RestoreTableToPointInTimeInputRequestTypeDef(
+    _RequiredRestoreTableToPointInTimeInputRequestTypeDef,
+    _OptionalRestoreTableToPointInTimeInputRequestTypeDef,
+):
+    pass
+
 ImportTableDescriptionTypeDef = TypedDict(
     "ImportTableDescriptionTypeDef",
     {
         "ImportArn": str,
         "ImportStatus": ImportStatusType,
         "TableArn": str,
         "TableId": str,
         "ClientToken": str,
-        "S3BucketSource": S3BucketSourceOutputTypeDef,
+        "S3BucketSource": S3BucketSourceTypeDef,
         "ErrorCount": int,
         "CloudWatchLogGroupArn": str,
         "InputFormat": InputFormatType,
         "InputFormatOptions": InputFormatOptionsOutputTypeDef,
         "InputCompressionType": InputCompressionTypeType,
         "TableCreationParameters": TableCreationParametersOutputTypeDef,
         "StartTime": datetime,
         "EndTime": datetime,
         "ProcessedSizeBytes": int,
         "ProcessedItemCount": int,
         "ImportedItemCount": int,
         "FailureCode": str,
         "FailureMessage": str,
     },
+    total=False,
 )
 
-GlobalTableDescriptionTypeDef = TypedDict(
-    "GlobalTableDescriptionTypeDef",
+TableCreationParametersUnionTypeDef = Union[
+    TableCreationParametersTypeDef, TableCreationParametersOutputTypeDef
+]
+BackupDescriptionTypeDef = TypedDict(
+    "BackupDescriptionTypeDef",
     {
-        "ReplicationGroup": List[ReplicaDescriptionTypeDef],
-        "GlobalTableArn": str,
-        "CreationDateTime": datetime,
-        "GlobalTableStatus": GlobalTableStatusType,
-        "GlobalTableName": str,
+        "BackupDetails": BackupDetailsTypeDef,
+        "SourceTableDetails": SourceTableDetailsTypeDef,
+        "SourceTableFeatureDetails": SourceTableFeatureDetailsTypeDef,
     },
+    total=False,
 )
 
-TableDescriptionTypeDef = TypedDict(
-    "TableDescriptionTypeDef",
+_RequiredTransactGetItemsInputRequestTypeDef = TypedDict(
+    "_RequiredTransactGetItemsInputRequestTypeDef",
     {
-        "AttributeDefinitions": List[AttributeDefinitionOutputTypeDef],
-        "TableName": str,
-        "KeySchema": List[KeySchemaElementOutputTypeDef],
-        "TableStatus": TableStatusType,
-        "CreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTypeDef,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "TableArn": str,
-        "TableId": str,
-        "BillingModeSummary": BillingModeSummaryTypeDef,
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTypeDef],
-        "StreamSpecification": StreamSpecificationOutputTypeDef,
-        "LatestStreamLabel": str,
-        "LatestStreamArn": str,
-        "GlobalTableVersion": str,
-        "Replicas": List[ReplicaDescriptionTypeDef],
-        "RestoreSummary": RestoreSummaryTypeDef,
-        "SSEDescription": SSEDescriptionTypeDef,
-        "ArchivalSummary": ArchivalSummaryTypeDef,
-        "TableClassSummary": TableClassSummaryTypeDef,
-        "DeletionProtectionEnabled": bool,
+        "TransactItems": Sequence[TransactGetItemTypeDef],
+    },
+)
+_OptionalTransactGetItemsInputRequestTypeDef = TypedDict(
+    "_OptionalTransactGetItemsInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
     },
+    total=False,
 )
 
-TableDescriptionTableTypeDef = TypedDict(
-    "TableDescriptionTableTypeDef",
+class TransactGetItemsInputRequestTypeDef(
+    _RequiredTransactGetItemsInputRequestTypeDef, _OptionalTransactGetItemsInputRequestTypeDef
+):
+    pass
+
+_RequiredBatchGetItemInputRequestTypeDef = TypedDict(
+    "_RequiredBatchGetItemInputRequestTypeDef",
     {
-        "AttributeDefinitions": List[AttributeDefinitionTableOutputTypeDef],
-        "TableName": str,
-        "KeySchema": List[KeySchemaElementTableOutputTypeDef],
-        "TableStatus": TableStatusType,
-        "CreationDateTime": datetime,
-        "ProvisionedThroughput": ProvisionedThroughputDescriptionTableTypeDef,
-        "TableSizeBytes": int,
-        "ItemCount": int,
-        "TableArn": str,
-        "TableId": str,
-        "BillingModeSummary": BillingModeSummaryTableTypeDef,
-        "LocalSecondaryIndexes": List[LocalSecondaryIndexDescriptionTableTypeDef],
-        "GlobalSecondaryIndexes": List[GlobalSecondaryIndexDescriptionTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableOutputTypeDef,
-        "LatestStreamLabel": str,
-        "LatestStreamArn": str,
-        "GlobalTableVersion": str,
-        "Replicas": List[ReplicaDescriptionTableTypeDef],
-        "RestoreSummary": RestoreSummaryTableTypeDef,
-        "SSEDescription": SSEDescriptionTableTypeDef,
-        "ArchivalSummary": ArchivalSummaryTableTypeDef,
-        "TableClassSummary": TableClassSummaryTableTypeDef,
-        "DeletionProtectionEnabled": bool,
+        "RequestItems": Mapping[str, KeysAndAttributesUnionTypeDef],
+    },
+)
+_OptionalBatchGetItemInputRequestTypeDef = TypedDict(
+    "_OptionalBatchGetItemInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+    },
+    total=False,
+)
+
+class BatchGetItemInputRequestTypeDef(
+    _RequiredBatchGetItemInputRequestTypeDef, _OptionalBatchGetItemInputRequestTypeDef
+):
+    pass
+
+_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
+    "_RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    {
+        "RequestItems": Mapping[str, KeysAndAttributesUnionTypeDef],
+    },
+)
+_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef = TypedDict(
+    "_OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+    },
+    total=False,
+)
+
+class BatchGetItemInputServiceResourceBatchGetItemTypeDef(
+    _RequiredBatchGetItemInputServiceResourceBatchGetItemTypeDef,
+    _OptionalBatchGetItemInputServiceResourceBatchGetItemTypeDef,
+):
+    pass
+
+WriteRequestUnionTypeDef = Union[WriteRequestTypeDef, WriteRequestOutputTypeDef]
+_RequiredTransactWriteItemsInputRequestTypeDef = TypedDict(
+    "_RequiredTransactWriteItemsInputRequestTypeDef",
+    {
+        "TransactItems": Sequence[TransactWriteItemTypeDef],
+    },
+)
+_OptionalTransactWriteItemsInputRequestTypeDef = TypedDict(
+    "_OptionalTransactWriteItemsInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+        "ClientRequestToken": str,
     },
+    total=False,
 )
 
+class TransactWriteItemsInputRequestTypeDef(
+    _RequiredTransactWriteItemsInputRequestTypeDef, _OptionalTransactWriteItemsInputRequestTypeDef
+):
+    pass
+
 ReplicaAutoScalingDescriptionTypeDef = TypedDict(
     "ReplicaAutoScalingDescriptionTypeDef",
     {
         "RegionName": str,
         "GlobalSecondaryIndexes": List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef],
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaStatus": ReplicaStatusType,
     },
+    total=False,
 )
 
-ReplicaSettingsDescriptionTypeDef = TypedDict(
-    "ReplicaSettingsDescriptionTypeDef",
+_RequiredReplicaSettingsDescriptionTypeDef = TypedDict(
+    "_RequiredReplicaSettingsDescriptionTypeDef",
     {
         "RegionName": str,
+    },
+)
+_OptionalReplicaSettingsDescriptionTypeDef = TypedDict(
+    "_OptionalReplicaSettingsDescriptionTypeDef",
+    {
         "ReplicaStatus": ReplicaStatusType,
         "ReplicaBillingModeSummary": BillingModeSummaryTypeDef,
         "ReplicaProvisionedReadCapacityUnits": int,
         "ReplicaProvisionedReadCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaProvisionedWriteCapacityUnits": int,
         "ReplicaProvisionedWriteCapacityAutoScalingSettings": AutoScalingSettingsDescriptionTypeDef,
         "ReplicaGlobalSecondaryIndexSettings": List[
             ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef
         ],
         "ReplicaTableClassSummary": TableClassSummaryTypeDef,
     },
+    total=False,
 )
 
+class ReplicaSettingsDescriptionTypeDef(
+    _RequiredReplicaSettingsDescriptionTypeDef, _OptionalReplicaSettingsDescriptionTypeDef
+):
+    pass
+
 _RequiredReplicaAutoScalingUpdateTypeDef = TypedDict(
     "_RequiredReplicaAutoScalingUpdateTypeDef",
     {
         "RegionName": str,
     },
 )
 _OptionalReplicaAutoScalingUpdateTypeDef = TypedDict(
@@ -5109,89 +3312,14 @@
 )
 
 class ReplicaSettingsUpdateTypeDef(
     _RequiredReplicaSettingsUpdateTypeDef, _OptionalReplicaSettingsUpdateTypeDef
 ):
     pass
 
-UpdateTableInputTableUpdateTypeDef = TypedDict(
-    "UpdateTableInputTableUpdateTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTableTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTableTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTableTypeDef],
-        "StreamSpecification": StreamSpecificationTableTypeDef,
-        "SSESpecification": SSESpecificationTableTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTableTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
-_RequiredUpdateTableInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateTableInputRequestTypeDef",
-    {
-        "TableName": str,
-    },
-)
-_OptionalUpdateTableInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateTableInputRequestTypeDef",
-    {
-        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
-        "BillingMode": BillingModeType,
-        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
-        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
-        "StreamSpecification": StreamSpecificationTypeDef,
-        "SSESpecification": SSESpecificationTypeDef,
-        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
-        "TableClass": TableClassType,
-        "DeletionProtectionEnabled": bool,
-    },
-    total=False,
-)
-
-class UpdateTableInputRequestTypeDef(
-    _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
-):
-    pass
-
-DeleteBackupOutputTypeDef = TypedDict(
-    "DeleteBackupOutputTypeDef",
-    {
-        "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBackupOutputTypeDef = TypedDict(
-    "DescribeBackupOutputTypeDef",
-    {
-        "BackupDescription": BackupDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeImportOutputTypeDef = TypedDict(
-    "DescribeImportOutputTypeDef",
-    {
-        "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ImportTableOutputTypeDef = TypedDict(
-    "ImportTableOutputTypeDef",
-    {
-        "ImportTableDescription": ImportTableDescriptionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateGlobalTableOutputTypeDef = TypedDict(
     "CreateGlobalTableOutputTypeDef",
     {
         "GlobalTableDescription": GlobalTableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5256,29 +3384,138 @@
     "UpdateTableOutputTypeDef",
     {
         "TableDescription": TableDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteTableOutputTableTypeDef = TypedDict(
-    "DeleteTableOutputTableTypeDef",
+_RequiredUpdateTableInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateTableInputRequestTypeDef",
+    {
+        "TableName": str,
+    },
+)
+_OptionalUpdateTableInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateTableInputRequestTypeDef",
+    {
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+class UpdateTableInputRequestTypeDef(
+    _RequiredUpdateTableInputRequestTypeDef, _OptionalUpdateTableInputRequestTypeDef
+):
+    pass
+
+UpdateTableInputTableUpdateTypeDef = TypedDict(
+    "UpdateTableInputTableUpdateTypeDef",
     {
-        "TableDescription": TableDescriptionTableTypeDef,
+        "AttributeDefinitions": Sequence[AttributeDefinitionTypeDef],
+        "BillingMode": BillingModeType,
+        "ProvisionedThroughput": ProvisionedThroughputTypeDef,
+        "GlobalSecondaryIndexUpdates": Sequence[GlobalSecondaryIndexUpdateTypeDef],
+        "StreamSpecification": StreamSpecificationTypeDef,
+        "SSESpecification": SSESpecificationTypeDef,
+        "ReplicaUpdates": Sequence[ReplicationGroupUpdateTypeDef],
+        "TableClass": TableClassType,
+        "DeletionProtectionEnabled": bool,
+    },
+    total=False,
+)
+
+DescribeImportOutputTypeDef = TypedDict(
+    "DescribeImportOutputTypeDef",
+    {
+        "ImportTableDescription": ImportTableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportTableOutputTypeDef = TypedDict(
+    "ImportTableOutputTypeDef",
+    {
+        "ImportTableDescription": ImportTableDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBackupOutputTypeDef = TypedDict(
+    "DeleteBackupOutputTypeDef",
+    {
+        "BackupDescription": BackupDescriptionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupOutputTypeDef = TypedDict(
+    "DescribeBackupOutputTypeDef",
+    {
+        "BackupDescription": BackupDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchWriteItemInputRequestTypeDef = TypedDict(
+    "_RequiredBatchWriteItemInputRequestTypeDef",
+    {
+        "RequestItems": Mapping[str, Sequence[WriteRequestUnionTypeDef]],
+    },
+)
+_OptionalBatchWriteItemInputRequestTypeDef = TypedDict(
+    "_OptionalBatchWriteItemInputRequestTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+    },
+    total=False,
+)
+
+class BatchWriteItemInputRequestTypeDef(
+    _RequiredBatchWriteItemInputRequestTypeDef, _OptionalBatchWriteItemInputRequestTypeDef
+):
+    pass
+
+_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
+    "_RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    {
+        "RequestItems": Mapping[str, Sequence[WriteRequestUnionTypeDef]],
+    },
+)
+_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef = TypedDict(
+    "_OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef",
+    {
+        "ReturnConsumedCapacity": ReturnConsumedCapacityType,
+        "ReturnItemCollectionMetrics": ReturnItemCollectionMetricsType,
+    },
+    total=False,
+)
+
+class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(
+    _RequiredBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+    _OptionalBatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
+):
+    pass
+
 TableAutoScalingDescriptionTypeDef = TypedDict(
     "TableAutoScalingDescriptionTypeDef",
     {
         "TableName": str,
         "TableStatus": TableStatusType,
         "Replicas": List[ReplicaAutoScalingDescriptionTypeDef],
     },
+    total=False,
 )
 
 DescribeGlobalTableSettingsOutputTypeDef = TypedDict(
     "DescribeGlobalTableSettingsOutputTypeDef",
     {
         "GlobalTableName": str,
         "ReplicaSettings": List[ReplicaSettingsDescriptionTypeDef],
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/waiter.py` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb/waiter.pyi` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/PKG-INFO` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodb
-Version: 2.5.2.post2
-Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.15.0
+Version: 2.5.2.post3
+Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore dynamodb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore dynamodb type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-dynamodb"></a>
 
 # types-aiobotocore-dynamodb
 
 [![PyPI - types-aiobotocore-dynamodb](https://img.shields.io/pypi/v/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dynamodb?color=blue)](https://pypistats.org/packages/types-aiobotocore-dynamodb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodb)](https://pepy.tech/project/types-aiobotocore-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DynamoDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-dynamodb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +77,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -448,83 +447,54 @@
 )
 
 
 def check_value(value: AttributeActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_dynamodb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_dynamodb.type_defs import (
     ResponseMetadataTypeDef,
-    ArchivalSummaryTableTypeDef,
     ArchivalSummaryTypeDef,
-    AttributeDefinitionOutputTypeDef,
-    AttributeDefinitionServiceResourceTypeDef,
-    AttributeDefinitionTableOutputTypeDef,
-    AttributeDefinitionTableTypeDef,
     AttributeDefinitionTypeDef,
-    AttributeValueServiceResourceTypeDef,
-    AttributeValueTableTypeDef,
     AttributeValueTypeDef,
-    AttributeValueUpdateTableTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef,
     AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,
     BackupDetailsTypeDef,
-    BackupSummaryTableTypeDef,
     BackupSummaryTypeDef,
-    KeysAndAttributesServiceResourceTypeDef,
-    KeysAndAttributesServiceResourceOutputTypeDef,
+    TableAttributeValueTypeDef,
     BatchStatementErrorTypeDef,
-    ItemCollectionMetricsServiceResourceTypeDef,
-    BillingModeSummaryTableTypeDef,
     BillingModeSummaryTypeDef,
-    CapacityServiceResourceTypeDef,
-    CapacityTableTypeDef,
     CapacityTypeDef,
-    ConditionTableTypeDef,
+    ConditionBaseImportTypeDef,
     PointInTimeRecoveryDescriptionTypeDef,
     ContributorInsightsSummaryTypeDef,
     CreateBackupInputRequestTypeDef,
-    KeySchemaElementTableTypeDef,
-    ProjectionTableTypeDef,
-    ProvisionedThroughputTableTypeDef,
     KeySchemaElementTypeDef,
     ProjectionTypeDef,
     ProvisionedThroughputTypeDef,
     ReplicaTypeDef,
     CreateReplicaActionTypeDef,
-    ProvisionedThroughputOverrideTableTypeDef,
     ProvisionedThroughputOverrideTypeDef,
     SSESpecificationTypeDef,
     StreamSpecificationTypeDef,
     TagTypeDef,
-    KeySchemaElementServiceResourceTypeDef,
-    ProvisionedThroughputServiceResourceTypeDef,
-    SSESpecificationServiceResourceTypeDef,
-    StreamSpecificationServiceResourceTypeDef,
-    TagServiceResourceTypeDef,
     CsvOptionsOutputTypeDef,
     CsvOptionsTypeDef,
     DeleteBackupInputRequestTypeDef,
-    DeleteGlobalSecondaryIndexActionTableTypeDef,
     DeleteGlobalSecondaryIndexActionTypeDef,
-    ExpectedAttributeValueTableTypeDef,
-    ItemCollectionMetricsTableTypeDef,
     DeleteReplicaActionTypeDef,
-    DeleteReplicationGroupMemberActionTableTypeDef,
     DeleteReplicationGroupMemberActionTypeDef,
-    DeleteRequestServiceResourceOutputTypeDef,
-    DeleteRequestServiceResourceTypeDef,
     DeleteTableInputRequestTypeDef,
     DescribeBackupInputRequestTypeDef,
     DescribeContinuousBackupsInputRequestTypeDef,
     DescribeContributorInsightsInputRequestTypeDef,
     FailureExceptionTypeDef,
     EndpointTypeDef,
     DescribeExportInputRequestTypeDef,
@@ -536,261 +506,215 @@
     KinesisDataStreamDestinationTypeDef,
     DescribeTableInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeTableReplicaAutoScalingInputRequestTypeDef,
     DescribeTimeToLiveInputRequestTypeDef,
     TimeToLiveDescriptionTypeDef,
     ExportSummaryTypeDef,
-    ExportTableToPointInTimeInputRequestTypeDef,
-    GetItemInputTableGetItemTypeDef,
-    KeySchemaElementTableOutputTypeDef,
-    ProjectionTableOutputTypeDef,
-    ProvisionedThroughputDescriptionTableTypeDef,
-    KeySchemaElementOutputTypeDef,
+    TimestampTypeDef,
     ProjectionOutputTypeDef,
     ProvisionedThroughputDescriptionTypeDef,
-    ProvisionedThroughputOutputTypeDef,
-    ProjectionServiceResourceTypeDef,
-    ReplicaOutputTypeDef,
-    S3BucketSourceOutputTypeDef,
     S3BucketSourceTypeDef,
     KinesisStreamingDestinationInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ListBackupsInputRequestTypeDef,
     ListContributorInsightsInputRequestTypeDef,
     ListExportsInputRequestTypeDef,
     ListGlobalTablesInputRequestTypeDef,
     ListImportsInputRequestTypeDef,
     ListTablesInputRequestTypeDef,
     ListTagsOfResourceInputRequestTypeDef,
-    TagTableTypeDef,
-    TagOutputTypeDef,
     PointInTimeRecoverySpecificationTypeDef,
-    ProvisionedThroughputOverrideOutputTypeDef,
-    ProvisionedThroughputOverrideTableOutputTypeDef,
-    PutRequestServiceResourceOutputTypeDef,
-    PutRequestServiceResourceTypeDef,
-    TableClassSummaryTableTypeDef,
     TableClassSummaryTypeDef,
-    RestoreSummaryTableTypeDef,
     RestoreSummaryTypeDef,
-    SSEDescriptionTableTypeDef,
     SSEDescriptionTypeDef,
-    SSESpecificationOutputTypeDef,
-    SSESpecificationTableTypeDef,
-    StreamSpecificationOutputTypeDef,
-    StreamSpecificationTableOutputTypeDef,
-    StreamSpecificationTableTypeDef,
     TableBatchWriterRequestTypeDef,
-    TimeToLiveSpecificationOutputTypeDef,
     TimeToLiveSpecificationTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateContributorInsightsInputRequestTypeDef,
-    ArchivalSummaryTableResponseMetadataTypeDef,
-    BillingModeSummaryTableResponseMetadataTypeDef,
+    ArchivalSummaryResponseTypeDef,
+    BillingModeSummaryResponseTypeDef,
     DescribeLimitsOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     KinesisStreamingDestinationOutputTypeDef,
-    ListTablesOutputTableTypeDef,
     ListTablesOutputTypeDef,
-    ProvisionedThroughputDescriptionTableResponseMetadataTypeDef,
-    RestoreSummaryTableResponseMetadataTypeDef,
-    SSEDescriptionTableResponseMetadataTypeDef,
-    StreamSpecificationTableResponseMetadataTypeDef,
-    TableClassSummaryTableResponseMetadataTypeDef,
+    ProvisionedThroughputDescriptionResponseTypeDef,
+    RestoreSummaryResponseTypeDef,
+    SSEDescriptionResponseTypeDef,
+    StreamSpecificationResponseTypeDef,
+    TableClassSummaryResponseTypeDef,
     UpdateContributorInsightsOutputTypeDef,
-    AttributeValueUpdateTypeDef,
-    BatchStatementRequestTypeDef,
-    ConditionCheckTypeDef,
-    ConditionTypeDef,
+    UniversalAttributeValueTypeDef,
+    AutoScalingPolicyDescriptionTypeDef,
+    AutoScalingPolicyUpdateTypeDef,
+    CreateBackupOutputTypeDef,
+    ListBackupsOutputTypeDef,
     DeleteRequestOutputTypeDef,
-    DeleteRequestTypeDef,
-    DeleteTypeDef,
-    ExecuteStatementInputRequestTypeDef,
-    ExpectedAttributeValueTypeDef,
-    GetItemInputRequestTypeDef,
-    GetTypeDef,
+    GetItemInputTableGetItemTypeDef,
     ItemCollectionMetricsTypeDef,
     ItemResponseTypeDef,
     KeysAndAttributesOutputTypeDef,
-    KeysAndAttributesTypeDef,
-    ParameterizedStatementTypeDef,
     PutRequestOutputTypeDef,
-    PutRequestTypeDef,
-    PutTypeDef,
-    UpdateTypeDef,
-    AutoScalingPolicyDescriptionTypeDef,
-    AutoScalingPolicyUpdateTypeDef,
-    CreateBackupOutputTypeDef,
-    ListBackupsOutputTableTypeDef,
-    ListBackupsOutputTypeDef,
-    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
     BatchStatementResponseTypeDef,
-    ConsumedCapacityServiceResourceTypeDef,
-    ConsumedCapacityTableTypeDef,
     ConsumedCapacityTypeDef,
-    QueryInputTableQueryTypeDef,
-    ScanInputTableScanTypeDef,
     ContinuousBackupsDescriptionTypeDef,
     ListContributorInsightsOutputTypeDef,
-    CreateGlobalSecondaryIndexActionTableTypeDef,
-    UpdateGlobalSecondaryIndexActionTableTypeDef,
     LocalSecondaryIndexTypeDef,
     CreateGlobalSecondaryIndexActionTypeDef,
     GlobalSecondaryIndexTypeDef,
+    SourceTableDetailsTypeDef,
     UpdateGlobalSecondaryIndexActionTypeDef,
     CreateGlobalTableInputRequestTypeDef,
-    ReplicaGlobalSecondaryIndexTableTypeDef,
+    GlobalTableTypeDef,
+    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexTypeDef,
+    ListTagsOfResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     InputFormatOptionsOutputTypeDef,
     InputFormatOptionsTypeDef,
-    DeleteItemInputTableDeleteItemTypeDef,
-    PutItemInputTablePutItemTypeDef,
-    UpdateItemInputTableUpdateItemTypeDef,
     ReplicaUpdateTypeDef,
     DescribeContributorInsightsOutputTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeExportOutputTypeDef,
     ExportTableToPointInTimeOutputTypeDef,
     DescribeKinesisStreamingDestinationOutputTypeDef,
     DescribeTableInputTableExistsWaitTypeDef,
     DescribeTableInputTableNotExistsWaitTypeDef,
     DescribeTimeToLiveOutputTypeDef,
     ListExportsOutputTypeDef,
-    LocalSecondaryIndexDescriptionTableTypeDef,
-    GlobalSecondaryIndexDescriptionTableTypeDef,
+    ExportTableToPointInTimeInputRequestTypeDef,
+    ListBackupsInputRequestTypeDef,
+    GlobalSecondaryIndexInfoTypeDef,
+    GlobalSecondaryIndexOutputTypeDef,
     LocalSecondaryIndexDescriptionTypeDef,
     LocalSecondaryIndexInfoTypeDef,
     GlobalSecondaryIndexDescriptionTypeDef,
-    GlobalSecondaryIndexInfoTypeDef,
-    GlobalSecondaryIndexOutputTypeDef,
-    SourceTableDetailsTypeDef,
-    GlobalSecondaryIndexServiceResourceTypeDef,
-    LocalSecondaryIndexServiceResourceTypeDef,
-    GlobalTableTypeDef,
     ImportSummaryTypeDef,
     ListBackupsInputListBackupsPaginateTypeDef,
     ListTablesInputListTablesPaginateTypeDef,
     ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef,
-    QueryInputQueryPaginateTypeDef,
-    ScanInputScanPaginateTypeDef,
-    ListTagsOfResourceOutputTableTypeDef,
-    ListTagsOfResourceOutputTypeDef,
     UpdateContinuousBackupsInputRequestTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTypeDef,
-    ReplicaGlobalSecondaryIndexDescriptionTableTypeDef,
-    WriteRequestServiceResourceOutputTypeDef,
-    WriteRequestServiceResourceTypeDef,
-    UpdateTimeToLiveOutputTypeDef,
     UpdateTimeToLiveInputRequestTypeDef,
-    BatchExecuteStatementInputRequestTypeDef,
-    QueryInputRequestTypeDef,
-    ScanInputRequestTypeDef,
-    DeleteItemInputRequestTypeDef,
-    PutItemInputRequestTypeDef,
-    UpdateItemInputRequestTypeDef,
-    TransactGetItemTypeDef,
-    BatchGetItemInputRequestTypeDef,
-    ExecuteTransactionInputRequestTypeDef,
-    WriteRequestOutputTypeDef,
-    WriteRequestTypeDef,
-    TransactWriteItemTypeDef,
+    UpdateTimeToLiveOutputTypeDef,
+    AttributeValueUpdateTypeDef,
+    BatchStatementRequestTypeDef,
+    ConditionCheckTypeDef,
+    ConditionTypeDef,
+    DeleteRequestTypeDef,
+    DeleteTypeDef,
+    ExecuteStatementInputRequestTypeDef,
+    ExpectedAttributeValueTypeDef,
+    GetItemInputRequestTypeDef,
+    GetTypeDef,
+    KeysAndAttributesTypeDef,
+    ParameterizedStatementTypeDef,
+    PutRequestTypeDef,
+    PutTypeDef,
+    UpdateTypeDef,
     AutoScalingSettingsDescriptionTypeDef,
     AutoScalingSettingsUpdateTypeDef,
-    BatchGetItemOutputServiceResourceTypeDef,
-    DeleteItemOutputTableTypeDef,
-    GetItemOutputTableTypeDef,
-    PutItemOutputTableTypeDef,
-    QueryOutputTableTypeDef,
-    ScanOutputTableTypeDef,
-    UpdateItemOutputTableTypeDef,
+    WriteRequestOutputTypeDef,
     BatchExecuteStatementOutputTypeDef,
     BatchGetItemOutputTypeDef,
     DeleteItemOutputTypeDef,
     ExecuteStatementOutputTypeDef,
     ExecuteTransactionOutputTypeDef,
     GetItemOutputTypeDef,
     PutItemOutputTypeDef,
     QueryOutputTypeDef,
     ScanOutputTypeDef,
     TransactGetItemsOutputTypeDef,
     TransactWriteItemsOutputTypeDef,
     UpdateItemOutputTypeDef,
     DescribeContinuousBackupsOutputTypeDef,
     UpdateContinuousBackupsOutputTypeDef,
-    GlobalSecondaryIndexUpdateTableTypeDef,
-    CreateTableInputRequestTypeDef,
-    RestoreTableFromBackupInputRequestTypeDef,
-    RestoreTableToPointInTimeInputRequestTypeDef,
     TableCreationParametersTypeDef,
     GlobalSecondaryIndexUpdateTypeDef,
-    CreateReplicationGroupMemberActionTableTypeDef,
-    UpdateReplicationGroupMemberActionTableTypeDef,
+    ListGlobalTablesOutputTypeDef,
+    ReplicaDescriptionTypeDef,
     CreateReplicationGroupMemberActionTypeDef,
     UpdateReplicationGroupMemberActionTypeDef,
+    InputFormatOptionsUnionTypeDef,
     UpdateGlobalTableInputRequestTypeDef,
-    SourceTableFeatureDetailsTypeDef,
+    GlobalSecondaryIndexUnionTypeDef,
     TableCreationParametersOutputTypeDef,
-    CreateTableInputServiceResourceCreateTableTypeDef,
-    ListGlobalTablesOutputTypeDef,
+    SourceTableFeatureDetailsTypeDef,
     ListImportsOutputTypeDef,
-    ReplicaDescriptionTypeDef,
-    ReplicaDescriptionTableTypeDef,
-    BatchWriteItemOutputServiceResourceTypeDef,
-    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
-    TransactGetItemsInputRequestTypeDef,
-    BatchWriteItemOutputTypeDef,
-    BatchWriteItemInputRequestTypeDef,
-    TransactWriteItemsInputRequestTypeDef,
+    BatchExecuteStatementInputRequestTypeDef,
+    QueryInputQueryPaginateTypeDef,
+    QueryInputRequestTypeDef,
+    QueryInputTableQueryTypeDef,
+    ScanInputRequestTypeDef,
+    ScanInputScanPaginateTypeDef,
+    ScanInputTableScanTypeDef,
+    DeleteItemInputRequestTypeDef,
+    DeleteItemInputTableDeleteItemTypeDef,
+    PutItemInputRequestTypeDef,
+    PutItemInputTablePutItemTypeDef,
+    UpdateItemInputRequestTypeDef,
+    UpdateItemInputTableUpdateItemTypeDef,
+    TransactGetItemTypeDef,
+    KeysAndAttributesUnionTypeDef,
+    ExecuteTransactionInputRequestTypeDef,
+    WriteRequestTypeDef,
+    TransactWriteItemTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef,
     ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef,
     GlobalSecondaryIndexAutoScalingUpdateTypeDef,
     GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef,
     ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef,
     ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef,
+    BatchWriteItemOutputTypeDef,
     ImportTableInputRequestTypeDef,
-    ReplicationGroupUpdateTableTypeDef,
-    ReplicationGroupUpdateTypeDef,
-    BackupDescriptionTypeDef,
-    ImportTableDescriptionTypeDef,
     GlobalTableDescriptionTypeDef,
     TableDescriptionTypeDef,
-    TableDescriptionTableTypeDef,
+    ReplicationGroupUpdateTypeDef,
+    CreateTableInputRequestTypeDef,
+    CreateTableInputServiceResourceCreateTableTypeDef,
+    RestoreTableFromBackupInputRequestTypeDef,
+    RestoreTableToPointInTimeInputRequestTypeDef,
+    ImportTableDescriptionTypeDef,
+    TableCreationParametersUnionTypeDef,
+    BackupDescriptionTypeDef,
+    TransactGetItemsInputRequestTypeDef,
+    BatchGetItemInputRequestTypeDef,
+    BatchGetItemInputServiceResourceBatchGetItemTypeDef,
+    WriteRequestUnionTypeDef,
+    TransactWriteItemsInputRequestTypeDef,
     ReplicaAutoScalingDescriptionTypeDef,
     ReplicaSettingsDescriptionTypeDef,
     ReplicaAutoScalingUpdateTypeDef,
     ReplicaSettingsUpdateTypeDef,
-    UpdateTableInputTableUpdateTypeDef,
-    UpdateTableInputRequestTypeDef,
-    DeleteBackupOutputTypeDef,
-    DescribeBackupOutputTypeDef,
-    DescribeImportOutputTypeDef,
-    ImportTableOutputTypeDef,
     CreateGlobalTableOutputTypeDef,
     DescribeGlobalTableOutputTypeDef,
     UpdateGlobalTableOutputTypeDef,
     CreateTableOutputTypeDef,
     DeleteTableOutputTypeDef,
     DescribeTableOutputTypeDef,
     RestoreTableFromBackupOutputTypeDef,
     RestoreTableToPointInTimeOutputTypeDef,
     UpdateTableOutputTypeDef,
-    DeleteTableOutputTableTypeDef,
+    UpdateTableInputRequestTypeDef,
+    UpdateTableInputTableUpdateTypeDef,
+    DescribeImportOutputTypeDef,
+    ImportTableOutputTypeDef,
+    DeleteBackupOutputTypeDef,
+    DescribeBackupOutputTypeDef,
+    BatchWriteItemInputRequestTypeDef,
+    BatchWriteItemInputServiceResourceBatchWriteItemTypeDef,
     TableAutoScalingDescriptionTypeDef,
     DescribeGlobalTableSettingsOutputTypeDef,
     UpdateGlobalTableSettingsOutputTypeDef,
     UpdateTableReplicaAutoScalingInputRequestTypeDef,
     UpdateGlobalTableSettingsInputRequestTypeDef,
     DescribeTableReplicaAutoScalingOutputTypeDef,
     UpdateTableReplicaAutoScalingOutputTypeDef,
 )
 
 
-def get_structure() -> ResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dynamodb-2.5.2.post2/types_aiobotocore_dynamodb.egg-info/SOURCES.txt` & `types-aiobotocore-dynamodb-2.5.2.post3/types_aiobotocore_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


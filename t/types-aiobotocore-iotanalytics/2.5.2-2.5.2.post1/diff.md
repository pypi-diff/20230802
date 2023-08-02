# Comparing `tmp/types-aiobotocore-iotanalytics-2.5.2.tar.gz` & `tmp/types-aiobotocore-iotanalytics-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotanalytics-2.5.2.tar", last modified: Sat Jul  8 01:43:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotanalytics-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
```

## Comparing `types-aiobotocore-iotanalytics-2.5.2.tar` & `types-aiobotocore-iotanalytics-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.530299 types-aiobotocore-iotanalytics-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18938 2023-07-08 01:43:46.526299 types-aiobotocore-iotanalytics-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17353 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:46.530299 types-aiobotocore-iotanalytics-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:32:38.000000 types-aiobotocore-iotanalytics-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.526299 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28254 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28206 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46258 2023-07-08 01:32:40.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46187 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:39.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.526299 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18938 2023-07-08 01:43:46.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:46.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:46.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:46.000000 types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.417563 types-aiobotocore-iotanalytics-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-08-02 14:52:26.409563 types-aiobotocore-iotanalytics-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18086 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.417563 types-aiobotocore-iotanalytics-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.409563 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28217 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28169 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-08-02 14:40:42.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-08-02 14:40:42.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52421 2023-08-02 14:40:43.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52341 2023-08-02 14:40:42.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.409563 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-08-02 14:52:26.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:26.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:26.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2/LICENSE` & `types-aiobotocore-iotanalytics-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2/PKG-INFO` & `types-aiobotocore-iotanalytics-2.5.2.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotanalytics
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTAnalytics 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTAnalytics 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotanalytics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotanalytics type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotanalytics"></a>
 
 # types-aiobotocore-iotanalytics
 
 [![PyPI - types-aiobotocore-iotanalytics](https://img.shields.io/pypi/v/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotanalytics?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotanalytics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotanalytics)](https://pepy.tech/project/types-aiobotocore-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTAnalytics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [types-aiobotocore-iotanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/).
 
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
@@ -330,40 +329,40 @@
 )
 
 
 def check_value(value: ChannelStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotanalytics.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotanalytics.type_defs import (
+    AddAttributesActivityOutputTypeDef,
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
-    MessageTypeDef,
+    ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
-    CustomerManagedChannelS3StorageSummaryTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
+    CustomerManagedChannelS3StorageSummaryTypeDef,
     RetentionPeriodTypeDef,
     ColumnTypeDef,
     ResourceConfigurationTypeDef,
     TagTypeDef,
     CreateDatasetContentRequestRequestTypeDef,
-    CreateDatasetContentResponseTypeDef,
     VersioningConfigurationTypeDef,
-    CreatePipelineResponseTypeDef,
     CustomerManagedDatastoreS3StorageSummaryTypeDef,
     CustomerManagedDatastoreS3StorageTypeDef,
     DatasetActionSummaryTypeDef,
     IotEventsDestinationConfigurationTypeDef,
     DatasetContentStatusTypeDef,
     DatasetContentVersionValueTypeDef,
     DatasetEntryTypeDef,
@@ -384,109 +383,130 @@
     DescribeChannelRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeDatastoreRequestRequestTypeDef,
     LoggingOptionsTypeDef,
     DescribePipelineRequestRequestTypeDef,
     DeviceRegistryEnrichActivityTypeDef,
     DeviceShadowEnrichActivityTypeDef,
-    EmptyResponseMetadataTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
     GlueConfigurationTypeDef,
     LambdaActivityTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-    ListDatasetContentsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    TimestampTypeDef,
     ListDatasetsRequestRequestTypeDef,
-    ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MathActivityTypeDef,
     OutputFileUriValueTypeDef,
-    PaginatorConfigTypeDef,
+    RemoveAttributesActivityOutputTypeDef,
+    SelectAttributesActivityOutputTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
-    ResponseMetadataTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    BatchPutMessageResponseTypeDef,
+    CreateDatasetContentResponseTypeDef,
+    CreatePipelineResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     RunPipelineActivityResponseTypeDef,
-    SampleChannelDataRequestRequestTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    BatchPutMessageResponseTypeDef,
-    BatchPutMessageRequestRequestTypeDef,
-    StartPipelineReprocessingRequestRequestTypeDef,
+    MessageTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
-    ChannelStorageSummaryTypeDef,
+    ChannelStorageOutputTypeDef,
     ChannelStorageTypeDef,
+    ChannelStorageSummaryTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
+    SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatasetContentSummaryTypeDef,
     GetDatasetContentResponseTypeDef,
     DatasetTriggerTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     DatastorePartitionTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     S3DestinationConfigurationTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListDatastoresRequestListDatastoresPaginateTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
+    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    ListDatasetContentsRequestRequestTypeDef,
+    SampleChannelDataRequestRequestTypeDef,
+    StartPipelineReprocessingRequestRequestTypeDef,
     VariableTypeDef,
+    PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
-    ChannelSummaryTypeDef,
+    BatchPutMessageRequestRequestTypeDef,
     ChannelTypeDef,
+    ChannelStorageUnionTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    ChannelSummaryTypeDef,
+    ParquetConfigurationOutputTypeDef,
     ParquetConfigurationTypeDef,
     ListDatasetContentsResponseTypeDef,
     DatasetSummaryTypeDef,
     DatastoreStorageSummaryTypeDef,
+    DatastoreStorageOutputTypeDef,
     DatastoreStorageTypeDef,
+    DatastorePartitionsOutputTypeDef,
     DatastorePartitionsTypeDef,
     LateDataRuleTypeDef,
+    SqlQueryDatasetActionOutputTypeDef,
     SqlQueryDatasetActionTypeDef,
     DatasetContentDeliveryDestinationTypeDef,
+    ContainerDatasetActionOutputTypeDef,
     ContainerDatasetActionTypeDef,
-    CreatePipelineRequestRequestTypeDef,
     PipelineTypeDef,
+    PipelineActivityUnionTypeDef,
     RunPipelineActivityRequestRequestTypeDef,
-    UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
-    ListChannelsResponseTypeDef,
     DescribeChannelResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     ListDatasetsResponseTypeDef,
+    DatastoreStorageUnionTypeDef,
     DatastoreSummaryTypeDef,
+    DatastorePartitionsUnionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
+    DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DescribePipelineResponseTypeDef,
-    CreateDatastoreRequestRequestTypeDef,
+    CreatePipelineRequestRequestTypeDef,
+    UpdatePipelineRequestRequestTypeDef,
     DatastoreTypeDef,
+    CreateDatastoreRequestRequestTypeDef,
+    FileFormatConfigurationUnionTypeDef,
     UpdateDatastoreRequestRequestTypeDef,
     ListDatastoresResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DatasetTypeDef,
-    UpdateDatasetRequestRequestTypeDef,
+    DatasetActionUnionTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeDatasetResponseTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    UpdateDatasetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddAttributesActivityTypeDef:
+def get_value() -> AddAttributesActivityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2/README.md` & `types-aiobotocore-iotanalytics-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iotanalytics"></a>
 
 # types-aiobotocore-iotanalytics
 
 [![PyPI - types-aiobotocore-iotanalytics](https://img.shields.io/pypi/v/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotanalytics?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotanalytics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotanalytics)](https://pepy.tech/project/types-aiobotocore-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTAnalytics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [types-aiobotocore-iotanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/).
 
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
@@ -297,40 +297,40 @@
 )
 
 
 def check_value(value: ChannelStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotanalytics.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotanalytics.type_defs import (
+    AddAttributesActivityOutputTypeDef,
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
-    MessageTypeDef,
+    ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
-    CustomerManagedChannelS3StorageSummaryTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
+    CustomerManagedChannelS3StorageSummaryTypeDef,
     RetentionPeriodTypeDef,
     ColumnTypeDef,
     ResourceConfigurationTypeDef,
     TagTypeDef,
     CreateDatasetContentRequestRequestTypeDef,
-    CreateDatasetContentResponseTypeDef,
     VersioningConfigurationTypeDef,
-    CreatePipelineResponseTypeDef,
     CustomerManagedDatastoreS3StorageSummaryTypeDef,
     CustomerManagedDatastoreS3StorageTypeDef,
     DatasetActionSummaryTypeDef,
     IotEventsDestinationConfigurationTypeDef,
     DatasetContentStatusTypeDef,
     DatasetContentVersionValueTypeDef,
     DatasetEntryTypeDef,
@@ -351,109 +351,130 @@
     DescribeChannelRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeDatastoreRequestRequestTypeDef,
     LoggingOptionsTypeDef,
     DescribePipelineRequestRequestTypeDef,
     DeviceRegistryEnrichActivityTypeDef,
     DeviceShadowEnrichActivityTypeDef,
-    EmptyResponseMetadataTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
     GlueConfigurationTypeDef,
     LambdaActivityTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-    ListDatasetContentsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    TimestampTypeDef,
     ListDatasetsRequestRequestTypeDef,
-    ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MathActivityTypeDef,
     OutputFileUriValueTypeDef,
-    PaginatorConfigTypeDef,
+    RemoveAttributesActivityOutputTypeDef,
+    SelectAttributesActivityOutputTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
-    ResponseMetadataTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    BatchPutMessageResponseTypeDef,
+    CreateDatasetContentResponseTypeDef,
+    CreatePipelineResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     RunPipelineActivityResponseTypeDef,
-    SampleChannelDataRequestRequestTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    BatchPutMessageResponseTypeDef,
-    BatchPutMessageRequestRequestTypeDef,
-    StartPipelineReprocessingRequestRequestTypeDef,
+    MessageTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
-    ChannelStorageSummaryTypeDef,
+    ChannelStorageOutputTypeDef,
     ChannelStorageTypeDef,
+    ChannelStorageSummaryTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
+    SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatasetContentSummaryTypeDef,
     GetDatasetContentResponseTypeDef,
     DatasetTriggerTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     DatastorePartitionTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     S3DestinationConfigurationTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListDatastoresRequestListDatastoresPaginateTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
+    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    ListDatasetContentsRequestRequestTypeDef,
+    SampleChannelDataRequestRequestTypeDef,
+    StartPipelineReprocessingRequestRequestTypeDef,
     VariableTypeDef,
+    PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
-    ChannelSummaryTypeDef,
+    BatchPutMessageRequestRequestTypeDef,
     ChannelTypeDef,
+    ChannelStorageUnionTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    ChannelSummaryTypeDef,
+    ParquetConfigurationOutputTypeDef,
     ParquetConfigurationTypeDef,
     ListDatasetContentsResponseTypeDef,
     DatasetSummaryTypeDef,
     DatastoreStorageSummaryTypeDef,
+    DatastoreStorageOutputTypeDef,
     DatastoreStorageTypeDef,
+    DatastorePartitionsOutputTypeDef,
     DatastorePartitionsTypeDef,
     LateDataRuleTypeDef,
+    SqlQueryDatasetActionOutputTypeDef,
     SqlQueryDatasetActionTypeDef,
     DatasetContentDeliveryDestinationTypeDef,
+    ContainerDatasetActionOutputTypeDef,
     ContainerDatasetActionTypeDef,
-    CreatePipelineRequestRequestTypeDef,
     PipelineTypeDef,
+    PipelineActivityUnionTypeDef,
     RunPipelineActivityRequestRequestTypeDef,
-    UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
-    ListChannelsResponseTypeDef,
     DescribeChannelResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     ListDatasetsResponseTypeDef,
+    DatastoreStorageUnionTypeDef,
     DatastoreSummaryTypeDef,
+    DatastorePartitionsUnionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
+    DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DescribePipelineResponseTypeDef,
-    CreateDatastoreRequestRequestTypeDef,
+    CreatePipelineRequestRequestTypeDef,
+    UpdatePipelineRequestRequestTypeDef,
     DatastoreTypeDef,
+    CreateDatastoreRequestRequestTypeDef,
+    FileFormatConfigurationUnionTypeDef,
     UpdateDatastoreRequestRequestTypeDef,
     ListDatastoresResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DatasetTypeDef,
-    UpdateDatasetRequestRequestTypeDef,
+    DatasetActionUnionTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeDatasetResponseTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    UpdateDatasetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddAttributesActivityTypeDef:
+def get_value() -> AddAttributesActivityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2/setup.py` & `types-aiobotocore-iotanalytics-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotanalytics",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iotanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTAnalytics 2.5.2 service generated with"
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
-    keywords="aiobotocore iotanalytics type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore iotanalytics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotanalytics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/"
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/__init__.py` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/__init__.pyi` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/__main__.py` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTAnalytics 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IoTAnalytics 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics\nOther"
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

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/client.py` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,65 +11,65 @@
 
     session = get_session()
     async with session.create_client("iotanalytics") as client:
         client: IoTAnalyticsClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .paginator import (
     ListChannelsPaginator,
     ListDatasetContentsPaginator,
     ListDatasetsPaginator,
     ListDatastoresPaginator,
     ListPipelinesPaginator,
 )
 from .type_defs import (
     BatchPutMessageResponseTypeDef,
+    BlobTypeDef,
     ChannelMessagesTypeDef,
-    ChannelStorageTypeDef,
+    ChannelStorageUnionTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetContentResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     CreatePipelineResponseTypeDef,
-    DatasetActionTypeDef,
+    DatasetActionUnionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetTriggerTypeDef,
-    DatastorePartitionsTypeDef,
-    DatastoreStorageTypeDef,
+    DatastorePartitionsUnionTypeDef,
+    DatastoreStorageUnionTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     DescribePipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    FileFormatConfigurationTypeDef,
+    FileFormatConfigurationUnionTypeDef,
     GetDatasetContentResponseTypeDef,
     LateDataRuleTypeDef,
     ListChannelsResponseTypeDef,
     ListDatasetContentsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListDatastoresResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LoggingOptionsTypeDef,
     MessageTypeDef,
-    PipelineActivityTypeDef,
+    PipelineActivityUnionTypeDef,
     RetentionPeriodTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     VersioningConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -150,30 +150,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#close)
         """
 
     async def create_channel(
         self,
         *,
         channelName: str,
-        channelStorage: ChannelStorageTypeDef = ...,
+        channelStorage: ChannelStorageUnionTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateChannelResponseTypeDef:
         """
         Used to create a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_channel)
         """
 
     async def create_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[DatasetActionTypeDef],
+        actions: Sequence[DatasetActionUnionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
@@ -195,32 +195,32 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_dataset_content)
         """
 
     async def create_datastore(
         self,
         *,
         datastoreName: str,
-        datastoreStorage: DatastoreStorageTypeDef = ...,
+        datastoreStorage: DatastoreStorageUnionTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...,
-        datastorePartitions: DatastorePartitionsTypeDef = ...
+        fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...,
+        datastorePartitions: DatastorePartitionsUnionTypeDef = ...
     ) -> CreateDatastoreResponseTypeDef:
         """
         Creates a data store, which is a repository for messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_datastore)
         """
 
     async def create_pipeline(
         self,
         *,
         pipelineName: str,
-        pipelineActivities: Sequence[PipelineActivityTypeDef],
+        pipelineActivities: Sequence[PipelineActivityUnionTypeDef],
         tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_pipeline)
@@ -348,16 +348,16 @@
 
     async def list_dataset_contents(
         self,
         *,
         datasetName: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        scheduledOnOrAfter: Union[datetime, str] = ...,
-        scheduledBefore: Union[datetime, str] = ...
+        scheduledOnOrAfter: TimestampTypeDef = ...,
+        scheduledBefore: TimestampTypeDef = ...
     ) -> ListDatasetContentsResponseTypeDef:
         """
         Lists information about dataset contents that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.list_dataset_contents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#list_dataset_contents)
         """
@@ -409,48 +409,45 @@
         Sets or updates the IoT Analytics logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.put_logging_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#put_logging_options)
         """
 
     async def run_pipeline_activity(
-        self,
-        *,
-        pipelineActivity: PipelineActivityTypeDef,
-        payloads: Sequence[Union[str, bytes, IO[Any], StreamingBody]]
+        self, *, pipelineActivity: PipelineActivityUnionTypeDef, payloads: Sequence[BlobTypeDef]
     ) -> RunPipelineActivityResponseTypeDef:
         """
         Simulates the results of running a pipeline activity on a message payload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.run_pipeline_activity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#run_pipeline_activity)
         """
 
     async def sample_channel_data(
         self,
         *,
         channelName: str,
         maxMessages: int = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...
     ) -> SampleChannelDataResponseTypeDef:
         """
         Retrieves a sample of messages from the specified channel ingested during the
         specified timeframe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.sample_channel_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#sample_channel_data)
         """
 
     async def start_pipeline_reprocessing(
         self,
         *,
         pipelineName: str,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         channelMessages: ChannelMessagesTypeDef = ...
     ) -> StartPipelineReprocessingResponseTypeDef:
         """
         Starts the reprocessing of raw message data through the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.start_pipeline_reprocessing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#start_pipeline_reprocessing)
@@ -472,29 +469,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#untag_resource)
         """
 
     async def update_channel(
         self,
         *,
         channelName: str,
-        channelStorage: ChannelStorageTypeDef = ...,
+        channelStorage: ChannelStorageUnionTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_channel)
         """
 
     async def update_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[DatasetActionTypeDef],
+        actions: Sequence[DatasetActionUnionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
@@ -505,26 +502,26 @@
         """
 
     async def update_datastore(
         self,
         *,
         datastoreName: str,
         retentionPeriod: RetentionPeriodTypeDef = ...,
-        datastoreStorage: DatastoreStorageTypeDef = ...,
-        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...
+        datastoreStorage: DatastoreStorageUnionTypeDef = ...,
+        fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_datastore)
         """
 
     async def update_pipeline(
-        self, *, pipelineName: str, pipelineActivities: Sequence[PipelineActivityTypeDef]
+        self, *, pipelineName: str, pipelineActivities: Sequence[PipelineActivityUnionTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/client.pyi` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,65 +11,65 @@
 
     session = get_session()
     async with session.create_client("iotanalytics") as client:
         client: IoTAnalyticsClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .paginator import (
     ListChannelsPaginator,
     ListDatasetContentsPaginator,
     ListDatasetsPaginator,
     ListDatastoresPaginator,
     ListPipelinesPaginator,
 )
 from .type_defs import (
     BatchPutMessageResponseTypeDef,
+    BlobTypeDef,
     ChannelMessagesTypeDef,
-    ChannelStorageTypeDef,
+    ChannelStorageUnionTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetContentResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     CreatePipelineResponseTypeDef,
-    DatasetActionTypeDef,
+    DatasetActionUnionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetTriggerTypeDef,
-    DatastorePartitionsTypeDef,
-    DatastoreStorageTypeDef,
+    DatastorePartitionsUnionTypeDef,
+    DatastoreStorageUnionTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     DescribePipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    FileFormatConfigurationTypeDef,
+    FileFormatConfigurationUnionTypeDef,
     GetDatasetContentResponseTypeDef,
     LateDataRuleTypeDef,
     ListChannelsResponseTypeDef,
     ListDatasetContentsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListDatastoresResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LoggingOptionsTypeDef,
     MessageTypeDef,
-    PipelineActivityTypeDef,
+    PipelineActivityUnionTypeDef,
     RetentionPeriodTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     VersioningConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -141,29 +141,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#close)
         """
     async def create_channel(
         self,
         *,
         channelName: str,
-        channelStorage: ChannelStorageTypeDef = ...,
+        channelStorage: ChannelStorageUnionTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateChannelResponseTypeDef:
         """
         Used to create a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_channel)
         """
     async def create_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[DatasetActionTypeDef],
+        actions: Sequence[DatasetActionUnionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
@@ -183,31 +183,31 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_dataset_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_dataset_content)
         """
     async def create_datastore(
         self,
         *,
         datastoreName: str,
-        datastoreStorage: DatastoreStorageTypeDef = ...,
+        datastoreStorage: DatastoreStorageUnionTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...,
-        datastorePartitions: DatastorePartitionsTypeDef = ...
+        fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...,
+        datastorePartitions: DatastorePartitionsUnionTypeDef = ...
     ) -> CreateDatastoreResponseTypeDef:
         """
         Creates a data store, which is a repository for messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_datastore)
         """
     async def create_pipeline(
         self,
         *,
         pipelineName: str,
-        pipelineActivities: Sequence[PipelineActivityTypeDef],
+        pipelineActivities: Sequence[PipelineActivityUnionTypeDef],
         tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_pipeline)
@@ -321,16 +321,16 @@
         """
     async def list_dataset_contents(
         self,
         *,
         datasetName: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        scheduledOnOrAfter: Union[datetime, str] = ...,
-        scheduledBefore: Union[datetime, str] = ...
+        scheduledOnOrAfter: TimestampTypeDef = ...,
+        scheduledBefore: TimestampTypeDef = ...
     ) -> ListDatasetContentsResponseTypeDef:
         """
         Lists information about dataset contents that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.list_dataset_contents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#list_dataset_contents)
         """
@@ -376,46 +376,43 @@
         """
         Sets or updates the IoT Analytics logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.put_logging_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#put_logging_options)
         """
     async def run_pipeline_activity(
-        self,
-        *,
-        pipelineActivity: PipelineActivityTypeDef,
-        payloads: Sequence[Union[str, bytes, IO[Any], StreamingBody]]
+        self, *, pipelineActivity: PipelineActivityUnionTypeDef, payloads: Sequence[BlobTypeDef]
     ) -> RunPipelineActivityResponseTypeDef:
         """
         Simulates the results of running a pipeline activity on a message payload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.run_pipeline_activity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#run_pipeline_activity)
         """
     async def sample_channel_data(
         self,
         *,
         channelName: str,
         maxMessages: int = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...
     ) -> SampleChannelDataResponseTypeDef:
         """
         Retrieves a sample of messages from the specified channel ingested during the
         specified timeframe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.sample_channel_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#sample_channel_data)
         """
     async def start_pipeline_reprocessing(
         self,
         *,
         pipelineName: str,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         channelMessages: ChannelMessagesTypeDef = ...
     ) -> StartPipelineReprocessingResponseTypeDef:
         """
         Starts the reprocessing of raw message data through the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.start_pipeline_reprocessing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#start_pipeline_reprocessing)
@@ -434,28 +431,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#untag_resource)
         """
     async def update_channel(
         self,
         *,
         channelName: str,
-        channelStorage: ChannelStorageTypeDef = ...,
+        channelStorage: ChannelStorageUnionTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_channel)
         """
     async def update_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[DatasetActionTypeDef],
+        actions: Sequence[DatasetActionUnionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
@@ -465,25 +462,25 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_dataset)
         """
     async def update_datastore(
         self,
         *,
         datastoreName: str,
         retentionPeriod: RetentionPeriodTypeDef = ...,
-        datastoreStorage: DatastoreStorageTypeDef = ...,
-        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...
+        datastoreStorage: DatastoreStorageUnionTypeDef = ...,
+        fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_datastore)
         """
     async def update_pipeline(
-        self, *, pipelineName: str, pipelineActivities: Sequence[PipelineActivityTypeDef]
+        self, *, pipelineName: str, pipelineActivities: Sequence[PipelineActivityUnionTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/literals.py` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/literals.pyi` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/paginator.py` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,27 +24,27 @@
         list_channels_paginator: ListChannelsPaginator = client.get_paginator("list_channels")
         list_dataset_contents_paginator: ListDatasetContentsPaginator = client.get_paginator("list_dataset_contents")
         list_datasets_paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")
         list_datastores_paginator: ListDatastoresPaginator = client.get_paginator("list_datastores")
         list_pipelines_paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ListChannelsResponseTypeDef,
     ListDatasetContentsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListDatastoresResponseTypeDef,
     ListPipelinesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListChannelsPaginator",
     "ListDatasetContentsPaginator",
     "ListDatasetsPaginator",
     "ListDatastoresPaginator",
@@ -65,15 +65,15 @@
 class ListChannelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listchannelspaginator)
         """
 
 
@@ -83,60 +83,60 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatasetcontentspaginator)
     """
 
     def paginate(
         self,
         *,
         datasetName: str,
-        scheduledOnOrAfter: Union[datetime, str] = ...,
-        scheduledBefore: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        scheduledOnOrAfter: TimestampTypeDef = ...,
+        scheduledBefore: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatasetcontentspaginator)
         """
 
 
 class ListDatasetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatasetspaginator)
         """
 
 
 class ListDatastoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatastorespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatastoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatastorespaginator)
         """
 
 
 class ListPipelinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listpipelinespaginator)
         """
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/paginator.pyi` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -24,27 +24,27 @@
         list_channels_paginator: ListChannelsPaginator = client.get_paginator("list_channels")
         list_dataset_contents_paginator: ListDatasetContentsPaginator = client.get_paginator("list_dataset_contents")
         list_datasets_paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")
         list_datastores_paginator: ListDatastoresPaginator = client.get_paginator("list_datastores")
         list_pipelines_paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ListChannelsResponseTypeDef,
     ListDatasetContentsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListDatastoresResponseTypeDef,
     ListPipelinesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListChannelsPaginator",
     "ListDatasetContentsPaginator",
     "ListDatasetsPaginator",
     "ListDatastoresPaginator",
@@ -62,15 +62,15 @@
 class ListChannelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listchannelspaginator)
         """
 
 class ListDatasetContentsPaginator(AioPaginator):
@@ -79,57 +79,57 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatasetcontentspaginator)
     """
 
     def paginate(
         self,
         *,
         datasetName: str,
-        scheduledOnOrAfter: Union[datetime, str] = ...,
-        scheduledBefore: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        scheduledOnOrAfter: TimestampTypeDef = ...,
+        scheduledBefore: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetContentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatasetcontentspaginator)
         """
 
 class ListDatasetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatasetspaginator)
         """
 
 class ListDatastoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatastorespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatastoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listdatastorespaginator)
         """
 
 class ListPipelinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/paginators/#listpipelinespaginator)
         """
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/type_defs.py` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotanalytics service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_iotanalytics.type_defs import AddAttributesActivityTypeDef
+    from types_aiobotocore_iotanalytics.type_defs import AddAttributesActivityOutputTypeDef
 
-    data: AddAttributesActivityTypeDef = {...}
+    data: AddAttributesActivityOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -33,33 +33,32 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AddAttributesActivityOutputTypeDef",
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
-    "MessageTypeDef",
+    "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
     "ChannelActivityTypeDef",
     "ChannelMessagesTypeDef",
     "EstimatedResourceSizeTypeDef",
-    "CustomerManagedChannelS3StorageSummaryTypeDef",
     "CustomerManagedChannelS3StorageTypeDef",
+    "CustomerManagedChannelS3StorageSummaryTypeDef",
     "RetentionPeriodTypeDef",
     "ColumnTypeDef",
     "ResourceConfigurationTypeDef",
     "TagTypeDef",
     "CreateDatasetContentRequestRequestTypeDef",
-    "CreateDatasetContentResponseTypeDef",
     "VersioningConfigurationTypeDef",
-    "CreatePipelineResponseTypeDef",
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     "CustomerManagedDatastoreS3StorageTypeDef",
     "DatasetActionSummaryTypeDef",
     "IotEventsDestinationConfigurationTypeDef",
     "DatasetContentStatusTypeDef",
     "DatasetContentVersionValueTypeDef",
     "DatasetEntryTypeDef",
@@ -80,107 +79,148 @@
     "DescribeChannelRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeDatastoreRequestRequestTypeDef",
     "LoggingOptionsTypeDef",
     "DescribePipelineRequestRequestTypeDef",
     "DeviceRegistryEnrichActivityTypeDef",
     "DeviceShadowEnrichActivityTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FilterActivityTypeDef",
     "GetDatasetContentRequestRequestTypeDef",
     "GlueConfigurationTypeDef",
     "LambdaActivityTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    "ListDatasetContentsRequestRequestTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "TimestampTypeDef",
     "ListDatasetsRequestRequestTypeDef",
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListDatastoresRequestRequestTypeDef",
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MathActivityTypeDef",
     "OutputFileUriValueTypeDef",
-    "PaginatorConfigTypeDef",
+    "RemoveAttributesActivityOutputTypeDef",
+    "SelectAttributesActivityOutputTypeDef",
     "RemoveAttributesActivityTypeDef",
     "SelectAttributesActivityTypeDef",
     "ReprocessingSummaryTypeDef",
-    "ResponseMetadataTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "BatchPutMessageResponseTypeDef",
+    "CreateDatasetContentResponseTypeDef",
+    "CreatePipelineResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "RunPipelineActivityResponseTypeDef",
-    "SampleChannelDataRequestRequestTypeDef",
     "SampleChannelDataResponseTypeDef",
     "StartPipelineReprocessingResponseTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "BatchPutMessageResponseTypeDef",
-    "BatchPutMessageRequestRequestTypeDef",
-    "StartPipelineReprocessingRequestRequestTypeDef",
+    "MessageTypeDef",
     "ChannelStatisticsTypeDef",
     "DatastoreStatisticsTypeDef",
-    "ChannelStorageSummaryTypeDef",
+    "ChannelStorageOutputTypeDef",
     "ChannelStorageTypeDef",
+    "ChannelStorageSummaryTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateDatastoreResponseTypeDef",
+    "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatasetContentSummaryTypeDef",
     "GetDatasetContentResponseTypeDef",
     "DatasetTriggerTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageTypeDef",
     "DatastorePartitionTypeDef",
     "LateDataRuleConfigurationTypeDef",
     "QueryFilterTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "S3DestinationConfigurationTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    "ListDatasetContentsRequestRequestTypeDef",
+    "SampleChannelDataRequestRequestTypeDef",
+    "StartPipelineReprocessingRequestRequestTypeDef",
     "VariableTypeDef",
+    "PipelineActivityOutputTypeDef",
     "PipelineActivityTypeDef",
     "PipelineSummaryTypeDef",
-    "ChannelSummaryTypeDef",
+    "BatchPutMessageRequestRequestTypeDef",
     "ChannelTypeDef",
+    "ChannelStorageUnionTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
+    "ChannelSummaryTypeDef",
+    "ParquetConfigurationOutputTypeDef",
     "ParquetConfigurationTypeDef",
     "ListDatasetContentsResponseTypeDef",
     "DatasetSummaryTypeDef",
     "DatastoreStorageSummaryTypeDef",
+    "DatastoreStorageOutputTypeDef",
     "DatastoreStorageTypeDef",
+    "DatastorePartitionsOutputTypeDef",
     "DatastorePartitionsTypeDef",
     "LateDataRuleTypeDef",
+    "SqlQueryDatasetActionOutputTypeDef",
     "SqlQueryDatasetActionTypeDef",
     "DatasetContentDeliveryDestinationTypeDef",
+    "ContainerDatasetActionOutputTypeDef",
     "ContainerDatasetActionTypeDef",
-    "CreatePipelineRequestRequestTypeDef",
     "PipelineTypeDef",
+    "PipelineActivityUnionTypeDef",
     "RunPipelineActivityRequestRequestTypeDef",
-    "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
-    "ListChannelsResponseTypeDef",
     "DescribeChannelResponseTypeDef",
+    "ListChannelsResponseTypeDef",
+    "FileFormatConfigurationOutputTypeDef",
     "FileFormatConfigurationTypeDef",
     "ListDatasetsResponseTypeDef",
+    "DatastoreStorageUnionTypeDef",
     "DatastoreSummaryTypeDef",
+    "DatastorePartitionsUnionTypeDef",
     "DatasetContentDeliveryRuleTypeDef",
+    "DatasetActionOutputTypeDef",
     "DatasetActionTypeDef",
     "DescribePipelineResponseTypeDef",
-    "CreateDatastoreRequestRequestTypeDef",
+    "CreatePipelineRequestRequestTypeDef",
+    "UpdatePipelineRequestRequestTypeDef",
     "DatastoreTypeDef",
+    "CreateDatastoreRequestRequestTypeDef",
+    "FileFormatConfigurationUnionTypeDef",
     "UpdateDatastoreRequestRequestTypeDef",
     "ListDatastoresResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
-    "UpdateDatasetRequestRequestTypeDef",
+    "DatasetActionUnionTypeDef",
     "DescribeDatastoreResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "UpdateDatasetRequestRequestTypeDef",
+)
+
+_RequiredAddAttributesActivityOutputTypeDef = TypedDict(
+    "_RequiredAddAttributesActivityOutputTypeDef",
+    {
+        "name": str,
+        "attributes": Dict[str, str],
+    },
+)
+_OptionalAddAttributesActivityOutputTypeDef = TypedDict(
+    "_OptionalAddAttributesActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
 )
 
+class AddAttributesActivityOutputTypeDef(
+    _RequiredAddAttributesActivityOutputTypeDef, _OptionalAddAttributesActivityOutputTypeDef
+):
+    pass
+
 _RequiredAddAttributesActivityTypeDef = TypedDict(
     "_RequiredAddAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
 )
@@ -188,39 +228,41 @@
     "_OptionalAddAttributesActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class AddAttributesActivityTypeDef(
     _RequiredAddAttributesActivityTypeDef, _OptionalAddAttributesActivityTypeDef
 ):
     pass
 
-
 BatchPutMessageErrorEntryTypeDef = TypedDict(
     "BatchPutMessageErrorEntryTypeDef",
     {
         "messageId": str,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-MessageTypeDef = TypedDict(
-    "MessageTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "messageId": str,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelPipelineReprocessingRequestRequestTypeDef = TypedDict(
     "CancelPipelineReprocessingRequestRequestTypeDef",
     {
         "pipelineName": str,
         "reprocessingId": str,
     },
 )
@@ -236,19 +278,17 @@
     "_OptionalChannelActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class ChannelActivityTypeDef(_RequiredChannelActivityTypeDef, _OptionalChannelActivityTypeDef):
     pass
 
-
 ChannelMessagesTypeDef = TypedDict(
     "ChannelMessagesTypeDef",
     {
         "s3Paths": Sequence[str],
     },
     total=False,
 )
@@ -258,24 +298,14 @@
     {
         "estimatedSizeInBytes": float,
         "estimatedOn": datetime,
     },
     total=False,
 )
 
-CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
-    "CustomerManagedChannelS3StorageSummaryTypeDef",
-    {
-        "bucket": str,
-        "keyPrefix": str,
-        "roleArn": str,
-    },
-    total=False,
-)
-
 _RequiredCustomerManagedChannelS3StorageTypeDef = TypedDict(
     "_RequiredCustomerManagedChannelS3StorageTypeDef",
     {
         "bucket": str,
         "roleArn": str,
     },
 )
@@ -283,20 +313,28 @@
     "_OptionalCustomerManagedChannelS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
-
 class CustomerManagedChannelS3StorageTypeDef(
     _RequiredCustomerManagedChannelS3StorageTypeDef, _OptionalCustomerManagedChannelS3StorageTypeDef
 ):
     pass
 
+CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
+    "CustomerManagedChannelS3StorageSummaryTypeDef",
+    {
+        "bucket": str,
+        "keyPrefix": str,
+        "roleArn": str,
+    },
+    total=False,
+)
 
 RetentionPeriodTypeDef = TypedDict(
     "RetentionPeriodTypeDef",
     {
         "unlimited": bool,
         "numberOfDays": int,
     },
@@ -337,48 +375,29 @@
     "_OptionalCreateDatasetContentRequestRequestTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
-
 class CreateDatasetContentRequestRequestTypeDef(
     _RequiredCreateDatasetContentRequestRequestTypeDef,
     _OptionalCreateDatasetContentRequestRequestTypeDef,
 ):
     pass
 
-
-CreateDatasetContentResponseTypeDef = TypedDict(
-    "CreateDatasetContentResponseTypeDef",
-    {
-        "versionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VersioningConfigurationTypeDef = TypedDict(
     "VersioningConfigurationTypeDef",
     {
         "unlimited": bool,
         "maxVersions": int,
     },
     total=False,
 )
 
-CreatePipelineResponseTypeDef = TypedDict(
-    "CreatePipelineResponseTypeDef",
-    {
-        "pipelineName": str,
-        "pipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomerManagedDatastoreS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
@@ -396,22 +415,20 @@
     "_OptionalCustomerManagedDatastoreS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
-
 class CustomerManagedDatastoreS3StorageTypeDef(
     _RequiredCustomerManagedDatastoreS3StorageTypeDef,
     _OptionalCustomerManagedDatastoreS3StorageTypeDef,
 ):
     pass
 
-
 DatasetActionSummaryTypeDef = TypedDict(
     "DatasetActionSummaryTypeDef",
     {
         "actionName": str,
         "actionType": DatasetActionTypeType,
     },
     total=False,
@@ -492,22 +509,20 @@
     "_OptionalIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
-
 class IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef(
     _RequiredIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
     _OptionalIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
 ):
     pass
 
-
 PartitionTypeDef = TypedDict(
     "PartitionTypeDef",
     {
         "attributeName": str,
     },
 )
 
@@ -521,21 +536,19 @@
     "_OptionalTimestampPartitionTypeDef",
     {
         "timestampFormat": str,
     },
     total=False,
 )
 
-
 class TimestampPartitionTypeDef(
     _RequiredTimestampPartitionTypeDef, _OptionalTimestampPartitionTypeDef
 ):
     pass
 
-
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 
@@ -549,22 +562,20 @@
     "_OptionalDeleteDatasetContentRequestRequestTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
-
 class DeleteDatasetContentRequestRequestTypeDef(
     _RequiredDeleteDatasetContentRequestRequestTypeDef,
     _OptionalDeleteDatasetContentRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 
@@ -607,21 +618,19 @@
     "_OptionalDescribeChannelRequestRequestTypeDef",
     {
         "includeStatistics": bool,
     },
     total=False,
 )
 
-
 class DescribeChannelRequestRequestTypeDef(
     _RequiredDescribeChannelRequestRequestTypeDef, _OptionalDescribeChannelRequestRequestTypeDef
 ):
     pass
 
-
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 
@@ -635,21 +644,19 @@
     "_OptionalDescribeDatastoreRequestRequestTypeDef",
     {
         "includeStatistics": bool,
     },
     total=False,
 )
 
-
 class DescribeDatastoreRequestRequestTypeDef(
     _RequiredDescribeDatastoreRequestRequestTypeDef, _OptionalDescribeDatastoreRequestRequestTypeDef
 ):
     pass
 
-
 LoggingOptionsTypeDef = TypedDict(
     "LoggingOptionsTypeDef",
     {
         "roleArn": str,
         "level": Literal["ERROR"],
         "enabled": bool,
     },
@@ -675,21 +682,19 @@
     "_OptionalDeviceRegistryEnrichActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class DeviceRegistryEnrichActivityTypeDef(
     _RequiredDeviceRegistryEnrichActivityTypeDef, _OptionalDeviceRegistryEnrichActivityTypeDef
 ):
     pass
 
-
 _RequiredDeviceShadowEnrichActivityTypeDef = TypedDict(
     "_RequiredDeviceShadowEnrichActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "thingName": str,
         "roleArn": str,
@@ -699,28 +704,19 @@
     "_OptionalDeviceShadowEnrichActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class DeviceShadowEnrichActivityTypeDef(
     _RequiredDeviceShadowEnrichActivityTypeDef, _OptionalDeviceShadowEnrichActivityTypeDef
 ):
     pass
 
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFilterActivityTypeDef = TypedDict(
     "_RequiredFilterActivityTypeDef",
     {
         "name": str,
         "filter": str,
     },
 )
@@ -728,40 +724,36 @@
     "_OptionalFilterActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class FilterActivityTypeDef(_RequiredFilterActivityTypeDef, _OptionalFilterActivityTypeDef):
     pass
 
-
 _RequiredGetDatasetContentRequestRequestTypeDef = TypedDict(
     "_RequiredGetDatasetContentRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 _OptionalGetDatasetContentRequestRequestTypeDef = TypedDict(
     "_OptionalGetDatasetContentRequestRequestTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
-
 class GetDatasetContentRequestRequestTypeDef(
     _RequiredGetDatasetContentRequestRequestTypeDef, _OptionalGetDatasetContentRequestRequestTypeDef
 ):
     pass
 
-
 GlueConfigurationTypeDef = TypedDict(
     "GlueConfigurationTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
@@ -778,127 +770,55 @@
     "_OptionalLambdaActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class LambdaActivityTypeDef(_RequiredLambdaActivityTypeDef, _OptionalLambdaActivityTypeDef):
     pass
 
-
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
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
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    {
-        "datasetName": str,
-    },
-)
-_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    {
-        "scheduledOnOrAfter": Union[datetime, str],
-        "scheduledBefore": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
-    _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-    _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDatasetContentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDatasetContentsRequestRequestTypeDef",
-    {
-        "datasetName": str,
-    },
-)
-_OptionalListDatasetContentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDatasetContentsRequestRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-        "scheduledOnOrAfter": Union[datetime, str],
-        "scheduledBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class ListDatasetContentsRequestRequestTypeDef(
-    _RequiredListDatasetContentsRequestRequestTypeDef,
-    _OptionalListDatasetContentsRequestRequestTypeDef,
-):
-    pass
-
-
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatastoresRequestRequestTypeDef = TypedDict(
     "ListDatastoresRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesRequestRequestTypeDef = TypedDict(
     "ListPipelinesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -923,36 +843,64 @@
     "_OptionalMathActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class MathActivityTypeDef(_RequiredMathActivityTypeDef, _OptionalMathActivityTypeDef):
     pass
 
-
 OutputFileUriValueTypeDef = TypedDict(
     "OutputFileUriValueTypeDef",
     {
         "fileName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredRemoveAttributesActivityOutputTypeDef = TypedDict(
+    "_RequiredRemoveAttributesActivityOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "name": str,
+        "attributes": List[str],
+    },
+)
+_OptionalRemoveAttributesActivityOutputTypeDef = TypedDict(
+    "_OptionalRemoveAttributesActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+class RemoveAttributesActivityOutputTypeDef(
+    _RequiredRemoveAttributesActivityOutputTypeDef, _OptionalRemoveAttributesActivityOutputTypeDef
+):
+    pass
+
+_RequiredSelectAttributesActivityOutputTypeDef = TypedDict(
+    "_RequiredSelectAttributesActivityOutputTypeDef",
+    {
+        "name": str,
+        "attributes": List[str],
+    },
+)
+_OptionalSelectAttributesActivityOutputTypeDef = TypedDict(
+    "_OptionalSelectAttributesActivityOutputTypeDef",
+    {
+        "next": str,
     },
     total=False,
 )
 
+class SelectAttributesActivityOutputTypeDef(
+    _RequiredSelectAttributesActivityOutputTypeDef, _OptionalSelectAttributesActivityOutputTypeDef
+):
+    pass
+
 _RequiredRemoveAttributesActivityTypeDef = TypedDict(
     "_RequiredRemoveAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -960,21 +908,19 @@
     "_OptionalRemoveAttributesActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class RemoveAttributesActivityTypeDef(
     _RequiredRemoveAttributesActivityTypeDef, _OptionalRemoveAttributesActivityTypeDef
 ):
     pass
 
-
 _RequiredSelectAttributesActivityTypeDef = TypedDict(
     "_RequiredSelectAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -982,138 +928,102 @@
     "_OptionalSelectAttributesActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
-
 class SelectAttributesActivityTypeDef(
     _RequiredSelectAttributesActivityTypeDef, _OptionalSelectAttributesActivityTypeDef
 ):
     pass
 
-
 ReprocessingSummaryTypeDef = TypedDict(
     "ReprocessingSummaryTypeDef",
     {
         "id": str,
         "status": ReprocessingStatusType,
         "creationTime": datetime,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
-RunPipelineActivityResponseTypeDef = TypedDict(
-    "RunPipelineActivityResponseTypeDef",
+BatchPutMessageResponseTypeDef = TypedDict(
+    "BatchPutMessageResponseTypeDef",
     {
-        "payloads": List[bytes],
-        "logResult": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSampleChannelDataRequestRequestTypeDef = TypedDict(
-    "_RequiredSampleChannelDataRequestRequestTypeDef",
-    {
-        "channelName": str,
-    },
-)
-_OptionalSampleChannelDataRequestRequestTypeDef = TypedDict(
-    "_OptionalSampleChannelDataRequestRequestTypeDef",
+CreateDatasetContentResponseTypeDef = TypedDict(
+    "CreateDatasetContentResponseTypeDef",
     {
-        "maxMessages": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "versionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class SampleChannelDataRequestRequestTypeDef(
-    _RequiredSampleChannelDataRequestRequestTypeDef, _OptionalSampleChannelDataRequestRequestTypeDef
-):
-    pass
-
-
-SampleChannelDataResponseTypeDef = TypedDict(
-    "SampleChannelDataResponseTypeDef",
+CreatePipelineResponseTypeDef = TypedDict(
+    "CreatePipelineResponseTypeDef",
     {
-        "payloads": List[bytes],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "pipelineName": str,
+        "pipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartPipelineReprocessingResponseTypeDef = TypedDict(
-    "StartPipelineReprocessingResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "reprocessingId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+RunPipelineActivityResponseTypeDef = TypedDict(
+    "RunPipelineActivityResponseTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "payloads": List[bytes],
+        "logResult": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutMessageResponseTypeDef = TypedDict(
-    "BatchPutMessageResponseTypeDef",
+SampleChannelDataResponseTypeDef = TypedDict(
+    "SampleChannelDataResponseTypeDef",
     {
-        "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "payloads": List[bytes],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutMessageRequestRequestTypeDef = TypedDict(
-    "BatchPutMessageRequestRequestTypeDef",
+StartPipelineReprocessingResponseTypeDef = TypedDict(
+    "StartPipelineReprocessingResponseTypeDef",
     {
-        "channelName": str,
-        "messages": Sequence[MessageTypeDef],
+        "reprocessingId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPipelineReprocessingRequestRequestTypeDef",
-    {
-        "pipelineName": str,
-    },
-)
-_OptionalStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPipelineReprocessingRequestRequestTypeDef",
+MessageTypeDef = TypedDict(
+    "MessageTypeDef",
     {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "channelMessages": ChannelMessagesTypeDef,
+        "messageId": str,
+        "payload": BlobTypeDef,
     },
-    total=False,
 )
 
-
-class StartPipelineReprocessingRequestRequestTypeDef(
-    _RequiredStartPipelineReprocessingRequestRequestTypeDef,
-    _OptionalStartPipelineReprocessingRequestRequestTypeDef,
-):
-    pass
-
-
 ChannelStatisticsTypeDef = TypedDict(
     "ChannelStatisticsTypeDef",
     {
         "size": EstimatedResourceSizeTypeDef,
     },
     total=False,
 )
@@ -1122,75 +1032,92 @@
     "DatastoreStatisticsTypeDef",
     {
         "size": EstimatedResourceSizeTypeDef,
     },
     total=False,
 )
 
-ChannelStorageSummaryTypeDef = TypedDict(
-    "ChannelStorageSummaryTypeDef",
+ChannelStorageOutputTypeDef = TypedDict(
+    "ChannelStorageOutputTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
+        "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
     },
     total=False,
 )
 
 ChannelStorageTypeDef = TypedDict(
     "ChannelStorageTypeDef",
     {
         "serviceManagedS3": Mapping[str, Any],
         "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
     },
     total=False,
 )
 
+ChannelStorageSummaryTypeDef = TypedDict(
+    "ChannelStorageSummaryTypeDef",
+    {
+        "serviceManagedS3": Dict[str, Any],
+        "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
+    },
+    total=False,
+)
+
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channelName": str,
         "channelArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "datasetName": str,
         "datasetArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDatastoreResponseTypeDef = TypedDict(
     "CreateDatastoreResponseTypeDef",
     {
         "datastoreName": str,
         "datastoreArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+SchemaDefinitionOutputTypeDef = TypedDict(
+    "SchemaDefinitionOutputTypeDef",
+    {
+        "columns": List[ColumnTypeDef],
+    },
+    total=False,
+)
+
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "columns": Sequence[ColumnTypeDef],
     },
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1212,15 +1139,15 @@
 
 GetDatasetContentResponseTypeDef = TypedDict(
     "GetDatasetContentResponseTypeDef",
     {
         "entries": List[DatasetEntryTypeDef],
         "timestamp": datetime,
         "status": DatasetContentStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetTriggerTypeDef = TypedDict(
     "DatasetTriggerTypeDef",
     {
         "schedule": ScheduleTypeDef,
@@ -1269,15 +1196,15 @@
     total=False,
 )
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
@@ -1296,20 +1223,138 @@
     "_OptionalS3DestinationConfigurationTypeDef",
     {
         "glueConfiguration": GlueConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class S3DestinationConfigurationTypeDef(
     _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    {
+        "datasetName": str,
+    },
+)
+_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    {
+        "scheduledOnOrAfter": TimestampTypeDef,
+        "scheduledBefore": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
+    _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+):
+    pass
+
+_RequiredListDatasetContentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDatasetContentsRequestRequestTypeDef",
+    {
+        "datasetName": str,
+    },
+)
+_OptionalListDatasetContentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDatasetContentsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+        "scheduledOnOrAfter": TimestampTypeDef,
+        "scheduledBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class ListDatasetContentsRequestRequestTypeDef(
+    _RequiredListDatasetContentsRequestRequestTypeDef,
+    _OptionalListDatasetContentsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSampleChannelDataRequestRequestTypeDef = TypedDict(
+    "_RequiredSampleChannelDataRequestRequestTypeDef",
+    {
+        "channelName": str,
+    },
+)
+_OptionalSampleChannelDataRequestRequestTypeDef = TypedDict(
+    "_OptionalSampleChannelDataRequestRequestTypeDef",
+    {
+        "maxMessages": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class SampleChannelDataRequestRequestTypeDef(
+    _RequiredSampleChannelDataRequestRequestTypeDef, _OptionalSampleChannelDataRequestRequestTypeDef
+):
+    pass
+
+_RequiredStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPipelineReprocessingRequestRequestTypeDef",
+    {
+        "pipelineName": str,
+    },
+)
+_OptionalStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPipelineReprocessingRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "channelMessages": ChannelMessagesTypeDef,
+    },
+    total=False,
+)
+
+class StartPipelineReprocessingRequestRequestTypeDef(
+    _RequiredStartPipelineReprocessingRequestRequestTypeDef,
+    _OptionalStartPipelineReprocessingRequestRequestTypeDef,
+):
+    pass
 
 _RequiredVariableTypeDef = TypedDict(
     "_RequiredVariableTypeDef",
     {
         "name": str,
     },
 )
@@ -1320,18 +1365,33 @@
         "doubleValue": float,
         "datasetContentVersionValue": DatasetContentVersionValueTypeDef,
         "outputFileUriValue": OutputFileUriValueTypeDef,
     },
     total=False,
 )
 
-
 class VariableTypeDef(_RequiredVariableTypeDef, _OptionalVariableTypeDef):
     pass
 
+PipelineActivityOutputTypeDef = TypedDict(
+    "PipelineActivityOutputTypeDef",
+    {
+        "channel": ChannelActivityTypeDef,
+        "lambda": LambdaActivityTypeDef,
+        "datastore": DatastoreActivityTypeDef,
+        "addAttributes": AddAttributesActivityOutputTypeDef,
+        "removeAttributes": RemoveAttributesActivityOutputTypeDef,
+        "selectAttributes": SelectAttributesActivityOutputTypeDef,
+        "filter": FilterActivityTypeDef,
+        "math": MathActivityTypeDef,
+        "deviceRegistryEnrich": DeviceRegistryEnrichActivityTypeDef,
+        "deviceShadowEnrich": DeviceShadowEnrichActivityTypeDef,
+    },
+    total=False,
+)
 
 PipelineActivityTypeDef = TypedDict(
     "PipelineActivityTypeDef",
     {
         "channel": ChannelActivityTypeDef,
         "lambda": LambdaActivityTypeDef,
         "datastore": DatastoreActivityTypeDef,
@@ -1353,42 +1413,38 @@
         "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
         "creationTime": datetime,
         "lastUpdateTime": datetime,
     },
     total=False,
 )
 
-ChannelSummaryTypeDef = TypedDict(
-    "ChannelSummaryTypeDef",
+BatchPutMessageRequestRequestTypeDef = TypedDict(
+    "BatchPutMessageRequestRequestTypeDef",
     {
         "channelName": str,
-        "channelStorage": ChannelStorageSummaryTypeDef,
-        "status": ChannelStatusType,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "lastMessageArrivalTime": datetime,
+        "messages": Sequence[MessageTypeDef],
     },
-    total=False,
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "name": str,
-        "storage": ChannelStorageTypeDef,
+        "storage": ChannelStorageOutputTypeDef,
         "arn": str,
         "status": ChannelStatusType,
         "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
     },
     total=False,
 )
 
+ChannelStorageUnionTypeDef = Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef]
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalCreateChannelRequestRequestTypeDef = TypedDict(
@@ -1397,21 +1453,19 @@
         "channelStorage": ChannelStorageTypeDef,
         "retentionPeriod": RetentionPeriodTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
@@ -1419,35 +1473,54 @@
     {
         "channelStorage": ChannelStorageTypeDef,
         "retentionPeriod": RetentionPeriodTypeDef,
     },
     total=False,
 )
 
-
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+ChannelSummaryTypeDef = TypedDict(
+    "ChannelSummaryTypeDef",
+    {
+        "channelName": str,
+        "channelStorage": ChannelStorageSummaryTypeDef,
+        "status": ChannelStatusType,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "lastMessageArrivalTime": datetime,
+    },
+    total=False,
+)
+
+ParquetConfigurationOutputTypeDef = TypedDict(
+    "ParquetConfigurationOutputTypeDef",
+    {
+        "schemaDefinition": SchemaDefinitionOutputTypeDef,
+    },
+    total=False,
+)
 
 ParquetConfigurationTypeDef = TypedDict(
     "ParquetConfigurationTypeDef",
     {
         "schemaDefinition": SchemaDefinitionTypeDef,
     },
     total=False,
 )
 
 ListDatasetContentsResponseTypeDef = TypedDict(
     "ListDatasetContentsResponseTypeDef",
     {
         "datasetContentSummaries": List[DatasetContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetSummaryTypeDef = TypedDict(
     "DatasetSummaryTypeDef",
     {
         "datasetName": str,
@@ -1466,24 +1539,42 @@
         "serviceManagedS3": Dict[str, Any],
         "customerManagedS3": CustomerManagedDatastoreS3StorageSummaryTypeDef,
         "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     },
     total=False,
 )
 
+DatastoreStorageOutputTypeDef = TypedDict(
+    "DatastoreStorageOutputTypeDef",
+    {
+        "serviceManagedS3": Dict[str, Any],
+        "customerManagedS3": CustomerManagedDatastoreS3StorageTypeDef,
+        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageTypeDef,
+    },
+    total=False,
+)
+
 DatastoreStorageTypeDef = TypedDict(
     "DatastoreStorageTypeDef",
     {
         "serviceManagedS3": Mapping[str, Any],
         "customerManagedS3": CustomerManagedDatastoreS3StorageTypeDef,
         "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     },
     total=False,
 )
 
+DatastorePartitionsOutputTypeDef = TypedDict(
+    "DatastorePartitionsOutputTypeDef",
+    {
+        "partitions": List[DatastorePartitionTypeDef],
+    },
+    total=False,
+)
+
 DatastorePartitionsTypeDef = TypedDict(
     "DatastorePartitionsTypeDef",
     {
         "partitions": Sequence[DatastorePartitionTypeDef],
     },
     total=False,
 )
@@ -1498,18 +1589,35 @@
     "_OptionalLateDataRuleTypeDef",
     {
         "ruleName": str,
     },
     total=False,
 )
 
-
 class LateDataRuleTypeDef(_RequiredLateDataRuleTypeDef, _OptionalLateDataRuleTypeDef):
     pass
 
+_RequiredSqlQueryDatasetActionOutputTypeDef = TypedDict(
+    "_RequiredSqlQueryDatasetActionOutputTypeDef",
+    {
+        "sqlQuery": str,
+    },
+)
+_OptionalSqlQueryDatasetActionOutputTypeDef = TypedDict(
+    "_OptionalSqlQueryDatasetActionOutputTypeDef",
+    {
+        "filters": List[QueryFilterTypeDef],
+    },
+    total=False,
+)
+
+class SqlQueryDatasetActionOutputTypeDef(
+    _RequiredSqlQueryDatasetActionOutputTypeDef, _OptionalSqlQueryDatasetActionOutputTypeDef
+):
+    pass
 
 _RequiredSqlQueryDatasetActionTypeDef = TypedDict(
     "_RequiredSqlQueryDatasetActionTypeDef",
     {
         "sqlQuery": str,
     },
 )
@@ -1517,129 +1625,126 @@
     "_OptionalSqlQueryDatasetActionTypeDef",
     {
         "filters": Sequence[QueryFilterTypeDef],
     },
     total=False,
 )
 
-
 class SqlQueryDatasetActionTypeDef(
     _RequiredSqlQueryDatasetActionTypeDef, _OptionalSqlQueryDatasetActionTypeDef
 ):
     pass
 
-
 DatasetContentDeliveryDestinationTypeDef = TypedDict(
     "DatasetContentDeliveryDestinationTypeDef",
     {
         "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationTypeDef,
         "s3DestinationConfiguration": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredContainerDatasetActionTypeDef = TypedDict(
-    "_RequiredContainerDatasetActionTypeDef",
+_RequiredContainerDatasetActionOutputTypeDef = TypedDict(
+    "_RequiredContainerDatasetActionOutputTypeDef",
     {
         "image": str,
         "executionRoleArn": str,
         "resourceConfiguration": ResourceConfigurationTypeDef,
     },
 )
-_OptionalContainerDatasetActionTypeDef = TypedDict(
-    "_OptionalContainerDatasetActionTypeDef",
+_OptionalContainerDatasetActionOutputTypeDef = TypedDict(
+    "_OptionalContainerDatasetActionOutputTypeDef",
     {
-        "variables": Sequence[VariableTypeDef],
+        "variables": List[VariableTypeDef],
     },
     total=False,
 )
 
-
-class ContainerDatasetActionTypeDef(
-    _RequiredContainerDatasetActionTypeDef, _OptionalContainerDatasetActionTypeDef
+class ContainerDatasetActionOutputTypeDef(
+    _RequiredContainerDatasetActionOutputTypeDef, _OptionalContainerDatasetActionOutputTypeDef
 ):
     pass
 
-
-_RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePipelineRequestRequestTypeDef",
+_RequiredContainerDatasetActionTypeDef = TypedDict(
+    "_RequiredContainerDatasetActionTypeDef",
     {
-        "pipelineName": str,
-        "pipelineActivities": Sequence[PipelineActivityTypeDef],
+        "image": str,
+        "executionRoleArn": str,
+        "resourceConfiguration": ResourceConfigurationTypeDef,
     },
 )
-_OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePipelineRequestRequestTypeDef",
+_OptionalContainerDatasetActionTypeDef = TypedDict(
+    "_OptionalContainerDatasetActionTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "variables": Sequence[VariableTypeDef],
     },
     total=False,
 )
 
-
-class CreatePipelineRequestRequestTypeDef(
-    _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
+class ContainerDatasetActionTypeDef(
+    _RequiredContainerDatasetActionTypeDef, _OptionalContainerDatasetActionTypeDef
 ):
     pass
 
-
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "name": str,
         "arn": str,
-        "activities": List[PipelineActivityTypeDef],
+        "activities": List[PipelineActivityOutputTypeDef],
         "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
         "creationTime": datetime,
         "lastUpdateTime": datetime,
     },
     total=False,
 )
 
+PipelineActivityUnionTypeDef = Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
 RunPipelineActivityRequestRequestTypeDef = TypedDict(
     "RunPipelineActivityRequestRequestTypeDef",
     {
         "pipelineActivity": PipelineActivityTypeDef,
-        "payloads": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-    },
-)
-
-UpdatePipelineRequestRequestTypeDef = TypedDict(
-    "UpdatePipelineRequestRequestTypeDef",
-    {
-        "pipelineName": str,
-        "pipelineActivities": Sequence[PipelineActivityTypeDef],
+        "payloads": Sequence[BlobTypeDef],
     },
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "pipelineSummaries": List[PipelineSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeChannelResponseTypeDef = TypedDict(
+    "DescribeChannelResponseTypeDef",
+    {
+        "channel": ChannelTypeDef,
+        "statistics": ChannelStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channelSummaries": List[ChannelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeChannelResponseTypeDef = TypedDict(
-    "DescribeChannelResponseTypeDef",
+FileFormatConfigurationOutputTypeDef = TypedDict(
+    "FileFormatConfigurationOutputTypeDef",
     {
-        "channel": ChannelTypeDef,
-        "statistics": ChannelStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "jsonConfiguration": Dict[str, Any],
+        "parquetConfiguration": ParquetConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 FileFormatConfigurationTypeDef = TypedDict(
     "FileFormatConfigurationTypeDef",
     {
         "jsonConfiguration": Mapping[str, Any],
         "parquetConfiguration": ParquetConfigurationTypeDef,
@@ -1648,53 +1753,65 @@
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "datasetSummaries": List[DatasetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DatastoreStorageUnionTypeDef = Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef]
 DatastoreSummaryTypeDef = TypedDict(
     "DatastoreSummaryTypeDef",
     {
         "datastoreName": str,
         "datastoreStorage": DatastoreStorageSummaryTypeDef,
         "status": DatastoreStatusType,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
         "fileFormatType": FileFormatTypeType,
-        "datastorePartitions": DatastorePartitionsTypeDef,
+        "datastorePartitions": DatastorePartitionsOutputTypeDef,
     },
     total=False,
 )
 
+DatastorePartitionsUnionTypeDef = Union[
+    DatastorePartitionsTypeDef, DatastorePartitionsOutputTypeDef
+]
 _RequiredDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_RequiredDatasetContentDeliveryRuleTypeDef",
     {
         "destination": DatasetContentDeliveryDestinationTypeDef,
     },
 )
 _OptionalDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_OptionalDatasetContentDeliveryRuleTypeDef",
     {
         "entryName": str,
     },
     total=False,
 )
 
-
 class DatasetContentDeliveryRuleTypeDef(
     _RequiredDatasetContentDeliveryRuleTypeDef, _OptionalDatasetContentDeliveryRuleTypeDef
 ):
     pass
 
+DatasetActionOutputTypeDef = TypedDict(
+    "DatasetActionOutputTypeDef",
+    {
+        "actionName": str,
+        "queryAction": SqlQueryDatasetActionOutputTypeDef,
+        "containerAction": ContainerDatasetActionOutputTypeDef,
+    },
+    total=False,
+)
 
 DatasetActionTypeDef = TypedDict(
     "DatasetActionTypeDef",
     {
         "actionName": str,
         "queryAction": SqlQueryDatasetActionTypeDef,
         "containerAction": ContainerDatasetActionTypeDef,
@@ -1702,60 +1819,89 @@
     total=False,
 )
 
 DescribePipelineResponseTypeDef = TypedDict(
     "DescribePipelineResponseTypeDef",
     {
         "pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatastoreRequestRequestTypeDef",
+_RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePipelineRequestRequestTypeDef",
     {
-        "datastoreName": str,
+        "pipelineName": str,
+        "pipelineActivities": Sequence[PipelineActivityUnionTypeDef],
     },
 )
-_OptionalCreateDatastoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatastoreRequestRequestTypeDef",
+_OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePipelineRequestRequestTypeDef",
     {
-        "datastoreStorage": DatastoreStorageTypeDef,
-        "retentionPeriod": RetentionPeriodTypeDef,
         "tags": Sequence[TagTypeDef],
-        "fileFormatConfiguration": FileFormatConfigurationTypeDef,
-        "datastorePartitions": DatastorePartitionsTypeDef,
     },
     total=False,
 )
 
-
-class CreateDatastoreRequestRequestTypeDef(
-    _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
+class CreatePipelineRequestRequestTypeDef(
+    _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
+UpdatePipelineRequestRequestTypeDef = TypedDict(
+    "UpdatePipelineRequestRequestTypeDef",
+    {
+        "pipelineName": str,
+        "pipelineActivities": Sequence[PipelineActivityUnionTypeDef],
+    },
+)
 
 DatastoreTypeDef = TypedDict(
     "DatastoreTypeDef",
     {
         "name": str,
-        "storage": DatastoreStorageTypeDef,
+        "storage": DatastoreStorageOutputTypeDef,
         "arn": str,
         "status": DatastoreStatusType,
         "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
+        "fileFormatConfiguration": FileFormatConfigurationOutputTypeDef,
+        "datastorePartitions": DatastorePartitionsOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatastoreRequestRequestTypeDef",
+    {
+        "datastoreName": str,
+    },
+)
+_OptionalCreateDatastoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatastoreRequestRequestTypeDef",
+    {
+        "datastoreStorage": DatastoreStorageTypeDef,
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "tags": Sequence[TagTypeDef],
         "fileFormatConfiguration": FileFormatConfigurationTypeDef,
         "datastorePartitions": DatastorePartitionsTypeDef,
     },
     total=False,
 )
 
+class CreateDatastoreRequestRequestTypeDef(
+    _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
+):
+    pass
+
+FileFormatConfigurationUnionTypeDef = Union[
+    FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
+]
 _RequiredUpdateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatastoreRequestRequestTypeDef",
     {
         "datastoreName": str,
     },
 )
 _OptionalUpdateDatastoreRequestRequestTypeDef = TypedDict(
@@ -1764,35 +1910,69 @@
         "retentionPeriod": RetentionPeriodTypeDef,
         "datastoreStorage": DatastoreStorageTypeDef,
         "fileFormatConfiguration": FileFormatConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDatastoreRequestRequestTypeDef(
     _RequiredUpdateDatastoreRequestRequestTypeDef, _OptionalUpdateDatastoreRequestRequestTypeDef
 ):
     pass
 
-
 ListDatastoresResponseTypeDef = TypedDict(
     "ListDatastoresResponseTypeDef",
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DatasetTypeDef = TypedDict(
+    "DatasetTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "actions": List[DatasetActionOutputTypeDef],
+        "triggers": List[DatasetTriggerTypeDef],
+        "contentDeliveryRules": List[DatasetContentDeliveryRuleTypeDef],
+        "status": DatasetStatusType,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "versioningConfiguration": VersioningConfigurationTypeDef,
+        "lateDataRules": List[LateDataRuleTypeDef],
+    },
+    total=False,
+)
+
+DatasetActionUnionTypeDef = Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]
+DescribeDatastoreResponseTypeDef = TypedDict(
+    "DescribeDatastoreResponseTypeDef",
+    {
+        "datastore": DatastoreTypeDef,
+        "statistics": DatastoreStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "dataset": DatasetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[DatasetActionTypeDef],
+        "actions": Sequence[DatasetActionUnionTypeDef],
     },
 )
 _OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
@@ -1800,74 +1980,35 @@
         "versioningConfiguration": VersioningConfigurationTypeDef,
         "tags": Sequence[TagTypeDef],
         "lateDataRules": Sequence[LateDataRuleTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-
-DatasetTypeDef = TypedDict(
-    "DatasetTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "actions": List[DatasetActionTypeDef],
-        "triggers": List[DatasetTriggerTypeDef],
-        "contentDeliveryRules": List[DatasetContentDeliveryRuleTypeDef],
-        "status": DatasetStatusType,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "retentionPeriod": RetentionPeriodTypeDef,
-        "versioningConfiguration": VersioningConfigurationTypeDef,
-        "lateDataRules": List[LateDataRuleTypeDef],
-    },
-    total=False,
-)
-
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[DatasetActionTypeDef],
+        "actions": Sequence[DatasetActionUnionTypeDef],
     },
 )
 _OptionalUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
         "retentionPeriod": RetentionPeriodTypeDef,
         "versioningConfiguration": VersioningConfigurationTypeDef,
         "lateDataRules": Sequence[LateDataRuleTypeDef],
     },
     total=False,
 )
 
-
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
-
-
-DescribeDatastoreResponseTypeDef = TypedDict(
-    "DescribeDatastoreResponseTypeDef",
-    {
-        "datastore": DatastoreTypeDef,
-        "statistics": DatastoreStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "dataset": DatasetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics/type_defs.pyi` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotanalytics service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_iotanalytics.type_defs import AddAttributesActivityTypeDef
+    from types_aiobotocore_iotanalytics.type_defs import AddAttributesActivityOutputTypeDef
 
-    data: AddAttributesActivityTypeDef = {...}
+    data: AddAttributesActivityOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -33,32 +33,33 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AddAttributesActivityOutputTypeDef",
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
-    "MessageTypeDef",
+    "ResponseMetadataTypeDef",
+    "BlobTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
     "ChannelActivityTypeDef",
     "ChannelMessagesTypeDef",
     "EstimatedResourceSizeTypeDef",
-    "CustomerManagedChannelS3StorageSummaryTypeDef",
     "CustomerManagedChannelS3StorageTypeDef",
+    "CustomerManagedChannelS3StorageSummaryTypeDef",
     "RetentionPeriodTypeDef",
     "ColumnTypeDef",
     "ResourceConfigurationTypeDef",
     "TagTypeDef",
     "CreateDatasetContentRequestRequestTypeDef",
-    "CreateDatasetContentResponseTypeDef",
     "VersioningConfigurationTypeDef",
-    "CreatePipelineResponseTypeDef",
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     "CustomerManagedDatastoreS3StorageTypeDef",
     "DatasetActionSummaryTypeDef",
     "IotEventsDestinationConfigurationTypeDef",
     "DatasetContentStatusTypeDef",
     "DatasetContentVersionValueTypeDef",
     "DatasetEntryTypeDef",
@@ -79,107 +80,150 @@
     "DescribeChannelRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeDatastoreRequestRequestTypeDef",
     "LoggingOptionsTypeDef",
     "DescribePipelineRequestRequestTypeDef",
     "DeviceRegistryEnrichActivityTypeDef",
     "DeviceShadowEnrichActivityTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FilterActivityTypeDef",
     "GetDatasetContentRequestRequestTypeDef",
     "GlueConfigurationTypeDef",
     "LambdaActivityTypeDef",
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChannelsRequestRequestTypeDef",
-    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    "ListDatasetContentsRequestRequestTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "TimestampTypeDef",
     "ListDatasetsRequestRequestTypeDef",
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListDatastoresRequestRequestTypeDef",
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MathActivityTypeDef",
     "OutputFileUriValueTypeDef",
-    "PaginatorConfigTypeDef",
+    "RemoveAttributesActivityOutputTypeDef",
+    "SelectAttributesActivityOutputTypeDef",
     "RemoveAttributesActivityTypeDef",
     "SelectAttributesActivityTypeDef",
     "ReprocessingSummaryTypeDef",
-    "ResponseMetadataTypeDef",
+    "UntagResourceRequestRequestTypeDef",
+    "BatchPutMessageResponseTypeDef",
+    "CreateDatasetContentResponseTypeDef",
+    "CreatePipelineResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "RunPipelineActivityResponseTypeDef",
-    "SampleChannelDataRequestRequestTypeDef",
     "SampleChannelDataResponseTypeDef",
     "StartPipelineReprocessingResponseTypeDef",
-    "UntagResourceRequestRequestTypeDef",
-    "BatchPutMessageResponseTypeDef",
-    "BatchPutMessageRequestRequestTypeDef",
-    "StartPipelineReprocessingRequestRequestTypeDef",
+    "MessageTypeDef",
     "ChannelStatisticsTypeDef",
     "DatastoreStatisticsTypeDef",
-    "ChannelStorageSummaryTypeDef",
+    "ChannelStorageOutputTypeDef",
     "ChannelStorageTypeDef",
+    "ChannelStorageSummaryTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateDatastoreResponseTypeDef",
+    "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatasetContentSummaryTypeDef",
     "GetDatasetContentResponseTypeDef",
     "DatasetTriggerTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageTypeDef",
     "DatastorePartitionTypeDef",
     "LateDataRuleConfigurationTypeDef",
     "QueryFilterTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "S3DestinationConfigurationTypeDef",
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    "ListDatasetContentsRequestRequestTypeDef",
+    "SampleChannelDataRequestRequestTypeDef",
+    "StartPipelineReprocessingRequestRequestTypeDef",
     "VariableTypeDef",
+    "PipelineActivityOutputTypeDef",
     "PipelineActivityTypeDef",
     "PipelineSummaryTypeDef",
-    "ChannelSummaryTypeDef",
+    "BatchPutMessageRequestRequestTypeDef",
     "ChannelTypeDef",
+    "ChannelStorageUnionTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
+    "ChannelSummaryTypeDef",
+    "ParquetConfigurationOutputTypeDef",
     "ParquetConfigurationTypeDef",
     "ListDatasetContentsResponseTypeDef",
     "DatasetSummaryTypeDef",
     "DatastoreStorageSummaryTypeDef",
+    "DatastoreStorageOutputTypeDef",
     "DatastoreStorageTypeDef",
+    "DatastorePartitionsOutputTypeDef",
     "DatastorePartitionsTypeDef",
     "LateDataRuleTypeDef",
+    "SqlQueryDatasetActionOutputTypeDef",
     "SqlQueryDatasetActionTypeDef",
     "DatasetContentDeliveryDestinationTypeDef",
+    "ContainerDatasetActionOutputTypeDef",
     "ContainerDatasetActionTypeDef",
-    "CreatePipelineRequestRequestTypeDef",
     "PipelineTypeDef",
+    "PipelineActivityUnionTypeDef",
     "RunPipelineActivityRequestRequestTypeDef",
-    "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
-    "ListChannelsResponseTypeDef",
     "DescribeChannelResponseTypeDef",
+    "ListChannelsResponseTypeDef",
+    "FileFormatConfigurationOutputTypeDef",
     "FileFormatConfigurationTypeDef",
     "ListDatasetsResponseTypeDef",
+    "DatastoreStorageUnionTypeDef",
     "DatastoreSummaryTypeDef",
+    "DatastorePartitionsUnionTypeDef",
     "DatasetContentDeliveryRuleTypeDef",
+    "DatasetActionOutputTypeDef",
     "DatasetActionTypeDef",
     "DescribePipelineResponseTypeDef",
-    "CreateDatastoreRequestRequestTypeDef",
+    "CreatePipelineRequestRequestTypeDef",
+    "UpdatePipelineRequestRequestTypeDef",
     "DatastoreTypeDef",
+    "CreateDatastoreRequestRequestTypeDef",
+    "FileFormatConfigurationUnionTypeDef",
     "UpdateDatastoreRequestRequestTypeDef",
     "ListDatastoresResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
-    "UpdateDatasetRequestRequestTypeDef",
+    "DatasetActionUnionTypeDef",
     "DescribeDatastoreResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "UpdateDatasetRequestRequestTypeDef",
 )
 
+_RequiredAddAttributesActivityOutputTypeDef = TypedDict(
+    "_RequiredAddAttributesActivityOutputTypeDef",
+    {
+        "name": str,
+        "attributes": Dict[str, str],
+    },
+)
+_OptionalAddAttributesActivityOutputTypeDef = TypedDict(
+    "_OptionalAddAttributesActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+
+class AddAttributesActivityOutputTypeDef(
+    _RequiredAddAttributesActivityOutputTypeDef, _OptionalAddAttributesActivityOutputTypeDef
+):
+    pass
+
+
 _RequiredAddAttributesActivityTypeDef = TypedDict(
     "_RequiredAddAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
 )
@@ -187,37 +231,43 @@
     "_OptionalAddAttributesActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class AddAttributesActivityTypeDef(
     _RequiredAddAttributesActivityTypeDef, _OptionalAddAttributesActivityTypeDef
 ):
     pass
 
+
 BatchPutMessageErrorEntryTypeDef = TypedDict(
     "BatchPutMessageErrorEntryTypeDef",
     {
         "messageId": str,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
-MessageTypeDef = TypedDict(
-    "MessageTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "messageId": str,
-        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelPipelineReprocessingRequestRequestTypeDef = TypedDict(
     "CancelPipelineReprocessingRequestRequestTypeDef",
     {
         "pipelineName": str,
         "reprocessingId": str,
     },
 )
@@ -233,17 +283,19 @@
     "_OptionalChannelActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class ChannelActivityTypeDef(_RequiredChannelActivityTypeDef, _OptionalChannelActivityTypeDef):
     pass
 
+
 ChannelMessagesTypeDef = TypedDict(
     "ChannelMessagesTypeDef",
     {
         "s3Paths": Sequence[str],
     },
     total=False,
 )
@@ -253,24 +305,14 @@
     {
         "estimatedSizeInBytes": float,
         "estimatedOn": datetime,
     },
     total=False,
 )
 
-CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
-    "CustomerManagedChannelS3StorageSummaryTypeDef",
-    {
-        "bucket": str,
-        "keyPrefix": str,
-        "roleArn": str,
-    },
-    total=False,
-)
-
 _RequiredCustomerManagedChannelS3StorageTypeDef = TypedDict(
     "_RequiredCustomerManagedChannelS3StorageTypeDef",
     {
         "bucket": str,
         "roleArn": str,
     },
 )
@@ -278,19 +320,31 @@
     "_OptionalCustomerManagedChannelS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
+
 class CustomerManagedChannelS3StorageTypeDef(
     _RequiredCustomerManagedChannelS3StorageTypeDef, _OptionalCustomerManagedChannelS3StorageTypeDef
 ):
     pass
 
+
+CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
+    "CustomerManagedChannelS3StorageSummaryTypeDef",
+    {
+        "bucket": str,
+        "keyPrefix": str,
+        "roleArn": str,
+    },
+    total=False,
+)
+
 RetentionPeriodTypeDef = TypedDict(
     "RetentionPeriodTypeDef",
     {
         "unlimited": bool,
         "numberOfDays": int,
     },
     total=False,
@@ -330,46 +384,31 @@
     "_OptionalCreateDatasetContentRequestRequestTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
+
 class CreateDatasetContentRequestRequestTypeDef(
     _RequiredCreateDatasetContentRequestRequestTypeDef,
     _OptionalCreateDatasetContentRequestRequestTypeDef,
 ):
     pass
 
-CreateDatasetContentResponseTypeDef = TypedDict(
-    "CreateDatasetContentResponseTypeDef",
-    {
-        "versionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 VersioningConfigurationTypeDef = TypedDict(
     "VersioningConfigurationTypeDef",
     {
         "unlimited": bool,
         "maxVersions": int,
     },
     total=False,
 )
 
-CreatePipelineResponseTypeDef = TypedDict(
-    "CreatePipelineResponseTypeDef",
-    {
-        "pipelineName": str,
-        "pipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomerManagedDatastoreS3StorageSummaryTypeDef = TypedDict(
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
         "roleArn": str,
     },
@@ -387,20 +426,22 @@
     "_OptionalCustomerManagedDatastoreS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
+
 class CustomerManagedDatastoreS3StorageTypeDef(
     _RequiredCustomerManagedDatastoreS3StorageTypeDef,
     _OptionalCustomerManagedDatastoreS3StorageTypeDef,
 ):
     pass
 
+
 DatasetActionSummaryTypeDef = TypedDict(
     "DatasetActionSummaryTypeDef",
     {
         "actionName": str,
         "actionType": DatasetActionTypeType,
     },
     total=False,
@@ -481,20 +522,22 @@
     "_OptionalIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef",
     {
         "keyPrefix": str,
     },
     total=False,
 )
 
+
 class IotSiteWiseCustomerManagedDatastoreS3StorageTypeDef(
     _RequiredIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
     _OptionalIotSiteWiseCustomerManagedDatastoreS3StorageTypeDef,
 ):
     pass
 
+
 PartitionTypeDef = TypedDict(
     "PartitionTypeDef",
     {
         "attributeName": str,
     },
 )
 
@@ -508,19 +551,21 @@
     "_OptionalTimestampPartitionTypeDef",
     {
         "timestampFormat": str,
     },
     total=False,
 )
 
+
 class TimestampPartitionTypeDef(
     _RequiredTimestampPartitionTypeDef, _OptionalTimestampPartitionTypeDef
 ):
     pass
 
+
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 
@@ -534,20 +579,22 @@
     "_OptionalDeleteDatasetContentRequestRequestTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
+
 class DeleteDatasetContentRequestRequestTypeDef(
     _RequiredDeleteDatasetContentRequestRequestTypeDef,
     _OptionalDeleteDatasetContentRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteDatasetRequestRequestTypeDef = TypedDict(
     "DeleteDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 
@@ -590,19 +637,21 @@
     "_OptionalDescribeChannelRequestRequestTypeDef",
     {
         "includeStatistics": bool,
     },
     total=False,
 )
 
+
 class DescribeChannelRequestRequestTypeDef(
     _RequiredDescribeChannelRequestRequestTypeDef, _OptionalDescribeChannelRequestRequestTypeDef
 ):
     pass
 
+
 DescribeDatasetRequestRequestTypeDef = TypedDict(
     "DescribeDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 
@@ -616,19 +665,21 @@
     "_OptionalDescribeDatastoreRequestRequestTypeDef",
     {
         "includeStatistics": bool,
     },
     total=False,
 )
 
+
 class DescribeDatastoreRequestRequestTypeDef(
     _RequiredDescribeDatastoreRequestRequestTypeDef, _OptionalDescribeDatastoreRequestRequestTypeDef
 ):
     pass
 
+
 LoggingOptionsTypeDef = TypedDict(
     "LoggingOptionsTypeDef",
     {
         "roleArn": str,
         "level": Literal["ERROR"],
         "enabled": bool,
     },
@@ -654,19 +705,21 @@
     "_OptionalDeviceRegistryEnrichActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class DeviceRegistryEnrichActivityTypeDef(
     _RequiredDeviceRegistryEnrichActivityTypeDef, _OptionalDeviceRegistryEnrichActivityTypeDef
 ):
     pass
 
+
 _RequiredDeviceShadowEnrichActivityTypeDef = TypedDict(
     "_RequiredDeviceShadowEnrichActivityTypeDef",
     {
         "name": str,
         "attribute": str,
         "thingName": str,
         "roleArn": str,
@@ -676,25 +729,20 @@
     "_OptionalDeviceShadowEnrichActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class DeviceShadowEnrichActivityTypeDef(
     _RequiredDeviceShadowEnrichActivityTypeDef, _OptionalDeviceShadowEnrichActivityTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredFilterActivityTypeDef = TypedDict(
     "_RequiredFilterActivityTypeDef",
     {
         "name": str,
         "filter": str,
     },
@@ -703,36 +751,40 @@
     "_OptionalFilterActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class FilterActivityTypeDef(_RequiredFilterActivityTypeDef, _OptionalFilterActivityTypeDef):
     pass
 
+
 _RequiredGetDatasetContentRequestRequestTypeDef = TypedDict(
     "_RequiredGetDatasetContentRequestRequestTypeDef",
     {
         "datasetName": str,
     },
 )
 _OptionalGetDatasetContentRequestRequestTypeDef = TypedDict(
     "_OptionalGetDatasetContentRequestRequestTypeDef",
     {
         "versionId": str,
     },
     total=False,
 )
 
+
 class GetDatasetContentRequestRequestTypeDef(
     _RequiredGetDatasetContentRequestRequestTypeDef, _OptionalGetDatasetContentRequestRequestTypeDef
 ):
     pass
 
+
 GlueConfigurationTypeDef = TypedDict(
     "GlueConfigurationTypeDef",
     {
         "tableName": str,
         "databaseName": str,
     },
 )
@@ -749,121 +801,57 @@
     "_OptionalLambdaActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class LambdaActivityTypeDef(_RequiredLambdaActivityTypeDef, _OptionalLambdaActivityTypeDef):
     pass
 
-ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
-    "ListChannelsRequestListChannelsPaginateTypeDef",
+
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
 
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
-    "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    {
-        "datasetName": str,
-    },
-)
-_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
-    "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
-    {
-        "scheduledOnOrAfter": Union[datetime, str],
-        "scheduledBefore": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
-    _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-    _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-):
-    pass
-
-_RequiredListDatasetContentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDatasetContentsRequestRequestTypeDef",
-    {
-        "datasetName": str,
-    },
-)
-_OptionalListDatasetContentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDatasetContentsRequestRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-        "scheduledOnOrAfter": Union[datetime, str],
-        "scheduledBefore": Union[datetime, str],
-    },
-    total=False,
-)
-
-class ListDatasetContentsRequestRequestTypeDef(
-    _RequiredListDatasetContentsRequestRequestTypeDef,
-    _OptionalListDatasetContentsRequestRequestTypeDef,
-):
-    pass
-
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
-    "ListDatastoresRequestListDatastoresPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatastoresRequestRequestTypeDef = TypedDict(
     "ListDatastoresRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesRequestRequestTypeDef = TypedDict(
     "ListPipelinesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -888,34 +876,70 @@
     "_OptionalMathActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class MathActivityTypeDef(_RequiredMathActivityTypeDef, _OptionalMathActivityTypeDef):
     pass
 
+
 OutputFileUriValueTypeDef = TypedDict(
     "OutputFileUriValueTypeDef",
     {
         "fileName": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredRemoveAttributesActivityOutputTypeDef = TypedDict(
+    "_RequiredRemoveAttributesActivityOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "name": str,
+        "attributes": List[str],
+    },
+)
+_OptionalRemoveAttributesActivityOutputTypeDef = TypedDict(
+    "_OptionalRemoveAttributesActivityOutputTypeDef",
+    {
+        "next": str,
     },
     total=False,
 )
 
+
+class RemoveAttributesActivityOutputTypeDef(
+    _RequiredRemoveAttributesActivityOutputTypeDef, _OptionalRemoveAttributesActivityOutputTypeDef
+):
+    pass
+
+
+_RequiredSelectAttributesActivityOutputTypeDef = TypedDict(
+    "_RequiredSelectAttributesActivityOutputTypeDef",
+    {
+        "name": str,
+        "attributes": List[str],
+    },
+)
+_OptionalSelectAttributesActivityOutputTypeDef = TypedDict(
+    "_OptionalSelectAttributesActivityOutputTypeDef",
+    {
+        "next": str,
+    },
+    total=False,
+)
+
+
+class SelectAttributesActivityOutputTypeDef(
+    _RequiredSelectAttributesActivityOutputTypeDef, _OptionalSelectAttributesActivityOutputTypeDef
+):
+    pass
+
+
 _RequiredRemoveAttributesActivityTypeDef = TypedDict(
     "_RequiredRemoveAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -923,19 +947,21 @@
     "_OptionalRemoveAttributesActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class RemoveAttributesActivityTypeDef(
     _RequiredRemoveAttributesActivityTypeDef, _OptionalRemoveAttributesActivityTypeDef
 ):
     pass
 
+
 _RequiredSelectAttributesActivityTypeDef = TypedDict(
     "_RequiredSelectAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -943,131 +969,103 @@
     "_OptionalSelectAttributesActivityTypeDef",
     {
         "next": str,
     },
     total=False,
 )
 
+
 class SelectAttributesActivityTypeDef(
     _RequiredSelectAttributesActivityTypeDef, _OptionalSelectAttributesActivityTypeDef
 ):
     pass
 
+
 ReprocessingSummaryTypeDef = TypedDict(
     "ReprocessingSummaryTypeDef",
     {
         "id": str,
         "status": ReprocessingStatusType,
         "creationTime": datetime,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
-RunPipelineActivityResponseTypeDef = TypedDict(
-    "RunPipelineActivityResponseTypeDef",
+BatchPutMessageResponseTypeDef = TypedDict(
+    "BatchPutMessageResponseTypeDef",
     {
-        "payloads": List[bytes],
-        "logResult": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSampleChannelDataRequestRequestTypeDef = TypedDict(
-    "_RequiredSampleChannelDataRequestRequestTypeDef",
-    {
-        "channelName": str,
-    },
-)
-_OptionalSampleChannelDataRequestRequestTypeDef = TypedDict(
-    "_OptionalSampleChannelDataRequestRequestTypeDef",
+CreateDatasetContentResponseTypeDef = TypedDict(
+    "CreateDatasetContentResponseTypeDef",
     {
-        "maxMessages": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "versionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class SampleChannelDataRequestRequestTypeDef(
-    _RequiredSampleChannelDataRequestRequestTypeDef, _OptionalSampleChannelDataRequestRequestTypeDef
-):
-    pass
-
-SampleChannelDataResponseTypeDef = TypedDict(
-    "SampleChannelDataResponseTypeDef",
+CreatePipelineResponseTypeDef = TypedDict(
+    "CreatePipelineResponseTypeDef",
     {
-        "payloads": List[bytes],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "pipelineName": str,
+        "pipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartPipelineReprocessingResponseTypeDef = TypedDict(
-    "StartPipelineReprocessingResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "reprocessingId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+RunPipelineActivityResponseTypeDef = TypedDict(
+    "RunPipelineActivityResponseTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "payloads": List[bytes],
+        "logResult": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutMessageResponseTypeDef = TypedDict(
-    "BatchPutMessageResponseTypeDef",
+SampleChannelDataResponseTypeDef = TypedDict(
+    "SampleChannelDataResponseTypeDef",
     {
-        "batchPutMessageErrorEntries": List[BatchPutMessageErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "payloads": List[bytes],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutMessageRequestRequestTypeDef = TypedDict(
-    "BatchPutMessageRequestRequestTypeDef",
+StartPipelineReprocessingResponseTypeDef = TypedDict(
+    "StartPipelineReprocessingResponseTypeDef",
     {
-        "channelName": str,
-        "messages": Sequence[MessageTypeDef],
+        "reprocessingId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
-    "_RequiredStartPipelineReprocessingRequestRequestTypeDef",
+MessageTypeDef = TypedDict(
+    "MessageTypeDef",
     {
-        "pipelineName": str,
+        "messageId": str,
+        "payload": BlobTypeDef,
     },
 )
-_OptionalStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
-    "_OptionalStartPipelineReprocessingRequestRequestTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "channelMessages": ChannelMessagesTypeDef,
-    },
-    total=False,
-)
-
-class StartPipelineReprocessingRequestRequestTypeDef(
-    _RequiredStartPipelineReprocessingRequestRequestTypeDef,
-    _OptionalStartPipelineReprocessingRequestRequestTypeDef,
-):
-    pass
 
 ChannelStatisticsTypeDef = TypedDict(
     "ChannelStatisticsTypeDef",
     {
         "size": EstimatedResourceSizeTypeDef,
     },
     total=False,
@@ -1077,75 +1075,92 @@
     "DatastoreStatisticsTypeDef",
     {
         "size": EstimatedResourceSizeTypeDef,
     },
     total=False,
 )
 
-ChannelStorageSummaryTypeDef = TypedDict(
-    "ChannelStorageSummaryTypeDef",
+ChannelStorageOutputTypeDef = TypedDict(
+    "ChannelStorageOutputTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
+        "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
     },
     total=False,
 )
 
 ChannelStorageTypeDef = TypedDict(
     "ChannelStorageTypeDef",
     {
         "serviceManagedS3": Mapping[str, Any],
         "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
     },
     total=False,
 )
 
+ChannelStorageSummaryTypeDef = TypedDict(
+    "ChannelStorageSummaryTypeDef",
+    {
+        "serviceManagedS3": Dict[str, Any],
+        "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
+    },
+    total=False,
+)
+
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channelName": str,
         "channelArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDatasetResponseTypeDef = TypedDict(
     "CreateDatasetResponseTypeDef",
     {
         "datasetName": str,
         "datasetArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDatastoreResponseTypeDef = TypedDict(
     "CreateDatastoreResponseTypeDef",
     {
         "datastoreName": str,
         "datastoreArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SchemaDefinitionOutputTypeDef = TypedDict(
+    "SchemaDefinitionOutputTypeDef",
+    {
+        "columns": List[ColumnTypeDef],
     },
+    total=False,
 )
 
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "columns": Sequence[ColumnTypeDef],
     },
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1167,15 +1182,15 @@
 
 GetDatasetContentResponseTypeDef = TypedDict(
     "GetDatasetContentResponseTypeDef",
     {
         "entries": List[DatasetEntryTypeDef],
         "timestamp": datetime,
         "status": DatasetContentStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetTriggerTypeDef = TypedDict(
     "DatasetTriggerTypeDef",
     {
         "schedule": ScheduleTypeDef,
@@ -1224,15 +1239,15 @@
     total=False,
 )
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
@@ -1251,19 +1266,149 @@
     "_OptionalS3DestinationConfigurationTypeDef",
     {
         "glueConfiguration": GlueConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class S3DestinationConfigurationTypeDef(
     _RequiredS3DestinationConfigurationTypeDef, _OptionalS3DestinationConfigurationTypeDef
 ):
     pass
 
+
+ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
+    "ListChannelsRequestListChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDatastoresRequestListDatastoresPaginateTypeDef = TypedDict(
+    "ListDatastoresRequestListDatastoresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
+    "_RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    {
+        "datasetName": str,
+    },
+)
+_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef = TypedDict(
+    "_OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
+    {
+        "scheduledOnOrAfter": TimestampTypeDef,
+        "scheduledBefore": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDatasetContentsRequestListDatasetContentsPaginateTypeDef(
+    _RequiredListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    _OptionalListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDatasetContentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDatasetContentsRequestRequestTypeDef",
+    {
+        "datasetName": str,
+    },
+)
+_OptionalListDatasetContentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDatasetContentsRequestRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+        "scheduledOnOrAfter": TimestampTypeDef,
+        "scheduledBefore": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDatasetContentsRequestRequestTypeDef(
+    _RequiredListDatasetContentsRequestRequestTypeDef,
+    _OptionalListDatasetContentsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSampleChannelDataRequestRequestTypeDef = TypedDict(
+    "_RequiredSampleChannelDataRequestRequestTypeDef",
+    {
+        "channelName": str,
+    },
+)
+_OptionalSampleChannelDataRequestRequestTypeDef = TypedDict(
+    "_OptionalSampleChannelDataRequestRequestTypeDef",
+    {
+        "maxMessages": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class SampleChannelDataRequestRequestTypeDef(
+    _RequiredSampleChannelDataRequestRequestTypeDef, _OptionalSampleChannelDataRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
+    "_RequiredStartPipelineReprocessingRequestRequestTypeDef",
+    {
+        "pipelineName": str,
+    },
+)
+_OptionalStartPipelineReprocessingRequestRequestTypeDef = TypedDict(
+    "_OptionalStartPipelineReprocessingRequestRequestTypeDef",
+    {
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "channelMessages": ChannelMessagesTypeDef,
+    },
+    total=False,
+)
+
+
+class StartPipelineReprocessingRequestRequestTypeDef(
+    _RequiredStartPipelineReprocessingRequestRequestTypeDef,
+    _OptionalStartPipelineReprocessingRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredVariableTypeDef = TypedDict(
     "_RequiredVariableTypeDef",
     {
         "name": str,
     },
 )
 _OptionalVariableTypeDef = TypedDict(
@@ -1273,17 +1418,36 @@
         "doubleValue": float,
         "datasetContentVersionValue": DatasetContentVersionValueTypeDef,
         "outputFileUriValue": OutputFileUriValueTypeDef,
     },
     total=False,
 )
 
+
 class VariableTypeDef(_RequiredVariableTypeDef, _OptionalVariableTypeDef):
     pass
 
+
+PipelineActivityOutputTypeDef = TypedDict(
+    "PipelineActivityOutputTypeDef",
+    {
+        "channel": ChannelActivityTypeDef,
+        "lambda": LambdaActivityTypeDef,
+        "datastore": DatastoreActivityTypeDef,
+        "addAttributes": AddAttributesActivityOutputTypeDef,
+        "removeAttributes": RemoveAttributesActivityOutputTypeDef,
+        "selectAttributes": SelectAttributesActivityOutputTypeDef,
+        "filter": FilterActivityTypeDef,
+        "math": MathActivityTypeDef,
+        "deviceRegistryEnrich": DeviceRegistryEnrichActivityTypeDef,
+        "deviceShadowEnrich": DeviceShadowEnrichActivityTypeDef,
+    },
+    total=False,
+)
+
 PipelineActivityTypeDef = TypedDict(
     "PipelineActivityTypeDef",
     {
         "channel": ChannelActivityTypeDef,
         "lambda": LambdaActivityTypeDef,
         "datastore": DatastoreActivityTypeDef,
         "addAttributes": AddAttributesActivityTypeDef,
@@ -1304,42 +1468,38 @@
         "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
         "creationTime": datetime,
         "lastUpdateTime": datetime,
     },
     total=False,
 )
 
-ChannelSummaryTypeDef = TypedDict(
-    "ChannelSummaryTypeDef",
+BatchPutMessageRequestRequestTypeDef = TypedDict(
+    "BatchPutMessageRequestRequestTypeDef",
     {
         "channelName": str,
-        "channelStorage": ChannelStorageSummaryTypeDef,
-        "status": ChannelStatusType,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "lastMessageArrivalTime": datetime,
+        "messages": Sequence[MessageTypeDef],
     },
-    total=False,
 )
 
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "name": str,
-        "storage": ChannelStorageTypeDef,
+        "storage": ChannelStorageOutputTypeDef,
         "arn": str,
         "status": ChannelStatusType,
         "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
     },
     total=False,
 )
 
+ChannelStorageUnionTypeDef = Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef]
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalCreateChannelRequestRequestTypeDef = TypedDict(
@@ -1348,19 +1508,21 @@
         "channelStorage": ChannelStorageTypeDef,
         "retentionPeriod": RetentionPeriodTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalUpdateChannelRequestRequestTypeDef = TypedDict(
@@ -1368,33 +1530,56 @@
     {
         "channelStorage": ChannelStorageTypeDef,
         "retentionPeriod": RetentionPeriodTypeDef,
     },
     total=False,
 )
 
+
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+
+ChannelSummaryTypeDef = TypedDict(
+    "ChannelSummaryTypeDef",
+    {
+        "channelName": str,
+        "channelStorage": ChannelStorageSummaryTypeDef,
+        "status": ChannelStatusType,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "lastMessageArrivalTime": datetime,
+    },
+    total=False,
+)
+
+ParquetConfigurationOutputTypeDef = TypedDict(
+    "ParquetConfigurationOutputTypeDef",
+    {
+        "schemaDefinition": SchemaDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
 ParquetConfigurationTypeDef = TypedDict(
     "ParquetConfigurationTypeDef",
     {
         "schemaDefinition": SchemaDefinitionTypeDef,
     },
     total=False,
 )
 
 ListDatasetContentsResponseTypeDef = TypedDict(
     "ListDatasetContentsResponseTypeDef",
     {
         "datasetContentSummaries": List[DatasetContentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetSummaryTypeDef = TypedDict(
     "DatasetSummaryTypeDef",
     {
         "datasetName": str,
@@ -1413,24 +1598,42 @@
         "serviceManagedS3": Dict[str, Any],
         "customerManagedS3": CustomerManagedDatastoreS3StorageSummaryTypeDef,
         "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     },
     total=False,
 )
 
+DatastoreStorageOutputTypeDef = TypedDict(
+    "DatastoreStorageOutputTypeDef",
+    {
+        "serviceManagedS3": Dict[str, Any],
+        "customerManagedS3": CustomerManagedDatastoreS3StorageTypeDef,
+        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageTypeDef,
+    },
+    total=False,
+)
+
 DatastoreStorageTypeDef = TypedDict(
     "DatastoreStorageTypeDef",
     {
         "serviceManagedS3": Mapping[str, Any],
         "customerManagedS3": CustomerManagedDatastoreS3StorageTypeDef,
         "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     },
     total=False,
 )
 
+DatastorePartitionsOutputTypeDef = TypedDict(
+    "DatastorePartitionsOutputTypeDef",
+    {
+        "partitions": List[DatastorePartitionTypeDef],
+    },
+    total=False,
+)
+
 DatastorePartitionsTypeDef = TypedDict(
     "DatastorePartitionsTypeDef",
     {
         "partitions": Sequence[DatastorePartitionTypeDef],
     },
     total=False,
 )
@@ -1445,140 +1648,172 @@
     "_OptionalLateDataRuleTypeDef",
     {
         "ruleName": str,
     },
     total=False,
 )
 
+
 class LateDataRuleTypeDef(_RequiredLateDataRuleTypeDef, _OptionalLateDataRuleTypeDef):
     pass
 
+
+_RequiredSqlQueryDatasetActionOutputTypeDef = TypedDict(
+    "_RequiredSqlQueryDatasetActionOutputTypeDef",
+    {
+        "sqlQuery": str,
+    },
+)
+_OptionalSqlQueryDatasetActionOutputTypeDef = TypedDict(
+    "_OptionalSqlQueryDatasetActionOutputTypeDef",
+    {
+        "filters": List[QueryFilterTypeDef],
+    },
+    total=False,
+)
+
+
+class SqlQueryDatasetActionOutputTypeDef(
+    _RequiredSqlQueryDatasetActionOutputTypeDef, _OptionalSqlQueryDatasetActionOutputTypeDef
+):
+    pass
+
+
 _RequiredSqlQueryDatasetActionTypeDef = TypedDict(
     "_RequiredSqlQueryDatasetActionTypeDef",
     {
         "sqlQuery": str,
     },
 )
 _OptionalSqlQueryDatasetActionTypeDef = TypedDict(
     "_OptionalSqlQueryDatasetActionTypeDef",
     {
         "filters": Sequence[QueryFilterTypeDef],
     },
     total=False,
 )
 
+
 class SqlQueryDatasetActionTypeDef(
     _RequiredSqlQueryDatasetActionTypeDef, _OptionalSqlQueryDatasetActionTypeDef
 ):
     pass
 
+
 DatasetContentDeliveryDestinationTypeDef = TypedDict(
     "DatasetContentDeliveryDestinationTypeDef",
     {
         "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationTypeDef,
         "s3DestinationConfiguration": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredContainerDatasetActionTypeDef = TypedDict(
-    "_RequiredContainerDatasetActionTypeDef",
+_RequiredContainerDatasetActionOutputTypeDef = TypedDict(
+    "_RequiredContainerDatasetActionOutputTypeDef",
     {
         "image": str,
         "executionRoleArn": str,
         "resourceConfiguration": ResourceConfigurationTypeDef,
     },
 )
-_OptionalContainerDatasetActionTypeDef = TypedDict(
-    "_OptionalContainerDatasetActionTypeDef",
+_OptionalContainerDatasetActionOutputTypeDef = TypedDict(
+    "_OptionalContainerDatasetActionOutputTypeDef",
     {
-        "variables": Sequence[VariableTypeDef],
+        "variables": List[VariableTypeDef],
     },
     total=False,
 )
 
-class ContainerDatasetActionTypeDef(
-    _RequiredContainerDatasetActionTypeDef, _OptionalContainerDatasetActionTypeDef
+
+class ContainerDatasetActionOutputTypeDef(
+    _RequiredContainerDatasetActionOutputTypeDef, _OptionalContainerDatasetActionOutputTypeDef
 ):
     pass
 
-_RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePipelineRequestRequestTypeDef",
+
+_RequiredContainerDatasetActionTypeDef = TypedDict(
+    "_RequiredContainerDatasetActionTypeDef",
     {
-        "pipelineName": str,
-        "pipelineActivities": Sequence[PipelineActivityTypeDef],
+        "image": str,
+        "executionRoleArn": str,
+        "resourceConfiguration": ResourceConfigurationTypeDef,
     },
 )
-_OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePipelineRequestRequestTypeDef",
+_OptionalContainerDatasetActionTypeDef = TypedDict(
+    "_OptionalContainerDatasetActionTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "variables": Sequence[VariableTypeDef],
     },
     total=False,
 )
 
-class CreatePipelineRequestRequestTypeDef(
-    _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
+
+class ContainerDatasetActionTypeDef(
+    _RequiredContainerDatasetActionTypeDef, _OptionalContainerDatasetActionTypeDef
 ):
     pass
 
+
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "name": str,
         "arn": str,
-        "activities": List[PipelineActivityTypeDef],
+        "activities": List[PipelineActivityOutputTypeDef],
         "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
         "creationTime": datetime,
         "lastUpdateTime": datetime,
     },
     total=False,
 )
 
+PipelineActivityUnionTypeDef = Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
 RunPipelineActivityRequestRequestTypeDef = TypedDict(
     "RunPipelineActivityRequestRequestTypeDef",
     {
         "pipelineActivity": PipelineActivityTypeDef,
-        "payloads": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-    },
-)
-
-UpdatePipelineRequestRequestTypeDef = TypedDict(
-    "UpdatePipelineRequestRequestTypeDef",
-    {
-        "pipelineName": str,
-        "pipelineActivities": Sequence[PipelineActivityTypeDef],
+        "payloads": Sequence[BlobTypeDef],
     },
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "pipelineSummaries": List[PipelineSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeChannelResponseTypeDef = TypedDict(
+    "DescribeChannelResponseTypeDef",
+    {
+        "channel": ChannelTypeDef,
+        "statistics": ChannelStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channelSummaries": List[ChannelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeChannelResponseTypeDef = TypedDict(
-    "DescribeChannelResponseTypeDef",
+FileFormatConfigurationOutputTypeDef = TypedDict(
+    "FileFormatConfigurationOutputTypeDef",
     {
-        "channel": ChannelTypeDef,
-        "statistics": ChannelStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "jsonConfiguration": Dict[str, Any],
+        "parquetConfiguration": ParquetConfigurationOutputTypeDef,
     },
+    total=False,
 )
 
 FileFormatConfigurationTypeDef = TypedDict(
     "FileFormatConfigurationTypeDef",
     {
         "jsonConfiguration": Mapping[str, Any],
         "parquetConfiguration": ParquetConfigurationTypeDef,
@@ -1587,110 +1822,161 @@
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "datasetSummaries": List[DatasetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DatastoreStorageUnionTypeDef = Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef]
 DatastoreSummaryTypeDef = TypedDict(
     "DatastoreSummaryTypeDef",
     {
         "datastoreName": str,
         "datastoreStorage": DatastoreStorageSummaryTypeDef,
         "status": DatastoreStatusType,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
         "fileFormatType": FileFormatTypeType,
-        "datastorePartitions": DatastorePartitionsTypeDef,
+        "datastorePartitions": DatastorePartitionsOutputTypeDef,
     },
     total=False,
 )
 
+DatastorePartitionsUnionTypeDef = Union[
+    DatastorePartitionsTypeDef, DatastorePartitionsOutputTypeDef
+]
 _RequiredDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_RequiredDatasetContentDeliveryRuleTypeDef",
     {
         "destination": DatasetContentDeliveryDestinationTypeDef,
     },
 )
 _OptionalDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_OptionalDatasetContentDeliveryRuleTypeDef",
     {
         "entryName": str,
     },
     total=False,
 )
 
+
 class DatasetContentDeliveryRuleTypeDef(
     _RequiredDatasetContentDeliveryRuleTypeDef, _OptionalDatasetContentDeliveryRuleTypeDef
 ):
     pass
 
+
+DatasetActionOutputTypeDef = TypedDict(
+    "DatasetActionOutputTypeDef",
+    {
+        "actionName": str,
+        "queryAction": SqlQueryDatasetActionOutputTypeDef,
+        "containerAction": ContainerDatasetActionOutputTypeDef,
+    },
+    total=False,
+)
+
 DatasetActionTypeDef = TypedDict(
     "DatasetActionTypeDef",
     {
         "actionName": str,
         "queryAction": SqlQueryDatasetActionTypeDef,
         "containerAction": ContainerDatasetActionTypeDef,
     },
     total=False,
 )
 
 DescribePipelineResponseTypeDef = TypedDict(
     "DescribePipelineResponseTypeDef",
     {
         "pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatastoreRequestRequestTypeDef",
+_RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePipelineRequestRequestTypeDef",
     {
-        "datastoreName": str,
+        "pipelineName": str,
+        "pipelineActivities": Sequence[PipelineActivityUnionTypeDef],
     },
 )
-_OptionalCreateDatastoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatastoreRequestRequestTypeDef",
+_OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePipelineRequestRequestTypeDef",
     {
-        "datastoreStorage": DatastoreStorageTypeDef,
-        "retentionPeriod": RetentionPeriodTypeDef,
         "tags": Sequence[TagTypeDef],
-        "fileFormatConfiguration": FileFormatConfigurationTypeDef,
-        "datastorePartitions": DatastorePartitionsTypeDef,
     },
     total=False,
 )
 
-class CreateDatastoreRequestRequestTypeDef(
-    _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
+
+class CreatePipelineRequestRequestTypeDef(
+    _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
+
+UpdatePipelineRequestRequestTypeDef = TypedDict(
+    "UpdatePipelineRequestRequestTypeDef",
+    {
+        "pipelineName": str,
+        "pipelineActivities": Sequence[PipelineActivityUnionTypeDef],
+    },
+)
+
 DatastoreTypeDef = TypedDict(
     "DatastoreTypeDef",
     {
         "name": str,
-        "storage": DatastoreStorageTypeDef,
+        "storage": DatastoreStorageOutputTypeDef,
         "arn": str,
         "status": DatastoreStatusType,
         "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
+        "fileFormatConfiguration": FileFormatConfigurationOutputTypeDef,
+        "datastorePartitions": DatastorePartitionsOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatastoreRequestRequestTypeDef",
+    {
+        "datastoreName": str,
+    },
+)
+_OptionalCreateDatastoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatastoreRequestRequestTypeDef",
+    {
+        "datastoreStorage": DatastoreStorageTypeDef,
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "tags": Sequence[TagTypeDef],
         "fileFormatConfiguration": FileFormatConfigurationTypeDef,
         "datastorePartitions": DatastorePartitionsTypeDef,
     },
     total=False,
 )
 
+
+class CreateDatastoreRequestRequestTypeDef(
+    _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
+):
+    pass
+
+
+FileFormatConfigurationUnionTypeDef = Union[
+    FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
+]
 _RequiredUpdateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatastoreRequestRequestTypeDef",
     {
         "datastoreName": str,
     },
 )
 _OptionalUpdateDatastoreRequestRequestTypeDef = TypedDict(
@@ -1699,33 +1985,71 @@
         "retentionPeriod": RetentionPeriodTypeDef,
         "datastoreStorage": DatastoreStorageTypeDef,
         "fileFormatConfiguration": FileFormatConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDatastoreRequestRequestTypeDef(
     _RequiredUpdateDatastoreRequestRequestTypeDef, _OptionalUpdateDatastoreRequestRequestTypeDef
 ):
     pass
 
+
 ListDatastoresResponseTypeDef = TypedDict(
     "ListDatastoresResponseTypeDef",
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DatasetTypeDef = TypedDict(
+    "DatasetTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "actions": List[DatasetActionOutputTypeDef],
+        "triggers": List[DatasetTriggerTypeDef],
+        "contentDeliveryRules": List[DatasetContentDeliveryRuleTypeDef],
+        "status": DatasetStatusType,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "versioningConfiguration": VersioningConfigurationTypeDef,
+        "lateDataRules": List[LateDataRuleTypeDef],
+    },
+    total=False,
+)
+
+DatasetActionUnionTypeDef = Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]
+DescribeDatastoreResponseTypeDef = TypedDict(
+    "DescribeDatastoreResponseTypeDef",
+    {
+        "datastore": DatastoreTypeDef,
+        "statistics": DatastoreStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "dataset": DatasetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[DatasetActionTypeDef],
+        "actions": Sequence[DatasetActionUnionTypeDef],
     },
 )
 _OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
@@ -1733,70 +2057,38 @@
         "versioningConfiguration": VersioningConfigurationTypeDef,
         "tags": Sequence[TagTypeDef],
         "lateDataRules": Sequence[LateDataRuleTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-DatasetTypeDef = TypedDict(
-    "DatasetTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "actions": List[DatasetActionTypeDef],
-        "triggers": List[DatasetTriggerTypeDef],
-        "contentDeliveryRules": List[DatasetContentDeliveryRuleTypeDef],
-        "status": DatasetStatusType,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "retentionPeriod": RetentionPeriodTypeDef,
-        "versioningConfiguration": VersioningConfigurationTypeDef,
-        "lateDataRules": List[LateDataRuleTypeDef],
-    },
-    total=False,
-)
 
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[DatasetActionTypeDef],
+        "actions": Sequence[DatasetActionUnionTypeDef],
     },
 )
 _OptionalUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
         "retentionPeriod": RetentionPeriodTypeDef,
         "versioningConfiguration": VersioningConfigurationTypeDef,
         "lateDataRules": Sequence[LateDataRuleTypeDef],
     },
     total=False,
 )
 
+
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
-
-DescribeDatastoreResponseTypeDef = TypedDict(
-    "DescribeDatastoreResponseTypeDef",
-    {
-        "datastore": DatastoreTypeDef,
-        "statistics": DatastoreStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "dataset": DatasetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics.egg-info/PKG-INFO` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotanalytics
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTAnalytics 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTAnalytics 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotanalytics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotanalytics type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotanalytics"></a>
 
 # types-aiobotocore-iotanalytics
 
 [![PyPI - types-aiobotocore-iotanalytics](https://img.shields.io/pypi/v/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotanalytics?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotanalytics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotanalytics)](https://pepy.tech/project/types-aiobotocore-iotanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTAnalytics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
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
 [types-aiobotocore-iotanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/).
 
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
@@ -330,40 +329,40 @@
 )
 
 
 def check_value(value: ChannelStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotanalytics.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotanalytics.type_defs import (
+    AddAttributesActivityOutputTypeDef,
     AddAttributesActivityTypeDef,
     BatchPutMessageErrorEntryTypeDef,
-    MessageTypeDef,
+    ResponseMetadataTypeDef,
+    BlobTypeDef,
     CancelPipelineReprocessingRequestRequestTypeDef,
     ChannelActivityTypeDef,
     ChannelMessagesTypeDef,
     EstimatedResourceSizeTypeDef,
-    CustomerManagedChannelS3StorageSummaryTypeDef,
     CustomerManagedChannelS3StorageTypeDef,
+    CustomerManagedChannelS3StorageSummaryTypeDef,
     RetentionPeriodTypeDef,
     ColumnTypeDef,
     ResourceConfigurationTypeDef,
     TagTypeDef,
     CreateDatasetContentRequestRequestTypeDef,
-    CreateDatasetContentResponseTypeDef,
     VersioningConfigurationTypeDef,
-    CreatePipelineResponseTypeDef,
     CustomerManagedDatastoreS3StorageSummaryTypeDef,
     CustomerManagedDatastoreS3StorageTypeDef,
     DatasetActionSummaryTypeDef,
     IotEventsDestinationConfigurationTypeDef,
     DatasetContentStatusTypeDef,
     DatasetContentVersionValueTypeDef,
     DatasetEntryTypeDef,
@@ -384,109 +383,130 @@
     DescribeChannelRequestRequestTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeDatastoreRequestRequestTypeDef,
     LoggingOptionsTypeDef,
     DescribePipelineRequestRequestTypeDef,
     DeviceRegistryEnrichActivityTypeDef,
     DeviceShadowEnrichActivityTypeDef,
-    EmptyResponseMetadataTypeDef,
     FilterActivityTypeDef,
     GetDatasetContentRequestRequestTypeDef,
     GlueConfigurationTypeDef,
     LambdaActivityTypeDef,
-    ListChannelsRequestListChannelsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChannelsRequestRequestTypeDef,
-    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
-    ListDatasetContentsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    TimestampTypeDef,
     ListDatasetsRequestRequestTypeDef,
-    ListDatastoresRequestListDatastoresPaginateTypeDef,
     ListDatastoresRequestRequestTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MathActivityTypeDef,
     OutputFileUriValueTypeDef,
-    PaginatorConfigTypeDef,
+    RemoveAttributesActivityOutputTypeDef,
+    SelectAttributesActivityOutputTypeDef,
     RemoveAttributesActivityTypeDef,
     SelectAttributesActivityTypeDef,
     ReprocessingSummaryTypeDef,
-    ResponseMetadataTypeDef,
+    UntagResourceRequestRequestTypeDef,
+    BatchPutMessageResponseTypeDef,
+    CreateDatasetContentResponseTypeDef,
+    CreatePipelineResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     RunPipelineActivityResponseTypeDef,
-    SampleChannelDataRequestRequestTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    BatchPutMessageResponseTypeDef,
-    BatchPutMessageRequestRequestTypeDef,
-    StartPipelineReprocessingRequestRequestTypeDef,
+    MessageTypeDef,
     ChannelStatisticsTypeDef,
     DatastoreStatisticsTypeDef,
-    ChannelStorageSummaryTypeDef,
+    ChannelStorageOutputTypeDef,
     ChannelStorageTypeDef,
+    ChannelStorageSummaryTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
+    SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatasetContentSummaryTypeDef,
     GetDatasetContentResponseTypeDef,
     DatasetTriggerTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     DatastorePartitionTypeDef,
     LateDataRuleConfigurationTypeDef,
     QueryFilterTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     S3DestinationConfigurationTypeDef,
+    ListChannelsRequestListChannelsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListDatastoresRequestListDatastoresPaginateTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
+    ListDatasetContentsRequestListDatasetContentsPaginateTypeDef,
+    ListDatasetContentsRequestRequestTypeDef,
+    SampleChannelDataRequestRequestTypeDef,
+    StartPipelineReprocessingRequestRequestTypeDef,
     VariableTypeDef,
+    PipelineActivityOutputTypeDef,
     PipelineActivityTypeDef,
     PipelineSummaryTypeDef,
-    ChannelSummaryTypeDef,
+    BatchPutMessageRequestRequestTypeDef,
     ChannelTypeDef,
+    ChannelStorageUnionTypeDef,
     CreateChannelRequestRequestTypeDef,
     UpdateChannelRequestRequestTypeDef,
+    ChannelSummaryTypeDef,
+    ParquetConfigurationOutputTypeDef,
     ParquetConfigurationTypeDef,
     ListDatasetContentsResponseTypeDef,
     DatasetSummaryTypeDef,
     DatastoreStorageSummaryTypeDef,
+    DatastoreStorageOutputTypeDef,
     DatastoreStorageTypeDef,
+    DatastorePartitionsOutputTypeDef,
     DatastorePartitionsTypeDef,
     LateDataRuleTypeDef,
+    SqlQueryDatasetActionOutputTypeDef,
     SqlQueryDatasetActionTypeDef,
     DatasetContentDeliveryDestinationTypeDef,
+    ContainerDatasetActionOutputTypeDef,
     ContainerDatasetActionTypeDef,
-    CreatePipelineRequestRequestTypeDef,
     PipelineTypeDef,
+    PipelineActivityUnionTypeDef,
     RunPipelineActivityRequestRequestTypeDef,
-    UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
-    ListChannelsResponseTypeDef,
     DescribeChannelResponseTypeDef,
+    ListChannelsResponseTypeDef,
+    FileFormatConfigurationOutputTypeDef,
     FileFormatConfigurationTypeDef,
     ListDatasetsResponseTypeDef,
+    DatastoreStorageUnionTypeDef,
     DatastoreSummaryTypeDef,
+    DatastorePartitionsUnionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
+    DatasetActionOutputTypeDef,
     DatasetActionTypeDef,
     DescribePipelineResponseTypeDef,
-    CreateDatastoreRequestRequestTypeDef,
+    CreatePipelineRequestRequestTypeDef,
+    UpdatePipelineRequestRequestTypeDef,
     DatastoreTypeDef,
+    CreateDatastoreRequestRequestTypeDef,
+    FileFormatConfigurationUnionTypeDef,
     UpdateDatastoreRequestRequestTypeDef,
     ListDatastoresResponseTypeDef,
-    CreateDatasetRequestRequestTypeDef,
     DatasetTypeDef,
-    UpdateDatasetRequestRequestTypeDef,
+    DatasetActionUnionTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeDatasetResponseTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    UpdateDatasetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AddAttributesActivityTypeDef:
+def get_value() -> AddAttributesActivityOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt` & `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*


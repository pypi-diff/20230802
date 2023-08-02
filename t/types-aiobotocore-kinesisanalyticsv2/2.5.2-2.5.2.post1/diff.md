# Comparing `tmp/types-aiobotocore-kinesisanalyticsv2-2.5.2.tar.gz` & `tmp/types-aiobotocore-kinesisanalyticsv2-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesisanalyticsv2-2.5.2.tar", last modified: Sat Jul  8 01:43:51 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesisanalyticsv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:31 2023, max compression
```

## Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.tar` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.394391 types-aiobotocore-kinesisanalyticsv2-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-07-08 01:43:51.390391 types-aiobotocore-kinesisanalyticsv2-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:51.394391 types-aiobotocore-kinesisanalyticsv2-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.378390 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29390 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29348 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9980 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69119 2023-07-08 01:33:30.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69018 2023-07-08 01:33:30.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:29.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.390391 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.513548 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21617 2023-08-02 14:52:31.513548 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:31.513548 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.509548 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29367 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29325 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-08-02 14:41:36.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9980 2023-08-02 14:41:35.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69867 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69764 2023-08-02 14:41:36.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.513548 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21617 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/LICENSE` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/PKG-INFO` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalyticsv2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore kinesisanalyticsv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore kinesisanalyticsv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesisanalyticsv2"></a>
 
 # types-aiobotocore-kinesisanalyticsv2
 
 [![PyPI - types-aiobotocore-kinesisanalyticsv2](https://img.shields.io/pypi/v/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesisanalyticsv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesisanalyticsv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalyticsv2)](https://pepy.tech/project/types-aiobotocore-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisAnalyticsV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [types-aiobotocore-kinesisanalyticsv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/).
 
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
@@ -327,74 +326,71 @@
 )
 
 
 def check_value(value: ApplicationModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesisanalyticsv2.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_kinesisanalyticsv2.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
     VpcConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationTypeDef,
     ApplicationSnapshotConfigurationUpdateTypeDef,
     VpcConfigurationUpdateTypeDef,
     ApplicationMaintenanceConfigurationDescriptionTypeDef,
     ApplicationMaintenanceConfigurationUpdateTypeDef,
     ApplicationRestoreConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
+    BlobTypeDef,
     CSVMappingParametersTypeDef,
     GlueDataCatalogConfigurationDescriptionTypeDef,
     GlueDataCatalogConfigurationTypeDef,
     GlueDataCatalogConfigurationUpdateTypeDef,
     CheckpointConfigurationDescriptionTypeDef,
     CheckpointConfigurationTypeDef,
     CheckpointConfigurationUpdateTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
     S3ApplicationCodeLocationDescriptionTypeDef,
     S3ContentLocationTypeDef,
     S3ContentLocationUpdateTypeDef,
     CreateApplicationPresignedUrlRequestRequestTypeDef,
-    CreateApplicationPresignedUrlResponseTypeDef,
     TagTypeDef,
     CreateApplicationSnapshotRequestRequestTypeDef,
     MavenReferenceTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
-    DeleteApplicationInputProcessingConfigurationResponseTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
-    DeleteApplicationOutputResponseTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationReferenceDataSourceResponseTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteApplicationSnapshotRequestRequestTypeDef,
+    TimestampTypeDef,
     DeleteApplicationVpcConfigurationRequestRequestTypeDef,
-    DeleteApplicationVpcConfigurationResponseTypeDef,
     S3ContentBaseLocationDescriptionTypeDef,
     S3ContentBaseLocationTypeDef,
     S3ContentBaseLocationUpdateTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeApplicationSnapshotRequestRequestTypeDef,
     SnapshotDetailsTypeDef,
     DescribeApplicationVersionRequestRequestTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     PropertyGroupTypeDef,
+    PropertyGroupOutputTypeDef,
     MonitoringConfigurationDescriptionTypeDef,
     ParallelismConfigurationDescriptionTypeDef,
     MonitoringConfigurationTypeDef,
     ParallelismConfigurationTypeDef,
     MonitoringConfigurationUpdateTypeDef,
     ParallelismConfigurationUpdateTypeDef,
     FlinkRunConfigurationTypeDef,
@@ -416,34 +412,36 @@
     KinesisFirehoseOutputUpdateTypeDef,
     KinesisStreamsOutputDescriptionTypeDef,
     KinesisStreamsOutputTypeDef,
     KinesisStreamsOutputUpdateTypeDef,
     LambdaOutputDescriptionTypeDef,
     LambdaOutputTypeDef,
     LambdaOutputUpdateTypeDef,
-    ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationSnapshotsRequestRequestTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
-    ResponseMetadataTypeDef,
     RollbackApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ZeppelinMonitoringConfigurationDescriptionTypeDef,
     ZeppelinMonitoringConfigurationTypeDef,
     ZeppelinMonitoringConfigurationUpdateTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionResponseTypeDef,
+    CreateApplicationPresignedUrlResponseTypeDef,
     DeleteApplicationCloudWatchLoggingOptionResponseTypeDef,
+    DeleteApplicationInputProcessingConfigurationResponseTypeDef,
+    DeleteApplicationOutputResponseTypeDef,
+    DeleteApplicationReferenceDataSourceResponseTypeDef,
+    DeleteApplicationVpcConfigurationResponseTypeDef,
     AddApplicationVpcConfigurationRequestRequestTypeDef,
     AddApplicationVpcConfigurationResponseTypeDef,
     UpdateApplicationMaintenanceConfigurationResponseTypeDef,
     UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     CatalogConfigurationDescriptionTypeDef,
@@ -452,35 +450,39 @@
     CodeContentDescriptionTypeDef,
     CodeContentTypeDef,
     CodeContentUpdateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomArtifactConfigurationDescriptionTypeDef,
     CustomArtifactConfigurationTypeDef,
+    DeleteApplicationRequestRequestTypeDef,
+    DeleteApplicationSnapshotRequestRequestTypeDef,
     DeployAsApplicationConfigurationDescriptionTypeDef,
     DeployAsApplicationConfigurationTypeDef,
     DeployAsApplicationConfigurationUpdateTypeDef,
     DescribeApplicationSnapshotResponseTypeDef,
     ListApplicationSnapshotsResponseTypeDef,
     SqlRunConfigurationTypeDef,
     EnvironmentPropertiesTypeDef,
-    EnvironmentPropertyDescriptionsTypeDef,
     EnvironmentPropertyUpdatesTypeDef,
+    EnvironmentPropertyDescriptionsTypeDef,
     FlinkApplicationConfigurationDescriptionTypeDef,
     FlinkApplicationConfigurationTypeDef,
     FlinkApplicationConfigurationUpdateTypeDef,
     RunConfigurationDescriptionTypeDef,
     RunConfigurationUpdateTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
+    ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ApplicationCodeConfigurationDescriptionTypeDef,
     ApplicationCodeConfigurationTypeDef,
     ApplicationCodeConfigurationUpdateTypeDef,
     ZeppelinApplicationConfigurationDescriptionTypeDef,
     ZeppelinApplicationConfigurationTypeDef,
     ZeppelinApplicationConfigurationUpdateTypeDef,
     RunConfigurationTypeDef,
@@ -488,26 +490,27 @@
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputResponseTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
     StartApplicationRequestRequestTypeDef,
     InputSchemaUpdateTypeDef,
+    SourceSchemaOutputTypeDef,
     SourceSchemaTypeDef,
     InputUpdateTypeDef,
     DiscoverInputSchemaResponseTypeDef,
     InputDescriptionTypeDef,
-    InputTypeDef,
     ReferenceDataSourceDescriptionTypeDef,
+    InputTypeDef,
     ReferenceDataSourceTypeDef,
     ReferenceDataSourceUpdateTypeDef,
     AddApplicationInputResponseTypeDef,
-    AddApplicationInputRequestRequestTypeDef,
     AddApplicationReferenceDataSourceResponseTypeDef,
     SqlApplicationConfigurationDescriptionTypeDef,
+    AddApplicationInputRequestRequestTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     SqlApplicationConfigurationTypeDef,
     SqlApplicationConfigurationUpdateTypeDef,
     ApplicationConfigurationDescriptionTypeDef,
     ApplicationConfigurationTypeDef,
     ApplicationConfigurationUpdateTypeDef,
     ApplicationDetailTypeDef,
@@ -517,15 +520,15 @@
     DescribeApplicationResponseTypeDef,
     DescribeApplicationVersionResponseTypeDef,
     RollbackApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLoggingOptionTypeDef:
+def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/README.md` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-kinesisanalyticsv2"></a>
 
 # types-aiobotocore-kinesisanalyticsv2
 
 [![PyPI - types-aiobotocore-kinesisanalyticsv2](https://img.shields.io/pypi/v/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesisanalyticsv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesisanalyticsv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalyticsv2)](https://pepy.tech/project/types-aiobotocore-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisAnalyticsV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [types-aiobotocore-kinesisanalyticsv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/).
 
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
@@ -294,74 +294,71 @@
 )
 
 
 def check_value(value: ApplicationModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesisanalyticsv2.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_kinesisanalyticsv2.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
     VpcConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationTypeDef,
     ApplicationSnapshotConfigurationUpdateTypeDef,
     VpcConfigurationUpdateTypeDef,
     ApplicationMaintenanceConfigurationDescriptionTypeDef,
     ApplicationMaintenanceConfigurationUpdateTypeDef,
     ApplicationRestoreConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
+    BlobTypeDef,
     CSVMappingParametersTypeDef,
     GlueDataCatalogConfigurationDescriptionTypeDef,
     GlueDataCatalogConfigurationTypeDef,
     GlueDataCatalogConfigurationUpdateTypeDef,
     CheckpointConfigurationDescriptionTypeDef,
     CheckpointConfigurationTypeDef,
     CheckpointConfigurationUpdateTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
     S3ApplicationCodeLocationDescriptionTypeDef,
     S3ContentLocationTypeDef,
     S3ContentLocationUpdateTypeDef,
     CreateApplicationPresignedUrlRequestRequestTypeDef,
-    CreateApplicationPresignedUrlResponseTypeDef,
     TagTypeDef,
     CreateApplicationSnapshotRequestRequestTypeDef,
     MavenReferenceTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
-    DeleteApplicationInputProcessingConfigurationResponseTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
-    DeleteApplicationOutputResponseTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationReferenceDataSourceResponseTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteApplicationSnapshotRequestRequestTypeDef,
+    TimestampTypeDef,
     DeleteApplicationVpcConfigurationRequestRequestTypeDef,
-    DeleteApplicationVpcConfigurationResponseTypeDef,
     S3ContentBaseLocationDescriptionTypeDef,
     S3ContentBaseLocationTypeDef,
     S3ContentBaseLocationUpdateTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeApplicationSnapshotRequestRequestTypeDef,
     SnapshotDetailsTypeDef,
     DescribeApplicationVersionRequestRequestTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     PropertyGroupTypeDef,
+    PropertyGroupOutputTypeDef,
     MonitoringConfigurationDescriptionTypeDef,
     ParallelismConfigurationDescriptionTypeDef,
     MonitoringConfigurationTypeDef,
     ParallelismConfigurationTypeDef,
     MonitoringConfigurationUpdateTypeDef,
     ParallelismConfigurationUpdateTypeDef,
     FlinkRunConfigurationTypeDef,
@@ -383,34 +380,36 @@
     KinesisFirehoseOutputUpdateTypeDef,
     KinesisStreamsOutputDescriptionTypeDef,
     KinesisStreamsOutputTypeDef,
     KinesisStreamsOutputUpdateTypeDef,
     LambdaOutputDescriptionTypeDef,
     LambdaOutputTypeDef,
     LambdaOutputUpdateTypeDef,
-    ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationSnapshotsRequestRequestTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
-    ResponseMetadataTypeDef,
     RollbackApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ZeppelinMonitoringConfigurationDescriptionTypeDef,
     ZeppelinMonitoringConfigurationTypeDef,
     ZeppelinMonitoringConfigurationUpdateTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionResponseTypeDef,
+    CreateApplicationPresignedUrlResponseTypeDef,
     DeleteApplicationCloudWatchLoggingOptionResponseTypeDef,
+    DeleteApplicationInputProcessingConfigurationResponseTypeDef,
+    DeleteApplicationOutputResponseTypeDef,
+    DeleteApplicationReferenceDataSourceResponseTypeDef,
+    DeleteApplicationVpcConfigurationResponseTypeDef,
     AddApplicationVpcConfigurationRequestRequestTypeDef,
     AddApplicationVpcConfigurationResponseTypeDef,
     UpdateApplicationMaintenanceConfigurationResponseTypeDef,
     UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     CatalogConfigurationDescriptionTypeDef,
@@ -419,35 +418,39 @@
     CodeContentDescriptionTypeDef,
     CodeContentTypeDef,
     CodeContentUpdateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomArtifactConfigurationDescriptionTypeDef,
     CustomArtifactConfigurationTypeDef,
+    DeleteApplicationRequestRequestTypeDef,
+    DeleteApplicationSnapshotRequestRequestTypeDef,
     DeployAsApplicationConfigurationDescriptionTypeDef,
     DeployAsApplicationConfigurationTypeDef,
     DeployAsApplicationConfigurationUpdateTypeDef,
     DescribeApplicationSnapshotResponseTypeDef,
     ListApplicationSnapshotsResponseTypeDef,
     SqlRunConfigurationTypeDef,
     EnvironmentPropertiesTypeDef,
-    EnvironmentPropertyDescriptionsTypeDef,
     EnvironmentPropertyUpdatesTypeDef,
+    EnvironmentPropertyDescriptionsTypeDef,
     FlinkApplicationConfigurationDescriptionTypeDef,
     FlinkApplicationConfigurationTypeDef,
     FlinkApplicationConfigurationUpdateTypeDef,
     RunConfigurationDescriptionTypeDef,
     RunConfigurationUpdateTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
+    ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ApplicationCodeConfigurationDescriptionTypeDef,
     ApplicationCodeConfigurationTypeDef,
     ApplicationCodeConfigurationUpdateTypeDef,
     ZeppelinApplicationConfigurationDescriptionTypeDef,
     ZeppelinApplicationConfigurationTypeDef,
     ZeppelinApplicationConfigurationUpdateTypeDef,
     RunConfigurationTypeDef,
@@ -455,26 +458,27 @@
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputResponseTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
     StartApplicationRequestRequestTypeDef,
     InputSchemaUpdateTypeDef,
+    SourceSchemaOutputTypeDef,
     SourceSchemaTypeDef,
     InputUpdateTypeDef,
     DiscoverInputSchemaResponseTypeDef,
     InputDescriptionTypeDef,
-    InputTypeDef,
     ReferenceDataSourceDescriptionTypeDef,
+    InputTypeDef,
     ReferenceDataSourceTypeDef,
     ReferenceDataSourceUpdateTypeDef,
     AddApplicationInputResponseTypeDef,
-    AddApplicationInputRequestRequestTypeDef,
     AddApplicationReferenceDataSourceResponseTypeDef,
     SqlApplicationConfigurationDescriptionTypeDef,
+    AddApplicationInputRequestRequestTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     SqlApplicationConfigurationTypeDef,
     SqlApplicationConfigurationUpdateTypeDef,
     ApplicationConfigurationDescriptionTypeDef,
     ApplicationConfigurationTypeDef,
     ApplicationConfigurationUpdateTypeDef,
     ApplicationDetailTypeDef,
@@ -484,15 +488,15 @@
     DescribeApplicationResponseTypeDef,
     DescribeApplicationVersionResponseTypeDef,
     RollbackApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLoggingOptionTypeDef:
+def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/setup.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesisanalyticsv2",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_kinesisanalyticsv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2 service generated with"
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
-    keywords=(
-        "aiobotocore kinesisanalyticsv2 type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore kinesisanalyticsv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kinesisanalyticsv2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/"
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/__init__.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/__init__.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/__main__.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2\nOther"
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

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/client.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("kinesisanalyticsv2") as client:
         client: KinesisAnalyticsV2Client
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ApplicationModeType, RuntimeEnvironmentType, UrlTypeType
 from .paginator import ListApplicationSnapshotsPaginator, ListApplicationsPaginator
 from .type_defs import (
@@ -56,14 +55,15 @@
     OutputTypeDef,
     ReferenceDataSourceTypeDef,
     RollbackApplicationResponseTypeDef,
     RunConfigurationTypeDef,
     RunConfigurationUpdateTypeDef,
     S3ConfigurationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateApplicationMaintenanceConfigurationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -256,15 +256,15 @@
         Creates a snapshot of the application's state data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.create_application_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#create_application_snapshot)
         """
 
     async def delete_application(
-        self, *, ApplicationName: str, CreateTimestamp: Union[datetime, str]
+        self, *, ApplicationName: str, CreateTimestamp: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         Deletes the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#delete_application)
         """
@@ -318,15 +318,15 @@
         """
 
     async def delete_application_snapshot(
         self,
         *,
         ApplicationName: str,
         SnapshotName: str,
-        SnapshotCreationTimestamp: Union[datetime, str]
+        SnapshotCreationTimestamp: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         Deletes a snapshot of application state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#delete_application_snapshot)
         """
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/client.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("kinesisanalyticsv2") as client:
         client: KinesisAnalyticsV2Client
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ApplicationModeType, RuntimeEnvironmentType, UrlTypeType
 from .paginator import ListApplicationSnapshotsPaginator, ListApplicationsPaginator
 from .type_defs import (
@@ -56,14 +55,15 @@
     OutputTypeDef,
     ReferenceDataSourceTypeDef,
     RollbackApplicationResponseTypeDef,
     RunConfigurationTypeDef,
     RunConfigurationUpdateTypeDef,
     S3ConfigurationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateApplicationMaintenanceConfigurationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
     VpcConfigurationTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -240,15 +240,15 @@
         """
         Creates a snapshot of the application's state data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.create_application_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#create_application_snapshot)
         """
     async def delete_application(
-        self, *, ApplicationName: str, CreateTimestamp: Union[datetime, str]
+        self, *, ApplicationName: str, CreateTimestamp: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         Deletes the specified application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#delete_application)
         """
@@ -297,15 +297,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#delete_application_reference_data_source)
         """
     async def delete_application_snapshot(
         self,
         *,
         ApplicationName: str,
         SnapshotName: str,
-        SnapshotCreationTimestamp: Union[datetime, str]
+        SnapshotCreationTimestamp: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         Deletes a snapshot of application state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#delete_application_snapshot)
         """
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/literals.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/literals.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/paginator.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -31,46 +31,42 @@
     ListApplicationSnapshotsResponseTypeDef,
     ListApplicationsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListApplicationSnapshotsPaginator", "ListApplicationsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListApplicationSnapshotsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplicationSnapshots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/paginators/#listapplicationsnapshotspaginator)
     """
 
     def paginate(
-        self, *, ApplicationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApplicationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplicationSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/paginators/#listapplicationsnapshotspaginator)
         """
 
-
 class ListApplicationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplications)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/paginators/#listapplicationspaginator)
         """
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/paginator.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,42 +31,46 @@
     ListApplicationSnapshotsResponseTypeDef,
     ListApplicationsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListApplicationSnapshotsPaginator", "ListApplicationsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListApplicationSnapshotsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplicationSnapshots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/paginators/#listapplicationsnapshotspaginator)
     """
 
     def paginate(
-        self, *, ApplicationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApplicationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplicationSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/paginators/#listapplicationsnapshotspaginator)
         """
 
+
 class ListApplicationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplications)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/paginators/#listapplicationspaginator)
         """
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/type_defs.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_kinesisanalyticsv2.type_defs import CloudWatchLoggingOptionTypeDef
 
-    data: CloudWatchLoggingOptionTypeDef = {...}
+    data: CloudWatchLoggingOptionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -38,63 +38,60 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "VpcConfigurationTypeDef",
     "VpcConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationTypeDef",
     "ApplicationSnapshotConfigurationUpdateTypeDef",
     "VpcConfigurationUpdateTypeDef",
     "ApplicationMaintenanceConfigurationDescriptionTypeDef",
     "ApplicationMaintenanceConfigurationUpdateTypeDef",
     "ApplicationRestoreConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
+    "BlobTypeDef",
     "CSVMappingParametersTypeDef",
     "GlueDataCatalogConfigurationDescriptionTypeDef",
     "GlueDataCatalogConfigurationTypeDef",
     "GlueDataCatalogConfigurationUpdateTypeDef",
     "CheckpointConfigurationDescriptionTypeDef",
     "CheckpointConfigurationTypeDef",
     "CheckpointConfigurationUpdateTypeDef",
     "CloudWatchLoggingOptionUpdateTypeDef",
     "S3ApplicationCodeLocationDescriptionTypeDef",
     "S3ContentLocationTypeDef",
     "S3ContentLocationUpdateTypeDef",
     "CreateApplicationPresignedUrlRequestRequestTypeDef",
-    "CreateApplicationPresignedUrlResponseTypeDef",
     "TagTypeDef",
     "CreateApplicationSnapshotRequestRequestTypeDef",
     "MavenReferenceTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
-    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
-    "DeleteApplicationOutputResponseTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
-    "DeleteApplicationReferenceDataSourceResponseTypeDef",
-    "DeleteApplicationRequestRequestTypeDef",
-    "DeleteApplicationSnapshotRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DeleteApplicationVpcConfigurationRequestRequestTypeDef",
-    "DeleteApplicationVpcConfigurationResponseTypeDef",
     "S3ContentBaseLocationDescriptionTypeDef",
     "S3ContentBaseLocationTypeDef",
     "S3ContentBaseLocationUpdateTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeApplicationSnapshotRequestRequestTypeDef",
     "SnapshotDetailsTypeDef",
     "DescribeApplicationVersionRequestRequestTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
     "PropertyGroupTypeDef",
+    "PropertyGroupOutputTypeDef",
     "MonitoringConfigurationDescriptionTypeDef",
     "ParallelismConfigurationDescriptionTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParallelismConfigurationTypeDef",
     "MonitoringConfigurationUpdateTypeDef",
     "ParallelismConfigurationUpdateTypeDef",
     "FlinkRunConfigurationTypeDef",
@@ -116,34 +113,36 @@
     "KinesisFirehoseOutputUpdateTypeDef",
     "KinesisStreamsOutputDescriptionTypeDef",
     "KinesisStreamsOutputTypeDef",
     "KinesisStreamsOutputUpdateTypeDef",
     "LambdaOutputDescriptionTypeDef",
     "LambdaOutputTypeDef",
     "LambdaOutputUpdateTypeDef",
-    "ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationSnapshotsRequestRequestTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "S3ReferenceDataSourceDescriptionTypeDef",
     "S3ReferenceDataSourceTypeDef",
     "S3ReferenceDataSourceUpdateTypeDef",
-    "ResponseMetadataTypeDef",
     "RollbackApplicationRequestRequestTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ZeppelinMonitoringConfigurationDescriptionTypeDef",
     "ZeppelinMonitoringConfigurationTypeDef",
     "ZeppelinMonitoringConfigurationUpdateTypeDef",
     "AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "AddApplicationCloudWatchLoggingOptionResponseTypeDef",
+    "CreateApplicationPresignedUrlResponseTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionResponseTypeDef",
+    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
+    "DeleteApplicationOutputResponseTypeDef",
+    "DeleteApplicationReferenceDataSourceResponseTypeDef",
+    "DeleteApplicationVpcConfigurationResponseTypeDef",
     "AddApplicationVpcConfigurationRequestRequestTypeDef",
     "AddApplicationVpcConfigurationResponseTypeDef",
     "UpdateApplicationMaintenanceConfigurationResponseTypeDef",
     "UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "CatalogConfigurationDescriptionTypeDef",
@@ -152,35 +151,39 @@
     "CodeContentDescriptionTypeDef",
     "CodeContentTypeDef",
     "CodeContentUpdateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomArtifactConfigurationDescriptionTypeDef",
     "CustomArtifactConfigurationTypeDef",
+    "DeleteApplicationRequestRequestTypeDef",
+    "DeleteApplicationSnapshotRequestRequestTypeDef",
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     "DeployAsApplicationConfigurationTypeDef",
     "DeployAsApplicationConfigurationUpdateTypeDef",
     "DescribeApplicationSnapshotResponseTypeDef",
     "ListApplicationSnapshotsResponseTypeDef",
     "SqlRunConfigurationTypeDef",
     "EnvironmentPropertiesTypeDef",
-    "EnvironmentPropertyDescriptionsTypeDef",
     "EnvironmentPropertyUpdatesTypeDef",
+    "EnvironmentPropertyDescriptionsTypeDef",
     "FlinkApplicationConfigurationDescriptionTypeDef",
     "FlinkApplicationConfigurationTypeDef",
     "FlinkApplicationConfigurationUpdateTypeDef",
     "RunConfigurationDescriptionTypeDef",
     "RunConfigurationUpdateTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
     "OutputUpdateTypeDef",
+    "ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ApplicationCodeConfigurationDescriptionTypeDef",
     "ApplicationCodeConfigurationTypeDef",
     "ApplicationCodeConfigurationUpdateTypeDef",
     "ZeppelinApplicationConfigurationDescriptionTypeDef",
     "ZeppelinApplicationConfigurationTypeDef",
     "ZeppelinApplicationConfigurationUpdateTypeDef",
     "RunConfigurationTypeDef",
@@ -188,26 +191,27 @@
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputResponseTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "InputSchemaUpdateTypeDef",
+    "SourceSchemaOutputTypeDef",
     "SourceSchemaTypeDef",
     "InputUpdateTypeDef",
     "DiscoverInputSchemaResponseTypeDef",
     "InputDescriptionTypeDef",
-    "InputTypeDef",
     "ReferenceDataSourceDescriptionTypeDef",
+    "InputTypeDef",
     "ReferenceDataSourceTypeDef",
     "ReferenceDataSourceUpdateTypeDef",
     "AddApplicationInputResponseTypeDef",
-    "AddApplicationInputRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceResponseTypeDef",
     "SqlApplicationConfigurationDescriptionTypeDef",
+    "AddApplicationInputRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     "SqlApplicationConfigurationTypeDef",
     "SqlApplicationConfigurationUpdateTypeDef",
     "ApplicationConfigurationDescriptionTypeDef",
     "ApplicationConfigurationTypeDef",
     "ApplicationConfigurationUpdateTypeDef",
     "ApplicationDetailTypeDef",
@@ -246,14 +250,25 @@
 class CloudWatchLoggingOptionDescriptionTypeDef(
     _RequiredCloudWatchLoggingOptionDescriptionTypeDef,
     _OptionalCloudWatchLoggingOptionDescriptionTypeDef,
 ):
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
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
 )
@@ -376,14 +391,15 @@
     "ApplicationVersionSummaryTypeDef",
     {
         "ApplicationVersionId": int,
         "ApplicationStatus": ApplicationStatusType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CSVMappingParametersTypeDef = TypedDict(
     "CSVMappingParametersTypeDef",
     {
         "RecordRowDelimiter": str,
         "RecordColumnDelimiter": str,
     },
 )
@@ -549,22 +565,14 @@
 class CreateApplicationPresignedUrlRequestRequestTypeDef(
     _RequiredCreateApplicationPresignedUrlRequestRequestTypeDef,
     _OptionalCreateApplicationPresignedUrlRequestRequestTypeDef,
 ):
     pass
 
 
-CreateApplicationPresignedUrlResponseTypeDef = TypedDict(
-    "CreateApplicationPresignedUrlResponseTypeDef",
-    {
-        "AuthorizedUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -626,76 +634,33 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "InputId": str,
     },
 )
 
-DeleteApplicationInputProcessingConfigurationResponseTypeDef = TypedDict(
-    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationOutputRequestRequestTypeDef = TypedDict(
     "DeleteApplicationOutputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "OutputId": str,
     },
 )
 
-DeleteApplicationOutputResponseTypeDef = TypedDict(
-    "DeleteApplicationOutputResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceId": str,
     },
 )
 
-DeleteApplicationReferenceDataSourceResponseTypeDef = TypedDict(
-    "DeleteApplicationReferenceDataSourceResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteApplicationRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "CreateTimestamp": Union[datetime, str],
-    },
-)
-
-DeleteApplicationSnapshotRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationSnapshotRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "SnapshotName": str,
-        "SnapshotCreationTimestamp": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "VpcConfigurationId": str,
     },
 )
@@ -712,23 +677,14 @@
 class DeleteApplicationVpcConfigurationRequestRequestTypeDef(
     _RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef,
     _OptionalDeleteApplicationVpcConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-DeleteApplicationVpcConfigurationResponseTypeDef = TypedDict(
-    "DeleteApplicationVpcConfigurationResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredS3ContentBaseLocationDescriptionTypeDef = TypedDict(
     "_RequiredS3ContentBaseLocationDescriptionTypeDef",
     {
         "BucketARN": str,
     },
 )
 _OptionalS3ContentBaseLocationDescriptionTypeDef = TypedDict(
@@ -863,14 +819,22 @@
     "PropertyGroupTypeDef",
     {
         "PropertyGroupId": str,
         "PropertyMap": Mapping[str, str],
     },
 )
 
+PropertyGroupOutputTypeDef = TypedDict(
+    "PropertyGroupOutputTypeDef",
+    {
+        "PropertyGroupId": str,
+        "PropertyMap": Dict[str, str],
+    },
+)
+
 MonitoringConfigurationDescriptionTypeDef = TypedDict(
     "MonitoringConfigurationDescriptionTypeDef",
     {
         "ConfigurationType": ConfigurationTypeType,
         "MetricsLevel": MetricsLevelType,
         "LogLevel": LogLevelType,
     },
@@ -1212,36 +1176,24 @@
 LambdaOutputUpdateTypeDef = TypedDict(
     "LambdaOutputUpdateTypeDef",
     {
         "ResourceARNUpdate": str,
     },
 )
 
-_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-    },
-)
-_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
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
-class ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef(
-    _RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
-    _OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListApplicationSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationSnapshotsRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 _OptionalListApplicationSnapshotsRequestRequestTypeDef = TypedDict(
@@ -1280,22 +1232,14 @@
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
@@ -1304,24 +1248,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 _RequiredS3ReferenceDataSourceDescriptionTypeDef = TypedDict(
     "_RequiredS3ReferenceDataSourceDescriptionTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
     },
 )
@@ -1355,25 +1289,14 @@
     {
         "BucketARNUpdate": str,
         "FileKeyUpdate": str,
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
 RollbackApplicationRequestRequestTypeDef = TypedDict(
     "RollbackApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
     },
 )
@@ -1455,25 +1378,69 @@
 
 AddApplicationCloudWatchLoggingOptionResponseTypeDef = TypedDict(
     "AddApplicationCloudWatchLoggingOptionResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationPresignedUrlResponseTypeDef = TypedDict(
+    "CreateApplicationPresignedUrlResponseTypeDef",
+    {
+        "AuthorizedUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteApplicationCloudWatchLoggingOptionResponseTypeDef = TypedDict(
     "DeleteApplicationCloudWatchLoggingOptionResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationInputProcessingConfigurationResponseTypeDef = TypedDict(
+    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationOutputResponseTypeDef = TypedDict(
+    "DeleteApplicationOutputResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationReferenceDataSourceResponseTypeDef = TypedDict(
+    "DeleteApplicationReferenceDataSourceResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationVpcConfigurationResponseTypeDef = TypedDict(
+    "DeleteApplicationVpcConfigurationResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAddApplicationVpcConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredAddApplicationVpcConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1499,26 +1466,26 @@
 
 AddApplicationVpcConfigurationResponseTypeDef = TypedDict(
     "AddApplicationVpcConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationMaintenanceConfigurationResponseTypeDef = TypedDict(
     "UpdateApplicationMaintenanceConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationMaintenanceConfigurationDescription": (
             ApplicationMaintenanceConfigurationDescriptionTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1529,24 +1496,24 @@
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationSummaries": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationVersionsResponseTypeDef = TypedDict(
     "ListApplicationVersionsResponseTypeDef",
     {
         "ApplicationVersionSummaries": List[ApplicationVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CatalogConfigurationDescriptionTypeDef = TypedDict(
     "CatalogConfigurationDescriptionTypeDef",
     {
         "GlueDataCatalogConfigurationDescription": GlueDataCatalogConfigurationDescriptionTypeDef,
@@ -1578,35 +1545,35 @@
     total=False,
 )
 
 CodeContentTypeDef = TypedDict(
     "CodeContentTypeDef",
     {
         "TextContent": str,
-        "ZipFileContent": Union[str, bytes, IO[Any], StreamingBody],
+        "ZipFileContent": BlobTypeDef,
         "S3ContentLocation": S3ContentLocationTypeDef,
     },
     total=False,
 )
 
 CodeContentUpdateTypeDef = TypedDict(
     "CodeContentUpdateTypeDef",
     {
         "TextContentUpdate": str,
-        "ZipFileContentUpdate": Union[str, bytes, IO[Any], StreamingBody],
+        "ZipFileContentUpdate": BlobTypeDef,
         "S3ContentLocationUpdate": S3ContentLocationUpdateTypeDef,
     },
     total=False,
 )
 
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
@@ -1642,14 +1609,31 @@
 
 class CustomArtifactConfigurationTypeDef(
     _RequiredCustomArtifactConfigurationTypeDef, _OptionalCustomArtifactConfigurationTypeDef
 ):
     pass
 
 
+DeleteApplicationRequestRequestTypeDef = TypedDict(
+    "DeleteApplicationRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "CreateTimestamp": TimestampTypeDef,
+    },
+)
+
+DeleteApplicationSnapshotRequestRequestTypeDef = TypedDict(
+    "DeleteApplicationSnapshotRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "SnapshotName": str,
+        "SnapshotCreationTimestamp": TimestampTypeDef,
+    },
+)
+
 DeployAsApplicationConfigurationDescriptionTypeDef = TypedDict(
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     {
         "S3ContentLocationDescription": S3ContentBaseLocationDescriptionTypeDef,
     },
 )
 
@@ -1668,24 +1652,24 @@
     total=False,
 )
 
 DescribeApplicationSnapshotResponseTypeDef = TypedDict(
     "DescribeApplicationSnapshotResponseTypeDef",
     {
         "SnapshotDetails": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationSnapshotsResponseTypeDef = TypedDict(
     "ListApplicationSnapshotsResponseTypeDef",
     {
         "SnapshotSummaries": List[SnapshotDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SqlRunConfigurationTypeDef = TypedDict(
     "SqlRunConfigurationTypeDef",
     {
         "InputId": str,
@@ -1696,27 +1680,27 @@
 EnvironmentPropertiesTypeDef = TypedDict(
     "EnvironmentPropertiesTypeDef",
     {
         "PropertyGroups": Sequence[PropertyGroupTypeDef],
     },
 )
 
-EnvironmentPropertyDescriptionsTypeDef = TypedDict(
-    "EnvironmentPropertyDescriptionsTypeDef",
+EnvironmentPropertyUpdatesTypeDef = TypedDict(
+    "EnvironmentPropertyUpdatesTypeDef",
     {
-        "PropertyGroupDescriptions": List[PropertyGroupTypeDef],
+        "PropertyGroups": Sequence[PropertyGroupTypeDef],
     },
-    total=False,
 )
 
-EnvironmentPropertyUpdatesTypeDef = TypedDict(
-    "EnvironmentPropertyUpdatesTypeDef",
+EnvironmentPropertyDescriptionsTypeDef = TypedDict(
+    "EnvironmentPropertyDescriptionsTypeDef",
     {
-        "PropertyGroups": Sequence[PropertyGroupTypeDef],
+        "PropertyGroupDescriptions": List[PropertyGroupOutputTypeDef],
     },
+    total=False,
 )
 
 FlinkApplicationConfigurationDescriptionTypeDef = TypedDict(
     "FlinkApplicationConfigurationDescriptionTypeDef",
     {
         "CheckpointConfigurationDescription": CheckpointConfigurationDescriptionTypeDef,
         "MonitoringConfigurationDescription": MonitoringConfigurationDescriptionTypeDef,
@@ -1849,14 +1833,44 @@
 )
 
 
 class OutputUpdateTypeDef(_RequiredOutputUpdateTypeDef, _OptionalOutputUpdateTypeDef):
     pass
 
 
+_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+    },
+)
+_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef(
+    _RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    _OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+):
+    pass
+
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredApplicationCodeConfigurationDescriptionTypeDef = TypedDict(
     "_RequiredApplicationCodeConfigurationDescriptionTypeDef",
     {
         "CodeContentType": CodeContentTypeType,
     },
 )
 _OptionalApplicationCodeConfigurationDescriptionTypeDef = TypedDict(
@@ -1968,15 +1982,15 @@
 AddApplicationInputProcessingConfigurationResponseTypeDef = TypedDict(
     "AddApplicationInputProcessingConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "InputId": str,
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddApplicationInputProcessingConfigurationRequestRequestTypeDef = TypedDict(
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -2032,15 +2046,15 @@
 
 AddApplicationOutputResponseTypeDef = TypedDict(
     "AddApplicationOutputResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "OutputDescriptions": List[OutputDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddApplicationOutputRequestRequestTypeDef = TypedDict(
     "AddApplicationOutputRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -2076,14 +2090,36 @@
         "RecordFormatUpdate": RecordFormatTypeDef,
         "RecordEncodingUpdate": str,
         "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
     },
     total=False,
 )
 
+_RequiredSourceSchemaOutputTypeDef = TypedDict(
+    "_RequiredSourceSchemaOutputTypeDef",
+    {
+        "RecordFormat": RecordFormatTypeDef,
+        "RecordColumns": List[RecordColumnTypeDef],
+    },
+)
+_OptionalSourceSchemaOutputTypeDef = TypedDict(
+    "_OptionalSourceSchemaOutputTypeDef",
+    {
+        "RecordEncoding": str,
+    },
+    total=False,
+)
+
+
+class SourceSchemaOutputTypeDef(
+    _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
+):
+    pass
+
+
 _RequiredSourceSchemaTypeDef = TypedDict(
     "_RequiredSourceSchemaTypeDef",
     {
         "RecordFormat": RecordFormatTypeDef,
         "RecordColumns": Sequence[RecordColumnTypeDef],
     },
 )
@@ -2123,81 +2159,81 @@
 class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
     pass
 
 
 DiscoverInputSchemaResponseTypeDef = TypedDict(
     "DiscoverInputSchemaResponseTypeDef",
     {
-        "InputSchema": SourceSchemaTypeDef,
+        "InputSchema": SourceSchemaOutputTypeDef,
         "ParsedInputRecords": List[List[str]],
         "ProcessedInputRecords": List[str],
         "RawInputRecords": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputDescriptionTypeDef = TypedDict(
     "InputDescriptionTypeDef",
     {
         "InputId": str,
         "NamePrefix": str,
         "InAppStreamNames": List[str],
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
         "KinesisStreamsInputDescription": KinesisStreamsInputDescriptionTypeDef,
         "KinesisFirehoseInputDescription": KinesisFirehoseInputDescriptionTypeDef,
-        "InputSchema": SourceSchemaTypeDef,
+        "InputSchema": SourceSchemaOutputTypeDef,
         "InputParallelism": InputParallelismTypeDef,
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredInputTypeDef = TypedDict(
-    "_RequiredInputTypeDef",
+_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_RequiredReferenceDataSourceDescriptionTypeDef",
     {
-        "NamePrefix": str,
-        "InputSchema": SourceSchemaTypeDef,
+        "ReferenceId": str,
+        "TableName": str,
+        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
     },
 )
-_OptionalInputTypeDef = TypedDict(
-    "_OptionalInputTypeDef",
+_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_OptionalReferenceDataSourceDescriptionTypeDef",
     {
-        "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
-        "KinesisStreamsInput": KinesisStreamsInputTypeDef,
-        "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
-        "InputParallelism": InputParallelismTypeDef,
+        "ReferenceSchema": SourceSchemaOutputTypeDef,
     },
     total=False,
 )
 
 
-class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
+class ReferenceDataSourceDescriptionTypeDef(
+    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
+):
     pass
 
 
-_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_RequiredReferenceDataSourceDescriptionTypeDef",
+_RequiredInputTypeDef = TypedDict(
+    "_RequiredInputTypeDef",
     {
-        "ReferenceId": str,
-        "TableName": str,
-        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
+        "NamePrefix": str,
+        "InputSchema": SourceSchemaTypeDef,
     },
 )
-_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_OptionalReferenceDataSourceDescriptionTypeDef",
+_OptionalInputTypeDef = TypedDict(
+    "_OptionalInputTypeDef",
     {
-        "ReferenceSchema": SourceSchemaTypeDef,
+        "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
+        "KinesisStreamsInput": KinesisStreamsInputTypeDef,
+        "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
+        "InputParallelism": InputParallelismTypeDef,
     },
     total=False,
 )
 
 
-class ReferenceDataSourceDescriptionTypeDef(
-    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
-):
+class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
     pass
 
 
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
@@ -2244,47 +2280,47 @@
 
 AddApplicationInputResponseTypeDef = TypedDict(
     "AddApplicationInputResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "InputDescriptions": List[InputDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AddApplicationInputRequestRequestTypeDef = TypedDict(
-    "AddApplicationInputRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "CurrentApplicationVersionId": int,
-        "Input": InputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddApplicationReferenceDataSourceResponseTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SqlApplicationConfigurationDescriptionTypeDef = TypedDict(
     "SqlApplicationConfigurationDescriptionTypeDef",
     {
         "InputDescriptions": List[InputDescriptionTypeDef],
         "OutputDescriptions": List[OutputDescriptionTypeDef],
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
     },
     total=False,
 )
 
+AddApplicationInputRequestRequestTypeDef = TypedDict(
+    "AddApplicationInputRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "CurrentApplicationVersionId": int,
+        "Input": InputTypeDef,
+    },
+)
+
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
@@ -2448,42 +2484,42 @@
     pass
 
 
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationVersionResponseTypeDef = TypedDict(
     "DescribeApplicationVersionResponseTypeDef",
     {
         "ApplicationVersionDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RollbackApplicationResponseTypeDef = TypedDict(
     "RollbackApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_kinesisanalyticsv2.type_defs import CloudWatchLoggingOptionTypeDef
 
-    data: CloudWatchLoggingOptionTypeDef = {...}
+    data: CloudWatchLoggingOptionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -37,63 +37,60 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "VpcConfigurationTypeDef",
     "VpcConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationTypeDef",
     "ApplicationSnapshotConfigurationUpdateTypeDef",
     "VpcConfigurationUpdateTypeDef",
     "ApplicationMaintenanceConfigurationDescriptionTypeDef",
     "ApplicationMaintenanceConfigurationUpdateTypeDef",
     "ApplicationRestoreConfigurationTypeDef",
     "ApplicationSummaryTypeDef",
     "ApplicationVersionSummaryTypeDef",
+    "BlobTypeDef",
     "CSVMappingParametersTypeDef",
     "GlueDataCatalogConfigurationDescriptionTypeDef",
     "GlueDataCatalogConfigurationTypeDef",
     "GlueDataCatalogConfigurationUpdateTypeDef",
     "CheckpointConfigurationDescriptionTypeDef",
     "CheckpointConfigurationTypeDef",
     "CheckpointConfigurationUpdateTypeDef",
     "CloudWatchLoggingOptionUpdateTypeDef",
     "S3ApplicationCodeLocationDescriptionTypeDef",
     "S3ContentLocationTypeDef",
     "S3ContentLocationUpdateTypeDef",
     "CreateApplicationPresignedUrlRequestRequestTypeDef",
-    "CreateApplicationPresignedUrlResponseTypeDef",
     "TagTypeDef",
     "CreateApplicationSnapshotRequestRequestTypeDef",
     "MavenReferenceTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
-    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
-    "DeleteApplicationOutputResponseTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
-    "DeleteApplicationReferenceDataSourceResponseTypeDef",
-    "DeleteApplicationRequestRequestTypeDef",
-    "DeleteApplicationSnapshotRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DeleteApplicationVpcConfigurationRequestRequestTypeDef",
-    "DeleteApplicationVpcConfigurationResponseTypeDef",
     "S3ContentBaseLocationDescriptionTypeDef",
     "S3ContentBaseLocationTypeDef",
     "S3ContentBaseLocationUpdateTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeApplicationSnapshotRequestRequestTypeDef",
     "SnapshotDetailsTypeDef",
     "DescribeApplicationVersionRequestRequestTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
     "PropertyGroupTypeDef",
+    "PropertyGroupOutputTypeDef",
     "MonitoringConfigurationDescriptionTypeDef",
     "ParallelismConfigurationDescriptionTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParallelismConfigurationTypeDef",
     "MonitoringConfigurationUpdateTypeDef",
     "ParallelismConfigurationUpdateTypeDef",
     "FlinkRunConfigurationTypeDef",
@@ -115,34 +112,36 @@
     "KinesisFirehoseOutputUpdateTypeDef",
     "KinesisStreamsOutputDescriptionTypeDef",
     "KinesisStreamsOutputTypeDef",
     "KinesisStreamsOutputUpdateTypeDef",
     "LambdaOutputDescriptionTypeDef",
     "LambdaOutputTypeDef",
     "LambdaOutputUpdateTypeDef",
-    "ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationSnapshotsRequestRequestTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "S3ReferenceDataSourceDescriptionTypeDef",
     "S3ReferenceDataSourceTypeDef",
     "S3ReferenceDataSourceUpdateTypeDef",
-    "ResponseMetadataTypeDef",
     "RollbackApplicationRequestRequestTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ZeppelinMonitoringConfigurationDescriptionTypeDef",
     "ZeppelinMonitoringConfigurationTypeDef",
     "ZeppelinMonitoringConfigurationUpdateTypeDef",
     "AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "AddApplicationCloudWatchLoggingOptionResponseTypeDef",
+    "CreateApplicationPresignedUrlResponseTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionResponseTypeDef",
+    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
+    "DeleteApplicationOutputResponseTypeDef",
+    "DeleteApplicationReferenceDataSourceResponseTypeDef",
+    "DeleteApplicationVpcConfigurationResponseTypeDef",
     "AddApplicationVpcConfigurationRequestRequestTypeDef",
     "AddApplicationVpcConfigurationResponseTypeDef",
     "UpdateApplicationMaintenanceConfigurationResponseTypeDef",
     "UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "CatalogConfigurationDescriptionTypeDef",
@@ -151,35 +150,39 @@
     "CodeContentDescriptionTypeDef",
     "CodeContentTypeDef",
     "CodeContentUpdateTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomArtifactConfigurationDescriptionTypeDef",
     "CustomArtifactConfigurationTypeDef",
+    "DeleteApplicationRequestRequestTypeDef",
+    "DeleteApplicationSnapshotRequestRequestTypeDef",
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     "DeployAsApplicationConfigurationTypeDef",
     "DeployAsApplicationConfigurationUpdateTypeDef",
     "DescribeApplicationSnapshotResponseTypeDef",
     "ListApplicationSnapshotsResponseTypeDef",
     "SqlRunConfigurationTypeDef",
     "EnvironmentPropertiesTypeDef",
-    "EnvironmentPropertyDescriptionsTypeDef",
     "EnvironmentPropertyUpdatesTypeDef",
+    "EnvironmentPropertyDescriptionsTypeDef",
     "FlinkApplicationConfigurationDescriptionTypeDef",
     "FlinkApplicationConfigurationTypeDef",
     "FlinkApplicationConfigurationUpdateTypeDef",
     "RunConfigurationDescriptionTypeDef",
     "RunConfigurationUpdateTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
     "OutputUpdateTypeDef",
+    "ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ApplicationCodeConfigurationDescriptionTypeDef",
     "ApplicationCodeConfigurationTypeDef",
     "ApplicationCodeConfigurationUpdateTypeDef",
     "ZeppelinApplicationConfigurationDescriptionTypeDef",
     "ZeppelinApplicationConfigurationTypeDef",
     "ZeppelinApplicationConfigurationUpdateTypeDef",
     "RunConfigurationTypeDef",
@@ -187,26 +190,27 @@
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputResponseTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "InputSchemaUpdateTypeDef",
+    "SourceSchemaOutputTypeDef",
     "SourceSchemaTypeDef",
     "InputUpdateTypeDef",
     "DiscoverInputSchemaResponseTypeDef",
     "InputDescriptionTypeDef",
-    "InputTypeDef",
     "ReferenceDataSourceDescriptionTypeDef",
+    "InputTypeDef",
     "ReferenceDataSourceTypeDef",
     "ReferenceDataSourceUpdateTypeDef",
     "AddApplicationInputResponseTypeDef",
-    "AddApplicationInputRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceResponseTypeDef",
     "SqlApplicationConfigurationDescriptionTypeDef",
+    "AddApplicationInputRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     "SqlApplicationConfigurationTypeDef",
     "SqlApplicationConfigurationUpdateTypeDef",
     "ApplicationConfigurationDescriptionTypeDef",
     "ApplicationConfigurationTypeDef",
     "ApplicationConfigurationUpdateTypeDef",
     "ApplicationDetailTypeDef",
@@ -243,14 +247,25 @@
 
 class CloudWatchLoggingOptionDescriptionTypeDef(
     _RequiredCloudWatchLoggingOptionDescriptionTypeDef,
     _OptionalCloudWatchLoggingOptionDescriptionTypeDef,
 ):
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
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
 )
@@ -367,14 +382,15 @@
     "ApplicationVersionSummaryTypeDef",
     {
         "ApplicationVersionId": int,
         "ApplicationStatus": ApplicationStatusType,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CSVMappingParametersTypeDef = TypedDict(
     "CSVMappingParametersTypeDef",
     {
         "RecordRowDelimiter": str,
         "RecordColumnDelimiter": str,
     },
 )
@@ -530,22 +546,14 @@
 
 class CreateApplicationPresignedUrlRequestRequestTypeDef(
     _RequiredCreateApplicationPresignedUrlRequestRequestTypeDef,
     _OptionalCreateApplicationPresignedUrlRequestRequestTypeDef,
 ):
     pass
 
-CreateApplicationPresignedUrlResponseTypeDef = TypedDict(
-    "CreateApplicationPresignedUrlResponseTypeDef",
-    {
-        "AuthorizedUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalTagTypeDef = TypedDict(
@@ -603,76 +611,33 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "InputId": str,
     },
 )
 
-DeleteApplicationInputProcessingConfigurationResponseTypeDef = TypedDict(
-    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationOutputRequestRequestTypeDef = TypedDict(
     "DeleteApplicationOutputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "OutputId": str,
     },
 )
 
-DeleteApplicationOutputResponseTypeDef = TypedDict(
-    "DeleteApplicationOutputResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceId": str,
     },
 )
 
-DeleteApplicationReferenceDataSourceResponseTypeDef = TypedDict(
-    "DeleteApplicationReferenceDataSourceResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteApplicationRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "CreateTimestamp": Union[datetime, str],
-    },
-)
-
-DeleteApplicationSnapshotRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationSnapshotRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "SnapshotName": str,
-        "SnapshotCreationTimestamp": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "VpcConfigurationId": str,
     },
 )
@@ -687,23 +652,14 @@
 
 class DeleteApplicationVpcConfigurationRequestRequestTypeDef(
     _RequiredDeleteApplicationVpcConfigurationRequestRequestTypeDef,
     _OptionalDeleteApplicationVpcConfigurationRequestRequestTypeDef,
 ):
     pass
 
-DeleteApplicationVpcConfigurationResponseTypeDef = TypedDict(
-    "DeleteApplicationVpcConfigurationResponseTypeDef",
-    {
-        "ApplicationARN": str,
-        "ApplicationVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredS3ContentBaseLocationDescriptionTypeDef = TypedDict(
     "_RequiredS3ContentBaseLocationDescriptionTypeDef",
     {
         "BucketARN": str,
     },
 )
 _OptionalS3ContentBaseLocationDescriptionTypeDef = TypedDict(
@@ -830,14 +786,22 @@
     "PropertyGroupTypeDef",
     {
         "PropertyGroupId": str,
         "PropertyMap": Mapping[str, str],
     },
 )
 
+PropertyGroupOutputTypeDef = TypedDict(
+    "PropertyGroupOutputTypeDef",
+    {
+        "PropertyGroupId": str,
+        "PropertyMap": Dict[str, str],
+    },
+)
+
 MonitoringConfigurationDescriptionTypeDef = TypedDict(
     "MonitoringConfigurationDescriptionTypeDef",
     {
         "ConfigurationType": ConfigurationTypeType,
         "MetricsLevel": MetricsLevelType,
         "LogLevel": LogLevelType,
     },
@@ -1161,34 +1125,24 @@
 LambdaOutputUpdateTypeDef = TypedDict(
     "LambdaOutputUpdateTypeDef",
     {
         "ResourceARNUpdate": str,
     },
 )
 
-_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-    },
-)
-_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
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
 
-class ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef(
-    _RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
-    _OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
-):
-    pass
-
 _RequiredListApplicationSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationSnapshotsRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 _OptionalListApplicationSnapshotsRequestRequestTypeDef = TypedDict(
@@ -1223,22 +1177,14 @@
 
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
@@ -1247,24 +1193,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 _RequiredS3ReferenceDataSourceDescriptionTypeDef = TypedDict(
     "_RequiredS3ReferenceDataSourceDescriptionTypeDef",
     {
         "BucketARN": str,
         "FileKey": str,
     },
 )
@@ -1296,25 +1232,14 @@
     {
         "BucketARNUpdate": str,
         "FileKeyUpdate": str,
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
 RollbackApplicationRequestRequestTypeDef = TypedDict(
     "RollbackApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
     },
 )
@@ -1392,25 +1317,69 @@
 
 AddApplicationCloudWatchLoggingOptionResponseTypeDef = TypedDict(
     "AddApplicationCloudWatchLoggingOptionResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationPresignedUrlResponseTypeDef = TypedDict(
+    "CreateApplicationPresignedUrlResponseTypeDef",
+    {
+        "AuthorizedUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteApplicationCloudWatchLoggingOptionResponseTypeDef = TypedDict(
     "DeleteApplicationCloudWatchLoggingOptionResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationInputProcessingConfigurationResponseTypeDef = TypedDict(
+    "DeleteApplicationInputProcessingConfigurationResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationOutputResponseTypeDef = TypedDict(
+    "DeleteApplicationOutputResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationReferenceDataSourceResponseTypeDef = TypedDict(
+    "DeleteApplicationReferenceDataSourceResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationVpcConfigurationResponseTypeDef = TypedDict(
+    "DeleteApplicationVpcConfigurationResponseTypeDef",
+    {
+        "ApplicationARN": str,
+        "ApplicationVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAddApplicationVpcConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredAddApplicationVpcConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1434,26 +1403,26 @@
 
 AddApplicationVpcConfigurationResponseTypeDef = TypedDict(
     "AddApplicationVpcConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "VpcConfigurationDescription": VpcConfigurationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationMaintenanceConfigurationResponseTypeDef = TypedDict(
     "UpdateApplicationMaintenanceConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationMaintenanceConfigurationDescription": (
             ApplicationMaintenanceConfigurationDescriptionTypeDef
         ),
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1464,24 +1433,24 @@
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationSummaries": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationVersionsResponseTypeDef = TypedDict(
     "ListApplicationVersionsResponseTypeDef",
     {
         "ApplicationVersionSummaries": List[ApplicationVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CatalogConfigurationDescriptionTypeDef = TypedDict(
     "CatalogConfigurationDescriptionTypeDef",
     {
         "GlueDataCatalogConfigurationDescription": GlueDataCatalogConfigurationDescriptionTypeDef,
@@ -1513,35 +1482,35 @@
     total=False,
 )
 
 CodeContentTypeDef = TypedDict(
     "CodeContentTypeDef",
     {
         "TextContent": str,
-        "ZipFileContent": Union[str, bytes, IO[Any], StreamingBody],
+        "ZipFileContent": BlobTypeDef,
         "S3ContentLocation": S3ContentLocationTypeDef,
     },
     total=False,
 )
 
 CodeContentUpdateTypeDef = TypedDict(
     "CodeContentUpdateTypeDef",
     {
         "TextContentUpdate": str,
-        "ZipFileContentUpdate": Union[str, bytes, IO[Any], StreamingBody],
+        "ZipFileContentUpdate": BlobTypeDef,
         "S3ContentLocationUpdate": S3ContentLocationUpdateTypeDef,
     },
     total=False,
 )
 
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
@@ -1575,14 +1544,31 @@
 )
 
 class CustomArtifactConfigurationTypeDef(
     _RequiredCustomArtifactConfigurationTypeDef, _OptionalCustomArtifactConfigurationTypeDef
 ):
     pass
 
+DeleteApplicationRequestRequestTypeDef = TypedDict(
+    "DeleteApplicationRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "CreateTimestamp": TimestampTypeDef,
+    },
+)
+
+DeleteApplicationSnapshotRequestRequestTypeDef = TypedDict(
+    "DeleteApplicationSnapshotRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "SnapshotName": str,
+        "SnapshotCreationTimestamp": TimestampTypeDef,
+    },
+)
+
 DeployAsApplicationConfigurationDescriptionTypeDef = TypedDict(
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     {
         "S3ContentLocationDescription": S3ContentBaseLocationDescriptionTypeDef,
     },
 )
 
@@ -1601,24 +1587,24 @@
     total=False,
 )
 
 DescribeApplicationSnapshotResponseTypeDef = TypedDict(
     "DescribeApplicationSnapshotResponseTypeDef",
     {
         "SnapshotDetails": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationSnapshotsResponseTypeDef = TypedDict(
     "ListApplicationSnapshotsResponseTypeDef",
     {
         "SnapshotSummaries": List[SnapshotDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SqlRunConfigurationTypeDef = TypedDict(
     "SqlRunConfigurationTypeDef",
     {
         "InputId": str,
@@ -1629,27 +1615,27 @@
 EnvironmentPropertiesTypeDef = TypedDict(
     "EnvironmentPropertiesTypeDef",
     {
         "PropertyGroups": Sequence[PropertyGroupTypeDef],
     },
 )
 
-EnvironmentPropertyDescriptionsTypeDef = TypedDict(
-    "EnvironmentPropertyDescriptionsTypeDef",
+EnvironmentPropertyUpdatesTypeDef = TypedDict(
+    "EnvironmentPropertyUpdatesTypeDef",
     {
-        "PropertyGroupDescriptions": List[PropertyGroupTypeDef],
+        "PropertyGroups": Sequence[PropertyGroupTypeDef],
     },
-    total=False,
 )
 
-EnvironmentPropertyUpdatesTypeDef = TypedDict(
-    "EnvironmentPropertyUpdatesTypeDef",
+EnvironmentPropertyDescriptionsTypeDef = TypedDict(
+    "EnvironmentPropertyDescriptionsTypeDef",
     {
-        "PropertyGroups": Sequence[PropertyGroupTypeDef],
+        "PropertyGroupDescriptions": List[PropertyGroupOutputTypeDef],
     },
+    total=False,
 )
 
 FlinkApplicationConfigurationDescriptionTypeDef = TypedDict(
     "FlinkApplicationConfigurationDescriptionTypeDef",
     {
         "CheckpointConfigurationDescription": CheckpointConfigurationDescriptionTypeDef,
         "MonitoringConfigurationDescription": MonitoringConfigurationDescriptionTypeDef,
@@ -1778,14 +1764,42 @@
     },
     total=False,
 )
 
 class OutputUpdateTypeDef(_RequiredOutputUpdateTypeDef, _OptionalOutputUpdateTypeDef):
     pass
 
+_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+    },
+)
+_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef(
+    _RequiredListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    _OptionalListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+):
+    pass
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredApplicationCodeConfigurationDescriptionTypeDef = TypedDict(
     "_RequiredApplicationCodeConfigurationDescriptionTypeDef",
     {
         "CodeContentType": CodeContentTypeType,
     },
 )
 _OptionalApplicationCodeConfigurationDescriptionTypeDef = TypedDict(
@@ -1891,15 +1905,15 @@
 AddApplicationInputProcessingConfigurationResponseTypeDef = TypedDict(
     "AddApplicationInputProcessingConfigurationResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "InputId": str,
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddApplicationInputProcessingConfigurationRequestRequestTypeDef = TypedDict(
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1951,15 +1965,15 @@
 
 AddApplicationOutputResponseTypeDef = TypedDict(
     "AddApplicationOutputResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "OutputDescriptions": List[OutputDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddApplicationOutputRequestRequestTypeDef = TypedDict(
     "AddApplicationOutputRequestRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1993,14 +2007,34 @@
         "RecordFormatUpdate": RecordFormatTypeDef,
         "RecordEncodingUpdate": str,
         "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
     },
     total=False,
 )
 
+_RequiredSourceSchemaOutputTypeDef = TypedDict(
+    "_RequiredSourceSchemaOutputTypeDef",
+    {
+        "RecordFormat": RecordFormatTypeDef,
+        "RecordColumns": List[RecordColumnTypeDef],
+    },
+)
+_OptionalSourceSchemaOutputTypeDef = TypedDict(
+    "_OptionalSourceSchemaOutputTypeDef",
+    {
+        "RecordEncoding": str,
+    },
+    total=False,
+)
+
+class SourceSchemaOutputTypeDef(
+    _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
+):
+    pass
+
 _RequiredSourceSchemaTypeDef = TypedDict(
     "_RequiredSourceSchemaTypeDef",
     {
         "RecordFormat": RecordFormatTypeDef,
         "RecordColumns": Sequence[RecordColumnTypeDef],
     },
 )
@@ -2036,38 +2070,59 @@
 
 class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
     pass
 
 DiscoverInputSchemaResponseTypeDef = TypedDict(
     "DiscoverInputSchemaResponseTypeDef",
     {
-        "InputSchema": SourceSchemaTypeDef,
+        "InputSchema": SourceSchemaOutputTypeDef,
         "ParsedInputRecords": List[List[str]],
         "ProcessedInputRecords": List[str],
         "RawInputRecords": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputDescriptionTypeDef = TypedDict(
     "InputDescriptionTypeDef",
     {
         "InputId": str,
         "NamePrefix": str,
         "InAppStreamNames": List[str],
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
         "KinesisStreamsInputDescription": KinesisStreamsInputDescriptionTypeDef,
         "KinesisFirehoseInputDescription": KinesisFirehoseInputDescriptionTypeDef,
-        "InputSchema": SourceSchemaTypeDef,
+        "InputSchema": SourceSchemaOutputTypeDef,
         "InputParallelism": InputParallelismTypeDef,
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_RequiredReferenceDataSourceDescriptionTypeDef",
+    {
+        "ReferenceId": str,
+        "TableName": str,
+        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
+    },
+)
+_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_OptionalReferenceDataSourceDescriptionTypeDef",
+    {
+        "ReferenceSchema": SourceSchemaOutputTypeDef,
+    },
+    total=False,
+)
+
+class ReferenceDataSourceDescriptionTypeDef(
+    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
+):
+    pass
+
 _RequiredInputTypeDef = TypedDict(
     "_RequiredInputTypeDef",
     {
         "NamePrefix": str,
         "InputSchema": SourceSchemaTypeDef,
     },
 )
@@ -2081,35 +2136,14 @@
     },
     total=False,
 )
 
 class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
     pass
 
-_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_RequiredReferenceDataSourceDescriptionTypeDef",
-    {
-        "ReferenceId": str,
-        "TableName": str,
-        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
-    },
-)
-_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_OptionalReferenceDataSourceDescriptionTypeDef",
-    {
-        "ReferenceSchema": SourceSchemaTypeDef,
-    },
-    total=False,
-)
-
-class ReferenceDataSourceDescriptionTypeDef(
-    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
-):
-    pass
-
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
         "ReferenceSchema": SourceSchemaTypeDef,
     },
 )
@@ -2149,47 +2183,47 @@
 
 AddApplicationInputResponseTypeDef = TypedDict(
     "AddApplicationInputResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "InputDescriptions": List[InputDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AddApplicationInputRequestRequestTypeDef = TypedDict(
-    "AddApplicationInputRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "CurrentApplicationVersionId": int,
-        "Input": InputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddApplicationReferenceDataSourceResponseTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SqlApplicationConfigurationDescriptionTypeDef = TypedDict(
     "SqlApplicationConfigurationDescriptionTypeDef",
     {
         "InputDescriptions": List[InputDescriptionTypeDef],
         "OutputDescriptions": List[OutputDescriptionTypeDef],
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
     },
     total=False,
 )
 
+AddApplicationInputRequestRequestTypeDef = TypedDict(
+    "AddApplicationInputRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "CurrentApplicationVersionId": int,
+        "Input": InputTypeDef,
+    },
+)
+
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
@@ -2347,42 +2381,42 @@
 ):
     pass
 
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationVersionResponseTypeDef = TypedDict(
     "DescribeApplicationVersionResponseTypeDef",
     {
         "ApplicationVersionDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RollbackApplicationResponseTypeDef = TypedDict(
     "RollbackApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationResponseTypeDef = TypedDict(
     "UpdateApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalyticsv2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore kinesisanalyticsv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore kinesisanalyticsv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesisanalyticsv2"></a>
 
 # types-aiobotocore-kinesisanalyticsv2
 
 [![PyPI - types-aiobotocore-kinesisanalyticsv2](https://img.shields.io/pypi/v/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesisanalyticsv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesisanalyticsv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalyticsv2)](https://pepy.tech/project/types-aiobotocore-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisAnalyticsV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [types-aiobotocore-kinesisanalyticsv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/).
 
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
@@ -327,74 +326,71 @@
 )
 
 
 def check_value(value: ApplicationModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesisanalyticsv2.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_kinesisanalyticsv2.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     VpcConfigurationTypeDef,
     VpcConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationDescriptionTypeDef,
     ApplicationSnapshotConfigurationTypeDef,
     ApplicationSnapshotConfigurationUpdateTypeDef,
     VpcConfigurationUpdateTypeDef,
     ApplicationMaintenanceConfigurationDescriptionTypeDef,
     ApplicationMaintenanceConfigurationUpdateTypeDef,
     ApplicationRestoreConfigurationTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
+    BlobTypeDef,
     CSVMappingParametersTypeDef,
     GlueDataCatalogConfigurationDescriptionTypeDef,
     GlueDataCatalogConfigurationTypeDef,
     GlueDataCatalogConfigurationUpdateTypeDef,
     CheckpointConfigurationDescriptionTypeDef,
     CheckpointConfigurationTypeDef,
     CheckpointConfigurationUpdateTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
     S3ApplicationCodeLocationDescriptionTypeDef,
     S3ContentLocationTypeDef,
     S3ContentLocationUpdateTypeDef,
     CreateApplicationPresignedUrlRequestRequestTypeDef,
-    CreateApplicationPresignedUrlResponseTypeDef,
     TagTypeDef,
     CreateApplicationSnapshotRequestRequestTypeDef,
     MavenReferenceTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
-    DeleteApplicationInputProcessingConfigurationResponseTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
-    DeleteApplicationOutputResponseTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationReferenceDataSourceResponseTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    DeleteApplicationSnapshotRequestRequestTypeDef,
+    TimestampTypeDef,
     DeleteApplicationVpcConfigurationRequestRequestTypeDef,
-    DeleteApplicationVpcConfigurationResponseTypeDef,
     S3ContentBaseLocationDescriptionTypeDef,
     S3ContentBaseLocationTypeDef,
     S3ContentBaseLocationUpdateTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeApplicationSnapshotRequestRequestTypeDef,
     SnapshotDetailsTypeDef,
     DescribeApplicationVersionRequestRequestTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     PropertyGroupTypeDef,
+    PropertyGroupOutputTypeDef,
     MonitoringConfigurationDescriptionTypeDef,
     ParallelismConfigurationDescriptionTypeDef,
     MonitoringConfigurationTypeDef,
     ParallelismConfigurationTypeDef,
     MonitoringConfigurationUpdateTypeDef,
     ParallelismConfigurationUpdateTypeDef,
     FlinkRunConfigurationTypeDef,
@@ -416,34 +412,36 @@
     KinesisFirehoseOutputUpdateTypeDef,
     KinesisStreamsOutputDescriptionTypeDef,
     KinesisStreamsOutputTypeDef,
     KinesisStreamsOutputUpdateTypeDef,
     LambdaOutputDescriptionTypeDef,
     LambdaOutputTypeDef,
     LambdaOutputUpdateTypeDef,
-    ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationSnapshotsRequestRequestTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
-    ResponseMetadataTypeDef,
     RollbackApplicationRequestRequestTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ZeppelinMonitoringConfigurationDescriptionTypeDef,
     ZeppelinMonitoringConfigurationTypeDef,
     ZeppelinMonitoringConfigurationUpdateTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionResponseTypeDef,
+    CreateApplicationPresignedUrlResponseTypeDef,
     DeleteApplicationCloudWatchLoggingOptionResponseTypeDef,
+    DeleteApplicationInputProcessingConfigurationResponseTypeDef,
+    DeleteApplicationOutputResponseTypeDef,
+    DeleteApplicationReferenceDataSourceResponseTypeDef,
+    DeleteApplicationVpcConfigurationResponseTypeDef,
     AddApplicationVpcConfigurationRequestRequestTypeDef,
     AddApplicationVpcConfigurationResponseTypeDef,
     UpdateApplicationMaintenanceConfigurationResponseTypeDef,
     UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     CatalogConfigurationDescriptionTypeDef,
@@ -452,35 +450,39 @@
     CodeContentDescriptionTypeDef,
     CodeContentTypeDef,
     CodeContentUpdateTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CustomArtifactConfigurationDescriptionTypeDef,
     CustomArtifactConfigurationTypeDef,
+    DeleteApplicationRequestRequestTypeDef,
+    DeleteApplicationSnapshotRequestRequestTypeDef,
     DeployAsApplicationConfigurationDescriptionTypeDef,
     DeployAsApplicationConfigurationTypeDef,
     DeployAsApplicationConfigurationUpdateTypeDef,
     DescribeApplicationSnapshotResponseTypeDef,
     ListApplicationSnapshotsResponseTypeDef,
     SqlRunConfigurationTypeDef,
     EnvironmentPropertiesTypeDef,
-    EnvironmentPropertyDescriptionsTypeDef,
     EnvironmentPropertyUpdatesTypeDef,
+    EnvironmentPropertyDescriptionsTypeDef,
     FlinkApplicationConfigurationDescriptionTypeDef,
     FlinkApplicationConfigurationTypeDef,
     FlinkApplicationConfigurationUpdateTypeDef,
     RunConfigurationDescriptionTypeDef,
     RunConfigurationUpdateTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
+    ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ApplicationCodeConfigurationDescriptionTypeDef,
     ApplicationCodeConfigurationTypeDef,
     ApplicationCodeConfigurationUpdateTypeDef,
     ZeppelinApplicationConfigurationDescriptionTypeDef,
     ZeppelinApplicationConfigurationTypeDef,
     ZeppelinApplicationConfigurationUpdateTypeDef,
     RunConfigurationTypeDef,
@@ -488,26 +490,27 @@
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputResponseTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
     StartApplicationRequestRequestTypeDef,
     InputSchemaUpdateTypeDef,
+    SourceSchemaOutputTypeDef,
     SourceSchemaTypeDef,
     InputUpdateTypeDef,
     DiscoverInputSchemaResponseTypeDef,
     InputDescriptionTypeDef,
-    InputTypeDef,
     ReferenceDataSourceDescriptionTypeDef,
+    InputTypeDef,
     ReferenceDataSourceTypeDef,
     ReferenceDataSourceUpdateTypeDef,
     AddApplicationInputResponseTypeDef,
-    AddApplicationInputRequestRequestTypeDef,
     AddApplicationReferenceDataSourceResponseTypeDef,
     SqlApplicationConfigurationDescriptionTypeDef,
+    AddApplicationInputRequestRequestTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     SqlApplicationConfigurationTypeDef,
     SqlApplicationConfigurationUpdateTypeDef,
     ApplicationConfigurationDescriptionTypeDef,
     ApplicationConfigurationTypeDef,
     ApplicationConfigurationUpdateTypeDef,
     ApplicationDetailTypeDef,
@@ -517,15 +520,15 @@
     DescribeApplicationResponseTypeDef,
     DescribeApplicationVersionResponseTypeDef,
     RollbackApplicationResponseTypeDef,
     UpdateApplicationResponseTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLoggingOptionTypeDef:
+def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


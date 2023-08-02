# Comparing `tmp/types-aiobotocore-drs-2.5.2.tar.gz` & `tmp/types-aiobotocore-drs-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-drs-2.5.2.tar", last modified: Sat Jul  8 01:43:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-drs-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
```

## Comparing `types-aiobotocore-drs-2.5.2.tar` & `types-aiobotocore-drs-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.882042 types-aiobotocore-drs-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-07-08 01:43:32.882042 types-aiobotocore-drs-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20669 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:32.882042 types-aiobotocore-drs-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.882042 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42020 2023-07-08 01:29:01.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41954 2023-07-08 01:29:01.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-07-08 01:29:01.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-07-08 01:29:01.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-07-08 01:29:01.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-07-08 01:29:01.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56978 2023-07-08 01:29:02.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56931 2023-07-08 01:29:02.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:29:00.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.882042 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-07-08 01:43:32.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:43:32.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:32.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:32.000000 types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.029601 types-aiobotocore-drs-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-08-02 14:52:12.029601 types-aiobotocore-drs-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20636 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.029601 types-aiobotocore-drs-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.025601 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41944 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41878 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17043 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17041 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13536 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56844 2023-08-02 14:36:42.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56797 2023-08-02 14:36:42.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:41.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.025601 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22138 2023-08-02 14:52:11.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:11.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:11.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:11.000000 types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-drs-2.5.2/LICENSE` & `types-aiobotocore-drs-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2/PKG-INFO` & `types-aiobotocore-drs-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-drs
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.drs 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.drs 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore drs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore drs type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-drs"></a>
 
 # types-aiobotocore-drs
 
 [![PyPI - types-aiobotocore-drs](https://img.shields.io/pypi/v/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-drs?color=blue)](https://pypistats.org/packages/types-aiobotocore-drs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-drs)](https://pepy.tech/project/types-aiobotocore-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.drs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [types-aiobotocore-drs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/).
 
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
@@ -381,114 +380,114 @@
 )
 
 
 def check_value(value: DataReplicationErrorStringType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_drs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_drs.type_defs import (
     AccountTypeDef,
     AssociateSourceNetworkStackRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CPUTypeDef,
     ConversionPropertiesTypeDef,
     CreateExtendedSourceServerRequestRequestTypeDef,
     LicensingTypeDef,
     PITPolicyRuleTypeDef,
     CreateSourceNetworkRequestRequestTypeDef,
-    CreateSourceNetworkResponseTypeDef,
     DataReplicationErrorTypeDef,
     DataReplicationInfoReplicatedDiskTypeDef,
     DataReplicationInitiationStepTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteRecoveryInstanceRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
     DeleteSourceNetworkRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
-    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
     DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     RecoverySnapshotTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
     DescribeSourceNetworksRequestFiltersTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DisconnectRecoveryInstanceRequestRequestTypeDef,
     DisconnectSourceServerRequestRequestTypeDef,
     DiskTypeDef,
-    EmptyResponseMetadataTypeDef,
     SourceNetworkDataTypeDef,
     ExportSourceNetworkCfnTemplateRequestRequestTypeDef,
-    ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationRequestRequestTypeDef,
-    GetFailbackReplicationConfigurationResponseTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ParticipatingServerTypeDef,
     LifeCycleLastLaunchInitiatedTypeDef,
-    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
     ListExtensibleSourceServersRequestRequestTypeDef,
     StagingSourceServerTypeDef,
-    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     ListStagingAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
-    PaginatorConfigTypeDef,
     ParticipatingResourceIDTypeDef,
     RecoveryInstanceDataReplicationErrorTypeDef,
     RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef,
     RecoveryInstanceDataReplicationInitiationStepTypeDef,
     RecoveryInstanceDiskTypeDef,
     RecoveryInstanceFailbackTypeDef,
     RecoveryLifeCycleTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     ReverseReplicationRequestRequestTypeDef,
-    ReverseReplicationResponseTypeDef,
     SourceCloudPropertiesTypeDef,
     StagingAreaTypeDef,
     StartFailbackLaunchRequestRequestTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
     StartSourceNetworkReplicationRequestRequestTypeDef,
     StopFailbackRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
     StopSourceNetworkReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateRecoveryInstancesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFailbackReplicationConfigurationRequestRequestTypeDef,
+    CreateSourceNetworkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportSourceNetworkCfnTemplateResponseTypeDef,
+    GetFailbackReplicationConfigurationResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ReverseReplicationResponseTypeDef,
     CreateLaunchConfigurationTemplateRequestRequestTypeDef,
     LaunchConfigurationTemplateTypeDef,
     LaunchConfigurationTypeDef,
     UpdateLaunchConfigurationRequestRequestTypeDef,
     UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     CreateReplicationConfigurationTemplateRequestRequestTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTemplateTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
+    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef,
     DescribeRecoveryInstancesRequestRequestTypeDef,
     DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     DescribeRecoverySnapshotsRequestRequestTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
@@ -517,15 +516,15 @@
     LifeCycleTypeDef,
     JobTypeDef,
     RecoveryInstanceDataReplicationInfoTypeDef,
     DescribeSourceNetworksResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
     StopSourceNetworkReplicationResponseTypeDef,
     JobLogTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     SourceServerTypeDef,
     AssociateSourceNetworkStackResponseTypeDef,
     DescribeJobsResponseTypeDef,
     StartFailbackLaunchResponseTypeDef,
     StartRecoveryResponseTypeDef,
     StartSourceNetworkRecoveryResponseTypeDef,
     TerminateRecoveryInstancesResponseTypeDef,
@@ -535,15 +534,15 @@
     DescribeSourceServersResponseTypeDef,
     StartReplicationResponseTypeDef,
     StopReplicationResponseTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountTypeDef:
+def get_value() -> AccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-drs-2.5.2/README.md` & `types-aiobotocore-drs-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-drs"></a>
 
 # types-aiobotocore-drs
 
 [![PyPI - types-aiobotocore-drs](https://img.shields.io/pypi/v/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-drs?color=blue)](https://pypistats.org/packages/types-aiobotocore-drs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-drs)](https://pepy.tech/project/types-aiobotocore-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.drs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [types-aiobotocore-drs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/).
 
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
@@ -348,114 +348,114 @@
 )
 
 
 def check_value(value: DataReplicationErrorStringType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_drs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_drs.type_defs import (
     AccountTypeDef,
     AssociateSourceNetworkStackRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CPUTypeDef,
     ConversionPropertiesTypeDef,
     CreateExtendedSourceServerRequestRequestTypeDef,
     LicensingTypeDef,
     PITPolicyRuleTypeDef,
     CreateSourceNetworkRequestRequestTypeDef,
-    CreateSourceNetworkResponseTypeDef,
     DataReplicationErrorTypeDef,
     DataReplicationInfoReplicatedDiskTypeDef,
     DataReplicationInitiationStepTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteRecoveryInstanceRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
     DeleteSourceNetworkRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
-    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
     DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     RecoverySnapshotTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
     DescribeSourceNetworksRequestFiltersTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DisconnectRecoveryInstanceRequestRequestTypeDef,
     DisconnectSourceServerRequestRequestTypeDef,
     DiskTypeDef,
-    EmptyResponseMetadataTypeDef,
     SourceNetworkDataTypeDef,
     ExportSourceNetworkCfnTemplateRequestRequestTypeDef,
-    ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationRequestRequestTypeDef,
-    GetFailbackReplicationConfigurationResponseTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ParticipatingServerTypeDef,
     LifeCycleLastLaunchInitiatedTypeDef,
-    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
     ListExtensibleSourceServersRequestRequestTypeDef,
     StagingSourceServerTypeDef,
-    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     ListStagingAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
-    PaginatorConfigTypeDef,
     ParticipatingResourceIDTypeDef,
     RecoveryInstanceDataReplicationErrorTypeDef,
     RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef,
     RecoveryInstanceDataReplicationInitiationStepTypeDef,
     RecoveryInstanceDiskTypeDef,
     RecoveryInstanceFailbackTypeDef,
     RecoveryLifeCycleTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     ReverseReplicationRequestRequestTypeDef,
-    ReverseReplicationResponseTypeDef,
     SourceCloudPropertiesTypeDef,
     StagingAreaTypeDef,
     StartFailbackLaunchRequestRequestTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
     StartSourceNetworkReplicationRequestRequestTypeDef,
     StopFailbackRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
     StopSourceNetworkReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateRecoveryInstancesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFailbackReplicationConfigurationRequestRequestTypeDef,
+    CreateSourceNetworkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportSourceNetworkCfnTemplateResponseTypeDef,
+    GetFailbackReplicationConfigurationResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ReverseReplicationResponseTypeDef,
     CreateLaunchConfigurationTemplateRequestRequestTypeDef,
     LaunchConfigurationTemplateTypeDef,
     LaunchConfigurationTypeDef,
     UpdateLaunchConfigurationRequestRequestTypeDef,
     UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     CreateReplicationConfigurationTemplateRequestRequestTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTemplateTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
+    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef,
     DescribeRecoveryInstancesRequestRequestTypeDef,
     DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     DescribeRecoverySnapshotsRequestRequestTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
@@ -484,15 +484,15 @@
     LifeCycleTypeDef,
     JobTypeDef,
     RecoveryInstanceDataReplicationInfoTypeDef,
     DescribeSourceNetworksResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
     StopSourceNetworkReplicationResponseTypeDef,
     JobLogTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     SourceServerTypeDef,
     AssociateSourceNetworkStackResponseTypeDef,
     DescribeJobsResponseTypeDef,
     StartFailbackLaunchResponseTypeDef,
     StartRecoveryResponseTypeDef,
     StartSourceNetworkRecoveryResponseTypeDef,
     TerminateRecoveryInstancesResponseTypeDef,
@@ -502,15 +502,15 @@
     DescribeSourceServersResponseTypeDef,
     StartReplicationResponseTypeDef,
     StopReplicationResponseTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountTypeDef:
+def get_value() -> AccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-drs-2.5.2/setup.py` & `types-aiobotocore-drs-2.5.2.post1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-drs",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_drs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.drs 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore drs type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore drs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_drs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/__init__.py` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/__init__.pyi` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/__main__.py` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.drs 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.drs 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs\nOther"
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

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/client.py` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,18 +64,18 @@
     LaunchConfigurationTypeDef,
     LicensingTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PITPolicyRuleTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTypeDef,
     ReverseReplicationResponseTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     StartFailbackLaunchResponseTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartRecoveryResponseTypeDef,
     StartReplicationResponseTypeDef,
     StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
     StartSourceNetworkRecoveryResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
@@ -201,15 +201,15 @@
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         autoReplicateNewDisks: bool = ...,
         ebsEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...
-    ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#create_replication_configuration_template)
         """
 
@@ -396,17 +396,15 @@
         """
         Disconnect a Recovery Instance from Elastic Disaster Recovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.disconnect_recovery_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#disconnect_recovery_instance)
         """
 
-    async def disconnect_source_server(
-        self, *, sourceServerID: str
-    ) -> SourceServerResponseMetadataTypeDef:
+    async def disconnect_source_server(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
         """
         Disconnects a specific Source Server from Elastic Disaster Recovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.disconnect_source_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#disconnect_source_server)
         """
 
@@ -497,17 +495,15 @@
         """
         List all tags for your Elastic Disaster Recovery resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#list_tags_for_resource)
         """
 
-    async def retry_data_replication(
-        self, *, sourceServerID: str
-    ) -> SourceServerResponseMetadataTypeDef:
+    async def retry_data_replication(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
         """
         WARNING: RetryDataReplication is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.retry_data_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#retry_data_replication)
         """
 
@@ -735,15 +731,15 @@
         ebsEncryptionKeyArn: str = ...,
         pitPolicy: Sequence[PITPolicyRuleTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...
-    ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates a ReplicationConfigurationTemplate by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#update_replication_configuration_template)
         """
```

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/client.pyi` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -64,18 +64,18 @@
     LaunchConfigurationTypeDef,
     LicensingTypeDef,
     ListExtensibleSourceServersResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PITPolicyRuleTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTypeDef,
     ReverseReplicationResponseTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     StartFailbackLaunchResponseTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartRecoveryResponseTypeDef,
     StartReplicationResponseTypeDef,
     StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
     StartSourceNetworkRecoveryResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
@@ -191,15 +191,15 @@
         replicationServersSecurityGroupsIDs: Sequence[str],
         stagingAreaSubnetId: str,
         stagingAreaTags: Mapping[str, str],
         useDedicatedReplicationServer: bool,
         autoReplicateNewDisks: bool = ...,
         ebsEncryptionKeyArn: str = ...,
         tags: Mapping[str, str] = ...
-    ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Creates a new ReplicationConfigurationTemplate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.create_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#create_replication_configuration_template)
         """
     async def create_source_network(
@@ -369,17 +369,15 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disconnect a Recovery Instance from Elastic Disaster Recovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.disconnect_recovery_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#disconnect_recovery_instance)
         """
-    async def disconnect_source_server(
-        self, *, sourceServerID: str
-    ) -> SourceServerResponseMetadataTypeDef:
+    async def disconnect_source_server(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
         """
         Disconnects a specific Source Server from Elastic Disaster Recovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.disconnect_source_server)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#disconnect_source_server)
         """
     async def export_source_network_cfn_template(
@@ -460,17 +458,15 @@
     ) -> ListTagsForResourceResponseTypeDef:
         """
         List all tags for your Elastic Disaster Recovery resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#list_tags_for_resource)
         """
-    async def retry_data_replication(
-        self, *, sourceServerID: str
-    ) -> SourceServerResponseMetadataTypeDef:
+    async def retry_data_replication(self, *, sourceServerID: str) -> SourceServerResponseTypeDef:
         """
         WARNING: RetryDataReplication is deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.retry_data_replication)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#retry_data_replication)
         """
     async def reverse_replication(
@@ -681,15 +677,15 @@
         ebsEncryptionKeyArn: str = ...,
         pitPolicy: Sequence[PITPolicyRuleTypeDef] = ...,
         replicationServerInstanceType: str = ...,
         replicationServersSecurityGroupsIDs: Sequence[str] = ...,
         stagingAreaSubnetId: str = ...,
         stagingAreaTags: Mapping[str, str] = ...,
         useDedicatedReplicationServer: bool = ...
-    ) -> ReplicationConfigurationTemplateResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationTemplateResponseTypeDef:
         """
         Updates a ReplicationConfigurationTemplate by ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Client.update_replication_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/client/#update_replication_configuration_template)
         """
     @overload
```

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/literals.py` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/literals.pyi` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/paginator.py` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 class DescribeJobLogItemsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobID: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describejoblogitemspaginator)
         """
 
 
@@ -108,15 +108,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describejobspaginator)
         """
 
 
@@ -126,15 +126,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
 
@@ -144,15 +144,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describerecoveryinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRecoveryInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describerecoveryinstancespaginator)
         """
 
 
@@ -164,15 +164,15 @@
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,
         order: RecoverySnapshotsOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRecoverySnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoverySnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describerecoverysnapshotspaginator)
         """
 
 
@@ -182,15 +182,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 
@@ -200,15 +200,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourcenetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSourceNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourcenetworkspaginator)
         """
 
 
@@ -218,43 +218,43 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourceserverspaginator)
         """
 
 
 class ListExtensibleSourceServersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#listextensiblesourceserverspaginator)
     """
 
     def paginate(
-        self, *, stagingAccountID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, stagingAccountID: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExtensibleSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#listextensiblesourceserverspaginator)
         """
 
 
 class ListStagingAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#liststagingaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStagingAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#liststagingaccountspaginator)
         """
```

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/paginator.pyi` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 class DescribeJobLogItemsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describejoblogitemspaginator)
     """
 
     def paginate(
-        self, *, jobID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobID: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeJobLogItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describejoblogitemspaginator)
         """
 
 class DescribeJobsPaginator(AioPaginator):
@@ -104,15 +104,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describejobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeJobsRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describejobspaginator)
         """
 
 class DescribeLaunchConfigurationTemplatesPaginator(AioPaginator):
@@ -121,15 +121,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describelaunchconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         launchConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeLaunchConfigurationTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describelaunchconfigurationtemplatespaginator)
         """
 
 class DescribeRecoveryInstancesPaginator(AioPaginator):
@@ -138,15 +138,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describerecoveryinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRecoveryInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describerecoveryinstancespaginator)
         """
 
 class DescribeRecoverySnapshotsPaginator(AioPaginator):
@@ -157,15 +157,15 @@
 
     def paginate(
         self,
         *,
         sourceServerID: str,
         filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,
         order: RecoverySnapshotsOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRecoverySnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoverySnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describerecoverysnapshotspaginator)
         """
 
 class DescribeReplicationConfigurationTemplatesPaginator(AioPaginator):
@@ -174,15 +174,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describereplicationconfigurationtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         replicationConfigurationTemplateIDs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeReplicationConfigurationTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describereplicationconfigurationtemplatespaginator)
         """
 
 class DescribeSourceNetworksPaginator(AioPaginator):
@@ -191,15 +191,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourcenetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSourceNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourcenetworkspaginator)
         """
 
 class DescribeSourceServersPaginator(AioPaginator):
@@ -208,41 +208,41 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourceserverspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: DescribeSourceServersRequestFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#describesourceserverspaginator)
         """
 
 class ListExtensibleSourceServersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#listextensiblesourceserverspaginator)
     """
 
     def paginate(
-        self, *, stagingAccountID: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, stagingAccountID: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExtensibleSourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#listextensiblesourceserverspaginator)
         """
 
 class ListStagingAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#liststagingaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStagingAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/paginators/#liststagingaccountspaginator)
         """
```

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/type_defs.py` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_drs.type_defs import AccountTypeDef
 
-    data: AccountTypeDef = {...}
+    data: AccountTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -54,103 +54,103 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountTypeDef",
     "AssociateSourceNetworkStackRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CPUTypeDef",
     "ConversionPropertiesTypeDef",
     "CreateExtendedSourceServerRequestRequestTypeDef",
     "LicensingTypeDef",
     "PITPolicyRuleTypeDef",
     "CreateSourceNetworkRequestRequestTypeDef",
-    "CreateSourceNetworkResponseTypeDef",
     "DataReplicationErrorTypeDef",
     "DataReplicationInfoReplicatedDiskTypeDef",
     "DataReplicationInitiationStepTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     "DeleteRecoveryInstanceRequestRequestTypeDef",
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     "DeleteSourceNetworkRequestRequestTypeDef",
     "DeleteSourceServerRequestRequestTypeDef",
-    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeJobLogItemsRequestRequestTypeDef",
     "DescribeJobsRequestFiltersTypeDef",
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestFiltersTypeDef",
     "DescribeRecoverySnapshotsRequestFiltersTypeDef",
     "RecoverySnapshotTypeDef",
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     "DescribeSourceNetworksRequestFiltersTypeDef",
     "DescribeSourceServersRequestFiltersTypeDef",
     "DisconnectRecoveryInstanceRequestRequestTypeDef",
     "DisconnectSourceServerRequestRequestTypeDef",
     "DiskTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "SourceNetworkDataTypeDef",
     "ExportSourceNetworkCfnTemplateRequestRequestTypeDef",
-    "ExportSourceNetworkCfnTemplateResponseTypeDef",
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
-    "GetFailbackReplicationConfigurationResponseTypeDef",
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ParticipatingServerTypeDef",
     "LifeCycleLastLaunchInitiatedTypeDef",
-    "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
     "ListExtensibleSourceServersRequestRequestTypeDef",
     "StagingSourceServerTypeDef",
-    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "ListStagingAccountsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
-    "PaginatorConfigTypeDef",
     "ParticipatingResourceIDTypeDef",
     "RecoveryInstanceDataReplicationErrorTypeDef",
     "RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef",
     "RecoveryInstanceDataReplicationInitiationStepTypeDef",
     "RecoveryInstanceDiskTypeDef",
     "RecoveryInstanceFailbackTypeDef",
     "RecoveryLifeCycleTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "ReverseReplicationRequestRequestTypeDef",
-    "ReverseReplicationResponseTypeDef",
     "SourceCloudPropertiesTypeDef",
     "StagingAreaTypeDef",
     "StartFailbackLaunchRequestRequestTypeDef",
     "StartRecoveryRequestSourceServerTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartSourceNetworkRecoveryRequestNetworkEntryTypeDef",
     "StartSourceNetworkReplicationRequestRequestTypeDef",
     "StopFailbackRequestRequestTypeDef",
     "StopReplicationRequestRequestTypeDef",
     "StopSourceNetworkReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateRecoveryInstancesRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFailbackReplicationConfigurationRequestRequestTypeDef",
+    "CreateSourceNetworkResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportSourceNetworkCfnTemplateResponseTypeDef",
+    "GetFailbackReplicationConfigurationResponseTypeDef",
     "ListStagingAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ReverseReplicationResponseTypeDef",
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
     "LaunchConfigurationTemplateTypeDef",
     "LaunchConfigurationTypeDef",
     "UpdateLaunchConfigurationRequestRequestTypeDef",
     "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "CreateReplicationConfigurationTemplateRequestRequestTypeDef",
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+    "ReplicationConfigurationTemplateResponseTypeDef",
     "ReplicationConfigurationTemplateTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     "DataReplicationInitiationTypeDef",
+    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     "DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     "DescribeRecoverySnapshotsRequestRequestTypeDef",
     "DescribeRecoverySnapshotsResponseTypeDef",
@@ -179,15 +179,15 @@
     "LifeCycleTypeDef",
     "JobTypeDef",
     "RecoveryInstanceDataReplicationInfoTypeDef",
     "DescribeSourceNetworksResponseTypeDef",
     "StartSourceNetworkReplicationResponseTypeDef",
     "StopSourceNetworkReplicationResponseTypeDef",
     "JobLogTypeDef",
-    "SourceServerResponseMetadataTypeDef",
+    "SourceServerResponseTypeDef",
     "SourceServerTypeDef",
     "AssociateSourceNetworkStackResponseTypeDef",
     "DescribeJobsResponseTypeDef",
     "StartFailbackLaunchResponseTypeDef",
     "StartRecoveryResponseTypeDef",
     "StartSourceNetworkRecoveryResponseTypeDef",
     "TerminateRecoveryInstancesResponseTypeDef",
@@ -212,14 +212,25 @@
     "AssociateSourceNetworkStackRequestRequestTypeDef",
     {
         "cfnStackName": str,
         "sourceNetworkID": str,
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
 CPUTypeDef = TypedDict(
     "CPUTypeDef",
     {
         "cores": int,
         "modelName": str,
     },
     total=False,
@@ -309,22 +320,14 @@
 class CreateSourceNetworkRequestRequestTypeDef(
     _RequiredCreateSourceNetworkRequestRequestTypeDef,
     _OptionalCreateSourceNetworkRequestRequestTypeDef,
 ):
     pass
 
 
-CreateSourceNetworkResponseTypeDef = TypedDict(
-    "CreateSourceNetworkResponseTypeDef",
-    {
-        "sourceNetworkID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataReplicationErrorTypeDef = TypedDict(
     "DataReplicationErrorTypeDef",
     {
         "error": DataReplicationErrorStringType,
         "rawError": str,
     },
     total=False,
@@ -389,36 +392,24 @@
 DeleteSourceServerRequestRequestTypeDef = TypedDict(
     "DeleteSourceServerRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
-_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    {
-        "jobID": str,
-    },
-)
-_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
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
-class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
-    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeJobLogItemsRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
@@ -444,23 +435,14 @@
         "fromDate": str,
         "jobIDs": Sequence[str],
         "toDate": str,
     },
     total=False,
 )
 
-DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
-    {
-        "launchConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeLaunchConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
     {
         "launchConfigurationTemplateIDs": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -503,23 +485,14 @@
 )
 
 
 class RecoverySnapshotTypeDef(_RequiredRecoverySnapshotTypeDef, _OptionalRecoverySnapshotTypeDef):
     pass
 
 
-DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
-    {
-        "replicationConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReplicationConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "replicationConfigurationTemplateIDs": Sequence[str],
     },
@@ -565,21 +538,14 @@
     {
         "bytes": int,
         "deviceName": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SourceNetworkDataTypeDef = TypedDict(
     "SourceNetworkDataTypeDef",
     {
         "sourceNetworkID": str,
         "sourceVpc": str,
         "stackName": str,
         "targetVpc": str,
@@ -590,40 +556,21 @@
 ExportSourceNetworkCfnTemplateRequestRequestTypeDef = TypedDict(
     "ExportSourceNetworkCfnTemplateRequestRequestTypeDef",
     {
         "sourceNetworkID": str,
     },
 )
 
-ExportSourceNetworkCfnTemplateResponseTypeDef = TypedDict(
-    "ExportSourceNetworkCfnTemplateResponseTypeDef",
-    {
-        "s3DestinationUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFailbackReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
-GetFailbackReplicationConfigurationResponseTypeDef = TypedDict(
-    "GetFailbackReplicationConfigurationResponseTypeDef",
-    {
-        "bandwidthThrottling": int,
-        "name": str,
-        "recoveryInstanceID": str,
-        "usePrivateIP": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "GetLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
@@ -661,36 +608,14 @@
         "apiCallDateTime": str,
         "jobID": str,
         "type": LastLaunchTypeType,
     },
     total=False,
 )
 
-_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
-    "_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    {
-        "stagingAccountID": str,
-    },
-)
-_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
-    "_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(
-    _RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-    _OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListExtensibleSourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListExtensibleSourceServersRequestRequestTypeDef",
     {
         "stagingAccountID": str,
     },
 )
 _OptionalListExtensibleSourceServersRequestRequestTypeDef = TypedDict(
@@ -716,22 +641,14 @@
         "arn": str,
         "hostname": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = TypedDict(
-    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStagingAccountsRequestRequestTypeDef = TypedDict(
     "ListStagingAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -740,22 +657,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "ips": List[str],
         "isPrimary": bool,
         "macAddress": str,
     },
@@ -766,24 +675,14 @@
     "OSTypeDef",
     {
         "fullString": str,
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
 ParticipatingResourceIDTypeDef = TypedDict(
     "ParticipatingResourceIDTypeDef",
     {
         "sourceNetworkID": str,
     },
     total=False,
 )
@@ -864,47 +763,28 @@
         "optimizedStagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "throughput": int,
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
 RetryDataReplicationRequestRequestTypeDef = TypedDict(
     "RetryDataReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
 ReverseReplicationRequestRequestTypeDef = TypedDict(
     "ReverseReplicationRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
-ReverseReplicationResponseTypeDef = TypedDict(
-    "ReverseReplicationResponseTypeDef",
-    {
-        "reversedDirectionSourceServerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SourceCloudPropertiesTypeDef = TypedDict(
     "SourceCloudPropertiesTypeDef",
     {
         "originAccountID": str,
         "originAvailabilityZone": str,
         "originRegion": str,
     },
@@ -1066,20 +946,70 @@
 class UpdateFailbackReplicationConfigurationRequestRequestTypeDef(
     _RequiredUpdateFailbackReplicationConfigurationRequestRequestTypeDef,
     _OptionalUpdateFailbackReplicationConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+CreateSourceNetworkResponseTypeDef = TypedDict(
+    "CreateSourceNetworkResponseTypeDef",
+    {
+        "sourceNetworkID": str,
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
+ExportSourceNetworkCfnTemplateResponseTypeDef = TypedDict(
+    "ExportSourceNetworkCfnTemplateResponseTypeDef",
+    {
+        "s3DestinationUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFailbackReplicationConfigurationResponseTypeDef = TypedDict(
+    "GetFailbackReplicationConfigurationResponseTypeDef",
+    {
+        "bandwidthThrottling": int,
+        "name": str,
+        "recoveryInstanceID": str,
+        "usePrivateIP": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListStagingAccountsResponseTypeDef = TypedDict(
     "ListStagingAccountsResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReverseReplicationResponseTypeDef = TypedDict(
+    "ReverseReplicationResponseTypeDef",
+    {
+        "reversedDirectionSourceServerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "copyPrivateIp": bool,
@@ -1116,15 +1046,15 @@
         "copyTags": bool,
         "ec2LaunchTemplateID": str,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "name": str,
         "sourceServerID": str,
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
@@ -1209,16 +1139,16 @@
 class CreateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef,
     _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+ReplicationConfigurationTemplateResponseTypeDef = TypedDict(
+    "ReplicationConfigurationTemplateResponseTypeDef",
     {
         "arn": str,
         "associateDefaultSecurityGroup": bool,
         "autoReplicateNewDisks": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
@@ -1229,15 +1159,15 @@
         "replicationConfigurationTemplateID": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "tags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredReplicationConfigurationTemplateTypeDef = TypedDict(
     "_RequiredReplicationConfigurationTemplateTypeDef",
     {
         "replicationConfigurationTemplateID": str,
@@ -1316,19 +1246,89 @@
         "nextAttemptDateTime": str,
         "startDateTime": str,
         "steps": List[DataReplicationInitiationStepTypeDef],
     },
     total=False,
 )
 
+_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    {
+        "jobID": str,
+    },
+)
+_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
+    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+):
+    pass
+
+
+DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    {
+        "launchConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    {
+        "replicationConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
+    "_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    {
+        "stagingAccountID": str,
+    },
+)
+_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
+    "_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(
+    _RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+    _OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+):
+    pass
+
+
+ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = TypedDict(
+    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
         "filters": DescribeJobsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
@@ -1339,15 +1339,15 @@
     total=False,
 )
 
 DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     {
         "filters": DescribeRecoveryInstancesRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeRecoveryInstancesRequestRequestTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     {
@@ -1365,15 +1365,15 @@
     },
 )
 _OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef = TypedDict(
     "_OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     {
         "filters": DescribeRecoverySnapshotsRequestFiltersTypeDef,
         "order": RecoverySnapshotsOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef(
     _RequiredDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
@@ -1408,23 +1408,23 @@
 
 
 DescribeRecoverySnapshotsResponseTypeDef = TypedDict(
     "DescribeRecoverySnapshotsResponseTypeDef",
     {
         "items": List[RecoverySnapshotTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef = TypedDict(
     "DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef",
     {
         "filters": DescribeSourceNetworksRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSourceNetworksRequestRequestTypeDef = TypedDict(
     "DescribeSourceNetworksRequestRequestTypeDef",
     {
@@ -1435,15 +1435,15 @@
     total=False,
 )
 
 DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
         "filters": DescribeSourceServersRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSourceServersRequestRequestTypeDef = TypedDict(
     "DescribeSourceServersRequestRequestTypeDef",
     {
@@ -1472,15 +1472,15 @@
 )
 
 ListExtensibleSourceServersResponseTypeDef = TypedDict(
     "ListExtensibleSourceServersResponseTypeDef",
     {
         "items": List[StagingSourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourcePropertiesTypeDef = TypedDict(
     "SourcePropertiesTypeDef",
     {
         "cpus": List[CPUTypeDef],
@@ -1562,15 +1562,15 @@
         "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
@@ -1652,41 +1652,41 @@
     pass
 
 
 CreateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
     "CreateLaunchConfigurationTemplateResponseTypeDef",
     {
         "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     {
         "items": List[LaunchConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
     "UpdateLaunchConfigurationTemplateResponseTypeDef",
     {
         "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     {
         "items": List[ReplicationConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataReplicationInfoTypeDef = TypedDict(
     "DataReplicationInfoTypeDef",
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
@@ -1767,61 +1767,61 @@
 )
 
 DescribeSourceNetworksResponseTypeDef = TypedDict(
     "DescribeSourceNetworksResponseTypeDef",
     {
         "items": List[SourceNetworkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSourceNetworkReplicationResponseTypeDef = TypedDict(
     "StartSourceNetworkReplicationResponseTypeDef",
     {
         "sourceNetwork": SourceNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopSourceNetworkReplicationResponseTypeDef = TypedDict(
     "StopSourceNetworkReplicationResponseTypeDef",
     {
         "sourceNetwork": SourceNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobLogTypeDef = TypedDict(
     "JobLogTypeDef",
     {
         "event": JobLogEventType,
         "eventData": JobLogEventDataTypeDef,
         "logDateTime": str,
     },
     total=False,
 )
 
-SourceServerResponseMetadataTypeDef = TypedDict(
-    "SourceServerResponseMetadataTypeDef",
+SourceServerResponseTypeDef = TypedDict(
+    "SourceServerResponseTypeDef",
     {
         "arn": str,
         "dataReplicationInfo": DataReplicationInfoTypeDef,
         "lastLaunchResult": LastLaunchResultType,
         "lifeCycle": LifeCycleTypeDef,
         "recoveryInstanceId": str,
         "replicationDirection": ReplicationDirectionType,
         "reversedDirectionSourceServerArn": str,
         "sourceCloudProperties": SourceCloudPropertiesTypeDef,
         "sourceNetworkID": str,
         "sourceProperties": SourcePropertiesTypeDef,
         "sourceServerID": str,
         "stagingArea": StagingAreaTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceServerTypeDef = TypedDict(
     "SourceServerTypeDef",
     {
         "arn": str,
@@ -1841,56 +1841,56 @@
     total=False,
 )
 
 AssociateSourceNetworkStackResponseTypeDef = TypedDict(
     "AssociateSourceNetworkStackResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "items": List[JobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFailbackLaunchResponseTypeDef = TypedDict(
     "StartFailbackLaunchResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartRecoveryResponseTypeDef = TypedDict(
     "StartRecoveryResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSourceNetworkRecoveryResponseTypeDef = TypedDict(
     "StartSourceNetworkRecoveryResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TerminateRecoveryInstancesResponseTypeDef = TypedDict(
     "TerminateRecoveryInstancesResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecoveryInstanceTypeDef = TypedDict(
     "RecoveryInstanceTypeDef",
     {
         "arn": str,
@@ -1912,52 +1912,52 @@
 )
 
 DescribeJobLogItemsResponseTypeDef = TypedDict(
     "DescribeJobLogItemsResponseTypeDef",
     {
         "items": List[JobLogTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExtendedSourceServerResponseTypeDef = TypedDict(
     "CreateExtendedSourceServerResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSourceServersResponseTypeDef = TypedDict(
     "DescribeSourceServersResponseTypeDef",
     {
         "items": List[SourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartReplicationResponseTypeDef = TypedDict(
     "StartReplicationResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopReplicationResponseTypeDef = TypedDict(
     "StopReplicationResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecoveryInstancesResponseTypeDef = TypedDict(
     "DescribeRecoveryInstancesResponseTypeDef",
     {
         "items": List[RecoveryInstanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs/type_defs.pyi` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_drs.type_defs import AccountTypeDef
 
-    data: AccountTypeDef = {...}
+    data: AccountTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -53,103 +53,103 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountTypeDef",
     "AssociateSourceNetworkStackRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CPUTypeDef",
     "ConversionPropertiesTypeDef",
     "CreateExtendedSourceServerRequestRequestTypeDef",
     "LicensingTypeDef",
     "PITPolicyRuleTypeDef",
     "CreateSourceNetworkRequestRequestTypeDef",
-    "CreateSourceNetworkResponseTypeDef",
     "DataReplicationErrorTypeDef",
     "DataReplicationInfoReplicatedDiskTypeDef",
     "DataReplicationInitiationStepTypeDef",
     "DeleteJobRequestRequestTypeDef",
     "DeleteLaunchConfigurationTemplateRequestRequestTypeDef",
     "DeleteRecoveryInstanceRequestRequestTypeDef",
     "DeleteReplicationConfigurationTemplateRequestRequestTypeDef",
     "DeleteSourceNetworkRequestRequestTypeDef",
     "DeleteSourceServerRequestRequestTypeDef",
-    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeJobLogItemsRequestRequestTypeDef",
     "DescribeJobsRequestFiltersTypeDef",
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestFiltersTypeDef",
     "DescribeRecoverySnapshotsRequestFiltersTypeDef",
     "RecoverySnapshotTypeDef",
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     "DescribeSourceNetworksRequestFiltersTypeDef",
     "DescribeSourceServersRequestFiltersTypeDef",
     "DisconnectRecoveryInstanceRequestRequestTypeDef",
     "DisconnectSourceServerRequestRequestTypeDef",
     "DiskTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "SourceNetworkDataTypeDef",
     "ExportSourceNetworkCfnTemplateRequestRequestTypeDef",
-    "ExportSourceNetworkCfnTemplateResponseTypeDef",
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
-    "GetFailbackReplicationConfigurationResponseTypeDef",
     "GetLaunchConfigurationRequestRequestTypeDef",
     "GetReplicationConfigurationRequestRequestTypeDef",
     "IdentificationHintsTypeDef",
     "ParticipatingServerTypeDef",
     "LifeCycleLastLaunchInitiatedTypeDef",
-    "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
     "ListExtensibleSourceServersRequestRequestTypeDef",
     "StagingSourceServerTypeDef",
-    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "ListStagingAccountsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NetworkInterfaceTypeDef",
     "OSTypeDef",
-    "PaginatorConfigTypeDef",
     "ParticipatingResourceIDTypeDef",
     "RecoveryInstanceDataReplicationErrorTypeDef",
     "RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef",
     "RecoveryInstanceDataReplicationInitiationStepTypeDef",
     "RecoveryInstanceDiskTypeDef",
     "RecoveryInstanceFailbackTypeDef",
     "RecoveryLifeCycleTypeDef",
     "ReplicationConfigurationReplicatedDiskTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryDataReplicationRequestRequestTypeDef",
     "ReverseReplicationRequestRequestTypeDef",
-    "ReverseReplicationResponseTypeDef",
     "SourceCloudPropertiesTypeDef",
     "StagingAreaTypeDef",
     "StartFailbackLaunchRequestRequestTypeDef",
     "StartRecoveryRequestSourceServerTypeDef",
     "StartReplicationRequestRequestTypeDef",
     "StartSourceNetworkRecoveryRequestNetworkEntryTypeDef",
     "StartSourceNetworkReplicationRequestRequestTypeDef",
     "StopFailbackRequestRequestTypeDef",
     "StopReplicationRequestRequestTypeDef",
     "StopSourceNetworkReplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateRecoveryInstancesRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFailbackReplicationConfigurationRequestRequestTypeDef",
+    "CreateSourceNetworkResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportSourceNetworkCfnTemplateResponseTypeDef",
+    "GetFailbackReplicationConfigurationResponseTypeDef",
     "ListStagingAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ReverseReplicationResponseTypeDef",
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
     "LaunchConfigurationTemplateTypeDef",
     "LaunchConfigurationTypeDef",
     "UpdateLaunchConfigurationRequestRequestTypeDef",
     "UpdateLaunchConfigurationTemplateRequestRequestTypeDef",
     "CreateReplicationConfigurationTemplateRequestRequestTypeDef",
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+    "ReplicationConfigurationTemplateResponseTypeDef",
     "ReplicationConfigurationTemplateTypeDef",
     "UpdateReplicationConfigurationTemplateRequestRequestTypeDef",
     "DataReplicationInitiationTypeDef",
+    "DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    "ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     "DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     "DescribeRecoverySnapshotsRequestRequestTypeDef",
     "DescribeRecoverySnapshotsResponseTypeDef",
@@ -178,15 +178,15 @@
     "LifeCycleTypeDef",
     "JobTypeDef",
     "RecoveryInstanceDataReplicationInfoTypeDef",
     "DescribeSourceNetworksResponseTypeDef",
     "StartSourceNetworkReplicationResponseTypeDef",
     "StopSourceNetworkReplicationResponseTypeDef",
     "JobLogTypeDef",
-    "SourceServerResponseMetadataTypeDef",
+    "SourceServerResponseTypeDef",
     "SourceServerTypeDef",
     "AssociateSourceNetworkStackResponseTypeDef",
     "DescribeJobsResponseTypeDef",
     "StartFailbackLaunchResponseTypeDef",
     "StartRecoveryResponseTypeDef",
     "StartSourceNetworkRecoveryResponseTypeDef",
     "TerminateRecoveryInstancesResponseTypeDef",
@@ -211,14 +211,25 @@
     "AssociateSourceNetworkStackRequestRequestTypeDef",
     {
         "cfnStackName": str,
         "sourceNetworkID": str,
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
 CPUTypeDef = TypedDict(
     "CPUTypeDef",
     {
         "cores": int,
         "modelName": str,
     },
     total=False,
@@ -302,22 +313,14 @@
 
 class CreateSourceNetworkRequestRequestTypeDef(
     _RequiredCreateSourceNetworkRequestRequestTypeDef,
     _OptionalCreateSourceNetworkRequestRequestTypeDef,
 ):
     pass
 
-CreateSourceNetworkResponseTypeDef = TypedDict(
-    "CreateSourceNetworkResponseTypeDef",
-    {
-        "sourceNetworkID": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataReplicationErrorTypeDef = TypedDict(
     "DataReplicationErrorTypeDef",
     {
         "error": DataReplicationErrorStringType,
         "rawError": str,
     },
     total=False,
@@ -382,34 +385,24 @@
 DeleteSourceServerRequestRequestTypeDef = TypedDict(
     "DeleteSourceServerRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
-_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
-    {
-        "jobID": str,
-    },
-)
-_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
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
 
-class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
-    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeJobLogItemsRequestRequestTypeDef",
     {
         "jobID": str,
     },
 )
 _OptionalDescribeJobLogItemsRequestRequestTypeDef = TypedDict(
@@ -433,23 +426,14 @@
         "fromDate": str,
         "jobIDs": Sequence[str],
         "toDate": str,
     },
     total=False,
 )
 
-DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
-    {
-        "launchConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeLaunchConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeLaunchConfigurationTemplatesRequestRequestTypeDef",
     {
         "launchConfigurationTemplateIDs": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -490,23 +474,14 @@
     },
     total=False,
 )
 
 class RecoverySnapshotTypeDef(_RequiredRecoverySnapshotTypeDef, _OptionalRecoverySnapshotTypeDef):
     pass
 
-DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
-    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
-    {
-        "replicationConfigurationTemplateIDs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReplicationConfigurationTemplatesRequestRequestTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "replicationConfigurationTemplateIDs": Sequence[str],
     },
@@ -552,21 +527,14 @@
     {
         "bytes": int,
         "deviceName": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SourceNetworkDataTypeDef = TypedDict(
     "SourceNetworkDataTypeDef",
     {
         "sourceNetworkID": str,
         "sourceVpc": str,
         "stackName": str,
         "targetVpc": str,
@@ -577,40 +545,21 @@
 ExportSourceNetworkCfnTemplateRequestRequestTypeDef = TypedDict(
     "ExportSourceNetworkCfnTemplateRequestRequestTypeDef",
     {
         "sourceNetworkID": str,
     },
 )
 
-ExportSourceNetworkCfnTemplateResponseTypeDef = TypedDict(
-    "ExportSourceNetworkCfnTemplateResponseTypeDef",
-    {
-        "s3DestinationUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFailbackReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "GetFailbackReplicationConfigurationRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
-GetFailbackReplicationConfigurationResponseTypeDef = TypedDict(
-    "GetFailbackReplicationConfigurationResponseTypeDef",
-    {
-        "bandwidthThrottling": int,
-        "name": str,
-        "recoveryInstanceID": str,
-        "usePrivateIP": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "GetLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
@@ -648,34 +597,14 @@
         "apiCallDateTime": str,
         "jobID": str,
         "type": LastLaunchTypeType,
     },
     total=False,
 )
 
-_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
-    "_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    {
-        "stagingAccountID": str,
-    },
-)
-_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
-    "_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(
-    _RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-    _OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
-):
-    pass
-
 _RequiredListExtensibleSourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListExtensibleSourceServersRequestRequestTypeDef",
     {
         "stagingAccountID": str,
     },
 )
 _OptionalListExtensibleSourceServersRequestRequestTypeDef = TypedDict(
@@ -699,22 +628,14 @@
         "arn": str,
         "hostname": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = TypedDict(
-    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStagingAccountsRequestRequestTypeDef = TypedDict(
     "ListStagingAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -723,22 +644,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "ips": List[str],
         "isPrimary": bool,
         "macAddress": str,
     },
@@ -749,24 +662,14 @@
     "OSTypeDef",
     {
         "fullString": str,
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
 ParticipatingResourceIDTypeDef = TypedDict(
     "ParticipatingResourceIDTypeDef",
     {
         "sourceNetworkID": str,
     },
     total=False,
 )
@@ -847,47 +750,28 @@
         "optimizedStagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "stagingDiskType": ReplicationConfigurationReplicatedDiskStagingDiskTypeType,
         "throughput": int,
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
 RetryDataReplicationRequestRequestTypeDef = TypedDict(
     "RetryDataReplicationRequestRequestTypeDef",
     {
         "sourceServerID": str,
     },
 )
 
 ReverseReplicationRequestRequestTypeDef = TypedDict(
     "ReverseReplicationRequestRequestTypeDef",
     {
         "recoveryInstanceID": str,
     },
 )
 
-ReverseReplicationResponseTypeDef = TypedDict(
-    "ReverseReplicationResponseTypeDef",
-    {
-        "reversedDirectionSourceServerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SourceCloudPropertiesTypeDef = TypedDict(
     "SourceCloudPropertiesTypeDef",
     {
         "originAccountID": str,
         "originAvailabilityZone": str,
         "originRegion": str,
     },
@@ -1041,20 +925,70 @@
 
 class UpdateFailbackReplicationConfigurationRequestRequestTypeDef(
     _RequiredUpdateFailbackReplicationConfigurationRequestRequestTypeDef,
     _OptionalUpdateFailbackReplicationConfigurationRequestRequestTypeDef,
 ):
     pass
 
+CreateSourceNetworkResponseTypeDef = TypedDict(
+    "CreateSourceNetworkResponseTypeDef",
+    {
+        "sourceNetworkID": str,
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
+ExportSourceNetworkCfnTemplateResponseTypeDef = TypedDict(
+    "ExportSourceNetworkCfnTemplateResponseTypeDef",
+    {
+        "s3DestinationUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFailbackReplicationConfigurationResponseTypeDef = TypedDict(
+    "GetFailbackReplicationConfigurationResponseTypeDef",
+    {
+        "bandwidthThrottling": int,
+        "name": str,
+        "recoveryInstanceID": str,
+        "usePrivateIP": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListStagingAccountsResponseTypeDef = TypedDict(
     "ListStagingAccountsResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReverseReplicationResponseTypeDef = TypedDict(
+    "ReverseReplicationResponseTypeDef",
+    {
+        "reversedDirectionSourceServerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLaunchConfigurationTemplateRequestRequestTypeDef = TypedDict(
     "CreateLaunchConfigurationTemplateRequestRequestTypeDef",
     {
         "copyPrivateIp": bool,
@@ -1091,15 +1025,15 @@
         "copyTags": bool,
         "ec2LaunchTemplateID": str,
         "launchDisposition": LaunchDispositionType,
         "licensing": LicensingTypeDef,
         "name": str,
         "sourceServerID": str,
         "targetInstanceTypeRightSizingMethod": TargetInstanceTypeRightSizingMethodType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateLaunchConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
@@ -1178,16 +1112,16 @@
 
 class CreateReplicationConfigurationTemplateRequestRequestTypeDef(
     _RequiredCreateReplicationConfigurationTemplateRequestRequestTypeDef,
     _OptionalCreateReplicationConfigurationTemplateRequestRequestTypeDef,
 ):
     pass
 
-ReplicationConfigurationTemplateResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationTemplateResponseMetadataTypeDef",
+ReplicationConfigurationTemplateResponseTypeDef = TypedDict(
+    "ReplicationConfigurationTemplateResponseTypeDef",
     {
         "arn": str,
         "associateDefaultSecurityGroup": bool,
         "autoReplicateNewDisks": bool,
         "bandwidthThrottling": int,
         "createPublicIP": bool,
         "dataPlaneRouting": ReplicationConfigurationDataPlaneRoutingType,
@@ -1198,15 +1132,15 @@
         "replicationConfigurationTemplateID": str,
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "tags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredReplicationConfigurationTemplateTypeDef = TypedDict(
     "_RequiredReplicationConfigurationTemplateTypeDef",
     {
         "replicationConfigurationTemplateID": str,
@@ -1281,19 +1215,85 @@
         "nextAttemptDateTime": str,
         "startDateTime": str,
         "steps": List[DataReplicationInitiationStepTypeDef],
     },
     total=False,
 )
 
+_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    {
+        "jobID": str,
+    },
+)
+_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef(
+    _RequiredDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    _OptionalDescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+):
+    pass
+
+DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef",
+    {
+        "launchConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = TypedDict(
+    "DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef",
+    {
+        "replicationConfigurationTemplateIDs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
+    "_RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    {
+        "stagingAccountID": str,
+    },
+)
+_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = TypedDict(
+    "_OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef(
+    _RequiredListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+    _OptionalListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+):
+    pass
+
+ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = TypedDict(
+    "ListStagingAccountsRequestListStagingAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeJobsRequestDescribeJobsPaginateTypeDef = TypedDict(
     "DescribeJobsRequestDescribeJobsPaginateTypeDef",
     {
         "filters": DescribeJobsRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeJobsRequestRequestTypeDef = TypedDict(
     "DescribeJobsRequestRequestTypeDef",
     {
@@ -1304,15 +1304,15 @@
     total=False,
 )
 
 DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef",
     {
         "filters": DescribeRecoveryInstancesRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeRecoveryInstancesRequestRequestTypeDef = TypedDict(
     "DescribeRecoveryInstancesRequestRequestTypeDef",
     {
@@ -1330,15 +1330,15 @@
     },
 )
 _OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef = TypedDict(
     "_OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef",
     {
         "filters": DescribeRecoverySnapshotsRequestFiltersTypeDef,
         "order": RecoverySnapshotsOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef(
     _RequiredDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     _OptionalDescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
@@ -1369,23 +1369,23 @@
     pass
 
 DescribeRecoverySnapshotsResponseTypeDef = TypedDict(
     "DescribeRecoverySnapshotsResponseTypeDef",
     {
         "items": List[RecoverySnapshotTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef = TypedDict(
     "DescribeSourceNetworksRequestDescribeSourceNetworksPaginateTypeDef",
     {
         "filters": DescribeSourceNetworksRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSourceNetworksRequestRequestTypeDef = TypedDict(
     "DescribeSourceNetworksRequestRequestTypeDef",
     {
@@ -1396,15 +1396,15 @@
     total=False,
 )
 
 DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = TypedDict(
     "DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef",
     {
         "filters": DescribeSourceServersRequestFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeSourceServersRequestRequestTypeDef = TypedDict(
     "DescribeSourceServersRequestRequestTypeDef",
     {
@@ -1433,15 +1433,15 @@
 )
 
 ListExtensibleSourceServersResponseTypeDef = TypedDict(
     "ListExtensibleSourceServersResponseTypeDef",
     {
         "items": List[StagingSourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourcePropertiesTypeDef = TypedDict(
     "SourcePropertiesTypeDef",
     {
         "cpus": List[CPUTypeDef],
@@ -1523,15 +1523,15 @@
         "replicatedDisks": List[ReplicationConfigurationReplicatedDiskTypeDef],
         "replicationServerInstanceType": str,
         "replicationServersSecurityGroupsIDs": List[str],
         "sourceServerID": str,
         "stagingAreaSubnetId": str,
         "stagingAreaTags": Dict[str, str],
         "useDedicatedReplicationServer": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateReplicationConfigurationRequestRequestTypeDef",
     {
         "sourceServerID": str,
@@ -1607,41 +1607,41 @@
 ):
     pass
 
 CreateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
     "CreateLaunchConfigurationTemplateResponseTypeDef",
     {
         "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLaunchConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeLaunchConfigurationTemplatesResponseTypeDef",
     {
         "items": List[LaunchConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLaunchConfigurationTemplateResponseTypeDef = TypedDict(
     "UpdateLaunchConfigurationTemplateResponseTypeDef",
     {
         "launchConfigurationTemplate": LaunchConfigurationTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationConfigurationTemplatesResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationTemplatesResponseTypeDef",
     {
         "items": List[ReplicationConfigurationTemplateTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataReplicationInfoTypeDef = TypedDict(
     "DataReplicationInfoTypeDef",
     {
         "dataReplicationError": DataReplicationErrorTypeDef,
@@ -1720,61 +1720,61 @@
 )
 
 DescribeSourceNetworksResponseTypeDef = TypedDict(
     "DescribeSourceNetworksResponseTypeDef",
     {
         "items": List[SourceNetworkTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSourceNetworkReplicationResponseTypeDef = TypedDict(
     "StartSourceNetworkReplicationResponseTypeDef",
     {
         "sourceNetwork": SourceNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopSourceNetworkReplicationResponseTypeDef = TypedDict(
     "StopSourceNetworkReplicationResponseTypeDef",
     {
         "sourceNetwork": SourceNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobLogTypeDef = TypedDict(
     "JobLogTypeDef",
     {
         "event": JobLogEventType,
         "eventData": JobLogEventDataTypeDef,
         "logDateTime": str,
     },
     total=False,
 )
 
-SourceServerResponseMetadataTypeDef = TypedDict(
-    "SourceServerResponseMetadataTypeDef",
+SourceServerResponseTypeDef = TypedDict(
+    "SourceServerResponseTypeDef",
     {
         "arn": str,
         "dataReplicationInfo": DataReplicationInfoTypeDef,
         "lastLaunchResult": LastLaunchResultType,
         "lifeCycle": LifeCycleTypeDef,
         "recoveryInstanceId": str,
         "replicationDirection": ReplicationDirectionType,
         "reversedDirectionSourceServerArn": str,
         "sourceCloudProperties": SourceCloudPropertiesTypeDef,
         "sourceNetworkID": str,
         "sourceProperties": SourcePropertiesTypeDef,
         "sourceServerID": str,
         "stagingArea": StagingAreaTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SourceServerTypeDef = TypedDict(
     "SourceServerTypeDef",
     {
         "arn": str,
@@ -1794,56 +1794,56 @@
     total=False,
 )
 
 AssociateSourceNetworkStackResponseTypeDef = TypedDict(
     "AssociateSourceNetworkStackResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "items": List[JobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFailbackLaunchResponseTypeDef = TypedDict(
     "StartFailbackLaunchResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartRecoveryResponseTypeDef = TypedDict(
     "StartRecoveryResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSourceNetworkRecoveryResponseTypeDef = TypedDict(
     "StartSourceNetworkRecoveryResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TerminateRecoveryInstancesResponseTypeDef = TypedDict(
     "TerminateRecoveryInstancesResponseTypeDef",
     {
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecoveryInstanceTypeDef = TypedDict(
     "RecoveryInstanceTypeDef",
     {
         "arn": str,
@@ -1865,52 +1865,52 @@
 )
 
 DescribeJobLogItemsResponseTypeDef = TypedDict(
     "DescribeJobLogItemsResponseTypeDef",
     {
         "items": List[JobLogTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExtendedSourceServerResponseTypeDef = TypedDict(
     "CreateExtendedSourceServerResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSourceServersResponseTypeDef = TypedDict(
     "DescribeSourceServersResponseTypeDef",
     {
         "items": List[SourceServerTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartReplicationResponseTypeDef = TypedDict(
     "StartReplicationResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopReplicationResponseTypeDef = TypedDict(
     "StopReplicationResponseTypeDef",
     {
         "sourceServer": SourceServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecoveryInstancesResponseTypeDef = TypedDict(
     "DescribeRecoveryInstancesResponseTypeDef",
     {
         "items": List[RecoveryInstanceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/PKG-INFO` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-drs
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.drs 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.drs 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore drs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore drs type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-drs"></a>
 
 # types-aiobotocore-drs
 
 [![PyPI - types-aiobotocore-drs](https://img.shields.io/pypi/v/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-drs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-drs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-drs?color=blue)](https://pypistats.org/packages/types-aiobotocore-drs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-drs)](https://pepy.tech/project/types-aiobotocore-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.drs 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
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
 [types-aiobotocore-drs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_drs/).
 
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
@@ -381,114 +380,114 @@
 )
 
 
 def check_value(value: DataReplicationErrorStringType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_drs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_drs.type_defs import (
     AccountTypeDef,
     AssociateSourceNetworkStackRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     CPUTypeDef,
     ConversionPropertiesTypeDef,
     CreateExtendedSourceServerRequestRequestTypeDef,
     LicensingTypeDef,
     PITPolicyRuleTypeDef,
     CreateSourceNetworkRequestRequestTypeDef,
-    CreateSourceNetworkResponseTypeDef,
     DataReplicationErrorTypeDef,
     DataReplicationInfoReplicatedDiskTypeDef,
     DataReplicationInitiationStepTypeDef,
     DeleteJobRequestRequestTypeDef,
     DeleteLaunchConfigurationTemplateRequestRequestTypeDef,
     DeleteRecoveryInstanceRequestRequestTypeDef,
     DeleteReplicationConfigurationTemplateRequestRequestTypeDef,
     DeleteSourceNetworkRequestRequestTypeDef,
     DeleteSourceServerRequestRequestTypeDef,
-    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeJobLogItemsRequestRequestTypeDef,
     DescribeJobsRequestFiltersTypeDef,
-    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
     DescribeLaunchConfigurationTemplatesRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestFiltersTypeDef,
     DescribeRecoverySnapshotsRequestFiltersTypeDef,
     RecoverySnapshotTypeDef,
-    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
     DescribeReplicationConfigurationTemplatesRequestRequestTypeDef,
     DescribeSourceNetworksRequestFiltersTypeDef,
     DescribeSourceServersRequestFiltersTypeDef,
     DisconnectRecoveryInstanceRequestRequestTypeDef,
     DisconnectSourceServerRequestRequestTypeDef,
     DiskTypeDef,
-    EmptyResponseMetadataTypeDef,
     SourceNetworkDataTypeDef,
     ExportSourceNetworkCfnTemplateRequestRequestTypeDef,
-    ExportSourceNetworkCfnTemplateResponseTypeDef,
     GetFailbackReplicationConfigurationRequestRequestTypeDef,
-    GetFailbackReplicationConfigurationResponseTypeDef,
     GetLaunchConfigurationRequestRequestTypeDef,
     GetReplicationConfigurationRequestRequestTypeDef,
     IdentificationHintsTypeDef,
     ParticipatingServerTypeDef,
     LifeCycleLastLaunchInitiatedTypeDef,
-    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
     ListExtensibleSourceServersRequestRequestTypeDef,
     StagingSourceServerTypeDef,
-    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     ListStagingAccountsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NetworkInterfaceTypeDef,
     OSTypeDef,
-    PaginatorConfigTypeDef,
     ParticipatingResourceIDTypeDef,
     RecoveryInstanceDataReplicationErrorTypeDef,
     RecoveryInstanceDataReplicationInfoReplicatedDiskTypeDef,
     RecoveryInstanceDataReplicationInitiationStepTypeDef,
     RecoveryInstanceDiskTypeDef,
     RecoveryInstanceFailbackTypeDef,
     RecoveryLifeCycleTypeDef,
     ReplicationConfigurationReplicatedDiskTypeDef,
-    ResponseMetadataTypeDef,
     RetryDataReplicationRequestRequestTypeDef,
     ReverseReplicationRequestRequestTypeDef,
-    ReverseReplicationResponseTypeDef,
     SourceCloudPropertiesTypeDef,
     StagingAreaTypeDef,
     StartFailbackLaunchRequestRequestTypeDef,
     StartRecoveryRequestSourceServerTypeDef,
     StartReplicationRequestRequestTypeDef,
     StartSourceNetworkRecoveryRequestNetworkEntryTypeDef,
     StartSourceNetworkReplicationRequestRequestTypeDef,
     StopFailbackRequestRequestTypeDef,
     StopReplicationRequestRequestTypeDef,
     StopSourceNetworkReplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateRecoveryInstancesRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFailbackReplicationConfigurationRequestRequestTypeDef,
+    CreateSourceNetworkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportSourceNetworkCfnTemplateResponseTypeDef,
+    GetFailbackReplicationConfigurationResponseTypeDef,
     ListStagingAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ReverseReplicationResponseTypeDef,
     CreateLaunchConfigurationTemplateRequestRequestTypeDef,
     LaunchConfigurationTemplateTypeDef,
     LaunchConfigurationTypeDef,
     UpdateLaunchConfigurationRequestRequestTypeDef,
     UpdateLaunchConfigurationTemplateRequestRequestTypeDef,
     CreateReplicationConfigurationTemplateRequestRequestTypeDef,
-    ReplicationConfigurationTemplateResponseMetadataTypeDef,
+    ReplicationConfigurationTemplateResponseTypeDef,
     ReplicationConfigurationTemplateTypeDef,
     UpdateReplicationConfigurationTemplateRequestRequestTypeDef,
     DataReplicationInitiationTypeDef,
+    DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef,
+    DescribeLaunchConfigurationTemplatesRequestDescribeLaunchConfigurationTemplatesPaginateTypeDef,
+    DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef,
+    ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef,
+    ListStagingAccountsRequestListStagingAccountsPaginateTypeDef,
     DescribeJobsRequestDescribeJobsPaginateTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef,
     DescribeRecoveryInstancesRequestRequestTypeDef,
     DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef,
     DescribeRecoverySnapshotsRequestRequestTypeDef,
     DescribeRecoverySnapshotsResponseTypeDef,
@@ -517,15 +516,15 @@
     LifeCycleTypeDef,
     JobTypeDef,
     RecoveryInstanceDataReplicationInfoTypeDef,
     DescribeSourceNetworksResponseTypeDef,
     StartSourceNetworkReplicationResponseTypeDef,
     StopSourceNetworkReplicationResponseTypeDef,
     JobLogTypeDef,
-    SourceServerResponseMetadataTypeDef,
+    SourceServerResponseTypeDef,
     SourceServerTypeDef,
     AssociateSourceNetworkStackResponseTypeDef,
     DescribeJobsResponseTypeDef,
     StartFailbackLaunchResponseTypeDef,
     StartRecoveryResponseTypeDef,
     StartSourceNetworkRecoveryResponseTypeDef,
     TerminateRecoveryInstancesResponseTypeDef,
@@ -535,15 +534,15 @@
     DescribeSourceServersResponseTypeDef,
     StartReplicationResponseTypeDef,
     StopReplicationResponseTypeDef,
     DescribeRecoveryInstancesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountTypeDef:
+def get_value() -> AccountTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-drs-2.5.2/types_aiobotocore_drs.egg-info/SOURCES.txt` & `types-aiobotocore-drs-2.5.2.post1/types_aiobotocore_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


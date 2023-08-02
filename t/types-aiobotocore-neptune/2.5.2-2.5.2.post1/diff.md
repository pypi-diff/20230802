# Comparing `tmp/types-aiobotocore-neptune-2.5.2.tar.gz` & `tmp/types-aiobotocore-neptune-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-neptune-2.5.2.tar", last modified: Sat Jul  8 01:44:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-neptune-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:43 2023, max compression
```

## Comparing `types-aiobotocore-neptune-2.5.2.tar` & `types-aiobotocore-neptune-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.682602 types-aiobotocore-neptune-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:35:37.000000 types-aiobotocore-neptune-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26169 2023-07-08 01:44:02.682602 types-aiobotocore-neptune-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24604 2023-07-08 01:35:37.000000 types-aiobotocore-neptune-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:02.682602 types-aiobotocore-neptune-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:35:37.000000 types-aiobotocore-neptune-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.682602 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-08 01:35:37.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-07-08 01:35:37.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:35:37.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70635 2023-07-08 01:35:37.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    70539 2023-07-08 01:35:37.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-07-08 01:35:39.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-07-08 01:35:39.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22262 2023-07-08 01:35:39.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-07-08 01:35:38.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:35:37.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    84596 2023-07-08 01:35:41.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    84519 2023-07-08 01:35:40.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:35:37.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-08 01:35:39.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-08 01:35:39.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.682602 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26169 2023-07-08 01:44:02.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-08 01:44:02.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:02.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:44:02.000000 types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.237512 types-aiobotocore-neptune-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-08-02 14:52:43.237512 types-aiobotocore-neptune-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24609 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:43.237512 types-aiobotocore-neptune-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.233512 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70608 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70512 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-08-02 14:43:56.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-08-02 14:43:56.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-08-02 14:43:56.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22165 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    84484 2023-08-02 14:43:57.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84407 2023-08-02 14:43:57.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-08-02 14:43:56.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-02 14:43:56.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.237512 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-08-02 14:52:43.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 14:52:43.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:43.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:52:43.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-neptune-2.5.2/LICENSE` & `types-aiobotocore-neptune-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2/PKG-INFO` & `types-aiobotocore-neptune-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-neptune
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Neptune 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Neptune 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore neptune type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore neptune type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-neptune"></a>
 
 # types-aiobotocore-neptune
 
 [![PyPI - types-aiobotocore-neptune](https://img.shields.io/pypi/v/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-neptune?color=blue)](https://pypistats.org/packages/types-aiobotocore-neptune)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-neptune)](https://pepy.tech/project/types-aiobotocore-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Neptune 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [types-aiobotocore-neptune docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -412,101 +411,101 @@
 )
 
 
 def check_value(value: ApplyMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_neptune.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_neptune.type_defs import (
     AddRoleToDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     CharacterSetTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     DBParameterGroupTypeDef,
-    CreateDBClusterEndpointOutputTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterEndpointTypeDef,
     DBClusterMemberTypeDef,
     DBClusterOptionGroupStatusTypeDef,
     ParameterTypeDef,
-    DBClusterParameterGroupNameMessageTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     ServerlessV2ScalingConfigurationInfoTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     TimezoneTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     DBParameterGroupStatusTypeDef,
     DBSecurityGroupMembershipTypeDef,
     DomainMembershipTypeDef,
     EndpointTypeDef,
     OptionGroupMembershipTypeDef,
-    DBParameterGroupNameMessageTypeDef,
     DeleteDBClusterEndpointMessageRequestTypeDef,
-    DeleteDBClusterEndpointOutputTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBParameterGroupMessageRequestTypeDef,
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
+    TimestampTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
     DescribeValidDBInstanceModificationsMessageRequestTypeDef,
     DoubleRangeTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     FailoverGlobalClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ModifyDBClusterEndpointMessageRequestTypeDef,
-    ModifyDBClusterEndpointOutputTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PromoteReadReplicaDBClusterMessageRequestTypeDef,
     RangeTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveRoleFromDBClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
+    CreateDBClusterEndpointOutputTypeDef,
     CreateEventSubscriptionResultTypeDef,
+    DBClusterParameterGroupNameMessageTypeDef,
+    DBParameterGroupNameMessageTypeDef,
+    DeleteDBClusterEndpointOutputTypeDef,
     DeleteEventSubscriptionResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
+    ModifyDBClusterEndpointOutputTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopyDBClusterParameterGroupMessageRequestTypeDef,
     CopyDBClusterSnapshotMessageRequestTypeDef,
     CopyDBParameterGroupMessageRequestTypeDef,
     CreateDBClusterEndpointMessageRequestTypeDef,
@@ -531,60 +530,61 @@
     DeleteDBClusterSnapshotResultTypeDef,
     CopyDBParameterGroupResultTypeDef,
     CreateDBParameterGroupResultTypeDef,
     DBParameterGroupsMessageTypeDef,
     CreateDBClusterMessageRequestTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
-    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     ModifyDBClusterParameterGroupMessageRequestTypeDef,
     ModifyDBParameterGroupMessageRequestTypeDef,
     ResetDBClusterParameterGroupMessageRequestTypeDef,
     ResetDBParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBEngineVersionTypeDef,
-    DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
     DescribeDBClusterEndpointsMessageRequestTypeDef,
-    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
-    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
-    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
-    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
-    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
-    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBInstancesMessageRequestTypeDef,
-    DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
     DescribeDBParameterGroupsMessageRequestTypeDef,
-    DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     DescribeDBParametersMessageRequestTypeDef,
-    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
+    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
+    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
+    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
+    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
+    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
+    DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
+    DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
+    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
+    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
@@ -622,15 +622,15 @@
     DBInstanceMessageTypeDef,
     DeleteDBInstanceResultTypeDef,
     ModifyDBInstanceResultTypeDef,
     RebootDBInstanceResultTypeDef,
 )
 
 
-def get_structure() -> AddRoleToDBClusterMessageRequestTypeDef:
+def get_value() -> AddRoleToDBClusterMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-neptune-2.5.2/README.md` & `types-aiobotocore-neptune-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-neptune"></a>
 
 # types-aiobotocore-neptune
 
 [![PyPI - types-aiobotocore-neptune](https://img.shields.io/pypi/v/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-neptune?color=blue)](https://pypistats.org/packages/types-aiobotocore-neptune)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-neptune)](https://pepy.tech/project/types-aiobotocore-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Neptune 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [types-aiobotocore-neptune docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -379,101 +379,101 @@
 )
 
 
 def check_value(value: ApplyMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_neptune.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_neptune.type_defs import (
     AddRoleToDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     CharacterSetTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     DBParameterGroupTypeDef,
-    CreateDBClusterEndpointOutputTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterEndpointTypeDef,
     DBClusterMemberTypeDef,
     DBClusterOptionGroupStatusTypeDef,
     ParameterTypeDef,
-    DBClusterParameterGroupNameMessageTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     ServerlessV2ScalingConfigurationInfoTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     TimezoneTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     DBParameterGroupStatusTypeDef,
     DBSecurityGroupMembershipTypeDef,
     DomainMembershipTypeDef,
     EndpointTypeDef,
     OptionGroupMembershipTypeDef,
-    DBParameterGroupNameMessageTypeDef,
     DeleteDBClusterEndpointMessageRequestTypeDef,
-    DeleteDBClusterEndpointOutputTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBParameterGroupMessageRequestTypeDef,
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
+    TimestampTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
     DescribeValidDBInstanceModificationsMessageRequestTypeDef,
     DoubleRangeTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     FailoverGlobalClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ModifyDBClusterEndpointMessageRequestTypeDef,
-    ModifyDBClusterEndpointOutputTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PromoteReadReplicaDBClusterMessageRequestTypeDef,
     RangeTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveRoleFromDBClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
+    CreateDBClusterEndpointOutputTypeDef,
     CreateEventSubscriptionResultTypeDef,
+    DBClusterParameterGroupNameMessageTypeDef,
+    DBParameterGroupNameMessageTypeDef,
+    DeleteDBClusterEndpointOutputTypeDef,
     DeleteEventSubscriptionResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
+    ModifyDBClusterEndpointOutputTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopyDBClusterParameterGroupMessageRequestTypeDef,
     CopyDBClusterSnapshotMessageRequestTypeDef,
     CopyDBParameterGroupMessageRequestTypeDef,
     CreateDBClusterEndpointMessageRequestTypeDef,
@@ -498,60 +498,61 @@
     DeleteDBClusterSnapshotResultTypeDef,
     CopyDBParameterGroupResultTypeDef,
     CreateDBParameterGroupResultTypeDef,
     DBParameterGroupsMessageTypeDef,
     CreateDBClusterMessageRequestTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
-    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     ModifyDBClusterParameterGroupMessageRequestTypeDef,
     ModifyDBParameterGroupMessageRequestTypeDef,
     ResetDBClusterParameterGroupMessageRequestTypeDef,
     ResetDBParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBEngineVersionTypeDef,
-    DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
     DescribeDBClusterEndpointsMessageRequestTypeDef,
-    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
-    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
-    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
-    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
-    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
-    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBInstancesMessageRequestTypeDef,
-    DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
     DescribeDBParameterGroupsMessageRequestTypeDef,
-    DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     DescribeDBParametersMessageRequestTypeDef,
-    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
+    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
+    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
+    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
+    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
+    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
+    DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
+    DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
+    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
+    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
@@ -589,15 +590,15 @@
     DBInstanceMessageTypeDef,
     DeleteDBInstanceResultTypeDef,
     ModifyDBInstanceResultTypeDef,
     RebootDBInstanceResultTypeDef,
 )
 
 
-def get_structure() -> AddRoleToDBClusterMessageRequestTypeDef:
+def get_value() -> AddRoleToDBClusterMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-neptune-2.5.2/setup.py` & `types-aiobotocore-neptune-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-neptune",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_neptune"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Neptune 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore neptune type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore neptune type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_neptune": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/"
```

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/__init__.py` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/__init__.pyi` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/client.py` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("neptune") as client:
         client: NeptuneClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import SourceTypeType
 from .paginator import (
     DescribeDBClusterEndpointsPaginator,
@@ -103,14 +102,15 @@
     RestoreDBClusterFromSnapshotResultTypeDef,
     RestoreDBClusterToPointInTimeResultTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     StartDBClusterResultTypeDef,
     StopDBClusterResultTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import DBInstanceAvailableWaiter, DBInstanceDeletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -856,16 +856,16 @@
         """
 
     async def describe_events(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> EventsMessageTypeDef:
         """
@@ -1271,15 +1271,15 @@
 
     async def restore_db_cluster_to_point_in_time(
         self,
         *,
         DBClusterIdentifier: str,
         SourceDBClusterIdentifier: str,
         RestoreType: str = ...,
-        RestoreToTime: Union[datetime, str] = ...,
+        RestoreToTime: TimestampTypeDef = ...,
         UseLatestRestorableTime: bool = ...,
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         OptionGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
```

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/client.pyi` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("neptune") as client:
         client: NeptuneClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import SourceTypeType
 from .paginator import (
     DescribeDBClusterEndpointsPaginator,
@@ -103,14 +102,15 @@
     RestoreDBClusterFromSnapshotResultTypeDef,
     RestoreDBClusterToPointInTimeResultTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     StartDBClusterResultTypeDef,
     StopDBClusterResultTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import DBInstanceAvailableWaiter, DBInstanceDeletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -809,16 +809,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/client/#describe_event_subscriptions)
         """
     async def describe_events(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> EventsMessageTypeDef:
         """
@@ -1197,15 +1197,15 @@
         """
     async def restore_db_cluster_to_point_in_time(
         self,
         *,
         DBClusterIdentifier: str,
         SourceDBClusterIdentifier: str,
         RestoreType: str = ...,
-        RestoreToTime: Union[datetime, str] = ...,
+        RestoreToTime: TimestampTypeDef = ...,
         UseLatestRestorableTime: bool = ...,
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         OptionGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
```

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/literals.py` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/literals.pyi` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/paginator.py` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,16 +46,15 @@
         describe_event_subscriptions_paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
         describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
         describe_global_clusters_paginator: DescribeGlobalClustersPaginator = client.get_paginator("describe_global_clusters")
         describe_orderable_db_instance_options_paginator: DescribeOrderableDBInstanceOptionsPaginator = client.get_paginator("describe_orderable_db_instance_options")
         describe_pending_maintenance_actions_paginator: DescribePendingMaintenanceActionsPaginator = client.get_paginator("describe_pending_maintenance_actions")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import SourceTypeType
 from .type_defs import (
     DBClusterEndpointMessageTypeDef,
@@ -72,14 +71,15 @@
     EventsMessageTypeDef,
     EventSubscriptionsMessageTypeDef,
     FilterTypeDef,
     GlobalClustersMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     PaginatorConfigTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeDBClusterEndpointsPaginator",
     "DescribeDBClusterParameterGroupsPaginator",
     "DescribeDBClusterParametersPaginator",
     "DescribeDBClusterSnapshotsPaginator",
@@ -116,15 +116,15 @@
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         DBClusterEndpointIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBClusterEndpointMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterendpointspaginator)
         """
 
 
@@ -135,15 +135,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterparametergroupspaginator)
         """
 
 
@@ -155,15 +155,15 @@
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterparameterspaginator)
         """
 
 
@@ -178,15 +178,15 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclustersnapshotspaginator)
         """
 
 
@@ -197,15 +197,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterspaginator)
         """
 
 
@@ -221,15 +221,15 @@
         Engine: str = ...,
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbengineversionspaginator)
         """
 
 
@@ -240,15 +240,15 @@
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbinstancespaginator)
         """
 
 
@@ -259,15 +259,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbparametergroupspaginator)
         """
 
 
@@ -279,15 +279,15 @@
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbparameterspaginator)
         """
 
 
@@ -298,15 +298,15 @@
     """
 
     def paginate(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbsubnetgroupspaginator)
         """
 
 
@@ -317,15 +317,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeenginedefaultparameterspaginator)
         """
 
 
@@ -336,15 +336,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -355,38 +355,35 @@
     """
 
     def paginate(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeeventspaginator)
         """
 
 
 class DescribeGlobalClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeGlobalClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeglobalclusterspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        GlobalClusterIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GlobalClusterIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeGlobalClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeglobalclusterspaginator)
         """
 
 
@@ -401,15 +398,15 @@
         *,
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[OrderableDBInstanceOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
 
@@ -420,13 +417,13 @@
     """
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[PendingMaintenanceActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describependingmaintenanceactionspaginator)
         """
```

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/paginator.pyi` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -46,16 +46,15 @@
         describe_event_subscriptions_paginator: DescribeEventSubscriptionsPaginator = client.get_paginator("describe_event_subscriptions")
         describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
         describe_global_clusters_paginator: DescribeGlobalClustersPaginator = client.get_paginator("describe_global_clusters")
         describe_orderable_db_instance_options_paginator: DescribeOrderableDBInstanceOptionsPaginator = client.get_paginator("describe_orderable_db_instance_options")
         describe_pending_maintenance_actions_paginator: DescribePendingMaintenanceActionsPaginator = client.get_paginator("describe_pending_maintenance_actions")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import SourceTypeType
 from .type_defs import (
     DBClusterEndpointMessageTypeDef,
@@ -72,14 +71,15 @@
     EventsMessageTypeDef,
     EventSubscriptionsMessageTypeDef,
     FilterTypeDef,
     GlobalClustersMessageTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     PaginatorConfigTypeDef,
     PendingMaintenanceActionsMessageTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeDBClusterEndpointsPaginator",
     "DescribeDBClusterParameterGroupsPaginator",
     "DescribeDBClusterParametersPaginator",
     "DescribeDBClusterSnapshotsPaginator",
@@ -113,15 +113,15 @@
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         DBClusterEndpointIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBClusterEndpointMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterendpointspaginator)
         """
 
 class DescribeDBClusterParameterGroupsPaginator(AioPaginator):
@@ -131,15 +131,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterparametergroupspaginator)
         """
 
 class DescribeDBClusterParametersPaginator(AioPaginator):
@@ -150,15 +150,15 @@
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterparameterspaginator)
         """
 
 class DescribeDBClusterSnapshotsPaginator(AioPaginator):
@@ -172,15 +172,15 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclustersnapshotspaginator)
         """
 
 class DescribeDBClustersPaginator(AioPaginator):
@@ -190,15 +190,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbclusterspaginator)
         """
 
 class DescribeDBEngineVersionsPaginator(AioPaginator):
@@ -213,15 +213,15 @@
         Engine: str = ...,
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbengineversionspaginator)
         """
 
 class DescribeDBInstancesPaginator(AioPaginator):
@@ -231,15 +231,15 @@
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbinstancespaginator)
         """
 
 class DescribeDBParameterGroupsPaginator(AioPaginator):
@@ -249,15 +249,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbparametergroupspaginator)
         """
 
 class DescribeDBParametersPaginator(AioPaginator):
@@ -268,15 +268,15 @@
 
     def paginate(
         self,
         *,
         DBParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbparameterspaginator)
         """
 
 class DescribeDBSubnetGroupsPaginator(AioPaginator):
@@ -286,15 +286,15 @@
     """
 
     def paginate(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DBSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeDBSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describedbsubnetgroupspaginator)
         """
 
 class DescribeEngineDefaultParametersPaginator(AioPaginator):
@@ -304,15 +304,15 @@
     """
 
     def paginate(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeenginedefaultparameterspaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(AioPaginator):
@@ -322,15 +322,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -340,37 +340,34 @@
     """
 
     def paginate(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeeventspaginator)
         """
 
 class DescribeGlobalClustersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeGlobalClusters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeglobalclusterspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        GlobalClusterIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GlobalClusterIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeGlobalClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeglobalclusterspaginator)
         """
 
 class DescribeOrderableDBInstanceOptionsPaginator(AioPaginator):
@@ -384,15 +381,15 @@
         *,
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[OrderableDBInstanceOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
 class DescribePendingMaintenanceActionsPaginator(AioPaginator):
@@ -402,13 +399,13 @@
     """
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[PendingMaintenanceActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/paginators/#describependingmaintenanceactionspaginator)
         """
```

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/type_defs.py` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_neptune.type_defs import AddRoleToDBClusterMessageRequestTypeDef
 
-    data: AddRoleToDBClusterMessageRequestTypeDef = {...}
+    data: AddRoleToDBClusterMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplyMethodType, SourceTypeType
@@ -23,89 +23,89 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddRoleToDBClusterMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "CharacterSetTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
     "DBClusterParameterGroupTypeDef",
     "DBClusterSnapshotTypeDef",
     "DBParameterGroupTypeDef",
-    "CreateDBClusterEndpointOutputTypeDef",
     "ServerlessV2ScalingConfigurationTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
     "ParameterTypeDef",
-    "DBClusterParameterGroupNameMessageTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "ServerlessV2ScalingConfigurationInfoTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "TimezoneTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "DBParameterGroupStatusTypeDef",
     "DBSecurityGroupMembershipTypeDef",
     "DomainMembershipTypeDef",
     "EndpointTypeDef",
     "OptionGroupMembershipTypeDef",
-    "DBParameterGroupNameMessageTypeDef",
     "DeleteDBClusterEndpointMessageRequestTypeDef",
-    "DeleteDBClusterEndpointOutputTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     "DeleteDBClusterSnapshotMessageRequestTypeDef",
     "DeleteDBInstanceMessageRequestTypeDef",
     "DeleteDBParameterGroupMessageRequestTypeDef",
     "DeleteDBSubnetGroupMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteGlobalClusterMessageRequestTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    "TimestampTypeDef",
     "DescribeGlobalClustersMessageRequestTypeDef",
     "DescribeValidDBInstanceModificationsMessageRequestTypeDef",
     "DoubleRangeTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "FailoverGlobalClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
     "ModifyDBClusterEndpointMessageRequestTypeDef",
-    "ModifyDBClusterEndpointOutputTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     "RangeTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveRoleFromDBClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
+    "CreateDBClusterEndpointOutputTypeDef",
     "CreateEventSubscriptionResultTypeDef",
+    "DBClusterParameterGroupNameMessageTypeDef",
+    "DBParameterGroupNameMessageTypeDef",
+    "DeleteDBClusterEndpointOutputTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
+    "ModifyDBClusterEndpointOutputTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopyDBClusterParameterGroupMessageRequestTypeDef",
     "CopyDBClusterSnapshotMessageRequestTypeDef",
     "CopyDBParameterGroupMessageRequestTypeDef",
     "CreateDBClusterEndpointMessageRequestTypeDef",
@@ -130,60 +130,61 @@
     "DeleteDBClusterSnapshotResultTypeDef",
     "CopyDBParameterGroupResultTypeDef",
     "CreateDBParameterGroupResultTypeDef",
     "DBParameterGroupsMessageTypeDef",
     "CreateDBClusterMessageRequestTypeDef",
     "ModifyDBClusterMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
-    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "ModifyDBClusterParameterGroupMessageRequestTypeDef",
     "ModifyDBParameterGroupMessageRequestTypeDef",
     "ResetDBClusterParameterGroupMessageRequestTypeDef",
     "ResetDBParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBEngineVersionTypeDef",
-    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
-    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
-    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
-    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
-    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
     "DescribeDBClustersMessageRequestTypeDef",
-    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     "DescribeDBEngineVersionsMessageRequestTypeDef",
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     "DescribeDBInstancesMessageRequestTypeDef",
-    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     "DescribeDBParameterGroupsMessageRequestTypeDef",
-    "DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     "DescribeDBParametersMessageRequestTypeDef",
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultClusterParametersMessageRequestTypeDef",
-    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
-    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
-    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
+    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
+    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
+    "DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
+    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
+    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "ValidStorageOptionsTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
@@ -268,14 +269,25 @@
         "EventCategoriesList": List[str],
         "Enabled": bool,
         "EventSubscriptionArn": str,
     },
     total=False,
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -370,31 +382,14 @@
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBParameterGroupArn": str,
     },
     total=False,
 )
 
-CreateDBClusterEndpointOutputTypeDef = TypedDict(
-    "CreateDBClusterEndpointOutputTypeDef",
-    {
-        "DBClusterEndpointIdentifier": str,
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointResourceIdentifier": str,
-        "Endpoint": str,
-        "Status": str,
-        "EndpointType": str,
-        "CustomEndpointType": str,
-        "StaticMembers": List[str],
-        "ExcludedMembers": List[str],
-        "DBClusterEndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ServerlessV2ScalingConfigurationTypeDef = TypedDict(
     "ServerlessV2ScalingConfigurationTypeDef",
     {
         "MinCapacity": float,
         "MaxCapacity": float,
     },
     total=False,
@@ -476,22 +471,14 @@
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ApplyMethod": ApplyMethodType,
     },
     total=False,
 )
 
-DBClusterParameterGroupNameMessageTypeDef = TypedDict(
-    "DBClusterParameterGroupNameMessageTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DBClusterRoleTypeDef = TypedDict(
     "DBClusterRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
         "FeatureName": str,
     },
@@ -601,46 +588,21 @@
     {
         "OptionGroupName": str,
         "Status": str,
     },
     total=False,
 )
 
-DBParameterGroupNameMessageTypeDef = TypedDict(
-    "DBParameterGroupNameMessageTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
     },
 )
 
-DeleteDBClusterEndpointOutputTypeDef = TypedDict(
-    "DeleteDBClusterEndpointOutputTypeDef",
-    {
-        "DBClusterEndpointIdentifier": str,
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointResourceIdentifier": str,
-        "Endpoint": str,
-        "Status": str,
-        "EndpointType": str,
-        "CustomEndpointType": str,
-        "StaticMembers": List[str],
-        "ExcludedMembers": List[str],
-        "DBClusterEndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 _OptionalDeleteDBClusterMessageRequestTypeDef = TypedDict(
@@ -727,14 +689,24 @@
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 DescribeDBClusterSnapshotAttributesMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
     },
 )
 
@@ -743,23 +715,15 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
-    {
-        "GlobalClusterIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
     "DescribeGlobalClustersMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -778,21 +742,14 @@
     {
         "From": float,
         "To": float,
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
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
     total=False,
@@ -858,31 +815,14 @@
 class ModifyDBClusterEndpointMessageRequestTypeDef(
     _RequiredModifyDBClusterEndpointMessageRequestTypeDef,
     _OptionalModifyDBClusterEndpointMessageRequestTypeDef,
 ):
     pass
 
 
-ModifyDBClusterEndpointOutputTypeDef = TypedDict(
-    "ModifyDBClusterEndpointOutputTypeDef",
-    {
-        "DBClusterEndpointIdentifier": str,
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointResourceIdentifier": str,
-        "Endpoint": str,
-        "Status": str,
-        "EndpointType": str,
-        "CustomEndpointType": str,
-        "StaticMembers": List[str],
-        "ExcludedMembers": List[str],
-        "DBClusterEndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -972,24 +912,14 @@
 class ModifyGlobalClusterMessageRequestTypeDef(
     _RequiredModifyGlobalClusterMessageRequestTypeDef,
     _OptionalModifyGlobalClusterMessageRequestTypeDef,
 ):
     pass
 
 
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
@@ -1080,25 +1010,14 @@
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceName": str,
         "TagKeys": Sequence[str],
     },
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
 StartDBClusterMessageRequestTypeDef = TypedDict(
     "StartDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
@@ -1109,56 +1028,130 @@
     },
 )
 
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDBClusterEndpointOutputTypeDef = TypedDict(
+    "CreateDBClusterEndpointOutputTypeDef",
+    {
+        "DBClusterEndpointIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointResourceIdentifier": str,
+        "Endpoint": str,
+        "Status": str,
+        "EndpointType": str,
+        "CustomEndpointType": str,
+        "StaticMembers": List[str],
+        "ExcludedMembers": List[str],
+        "DBClusterEndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEventSubscriptionResultTypeDef = TypedDict(
     "CreateEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DBClusterParameterGroupNameMessageTypeDef = TypedDict(
+    "DBClusterParameterGroupNameMessageTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DBParameterGroupNameMessageTypeDef = TypedDict(
+    "DBParameterGroupNameMessageTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDBClusterEndpointOutputTypeDef = TypedDict(
+    "DeleteDBClusterEndpointOutputTypeDef",
+    {
+        "DBClusterEndpointIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointResourceIdentifier": str,
+        "Endpoint": str,
+        "Status": str,
+        "EndpointType": str,
+        "CustomEndpointType": str,
+        "StaticMembers": List[str],
+        "ExcludedMembers": List[str],
+        "DBClusterEndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventSubscriptionResultTypeDef = TypedDict(
     "DeleteEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventSubscriptionsMessageTypeDef = TypedDict(
     "EventSubscriptionsMessageTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyDBClusterEndpointOutputTypeDef = TypedDict(
+    "ModifyDBClusterEndpointOutputTypeDef",
+    {
+        "DBClusterEndpointIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointResourceIdentifier": str,
+        "Endpoint": str,
+        "Status": str,
+        "EndpointType": str,
+        "CustomEndpointType": str,
+        "StaticMembers": List[str],
+        "ExcludedMembers": List[str],
+        "DBClusterEndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyEventSubscriptionResultTypeDef = TypedDict(
     "ModifyEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveSourceIdentifierFromSubscriptionResultTypeDef = TypedDict(
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
     {
         "ResourceName": str,
@@ -1451,15 +1444,15 @@
     pass
 
 
 TagListMessageTypeDef = TypedDict(
     "TagListMessageTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
@@ -1588,90 +1581,90 @@
     total=False,
 )
 
 CopyDBClusterParameterGroupResultTypeDef = TypedDict(
     "CopyDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterParameterGroupResultTypeDef = TypedDict(
     "CreateDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupsMessageTypeDef = TypedDict(
     "DBClusterParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "DBClusterParameterGroups": List[DBClusterParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDBClusterSnapshotResultTypeDef = TypedDict(
     "CopyDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterSnapshotResultTypeDef = TypedDict(
     "CreateDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterSnapshotMessageTypeDef = TypedDict(
     "DBClusterSnapshotMessageTypeDef",
     {
         "Marker": str,
         "DBClusterSnapshots": List[DBClusterSnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBClusterSnapshotResultTypeDef = TypedDict(
     "DeleteDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDBParameterGroupResultTypeDef = TypedDict(
     "CopyDBParameterGroupResultTypeDef",
     {
         "DBParameterGroup": DBParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBParameterGroupResultTypeDef = TypedDict(
     "CreateDBParameterGroupResultTypeDef",
     {
         "DBParameterGroup": DBParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBParameterGroupsMessageTypeDef = TypedDict(
     "DBParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "DBParameterGroups": List[DBParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
@@ -1790,74 +1783,38 @@
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBClusterFromSnapshotMessageRequestTypeDef,
 ):
     pass
 
 
-_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
-    "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "SourceDBClusterIdentifier": str,
-    },
-)
-_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
-    "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
-    {
-        "RestoreType": str,
-        "RestoreToTime": Union[datetime, str],
-        "UseLatestRestorableTime": bool,
-        "Port": int,
-        "DBSubnetGroupName": str,
-        "OptionGroupName": str,
-        "VpcSecurityGroupIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "EnableIAMDatabaseAuthentication": bool,
-        "EnableCloudwatchLogsExports": Sequence[str],
-        "DBClusterParameterGroupName": str,
-        "DeletionProtection": bool,
-        "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
-    _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
-    _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
-):
-    pass
-
-
 DBClusterEndpointMessageTypeDef = TypedDict(
     "DBClusterEndpointMessageTypeDef",
     {
         "Marker": str,
         "DBClusterEndpoints": List[DBClusterEndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBParameterGroupDetailsTypeDef = TypedDict(
     "DBParameterGroupDetailsTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
@@ -1954,82 +1911,37 @@
         "SupportsLogExportsToCloudwatchLogs": bool,
         "SupportsReadReplica": bool,
         "SupportsGlobalDatabases": bool,
     },
     total=False,
 )
 
-DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
-    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
-    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeDBClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDBClusterParametersMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
     },
 )
 _OptionalDescribeDBClusterParametersMessageRequestTypeDef = TypedDict(
@@ -2047,28 +1959,14 @@
 class DescribeDBClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDBClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDBClusterParametersMessageRequestTypeDef,
 ):
     pass
 
 
-DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "DBClusterSnapshotIdentifier": str,
-        "SnapshotType": str,
-        "Filters": Sequence[FilterTypeDef],
-        "IncludeShared": bool,
-        "IncludePublic": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
@@ -2076,50 +1974,25 @@
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
     },
     total=False,
 )
 
-DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
-    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClustersMessageRequestTypeDef = TypedDict(
     "DescribeDBClustersMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
-    {
-        "Engine": str,
-        "EngineVersion": str,
-        "DBParameterGroupFamily": str,
-        "Filters": Sequence[FilterTypeDef],
-        "DefaultOnly": bool,
-        "ListSupportedCharacterSets": bool,
-        "ListSupportedTimezones": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBEngineVersionsMessageRequestTypeDef = TypedDict(
     "DescribeDBEngineVersionsMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "Filters": Sequence[FilterTypeDef],
@@ -2128,358 +2001,420 @@
         "DefaultOnly": bool,
         "ListSupportedCharacterSets": bool,
         "ListSupportedTimezones": bool,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+DescribeDBInstancesMessageRequestTypeDef = TypedDict(
+    "DescribeDBInstancesMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageRequestTypeDef = TypedDict(
-    "DescribeDBInstancesMessageRequestTypeDef",
+DescribeDBParameterGroupsMessageRequestTypeDef = TypedDict(
+    "DescribeDBParameterGroupsMessageRequestTypeDef",
     {
-        "DBInstanceIdentifier": str,
+        "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
+_RequiredDescribeDBParametersMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeDBParametersMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
+    },
+)
+_OptionalDescribeDBParametersMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeDBParametersMessageRequestTypeDef",
+    {
+        "Source": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-DescribeDBParameterGroupsMessageRequestTypeDef = TypedDict(
-    "DescribeDBParameterGroupsMessageRequestTypeDef",
+
+class DescribeDBParametersMessageRequestTypeDef(
+    _RequiredDescribeDBParametersMessageRequestTypeDef,
+    _OptionalDescribeDBParametersMessageRequestTypeDef,
+):
+    pass
+
+
+DescribeDBSubnetGroupsMessageRequestTypeDef = TypedDict(
+    "DescribeDBSubnetGroupsMessageRequestTypeDef",
     {
-        "DBParameterGroupName": str,
+        "DBSubnetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
+_RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef",
     {
-        "DBParameterGroupName": str,
+        "DBParameterGroupFamily": str,
     },
 )
-_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
+_OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef",
     {
-        "Source": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
 
-class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(
-    _RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
-    _OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
+class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(
+    _RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
+    _OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeDBParametersMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeDBParametersMessageRequestTypeDef",
+_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
-        "DBParameterGroupName": str,
+        "DBParameterGroupFamily": str,
     },
 )
-_OptionalDescribeDBParametersMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeDBParametersMessageRequestTypeDef",
+_OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
-        "Source": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
 
-class DescribeDBParametersMessageRequestTypeDef(
-    _RequiredDescribeDBParametersMessageRequestTypeDef,
-    _OptionalDescribeDBParametersMessageRequestTypeDef,
+class DescribeEngineDefaultParametersMessageRequestTypeDef(
+    _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
+    _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
 
-DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
+DescribeEventCategoriesMessageRequestTypeDef = TypedDict(
+    "DescribeEventCategoriesMessageRequestTypeDef",
     {
-        "DBSubnetGroupName": str,
+        "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeDBSubnetGroupsMessageRequestTypeDef = TypedDict(
-    "DescribeDBSubnetGroupsMessageRequestTypeDef",
+DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
-        "DBSubnetGroupName": str,
+        "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef",
+_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     {
-        "DBParameterGroupFamily": str,
+        "Engine": str,
     },
 )
-_OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef",
+_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     {
+        "EngineVersion": str,
+        "DBInstanceClass": str,
+        "LicenseModel": str,
+        "Vpc": bool,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
 
-class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(
-    _RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
-    _OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
+class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
+    _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
+    _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
+    "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     {
-        "DBParameterGroupFamily": str,
+        "ResourceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "Marker": str,
+        "MaxRecords": int,
     },
+    total=False,
 )
-_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+
+_RequiredListTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_RequiredListTagsForResourceMessageRequestTypeDef",
+    {
+        "ResourceName": str,
+    },
+)
+_OptionalListTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_OptionalListTagsForResourceMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 
-class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
-    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+class ListTagsForResourceMessageRequestTypeDef(
+    _RequiredListTagsForResourceMessageRequestTypeDef,
+    _OptionalListTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
+DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     {
-        "DBParameterGroupFamily": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultParametersMessageRequestTypeDef",
+
+DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     {
+        "DBClusterParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class DescribeEngineDefaultParametersMessageRequestTypeDef(
-    _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
-    _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
+class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
+    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
 ):
     pass
 
 
-DescribeEventCategoriesMessageRequestTypeDef = TypedDict(
-    "DescribeEventCategoriesMessageRequestTypeDef",
+DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     {
-        "SourceType": str,
+        "DBClusterIdentifier": str,
+        "DBClusterSnapshotIdentifier": str,
+        "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
+        "IncludeShared": bool,
+        "IncludePublic": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
     {
-        "SubscriptionName": str,
+        "DBClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageRequestTypeDef",
+DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     {
-        "SubscriptionName": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "DBParameterGroupFamily": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "DefaultOnly": bool,
+        "ListSupportedCharacterSets": bool,
+        "ListSupportedTimezones": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
+        "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
+DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
+        "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     {
-        "Engine": str,
+        "DBParameterGroupName": str,
     },
 )
-_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     {
-        "EngineVersion": str,
-        "DBInstanceClass": str,
-        "LicenseModel": str,
-        "Vpc": bool,
+        "Source": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
-    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
-    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(
+    _RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
+    _OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
 ):
     pass
 
 
-_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
+DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     {
-        "Engine": str,
+        "DBSubnetGroupName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
+
+_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "DBParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     {
-        "EngineVersion": str,
-        "DBInstanceClass": str,
-        "LicenseModel": str,
-        "Vpc": bool,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
-    _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
+class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
+    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
 ):
     pass
 
 
-DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
-    TypedDict(
-        "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
-        {
-            "ResourceIdentifier": str,
-            "Filters": Sequence[FilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
-DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
-    "DescribePendingMaintenanceActionsMessageRequestTypeDef",
+DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
+    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     {
-        "ResourceIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "Marker": str,
-        "MaxRecords": int,
+        "GlobalClusterIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceMessageRequestTypeDef = TypedDict(
-    "_RequiredListTagsForResourceMessageRequestTypeDef",
+_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     {
-        "ResourceName": str,
+        "Engine": str,
     },
 )
-_OptionalListTagsForResourceMessageRequestTypeDef = TypedDict(
-    "_OptionalListTagsForResourceMessageRequestTypeDef",
+_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     {
+        "EngineVersion": str,
+        "DBInstanceClass": str,
+        "LicenseModel": str,
+        "Vpc": bool,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListTagsForResourceMessageRequestTypeDef(
-    _RequiredListTagsForResourceMessageRequestTypeDef,
-    _OptionalListTagsForResourceMessageRequestTypeDef,
+class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
+    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
 ):
     pass
 
 
+DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
+    TypedDict(
+        "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
+        {
+            "ResourceIdentifier": str,
+            "Filters": Sequence[FilterTypeDef],
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
 DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef = TypedDict(
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     {
         "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -2496,28 +2431,95 @@
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
+    "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "SourceDBClusterIdentifier": str,
+    },
+)
+_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
+    "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
+    {
+        "RestoreType": str,
+        "RestoreToTime": TimestampTypeDef,
+        "UseLatestRestorableTime": bool,
+        "Port": int,
+        "DBSubnetGroupName": str,
+        "OptionGroupName": str,
+        "VpcSecurityGroupIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "EnableIAMDatabaseAuthentication": bool,
+        "EnableCloudwatchLogsExports": Sequence[str],
+        "DBClusterParameterGroupName": str,
+        "DeletionProtection": bool,
+        "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
+    _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
+    _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
+):
+    pass
+
+
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventsMessageTypeDef = TypedDict(
     "EventsMessageTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalClusterTypeDef = TypedDict(
     "GlobalClusterTypeDef",
     {
         "GlobalClusterIdentifier": str,
@@ -2554,15 +2556,15 @@
 )
 
 OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
     "OrderableDBInstanceOptionsMessageTypeDef",
     {
         "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBSubnetGroupTypeDef = TypedDict(
     "DBSubnetGroupTypeDef",
     {
         "DBSubnetGroupName": str,
@@ -2625,114 +2627,114 @@
     total=False,
 )
 
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEngineDefaultParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBClusterSnapshotAttributeResultTypeDef = TypedDict(
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBEngineVersionMessageTypeDef = TypedDict(
     "DBEngineVersionMessageTypeDef",
     {
         "Marker": str,
         "DBEngineVersions": List[DBEngineVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGlobalClusterResultTypeDef = TypedDict(
     "CreateGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGlobalClusterResultTypeDef = TypedDict(
     "DeleteGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverGlobalClusterResultTypeDef = TypedDict(
     "FailoverGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalClustersMessageTypeDef = TypedDict(
     "GlobalClustersMessageTypeDef",
     {
         "Marker": str,
         "GlobalClusters": List[GlobalClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyGlobalClusterResultTypeDef = TypedDict(
     "ModifyGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveFromGlobalClusterResultTypeDef = TypedDict(
     "RemoveFromGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PendingMaintenanceActionsMessageTypeDef = TypedDict(
     "PendingMaintenanceActionsMessageTypeDef",
     {
         "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidDBInstanceModificationsMessageTypeDef = TypedDict(
     "ValidDBInstanceModificationsMessageTypeDef",
     {
         "Storage": List[ValidStorageOptionsTypeDef],
@@ -2740,15 +2742,15 @@
     total=False,
 )
 
 CreateDBSubnetGroupResultTypeDef = TypedDict(
     "CreateDBSubnetGroupResultTypeDef",
     {
         "DBSubnetGroup": DBSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBInstanceTypeDef = TypedDict(
     "DBInstanceTypeDef",
     {
         "DBInstanceIdentifier": str,
@@ -2809,148 +2811,148 @@
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "DBSubnetGroups": List[DBSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBSubnetGroupResultTypeDef = TypedDict(
     "ModifyDBSubnetGroupResultTypeDef",
     {
         "DBSubnetGroup": DBSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterResultTypeDef = TypedDict(
     "CreateDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterMessageTypeDef = TypedDict(
     "DBClusterMessageTypeDef",
     {
         "Marker": str,
         "DBClusters": List[DBClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBClusterResultTypeDef = TypedDict(
     "DeleteDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverDBClusterResultTypeDef = TypedDict(
     "FailoverDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBClusterResultTypeDef = TypedDict(
     "ModifyDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PromoteReadReplicaDBClusterResultTypeDef = TypedDict(
     "PromoteReadReplicaDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreDBClusterFromSnapshotResultTypeDef = TypedDict(
     "RestoreDBClusterFromSnapshotResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreDBClusterToPointInTimeResultTypeDef = TypedDict(
     "RestoreDBClusterToPointInTimeResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDBClusterResultTypeDef = TypedDict(
     "StartDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopDBClusterResultTypeDef = TypedDict(
     "StopDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeValidDBInstanceModificationsResultTypeDef = TypedDict(
     "DescribeValidDBInstanceModificationsResultTypeDef",
     {
         "ValidDBInstanceModificationsMessage": ValidDBInstanceModificationsMessageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBInstanceResultTypeDef = TypedDict(
     "CreateDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBInstanceMessageTypeDef = TypedDict(
     "DBInstanceMessageTypeDef",
     {
         "Marker": str,
         "DBInstances": List[DBInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBInstanceResultTypeDef = TypedDict(
     "DeleteDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBInstanceResultTypeDef = TypedDict(
     "ModifyDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootDBInstanceResultTypeDef = TypedDict(
     "RebootDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/type_defs.pyi` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_neptune.type_defs import AddRoleToDBClusterMessageRequestTypeDef
 
-    data: AddRoleToDBClusterMessageRequestTypeDef = {...}
+    data: AddRoleToDBClusterMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplyMethodType, SourceTypeType
@@ -22,89 +22,89 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddRoleToDBClusterMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "CharacterSetTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
     "DBClusterParameterGroupTypeDef",
     "DBClusterSnapshotTypeDef",
     "DBParameterGroupTypeDef",
-    "CreateDBClusterEndpointOutputTypeDef",
     "ServerlessV2ScalingConfigurationTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterEndpointTypeDef",
     "DBClusterMemberTypeDef",
     "DBClusterOptionGroupStatusTypeDef",
     "ParameterTypeDef",
-    "DBClusterParameterGroupNameMessageTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "ServerlessV2ScalingConfigurationInfoTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "TimezoneTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "DBParameterGroupStatusTypeDef",
     "DBSecurityGroupMembershipTypeDef",
     "DomainMembershipTypeDef",
     "EndpointTypeDef",
     "OptionGroupMembershipTypeDef",
-    "DBParameterGroupNameMessageTypeDef",
     "DeleteDBClusterEndpointMessageRequestTypeDef",
-    "DeleteDBClusterEndpointOutputTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     "DeleteDBClusterSnapshotMessageRequestTypeDef",
     "DeleteDBInstanceMessageRequestTypeDef",
     "DeleteDBParameterGroupMessageRequestTypeDef",
     "DeleteDBSubnetGroupMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteGlobalClusterMessageRequestTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    "TimestampTypeDef",
     "DescribeGlobalClustersMessageRequestTypeDef",
     "DescribeValidDBInstanceModificationsMessageRequestTypeDef",
     "DoubleRangeTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "FailoverGlobalClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
     "ModifyDBClusterEndpointMessageRequestTypeDef",
-    "ModifyDBClusterEndpointOutputTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PromoteReadReplicaDBClusterMessageRequestTypeDef",
     "RangeTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveRoleFromDBClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
+    "CreateDBClusterEndpointOutputTypeDef",
     "CreateEventSubscriptionResultTypeDef",
+    "DBClusterParameterGroupNameMessageTypeDef",
+    "DBParameterGroupNameMessageTypeDef",
+    "DeleteDBClusterEndpointOutputTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
+    "ModifyDBClusterEndpointOutputTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopyDBClusterParameterGroupMessageRequestTypeDef",
     "CopyDBClusterSnapshotMessageRequestTypeDef",
     "CopyDBParameterGroupMessageRequestTypeDef",
     "CreateDBClusterEndpointMessageRequestTypeDef",
@@ -129,60 +129,61 @@
     "DeleteDBClusterSnapshotResultTypeDef",
     "CopyDBParameterGroupResultTypeDef",
     "CreateDBParameterGroupResultTypeDef",
     "DBParameterGroupsMessageTypeDef",
     "CreateDBClusterMessageRequestTypeDef",
     "ModifyDBClusterMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
-    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "DBClusterEndpointMessageTypeDef",
     "DBClusterParameterGroupDetailsTypeDef",
     "DBParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "ModifyDBClusterParameterGroupMessageRequestTypeDef",
     "ModifyDBParameterGroupMessageRequestTypeDef",
     "ResetDBClusterParameterGroupMessageRequestTypeDef",
     "ResetDBParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBEngineVersionTypeDef",
-    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
-    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
-    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     "DescribeDBClusterParametersMessageRequestTypeDef",
-    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
-    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
     "DescribeDBClustersMessageRequestTypeDef",
-    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     "DescribeDBEngineVersionsMessageRequestTypeDef",
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     "DescribeDBInstancesMessageRequestTypeDef",
-    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     "DescribeDBParameterGroupsMessageRequestTypeDef",
-    "DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     "DescribeDBParametersMessageRequestTypeDef",
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultClusterParametersMessageRequestTypeDef",
-    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
-    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
-    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
+    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
+    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
+    "DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
+    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
+    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "EventCategoriesMessageTypeDef",
     "EventsMessageTypeDef",
     "GlobalClusterTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "ValidStorageOptionsTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
@@ -265,14 +266,25 @@
         "EventCategoriesList": List[str],
         "Enabled": bool,
         "EventSubscriptionArn": str,
     },
     total=False,
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -367,31 +379,14 @@
         "DBParameterGroupFamily": str,
         "Description": str,
         "DBParameterGroupArn": str,
     },
     total=False,
 )
 
-CreateDBClusterEndpointOutputTypeDef = TypedDict(
-    "CreateDBClusterEndpointOutputTypeDef",
-    {
-        "DBClusterEndpointIdentifier": str,
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointResourceIdentifier": str,
-        "Endpoint": str,
-        "Status": str,
-        "EndpointType": str,
-        "CustomEndpointType": str,
-        "StaticMembers": List[str],
-        "ExcludedMembers": List[str],
-        "DBClusterEndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ServerlessV2ScalingConfigurationTypeDef = TypedDict(
     "ServerlessV2ScalingConfigurationTypeDef",
     {
         "MinCapacity": float,
         "MaxCapacity": float,
     },
     total=False,
@@ -471,22 +466,14 @@
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ApplyMethod": ApplyMethodType,
     },
     total=False,
 )
 
-DBClusterParameterGroupNameMessageTypeDef = TypedDict(
-    "DBClusterParameterGroupNameMessageTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DBClusterRoleTypeDef = TypedDict(
     "DBClusterRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
         "FeatureName": str,
     },
@@ -596,46 +583,21 @@
     {
         "OptionGroupName": str,
         "Status": str,
     },
     total=False,
 )
 
-DBParameterGroupNameMessageTypeDef = TypedDict(
-    "DBParameterGroupNameMessageTypeDef",
-    {
-        "DBParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDBClusterEndpointMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterEndpointMessageRequestTypeDef",
     {
         "DBClusterEndpointIdentifier": str,
     },
 )
 
-DeleteDBClusterEndpointOutputTypeDef = TypedDict(
-    "DeleteDBClusterEndpointOutputTypeDef",
-    {
-        "DBClusterEndpointIdentifier": str,
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointResourceIdentifier": str,
-        "Endpoint": str,
-        "Status": str,
-        "EndpointType": str,
-        "CustomEndpointType": str,
-        "StaticMembers": List[str],
-        "ExcludedMembers": List[str],
-        "DBClusterEndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 _OptionalDeleteDBClusterMessageRequestTypeDef = TypedDict(
@@ -718,14 +680,24 @@
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 DescribeDBClusterSnapshotAttributesMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
     },
 )
 
@@ -734,23 +706,15 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
-    {
-        "GlobalClusterIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
     "DescribeGlobalClustersMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -769,21 +733,14 @@
     {
         "From": float,
         "To": float,
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
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
     total=False,
@@ -847,31 +804,14 @@
 
 class ModifyDBClusterEndpointMessageRequestTypeDef(
     _RequiredModifyDBClusterEndpointMessageRequestTypeDef,
     _OptionalModifyDBClusterEndpointMessageRequestTypeDef,
 ):
     pass
 
-ModifyDBClusterEndpointOutputTypeDef = TypedDict(
-    "ModifyDBClusterEndpointOutputTypeDef",
-    {
-        "DBClusterEndpointIdentifier": str,
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointResourceIdentifier": str,
-        "Endpoint": str,
-        "Status": str,
-        "EndpointType": str,
-        "CustomEndpointType": str,
-        "StaticMembers": List[str],
-        "ExcludedMembers": List[str],
-        "DBClusterEndpointArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "AttributeName": str,
     },
 )
@@ -953,24 +893,14 @@
 
 class ModifyGlobalClusterMessageRequestTypeDef(
     _RequiredModifyGlobalClusterMessageRequestTypeDef,
     _OptionalModifyGlobalClusterMessageRequestTypeDef,
 ):
     pass
 
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
@@ -1057,25 +987,14 @@
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceName": str,
         "TagKeys": Sequence[str],
     },
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
 StartDBClusterMessageRequestTypeDef = TypedDict(
     "StartDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
     },
 )
 
@@ -1086,56 +1005,130 @@
     },
 )
 
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDBClusterEndpointOutputTypeDef = TypedDict(
+    "CreateDBClusterEndpointOutputTypeDef",
+    {
+        "DBClusterEndpointIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointResourceIdentifier": str,
+        "Endpoint": str,
+        "Status": str,
+        "EndpointType": str,
+        "CustomEndpointType": str,
+        "StaticMembers": List[str],
+        "ExcludedMembers": List[str],
+        "DBClusterEndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEventSubscriptionResultTypeDef = TypedDict(
     "CreateEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DBClusterParameterGroupNameMessageTypeDef = TypedDict(
+    "DBClusterParameterGroupNameMessageTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DBParameterGroupNameMessageTypeDef = TypedDict(
+    "DBParameterGroupNameMessageTypeDef",
+    {
+        "DBParameterGroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDBClusterEndpointOutputTypeDef = TypedDict(
+    "DeleteDBClusterEndpointOutputTypeDef",
+    {
+        "DBClusterEndpointIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointResourceIdentifier": str,
+        "Endpoint": str,
+        "Status": str,
+        "EndpointType": str,
+        "CustomEndpointType": str,
+        "StaticMembers": List[str],
+        "ExcludedMembers": List[str],
+        "DBClusterEndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventSubscriptionResultTypeDef = TypedDict(
     "DeleteEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventSubscriptionsMessageTypeDef = TypedDict(
     "EventSubscriptionsMessageTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyDBClusterEndpointOutputTypeDef = TypedDict(
+    "ModifyDBClusterEndpointOutputTypeDef",
+    {
+        "DBClusterEndpointIdentifier": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointResourceIdentifier": str,
+        "Endpoint": str,
+        "Status": str,
+        "EndpointType": str,
+        "CustomEndpointType": str,
+        "StaticMembers": List[str],
+        "ExcludedMembers": List[str],
+        "DBClusterEndpointArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyEventSubscriptionResultTypeDef = TypedDict(
     "ModifyEventSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveSourceIdentifierFromSubscriptionResultTypeDef = TypedDict(
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
     {
         "ResourceName": str,
@@ -1408,15 +1401,15 @@
 ):
     pass
 
 TagListMessageTypeDef = TypedDict(
     "TagListMessageTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OrderableDBInstanceOptionTypeDef = TypedDict(
     "OrderableDBInstanceOptionTypeDef",
     {
         "Engine": str,
@@ -1543,90 +1536,90 @@
     total=False,
 )
 
 CopyDBClusterParameterGroupResultTypeDef = TypedDict(
     "CopyDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterParameterGroupResultTypeDef = TypedDict(
     "CreateDBClusterParameterGroupResultTypeDef",
     {
         "DBClusterParameterGroup": DBClusterParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupsMessageTypeDef = TypedDict(
     "DBClusterParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "DBClusterParameterGroups": List[DBClusterParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDBClusterSnapshotResultTypeDef = TypedDict(
     "CopyDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterSnapshotResultTypeDef = TypedDict(
     "CreateDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterSnapshotMessageTypeDef = TypedDict(
     "DBClusterSnapshotMessageTypeDef",
     {
         "Marker": str,
         "DBClusterSnapshots": List[DBClusterSnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBClusterSnapshotResultTypeDef = TypedDict(
     "DeleteDBClusterSnapshotResultTypeDef",
     {
         "DBClusterSnapshot": DBClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyDBParameterGroupResultTypeDef = TypedDict(
     "CopyDBParameterGroupResultTypeDef",
     {
         "DBParameterGroup": DBParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBParameterGroupResultTypeDef = TypedDict(
     "CreateDBParameterGroupResultTypeDef",
     {
         "DBParameterGroup": DBParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBParameterGroupsMessageTypeDef = TypedDict(
     "DBParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "DBParameterGroups": List[DBParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
@@ -1739,72 +1732,38 @@
 
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBClusterFromSnapshotMessageRequestTypeDef,
 ):
     pass
 
-_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
-    "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "SourceDBClusterIdentifier": str,
-    },
-)
-_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
-    "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
-    {
-        "RestoreType": str,
-        "RestoreToTime": Union[datetime, str],
-        "UseLatestRestorableTime": bool,
-        "Port": int,
-        "DBSubnetGroupName": str,
-        "OptionGroupName": str,
-        "VpcSecurityGroupIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "EnableIAMDatabaseAuthentication": bool,
-        "EnableCloudwatchLogsExports": Sequence[str],
-        "DBClusterParameterGroupName": str,
-        "DeletionProtection": bool,
-        "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
-    _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
-    _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
-):
-    pass
-
 DBClusterEndpointMessageTypeDef = TypedDict(
     "DBClusterEndpointMessageTypeDef",
     {
         "Marker": str,
         "DBClusterEndpoints": List[DBClusterEndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBParameterGroupDetailsTypeDef = TypedDict(
     "DBParameterGroupDetailsTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "DBParameterGroupFamily": str,
@@ -1897,80 +1856,37 @@
         "SupportsLogExportsToCloudwatchLogs": bool,
         "SupportsReadReplica": bool,
         "SupportsGlobalDatabases": bool,
     },
     total=False,
 )
 
-DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "DBClusterEndpointIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterEndpointsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterEndpointIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterParameterGroupsMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
-    {
-        "DBClusterParameterGroupName": str,
-    },
-)
-_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
-    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
-    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeDBClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDBClusterParametersMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
     },
 )
 _OptionalDescribeDBClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1986,28 +1902,14 @@
 
 class DescribeDBClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDBClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDBClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "DBClusterSnapshotIdentifier": str,
-        "SnapshotType": str,
-        "Filters": Sequence[FilterTypeDef],
-        "IncludeShared": bool,
-        "IncludePublic": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
@@ -2015,50 +1917,25 @@
         "Marker": str,
         "IncludeShared": bool,
         "IncludePublic": bool,
     },
     total=False,
 )
 
-DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
-    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
-    {
-        "DBClusterIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBClustersMessageRequestTypeDef = TypedDict(
     "DescribeDBClustersMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
-    {
-        "Engine": str,
-        "EngineVersion": str,
-        "DBParameterGroupFamily": str,
-        "Filters": Sequence[FilterTypeDef],
-        "DefaultOnly": bool,
-        "ListSupportedCharacterSets": bool,
-        "ListSupportedTimezones": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBEngineVersionsMessageRequestTypeDef = TypedDict(
     "DescribeDBEngineVersionsMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "DBParameterGroupFamily": str,
         "Filters": Sequence[FilterTypeDef],
@@ -2067,380 +1944,505 @@
         "DefaultOnly": bool,
         "ListSupportedCharacterSets": bool,
         "ListSupportedTimezones": bool,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+DescribeDBInstancesMessageRequestTypeDef = TypedDict(
+    "DescribeDBInstancesMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageRequestTypeDef = TypedDict(
-    "DescribeDBInstancesMessageRequestTypeDef",
+DescribeDBParameterGroupsMessageRequestTypeDef = TypedDict(
+    "DescribeDBParameterGroupsMessageRequestTypeDef",
     {
-        "DBInstanceIdentifier": str,
+        "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
+_RequiredDescribeDBParametersMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeDBParametersMessageRequestTypeDef",
     {
         "DBParameterGroupName": str,
+    },
+)
+_OptionalDescribeDBParametersMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeDBParametersMessageRequestTypeDef",
+    {
+        "Source": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-DescribeDBParameterGroupsMessageRequestTypeDef = TypedDict(
-    "DescribeDBParameterGroupsMessageRequestTypeDef",
+class DescribeDBParametersMessageRequestTypeDef(
+    _RequiredDescribeDBParametersMessageRequestTypeDef,
+    _OptionalDescribeDBParametersMessageRequestTypeDef,
+):
+    pass
+
+DescribeDBSubnetGroupsMessageRequestTypeDef = TypedDict(
+    "DescribeDBSubnetGroupsMessageRequestTypeDef",
     {
-        "DBParameterGroupName": str,
+        "DBSubnetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
+_RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef",
     {
-        "DBParameterGroupName": str,
+        "DBParameterGroupFamily": str,
     },
 )
-_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
+_OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef",
     {
-        "Source": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(
-    _RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
-    _OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
+class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(
+    _RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
+    _OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeDBParametersMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeDBParametersMessageRequestTypeDef",
+_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
-        "DBParameterGroupName": str,
+        "DBParameterGroupFamily": str,
     },
 )
-_OptionalDescribeDBParametersMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeDBParametersMessageRequestTypeDef",
+_OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
-        "Source": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-class DescribeDBParametersMessageRequestTypeDef(
-    _RequiredDescribeDBParametersMessageRequestTypeDef,
-    _OptionalDescribeDBParametersMessageRequestTypeDef,
+class DescribeEngineDefaultParametersMessageRequestTypeDef(
+    _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
+    _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
+DescribeEventCategoriesMessageRequestTypeDef = TypedDict(
+    "DescribeEventCategoriesMessageRequestTypeDef",
     {
-        "DBSubnetGroupName": str,
+        "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeDBSubnetGroupsMessageRequestTypeDef = TypedDict(
-    "DescribeDBSubnetGroupsMessageRequestTypeDef",
+DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
-        "DBSubnetGroupName": str,
+        "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef",
+_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     {
-        "DBParameterGroupFamily": str,
+        "Engine": str,
     },
 )
-_OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef",
+_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     {
+        "EngineVersion": str,
+        "DBInstanceClass": str,
+        "LicenseModel": str,
+        "Vpc": bool,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(
-    _RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
-    _OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
+class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
+    _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
+    _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
+    "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     {
-        "DBParameterGroupFamily": str,
+        "ResourceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "Marker": str,
+        "MaxRecords": int,
     },
+    total=False,
 )
-_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+
+_RequiredListTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_RequiredListTagsForResourceMessageRequestTypeDef",
+    {
+        "ResourceName": str,
+    },
+)
+_OptionalListTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_OptionalListTagsForResourceMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
-    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+class ListTagsForResourceMessageRequestTypeDef(
+    _RequiredListTagsForResourceMessageRequestTypeDef,
+    _OptionalListTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
+DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef",
     {
-        "DBParameterGroupFamily": str,
+        "DBClusterIdentifier": str,
+        "DBClusterEndpointIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultParametersMessageRequestTypeDef",
+
+DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     {
+        "DBClusterParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class DescribeEngineDefaultParametersMessageRequestTypeDef(
-    _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
-    _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
+_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    {
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
+    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
 ):
     pass
 
-DescribeEventCategoriesMessageRequestTypeDef = TypedDict(
-    "DescribeEventCategoriesMessageRequestTypeDef",
+DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
     {
-        "SourceType": str,
+        "DBClusterIdentifier": str,
+        "DBClusterSnapshotIdentifier": str,
+        "SnapshotType": str,
         "Filters": Sequence[FilterTypeDef],
+        "IncludeShared": bool,
+        "IncludePublic": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
     {
-        "SubscriptionName": str,
+        "DBClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageRequestTypeDef",
+DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     {
-        "SubscriptionName": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "DBParameterGroupFamily": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "DefaultOnly": bool,
+        "ListSupportedCharacterSets": bool,
+        "ListSupportedTimezones": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
     {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
+        "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
+DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef",
     {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
+        "DBParameterGroupName": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     {
-        "Engine": str,
+        "DBParameterGroupName": str,
     },
 )
-_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef",
     {
-        "EngineVersion": str,
-        "DBInstanceClass": str,
-        "LicenseModel": str,
-        "Vpc": bool,
+        "Source": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
-    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
-    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+class DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef(
+    _RequiredDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
+    _OptionalDescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
 ):
     pass
 
-_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
+DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
+    {
+        "DBSubnetGroupName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "DBParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
+    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+):
+    pass
+
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
+    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+    {
+        "GlobalClusterIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     {
         "Engine": str,
     },
 )
-_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
+_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     {
         "EngineVersion": str,
         "DBInstanceClass": str,
         "LicenseModel": str,
         "Vpc": bool,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
-    _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
+class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
+    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
 ):
     pass
 
 DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef = (
     TypedDict(
         "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
         {
             "ResourceIdentifier": str,
             "Filters": Sequence[FilterTypeDef],
-            "PaginationConfig": "PaginatorConfigTypeDef",
+            "PaginationConfig": PaginatorConfigTypeDef,
         },
         total=False,
     )
 )
 
-DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
-    "DescribePendingMaintenanceActionsMessageRequestTypeDef",
+DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     {
-        "ResourceIdentifier": str,
+        "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "Marker": str,
         "MaxRecords": int,
+        "Marker": str,
+        "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceMessageRequestTypeDef = TypedDict(
-    "_RequiredListTagsForResourceMessageRequestTypeDef",
+DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
     {
-        "ResourceName": str,
+        "DBInstanceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "MaxRecords": int,
+        "Marker": str,
+        "WaiterConfig": WaiterConfigTypeDef,
     },
+    total=False,
 )
-_OptionalListTagsForResourceMessageRequestTypeDef = TypedDict(
-    "_OptionalListTagsForResourceMessageRequestTypeDef",
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "EventCategories": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListTagsForResourceMessageRequestTypeDef(
-    _RequiredListTagsForResourceMessageRequestTypeDef,
-    _OptionalListTagsForResourceMessageRequestTypeDef,
-):
-    pass
-
-DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
     {
-        "DBInstanceIdentifier": str,
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "EventCategories": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
-        "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef",
+_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
+    "_RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef",
     {
-        "DBInstanceIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-        "WaiterConfig": WaiterConfigTypeDef,
+        "DBClusterIdentifier": str,
+        "SourceDBClusterIdentifier": str,
+    },
+)
+_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef = TypedDict(
+    "_OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef",
+    {
+        "RestoreType": str,
+        "RestoreToTime": TimestampTypeDef,
+        "UseLatestRestorableTime": bool,
+        "Port": int,
+        "DBSubnetGroupName": str,
+        "OptionGroupName": str,
+        "VpcSecurityGroupIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "EnableIAMDatabaseAuthentication": bool,
+        "EnableCloudwatchLogsExports": Sequence[str],
+        "DBClusterParameterGroupName": str,
+        "DeletionProtection": bool,
+        "ServerlessV2ScalingConfiguration": ServerlessV2ScalingConfigurationTypeDef,
     },
     total=False,
 )
 
+class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
+    _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
+    _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
+):
+    pass
+
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventsMessageTypeDef = TypedDict(
     "EventsMessageTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalClusterTypeDef = TypedDict(
     "GlobalClusterTypeDef",
     {
         "GlobalClusterIdentifier": str,
@@ -2477,15 +2479,15 @@
 )
 
 OrderableDBInstanceOptionsMessageTypeDef = TypedDict(
     "OrderableDBInstanceOptionsMessageTypeDef",
     {
         "OrderableDBInstanceOptions": List[OrderableDBInstanceOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBSubnetGroupTypeDef = TypedDict(
     "DBSubnetGroupTypeDef",
     {
         "DBSubnetGroupName": str,
@@ -2548,114 +2550,114 @@
     total=False,
 )
 
 DescribeEngineDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultClusterParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEngineDefaultParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DescribeDBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBClusterSnapshotAttributeResultTypeDef = TypedDict(
     "ModifyDBClusterSnapshotAttributeResultTypeDef",
     {
         "DBClusterSnapshotAttributesResult": DBClusterSnapshotAttributesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBEngineVersionMessageTypeDef = TypedDict(
     "DBEngineVersionMessageTypeDef",
     {
         "Marker": str,
         "DBEngineVersions": List[DBEngineVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGlobalClusterResultTypeDef = TypedDict(
     "CreateGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGlobalClusterResultTypeDef = TypedDict(
     "DeleteGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverGlobalClusterResultTypeDef = TypedDict(
     "FailoverGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlobalClustersMessageTypeDef = TypedDict(
     "GlobalClustersMessageTypeDef",
     {
         "Marker": str,
         "GlobalClusters": List[GlobalClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyGlobalClusterResultTypeDef = TypedDict(
     "ModifyGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveFromGlobalClusterResultTypeDef = TypedDict(
     "RemoveFromGlobalClusterResultTypeDef",
     {
         "GlobalCluster": GlobalClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplyPendingMaintenanceActionResultTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResultTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PendingMaintenanceActionsMessageTypeDef = TypedDict(
     "PendingMaintenanceActionsMessageTypeDef",
     {
         "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidDBInstanceModificationsMessageTypeDef = TypedDict(
     "ValidDBInstanceModificationsMessageTypeDef",
     {
         "Storage": List[ValidStorageOptionsTypeDef],
@@ -2663,15 +2665,15 @@
     total=False,
 )
 
 CreateDBSubnetGroupResultTypeDef = TypedDict(
     "CreateDBSubnetGroupResultTypeDef",
     {
         "DBSubnetGroup": DBSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBInstanceTypeDef = TypedDict(
     "DBInstanceTypeDef",
     {
         "DBInstanceIdentifier": str,
@@ -2732,148 +2734,148 @@
 )
 
 DBSubnetGroupMessageTypeDef = TypedDict(
     "DBSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "DBSubnetGroups": List[DBSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBSubnetGroupResultTypeDef = TypedDict(
     "ModifyDBSubnetGroupResultTypeDef",
     {
         "DBSubnetGroup": DBSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBClusterResultTypeDef = TypedDict(
     "CreateDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBClusterMessageTypeDef = TypedDict(
     "DBClusterMessageTypeDef",
     {
         "Marker": str,
         "DBClusters": List[DBClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBClusterResultTypeDef = TypedDict(
     "DeleteDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverDBClusterResultTypeDef = TypedDict(
     "FailoverDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBClusterResultTypeDef = TypedDict(
     "ModifyDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PromoteReadReplicaDBClusterResultTypeDef = TypedDict(
     "PromoteReadReplicaDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreDBClusterFromSnapshotResultTypeDef = TypedDict(
     "RestoreDBClusterFromSnapshotResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreDBClusterToPointInTimeResultTypeDef = TypedDict(
     "RestoreDBClusterToPointInTimeResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDBClusterResultTypeDef = TypedDict(
     "StartDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopDBClusterResultTypeDef = TypedDict(
     "StopDBClusterResultTypeDef",
     {
         "DBCluster": DBClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeValidDBInstanceModificationsResultTypeDef = TypedDict(
     "DescribeValidDBInstanceModificationsResultTypeDef",
     {
         "ValidDBInstanceModificationsMessage": ValidDBInstanceModificationsMessageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDBInstanceResultTypeDef = TypedDict(
     "CreateDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DBInstanceMessageTypeDef = TypedDict(
     "DBInstanceMessageTypeDef",
     {
         "Marker": str,
         "DBInstances": List[DBInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDBInstanceResultTypeDef = TypedDict(
     "DeleteDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyDBInstanceResultTypeDef = TypedDict(
     "ModifyDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootDBInstanceResultTypeDef = TypedDict(
     "RebootDBInstanceResultTypeDef",
     {
         "DBInstance": DBInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/waiter.py` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune/waiter.pyi` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune.egg-info/PKG-INFO` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-neptune
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Neptune 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Neptune 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore neptune type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore neptune type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-neptune"></a>
 
 # types-aiobotocore-neptune
 
 [![PyPI - types-aiobotocore-neptune](https://img.shields.io/pypi/v/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-neptune.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptune)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-neptune?color=blue)](https://pypistats.org/packages/types-aiobotocore-neptune)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-neptune)](https://pepy.tech/project/types-aiobotocore-neptune)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Neptune 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune)
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
 [types-aiobotocore-neptune docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -412,101 +411,101 @@
 )
 
 
 def check_value(value: ApplyMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_neptune.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_neptune.type_defs import (
     AddRoleToDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     CharacterSetTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     DBParameterGroupTypeDef,
-    CreateDBClusterEndpointOutputTypeDef,
     ServerlessV2ScalingConfigurationTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterEndpointTypeDef,
     DBClusterMemberTypeDef,
     DBClusterOptionGroupStatusTypeDef,
     ParameterTypeDef,
-    DBClusterParameterGroupNameMessageTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     ServerlessV2ScalingConfigurationInfoTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     TimezoneTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     DBParameterGroupStatusTypeDef,
     DBSecurityGroupMembershipTypeDef,
     DomainMembershipTypeDef,
     EndpointTypeDef,
     OptionGroupMembershipTypeDef,
-    DBParameterGroupNameMessageTypeDef,
     DeleteDBClusterEndpointMessageRequestTypeDef,
-    DeleteDBClusterEndpointOutputTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBParameterGroupMessageRequestTypeDef,
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
+    TimestampTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
     DescribeValidDBInstanceModificationsMessageRequestTypeDef,
     DoubleRangeTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     FailoverGlobalClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ModifyDBClusterEndpointMessageRequestTypeDef,
-    ModifyDBClusterEndpointOutputTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PromoteReadReplicaDBClusterMessageRequestTypeDef,
     RangeTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveRoleFromDBClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
+    CreateDBClusterEndpointOutputTypeDef,
     CreateEventSubscriptionResultTypeDef,
+    DBClusterParameterGroupNameMessageTypeDef,
+    DBParameterGroupNameMessageTypeDef,
+    DeleteDBClusterEndpointOutputTypeDef,
     DeleteEventSubscriptionResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
+    ModifyDBClusterEndpointOutputTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopyDBClusterParameterGroupMessageRequestTypeDef,
     CopyDBClusterSnapshotMessageRequestTypeDef,
     CopyDBParameterGroupMessageRequestTypeDef,
     CreateDBClusterEndpointMessageRequestTypeDef,
@@ -531,60 +530,61 @@
     DeleteDBClusterSnapshotResultTypeDef,
     CopyDBParameterGroupResultTypeDef,
     CreateDBParameterGroupResultTypeDef,
     DBParameterGroupsMessageTypeDef,
     CreateDBClusterMessageRequestTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
-    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     DBClusterEndpointMessageTypeDef,
     DBClusterParameterGroupDetailsTypeDef,
     DBParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     ModifyDBClusterParameterGroupMessageRequestTypeDef,
     ModifyDBParameterGroupMessageRequestTypeDef,
     ResetDBClusterParameterGroupMessageRequestTypeDef,
     ResetDBParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBEngineVersionTypeDef,
-    DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
     DescribeDBClusterEndpointsMessageRequestTypeDef,
-    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
     DescribeDBClusterParameterGroupsMessageRequestTypeDef,
-    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
     DescribeDBClusterParametersMessageRequestTypeDef,
-    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
     DescribeDBClusterSnapshotsMessageRequestTypeDef,
-    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
     DescribeDBClustersMessageRequestTypeDef,
-    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
     DescribeDBEngineVersionsMessageRequestTypeDef,
-    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
     DescribeDBInstancesMessageRequestTypeDef,
-    DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
     DescribeDBParameterGroupsMessageRequestTypeDef,
-    DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
     DescribeDBParametersMessageRequestTypeDef,
-    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    DescribeDBClusterEndpointsMessageDescribeDBClusterEndpointsPaginateTypeDef,
+    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
+    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
+    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
+    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
+    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
+    DescribeDBParameterGroupsMessageDescribeDBParameterGroupsPaginateTypeDef,
+    DescribeDBParametersMessageDescribeDBParametersPaginateTypeDef,
+    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
+    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef,
     DescribeDBInstancesMessageDBInstanceDeletedWaitTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     GlobalClusterTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     ValidStorageOptionsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
@@ -622,15 +622,15 @@
     DBInstanceMessageTypeDef,
     DeleteDBInstanceResultTypeDef,
     ModifyDBInstanceResultTypeDef,
     RebootDBInstanceResultTypeDef,
 )
 
 
-def get_structure() -> AddRoleToDBClusterMessageRequestTypeDef:
+def get_value() -> AddRoleToDBClusterMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-neptune-2.5.2/types_aiobotocore_neptune.egg-info/SOURCES.txt` & `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/SOURCES.txt`

 * *Files identical despite different names*


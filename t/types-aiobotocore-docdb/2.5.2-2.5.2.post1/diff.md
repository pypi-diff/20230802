# Comparing `tmp/types-aiobotocore-docdb-2.5.2.tar.gz` & `tmp/types-aiobotocore-docdb-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-docdb-2.5.2.tar", last modified: Sat Jul  8 01:43:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-docdb-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
```

## Comparing `types-aiobotocore-docdb-2.5.2.tar` & `types-aiobotocore-docdb-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.834041 types-aiobotocore-docdb-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:55.000000 types-aiobotocore-docdb-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23227 2023-07-08 01:43:32.834041 types-aiobotocore-docdb-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-07-08 01:28:55.000000 types-aiobotocore-docdb-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:32.834041 types-aiobotocore-docdb-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-08 01:28:55.000000 types-aiobotocore-docdb-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.830041 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-08 01:28:55.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-08 01:28:55.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-08 01:28:55.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53716 2023-07-08 01:28:57.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    53639 2023-07-08 01:28:56.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-07-08 01:28:57.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-07-08 01:28:57.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-07-08 01:28:57.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18105 2023-07-08 01:28:57.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:55.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    60571 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    60518 2023-07-08 01:28:58.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:55.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-08 01:28:57.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-08 01:28:57.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.834041 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23227 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 01:43:32.000000 types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.037601 types-aiobotocore-docdb-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23185 2023-08-02 14:52:12.037601 types-aiobotocore-docdb-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21675 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.037601 types-aiobotocore-docdb-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.029601 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53689 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53612 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60489 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60436 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:36.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-08-02 14:36:37.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.037601 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23185 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-docdb-2.5.2/LICENSE` & `types-aiobotocore-docdb-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2/PKG-INFO` & `types-aiobotocore-docdb-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DocDB 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DocDB 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore docdb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore docdb type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-docdb"></a>
 
 # types-aiobotocore-docdb
 
 [![PyPI - types-aiobotocore-docdb](https://img.shields.io/pypi/v/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-docdb?color=blue)](https://pypistats.org/packages/types-aiobotocore-docdb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb)](https://pepy.tech/project/types-aiobotocore-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DocDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
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
 [types-aiobotocore-docdb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/).
 
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
@@ -396,89 +395,89 @@
 )
 
 
 def check_value(value: ApplyMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_docdb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_docdb.type_defs import (
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     CertificateTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterMemberTypeDef,
     ParameterTypeDef,
-    DBClusterParameterGroupNameMessageTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     EndpointTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     PendingMaintenanceActionTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
+    DBClusterParameterGroupNameMessageTypeDef,
     DeleteEventSubscriptionResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopyDBClusterParameterGroupMessageRequestTypeDef,
     CopyDBClusterSnapshotMessageRequestTypeDef,
     CreateDBClusterMessageRequestTypeDef,
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
-    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     CertificateMessageTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
@@ -490,45 +489,46 @@
     DBClusterParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     ModifyDBClusterParameterGroupMessageRequestTypeDef,
     ResetDBClusterParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBClusterTypeDef,
     DBEngineVersionTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
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
-    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
-    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
+    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
+    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
+    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
+    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
+    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
+    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
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
     PendingModifiedValuesTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
@@ -560,15 +560,15 @@
     DBInstanceMessageTypeDef,
     DeleteDBInstanceResultTypeDef,
     ModifyDBInstanceResultTypeDef,
     RebootDBInstanceResultTypeDef,
 )
 
 
-def get_structure() -> AddSourceIdentifierToSubscriptionMessageRequestTypeDef:
+def get_value() -> AddSourceIdentifierToSubscriptionMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-docdb-2.5.2/README.md` & `types-aiobotocore-docdb-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-docdb"></a>
 
 # types-aiobotocore-docdb
 
 [![PyPI - types-aiobotocore-docdb](https://img.shields.io/pypi/v/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-docdb?color=blue)](https://pypistats.org/packages/types-aiobotocore-docdb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb)](https://pepy.tech/project/types-aiobotocore-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DocDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
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
 [types-aiobotocore-docdb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/).
 
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
@@ -363,89 +363,89 @@
 )
 
 
 def check_value(value: ApplyMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_docdb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_docdb.type_defs import (
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     CertificateTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterMemberTypeDef,
     ParameterTypeDef,
-    DBClusterParameterGroupNameMessageTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     EndpointTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     PendingMaintenanceActionTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
+    DBClusterParameterGroupNameMessageTypeDef,
     DeleteEventSubscriptionResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopyDBClusterParameterGroupMessageRequestTypeDef,
     CopyDBClusterSnapshotMessageRequestTypeDef,
     CreateDBClusterMessageRequestTypeDef,
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
-    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     CertificateMessageTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
@@ -457,45 +457,46 @@
     DBClusterParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     ModifyDBClusterParameterGroupMessageRequestTypeDef,
     ResetDBClusterParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBClusterTypeDef,
     DBEngineVersionTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
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
-    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
-    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
+    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
+    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
+    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
+    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
+    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
+    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
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
     PendingModifiedValuesTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
@@ -527,15 +528,15 @@
     DBInstanceMessageTypeDef,
     DeleteDBInstanceResultTypeDef,
     ModifyDBInstanceResultTypeDef,
     RebootDBInstanceResultTypeDef,
 )
 
 
-def get_structure() -> AddSourceIdentifierToSubscriptionMessageRequestTypeDef:
+def get_value() -> AddSourceIdentifierToSubscriptionMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-docdb-2.5.2/setup.py` & `types-aiobotocore-docdb-2.5.2.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-docdb",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_docdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DocDB 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore docdb type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore docdb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_docdb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/"
```

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/__init__.py` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/__init__.pyi` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/__main__.py` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DocDB 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.DocDB 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB\nOther"
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

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/client.py` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("docdb") as client:
         client: DocDBClient
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
     DescribeCertificatesPaginator,
@@ -87,14 +86,15 @@
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     RestoreDBClusterFromSnapshotResultTypeDef,
     RestoreDBClusterToPointInTimeResultTypeDef,
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
@@ -664,16 +664,16 @@
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
@@ -965,15 +965,15 @@
 
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
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
```

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/client.pyi` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("docdb") as client:
         client: DocDBClient
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
     DescribeCertificatesPaginator,
@@ -87,14 +86,15 @@
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     RestoreDBClusterFromSnapshotResultTypeDef,
     RestoreDBClusterToPointInTimeResultTypeDef,
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
@@ -626,16 +626,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_event_subscriptions)
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
@@ -907,15 +907,15 @@
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
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
```

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/literals.py` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/literals.pyi` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/paginator.py` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
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
     CertificateMessageTypeDef,
@@ -63,14 +62,15 @@
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
     "DescribeCertificatesPaginator",
     "DescribeDBClusterParameterGroupsPaginator",
     "DescribeDBClusterParametersPaginator",
     "DescribeDBClusterSnapshotsPaginator",
@@ -103,15 +103,15 @@
     """
 
     def paginate(
         self,
         *,
         CertificateIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describecertificatespaginator)
         """
 
 
@@ -122,15 +122,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclusterparametergroupspaginator)
         """
 
 
@@ -142,15 +142,15 @@
 
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclusterparameterspaginator)
         """
 
 
@@ -165,15 +165,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclustersnapshotspaginator)
         """
 
 
@@ -184,15 +184,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclusterspaginator)
         """
 
 
@@ -208,15 +208,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbengineversionspaginator)
         """
 
 
@@ -227,15 +227,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbinstancespaginator)
         """
 
 
@@ -246,15 +246,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbsubnetgroupspaginator)
         """
 
 
@@ -265,15 +265,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -284,20 +284,20 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeeventspaginator)
         """
 
 
@@ -308,15 +308,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeGlobalClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeglobalclusterspaginator)
         """
 
 
@@ -331,15 +331,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
 
@@ -350,13 +350,13 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describependingmaintenanceactionspaginator)
         """
```

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/paginator.pyi` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,15 @@
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
     CertificateMessageTypeDef,
@@ -63,14 +62,15 @@
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
     "DescribeCertificatesPaginator",
     "DescribeDBClusterParameterGroupsPaginator",
     "DescribeDBClusterParametersPaginator",
     "DescribeDBClusterSnapshotsPaginator",
@@ -100,15 +100,15 @@
     """
 
     def paginate(
         self,
         *,
         CertificateIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describecertificatespaginator)
         """
 
 class DescribeDBClusterParameterGroupsPaginator(AioPaginator):
@@ -118,15 +118,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclusterparametergroupspaginator)
         """
 
 class DescribeDBClusterParametersPaginator(AioPaginator):
@@ -137,15 +137,15 @@
 
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclusterparameterspaginator)
         """
 
 class DescribeDBClusterSnapshotsPaginator(AioPaginator):
@@ -159,15 +159,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclustersnapshotspaginator)
         """
 
 class DescribeDBClustersPaginator(AioPaginator):
@@ -177,15 +177,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclusterspaginator)
         """
 
 class DescribeDBEngineVersionsPaginator(AioPaginator):
@@ -200,15 +200,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbengineversionspaginator)
         """
 
 class DescribeDBInstancesPaginator(AioPaginator):
@@ -218,15 +218,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbinstancespaginator)
         """
 
 class DescribeDBSubnetGroupsPaginator(AioPaginator):
@@ -236,15 +236,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbsubnetgroupspaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(AioPaginator):
@@ -254,15 +254,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -272,20 +272,20 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeeventspaginator)
         """
 
 class DescribeGlobalClustersPaginator(AioPaginator):
@@ -295,15 +295,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeGlobalClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeglobalclusterspaginator)
         """
 
 class DescribeOrderableDBInstanceOptionsPaginator(AioPaginator):
@@ -317,15 +317,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
 class DescribePendingMaintenanceActionsPaginator(AioPaginator):
@@ -335,13 +335,13 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describependingmaintenanceactionspaginator)
         """
```

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/type_defs.py` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,96 +4,95 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_docdb.type_defs import AddSourceIdentifierToSubscriptionMessageRequestTypeDef
 
-    data: AddSourceIdentifierToSubscriptionMessageRequestTypeDef = {...}
+    data: AddSourceIdentifierToSubscriptionMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplyMethodType, SourceTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "CertificateTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "DBClusterParameterGroupTypeDef",
     "DBClusterSnapshotTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterMemberTypeDef",
     "ParameterTypeDef",
-    "DBClusterParameterGroupNameMessageTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "EndpointTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     "DeleteDBClusterSnapshotMessageRequestTypeDef",
     "DeleteDBInstanceMessageRequestTypeDef",
     "DeleteDBSubnetGroupMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteGlobalClusterMessageRequestTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
+    "DBClusterParameterGroupNameMessageTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopyDBClusterParameterGroupMessageRequestTypeDef",
     "CopyDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBClusterMessageRequestTypeDef",
     "CreateDBClusterParameterGroupMessageRequestTypeDef",
     "CreateDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBInstanceMessageRequestTypeDef",
     "CreateDBSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
-    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "TagListMessageTypeDef",
     "OrderableDBInstanceOptionTypeDef",
     "SubnetTypeDef",
     "CertificateMessageTypeDef",
     "ModifyDBClusterMessageRequestTypeDef",
     "CopyDBClusterParameterGroupResultTypeDef",
     "CreateDBClusterParameterGroupResultTypeDef",
@@ -105,45 +104,46 @@
     "DBClusterParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "ModifyDBClusterParameterGroupMessageRequestTypeDef",
     "ResetDBClusterParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBClusterTypeDef",
     "DBEngineVersionTypeDef",
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
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
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultClusterParametersMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     "DescribeGlobalClustersMessageRequestTypeDef",
-    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
-    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
+    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
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
     "PendingModifiedValuesTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
@@ -199,14 +199,25 @@
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
@@ -301,22 +312,20 @@
         "DeletionProtection": bool,
         "DatabaseName": str,
         "StorageEncrypted": bool,
     },
     total=False,
 )
 
-
 class CreateGlobalClusterMessageRequestTypeDef(
     _RequiredCreateGlobalClusterMessageRequestTypeDef,
     _OptionalCreateGlobalClusterMessageRequestTypeDef,
 ):
     pass
 
-
 DBClusterMemberTypeDef = TypedDict(
     "DBClusterMemberTypeDef",
     {
         "DBInstanceIdentifier": str,
         "IsClusterWriter": bool,
         "DBClusterParameterGroupStatus": str,
         "PromotionTier": int,
@@ -337,22 +346,14 @@
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
     },
     total=False,
@@ -420,21 +421,19 @@
     {
         "SkipFinalSnapshot": bool,
         "FinalDBSnapshotIdentifier": str,
     },
     total=False,
 )
 
-
 class DeleteDBClusterMessageRequestTypeDef(
     _RequiredDeleteDBClusterMessageRequestTypeDef, _OptionalDeleteDBClusterMessageRequestTypeDef
 ):
     pass
 
-
 DeleteDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
     },
 )
 
@@ -477,14 +476,24 @@
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
 
@@ -493,21 +502,15 @@
     {
         "Delay": int,
         "MaxAttempts": int,
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
+TimestampTypeDef = Union[datetime, str]
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
     total=False,
@@ -557,22 +560,20 @@
     {
         "ValuesToAdd": Sequence[str],
         "ValuesToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyDBClusterSnapshotAttributeMessageRequestTypeDef(
     _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     _OptionalModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 _OptionalModifyDBInstanceMessageRequestTypeDef = TypedDict(
@@ -588,21 +589,19 @@
         "PromotionTier": int,
         "EnablePerformanceInsights": bool,
         "PerformanceInsightsKMSKeyId": str,
     },
     total=False,
 )
 
-
 class ModifyDBInstanceMessageRequestTypeDef(
     _RequiredModifyDBInstanceMessageRequestTypeDef, _OptionalModifyDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredModifyDBSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -610,22 +609,20 @@
     "_OptionalModifyDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupDescription": str,
     },
     total=False,
 )
 
-
 class ModifyDBSubnetGroupMessageRequestTypeDef(
     _RequiredModifyDBSubnetGroupMessageRequestTypeDef,
     _OptionalModifyDBSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
     },
 )
 _OptionalModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
@@ -635,22 +632,20 @@
         "SourceType": str,
         "EventCategories": Sequence[str],
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class ModifyEventSubscriptionMessageRequestTypeDef(
     _RequiredModifyEventSubscriptionMessageRequestTypeDef,
     _OptionalModifyEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyGlobalClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
     },
 )
 _OptionalModifyGlobalClusterMessageRequestTypeDef = TypedDict(
@@ -658,32 +653,20 @@
     {
         "NewGlobalClusterIdentifier": str,
         "DeletionProtection": bool,
     },
     total=False,
 )
 
-
 class ModifyGlobalClusterMessageRequestTypeDef(
     _RequiredModifyGlobalClusterMessageRequestTypeDef,
     _OptionalModifyGlobalClusterMessageRequestTypeDef,
 ):
     pass
 
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
 PendingCloudwatchLogsExportsTypeDef = TypedDict(
     "PendingCloudwatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": List[str],
         "LogTypesToDisable": List[str],
     },
     total=False,
@@ -712,21 +695,19 @@
     "_OptionalRebootDBInstanceMessageRequestTypeDef",
     {
         "ForceFailover": bool,
     },
     total=False,
 )
 
-
 class RebootDBInstanceMessageRequestTypeDef(
     _RequiredRebootDBInstanceMessageRequestTypeDef, _OptionalRebootDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
 RemoveFromGlobalClusterMessageRequestTypeDef = TypedDict(
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "DbClusterIdentifier": str,
     },
 )
@@ -743,25 +724,14 @@
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
 
@@ -772,56 +742,71 @@
     },
 )
 
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -841,22 +826,20 @@
     "_OptionalCopyDBClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopyDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredCopyDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalCopyDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCopyDBClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBClusterSnapshotMessageRequestTypeDef",
     {
         "SourceDBClusterSnapshotIdentifier": str,
         "TargetDBClusterSnapshotIdentifier": str,
     },
 )
@@ -868,22 +851,20 @@
         "CopyTags": bool,
         "Tags": Sequence[TagTypeDef],
         "SourceRegion": str,
     },
     total=False,
 )
 
-
 class CopyDBClusterSnapshotMessageRequestTypeDef(
     _RequiredCopyDBClusterSnapshotMessageRequestTypeDef,
     _OptionalCopyDBClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "Engine": str,
     },
 )
@@ -909,21 +890,19 @@
         "DeletionProtection": bool,
         "GlobalClusterIdentifier": str,
         "SourceRegion": str,
     },
     total=False,
 )
 
-
 class CreateDBClusterMessageRequestTypeDef(
     _RequiredCreateDBClusterMessageRequestTypeDef, _OptionalCreateDBClusterMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
     },
@@ -932,22 +911,20 @@
     "_OptionalCreateDBClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredCreateDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalCreateDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterSnapshotMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterIdentifier": str,
     },
 )
@@ -955,22 +932,20 @@
     "_OptionalCreateDBClusterSnapshotMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBClusterSnapshotMessageRequestTypeDef(
     _RequiredCreateDBClusterSnapshotMessageRequestTypeDef,
     _OptionalCreateDBClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
         "Engine": str,
         "DBClusterIdentifier": str,
@@ -987,21 +962,19 @@
         "PromotionTier": int,
         "EnablePerformanceInsights": bool,
         "PerformanceInsightsKMSKeyId": str,
     },
     total=False,
 )
 
-
 class CreateDBInstanceMessageRequestTypeDef(
     _RequiredCreateDBInstanceMessageRequestTypeDef, _OptionalCreateDBInstanceMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateDBSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -1010,22 +983,20 @@
     "_OptionalCreateDBSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDBSubnetGroupMessageRequestTypeDef(
     _RequiredCreateDBSubnetGroupMessageRequestTypeDef,
     _OptionalCreateDBSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "SnsTopicArn": str,
     },
 )
@@ -1037,22 +1008,20 @@
         "SourceIds": Sequence[str],
         "Enabled": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "Engine": str,
     },
@@ -1070,59 +1039,25 @@
         "EnableCloudwatchLogsExports": Sequence[str],
         "DeletionProtection": bool,
         "DBClusterParameterGroupName": str,
     },
     total=False,
 )
 
-
 class RestoreDBClusterFromSnapshotMessageRequestTypeDef(
     _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef,
     _OptionalRestoreDBClusterFromSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
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
-        "VpcSecurityGroupIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "EnableCloudwatchLogsExports": Sequence[str],
-        "DeletionProtection": bool,
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
@@ -1146,15 +1081,15 @@
 )
 
 CertificateMessageTypeDef = TypedDict(
     "CertificateMessageTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredModifyDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
@@ -1175,85 +1110,83 @@
         "CloudwatchLogsExportConfiguration": CloudwatchLogsExportConfigurationTypeDef,
         "EngineVersion": str,
         "DeletionProtection": bool,
     },
     total=False,
 )
 
-
 class ModifyDBClusterMessageRequestTypeDef(
     _RequiredModifyDBClusterMessageRequestTypeDef, _OptionalModifyDBClusterMessageRequestTypeDef
 ):
     pass
 
-
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
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
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
@@ -1282,22 +1215,20 @@
     {
         "ResetAllParameters": bool,
         "Parameters": Sequence[ParameterTypeDef],
     },
     total=False,
 )
 
-
 class ResetDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
     total=False,
@@ -1353,80 +1284,36 @@
         "ValidUpgradeTarget": List[UpgradeTargetTypeDef],
         "ExportableLogTypes": List[str],
         "SupportsLogExportsToCloudwatchLogs": bool,
     },
     total=False,
 )
 
-DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
-    {
-        "CertificateIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeCertificatesMessageRequestTypeDef",
     {
         "CertificateIdentifier": str,
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
@@ -1436,36 +1323,20 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeDBClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDBClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDBClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-
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
@@ -1473,50 +1344,25 @@
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
@@ -1525,45 +1371,25 @@
         "DefaultOnly": bool,
         "ListSupportedCharacterSets": bool,
         "ListSupportedTimezones": bool,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
-    {
-        "DBInstanceIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBInstancesMessageRequestTypeDef = TypedDict(
     "DescribeDBInstancesMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
-    {
-        "DBSubnetGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -1583,203 +1409,265 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeEventCategoriesMessageRequestTypeDef = TypedDict(
     "DescribeEventCategoriesMessageRequestTypeDef",
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageRequestTypeDef",
+DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
+    "DescribeGlobalClustersMessageRequestTypeDef",
     {
-        "SubscriptionName": str,
+        "GlobalClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
+        "Engine": str,
+    },
+)
+_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
+    {
+        "EngineVersion": str,
+        "DBInstanceClass": str,
+        "LicenseModel": str,
+        "Vpc": bool,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
+class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
+    _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
+    _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
+):
+    pass
+
+DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
+    "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
+        "ResourceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
         "Marker": str,
+        "MaxRecords": int,
     },
     total=False,
 )
 
-DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+_RequiredListTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_RequiredListTagsForResourceMessageRequestTypeDef",
+    {
+        "ResourceName": str,
+    },
+)
+_OptionalListTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_OptionalListTagsForResourceMessageRequestTypeDef",
     {
-        "GlobalClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
-    "DescribeGlobalClustersMessageRequestTypeDef",
+class ListTagsForResourceMessageRequestTypeDef(
+    _RequiredListTagsForResourceMessageRequestTypeDef,
+    _OptionalListTagsForResourceMessageRequestTypeDef,
+):
+    pass
+
+DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     {
-        "GlobalClusterIdentifier": str,
+        "CertificateIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     {
-        "Engine": str,
+        "DBClusterParameterGroupName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+
+_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     {
-        "EngineVersion": str,
-        "DBInstanceClass": str,
-        "LicenseModel": str,
-        "Vpc": bool,
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
-    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
-    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
+    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
 ):
     pass
 
+DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "DBClusterSnapshotIdentifier": str,
+        "SnapshotType": str,
+        "Filters": Sequence[FilterTypeDef],
+        "IncludeShared": bool,
+        "IncludePublic": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
+DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
     {
-        "Engine": str,
+        "DBClusterIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
+
+DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     {
+        "Engine": str,
         "EngineVersion": str,
-        "DBInstanceClass": str,
-        "LicenseModel": str,
-        "Vpc": bool,
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
 
+DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+    {
+        "DBInstanceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
-    _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-):
-    pass
-
+DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
+    {
+        "DBSubnetGroupName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
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
+        "GlobalClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "Marker": str,
-        "MaxRecords": int,
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
 
-
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
 
 DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef = TypedDict(
     "DescribeDBInstancesMessageDBInstanceAvailableWaitTypeDef",
     {
         "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
@@ -1797,28 +1685,89 @@
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
+        "VpcSecurityGroupIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "EnableCloudwatchLogsExports": Sequence[str],
+        "DeletionProtection": bool,
+    },
+    total=False,
+)
+
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
@@ -1866,15 +1815,15 @@
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
@@ -1887,179 +1836,179 @@
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
@@ -2094,59 +2043,59 @@
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

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/type_defs.pyi` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,95 +4,96 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_docdb.type_defs import AddSourceIdentifierToSubscriptionMessageRequestTypeDef
 
-    data: AddSourceIdentifierToSubscriptionMessageRequestTypeDef = {...}
+    data: AddSourceIdentifierToSubscriptionMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplyMethodType, SourceTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "CertificateTypeDef",
     "CloudwatchLogsExportConfigurationTypeDef",
     "DBClusterParameterGroupTypeDef",
     "DBClusterSnapshotTypeDef",
     "CreateGlobalClusterMessageRequestTypeDef",
     "DBClusterMemberTypeDef",
     "ParameterTypeDef",
-    "DBClusterParameterGroupNameMessageTypeDef",
     "DBClusterRoleTypeDef",
     "DBClusterSnapshotAttributeTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "UpgradeTargetTypeDef",
     "DBInstanceStatusInfoTypeDef",
     "EndpointTypeDef",
     "DeleteDBClusterMessageRequestTypeDef",
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     "DeleteDBClusterSnapshotMessageRequestTypeDef",
     "DeleteDBInstanceMessageRequestTypeDef",
     "DeleteDBSubnetGroupMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteGlobalClusterMessageRequestTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDBClusterSnapshotAttributesMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "EventCategoriesMapTypeDef",
     "EventTypeDef",
     "FailoverDBClusterMessageRequestTypeDef",
     "GlobalClusterMemberTypeDef",
     "ModifyDBClusterSnapshotAttributeMessageRequestTypeDef",
     "ModifyDBInstanceMessageRequestTypeDef",
     "ModifyDBSubnetGroupMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyGlobalClusterMessageRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PendingCloudwatchLogsExportsTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RebootDBInstanceMessageRequestTypeDef",
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     "RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartDBClusterMessageRequestTypeDef",
     "StopDBClusterMessageRequestTypeDef",
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     "CreateEventSubscriptionResultTypeDef",
+    "DBClusterParameterGroupNameMessageTypeDef",
     "DeleteEventSubscriptionResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EventSubscriptionsMessageTypeDef",
     "ModifyEventSubscriptionResultTypeDef",
     "RemoveSourceIdentifierFromSubscriptionResultTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopyDBClusterParameterGroupMessageRequestTypeDef",
     "CopyDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBClusterMessageRequestTypeDef",
     "CreateDBClusterParameterGroupMessageRequestTypeDef",
     "CreateDBClusterSnapshotMessageRequestTypeDef",
     "CreateDBInstanceMessageRequestTypeDef",
     "CreateDBSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "RestoreDBClusterFromSnapshotMessageRequestTypeDef",
-    "RestoreDBClusterToPointInTimeMessageRequestTypeDef",
     "TagListMessageTypeDef",
     "OrderableDBInstanceOptionTypeDef",
     "SubnetTypeDef",
     "CertificateMessageTypeDef",
     "ModifyDBClusterMessageRequestTypeDef",
     "CopyDBClusterParameterGroupResultTypeDef",
     "CreateDBClusterParameterGroupResultTypeDef",
@@ -104,45 +105,46 @@
     "DBClusterParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "ModifyDBClusterParameterGroupMessageRequestTypeDef",
     "ResetDBClusterParameterGroupMessageRequestTypeDef",
     "DBClusterSnapshotAttributesResultTypeDef",
     "DBClusterTypeDef",
     "DBEngineVersionTypeDef",
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
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
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     "DescribeEngineDefaultClusterParametersMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
     "DescribeGlobalClustersMessageRequestTypeDef",
-    "DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
     "DescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
-    "DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
+    "DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
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
     "PendingModifiedValuesTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "OrderableDBInstanceOptionsMessageTypeDef",
     "DBSubnetGroupTypeDef",
@@ -198,14 +200,25 @@
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
@@ -300,20 +313,22 @@
         "DeletionProtection": bool,
         "DatabaseName": str,
         "StorageEncrypted": bool,
     },
     total=False,
 )
 
+
 class CreateGlobalClusterMessageRequestTypeDef(
     _RequiredCreateGlobalClusterMessageRequestTypeDef,
     _OptionalCreateGlobalClusterMessageRequestTypeDef,
 ):
     pass
 
+
 DBClusterMemberTypeDef = TypedDict(
     "DBClusterMemberTypeDef",
     {
         "DBInstanceIdentifier": str,
         "IsClusterWriter": bool,
         "DBClusterParameterGroupStatus": str,
         "PromotionTier": int,
@@ -334,22 +349,14 @@
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
     },
     total=False,
@@ -417,19 +424,21 @@
     {
         "SkipFinalSnapshot": bool,
         "FinalDBSnapshotIdentifier": str,
     },
     total=False,
 )
 
+
 class DeleteDBClusterMessageRequestTypeDef(
     _RequiredDeleteDBClusterMessageRequestTypeDef, _OptionalDeleteDBClusterMessageRequestTypeDef
 ):
     pass
 
+
 DeleteDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
     },
 )
 
@@ -472,14 +481,24 @@
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
 
@@ -488,21 +507,15 @@
     {
         "Delay": int,
         "MaxAttempts": int,
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
+TimestampTypeDef = Union[datetime, str]
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
         "EventCategories": List[str],
     },
     total=False,
@@ -552,20 +565,22 @@
     {
         "ValuesToAdd": Sequence[str],
         "ValuesToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyDBClusterSnapshotAttributeMessageRequestTypeDef(
     _RequiredModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     _OptionalModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
     },
 )
 _OptionalModifyDBInstanceMessageRequestTypeDef = TypedDict(
@@ -581,19 +596,21 @@
         "PromotionTier": int,
         "EnablePerformanceInsights": bool,
         "PerformanceInsightsKMSKeyId": str,
     },
     total=False,
 )
 
+
 class ModifyDBInstanceMessageRequestTypeDef(
     _RequiredModifyDBInstanceMessageRequestTypeDef, _OptionalModifyDBInstanceMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredModifyDBSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -601,20 +618,22 @@
     "_OptionalModifyDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupDescription": str,
     },
     total=False,
 )
 
+
 class ModifyDBSubnetGroupMessageRequestTypeDef(
     _RequiredModifyDBSubnetGroupMessageRequestTypeDef,
     _OptionalModifyDBSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
     },
 )
 _OptionalModifyEventSubscriptionMessageRequestTypeDef = TypedDict(
@@ -624,20 +643,22 @@
         "SourceType": str,
         "EventCategories": Sequence[str],
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class ModifyEventSubscriptionMessageRequestTypeDef(
     _RequiredModifyEventSubscriptionMessageRequestTypeDef,
     _OptionalModifyEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyGlobalClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
     },
 )
 _OptionalModifyGlobalClusterMessageRequestTypeDef = TypedDict(
@@ -645,29 +666,21 @@
     {
         "NewGlobalClusterIdentifier": str,
         "DeletionProtection": bool,
     },
     total=False,
 )
 
+
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
 
 PendingCloudwatchLogsExportsTypeDef = TypedDict(
     "PendingCloudwatchLogsExportsTypeDef",
     {
         "LogTypesToEnable": List[str],
         "LogTypesToDisable": List[str],
     },
@@ -697,19 +710,21 @@
     "_OptionalRebootDBInstanceMessageRequestTypeDef",
     {
         "ForceFailover": bool,
     },
     total=False,
 )
 
+
 class RebootDBInstanceMessageRequestTypeDef(
     _RequiredRebootDBInstanceMessageRequestTypeDef, _OptionalRebootDBInstanceMessageRequestTypeDef
 ):
     pass
 
+
 RemoveFromGlobalClusterMessageRequestTypeDef = TypedDict(
     "RemoveFromGlobalClusterMessageRequestTypeDef",
     {
         "GlobalClusterIdentifier": str,
         "DbClusterIdentifier": str,
     },
 )
@@ -726,25 +741,14 @@
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
 
@@ -755,56 +759,71 @@
     },
 )
 
 AddSourceIdentifierToSubscriptionResultTypeDef = TypedDict(
     "AddSourceIdentifierToSubscriptionResultTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -824,20 +843,22 @@
     "_OptionalCopyDBClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopyDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredCopyDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalCopyDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCopyDBClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCopyDBClusterSnapshotMessageRequestTypeDef",
     {
         "SourceDBClusterSnapshotIdentifier": str,
         "TargetDBClusterSnapshotIdentifier": str,
     },
 )
@@ -849,20 +870,22 @@
         "CopyTags": bool,
         "Tags": Sequence[TagTypeDef],
         "SourceRegion": str,
     },
     total=False,
 )
 
+
 class CopyDBClusterSnapshotMessageRequestTypeDef(
     _RequiredCopyDBClusterSnapshotMessageRequestTypeDef,
     _OptionalCopyDBClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "Engine": str,
     },
 )
@@ -888,19 +911,21 @@
         "DeletionProtection": bool,
         "GlobalClusterIdentifier": str,
         "SourceRegion": str,
     },
     total=False,
 )
 
+
 class CreateDBClusterMessageRequestTypeDef(
     _RequiredCreateDBClusterMessageRequestTypeDef, _OptionalCreateDBClusterMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateDBClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterParameterGroupMessageRequestTypeDef",
     {
         "DBClusterParameterGroupName": str,
         "DBParameterGroupFamily": str,
         "Description": str,
     },
@@ -909,20 +934,22 @@
     "_OptionalCreateDBClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredCreateDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalCreateDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBClusterSnapshotMessageRequestTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterIdentifier": str,
     },
 )
@@ -930,20 +957,22 @@
     "_OptionalCreateDBClusterSnapshotMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBClusterSnapshotMessageRequestTypeDef(
     _RequiredCreateDBClusterSnapshotMessageRequestTypeDef,
     _OptionalCreateDBClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDBInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBInstanceMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
         "Engine": str,
         "DBClusterIdentifier": str,
@@ -960,19 +989,21 @@
         "PromotionTier": int,
         "EnablePerformanceInsights": bool,
         "PerformanceInsightsKMSKeyId": str,
     },
     total=False,
 )
 
+
 class CreateDBInstanceMessageRequestTypeDef(
     _RequiredCreateDBInstanceMessageRequestTypeDef, _OptionalCreateDBInstanceMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateDBSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateDBSubnetGroupMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "DBSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -981,20 +1012,22 @@
     "_OptionalCreateDBSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDBSubnetGroupMessageRequestTypeDef(
     _RequiredCreateDBSubnetGroupMessageRequestTypeDef,
     _OptionalCreateDBSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateEventSubscriptionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEventSubscriptionMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "SnsTopicArn": str,
     },
 )
@@ -1006,20 +1039,22 @@
         "SourceIds": Sequence[str],
         "Enabled": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateEventSubscriptionMessageRequestTypeDef(
     _RequiredCreateEventSubscriptionMessageRequestTypeDef,
     _OptionalCreateEventSubscriptionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreDBClusterFromSnapshotMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "Engine": str,
     },
@@ -1037,55 +1072,27 @@
         "EnableCloudwatchLogsExports": Sequence[str],
         "DeletionProtection": bool,
         "DBClusterParameterGroupName": str,
     },
     total=False,
 )
 
+
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
-        "VpcSecurityGroupIds": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "EnableCloudwatchLogsExports": Sequence[str],
-        "DeletionProtection": bool,
-    },
-    total=False,
-)
-
-class RestoreDBClusterToPointInTimeMessageRequestTypeDef(
-    _RequiredRestoreDBClusterToPointInTimeMessageRequestTypeDef,
-    _OptionalRestoreDBClusterToPointInTimeMessageRequestTypeDef,
-):
-    pass
 
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
@@ -1109,15 +1116,15 @@
 )
 
 CertificateMessageTypeDef = TypedDict(
     "CertificateMessageTypeDef",
     {
         "Certificates": List[CertificateTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredModifyDBClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyDBClusterMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
@@ -1138,83 +1145,85 @@
         "CloudwatchLogsExportConfiguration": CloudwatchLogsExportConfigurationTypeDef,
         "EngineVersion": str,
         "DeletionProtection": bool,
     },
     total=False,
 )
 
+
 class ModifyDBClusterMessageRequestTypeDef(
     _RequiredModifyDBClusterMessageRequestTypeDef, _OptionalModifyDBClusterMessageRequestTypeDef
 ):
     pass
 
+
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
 
 DBClusterParameterGroupDetailsTypeDef = TypedDict(
     "DBClusterParameterGroupDetailsTypeDef",
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
@@ -1243,20 +1252,22 @@
     {
         "ResetAllParameters": bool,
         "Parameters": Sequence[ParameterTypeDef],
     },
     total=False,
 )
 
+
 class ResetDBClusterParameterGroupMessageRequestTypeDef(
     _RequiredResetDBClusterParameterGroupMessageRequestTypeDef,
     _OptionalResetDBClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 DBClusterSnapshotAttributesResultTypeDef = TypedDict(
     "DBClusterSnapshotAttributesResultTypeDef",
     {
         "DBClusterSnapshotIdentifier": str,
         "DBClusterSnapshotAttributes": List[DBClusterSnapshotAttributeTypeDef],
     },
     total=False,
@@ -1312,78 +1323,36 @@
         "ValidUpgradeTarget": List[UpgradeTargetTypeDef],
         "ExportableLogTypes": List[str],
         "SupportsLogExportsToCloudwatchLogs": bool,
     },
     total=False,
 )
 
-DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
-    {
-        "CertificateIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeCertificatesMessageRequestTypeDef",
     {
         "CertificateIdentifier": str,
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
@@ -1393,33 +1362,21 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
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
 
 DescribeDBClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeDBClusterSnapshotsMessageRequestTypeDef",
     {
         "DBClusterIdentifier": str,
         "DBClusterSnapshotIdentifier": str,
         "SnapshotType": str,
@@ -1428,50 +1385,25 @@
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
@@ -1480,45 +1412,25 @@
         "DefaultOnly": bool,
         "ListSupportedCharacterSets": bool,
         "ListSupportedTimezones": bool,
     },
     total=False,
 )
 
-DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
-    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
-    {
-        "DBInstanceIdentifier": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBInstancesMessageRequestTypeDef = TypedDict(
     "DescribeDBInstancesMessageRequestTypeDef",
     {
         "DBInstanceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef",
-    {
-        "DBSubnetGroupName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDBSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeDBSubnetGroupsMessageRequestTypeDef",
     {
         "DBSubnetGroupName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -1538,234 +1450,377 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeEngineDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeEventCategoriesMessageRequestTypeDef = TypedDict(
     "DescribeEventCategoriesMessageRequestTypeDef",
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageRequestTypeDef",
+DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
+    "DescribeGlobalClustersMessageRequestTypeDef",
     {
-        "SubscriptionName": str,
+        "GlobalClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
     {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
+        "Engine": str,
+    },
+)
+_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
+    {
+        "EngineVersion": str,
+        "DBInstanceClass": str,
+        "LicenseModel": str,
+        "Vpc": bool,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
+
+class DescribeOrderableDBInstanceOptionsMessageRequestTypeDef(
+    _RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
+    _OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
+):
+    pass
+
+
+DescribePendingMaintenanceActionsMessageRequestTypeDef = TypedDict(
+    "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
+        "ResourceIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
         "Marker": str,
+        "MaxRecords": int,
     },
     total=False,
 )
 
-DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef = TypedDict(
-    "DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef",
+_RequiredListTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_RequiredListTagsForResourceMessageRequestTypeDef",
+    {
+        "ResourceName": str,
+    },
+)
+_OptionalListTagsForResourceMessageRequestTypeDef = TypedDict(
+    "_OptionalListTagsForResourceMessageRequestTypeDef",
     {
-        "GlobalClusterIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeGlobalClustersMessageRequestTypeDef = TypedDict(
-    "DescribeGlobalClustersMessageRequestTypeDef",
+
+class ListTagsForResourceMessageRequestTypeDef(
+    _RequiredListTagsForResourceMessageRequestTypeDef,
+    _OptionalListTagsForResourceMessageRequestTypeDef,
+):
+    pass
+
+
+DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     {
-        "GlobalClusterIdentifier": str,
+        "CertificateIdentifier": str,
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef",
     {
-        "Engine": str,
+        "DBClusterParameterGroupName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+
+_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
     {
-        "EngineVersion": str,
-        "DBInstanceClass": str,
-        "LicenseModel": str,
-        "Vpc": bool,
+        "DBClusterParameterGroupName": str,
+    },
+)
+_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef",
+    {
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
+
+class DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef(
+    _RequiredDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    _OptionalDescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
 ):
     pass
 
-_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
+
+DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "DBClusterSnapshotIdentifier": str,
+        "SnapshotType": str,
+        "Filters": Sequence[FilterTypeDef],
+        "IncludeShared": bool,
+        "IncludePublic": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef = TypedDict(
+    "DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef",
+    {
+        "DBClusterIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef",
     {
         "Engine": str,
+        "EngineVersion": str,
+        "DBParameterGroupFamily": str,
+        "Filters": Sequence[FilterTypeDef],
+        "DefaultOnly": bool,
+        "ListSupportedCharacterSets": bool,
+        "ListSupportedTimezones": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeOrderableDBInstanceOptionsMessageRequestTypeDef",
+
+DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef = TypedDict(
+    "DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef",
+    {
+        "DBInstanceIdentifier": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
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
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef",
+    {
+        "Engine": str,
+    },
+)
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
+
+class DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef(
+    _RequiredDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
+    _OptionalDescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
 ):
     pass
 
+
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
+        "VpcSecurityGroupIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "EnableCloudwatchLogsExports": Sequence[str],
+        "DeletionProtection": bool,
     },
     total=False,
 )
 
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
@@ -1813,15 +1868,15 @@
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
@@ -1834,179 +1889,179 @@
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
@@ -2041,59 +2096,59 @@
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

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/waiter.py` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb/waiter.pyi` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb.egg-info/PKG-INFO` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DocDB 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DocDB 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore docdb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore docdb type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-docdb"></a>
 
 # types-aiobotocore-docdb
 
 [![PyPI - types-aiobotocore-docdb](https://img.shields.io/pypi/v/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-docdb?color=blue)](https://pypistats.org/packages/types-aiobotocore-docdb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb)](https://pepy.tech/project/types-aiobotocore-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DocDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
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
 [types-aiobotocore-docdb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/).
 
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
@@ -396,89 +395,89 @@
 )
 
 
 def check_value(value: ApplyMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_docdb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_docdb.type_defs import (
     AddSourceIdentifierToSubscriptionMessageRequestTypeDef,
     EventSubscriptionTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     CertificateTypeDef,
     CloudwatchLogsExportConfigurationTypeDef,
     DBClusterParameterGroupTypeDef,
     DBClusterSnapshotTypeDef,
     CreateGlobalClusterMessageRequestTypeDef,
     DBClusterMemberTypeDef,
     ParameterTypeDef,
-    DBClusterParameterGroupNameMessageTypeDef,
     DBClusterRoleTypeDef,
     DBClusterSnapshotAttributeTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     UpgradeTargetTypeDef,
     DBInstanceStatusInfoTypeDef,
     EndpointTypeDef,
     DeleteDBClusterMessageRequestTypeDef,
     DeleteDBClusterParameterGroupMessageRequestTypeDef,
     DeleteDBClusterSnapshotMessageRequestTypeDef,
     DeleteDBInstanceMessageRequestTypeDef,
     DeleteDBSubnetGroupMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteGlobalClusterMessageRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDBClusterSnapshotAttributesMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampTypeDef,
     EventCategoriesMapTypeDef,
     EventTypeDef,
     FailoverDBClusterMessageRequestTypeDef,
     GlobalClusterMemberTypeDef,
     ModifyDBClusterSnapshotAttributeMessageRequestTypeDef,
     ModifyDBInstanceMessageRequestTypeDef,
     ModifyDBSubnetGroupMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyGlobalClusterMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingCloudwatchLogsExportsTypeDef,
     PendingMaintenanceActionTypeDef,
     RebootDBInstanceMessageRequestTypeDef,
     RemoveFromGlobalClusterMessageRequestTypeDef,
     RemoveSourceIdentifierFromSubscriptionMessageRequestTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartDBClusterMessageRequestTypeDef,
     StopDBClusterMessageRequestTypeDef,
     AddSourceIdentifierToSubscriptionResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
+    DBClusterParameterGroupNameMessageTypeDef,
     DeleteEventSubscriptionResultTypeDef,
+    EmptyResponseMetadataTypeDef,
     EventSubscriptionsMessageTypeDef,
     ModifyEventSubscriptionResultTypeDef,
     RemoveSourceIdentifierFromSubscriptionResultTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopyDBClusterParameterGroupMessageRequestTypeDef,
     CopyDBClusterSnapshotMessageRequestTypeDef,
     CreateDBClusterMessageRequestTypeDef,
     CreateDBClusterParameterGroupMessageRequestTypeDef,
     CreateDBClusterSnapshotMessageRequestTypeDef,
     CreateDBInstanceMessageRequestTypeDef,
     CreateDBSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     RestoreDBClusterFromSnapshotMessageRequestTypeDef,
-    RestoreDBClusterToPointInTimeMessageRequestTypeDef,
     TagListMessageTypeDef,
     OrderableDBInstanceOptionTypeDef,
     SubnetTypeDef,
     CertificateMessageTypeDef,
     ModifyDBClusterMessageRequestTypeDef,
     CopyDBClusterParameterGroupResultTypeDef,
     CreateDBClusterParameterGroupResultTypeDef,
@@ -490,45 +489,46 @@
     DBClusterParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     ModifyDBClusterParameterGroupMessageRequestTypeDef,
     ResetDBClusterParameterGroupMessageRequestTypeDef,
     DBClusterSnapshotAttributesResultTypeDef,
     DBClusterTypeDef,
     DBEngineVersionTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
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
-    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
     DescribeDBSubnetGroupsMessageRequestTypeDef,
     DescribeEngineDefaultClusterParametersMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    DescribeGlobalClustersMessageDescribeGlobalClustersPaginateTypeDef,
     DescribeGlobalClustersMessageRequestTypeDef,
-    DescribeOrderableDBInstanceOptionsMessageDescribeOrderableDBInstanceOptionsPaginateTypeDef,
     DescribeOrderableDBInstanceOptionsMessageRequestTypeDef,
-    DescribePendingMaintenanceActionsMessageDescribePendingMaintenanceActionsPaginateTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
+    DescribeDBClusterParameterGroupsMessageDescribeDBClusterParameterGroupsPaginateTypeDef,
+    DescribeDBClusterParametersMessageDescribeDBClusterParametersPaginateTypeDef,
+    DescribeDBClusterSnapshotsMessageDescribeDBClusterSnapshotsPaginateTypeDef,
+    DescribeDBClustersMessageDescribeDBClustersPaginateTypeDef,
+    DescribeDBEngineVersionsMessageDescribeDBEngineVersionsPaginateTypeDef,
+    DescribeDBInstancesMessageDescribeDBInstancesPaginateTypeDef,
+    DescribeDBSubnetGroupsMessageDescribeDBSubnetGroupsPaginateTypeDef,
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
     PendingModifiedValuesTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     OrderableDBInstanceOptionsMessageTypeDef,
     DBSubnetGroupTypeDef,
@@ -560,15 +560,15 @@
     DBInstanceMessageTypeDef,
     DeleteDBInstanceResultTypeDef,
     ModifyDBInstanceResultTypeDef,
     RebootDBInstanceResultTypeDef,
 )
 
 
-def get_structure() -> AddSourceIdentifierToSubscriptionMessageRequestTypeDef:
+def get_value() -> AddSourceIdentifierToSubscriptionMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-docdb-2.5.2/types_aiobotocore_docdb.egg-info/SOURCES.txt` & `types-aiobotocore-docdb-2.5.2.post1/types_aiobotocore_docdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-elasticache-2.5.2.tar.gz` & `tmp/types-aiobotocore-elasticache-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elasticache-2.5.2.tar", last modified: Sat Jul  8 01:43:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-elasticache-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
```

## Comparing `types-aiobotocore-elasticache-2.5.2.tar` & `types-aiobotocore-elasticache-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.362089 types-aiobotocore-elasticache-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27927 2023-07-08 01:43:35.358088 types-aiobotocore-elasticache-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26346 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:35.362089 types-aiobotocore-elasticache-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-08 01:30:20.000000 types-aiobotocore-elasticache-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.354088 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71044 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    70949 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-07-08 01:30:22.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23603 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23584 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86404 2023-07-08 01:30:24.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86337 2023-07-08 01:30:22.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-08 01:30:21.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.358088 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27927 2023-07-08 01:43:35.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-08 01:43:35.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:35.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:43:35.000000 types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.785593 types-aiobotocore-elasticache-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27950 2023-08-02 14:52:14.785593 types-aiobotocore-elasticache-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26416 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.785593 types-aiobotocore-elasticache-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.785593 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70967 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70872 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-08-02 14:38:10.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-08-02 14:38:10.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23522 2023-08-02 14:38:09.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23503 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86837 2023-08-02 14:38:12.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86770 2023-08-02 14:38:11.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:08.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-08-02 14:38:10.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-08-02 14:38:09.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.785593 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27950 2023-08-02 14:52:14.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-02 14:52:14.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:14.000000 types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elasticache-2.5.2/LICENSE` & `types-aiobotocore-elasticache-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2/PKG-INFO` & `types-aiobotocore-elasticache-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elasticache
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElastiCache 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElastiCache 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore elasticache type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore elasticache type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elasticache"></a>
 
 # types-aiobotocore-elasticache
 
 [![PyPI - types-aiobotocore-elasticache](https://img.shields.io/pypi/v/types-aiobotocore-elasticache.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticache)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticache.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticache)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elasticache?color=blue)](https://pypistats.org/packages/types-aiobotocore-elasticache)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticache)](https://pepy.tech/project/types-aiobotocore-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElastiCache 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [types-aiobotocore-elasticache docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/).
 
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
@@ -456,25 +455,25 @@
 )
 
 
 def check_value(value: AZModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elasticache.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elasticache.type_defs import (
     TagTypeDef,
-    AllowedNodeTypeModificationsMessageTypeDef,
+    ResponseMetadataTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     BatchApplyUpdateActionMessageRequestTypeDef,
     BatchStopUpdateActionMessageRequestTypeDef,
     CacheParameterGroupStatusTypeDef,
@@ -482,184 +481,187 @@
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     SecurityGroupMembershipTypeDef,
     CacheEngineVersionTypeDef,
     CacheNodeTypeSpecificValueTypeDef,
     CacheNodeUpdateStatusTypeDef,
     ParameterTypeDef,
-    CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
-    NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     DeleteCacheClusterMessageRequestTypeDef,
     DeleteCacheParameterGroupMessageRequestTypeDef,
     DeleteCacheSecurityGroupMessageRequestTypeDef,
     DeleteCacheSubnetGroupMessageRequestTypeDef,
     DeleteGlobalReplicationGroupMessageRequestTypeDef,
     DeleteReplicationGroupMessageRequestTypeDef,
     DeleteSnapshotMessageRequestTypeDef,
     DeleteUserGroupMessageRequestTypeDef,
     DeleteUserMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCacheClustersMessageRequestTypeDef,
-    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
     DescribeCacheEngineVersionsMessageRequestTypeDef,
-    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
     DescribeCacheParameterGroupsMessageRequestTypeDef,
-    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     DescribeCacheParametersMessageRequestTypeDef,
-    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
     DescribeCacheSecurityGroupsMessageRequestTypeDef,
-    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
     DescribeCacheSubnetGroupsMessageRequestTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
+    TimestampTypeDef,
     DescribeGlobalReplicationGroupsMessageRequestTypeDef,
-    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
     DescribeReplicationGroupsMessageRequestTypeDef,
-    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
     DescribeReservedCacheNodesMessageRequestTypeDef,
-    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
     DescribeReservedCacheNodesOfferingsMessageRequestTypeDef,
-    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
     DescribeServiceUpdatesMessageRequestTypeDef,
-    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
-    TimeRangeFilterTypeDef,
-    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
     GlobalReplicationGroupInfoTypeDef,
     GlobalReplicationGroupMemberTypeDef,
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
+    NodeGroupConfigurationTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
-    PaginatorConfigTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
     SlotMigrationTypeDef,
-    ResponseMetadataTypeDef,
     RevokeCacheSecurityGroupIngressMessageRequestTypeDef,
     ServiceUpdateTypeDef,
     SubnetOutpostTypeDef,
     TestFailoverMessageRequestTypeDef,
     UnprocessedUpdateActionTypeDef,
     UserGroupPendingChangesTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
+    AllowedNodeTypeModificationsMessageTypeDef,
+    CacheParameterGroupNameMessageTypeDef,
+    EmptyResponseMetadataTypeDef,
     TagListMessageTypeDef,
     CreateUserMessageRequestTypeDef,
     ModifyUserMessageRequestTypeDef,
-    UserResponseMetadataTypeDef,
+    UserResponseTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
     CacheSecurityGroupTypeDef,
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
-    NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
-    DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
-    DescribeUpdateActionsMessageRequestTypeDef,
+    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
+    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
+    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
+    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
+    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
+    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
+    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
+    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
+    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
+    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
+    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    TimeRangeFilterTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
+    NodeSnapshotTypeDef,
+    NodeGroupConfigurationUnionTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
     UpdateActionResultsMessageTypeDef,
-    UserGroupResponseMetadataTypeDef,
+    UserGroupResponseTypeDef,
     UserGroupTypeDef,
     DescribeUsersResultTypeDef,
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
-    SnapshotTypeDef,
+    DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
+    DescribeUpdateActionsMessageRequestTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
+    SnapshotTypeDef,
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
-    CopySnapshotResultTypeDef,
-    CreateSnapshotResultTypeDef,
-    DeleteSnapshotResultTypeDef,
-    DescribeSnapshotsListMessageTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ReplicationGroupPendingModifiedValuesTypeDef,
+    CopySnapshotResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     CacheClusterTypeDef,
     ReplicationGroupTypeDef,
     CacheClusterMessageTypeDef,
@@ -676,15 +678,15 @@
     ModifyReplicationGroupShardConfigurationResultTypeDef,
     ReplicationGroupMessageTypeDef,
     StartMigrationResponseTypeDef,
     TestFailoverResultTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elasticache-2.5.2/README.md` & `types-aiobotocore-elasticache-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-elasticache"></a>
 
 # types-aiobotocore-elasticache
 
 [![PyPI - types-aiobotocore-elasticache](https://img.shields.io/pypi/v/types-aiobotocore-elasticache.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticache)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticache.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticache)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elasticache?color=blue)](https://pypistats.org/packages/types-aiobotocore-elasticache)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticache)](https://pepy.tech/project/types-aiobotocore-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElastiCache 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [types-aiobotocore-elasticache docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/).
 
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
@@ -423,25 +423,25 @@
 )
 
 
 def check_value(value: AZModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elasticache.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elasticache.type_defs import (
     TagTypeDef,
-    AllowedNodeTypeModificationsMessageTypeDef,
+    ResponseMetadataTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     BatchApplyUpdateActionMessageRequestTypeDef,
     BatchStopUpdateActionMessageRequestTypeDef,
     CacheParameterGroupStatusTypeDef,
@@ -449,184 +449,187 @@
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     SecurityGroupMembershipTypeDef,
     CacheEngineVersionTypeDef,
     CacheNodeTypeSpecificValueTypeDef,
     CacheNodeUpdateStatusTypeDef,
     ParameterTypeDef,
-    CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
-    NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     DeleteCacheClusterMessageRequestTypeDef,
     DeleteCacheParameterGroupMessageRequestTypeDef,
     DeleteCacheSecurityGroupMessageRequestTypeDef,
     DeleteCacheSubnetGroupMessageRequestTypeDef,
     DeleteGlobalReplicationGroupMessageRequestTypeDef,
     DeleteReplicationGroupMessageRequestTypeDef,
     DeleteSnapshotMessageRequestTypeDef,
     DeleteUserGroupMessageRequestTypeDef,
     DeleteUserMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCacheClustersMessageRequestTypeDef,
-    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
     DescribeCacheEngineVersionsMessageRequestTypeDef,
-    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
     DescribeCacheParameterGroupsMessageRequestTypeDef,
-    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     DescribeCacheParametersMessageRequestTypeDef,
-    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
     DescribeCacheSecurityGroupsMessageRequestTypeDef,
-    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
     DescribeCacheSubnetGroupsMessageRequestTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
+    TimestampTypeDef,
     DescribeGlobalReplicationGroupsMessageRequestTypeDef,
-    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
     DescribeReplicationGroupsMessageRequestTypeDef,
-    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
     DescribeReservedCacheNodesMessageRequestTypeDef,
-    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
     DescribeReservedCacheNodesOfferingsMessageRequestTypeDef,
-    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
     DescribeServiceUpdatesMessageRequestTypeDef,
-    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
-    TimeRangeFilterTypeDef,
-    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
     GlobalReplicationGroupInfoTypeDef,
     GlobalReplicationGroupMemberTypeDef,
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
+    NodeGroupConfigurationTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
-    PaginatorConfigTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
     SlotMigrationTypeDef,
-    ResponseMetadataTypeDef,
     RevokeCacheSecurityGroupIngressMessageRequestTypeDef,
     ServiceUpdateTypeDef,
     SubnetOutpostTypeDef,
     TestFailoverMessageRequestTypeDef,
     UnprocessedUpdateActionTypeDef,
     UserGroupPendingChangesTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
+    AllowedNodeTypeModificationsMessageTypeDef,
+    CacheParameterGroupNameMessageTypeDef,
+    EmptyResponseMetadataTypeDef,
     TagListMessageTypeDef,
     CreateUserMessageRequestTypeDef,
     ModifyUserMessageRequestTypeDef,
-    UserResponseMetadataTypeDef,
+    UserResponseTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
     CacheSecurityGroupTypeDef,
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
-    NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
-    DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
-    DescribeUpdateActionsMessageRequestTypeDef,
+    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
+    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
+    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
+    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
+    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
+    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
+    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
+    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
+    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
+    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
+    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    TimeRangeFilterTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
+    NodeSnapshotTypeDef,
+    NodeGroupConfigurationUnionTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
     UpdateActionResultsMessageTypeDef,
-    UserGroupResponseMetadataTypeDef,
+    UserGroupResponseTypeDef,
     UserGroupTypeDef,
     DescribeUsersResultTypeDef,
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
-    SnapshotTypeDef,
+    DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
+    DescribeUpdateActionsMessageRequestTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
+    SnapshotTypeDef,
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
-    CopySnapshotResultTypeDef,
-    CreateSnapshotResultTypeDef,
-    DeleteSnapshotResultTypeDef,
-    DescribeSnapshotsListMessageTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ReplicationGroupPendingModifiedValuesTypeDef,
+    CopySnapshotResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     CacheClusterTypeDef,
     ReplicationGroupTypeDef,
     CacheClusterMessageTypeDef,
@@ -643,15 +646,15 @@
     ModifyReplicationGroupShardConfigurationResultTypeDef,
     ReplicationGroupMessageTypeDef,
     StartMigrationResponseTypeDef,
     TestFailoverResultTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elasticache-2.5.2/setup.py` & `types-aiobotocore-elasticache-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elasticache",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_elasticache"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElastiCache 2.5.2 service generated with"
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
-    keywords="aiobotocore elasticache type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore elasticache type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_elasticache": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/"
```

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/__init__.py` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/__init__.pyi` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/__main__.py` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElastiCache 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ElastiCache 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache\nOther"
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

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/client.py` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("elasticache") as client:
         client: ElastiCacheClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AuthTokenUpdateStrategyTypeType,
     AZModeType,
@@ -94,15 +93,15 @@
     IncreaseReplicaCountResultTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     ModifyCacheClusterResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     ModifyReplicationGroupResultTypeDef,
     ModifyReplicationGroupShardConfigurationResultTypeDef,
-    NodeGroupConfigurationTypeDef,
+    NodeGroupConfigurationUnionTypeDef,
     ParameterNameValueTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     RebootCacheClusterResultTypeDef,
     RegionalConfigurationTypeDef,
     ReplicationGroupMessageTypeDef,
     ReservedCacheNodeMessageTypeDef,
@@ -111,18 +110,19 @@
     RevokeCacheSecurityGroupIngressResultTypeDef,
     ServiceUpdatesMessageTypeDef,
     StartMigrationResponseTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
     TestFailoverResultTypeDef,
     TimeRangeFilterTypeDef,
+    TimestampTypeDef,
     UpdateActionResultsMessageTypeDef,
     UpdateActionsMessageTypeDef,
-    UserGroupResponseMetadataTypeDef,
-    UserResponseMetadataTypeDef,
+    UserGroupResponseTypeDef,
+    UserResponseTypeDef,
 )
 from .waiter import (
     CacheClusterAvailableWaiter,
     CacheClusterDeletedWaiter,
     ReplicationGroupAvailableWaiter,
     ReplicationGroupDeletedWaiter,
 )
@@ -431,15 +431,15 @@
         PrimaryClusterId: str = ...,
         AutomaticFailoverEnabled: bool = ...,
         MultiAZEnabled: bool = ...,
         NumCacheClusters: int = ...,
         PreferredCacheClusterAZs: Sequence[str] = ...,
         NumNodeGroups: int = ...,
         ReplicasPerNodeGroup: int = ...,
-        NodeGroupConfiguration: Sequence[NodeGroupConfigurationTypeDef] = ...,
+        NodeGroupConfiguration: Sequence[NodeGroupConfigurationUnionTypeDef] = ...,
         CacheNodeType: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupName: str = ...,
         CacheSubnetGroupName: str = ...,
         CacheSecurityGroupNames: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
@@ -496,30 +496,30 @@
         UserName: str,
         Engine: str,
         AccessString: str,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AuthenticationMode: AuthenticationModeTypeDef = ...
-    ) -> UserResponseMetadataTypeDef:
+    ) -> UserResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_user)
         """
 
     async def create_user_group(
         self,
         *,
         UserGroupId: str,
         Engine: str,
         UserIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> UserGroupResponseMetadataTypeDef:
+    ) -> UserGroupResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_user_group)
         """
 
@@ -628,23 +628,23 @@
         """
         Deletes an existing snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#delete_snapshot)
         """
 
-    async def delete_user(self, *, UserId: str) -> UserResponseMetadataTypeDef:
+    async def delete_user(self, *, UserId: str) -> UserResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Deletes a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#delete_user)
         """
 
-    async def delete_user_group(self, *, UserGroupId: str) -> UserGroupResponseMetadataTypeDef:
+    async def delete_user_group(self, *, UserGroupId: str) -> UserGroupResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Deletes a user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_user_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#delete_user_group)
         """
 
@@ -740,16 +740,16 @@
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
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> EventsMessageTypeDef:
         """
         Returns events related to clusters, cache security groups, and cache parameter
         groups.
@@ -1130,29 +1130,29 @@
         *,
         UserId: str,
         AccessString: str = ...,
         AppendAccessString: str = ...,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
         AuthenticationMode: AuthenticationModeTypeDef = ...
-    ) -> UserResponseMetadataTypeDef:
+    ) -> UserResponseTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_user)
         """
 
     async def modify_user_group(
         self,
         *,
         UserGroupId: str,
         UserIdsToAdd: Sequence[str] = ...,
         UserIdsToRemove: Sequence[str] = ...
-    ) -> UserGroupResponseMetadataTypeDef:
+    ) -> UserGroupResponseTypeDef:
         """
         Changes the list of users that belong to the user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_user_group)
         """
```

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/client.pyi` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("elasticache") as client:
         client: ElastiCacheClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AuthTokenUpdateStrategyTypeType,
     AZModeType,
@@ -94,15 +93,15 @@
     IncreaseReplicaCountResultTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     ModifyCacheClusterResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     ModifyReplicationGroupResultTypeDef,
     ModifyReplicationGroupShardConfigurationResultTypeDef,
-    NodeGroupConfigurationTypeDef,
+    NodeGroupConfigurationUnionTypeDef,
     ParameterNameValueTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     RebootCacheClusterResultTypeDef,
     RegionalConfigurationTypeDef,
     ReplicationGroupMessageTypeDef,
     ReservedCacheNodeMessageTypeDef,
@@ -111,18 +110,19 @@
     RevokeCacheSecurityGroupIngressResultTypeDef,
     ServiceUpdatesMessageTypeDef,
     StartMigrationResponseTypeDef,
     TagListMessageTypeDef,
     TagTypeDef,
     TestFailoverResultTypeDef,
     TimeRangeFilterTypeDef,
+    TimestampTypeDef,
     UpdateActionResultsMessageTypeDef,
     UpdateActionsMessageTypeDef,
-    UserGroupResponseMetadataTypeDef,
-    UserResponseMetadataTypeDef,
+    UserGroupResponseTypeDef,
+    UserResponseTypeDef,
 )
 from .waiter import (
     CacheClusterAvailableWaiter,
     CacheClusterDeletedWaiter,
     ReplicationGroupAvailableWaiter,
     ReplicationGroupDeletedWaiter,
 )
@@ -413,15 +413,15 @@
         PrimaryClusterId: str = ...,
         AutomaticFailoverEnabled: bool = ...,
         MultiAZEnabled: bool = ...,
         NumCacheClusters: int = ...,
         PreferredCacheClusterAZs: Sequence[str] = ...,
         NumNodeGroups: int = ...,
         ReplicasPerNodeGroup: int = ...,
-        NodeGroupConfiguration: Sequence[NodeGroupConfigurationTypeDef] = ...,
+        NodeGroupConfiguration: Sequence[NodeGroupConfigurationUnionTypeDef] = ...,
         CacheNodeType: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupName: str = ...,
         CacheSubnetGroupName: str = ...,
         CacheSecurityGroupNames: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
@@ -476,29 +476,29 @@
         UserName: str,
         Engine: str,
         AccessString: str,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AuthenticationMode: AuthenticationModeTypeDef = ...
-    ) -> UserResponseMetadataTypeDef:
+    ) -> UserResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_user)
         """
     async def create_user_group(
         self,
         *,
         UserGroupId: str,
         Engine: str,
         UserIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> UserGroupResponseMetadataTypeDef:
+    ) -> UserGroupResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Creates a Redis user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.create_user_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#create_user_group)
         """
     async def decrease_node_groups_in_global_replication_group(
@@ -597,22 +597,22 @@
     async def delete_snapshot(self, *, SnapshotName: str) -> DeleteSnapshotResultTypeDef:
         """
         Deletes an existing snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#delete_snapshot)
         """
-    async def delete_user(self, *, UserId: str) -> UserResponseMetadataTypeDef:
+    async def delete_user(self, *, UserId: str) -> UserResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Deletes a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#delete_user)
         """
-    async def delete_user_group(self, *, UserGroupId: str) -> UserGroupResponseMetadataTypeDef:
+    async def delete_user_group(self, *, UserGroupId: str) -> UserGroupResponseTypeDef:
         """
         For Redis engine version 6.0 onwards: Deletes a user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.delete_user_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#delete_user_group)
         """
     async def describe_cache_clusters(
@@ -700,16 +700,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#describe_engine_default_parameters)
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
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> EventsMessageTypeDef:
         """
         Returns events related to clusters, cache security groups, and cache parameter
         groups.
@@ -1067,28 +1067,28 @@
         *,
         UserId: str,
         AccessString: str = ...,
         AppendAccessString: str = ...,
         Passwords: Sequence[str] = ...,
         NoPasswordRequired: bool = ...,
         AuthenticationMode: AuthenticationModeTypeDef = ...
-    ) -> UserResponseMetadataTypeDef:
+    ) -> UserResponseTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_user)
         """
     async def modify_user_group(
         self,
         *,
         UserGroupId: str,
         UserIdsToAdd: Sequence[str] = ...,
         UserIdsToRemove: Sequence[str] = ...
-    ) -> UserGroupResponseMetadataTypeDef:
+    ) -> UserGroupResponseTypeDef:
         """
         Changes the list of users that belong to the user group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Client.modify_user_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/client/#modify_user_group)
         """
     async def purchase_reserved_cache_nodes_offering(
```

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/literals.py` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/literals.pyi` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/paginator.py` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/paginator.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,16 +48,15 @@
         describe_service_updates_paginator: DescribeServiceUpdatesPaginator = client.get_paginator("describe_service_updates")
         describe_snapshots_paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")
         describe_update_actions_paginator: DescribeUpdateActionsPaginator = client.get_paginator("describe_update_actions")
         describe_user_groups_paginator: DescribeUserGroupsPaginator = client.get_paginator("describe_user_groups")
         describe_users_paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import ServiceUpdateStatusType, SourceTypeType, UpdateActionStatusType
 from .type_defs import (
     CacheClusterMessageTypeDef,
@@ -75,14 +74,15 @@
     FilterTypeDef,
     PaginatorConfigTypeDef,
     ReplicationGroupMessageTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     ServiceUpdatesMessageTypeDef,
     TimeRangeFilterTypeDef,
+    TimestampTypeDef,
     UpdateActionsMessageTypeDef,
 )
 
 __all__ = (
     "DescribeCacheClustersPaginator",
     "DescribeCacheEngineVersionsPaginator",
     "DescribeCacheParameterGroupsPaginator",
@@ -121,15 +121,15 @@
 
     def paginate(
         self,
         *,
         CacheClusterId: str = ...,
         ShowCacheNodeInfo: bool = ...,
         ShowCacheClustersNotInReplicationGroups: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CacheClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheclusterspaginator)
         """
 
 
@@ -142,33 +142,30 @@
     def paginate(
         self,
         *,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupFamily: str = ...,
         DefaultOnly: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CacheEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheengineversionspaginator)
         """
 
 
 class DescribeCacheParameterGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameterGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheparametergroupspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        CacheParameterGroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheParameterGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CacheParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheparametergroupspaginator)
         """
 
 
@@ -179,60 +176,60 @@
     """
 
     def paginate(
         self,
         *,
         CacheParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CacheParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheparameterspaginator)
         """
 
 
 class DescribeCacheSecurityGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSecurityGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecachesecuritygroupspaginator)
     """
 
     def paginate(
-        self, *, CacheSecurityGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheSecurityGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CacheSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSecurityGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecachesecuritygroupspaginator)
         """
 
 
 class DescribeCacheSubnetGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSubnetGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecachesubnetgroupspaginator)
     """
 
     def paginate(
-        self, *, CacheSubnetGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheSubnetGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CacheSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecachesubnetgroupspaginator)
         """
 
 
 class DescribeEngineDefaultParametersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEngineDefaultParameters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeenginedefaultparameterspaginator)
     """
 
     def paginate(
-        self, *, CacheParameterGroupFamily: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheParameterGroupFamily: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeenginedefaultparameterspaginator)
         """
 
 
@@ -243,18 +240,18 @@
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
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeeventspaginator)
         """
 
 
@@ -265,30 +262,30 @@
     """
 
     def paginate(
         self,
         *,
         GlobalReplicationGroupId: str = ...,
         ShowMemberInfo: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeGlobalReplicationGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeGlobalReplicationGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeglobalreplicationgroupspaginator)
         """
 
 
 class DescribeReplicationGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReplicationGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describereplicationgroupspaginator)
     """
 
     def paginate(
-        self, *, ReplicationGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReplicationGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ReplicationGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReplicationGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describereplicationgroupspaginator)
         """
 
 
@@ -303,15 +300,15 @@
         *,
         ReservedCacheNodeId: str = ...,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ReservedCacheNodeMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describereservedcachenodespaginator)
         """
 
 
@@ -325,15 +322,15 @@
         self,
         *,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ReservedCacheNodesOfferingMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodesOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describereservedcachenodesofferingspaginator)
         """
 
 
@@ -344,15 +341,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceUpdateName: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ServiceUpdatesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeServiceUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeserviceupdatespaginator)
         """
 
 
@@ -366,15 +363,15 @@
         self,
         *,
         ReplicationGroupId: str = ...,
         CacheClusterId: str = ...,
         SnapshotName: str = ...,
         SnapshotSource: str = ...,
         ShowNodeGroupConfig: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSnapshotsListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describesnapshotspaginator)
         """
 
 
@@ -391,30 +388,30 @@
         ReplicationGroupIds: Sequence[str] = ...,
         CacheClusterIds: Sequence[str] = ...,
         Engine: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
         ServiceUpdateTimeRange: TimeRangeFilterTypeDef = ...,
         UpdateActionStatus: Sequence[UpdateActionStatusType] = ...,
         ShowNodeLevelUpdateStatus: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[UpdateActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUpdateActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeupdateactionspaginator)
         """
 
 
 class DescribeUserGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUserGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeusergroupspaginator)
     """
 
     def paginate(
-        self, *, UserGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeUserGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUserGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeusergroupspaginator)
         """
 
 
@@ -426,13 +423,13 @@
 
     def paginate(
         self,
         *,
         Engine: str = ...,
         UserId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeuserspaginator)
         """
```

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/paginator.pyi` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -48,16 +48,15 @@
         describe_service_updates_paginator: DescribeServiceUpdatesPaginator = client.get_paginator("describe_service_updates")
         describe_snapshots_paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")
         describe_update_actions_paginator: DescribeUpdateActionsPaginator = client.get_paginator("describe_update_actions")
         describe_user_groups_paginator: DescribeUserGroupsPaginator = client.get_paginator("describe_user_groups")
         describe_users_paginator: DescribeUsersPaginator = client.get_paginator("describe_users")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import ServiceUpdateStatusType, SourceTypeType, UpdateActionStatusType
 from .type_defs import (
     CacheClusterMessageTypeDef,
@@ -75,14 +74,15 @@
     FilterTypeDef,
     PaginatorConfigTypeDef,
     ReplicationGroupMessageTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     ServiceUpdatesMessageTypeDef,
     TimeRangeFilterTypeDef,
+    TimestampTypeDef,
     UpdateActionsMessageTypeDef,
 )
 
 __all__ = (
     "DescribeCacheClustersPaginator",
     "DescribeCacheEngineVersionsPaginator",
     "DescribeCacheParameterGroupsPaginator",
@@ -118,15 +118,15 @@
 
     def paginate(
         self,
         *,
         CacheClusterId: str = ...,
         ShowCacheNodeInfo: bool = ...,
         ShowCacheClustersNotInReplicationGroups: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CacheClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheclusterspaginator)
         """
 
 class DescribeCacheEngineVersionsPaginator(AioPaginator):
@@ -138,32 +138,29 @@
     def paginate(
         self,
         *,
         Engine: str = ...,
         EngineVersion: str = ...,
         CacheParameterGroupFamily: str = ...,
         DefaultOnly: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CacheEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheengineversionspaginator)
         """
 
 class DescribeCacheParameterGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameterGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheparametergroupspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        CacheParameterGroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheParameterGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CacheParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheparametergroupspaginator)
         """
 
 class DescribeCacheParametersPaginator(AioPaginator):
@@ -173,57 +170,57 @@
     """
 
     def paginate(
         self,
         *,
         CacheParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CacheParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecacheparameterspaginator)
         """
 
 class DescribeCacheSecurityGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSecurityGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecachesecuritygroupspaginator)
     """
 
     def paginate(
-        self, *, CacheSecurityGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheSecurityGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CacheSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSecurityGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecachesecuritygroupspaginator)
         """
 
 class DescribeCacheSubnetGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSubnetGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecachesubnetgroupspaginator)
     """
 
     def paginate(
-        self, *, CacheSubnetGroupName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheSubnetGroupName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CacheSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeCacheSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describecachesubnetgroupspaginator)
         """
 
 class DescribeEngineDefaultParametersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEngineDefaultParameters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeenginedefaultparameterspaginator)
     """
 
     def paginate(
-        self, *, CacheParameterGroupFamily: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CacheParameterGroupFamily: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEngineDefaultParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEngineDefaultParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeenginedefaultparameterspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -233,18 +230,18 @@
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
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeeventspaginator)
         """
 
 class DescribeGlobalReplicationGroupsPaginator(AioPaginator):
@@ -254,29 +251,29 @@
     """
 
     def paginate(
         self,
         *,
         GlobalReplicationGroupId: str = ...,
         ShowMemberInfo: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeGlobalReplicationGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeGlobalReplicationGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeglobalreplicationgroupspaginator)
         """
 
 class DescribeReplicationGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReplicationGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describereplicationgroupspaginator)
     """
 
     def paginate(
-        self, *, ReplicationGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReplicationGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ReplicationGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReplicationGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describereplicationgroupspaginator)
         """
 
 class DescribeReservedCacheNodesPaginator(AioPaginator):
@@ -290,15 +287,15 @@
         *,
         ReservedCacheNodeId: str = ...,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ReservedCacheNodeMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describereservedcachenodespaginator)
         """
 
 class DescribeReservedCacheNodesOfferingsPaginator(AioPaginator):
@@ -311,15 +308,15 @@
         self,
         *,
         ReservedCacheNodesOfferingId: str = ...,
         CacheNodeType: str = ...,
         Duration: str = ...,
         ProductDescription: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ReservedCacheNodesOfferingMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeReservedCacheNodesOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describereservedcachenodesofferingspaginator)
         """
 
 class DescribeServiceUpdatesPaginator(AioPaginator):
@@ -329,15 +326,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceUpdateName: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ServiceUpdatesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeServiceUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeserviceupdatespaginator)
         """
 
 class DescribeSnapshotsPaginator(AioPaginator):
@@ -350,15 +347,15 @@
         self,
         *,
         ReplicationGroupId: str = ...,
         CacheClusterId: str = ...,
         SnapshotName: str = ...,
         SnapshotSource: str = ...,
         ShowNodeGroupConfig: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSnapshotsListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describesnapshotspaginator)
         """
 
 class DescribeUpdateActionsPaginator(AioPaginator):
@@ -374,29 +371,29 @@
         ReplicationGroupIds: Sequence[str] = ...,
         CacheClusterIds: Sequence[str] = ...,
         Engine: str = ...,
         ServiceUpdateStatus: Sequence[ServiceUpdateStatusType] = ...,
         ServiceUpdateTimeRange: TimeRangeFilterTypeDef = ...,
         UpdateActionStatus: Sequence[UpdateActionStatusType] = ...,
         ShowNodeLevelUpdateStatus: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[UpdateActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUpdateActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeupdateactionspaginator)
         """
 
 class DescribeUserGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUserGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeusergroupspaginator)
     """
 
     def paginate(
-        self, *, UserGroupId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserGroupId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeUserGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUserGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeusergroupspaginator)
         """
 
 class DescribeUsersPaginator(AioPaginator):
@@ -407,13 +404,13 @@
 
     def paginate(
         self,
         *,
         Engine: str = ...,
         UserId: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeUsersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache.Paginator.DescribeUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/paginators/#describeuserspaginator)
         """
```

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/type_defs.py` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_elasticache.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -52,15 +52,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "AllowedNodeTypeModificationsMessageTypeDef",
+    "ResponseMetadataTypeDef",
     "AuthenticationModeTypeDef",
     "AuthenticationTypeDef",
     "AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchApplyUpdateActionMessageRequestTypeDef",
     "BatchStopUpdateActionMessageRequestTypeDef",
     "CacheParameterGroupStatusTypeDef",
@@ -68,184 +68,187 @@
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "SecurityGroupMembershipTypeDef",
     "CacheEngineVersionTypeDef",
     "CacheNodeTypeSpecificValueTypeDef",
     "CacheNodeUpdateStatusTypeDef",
     "ParameterTypeDef",
-    "CacheParameterGroupNameMessageTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
-    "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteCacheClusterMessageRequestTypeDef",
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     "DeleteCacheSecurityGroupMessageRequestTypeDef",
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
     "DeleteGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteReplicationGroupMessageRequestTypeDef",
     "DeleteSnapshotMessageRequestTypeDef",
     "DeleteUserGroupMessageRequestTypeDef",
     "DeleteUserMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCacheClustersMessageRequestTypeDef",
-    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
-    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
-    "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
     "DescribeCacheParametersMessageRequestTypeDef",
-    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
-    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
-    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
-    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
+    "TimestampTypeDef",
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
-    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
     "DescribeReplicationGroupsMessageRequestTypeDef",
-    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
     "DescribeReservedCacheNodesMessageRequestTypeDef",
-    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
-    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
     "DescribeServiceUpdatesMessageRequestTypeDef",
-    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsMessageRequestTypeDef",
-    "TimeRangeFilterTypeDef",
-    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
     "DescribeUserGroupsMessageRequestTypeDef",
     "FilterTypeDef",
     "KinesisFirehoseDestinationDetailsTypeDef",
     "DisassociateGlobalReplicationGroupMessageRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventTypeDef",
     "FailoverGlobalReplicationGroupMessageRequestTypeDef",
     "GlobalNodeGroupTypeDef",
     "GlobalReplicationGroupInfoTypeDef",
     "GlobalReplicationGroupMemberTypeDef",
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
+    "NodeGroupConfigurationOutputTypeDef",
+    "NodeGroupConfigurationTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
-    "PaginatorConfigTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
     "SlotMigrationTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     "ServiceUpdateTypeDef",
     "SubnetOutpostTypeDef",
     "TestFailoverMessageRequestTypeDef",
     "UnprocessedUpdateActionTypeDef",
     "UserGroupPendingChangesTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopySnapshotMessageRequestTypeDef",
     "CreateCacheParameterGroupMessageRequestTypeDef",
     "CreateCacheSecurityGroupMessageRequestTypeDef",
     "CreateCacheSubnetGroupMessageRequestTypeDef",
     "CreateSnapshotMessageRequestTypeDef",
     "CreateUserGroupMessageRequestTypeDef",
     "PurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
+    "AllowedNodeTypeModificationsMessageTypeDef",
+    "CacheParameterGroupNameMessageTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "TagListMessageTypeDef",
     "CreateUserMessageRequestTypeDef",
     "ModifyUserMessageRequestTypeDef",
-    "UserResponseMetadataTypeDef",
+    "UserResponseTypeDef",
     "UserTypeDef",
     "CacheNodeTypeDef",
     "NodeGroupMemberTypeDef",
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
     "CacheSecurityGroupTypeDef",
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
-    "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
-    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
-    "DescribeUpdateActionsMessageRequestTypeDef",
+    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
+    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
+    "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
+    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
+    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
+    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
+    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
+    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
+    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
+    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
+    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
+    "TimeRangeFilterTypeDef",
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     "DescribeUsersMessageRequestTypeDef",
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
+    "NodeSnapshotTypeDef",
+    "NodeGroupConfigurationUnionTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
     "UpdateActionResultsMessageTypeDef",
-    "UserGroupResponseMetadataTypeDef",
+    "UserGroupResponseTypeDef",
     "UserGroupTypeDef",
     "DescribeUsersResultTypeDef",
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
-    "SnapshotTypeDef",
+    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
+    "DescribeUpdateActionsMessageRequestTypeDef",
     "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "DeleteGlobalReplicationGroupResultTypeDef",
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "ModifyGlobalReplicationGroupResultTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
+    "SnapshotTypeDef",
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
-    "CopySnapshotResultTypeDef",
-    "CreateSnapshotResultTypeDef",
-    "DeleteSnapshotResultTypeDef",
-    "DescribeSnapshotsListMessageTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReplicationGroupPendingModifiedValuesTypeDef",
+    "CopySnapshotResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
     "ModifyCacheSubnetGroupResultTypeDef",
     "CacheClusterTypeDef",
     "ReplicationGroupTypeDef",
     "CacheClusterMessageTypeDef",
@@ -270,20 +273,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
-    "AllowedNodeTypeModificationsMessageTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ScaleUpModifications": List[str],
-        "ScaleDownModifications": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AuthenticationModeTypeDef = TypedDict(
     "AuthenticationModeTypeDef",
     {
         "Type": InputAuthenticationTypeType,
@@ -458,22 +463,14 @@
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ChangeType": ChangeTypeType,
     },
     total=False,
 )
 
-CacheParameterGroupNameMessageTypeDef = TypedDict(
-    "CacheParameterGroupNameMessageTypeDef",
-    {
-        "CacheParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CacheParameterGroupTypeDef = TypedDict(
     "CacheParameterGroupTypeDef",
     {
         "CacheParameterGroupName": str,
         "CacheParameterGroupFamily": str,
         "Description": str,
         "IsGlobal": bool,
@@ -561,28 +558,14 @@
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
-NodeGroupConfigurationTypeDef = TypedDict(
-    "NodeGroupConfigurationTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": List[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": List[str],
-    },
-    total=False,
-)
-
 CustomerNodeEndpointTypeDef = TypedDict(
     "CustomerNodeEndpointTypeDef",
     {
         "Address": str,
         "Port": int,
     },
     total=False,
@@ -713,21 +696,20 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef = TypedDict(
-    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CacheClusterId": str,
-        "ShowCacheNodeInfo": bool,
-        "ShowCacheClustersNotInReplicationGroups": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeCacheClustersMessageRequestTypeDef = TypedDict(
     "DescribeCacheClustersMessageRequestTypeDef",
     {
@@ -736,81 +718,37 @@
         "Marker": str,
         "ShowCacheNodeInfo": bool,
         "ShowCacheClustersNotInReplicationGroups": bool,
     },
     total=False,
 )
 
-DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
-    {
-        "Engine": str,
-        "EngineVersion": str,
-        "CacheParameterGroupFamily": str,
-        "DefaultOnly": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheEngineVersionsMessageRequestTypeDef = TypedDict(
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupFamily": str,
         "MaxRecords": int,
         "Marker": str,
         "DefaultOnly": bool,
     },
     total=False,
 )
 
-DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
-    {
-        "CacheParameterGroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    {
-        "CacheParameterGroupName": str,
-    },
-)
-_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
-    _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-    _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeCacheParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeCacheParametersMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
     },
 )
 _OptionalDescribeCacheParametersMessageRequestTypeDef = TypedDict(
@@ -827,74 +765,34 @@
 class DescribeCacheParametersMessageRequestTypeDef(
     _RequiredDescribeCacheParametersMessageRequestTypeDef,
     _OptionalDescribeCacheParametersMessageRequestTypeDef,
 ):
     pass
 
 
-DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
-    {
-        "CacheSecurityGroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
-    {
-        "CacheSubnetGroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
     {
         "CacheSubnetGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "CacheParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
-    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
         "CacheParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
@@ -910,95 +808,36 @@
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "MaxRecords": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
-DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
-    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
-    {
-        "GlobalReplicationGroupId": str,
-        "ShowMemberInfo": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DescribeGlobalReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
         "ShowMemberInfo": bool,
     },
     total=False,
 )
 
-DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef = TypedDict(
-    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
-    {
-        "ReplicationGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationGroupsMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
-    {
-        "ReservedCacheNodeId": str,
-        "ReservedCacheNodesOfferingId": str,
-        "CacheNodeType": str,
-        "Duration": str,
-        "ProductDescription": str,
-        "OfferingType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedCacheNodesMessageRequestTypeDef = TypedDict(
     "DescribeReservedCacheNodesMessageRequestTypeDef",
     {
         "ReservedCacheNodeId": str,
         "ReservedCacheNodesOfferingId": str,
         "CacheNodeType": str,
         "Duration": str,
@@ -1006,107 +845,53 @@
         "OfferingType": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
-    {
-        "ReservedCacheNodesOfferingId": str,
-        "CacheNodeType": str,
-        "Duration": str,
-        "ProductDescription": str,
-        "OfferingType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedCacheNodesOfferingsMessageRequestTypeDef = TypedDict(
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
     {
         "ReservedCacheNodesOfferingId": str,
         "CacheNodeType": str,
         "Duration": str,
         "ProductDescription": str,
         "OfferingType": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef = TypedDict(
-    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
-    {
-        "ServiceUpdateName": str,
-        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeServiceUpdatesMessageRequestTypeDef = TypedDict(
     "DescribeServiceUpdatesMessageRequestTypeDef",
     {
         "ServiceUpdateName": str,
         "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
-    {
-        "ReplicationGroupId": str,
-        "CacheClusterId": str,
-        "SnapshotName": str,
-        "SnapshotSource": str,
-        "ShowNodeGroupConfig": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotsMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "SnapshotName": str,
         "SnapshotSource": str,
         "Marker": str,
         "MaxRecords": int,
         "ShowNodeGroupConfig": bool,
     },
     total=False,
 )
 
-TimeRangeFilterTypeDef = TypedDict(
-    "TimeRangeFilterTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef = TypedDict(
-    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
-    {
-        "UserGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUserGroupsMessageRequestTypeDef = TypedDict(
     "DescribeUserGroupsMessageRequestTypeDef",
     {
         "UserGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1134,21 +919,14 @@
     {
         "GlobalReplicationGroupId": str,
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
@@ -1297,14 +1075,42 @@
 
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
 
+NodeGroupConfigurationOutputTypeDef = TypedDict(
+    "NodeGroupConfigurationOutputTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": List[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": List[str],
+    },
+    total=False,
+)
+
+NodeGroupConfigurationTypeDef = TypedDict(
+    "NodeGroupConfigurationTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": Sequence[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": Sequence[str],
+    },
+    total=False,
+)
+
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1313,24 +1119,14 @@
         "NodeUpdateInitiatedBy": NodeUpdateInitiatedByType,
         "NodeUpdateInitiatedDate": datetime,
         "NodeUpdateStatusModifiedDate": datetime,
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
 ProcessedUpdateActionTypeDef = TypedDict(
     "ProcessedUpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "UpdateActionStatus": UpdateActionStatusType,
@@ -1384,25 +1180,14 @@
     "SlotMigrationTypeDef",
     {
         "ProgressPercentage": float,
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
 RevokeCacheSecurityGroupIngressMessageRequestTypeDef = TypedDict(
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
@@ -1634,19 +1419,43 @@
 class PurchaseReservedCacheNodesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
 ):
     pass
 
 
+AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
+    "AllowedNodeTypeModificationsMessageTypeDef",
+    {
+        "ScaleUpModifications": List[str],
+        "ScaleDownModifications": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CacheParameterGroupNameMessageTypeDef = TypedDict(
+    "CacheParameterGroupNameMessageTypeDef",
+    {
+        "CacheParameterGroupName": str,
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
 TagListMessageTypeDef = TypedDict(
     "TagListMessageTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserMessageRequestTypeDef = TypedDict(
     "_RequiredCreateUserMessageRequestTypeDef",
     {
         "UserId": str,
@@ -1694,27 +1503,27 @@
 
 class ModifyUserMessageRequestTypeDef(
     _RequiredModifyUserMessageRequestTypeDef, _OptionalModifyUserMessageRequestTypeDef
 ):
     pass
 
 
-UserResponseMetadataTypeDef = TypedDict(
-    "UserResponseMetadataTypeDef",
+UserResponseTypeDef = TypedDict(
+    "UserResponseTypeDef",
     {
         "UserId": str,
         "UserName": str,
         "Status": str,
         "Engine": str,
         "MinimumEngineVersion": str,
         "AccessString": str,
         "UserGroupIds": List[str],
         "Authentication": AuthenticationTypeDef,
         "ARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "UserId": str,
@@ -1759,15 +1568,15 @@
 )
 
 CacheEngineVersionMessageTypeDef = TypedDict(
     "CacheEngineVersionMessageTypeDef",
     {
         "Marker": str,
         "CacheEngineVersions": List[CacheEngineVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheNodeTypeSpecificParameterTypeDef = TypedDict(
     "CacheNodeTypeSpecificParameterTypeDef",
     {
         "ParameterName": str,
@@ -1784,23 +1593,23 @@
 )
 
 CacheParameterGroupsMessageTypeDef = TypedDict(
     "CacheParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "CacheParameterGroups": List[CacheParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheParameterGroupResultTypeDef = TypedDict(
     "CreateCacheParameterGroupResultTypeDef",
     {
         "CacheParameterGroup": CacheParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSecurityGroupTypeDef = TypedDict(
     "CacheSecurityGroupTypeDef",
     {
         "OwnerId": str,
@@ -1857,28 +1666,14 @@
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
 
-NodeSnapshotTypeDef = TypedDict(
-    "NodeSnapshotTypeDef",
-    {
-        "CacheClusterId": str,
-        "NodeGroupId": str,
-        "CacheNodeId": str,
-        "NodeGroupConfiguration": NodeGroupConfigurationTypeDef,
-        "CacheSize": str,
-        "CacheNodeCreateTime": datetime,
-        "SnapshotCreateTime": datetime,
-    },
-    total=False,
-)
-
 StartMigrationMessageRequestTypeDef = TypedDict(
     "StartMigrationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
     },
 )
@@ -1927,54 +1722,230 @@
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
-    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
+DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef = TypedDict(
+    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+    {
+        "CacheClusterId": str,
+        "ShowCacheNodeInfo": bool,
+        "ShowCacheClustersNotInReplicationGroups": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
     {
-        "ServiceUpdateName": str,
-        "ReplicationGroupIds": Sequence[str],
-        "CacheClusterIds": Sequence[str],
         "Engine": str,
-        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
-        "UpdateActionStatus": Sequence[UpdateActionStatusType],
-        "ShowNodeLevelUpdateStatus": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "EngineVersion": str,
+        "CacheParameterGroupFamily": str,
+        "DefaultOnly": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeUpdateActionsMessageRequestTypeDef = TypedDict(
-    "DescribeUpdateActionsMessageRequestTypeDef",
+DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
+    {
+        "CacheParameterGroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    {
+        "CacheParameterGroupName": str,
+    },
+)
+_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
+    _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+    _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+):
+    pass
+
+
+DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
+    {
+        "CacheSecurityGroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
+    {
+        "CacheSubnetGroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "CacheParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
+    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+):
+    pass
+
+
+DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
+    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
+    {
+        "GlobalReplicationGroupId": str,
+        "ShowMemberInfo": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef = TypedDict(
+    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
+    {
+        "ReservedCacheNodeId": str,
+        "ReservedCacheNodesOfferingId": str,
+        "CacheNodeType": str,
+        "Duration": str,
+        "ProductDescription": str,
+        "OfferingType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
+    {
+        "ReservedCacheNodesOfferingId": str,
+        "CacheNodeType": str,
+        "Duration": str,
+        "ProductDescription": str,
+        "OfferingType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef = TypedDict(
+    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
     {
         "ServiceUpdateName": str,
-        "ReplicationGroupIds": Sequence[str],
-        "CacheClusterIds": Sequence[str],
-        "Engine": str,
         "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
-        "UpdateActionStatus": Sequence[UpdateActionStatusType],
-        "ShowNodeLevelUpdateStatus": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "CacheClusterId": str,
+        "SnapshotName": str,
+        "SnapshotSource": str,
+        "ShowNodeGroupConfig": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef = TypedDict(
+    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
+    {
+        "UserGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
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
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+TimeRangeFilterTypeDef = TypedDict(
+    "TimeRangeFilterTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 DescribeUsersMessageDescribeUsersPaginateTypeDef = TypedDict(
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     {
         "Engine": str,
         "UserId": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeUsersMessageRequestTypeDef = TypedDict(
     "DescribeUsersMessageRequestTypeDef",
     {
@@ -1997,15 +1968,15 @@
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
 
 GlobalReplicationGroupTypeDef = TypedDict(
     "GlobalReplicationGroupTypeDef",
     {
         "GlobalReplicationGroupId": str,
@@ -2087,14 +2058,31 @@
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
 )
 
+NodeSnapshotTypeDef = TypedDict(
+    "NodeSnapshotTypeDef",
+    {
+        "CacheClusterId": str,
+        "NodeGroupId": str,
+        "CacheNodeId": str,
+        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
+        "CacheSize": str,
+        "CacheNodeCreateTime": datetime,
+        "SnapshotCreateTime": datetime,
+    },
+    total=False,
+)
+
+NodeGroupConfigurationUnionTypeDef = Union[
+    NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef
+]
 NodeGroupUpdateStatusTypeDef = TypedDict(
     "NodeGroupUpdateStatusTypeDef",
     {
         "NodeGroupId": str,
         "NodeGroupMemberUpdateStatus": List[NodeGroupMemberUpdateStatusTypeDef],
     },
     total=False,
@@ -2144,15 +2132,15 @@
 )
 
 ServiceUpdatesMessageTypeDef = TypedDict(
     "ServiceUpdatesMessageTypeDef",
     {
         "Marker": str,
         "ServiceUpdates": List[ServiceUpdateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
@@ -2164,30 +2152,30 @@
 )
 
 UpdateActionResultsMessageTypeDef = TypedDict(
     "UpdateActionResultsMessageTypeDef",
     {
         "ProcessedUpdateActions": List[ProcessedUpdateActionTypeDef],
         "UnprocessedUpdateActions": List[UnprocessedUpdateActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserGroupResponseMetadataTypeDef = TypedDict(
-    "UserGroupResponseMetadataTypeDef",
+UserGroupResponseTypeDef = TypedDict(
+    "UserGroupResponseTypeDef",
     {
         "UserGroupId": str,
         "Status": str,
         "Engine": str,
         "UserIds": List[str],
         "MinimumEngineVersion": str,
         "PendingChanges": UserGroupPendingChangesTypeDef,
         "ReplicationGroups": List[str],
         "ARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserGroupTypeDef = TypedDict(
     "UserGroupTypeDef",
     {
         "UserGroupId": str,
@@ -2203,15 +2191,15 @@
 )
 
 DescribeUsersResultTypeDef = TypedDict(
     "DescribeUsersResultTypeDef",
     {
         "Users": List[UserTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NodeGroupTypeDef = TypedDict(
     "NodeGroupTypeDef",
     {
         "NodeGroupId": str,
@@ -2226,15 +2214,15 @@
 
 CacheParameterGroupDetailsTypeDef = TypedDict(
     "CacheParameterGroupDetailsTypeDef",
     {
         "Marker": str,
         "Parameters": List[ParameterTypeDef],
         "CacheNodeTypeSpecificParameters": List[CacheNodeTypeSpecificParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "CacheParameterGroupFamily": str,
@@ -2245,74 +2233,72 @@
     total=False,
 )
 
 AuthorizeCacheSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSecurityGroupMessageTypeDef = TypedDict(
     "CacheSecurityGroupMessageTypeDef",
     {
         "Marker": str,
         "CacheSecurityGroups": List[CacheSecurityGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheSecurityGroupResultTypeDef = TypedDict(
     "CreateCacheSecurityGroupResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RevokeCacheSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
+DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
+    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     {
-        "SnapshotName": str,
-        "ReplicationGroupId": str,
-        "ReplicationGroupDescription": str,
-        "CacheClusterId": str,
-        "SnapshotStatus": str,
-        "SnapshotSource": str,
-        "CacheNodeType": str,
+        "ServiceUpdateName": str,
+        "ReplicationGroupIds": Sequence[str],
+        "CacheClusterIds": Sequence[str],
         "Engine": str,
-        "EngineVersion": str,
-        "NumCacheNodes": int,
-        "PreferredAvailabilityZone": str,
-        "PreferredOutpostArn": str,
-        "CacheClusterCreateTime": datetime,
-        "PreferredMaintenanceWindow": str,
-        "TopicArn": str,
-        "Port": int,
-        "CacheParameterGroupName": str,
-        "CacheSubnetGroupName": str,
-        "VpcId": str,
-        "AutoMinorVersionUpgrade": bool,
-        "SnapshotRetentionLimit": int,
-        "SnapshotWindow": str,
-        "NumNodeGroups": int,
-        "AutomaticFailover": AutomaticFailoverStatusType,
-        "NodeSnapshots": List[NodeSnapshotTypeDef],
-        "KmsKeyId": str,
-        "ARN": str,
-        "DataTiering": DataTieringStatusType,
+        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
+        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
+        "UpdateActionStatus": Sequence[UpdateActionStatusType],
+        "ShowNodeLevelUpdateStatus": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeUpdateActionsMessageRequestTypeDef = TypedDict(
+    "DescribeUpdateActionsMessageRequestTypeDef",
+    {
+        "ServiceUpdateName": str,
+        "ReplicationGroupIds": Sequence[str],
+        "CacheClusterIds": Sequence[str],
+        "Engine": str,
+        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
+        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
+        "UpdateActionStatus": Sequence[UpdateActionStatusType],
+        "ShowNodeLevelUpdateStatus": bool,
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
 LogDeliveryConfigurationRequestTypeDef = TypedDict(
     "LogDeliveryConfigurationRequestTypeDef",
     {
@@ -2349,80 +2335,80 @@
     total=False,
 )
 
 CreateGlobalReplicationGroupResultTypeDef = TypedDict(
     "CreateGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGlobalReplicationGroupResultTypeDef = TypedDict(
     "DeleteGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGlobalReplicationGroupsResultTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsResultTypeDef",
     {
         "Marker": str,
         "GlobalReplicationGroups": List[GlobalReplicationGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateGlobalReplicationGroupResultTypeDef = TypedDict(
     "DisassociateGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverGlobalReplicationGroupResultTypeDef = TypedDict(
     "FailoverGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyGlobalReplicationGroupResultTypeDef = TypedDict(
     "ModifyGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebalanceSlotsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
@@ -2442,14 +2428,49 @@
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
 
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotName": str,
+        "ReplicationGroupId": str,
+        "ReplicationGroupDescription": str,
+        "CacheClusterId": str,
+        "SnapshotStatus": str,
+        "SnapshotSource": str,
+        "CacheNodeType": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "NumCacheNodes": int,
+        "PreferredAvailabilityZone": str,
+        "PreferredOutpostArn": str,
+        "CacheClusterCreateTime": datetime,
+        "PreferredMaintenanceWindow": str,
+        "TopicArn": str,
+        "Port": int,
+        "CacheParameterGroupName": str,
+        "CacheSubnetGroupName": str,
+        "VpcId": str,
+        "AutoMinorVersionUpgrade": bool,
+        "SnapshotRetentionLimit": int,
+        "SnapshotWindow": str,
+        "NumNodeGroups": int,
+        "AutomaticFailover": AutomaticFailoverStatusType,
+        "NodeSnapshots": List[NodeSnapshotTypeDef],
+        "KmsKeyId": str,
+        "ARN": str,
+        "DataTiering": DataTieringStatusType,
+    },
+    total=False,
+)
+
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2470,33 +2491,33 @@
     total=False,
 )
 
 PurchaseReservedCacheNodesOfferingResultTypeDef = TypedDict(
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     {
         "ReservedCacheNode": ReservedCacheNodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedCacheNodeMessageTypeDef = TypedDict(
     "ReservedCacheNodeMessageTypeDef",
     {
         "Marker": str,
         "ReservedCacheNodes": List[ReservedCacheNodeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedCacheNodesOfferingMessageTypeDef = TypedDict(
     "ReservedCacheNodesOfferingMessageTypeDef",
     {
         "Marker": str,
         "ReservedCacheNodesOfferings": List[ReservedCacheNodesOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSubnetGroupTypeDef = TypedDict(
     "CacheSubnetGroupTypeDef",
     {
         "CacheSubnetGroupName": str,
@@ -2510,56 +2531,23 @@
 )
 
 DescribeUserGroupsResultTypeDef = TypedDict(
     "DescribeUserGroupsResultTypeDef",
     {
         "UserGroups": List[UserGroupTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEngineDefaultParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CopySnapshotResultTypeDef = TypedDict(
-    "CopySnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeSnapshotsListMessageTypeDef = TypedDict(
-    "DescribeSnapshotsListMessageTypeDef",
-    {
-        "Marker": str,
-        "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
@@ -2623,15 +2611,15 @@
         "PrimaryClusterId": str,
         "AutomaticFailoverEnabled": bool,
         "MultiAZEnabled": bool,
         "NumCacheClusters": int,
         "PreferredCacheClusterAZs": Sequence[str],
         "NumNodeGroups": int,
         "ReplicasPerNodeGroup": int,
-        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationTypeDef],
+        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationUnionTypeDef],
         "CacheNodeType": str,
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupName": str,
         "CacheSubnetGroupName": str,
         "CacheSecurityGroupNames": Sequence[str],
         "SecurityGroupIds": Sequence[str],
@@ -2784,45 +2772,78 @@
         "TransitEncryptionEnabled": bool,
         "TransitEncryptionMode": TransitEncryptionModeType,
         "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
+CopySnapshotResultTypeDef = TypedDict(
+    "CopySnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSnapshotsListMessageTypeDef = TypedDict(
+    "DescribeSnapshotsListMessageTypeDef",
+    {
+        "Marker": str,
+        "Snapshots": List[SnapshotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSubnetGroupMessageTypeDef = TypedDict(
     "CacheSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "CacheSubnetGroups": List[CacheSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheSubnetGroupResultTypeDef = TypedDict(
     "CreateCacheSubnetGroupResultTypeDef",
     {
         "CacheSubnetGroup": CacheSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyCacheSubnetGroupResultTypeDef = TypedDict(
     "ModifyCacheSubnetGroupResultTypeDef",
     {
         "CacheSubnetGroup": CacheSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheClusterTypeDef = TypedDict(
     "CacheClusterTypeDef",
     {
         "CacheClusterId": str,
@@ -2901,123 +2922,123 @@
 )
 
 CacheClusterMessageTypeDef = TypedDict(
     "CacheClusterMessageTypeDef",
     {
         "Marker": str,
         "CacheClusters": List[CacheClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheClusterResultTypeDef = TypedDict(
     "CreateCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCacheClusterResultTypeDef = TypedDict(
     "DeleteCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyCacheClusterResultTypeDef = TypedDict(
     "ModifyCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootCacheClusterResultTypeDef = TypedDict(
     "RebootCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompleteMigrationResponseTypeDef = TypedDict(
     "CompleteMigrationResponseTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateReplicationGroupResultTypeDef = TypedDict(
     "CreateReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DecreaseReplicaCountResultTypeDef = TypedDict(
     "DecreaseReplicaCountResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteReplicationGroupResultTypeDef = TypedDict(
     "DeleteReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IncreaseReplicaCountResultTypeDef = TypedDict(
     "IncreaseReplicaCountResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationGroupResultTypeDef = TypedDict(
     "ModifyReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationGroupShardConfigurationResultTypeDef = TypedDict(
     "ModifyReplicationGroupShardConfigurationResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicationGroupMessageTypeDef = TypedDict(
     "ReplicationGroupMessageTypeDef",
     {
         "Marker": str,
         "ReplicationGroups": List[ReplicationGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMigrationResponseTypeDef = TypedDict(
     "StartMigrationResponseTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestFailoverResultTypeDef = TypedDict(
     "TestFailoverResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/type_defs.pyi` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_elasticache.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -51,15 +51,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "AllowedNodeTypeModificationsMessageTypeDef",
+    "ResponseMetadataTypeDef",
     "AuthenticationModeTypeDef",
     "AuthenticationTypeDef",
     "AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchApplyUpdateActionMessageRequestTypeDef",
     "BatchStopUpdateActionMessageRequestTypeDef",
     "CacheParameterGroupStatusTypeDef",
@@ -67,184 +67,187 @@
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "SecurityGroupMembershipTypeDef",
     "CacheEngineVersionTypeDef",
     "CacheNodeTypeSpecificValueTypeDef",
     "CacheNodeUpdateStatusTypeDef",
     "ParameterTypeDef",
-    "CacheParameterGroupNameMessageTypeDef",
     "CacheParameterGroupTypeDef",
     "EC2SecurityGroupTypeDef",
     "CloudWatchLogsDestinationDetailsTypeDef",
     "CompleteMigrationMessageRequestTypeDef",
     "ConfigureShardTypeDef",
     "CreateGlobalReplicationGroupMessageRequestTypeDef",
-    "NodeGroupConfigurationTypeDef",
     "CustomerNodeEndpointTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteCacheClusterMessageRequestTypeDef",
     "DeleteCacheParameterGroupMessageRequestTypeDef",
     "DeleteCacheSecurityGroupMessageRequestTypeDef",
     "DeleteCacheSubnetGroupMessageRequestTypeDef",
     "DeleteGlobalReplicationGroupMessageRequestTypeDef",
     "DeleteReplicationGroupMessageRequestTypeDef",
     "DeleteSnapshotMessageRequestTypeDef",
     "DeleteUserGroupMessageRequestTypeDef",
     "DeleteUserMessageRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeCacheClustersMessageRequestTypeDef",
-    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
-    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
-    "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
     "DescribeCacheParametersMessageRequestTypeDef",
-    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
-    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
-    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
     "DescribeEngineDefaultParametersMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
-    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
+    "TimestampTypeDef",
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
-    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
     "DescribeReplicationGroupsMessageRequestTypeDef",
-    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
     "DescribeReservedCacheNodesMessageRequestTypeDef",
-    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
-    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
     "DescribeServiceUpdatesMessageRequestTypeDef",
-    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsMessageRequestTypeDef",
-    "TimeRangeFilterTypeDef",
-    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
     "DescribeUserGroupsMessageRequestTypeDef",
     "FilterTypeDef",
     "KinesisFirehoseDestinationDetailsTypeDef",
     "DisassociateGlobalReplicationGroupMessageRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EventTypeDef",
     "FailoverGlobalReplicationGroupMessageRequestTypeDef",
     "GlobalNodeGroupTypeDef",
     "GlobalReplicationGroupInfoTypeDef",
     "GlobalReplicationGroupMemberTypeDef",
     "ListAllowedNodeTypeModificationsMessageRequestTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ParameterNameValueTypeDef",
     "ModifyCacheSubnetGroupMessageRequestTypeDef",
     "ModifyGlobalReplicationGroupMessageRequestTypeDef",
     "ReshardingConfigurationTypeDef",
     "ModifyUserGroupMessageRequestTypeDef",
+    "NodeGroupConfigurationOutputTypeDef",
+    "NodeGroupConfigurationTypeDef",
     "NodeGroupMemberUpdateStatusTypeDef",
-    "PaginatorConfigTypeDef",
     "ProcessedUpdateActionTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef",
     "RebootCacheClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "UserGroupsUpdateStatusTypeDef",
     "SlotMigrationTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     "ServiceUpdateTypeDef",
     "SubnetOutpostTypeDef",
     "TestFailoverMessageRequestTypeDef",
     "UnprocessedUpdateActionTypeDef",
     "UserGroupPendingChangesTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CopySnapshotMessageRequestTypeDef",
     "CreateCacheParameterGroupMessageRequestTypeDef",
     "CreateCacheSecurityGroupMessageRequestTypeDef",
     "CreateCacheSubnetGroupMessageRequestTypeDef",
     "CreateSnapshotMessageRequestTypeDef",
     "CreateUserGroupMessageRequestTypeDef",
     "PurchaseReservedCacheNodesOfferingMessageRequestTypeDef",
+    "AllowedNodeTypeModificationsMessageTypeDef",
+    "CacheParameterGroupNameMessageTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "TagListMessageTypeDef",
     "CreateUserMessageRequestTypeDef",
     "ModifyUserMessageRequestTypeDef",
-    "UserResponseMetadataTypeDef",
+    "UserResponseTypeDef",
     "UserTypeDef",
     "CacheNodeTypeDef",
     "NodeGroupMemberTypeDef",
     "CacheEngineVersionMessageTypeDef",
     "CacheNodeTypeSpecificParameterTypeDef",
     "CacheParameterGroupsMessageTypeDef",
     "CreateCacheParameterGroupResultTypeDef",
     "CacheSecurityGroupTypeDef",
     "DecreaseReplicaCountMessageRequestTypeDef",
     "IncreaseReplicaCountMessageRequestTypeDef",
-    "NodeSnapshotTypeDef",
     "StartMigrationMessageRequestTypeDef",
     "DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef",
     "DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef",
     "DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef",
-    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
-    "DescribeUpdateActionsMessageRequestTypeDef",
+    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
+    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
+    "DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
+    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
+    "DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
+    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
+    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
+    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
+    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
+    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
+    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
+    "TimeRangeFilterTypeDef",
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     "DescribeUsersMessageRequestTypeDef",
     "DestinationDetailsTypeDef",
     "EventsMessageTypeDef",
     "GlobalReplicationGroupTypeDef",
     "ModifyCacheParameterGroupMessageRequestTypeDef",
     "ResetCacheParameterGroupMessageRequestTypeDef",
     "ModifyReplicationGroupShardConfigurationMessageRequestTypeDef",
     "RegionalConfigurationTypeDef",
+    "NodeSnapshotTypeDef",
+    "NodeGroupConfigurationUnionTypeDef",
     "NodeGroupUpdateStatusTypeDef",
     "ReservedCacheNodeTypeDef",
     "ReservedCacheNodesOfferingTypeDef",
     "ReshardingStatusTypeDef",
     "ServiceUpdatesMessageTypeDef",
     "SubnetTypeDef",
     "UpdateActionResultsMessageTypeDef",
-    "UserGroupResponseMetadataTypeDef",
+    "UserGroupResponseTypeDef",
     "UserGroupTypeDef",
     "DescribeUsersResultTypeDef",
     "NodeGroupTypeDef",
     "CacheParameterGroupDetailsTypeDef",
     "EngineDefaultsTypeDef",
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     "CacheSecurityGroupMessageTypeDef",
     "CreateCacheSecurityGroupResultTypeDef",
     "RevokeCacheSecurityGroupIngressResultTypeDef",
-    "SnapshotTypeDef",
+    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
+    "DescribeUpdateActionsMessageRequestTypeDef",
     "LogDeliveryConfigurationRequestTypeDef",
     "LogDeliveryConfigurationTypeDef",
     "PendingLogDeliveryConfigurationTypeDef",
     "CreateGlobalReplicationGroupResultTypeDef",
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "DeleteGlobalReplicationGroupResultTypeDef",
     "DescribeGlobalReplicationGroupsResultTypeDef",
     "DisassociateGlobalReplicationGroupResultTypeDef",
     "FailoverGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     "ModifyGlobalReplicationGroupResultTypeDef",
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     "IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
+    "SnapshotTypeDef",
     "UpdateActionTypeDef",
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     "ReservedCacheNodeMessageTypeDef",
     "ReservedCacheNodesOfferingMessageTypeDef",
     "CacheSubnetGroupTypeDef",
     "DescribeUserGroupsResultTypeDef",
     "DescribeEngineDefaultParametersResultTypeDef",
-    "CopySnapshotResultTypeDef",
-    "CreateSnapshotResultTypeDef",
-    "DeleteSnapshotResultTypeDef",
-    "DescribeSnapshotsListMessageTypeDef",
     "CreateCacheClusterMessageRequestTypeDef",
     "CreateReplicationGroupMessageRequestTypeDef",
     "ModifyCacheClusterMessageRequestTypeDef",
     "ModifyReplicationGroupMessageRequestTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReplicationGroupPendingModifiedValuesTypeDef",
+    "CopySnapshotResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DescribeSnapshotsListMessageTypeDef",
     "UpdateActionsMessageTypeDef",
     "CacheSubnetGroupMessageTypeDef",
     "CreateCacheSubnetGroupResultTypeDef",
     "ModifyCacheSubnetGroupResultTypeDef",
     "CacheClusterTypeDef",
     "ReplicationGroupTypeDef",
     "CacheClusterMessageTypeDef",
@@ -269,20 +272,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
-    "AllowedNodeTypeModificationsMessageTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ScaleUpModifications": List[str],
-        "ScaleDownModifications": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AuthenticationModeTypeDef = TypedDict(
     "AuthenticationModeTypeDef",
     {
         "Type": InputAuthenticationTypeType,
@@ -453,22 +458,14 @@
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
         "ChangeType": ChangeTypeType,
     },
     total=False,
 )
 
-CacheParameterGroupNameMessageTypeDef = TypedDict(
-    "CacheParameterGroupNameMessageTypeDef",
-    {
-        "CacheParameterGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CacheParameterGroupTypeDef = TypedDict(
     "CacheParameterGroupTypeDef",
     {
         "CacheParameterGroupName": str,
         "CacheParameterGroupFamily": str,
         "Description": str,
         "IsGlobal": bool,
@@ -550,28 +547,14 @@
 
 class CreateGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredCreateGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalCreateGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
-NodeGroupConfigurationTypeDef = TypedDict(
-    "NodeGroupConfigurationTypeDef",
-    {
-        "NodeGroupId": str,
-        "Slots": str,
-        "ReplicaCount": int,
-        "PrimaryAvailabilityZone": str,
-        "ReplicaAvailabilityZones": List[str],
-        "PrimaryOutpostArn": str,
-        "ReplicaOutpostArns": List[str],
-    },
-    total=False,
-)
-
 CustomerNodeEndpointTypeDef = TypedDict(
     "CustomerNodeEndpointTypeDef",
     {
         "Address": str,
         "Port": int,
     },
     total=False,
@@ -696,21 +679,20 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef = TypedDict(
-    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CacheClusterId": str,
-        "ShowCacheNodeInfo": bool,
-        "ShowCacheClustersNotInReplicationGroups": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeCacheClustersMessageRequestTypeDef = TypedDict(
     "DescribeCacheClustersMessageRequestTypeDef",
     {
@@ -719,79 +701,37 @@
         "Marker": str,
         "ShowCacheNodeInfo": bool,
         "ShowCacheClustersNotInReplicationGroups": bool,
     },
     total=False,
 )
 
-DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef = TypedDict(
-    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
-    {
-        "Engine": str,
-        "EngineVersion": str,
-        "CacheParameterGroupFamily": str,
-        "DefaultOnly": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheEngineVersionsMessageRequestTypeDef = TypedDict(
     "DescribeCacheEngineVersionsMessageRequestTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupFamily": str,
         "MaxRecords": int,
         "Marker": str,
         "DefaultOnly": bool,
     },
     total=False,
 )
 
-DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
-    {
-        "CacheParameterGroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheParameterGroupsMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    {
-        "CacheParameterGroupName": str,
-    },
-)
-_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
-    _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-    _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeCacheParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeCacheParametersMessageRequestTypeDef",
     {
         "CacheParameterGroupName": str,
     },
 )
 _OptionalDescribeCacheParametersMessageRequestTypeDef = TypedDict(
@@ -806,72 +746,34 @@
 
 class DescribeCacheParametersMessageRequestTypeDef(
     _RequiredDescribeCacheParametersMessageRequestTypeDef,
     _OptionalDescribeCacheParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
-    {
-        "CacheSecurityGroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSecurityGroupsMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
-    {
-        "CacheSubnetGroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCacheSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeCacheSubnetGroupsMessageRequestTypeDef",
     {
         "CacheSubnetGroupName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "CacheParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef(
-    _RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-    _OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeEngineDefaultParametersMessageRequestTypeDef",
     {
         "CacheParameterGroupFamily": str,
     },
 )
 _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef = TypedDict(
@@ -885,95 +787,36 @@
 
 class DescribeEngineDefaultParametersMessageRequestTypeDef(
     _RequiredDescribeEngineDefaultParametersMessageRequestTypeDef,
     _OptionalDescribeEngineDefaultParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "MaxRecords": int,
-        "Marker": str,
-    },
-    total=False,
-)
-
-DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
-    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
-    {
-        "GlobalReplicationGroupId": str,
-        "ShowMemberInfo": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 DescribeGlobalReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
         "ShowMemberInfo": bool,
     },
     total=False,
 )
 
-DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef = TypedDict(
-    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
-    {
-        "ReplicationGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReplicationGroupsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationGroupsMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
-    {
-        "ReservedCacheNodeId": str,
-        "ReservedCacheNodesOfferingId": str,
-        "CacheNodeType": str,
-        "Duration": str,
-        "ProductDescription": str,
-        "OfferingType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedCacheNodesMessageRequestTypeDef = TypedDict(
     "DescribeReservedCacheNodesMessageRequestTypeDef",
     {
         "ReservedCacheNodeId": str,
         "ReservedCacheNodesOfferingId": str,
         "CacheNodeType": str,
         "Duration": str,
@@ -981,107 +824,53 @@
         "OfferingType": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
-    {
-        "ReservedCacheNodesOfferingId": str,
-        "CacheNodeType": str,
-        "Duration": str,
-        "ProductDescription": str,
-        "OfferingType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedCacheNodesOfferingsMessageRequestTypeDef = TypedDict(
     "DescribeReservedCacheNodesOfferingsMessageRequestTypeDef",
     {
         "ReservedCacheNodesOfferingId": str,
         "CacheNodeType": str,
         "Duration": str,
         "ProductDescription": str,
         "OfferingType": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef = TypedDict(
-    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
-    {
-        "ServiceUpdateName": str,
-        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeServiceUpdatesMessageRequestTypeDef = TypedDict(
     "DescribeServiceUpdatesMessageRequestTypeDef",
     {
         "ServiceUpdateName": str,
         "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
-    {
-        "ReplicationGroupId": str,
-        "CacheClusterId": str,
-        "SnapshotName": str,
-        "SnapshotSource": str,
-        "ShowNodeGroupConfig": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotsMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "SnapshotName": str,
         "SnapshotSource": str,
         "Marker": str,
         "MaxRecords": int,
         "ShowNodeGroupConfig": bool,
     },
     total=False,
 )
 
-TimeRangeFilterTypeDef = TypedDict(
-    "TimeRangeFilterTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef = TypedDict(
-    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
-    {
-        "UserGroupId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUserGroupsMessageRequestTypeDef = TypedDict(
     "DescribeUserGroupsMessageRequestTypeDef",
     {
         "UserGroupId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1109,21 +898,14 @@
     {
         "GlobalReplicationGroupId": str,
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
@@ -1266,14 +1048,42 @@
 )
 
 class ModifyUserGroupMessageRequestTypeDef(
     _RequiredModifyUserGroupMessageRequestTypeDef, _OptionalModifyUserGroupMessageRequestTypeDef
 ):
     pass
 
+NodeGroupConfigurationOutputTypeDef = TypedDict(
+    "NodeGroupConfigurationOutputTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": List[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": List[str],
+    },
+    total=False,
+)
+
+NodeGroupConfigurationTypeDef = TypedDict(
+    "NodeGroupConfigurationTypeDef",
+    {
+        "NodeGroupId": str,
+        "Slots": str,
+        "ReplicaCount": int,
+        "PrimaryAvailabilityZone": str,
+        "ReplicaAvailabilityZones": Sequence[str],
+        "PrimaryOutpostArn": str,
+        "ReplicaOutpostArns": Sequence[str],
+    },
+    total=False,
+)
+
 NodeGroupMemberUpdateStatusTypeDef = TypedDict(
     "NodeGroupMemberUpdateStatusTypeDef",
     {
         "CacheClusterId": str,
         "CacheNodeId": str,
         "NodeUpdateStatus": NodeUpdateStatusType,
         "NodeDeletionDate": datetime,
@@ -1282,24 +1092,14 @@
         "NodeUpdateInitiatedBy": NodeUpdateInitiatedByType,
         "NodeUpdateInitiatedDate": datetime,
         "NodeUpdateStatusModifiedDate": datetime,
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
 ProcessedUpdateActionTypeDef = TypedDict(
     "ProcessedUpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "UpdateActionStatus": UpdateActionStatusType,
@@ -1353,25 +1153,14 @@
     "SlotMigrationTypeDef",
     {
         "ProgressPercentage": float,
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
 RevokeCacheSecurityGroupIngressMessageRequestTypeDef = TypedDict(
     "RevokeCacheSecurityGroupIngressMessageRequestTypeDef",
     {
         "CacheSecurityGroupName": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
@@ -1589,19 +1378,43 @@
 
 class PurchaseReservedCacheNodesOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
 ):
     pass
 
+AllowedNodeTypeModificationsMessageTypeDef = TypedDict(
+    "AllowedNodeTypeModificationsMessageTypeDef",
+    {
+        "ScaleUpModifications": List[str],
+        "ScaleDownModifications": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CacheParameterGroupNameMessageTypeDef = TypedDict(
+    "CacheParameterGroupNameMessageTypeDef",
+    {
+        "CacheParameterGroupName": str,
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
 TagListMessageTypeDef = TypedDict(
     "TagListMessageTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserMessageRequestTypeDef = TypedDict(
     "_RequiredCreateUserMessageRequestTypeDef",
     {
         "UserId": str,
@@ -1645,27 +1458,27 @@
 )
 
 class ModifyUserMessageRequestTypeDef(
     _RequiredModifyUserMessageRequestTypeDef, _OptionalModifyUserMessageRequestTypeDef
 ):
     pass
 
-UserResponseMetadataTypeDef = TypedDict(
-    "UserResponseMetadataTypeDef",
+UserResponseTypeDef = TypedDict(
+    "UserResponseTypeDef",
     {
         "UserId": str,
         "UserName": str,
         "Status": str,
         "Engine": str,
         "MinimumEngineVersion": str,
         "AccessString": str,
         "UserGroupIds": List[str],
         "Authentication": AuthenticationTypeDef,
         "ARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "UserId": str,
@@ -1710,15 +1523,15 @@
 )
 
 CacheEngineVersionMessageTypeDef = TypedDict(
     "CacheEngineVersionMessageTypeDef",
     {
         "Marker": str,
         "CacheEngineVersions": List[CacheEngineVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheNodeTypeSpecificParameterTypeDef = TypedDict(
     "CacheNodeTypeSpecificParameterTypeDef",
     {
         "ParameterName": str,
@@ -1735,23 +1548,23 @@
 )
 
 CacheParameterGroupsMessageTypeDef = TypedDict(
     "CacheParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "CacheParameterGroups": List[CacheParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheParameterGroupResultTypeDef = TypedDict(
     "CreateCacheParameterGroupResultTypeDef",
     {
         "CacheParameterGroup": CacheParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSecurityGroupTypeDef = TypedDict(
     "CacheSecurityGroupTypeDef",
     {
         "OwnerId": str,
@@ -1804,28 +1617,14 @@
 
 class IncreaseReplicaCountMessageRequestTypeDef(
     _RequiredIncreaseReplicaCountMessageRequestTypeDef,
     _OptionalIncreaseReplicaCountMessageRequestTypeDef,
 ):
     pass
 
-NodeSnapshotTypeDef = TypedDict(
-    "NodeSnapshotTypeDef",
-    {
-        "CacheClusterId": str,
-        "NodeGroupId": str,
-        "CacheNodeId": str,
-        "NodeGroupConfiguration": NodeGroupConfigurationTypeDef,
-        "CacheSize": str,
-        "CacheNodeCreateTime": datetime,
-        "SnapshotCreateTime": datetime,
-    },
-    total=False,
-)
-
 StartMigrationMessageRequestTypeDef = TypedDict(
     "StartMigrationMessageRequestTypeDef",
     {
         "ReplicationGroupId": str,
         "CustomerNodeEndpointList": Sequence[CustomerNodeEndpointTypeDef],
     },
 )
@@ -1874,54 +1673,226 @@
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
-    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
+DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef = TypedDict(
+    "DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef",
+    {
+        "CacheClusterId": str,
+        "ShowCacheNodeInfo": bool,
+        "ShowCacheClustersNotInReplicationGroups": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef = TypedDict(
+    "DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef",
     {
-        "ServiceUpdateName": str,
-        "ReplicationGroupIds": Sequence[str],
-        "CacheClusterIds": Sequence[str],
         "Engine": str,
-        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
-        "UpdateActionStatus": Sequence[UpdateActionStatusType],
-        "ShowNodeLevelUpdateStatus": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "EngineVersion": str,
+        "CacheParameterGroupFamily": str,
+        "DefaultOnly": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeUpdateActionsMessageRequestTypeDef = TypedDict(
-    "DescribeUpdateActionsMessageRequestTypeDef",
+DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef",
+    {
+        "CacheParameterGroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    {
+        "CacheParameterGroupName": str,
+    },
+)
+_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef(
+    _RequiredDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+    _OptionalDescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+):
+    pass
+
+DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef",
+    {
+        "CacheSecurityGroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef",
+    {
+        "CacheSubnetGroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
+        "CacheParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef",
+    {
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
+DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef = TypedDict(
+    "DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef",
+    {
+        "GlobalReplicationGroupId": str,
+        "ShowMemberInfo": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef = TypedDict(
+    "DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef",
+    {
+        "ReservedCacheNodeId": str,
+        "ReservedCacheNodesOfferingId": str,
+        "CacheNodeType": str,
+        "Duration": str,
+        "ProductDescription": str,
+        "OfferingType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef",
+    {
+        "ReservedCacheNodesOfferingId": str,
+        "CacheNodeType": str,
+        "Duration": str,
+        "ProductDescription": str,
+        "OfferingType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef = TypedDict(
+    "DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef",
     {
         "ServiceUpdateName": str,
-        "ReplicationGroupIds": Sequence[str],
-        "CacheClusterIds": Sequence[str],
-        "Engine": str,
         "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
-        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
-        "UpdateActionStatus": Sequence[UpdateActionStatusType],
-        "ShowNodeLevelUpdateStatus": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef",
+    {
+        "ReplicationGroupId": str,
+        "CacheClusterId": str,
+        "SnapshotName": str,
+        "SnapshotSource": str,
+        "ShowNodeGroupConfig": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef = TypedDict(
+    "DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef",
+    {
+        "UserGroupId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": SourceTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
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
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+TimeRangeFilterTypeDef = TypedDict(
+    "TimeRangeFilterTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 DescribeUsersMessageDescribeUsersPaginateTypeDef = TypedDict(
     "DescribeUsersMessageDescribeUsersPaginateTypeDef",
     {
         "Engine": str,
         "UserId": str,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeUsersMessageRequestTypeDef = TypedDict(
     "DescribeUsersMessageRequestTypeDef",
     {
@@ -1944,15 +1915,15 @@
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
 
 GlobalReplicationGroupTypeDef = TypedDict(
     "GlobalReplicationGroupTypeDef",
     {
         "GlobalReplicationGroupId": str,
@@ -2030,14 +2001,31 @@
     {
         "ReplicationGroupId": str,
         "ReplicationGroupRegion": str,
         "ReshardingConfiguration": Sequence[ReshardingConfigurationTypeDef],
     },
 )
 
+NodeSnapshotTypeDef = TypedDict(
+    "NodeSnapshotTypeDef",
+    {
+        "CacheClusterId": str,
+        "NodeGroupId": str,
+        "CacheNodeId": str,
+        "NodeGroupConfiguration": NodeGroupConfigurationOutputTypeDef,
+        "CacheSize": str,
+        "CacheNodeCreateTime": datetime,
+        "SnapshotCreateTime": datetime,
+    },
+    total=False,
+)
+
+NodeGroupConfigurationUnionTypeDef = Union[
+    NodeGroupConfigurationTypeDef, NodeGroupConfigurationOutputTypeDef
+]
 NodeGroupUpdateStatusTypeDef = TypedDict(
     "NodeGroupUpdateStatusTypeDef",
     {
         "NodeGroupId": str,
         "NodeGroupMemberUpdateStatus": List[NodeGroupMemberUpdateStatusTypeDef],
     },
     total=False,
@@ -2087,15 +2075,15 @@
 )
 
 ServiceUpdatesMessageTypeDef = TypedDict(
     "ServiceUpdatesMessageTypeDef",
     {
         "Marker": str,
         "ServiceUpdates": List[ServiceUpdateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
@@ -2107,30 +2095,30 @@
 )
 
 UpdateActionResultsMessageTypeDef = TypedDict(
     "UpdateActionResultsMessageTypeDef",
     {
         "ProcessedUpdateActions": List[ProcessedUpdateActionTypeDef],
         "UnprocessedUpdateActions": List[UnprocessedUpdateActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserGroupResponseMetadataTypeDef = TypedDict(
-    "UserGroupResponseMetadataTypeDef",
+UserGroupResponseTypeDef = TypedDict(
+    "UserGroupResponseTypeDef",
     {
         "UserGroupId": str,
         "Status": str,
         "Engine": str,
         "UserIds": List[str],
         "MinimumEngineVersion": str,
         "PendingChanges": UserGroupPendingChangesTypeDef,
         "ReplicationGroups": List[str],
         "ARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserGroupTypeDef = TypedDict(
     "UserGroupTypeDef",
     {
         "UserGroupId": str,
@@ -2146,15 +2134,15 @@
 )
 
 DescribeUsersResultTypeDef = TypedDict(
     "DescribeUsersResultTypeDef",
     {
         "Users": List[UserTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NodeGroupTypeDef = TypedDict(
     "NodeGroupTypeDef",
     {
         "NodeGroupId": str,
@@ -2169,15 +2157,15 @@
 
 CacheParameterGroupDetailsTypeDef = TypedDict(
     "CacheParameterGroupDetailsTypeDef",
     {
         "Marker": str,
         "Parameters": List[ParameterTypeDef],
         "CacheNodeTypeSpecificParameters": List[CacheNodeTypeSpecificParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EngineDefaultsTypeDef = TypedDict(
     "EngineDefaultsTypeDef",
     {
         "CacheParameterGroupFamily": str,
@@ -2188,74 +2176,72 @@
     total=False,
 )
 
 AuthorizeCacheSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSecurityGroupMessageTypeDef = TypedDict(
     "CacheSecurityGroupMessageTypeDef",
     {
         "Marker": str,
         "CacheSecurityGroups": List[CacheSecurityGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheSecurityGroupResultTypeDef = TypedDict(
     "CreateCacheSecurityGroupResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RevokeCacheSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeCacheSecurityGroupIngressResultTypeDef",
     {
         "CacheSecurityGroup": CacheSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
+DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef = TypedDict(
+    "DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef",
     {
-        "SnapshotName": str,
-        "ReplicationGroupId": str,
-        "ReplicationGroupDescription": str,
-        "CacheClusterId": str,
-        "SnapshotStatus": str,
-        "SnapshotSource": str,
-        "CacheNodeType": str,
+        "ServiceUpdateName": str,
+        "ReplicationGroupIds": Sequence[str],
+        "CacheClusterIds": Sequence[str],
         "Engine": str,
-        "EngineVersion": str,
-        "NumCacheNodes": int,
-        "PreferredAvailabilityZone": str,
-        "PreferredOutpostArn": str,
-        "CacheClusterCreateTime": datetime,
-        "PreferredMaintenanceWindow": str,
-        "TopicArn": str,
-        "Port": int,
-        "CacheParameterGroupName": str,
-        "CacheSubnetGroupName": str,
-        "VpcId": str,
-        "AutoMinorVersionUpgrade": bool,
-        "SnapshotRetentionLimit": int,
-        "SnapshotWindow": str,
-        "NumNodeGroups": int,
-        "AutomaticFailover": AutomaticFailoverStatusType,
-        "NodeSnapshots": List[NodeSnapshotTypeDef],
-        "KmsKeyId": str,
-        "ARN": str,
-        "DataTiering": DataTieringStatusType,
+        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
+        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
+        "UpdateActionStatus": Sequence[UpdateActionStatusType],
+        "ShowNodeLevelUpdateStatus": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeUpdateActionsMessageRequestTypeDef = TypedDict(
+    "DescribeUpdateActionsMessageRequestTypeDef",
+    {
+        "ServiceUpdateName": str,
+        "ReplicationGroupIds": Sequence[str],
+        "CacheClusterIds": Sequence[str],
+        "Engine": str,
+        "ServiceUpdateStatus": Sequence[ServiceUpdateStatusType],
+        "ServiceUpdateTimeRange": TimeRangeFilterTypeDef,
+        "UpdateActionStatus": Sequence[UpdateActionStatusType],
+        "ShowNodeLevelUpdateStatus": bool,
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
 LogDeliveryConfigurationRequestTypeDef = TypedDict(
     "LogDeliveryConfigurationRequestTypeDef",
     {
@@ -2292,80 +2278,80 @@
     total=False,
 )
 
 CreateGlobalReplicationGroupResultTypeDef = TypedDict(
     "CreateGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGlobalReplicationGroupResultTypeDef = TypedDict(
     "DeleteGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGlobalReplicationGroupsResultTypeDef = TypedDict(
     "DescribeGlobalReplicationGroupsResultTypeDef",
     {
         "Marker": str,
         "GlobalReplicationGroups": List[GlobalReplicationGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateGlobalReplicationGroupResultTypeDef = TypedDict(
     "DisassociateGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailoverGlobalReplicationGroupResultTypeDef = TypedDict(
     "FailoverGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyGlobalReplicationGroupResultTypeDef = TypedDict(
     "ModifyGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebalanceSlotsInGlobalReplicationGroupResultTypeDef = TypedDict(
     "RebalanceSlotsInGlobalReplicationGroupResultTypeDef",
     {
         "GlobalReplicationGroup": GlobalReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef = TypedDict(
     "_RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef",
     {
         "GlobalReplicationGroupId": str,
@@ -2383,14 +2369,49 @@
 
 class IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef(
     _RequiredIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     _OptionalIncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
 ):
     pass
 
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotName": str,
+        "ReplicationGroupId": str,
+        "ReplicationGroupDescription": str,
+        "CacheClusterId": str,
+        "SnapshotStatus": str,
+        "SnapshotSource": str,
+        "CacheNodeType": str,
+        "Engine": str,
+        "EngineVersion": str,
+        "NumCacheNodes": int,
+        "PreferredAvailabilityZone": str,
+        "PreferredOutpostArn": str,
+        "CacheClusterCreateTime": datetime,
+        "PreferredMaintenanceWindow": str,
+        "TopicArn": str,
+        "Port": int,
+        "CacheParameterGroupName": str,
+        "CacheSubnetGroupName": str,
+        "VpcId": str,
+        "AutoMinorVersionUpgrade": bool,
+        "SnapshotRetentionLimit": int,
+        "SnapshotWindow": str,
+        "NumNodeGroups": int,
+        "AutomaticFailover": AutomaticFailoverStatusType,
+        "NodeSnapshots": List[NodeSnapshotTypeDef],
+        "KmsKeyId": str,
+        "ARN": str,
+        "DataTiering": DataTieringStatusType,
+    },
+    total=False,
+)
+
 UpdateActionTypeDef = TypedDict(
     "UpdateActionTypeDef",
     {
         "ReplicationGroupId": str,
         "CacheClusterId": str,
         "ServiceUpdateName": str,
         "ServiceUpdateReleaseDate": datetime,
@@ -2411,33 +2432,33 @@
     total=False,
 )
 
 PurchaseReservedCacheNodesOfferingResultTypeDef = TypedDict(
     "PurchaseReservedCacheNodesOfferingResultTypeDef",
     {
         "ReservedCacheNode": ReservedCacheNodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedCacheNodeMessageTypeDef = TypedDict(
     "ReservedCacheNodeMessageTypeDef",
     {
         "Marker": str,
         "ReservedCacheNodes": List[ReservedCacheNodeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedCacheNodesOfferingMessageTypeDef = TypedDict(
     "ReservedCacheNodesOfferingMessageTypeDef",
     {
         "Marker": str,
         "ReservedCacheNodesOfferings": List[ReservedCacheNodesOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSubnetGroupTypeDef = TypedDict(
     "CacheSubnetGroupTypeDef",
     {
         "CacheSubnetGroupName": str,
@@ -2451,56 +2472,23 @@
 )
 
 DescribeUserGroupsResultTypeDef = TypedDict(
     "DescribeUserGroupsResultTypeDef",
     {
         "UserGroups": List[UserGroupTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEngineDefaultParametersResultTypeDef = TypedDict(
     "DescribeEngineDefaultParametersResultTypeDef",
     {
         "EngineDefaults": EngineDefaultsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CopySnapshotResultTypeDef = TypedDict(
-    "CopySnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeSnapshotsListMessageTypeDef = TypedDict(
-    "DescribeSnapshotsListMessageTypeDef",
-    {
-        "Marker": str,
-        "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCacheClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateCacheClusterMessageRequestTypeDef",
     {
         "CacheClusterId": str,
@@ -2562,15 +2550,15 @@
         "PrimaryClusterId": str,
         "AutomaticFailoverEnabled": bool,
         "MultiAZEnabled": bool,
         "NumCacheClusters": int,
         "PreferredCacheClusterAZs": Sequence[str],
         "NumNodeGroups": int,
         "ReplicasPerNodeGroup": int,
-        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationTypeDef],
+        "NodeGroupConfiguration": Sequence[NodeGroupConfigurationUnionTypeDef],
         "CacheNodeType": str,
         "Engine": str,
         "EngineVersion": str,
         "CacheParameterGroupName": str,
         "CacheSubnetGroupName": str,
         "CacheSecurityGroupNames": Sequence[str],
         "SecurityGroupIds": Sequence[str],
@@ -2717,45 +2705,78 @@
         "TransitEncryptionEnabled": bool,
         "TransitEncryptionMode": TransitEncryptionModeType,
         "ClusterMode": ClusterModeType,
     },
     total=False,
 )
 
+CopySnapshotResultTypeDef = TypedDict(
+    "CopySnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "Snapshot": SnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSnapshotsListMessageTypeDef = TypedDict(
+    "DescribeSnapshotsListMessageTypeDef",
+    {
+        "Marker": str,
+        "Snapshots": List[SnapshotTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateActionsMessageTypeDef = TypedDict(
     "UpdateActionsMessageTypeDef",
     {
         "Marker": str,
         "UpdateActions": List[UpdateActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSubnetGroupMessageTypeDef = TypedDict(
     "CacheSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "CacheSubnetGroups": List[CacheSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheSubnetGroupResultTypeDef = TypedDict(
     "CreateCacheSubnetGroupResultTypeDef",
     {
         "CacheSubnetGroup": CacheSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyCacheSubnetGroupResultTypeDef = TypedDict(
     "ModifyCacheSubnetGroupResultTypeDef",
     {
         "CacheSubnetGroup": CacheSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheClusterTypeDef = TypedDict(
     "CacheClusterTypeDef",
     {
         "CacheClusterId": str,
@@ -2834,123 +2855,123 @@
 )
 
 CacheClusterMessageTypeDef = TypedDict(
     "CacheClusterMessageTypeDef",
     {
         "Marker": str,
         "CacheClusters": List[CacheClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCacheClusterResultTypeDef = TypedDict(
     "CreateCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCacheClusterResultTypeDef = TypedDict(
     "DeleteCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyCacheClusterResultTypeDef = TypedDict(
     "ModifyCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootCacheClusterResultTypeDef = TypedDict(
     "RebootCacheClusterResultTypeDef",
     {
         "CacheCluster": CacheClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompleteMigrationResponseTypeDef = TypedDict(
     "CompleteMigrationResponseTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateReplicationGroupResultTypeDef = TypedDict(
     "CreateReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DecreaseReplicaCountResultTypeDef = TypedDict(
     "DecreaseReplicaCountResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteReplicationGroupResultTypeDef = TypedDict(
     "DeleteReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IncreaseReplicaCountResultTypeDef = TypedDict(
     "IncreaseReplicaCountResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationGroupResultTypeDef = TypedDict(
     "ModifyReplicationGroupResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationGroupShardConfigurationResultTypeDef = TypedDict(
     "ModifyReplicationGroupShardConfigurationResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicationGroupMessageTypeDef = TypedDict(
     "ReplicationGroupMessageTypeDef",
     {
         "Marker": str,
         "ReplicationGroups": List[ReplicationGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMigrationResponseTypeDef = TypedDict(
     "StartMigrationResponseTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestFailoverResultTypeDef = TypedDict(
     "TestFailoverResultTypeDef",
     {
         "ReplicationGroup": ReplicationGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/waiter.py` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache/waiter.pyi` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache.egg-info/PKG-INFO` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elasticache
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElastiCache 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElastiCache 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore elasticache type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore elasticache type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elasticache"></a>
 
 # types-aiobotocore-elasticache
 
 [![PyPI - types-aiobotocore-elasticache](https://img.shields.io/pypi/v/types-aiobotocore-elasticache.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticache)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticache.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticache)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elasticache?color=blue)](https://pypistats.org/packages/types-aiobotocore-elasticache)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticache)](https://pepy.tech/project/types-aiobotocore-elasticache)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElastiCache 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#ElastiCache)
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
 [types-aiobotocore-elasticache docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticache/).
 
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
@@ -456,25 +455,25 @@
 )
 
 
 def check_value(value: AZModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elasticache.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elasticache.type_defs import (
     TagTypeDef,
-    AllowedNodeTypeModificationsMessageTypeDef,
+    ResponseMetadataTypeDef,
     AuthenticationModeTypeDef,
     AuthenticationTypeDef,
     AuthorizeCacheSecurityGroupIngressMessageRequestTypeDef,
     AvailabilityZoneTypeDef,
     BatchApplyUpdateActionMessageRequestTypeDef,
     BatchStopUpdateActionMessageRequestTypeDef,
     CacheParameterGroupStatusTypeDef,
@@ -482,184 +481,187 @@
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     SecurityGroupMembershipTypeDef,
     CacheEngineVersionTypeDef,
     CacheNodeTypeSpecificValueTypeDef,
     CacheNodeUpdateStatusTypeDef,
     ParameterTypeDef,
-    CacheParameterGroupNameMessageTypeDef,
     CacheParameterGroupTypeDef,
     EC2SecurityGroupTypeDef,
     CloudWatchLogsDestinationDetailsTypeDef,
     CompleteMigrationMessageRequestTypeDef,
     ConfigureShardTypeDef,
     CreateGlobalReplicationGroupMessageRequestTypeDef,
-    NodeGroupConfigurationTypeDef,
     CustomerNodeEndpointTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
     DeleteCacheClusterMessageRequestTypeDef,
     DeleteCacheParameterGroupMessageRequestTypeDef,
     DeleteCacheSecurityGroupMessageRequestTypeDef,
     DeleteCacheSubnetGroupMessageRequestTypeDef,
     DeleteGlobalReplicationGroupMessageRequestTypeDef,
     DeleteReplicationGroupMessageRequestTypeDef,
     DeleteSnapshotMessageRequestTypeDef,
     DeleteUserGroupMessageRequestTypeDef,
     DeleteUserMessageRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeCacheClustersMessageRequestTypeDef,
-    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
     DescribeCacheEngineVersionsMessageRequestTypeDef,
-    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
     DescribeCacheParameterGroupsMessageRequestTypeDef,
-    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
     DescribeCacheParametersMessageRequestTypeDef,
-    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
     DescribeCacheSecurityGroupsMessageRequestTypeDef,
-    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
     DescribeCacheSubnetGroupsMessageRequestTypeDef,
-    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
     DescribeEngineDefaultParametersMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
+    TimestampTypeDef,
     DescribeGlobalReplicationGroupsMessageRequestTypeDef,
-    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
     DescribeReplicationGroupsMessageRequestTypeDef,
-    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
     DescribeReservedCacheNodesMessageRequestTypeDef,
-    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
     DescribeReservedCacheNodesOfferingsMessageRequestTypeDef,
-    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
     DescribeServiceUpdatesMessageRequestTypeDef,
-    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsMessageRequestTypeDef,
-    TimeRangeFilterTypeDef,
-    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
     DescribeUserGroupsMessageRequestTypeDef,
     FilterTypeDef,
     KinesisFirehoseDestinationDetailsTypeDef,
     DisassociateGlobalReplicationGroupMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EventTypeDef,
     FailoverGlobalReplicationGroupMessageRequestTypeDef,
     GlobalNodeGroupTypeDef,
     GlobalReplicationGroupInfoTypeDef,
     GlobalReplicationGroupMemberTypeDef,
     ListAllowedNodeTypeModificationsMessageRequestTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ParameterNameValueTypeDef,
     ModifyCacheSubnetGroupMessageRequestTypeDef,
     ModifyGlobalReplicationGroupMessageRequestTypeDef,
     ReshardingConfigurationTypeDef,
     ModifyUserGroupMessageRequestTypeDef,
+    NodeGroupConfigurationOutputTypeDef,
+    NodeGroupConfigurationTypeDef,
     NodeGroupMemberUpdateStatusTypeDef,
-    PaginatorConfigTypeDef,
     ProcessedUpdateActionTypeDef,
     RebalanceSlotsInGlobalReplicationGroupMessageRequestTypeDef,
     RebootCacheClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     UserGroupsUpdateStatusTypeDef,
     SlotMigrationTypeDef,
-    ResponseMetadataTypeDef,
     RevokeCacheSecurityGroupIngressMessageRequestTypeDef,
     ServiceUpdateTypeDef,
     SubnetOutpostTypeDef,
     TestFailoverMessageRequestTypeDef,
     UnprocessedUpdateActionTypeDef,
     UserGroupPendingChangesTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CopySnapshotMessageRequestTypeDef,
     CreateCacheParameterGroupMessageRequestTypeDef,
     CreateCacheSecurityGroupMessageRequestTypeDef,
     CreateCacheSubnetGroupMessageRequestTypeDef,
     CreateSnapshotMessageRequestTypeDef,
     CreateUserGroupMessageRequestTypeDef,
     PurchaseReservedCacheNodesOfferingMessageRequestTypeDef,
+    AllowedNodeTypeModificationsMessageTypeDef,
+    CacheParameterGroupNameMessageTypeDef,
+    EmptyResponseMetadataTypeDef,
     TagListMessageTypeDef,
     CreateUserMessageRequestTypeDef,
     ModifyUserMessageRequestTypeDef,
-    UserResponseMetadataTypeDef,
+    UserResponseTypeDef,
     UserTypeDef,
     CacheNodeTypeDef,
     NodeGroupMemberTypeDef,
     CacheEngineVersionMessageTypeDef,
     CacheNodeTypeSpecificParameterTypeDef,
     CacheParameterGroupsMessageTypeDef,
     CreateCacheParameterGroupResultTypeDef,
     CacheSecurityGroupTypeDef,
     DecreaseReplicaCountMessageRequestTypeDef,
     IncreaseReplicaCountMessageRequestTypeDef,
-    NodeSnapshotTypeDef,
     StartMigrationMessageRequestTypeDef,
     DescribeCacheClustersMessageCacheClusterAvailableWaitTypeDef,
     DescribeCacheClustersMessageCacheClusterDeletedWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupAvailableWaitTypeDef,
     DescribeReplicationGroupsMessageReplicationGroupDeletedWaitTypeDef,
-    DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
-    DescribeUpdateActionsMessageRequestTypeDef,
+    DescribeCacheClustersMessageDescribeCacheClustersPaginateTypeDef,
+    DescribeCacheEngineVersionsMessageDescribeCacheEngineVersionsPaginateTypeDef,
+    DescribeCacheParameterGroupsMessageDescribeCacheParameterGroupsPaginateTypeDef,
+    DescribeCacheParametersMessageDescribeCacheParametersPaginateTypeDef,
+    DescribeCacheSecurityGroupsMessageDescribeCacheSecurityGroupsPaginateTypeDef,
+    DescribeCacheSubnetGroupsMessageDescribeCacheSubnetGroupsPaginateTypeDef,
+    DescribeEngineDefaultParametersMessageDescribeEngineDefaultParametersPaginateTypeDef,
+    DescribeGlobalReplicationGroupsMessageDescribeGlobalReplicationGroupsPaginateTypeDef,
+    DescribeReplicationGroupsMessageDescribeReplicationGroupsPaginateTypeDef,
+    DescribeReservedCacheNodesMessageDescribeReservedCacheNodesPaginateTypeDef,
+    DescribeReservedCacheNodesOfferingsMessageDescribeReservedCacheNodesOfferingsPaginateTypeDef,
+    DescribeServiceUpdatesMessageDescribeServiceUpdatesPaginateTypeDef,
+    DescribeSnapshotsMessageDescribeSnapshotsPaginateTypeDef,
+    DescribeUserGroupsMessageDescribeUserGroupsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    TimeRangeFilterTypeDef,
     DescribeUsersMessageDescribeUsersPaginateTypeDef,
     DescribeUsersMessageRequestTypeDef,
     DestinationDetailsTypeDef,
     EventsMessageTypeDef,
     GlobalReplicationGroupTypeDef,
     ModifyCacheParameterGroupMessageRequestTypeDef,
     ResetCacheParameterGroupMessageRequestTypeDef,
     ModifyReplicationGroupShardConfigurationMessageRequestTypeDef,
     RegionalConfigurationTypeDef,
+    NodeSnapshotTypeDef,
+    NodeGroupConfigurationUnionTypeDef,
     NodeGroupUpdateStatusTypeDef,
     ReservedCacheNodeTypeDef,
     ReservedCacheNodesOfferingTypeDef,
     ReshardingStatusTypeDef,
     ServiceUpdatesMessageTypeDef,
     SubnetTypeDef,
     UpdateActionResultsMessageTypeDef,
-    UserGroupResponseMetadataTypeDef,
+    UserGroupResponseTypeDef,
     UserGroupTypeDef,
     DescribeUsersResultTypeDef,
     NodeGroupTypeDef,
     CacheParameterGroupDetailsTypeDef,
     EngineDefaultsTypeDef,
     AuthorizeCacheSecurityGroupIngressResultTypeDef,
     CacheSecurityGroupMessageTypeDef,
     CreateCacheSecurityGroupResultTypeDef,
     RevokeCacheSecurityGroupIngressResultTypeDef,
-    SnapshotTypeDef,
+    DescribeUpdateActionsMessageDescribeUpdateActionsPaginateTypeDef,
+    DescribeUpdateActionsMessageRequestTypeDef,
     LogDeliveryConfigurationRequestTypeDef,
     LogDeliveryConfigurationTypeDef,
     PendingLogDeliveryConfigurationTypeDef,
     CreateGlobalReplicationGroupResultTypeDef,
     DecreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     DeleteGlobalReplicationGroupResultTypeDef,
     DescribeGlobalReplicationGroupsResultTypeDef,
     DisassociateGlobalReplicationGroupResultTypeDef,
     FailoverGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupResultTypeDef,
     ModifyGlobalReplicationGroupResultTypeDef,
     RebalanceSlotsInGlobalReplicationGroupResultTypeDef,
     IncreaseNodeGroupsInGlobalReplicationGroupMessageRequestTypeDef,
+    SnapshotTypeDef,
     UpdateActionTypeDef,
     PurchaseReservedCacheNodesOfferingResultTypeDef,
     ReservedCacheNodeMessageTypeDef,
     ReservedCacheNodesOfferingMessageTypeDef,
     CacheSubnetGroupTypeDef,
     DescribeUserGroupsResultTypeDef,
     DescribeEngineDefaultParametersResultTypeDef,
-    CopySnapshotResultTypeDef,
-    CreateSnapshotResultTypeDef,
-    DeleteSnapshotResultTypeDef,
-    DescribeSnapshotsListMessageTypeDef,
     CreateCacheClusterMessageRequestTypeDef,
     CreateReplicationGroupMessageRequestTypeDef,
     ModifyCacheClusterMessageRequestTypeDef,
     ModifyReplicationGroupMessageRequestTypeDef,
     PendingModifiedValuesTypeDef,
     ReplicationGroupPendingModifiedValuesTypeDef,
+    CopySnapshotResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DescribeSnapshotsListMessageTypeDef,
     UpdateActionsMessageTypeDef,
     CacheSubnetGroupMessageTypeDef,
     CreateCacheSubnetGroupResultTypeDef,
     ModifyCacheSubnetGroupResultTypeDef,
     CacheClusterTypeDef,
     ReplicationGroupTypeDef,
     CacheClusterMessageTypeDef,
@@ -676,15 +678,15 @@
     ModifyReplicationGroupShardConfigurationResultTypeDef,
     ReplicationGroupMessageTypeDef,
     StartMigrationResponseTypeDef,
     TestFailoverResultTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elasticache-2.5.2/types_aiobotocore_elasticache.egg-info/SOURCES.txt` & `types-aiobotocore-elasticache-2.5.2.post1/types_aiobotocore_elasticache.egg-info/SOURCES.txt`

 * *Files identical despite different names*


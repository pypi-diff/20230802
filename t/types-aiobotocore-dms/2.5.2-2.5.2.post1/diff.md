# Comparing `tmp/types-aiobotocore-dms-2.5.2.tar.gz` & `tmp/types-aiobotocore-dms-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dms-2.5.2.tar", last modified: Sat Jul  8 01:43:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-dms-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:11 2023, max compression
```

## Comparing `types-aiobotocore-dms-2.5.2.tar` & `types-aiobotocore-dms-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.046026 types-aiobotocore-dms-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28954 2023-07-08 01:43:32.046026 types-aiobotocore-dms-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27384 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:32.046026 types-aiobotocore-dms-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.046026 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69200 2023-07-08 01:28:52.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    69101 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-07-08 01:28:53.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-08 01:28:53.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17836 2023-07-08 01:28:52.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17820 2023-07-08 01:28:52.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    92980 2023-07-08 01:28:55.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    92929 2023-07-08 01:28:54.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:51.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-08 01:28:52.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-07-08 01:28:52.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.046026 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28954 2023-07-08 01:43:31.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:31.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:31.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:31.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:31.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:31.000000 types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.821601 types-aiobotocore-dms-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-08-02 14:52:11.817601 types-aiobotocore-dms-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27471 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:11.821601 types-aiobotocore-dms-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.817601 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69116 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69017 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14827 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17787 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17771 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    94720 2023-08-02 14:36:35.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94669 2023-08-02 14:36:33.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:31.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10050 2023-08-02 14:36:32.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.817601 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28994 2023-08-02 14:52:11.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:11.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:11.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:11.000000 types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dms-2.5.2/LICENSE` & `types-aiobotocore-dms-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2/PKG-INFO` & `types-aiobotocore-dms-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dms
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore dms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore dms type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-dms"></a>
 
 # types-aiobotocore-dms
 
 [![PyPI - types-aiobotocore-dms](https://img.shields.io/pypi/v/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dms?color=blue)](https://pypistats.org/packages/types-aiobotocore-dms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dms)](https://pepy.tech/project/types-aiobotocore-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DatabaseMigrationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
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
 [types-aiobotocore-dms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/).
 
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
@@ -458,28 +457,30 @@
 )
 
 
 def check_value(value: AuthMechanismValueType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_dms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_dms.type_defs import (
     AccountQuotaTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     AvailabilityZoneTypeDef,
     BatchStartRecommendationsErrorEntryTypeDef,
+    BlobTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
     CertificateTypeDef,
     CollectorHealthCheckTypeDef,
     InventoryDataTypeDef,
     CollectorShortInfoResponseTypeDef,
     ConnectionTypeDef,
     DmsTransferSettingsTypeDef,
@@ -498,143 +499,143 @@
     PostgreSQLSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     EventSubscriptionTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
+    TimestampTypeDef,
     DatabaseInstanceSoftwareDetailsResponseTypeDef,
     ServerShortInfoResponseTypeDef,
     DatabaseShortInfoResponseTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
     EndpointSettingTypeDef,
     SupportedEndpointTypeTypeDef,
     EventCategoryGroupTypeDef,
     EventTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
     FleetAdvisorLsaAnalysisResponseTypeDef,
     FleetAdvisorSchemaObjectResponseTypeDef,
-    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
     OrderableReplicationInstanceTypeDef,
     LimitationTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
     RefreshSchemasStatusTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     ReplicationInstanceTaskLogTypeDef,
-    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
     ReplicationTaskAssessmentResultTypeDef,
     ReplicationTaskIndividualAssessmentTypeDef,
-    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
-    DescribeSchemasResponseTypeDef,
     TableStatisticsTypeDef,
-    EmptyResponseMetadataTypeDef,
+    OracleSettingsOutputTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
-    ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     RdsConfigurationTypeDef,
     RdsRequirementsTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
-    ReloadTablesResponseTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     ReplicationPendingModifiedValuesTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ReplicationTaskAssessmentRunProgressTypeDef,
     ReplicationTaskStatsTypeDef,
-    ResponseMetadataTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
     SchemaShortInfoResponseTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
-    StartReplicationTaskMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
-    CreateReplicationTaskMessageRequestTypeDef,
-    ImportCertificateMessageRequestTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
+    DescribeSchemasResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ReloadTablesResponseTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
     SubnetTypeDef,
     BatchStartRecommendationsResponseTypeDef,
+    ImportCertificateMessageRequestTypeDef,
     DeleteCertificateResponseTypeDef,
     DescribeCertificatesResponseTypeDef,
     ImportCertificateResponseTypeDef,
     CollectorResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     DescribeConnectionsResponseTypeDef,
     TestConnectionResponseTypeDef,
     CreateEndpointMessageRequestTypeDef,
-    EndpointTypeDef,
     ModifyEndpointMessageRequestTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     DeleteEventSubscriptionResponseTypeDef,
     DescribeEventSubscriptionsResponseTypeDef,
     ModifyEventSubscriptionResponseTypeDef,
+    CreateReplicationTaskMessageRequestTypeDef,
+    ModifyReplicationTaskMessageRequestTypeDef,
+    StartReplicationTaskMessageRequestTypeDef,
     DatabaseResponseTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
-    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
-    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
-    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
     DescribeEndpointsMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeFleetAdvisorCollectorsRequestRequestTypeDef,
     DescribeFleetAdvisorDatabasesRequestRequestTypeDef,
     DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef,
     DescribeFleetAdvisorSchemasRequestRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     DescribeRecommendationLimitationsRequestRequestTypeDef,
     DescribeRecommendationsRequestRequestTypeDef,
-    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
     DescribeReplicationInstancesMessageRequestTypeDef,
-    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
     DescribeReplicationSubnetGroupsMessageRequestTypeDef,
     DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef,
     DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef,
-    DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
     DescribeReplicationTasksMessageRequestTypeDef,
-    DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
     DescribeTableStatisticsMessageRequestTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
+    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
+    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
+    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
+    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
+    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
+    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
+    DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
+    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+    DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
     DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef,
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
@@ -649,29 +650,31 @@
     DescribeRecommendationLimitationsResponseTypeDef,
     DescribeRefreshSchemasStatusResponseTypeDef,
     RefreshSchemasResponseTypeDef,
     DescribeReplicationInstanceTaskLogsResponseTypeDef,
     DescribeReplicationTaskAssessmentResultsResponseTypeDef,
     DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
     DescribeTableStatisticsResponseTypeDef,
+    EndpointTypeDef,
+    OracleSettingsUnionTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     RdsRecommendationTypeDef,
     StartRecommendationsRequestEntryTypeDef,
     StartRecommendationsRequestRequestTypeDef,
     ReloadTablesMessageRequestTypeDef,
     ReplicationTaskAssessmentRunTypeDef,
     ReplicationTaskTypeDef,
     SchemaResponseTypeDef,
     ReplicationSubnetGroupTypeDef,
     DescribeFleetAdvisorCollectorsResponseTypeDef,
+    DescribeFleetAdvisorDatabasesResponseTypeDef,
     CreateEndpointResponseTypeDef,
     DeleteEndpointResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     ModifyEndpointResponseTypeDef,
-    DescribeFleetAdvisorDatabasesResponseTypeDef,
     ApplyPendingMaintenanceActionResponseTypeDef,
     DescribePendingMaintenanceActionsResponseTypeDef,
     RecommendationDataTypeDef,
     BatchStartRecommendationsRequestRequestTypeDef,
     CancelReplicationTaskAssessmentRunResponseTypeDef,
     DeleteReplicationTaskAssessmentRunResponseTypeDef,
     DescribeReplicationTaskAssessmentRunsResponseTypeDef,
@@ -695,15 +698,15 @@
     DescribeReplicationInstancesResponseTypeDef,
     ModifyReplicationInstanceResponseTypeDef,
     RebootReplicationInstanceResponseTypeDef,
     DescribeRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountQuotaTypeDef:
+def get_value() -> AccountQuotaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dms-2.5.2/README.md` & `types-aiobotocore-dms-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-dms"></a>
 
 # types-aiobotocore-dms
 
 [![PyPI - types-aiobotocore-dms](https://img.shields.io/pypi/v/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dms?color=blue)](https://pypistats.org/packages/types-aiobotocore-dms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dms)](https://pepy.tech/project/types-aiobotocore-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DatabaseMigrationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
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
 [types-aiobotocore-dms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/).
 
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
@@ -425,28 +425,30 @@
 )
 
 
 def check_value(value: AuthMechanismValueType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_dms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_dms.type_defs import (
     AccountQuotaTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     AvailabilityZoneTypeDef,
     BatchStartRecommendationsErrorEntryTypeDef,
+    BlobTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
     CertificateTypeDef,
     CollectorHealthCheckTypeDef,
     InventoryDataTypeDef,
     CollectorShortInfoResponseTypeDef,
     ConnectionTypeDef,
     DmsTransferSettingsTypeDef,
@@ -465,143 +467,143 @@
     PostgreSQLSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     EventSubscriptionTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
+    TimestampTypeDef,
     DatabaseInstanceSoftwareDetailsResponseTypeDef,
     ServerShortInfoResponseTypeDef,
     DatabaseShortInfoResponseTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
     EndpointSettingTypeDef,
     SupportedEndpointTypeTypeDef,
     EventCategoryGroupTypeDef,
     EventTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
     FleetAdvisorLsaAnalysisResponseTypeDef,
     FleetAdvisorSchemaObjectResponseTypeDef,
-    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
     OrderableReplicationInstanceTypeDef,
     LimitationTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
     RefreshSchemasStatusTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     ReplicationInstanceTaskLogTypeDef,
-    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
     ReplicationTaskAssessmentResultTypeDef,
     ReplicationTaskIndividualAssessmentTypeDef,
-    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
-    DescribeSchemasResponseTypeDef,
     TableStatisticsTypeDef,
-    EmptyResponseMetadataTypeDef,
+    OracleSettingsOutputTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
-    ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     RdsConfigurationTypeDef,
     RdsRequirementsTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
-    ReloadTablesResponseTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     ReplicationPendingModifiedValuesTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ReplicationTaskAssessmentRunProgressTypeDef,
     ReplicationTaskStatsTypeDef,
-    ResponseMetadataTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
     SchemaShortInfoResponseTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
-    StartReplicationTaskMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
-    CreateReplicationTaskMessageRequestTypeDef,
-    ImportCertificateMessageRequestTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
+    DescribeSchemasResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ReloadTablesResponseTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
     SubnetTypeDef,
     BatchStartRecommendationsResponseTypeDef,
+    ImportCertificateMessageRequestTypeDef,
     DeleteCertificateResponseTypeDef,
     DescribeCertificatesResponseTypeDef,
     ImportCertificateResponseTypeDef,
     CollectorResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     DescribeConnectionsResponseTypeDef,
     TestConnectionResponseTypeDef,
     CreateEndpointMessageRequestTypeDef,
-    EndpointTypeDef,
     ModifyEndpointMessageRequestTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     DeleteEventSubscriptionResponseTypeDef,
     DescribeEventSubscriptionsResponseTypeDef,
     ModifyEventSubscriptionResponseTypeDef,
+    CreateReplicationTaskMessageRequestTypeDef,
+    ModifyReplicationTaskMessageRequestTypeDef,
+    StartReplicationTaskMessageRequestTypeDef,
     DatabaseResponseTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
-    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
-    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
-    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
     DescribeEndpointsMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeFleetAdvisorCollectorsRequestRequestTypeDef,
     DescribeFleetAdvisorDatabasesRequestRequestTypeDef,
     DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef,
     DescribeFleetAdvisorSchemasRequestRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     DescribeRecommendationLimitationsRequestRequestTypeDef,
     DescribeRecommendationsRequestRequestTypeDef,
-    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
     DescribeReplicationInstancesMessageRequestTypeDef,
-    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
     DescribeReplicationSubnetGroupsMessageRequestTypeDef,
     DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef,
     DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef,
-    DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
     DescribeReplicationTasksMessageRequestTypeDef,
-    DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
     DescribeTableStatisticsMessageRequestTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
+    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
+    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
+    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
+    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
+    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
+    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
+    DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
+    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+    DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
     DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef,
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
@@ -616,29 +618,31 @@
     DescribeRecommendationLimitationsResponseTypeDef,
     DescribeRefreshSchemasStatusResponseTypeDef,
     RefreshSchemasResponseTypeDef,
     DescribeReplicationInstanceTaskLogsResponseTypeDef,
     DescribeReplicationTaskAssessmentResultsResponseTypeDef,
     DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
     DescribeTableStatisticsResponseTypeDef,
+    EndpointTypeDef,
+    OracleSettingsUnionTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     RdsRecommendationTypeDef,
     StartRecommendationsRequestEntryTypeDef,
     StartRecommendationsRequestRequestTypeDef,
     ReloadTablesMessageRequestTypeDef,
     ReplicationTaskAssessmentRunTypeDef,
     ReplicationTaskTypeDef,
     SchemaResponseTypeDef,
     ReplicationSubnetGroupTypeDef,
     DescribeFleetAdvisorCollectorsResponseTypeDef,
+    DescribeFleetAdvisorDatabasesResponseTypeDef,
     CreateEndpointResponseTypeDef,
     DeleteEndpointResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     ModifyEndpointResponseTypeDef,
-    DescribeFleetAdvisorDatabasesResponseTypeDef,
     ApplyPendingMaintenanceActionResponseTypeDef,
     DescribePendingMaintenanceActionsResponseTypeDef,
     RecommendationDataTypeDef,
     BatchStartRecommendationsRequestRequestTypeDef,
     CancelReplicationTaskAssessmentRunResponseTypeDef,
     DeleteReplicationTaskAssessmentRunResponseTypeDef,
     DescribeReplicationTaskAssessmentRunsResponseTypeDef,
@@ -662,15 +666,15 @@
     DescribeReplicationInstancesResponseTypeDef,
     ModifyReplicationInstanceResponseTypeDef,
     RebootReplicationInstanceResponseTypeDef,
     DescribeRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountQuotaTypeDef:
+def get_value() -> AccountQuotaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dms-2.5.2/setup.py` & `types-aiobotocore-dms-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dms",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_dms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DatabaseMigrationService 2.5.2 service generated with"
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
-    keywords="aiobotocore dms type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore dms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_dms": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/__init__.py` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/__init__.pyi` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/__main__.py` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.DatabaseMigrationService 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService\nOther"
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

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/client.py` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 
     session = get_session()
     async with session.create_client("dms") as client:
         client: DatabaseMigrationServiceClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     DmsSslModeValueType,
     MigrationTypeValueType,
     ReloadOptionValueType,
     ReplicationEndpointTypeValueType,
@@ -43,14 +41,15 @@
     DescribeReplicationTasksPaginator,
     DescribeSchemasPaginator,
     DescribeTableStatisticsPaginator,
 )
 from .type_defs import (
     ApplyPendingMaintenanceActionResponseTypeDef,
     BatchStartRecommendationsResponseTypeDef,
+    BlobTypeDef,
     CancelReplicationTaskAssessmentRunResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     CreateFleetAdvisorCollectorResponseTypeDef,
     CreateReplicationInstanceResponseTypeDef,
     CreateReplicationSubnetGroupResponseTypeDef,
     CreateReplicationTaskResponseTypeDef,
@@ -109,15 +108,15 @@
     ModifyReplicationInstanceResponseTypeDef,
     ModifyReplicationSubnetGroupResponseTypeDef,
     ModifyReplicationTaskResponseTypeDef,
     MongoDbSettingsTypeDef,
     MoveReplicationTaskResponseTypeDef,
     MySQLSettingsTypeDef,
     NeptuneSettingsTypeDef,
-    OracleSettingsTypeDef,
+    OracleSettingsUnionTypeDef,
     PostgreSQLSettingsTypeDef,
     RebootReplicationInstanceResponseTypeDef,
     RecommendationSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     RefreshSchemasResponseTypeDef,
     ReloadTablesResponseTypeDef,
@@ -128,14 +127,15 @@
     StartReplicationTaskAssessmentRunResponseTypeDef,
     StartReplicationTaskResponseTypeDef,
     StopReplicationTaskResponseTypeDef,
     SybaseSettingsTypeDef,
     TableToReloadTypeDef,
     TagTypeDef,
     TestConnectionResponseTypeDef,
+    TimestampTypeDef,
     UpdateSubscriptionsToEventBridgeResponseTypeDef,
 )
 from .waiter import (
     EndpointDeletedWaiter,
     ReplicationInstanceAvailableWaiter,
     ReplicationInstanceDeletedWaiter,
     ReplicationTaskDeletedWaiter,
@@ -292,15 +292,15 @@
         KinesisSettings: KinesisSettingsTypeDef = ...,
         KafkaSettings: KafkaSettingsTypeDef = ...,
         ElasticsearchSettings: ElasticsearchSettingsTypeDef = ...,
         NeptuneSettings: NeptuneSettingsTypeDef = ...,
         RedshiftSettings: RedshiftSettingsTypeDef = ...,
         PostgreSQLSettings: PostgreSQLSettingsTypeDef = ...,
         MySQLSettings: MySQLSettingsTypeDef = ...,
-        OracleSettings: OracleSettingsTypeDef = ...,
+        OracleSettings: OracleSettingsUnionTypeDef = ...,
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         ResourceIdentifier: str = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...
@@ -393,15 +393,15 @@
         ReplicationTaskIdentifier: str,
         SourceEndpointArn: str,
         TargetEndpointArn: str,
         ReplicationInstanceArn: str,
         MigrationType: MigrationTypeValueType,
         TableMappings: str,
         ReplicationTaskSettings: str = ...,
-        CdcStartTime: Union[datetime, str] = ...,
+        CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TaskData: str = ...,
         ResourceIdentifier: str = ...
     ) -> CreateReplicationTaskResponseTypeDef:
         """
@@ -613,16 +613,16 @@
         """
 
     async def describe_events(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: Literal["replication-instance"] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> DescribeEventsResponseTypeDef:
         """
@@ -863,15 +863,15 @@
         """
 
     async def import_certificate(
         self,
         *,
         CertificateIdentifier: str,
         CertificatePem: str = ...,
-        CertificateWallet: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        CertificateWallet: BlobTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> ImportCertificateResponseTypeDef:
         """
         Uploads the specified certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.import_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#import_certificate)
@@ -912,15 +912,15 @@
         KinesisSettings: KinesisSettingsTypeDef = ...,
         KafkaSettings: KafkaSettingsTypeDef = ...,
         ElasticsearchSettings: ElasticsearchSettingsTypeDef = ...,
         NeptuneSettings: NeptuneSettingsTypeDef = ...,
         RedshiftSettings: RedshiftSettingsTypeDef = ...,
         PostgreSQLSettings: PostgreSQLSettingsTypeDef = ...,
         MySQLSettings: MySQLSettingsTypeDef = ...,
-        OracleSettings: OracleSettingsTypeDef = ...,
+        OracleSettings: OracleSettingsUnionTypeDef = ...,
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         ExactSettings: bool = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...
@@ -989,15 +989,15 @@
         self,
         *,
         ReplicationTaskArn: str,
         ReplicationTaskIdentifier: str = ...,
         MigrationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationTaskSettings: str = ...,
-        CdcStartTime: Union[datetime, str] = ...,
+        CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         TaskData: str = ...
     ) -> ModifyReplicationTaskResponseTypeDef:
         """
         Modifies the specified replication task.
 
@@ -1086,15 +1086,15 @@
         """
 
     async def start_replication_task(
         self,
         *,
         ReplicationTaskArn: str,
         StartReplicationTaskType: StartReplicationTaskTypeValueType,
-        CdcStartTime: Union[datetime, str] = ...,
+        CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...
     ) -> StartReplicationTaskResponseTypeDef:
         """
         Starts the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task)
```

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/client.pyi` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 
     session = get_session()
     async with session.create_client("dms") as client:
         client: DatabaseMigrationServiceClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     DmsSslModeValueType,
     MigrationTypeValueType,
     ReloadOptionValueType,
     ReplicationEndpointTypeValueType,
@@ -43,14 +41,15 @@
     DescribeReplicationTasksPaginator,
     DescribeSchemasPaginator,
     DescribeTableStatisticsPaginator,
 )
 from .type_defs import (
     ApplyPendingMaintenanceActionResponseTypeDef,
     BatchStartRecommendationsResponseTypeDef,
+    BlobTypeDef,
     CancelReplicationTaskAssessmentRunResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     CreateFleetAdvisorCollectorResponseTypeDef,
     CreateReplicationInstanceResponseTypeDef,
     CreateReplicationSubnetGroupResponseTypeDef,
     CreateReplicationTaskResponseTypeDef,
@@ -109,15 +108,15 @@
     ModifyReplicationInstanceResponseTypeDef,
     ModifyReplicationSubnetGroupResponseTypeDef,
     ModifyReplicationTaskResponseTypeDef,
     MongoDbSettingsTypeDef,
     MoveReplicationTaskResponseTypeDef,
     MySQLSettingsTypeDef,
     NeptuneSettingsTypeDef,
-    OracleSettingsTypeDef,
+    OracleSettingsUnionTypeDef,
     PostgreSQLSettingsTypeDef,
     RebootReplicationInstanceResponseTypeDef,
     RecommendationSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     RefreshSchemasResponseTypeDef,
     ReloadTablesResponseTypeDef,
@@ -128,14 +127,15 @@
     StartReplicationTaskAssessmentRunResponseTypeDef,
     StartReplicationTaskResponseTypeDef,
     StopReplicationTaskResponseTypeDef,
     SybaseSettingsTypeDef,
     TableToReloadTypeDef,
     TagTypeDef,
     TestConnectionResponseTypeDef,
+    TimestampTypeDef,
     UpdateSubscriptionsToEventBridgeResponseTypeDef,
 )
 from .waiter import (
     EndpointDeletedWaiter,
     ReplicationInstanceAvailableWaiter,
     ReplicationInstanceDeletedWaiter,
     ReplicationTaskDeletedWaiter,
@@ -281,15 +281,15 @@
         KinesisSettings: KinesisSettingsTypeDef = ...,
         KafkaSettings: KafkaSettingsTypeDef = ...,
         ElasticsearchSettings: ElasticsearchSettingsTypeDef = ...,
         NeptuneSettings: NeptuneSettingsTypeDef = ...,
         RedshiftSettings: RedshiftSettingsTypeDef = ...,
         PostgreSQLSettings: PostgreSQLSettingsTypeDef = ...,
         MySQLSettings: MySQLSettingsTypeDef = ...,
-        OracleSettings: OracleSettingsTypeDef = ...,
+        OracleSettings: OracleSettingsUnionTypeDef = ...,
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         ResourceIdentifier: str = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...
@@ -377,15 +377,15 @@
         ReplicationTaskIdentifier: str,
         SourceEndpointArn: str,
         TargetEndpointArn: str,
         ReplicationInstanceArn: str,
         MigrationType: MigrationTypeValueType,
         TableMappings: str,
         ReplicationTaskSettings: str = ...,
-        CdcStartTime: Union[datetime, str] = ...,
+        CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TaskData: str = ...,
         ResourceIdentifier: str = ...
     ) -> CreateReplicationTaskResponseTypeDef:
         """
@@ -577,16 +577,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#describe_event_subscriptions)
         """
     async def describe_events(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: Literal["replication-instance"] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> DescribeEventsResponseTypeDef:
         """
@@ -806,15 +806,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#generate_presigned_url)
         """
     async def import_certificate(
         self,
         *,
         CertificateIdentifier: str,
         CertificatePem: str = ...,
-        CertificateWallet: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        CertificateWallet: BlobTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> ImportCertificateResponseTypeDef:
         """
         Uploads the specified certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.import_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#import_certificate)
@@ -853,15 +853,15 @@
         KinesisSettings: KinesisSettingsTypeDef = ...,
         KafkaSettings: KafkaSettingsTypeDef = ...,
         ElasticsearchSettings: ElasticsearchSettingsTypeDef = ...,
         NeptuneSettings: NeptuneSettingsTypeDef = ...,
         RedshiftSettings: RedshiftSettingsTypeDef = ...,
         PostgreSQLSettings: PostgreSQLSettingsTypeDef = ...,
         MySQLSettings: MySQLSettingsTypeDef = ...,
-        OracleSettings: OracleSettingsTypeDef = ...,
+        OracleSettings: OracleSettingsUnionTypeDef = ...,
         SybaseSettings: SybaseSettingsTypeDef = ...,
         MicrosoftSQLServerSettings: MicrosoftSQLServerSettingsTypeDef = ...,
         IBMDb2Settings: IBMDb2SettingsTypeDef = ...,
         DocDbSettings: DocDbSettingsTypeDef = ...,
         RedisSettings: RedisSettingsTypeDef = ...,
         ExactSettings: bool = ...,
         GcpMySQLSettings: GcpMySQLSettingsTypeDef = ...
@@ -926,15 +926,15 @@
         self,
         *,
         ReplicationTaskArn: str,
         ReplicationTaskIdentifier: str = ...,
         MigrationType: MigrationTypeValueType = ...,
         TableMappings: str = ...,
         ReplicationTaskSettings: str = ...,
-        CdcStartTime: Union[datetime, str] = ...,
+        CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...,
         TaskData: str = ...
     ) -> ModifyReplicationTaskResponseTypeDef:
         """
         Modifies the specified replication task.
 
@@ -1015,15 +1015,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/client/#start_recommendations)
         """
     async def start_replication_task(
         self,
         *,
         ReplicationTaskArn: str,
         StartReplicationTaskType: StartReplicationTaskTypeValueType,
-        CdcStartTime: Union[datetime, str] = ...,
+        CdcStartTime: TimestampTypeDef = ...,
         CdcStartPosition: str = ...,
         CdcStopPosition: str = ...
     ) -> StartReplicationTaskResponseTypeDef:
         """
         Starts the replication task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Client.start_replication_task)
```

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/literals.py` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/literals.pyi` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/paginator.py` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,15 @@
         describe_replication_task_assessment_results_paginator: DescribeReplicationTaskAssessmentResultsPaginator = client.get_paginator("describe_replication_task_assessment_results")
         describe_replication_tasks_paginator: DescribeReplicationTasksPaginator = client.get_paginator("describe_replication_tasks")
         describe_schemas_paginator: DescribeSchemasPaginator = client.get_paginator("describe_schemas")
         describe_table_statistics_paginator: DescribeTableStatisticsPaginator = client.get_paginator("describe_table_statistics")
     ```
 """
 import sys
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     DescribeCertificatesResponseTypeDef,
     DescribeConnectionsResponseTypeDef,
@@ -63,14 +62,15 @@
     DescribeReplicationSubnetGroupsResponseTypeDef,
     DescribeReplicationTaskAssessmentResultsResponseTypeDef,
     DescribeReplicationTasksResponseTypeDef,
     DescribeSchemasResponseTypeDef,
     DescribeTableStatisticsResponseTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -108,15 +108,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describecertificatespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describecertificatespaginator)
         """
 
 
@@ -126,15 +126,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeconnectionspaginator)
         """
 
 
@@ -144,15 +144,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEndpointTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointtypespaginator)
         """
 
 
@@ -162,15 +162,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointspaginator)
         """
 
 
@@ -181,15 +181,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -200,35 +200,35 @@
     """
 
     def paginate(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: Literal["replication-instance"] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeeventspaginator)
         """
 
 
 class DescribeOrderableReplicationInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeorderablereplicationinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOrderableReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeorderablereplicationinstancespaginator)
         """
 
 
@@ -238,15 +238,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationinstancespaginator)
         """
 
 
@@ -256,30 +256,30 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationsubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationsubnetgroupspaginator)
         """
 
 
 class DescribeReplicationTaskAssessmentResultsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationtaskassessmentresultspaginator)
     """
 
     def paginate(
-        self, *, ReplicationTaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReplicationTaskArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReplicationTaskAssessmentResultsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationtaskassessmentresultspaginator)
         """
 
 
@@ -290,30 +290,30 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         WithoutSettings: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReplicationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationtaskspaginator)
         """
 
 
 class DescribeSchemasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeschemaspaginator)
     """
 
     def paginate(
-        self, *, EndpointArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, EndpointArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeschemaspaginator)
         """
 
 
@@ -324,13 +324,13 @@
     """
 
     def paginate(
         self,
         *,
         ReplicationTaskArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTableStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describetablestatisticspaginator)
         """
```

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/paginator.pyi` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,15 @@
         describe_replication_task_assessment_results_paginator: DescribeReplicationTaskAssessmentResultsPaginator = client.get_paginator("describe_replication_task_assessment_results")
         describe_replication_tasks_paginator: DescribeReplicationTasksPaginator = client.get_paginator("describe_replication_tasks")
         describe_schemas_paginator: DescribeSchemasPaginator = client.get_paginator("describe_schemas")
         describe_table_statistics_paginator: DescribeTableStatisticsPaginator = client.get_paginator("describe_table_statistics")
     ```
 """
 import sys
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     DescribeCertificatesResponseTypeDef,
     DescribeConnectionsResponseTypeDef,
@@ -63,14 +62,15 @@
     DescribeReplicationSubnetGroupsResponseTypeDef,
     DescribeReplicationTaskAssessmentResultsResponseTypeDef,
     DescribeReplicationTasksResponseTypeDef,
     DescribeSchemasResponseTypeDef,
     DescribeTableStatisticsResponseTypeDef,
     FilterTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -104,15 +104,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describecertificatespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describecertificatespaginator)
         """
 
 class DescribeConnectionsPaginator(AioPaginator):
@@ -121,15 +121,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeconnectionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeConnections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeconnectionspaginator)
         """
 
 class DescribeEndpointTypesPaginator(AioPaginator):
@@ -138,15 +138,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointtypespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEndpointTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpointTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointtypespaginator)
         """
 
 class DescribeEndpointsPaginator(AioPaginator):
@@ -155,15 +155,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeendpointspaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(AioPaginator):
@@ -173,15 +173,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -191,34 +191,34 @@
     """
 
     def paginate(
         self,
         *,
         SourceIdentifier: str = ...,
         SourceType: Literal["replication-instance"] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeeventspaginator)
         """
 
 class DescribeOrderableReplicationInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeorderablereplicationinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOrderableReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeOrderableReplicationInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeorderablereplicationinstancespaginator)
         """
 
 class DescribeReplicationInstancesPaginator(AioPaginator):
@@ -227,15 +227,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReplicationInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationinstancespaginator)
         """
 
 class DescribeReplicationSubnetGroupsPaginator(AioPaginator):
@@ -244,29 +244,29 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationsubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReplicationSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationsubnetgroupspaginator)
         """
 
 class DescribeReplicationTaskAssessmentResultsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationtaskassessmentresultspaginator)
     """
 
     def paginate(
-        self, *, ReplicationTaskArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReplicationTaskArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReplicationTaskAssessmentResultsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTaskAssessmentResults.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationtaskassessmentresultspaginator)
         """
 
 class DescribeReplicationTasksPaginator(AioPaginator):
@@ -276,29 +276,29 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         WithoutSettings: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReplicationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeReplicationTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describereplicationtaskspaginator)
         """
 
 class DescribeSchemasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeschemaspaginator)
     """
 
     def paginate(
-        self, *, EndpointArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, EndpointArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describeschemaspaginator)
         """
 
 class DescribeTableStatisticsPaginator(AioPaginator):
@@ -308,13 +308,13 @@
     """
 
     def paginate(
         self,
         *,
         ReplicationTaskArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTableStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService.Paginator.DescribeTableStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/paginators/#describetablestatisticspaginator)
         """
```

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/type_defs.py` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_dms.type_defs import AccountQuotaTypeDef
 
-    data: AccountQuotaTypeDef = {...}
+    data: AccountQuotaTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -56,21 +56,22 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountQuotaTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchStartRecommendationsErrorEntryTypeDef",
+    "BlobTypeDef",
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     "CertificateTypeDef",
     "CollectorHealthCheckTypeDef",
     "InventoryDataTypeDef",
     "CollectorShortInfoResponseTypeDef",
     "ConnectionTypeDef",
     "DmsTransferSettingsTypeDef",
@@ -89,143 +90,143 @@
     "PostgreSQLSettingsTypeDef",
     "RedisSettingsTypeDef",
     "RedshiftSettingsTypeDef",
     "S3SettingsTypeDef",
     "SybaseSettingsTypeDef",
     "EventSubscriptionTypeDef",
     "CreateFleetAdvisorCollectorRequestRequestTypeDef",
-    "CreateFleetAdvisorCollectorResponseTypeDef",
+    "TimestampTypeDef",
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     "ServerShortInfoResponseTypeDef",
     "DatabaseShortInfoResponseTypeDef",
     "DeleteCertificateMessageRequestTypeDef",
     "DeleteCollectorRequestRequestTypeDef",
     "DeleteConnectionMessageRequestTypeDef",
     "DeleteEndpointMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
     "DeleteReplicationInstanceMessageRequestTypeDef",
     "DeleteReplicationSubnetGroupMessageRequestTypeDef",
     "DeleteReplicationTaskAssessmentRunMessageRequestTypeDef",
     "DeleteReplicationTaskMessageRequestTypeDef",
     "DescribeApplicableIndividualAssessmentsMessageRequestTypeDef",
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEndpointSettingsMessageRequestTypeDef",
     "EndpointSettingTypeDef",
     "SupportedEndpointTypeTypeDef",
     "EventCategoryGroupTypeDef",
     "EventTypeDef",
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
     "FleetAdvisorLsaAnalysisResponseTypeDef",
     "FleetAdvisorSchemaObjectResponseTypeDef",
-    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     "OrderableReplicationInstanceTypeDef",
     "LimitationTypeDef",
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     "RefreshSchemasStatusTypeDef",
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
     "ReplicationInstanceTaskLogTypeDef",
-    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     "ReplicationTaskAssessmentResultTypeDef",
     "ReplicationTaskIndividualAssessmentTypeDef",
-    "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
-    "DescribeSchemasResponseTypeDef",
     "TableStatisticsTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "OracleSettingsOutputTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
-    "ModifyReplicationTaskMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RdsConfigurationTypeDef",
     "RdsRequirementsTypeDef",
     "RebootReplicationInstanceMessageRequestTypeDef",
     "RecommendationSettingsTypeDef",
     "RefreshSchemasMessageRequestTypeDef",
     "TableToReloadTypeDef",
-    "ReloadTablesResponseTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "ReplicationPendingModifiedValuesTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ReplicationTaskAssessmentRunProgressTypeDef",
     "ReplicationTaskStatsTypeDef",
-    "ResponseMetadataTypeDef",
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
     "SchemaShortInfoResponseTypeDef",
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     "StartReplicationTaskAssessmentRunMessageRequestTypeDef",
-    "StartReplicationTaskMessageRequestTypeDef",
     "StopReplicationTaskMessageRequestTypeDef",
     "TestConnectionMessageRequestTypeDef",
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateReplicationInstanceMessageRequestTypeDef",
     "CreateReplicationSubnetGroupMessageRequestTypeDef",
-    "CreateReplicationTaskMessageRequestTypeDef",
-    "ImportCertificateMessageRequestTypeDef",
+    "CreateFleetAdvisorCollectorResponseTypeDef",
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
+    "DescribeSchemasResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ReloadTablesResponseTypeDef",
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
     "SubnetTypeDef",
     "BatchStartRecommendationsResponseTypeDef",
+    "ImportCertificateMessageRequestTypeDef",
     "DeleteCertificateResponseTypeDef",
     "DescribeCertificatesResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "CollectorResponseTypeDef",
     "DeleteConnectionResponseTypeDef",
     "DescribeConnectionsResponseTypeDef",
     "TestConnectionResponseTypeDef",
     "CreateEndpointMessageRequestTypeDef",
-    "EndpointTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
     "CreateEventSubscriptionResponseTypeDef",
     "DeleteEventSubscriptionResponseTypeDef",
     "DescribeEventSubscriptionsResponseTypeDef",
     "ModifyEventSubscriptionResponseTypeDef",
+    "CreateReplicationTaskMessageRequestTypeDef",
+    "ModifyReplicationTaskMessageRequestTypeDef",
+    "StartReplicationTaskMessageRequestTypeDef",
     "DatabaseResponseTypeDef",
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
-    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     "DescribeConnectionsMessageRequestTypeDef",
-    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     "DescribeEndpointTypesMessageRequestTypeDef",
-    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
     "DescribeEndpointsMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
     "DescribeFleetAdvisorCollectorsRequestRequestTypeDef",
     "DescribeFleetAdvisorDatabasesRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemasRequestRequestTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "DescribeRecommendationLimitationsRequestRequestTypeDef",
     "DescribeRecommendationsRequestRequestTypeDef",
-    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
     "DescribeReplicationInstancesMessageRequestTypeDef",
-    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
     "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
     "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
-    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
     "DescribeReplicationTasksMessageRequestTypeDef",
-    "DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     "DescribeTableStatisticsMessageRequestTypeDef",
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
+    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
+    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
+    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
+    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
+    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
+    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
+    "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    "DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     "DescribeEndpointsMessageEndpointDeletedWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef",
@@ -240,29 +241,31 @@
     "DescribeRecommendationLimitationsResponseTypeDef",
     "DescribeRefreshSchemasStatusResponseTypeDef",
     "RefreshSchemasResponseTypeDef",
     "DescribeReplicationInstanceTaskLogsResponseTypeDef",
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
     "DescribeTableStatisticsResponseTypeDef",
+    "EndpointTypeDef",
+    "OracleSettingsUnionTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "RdsRecommendationTypeDef",
     "StartRecommendationsRequestEntryTypeDef",
     "StartRecommendationsRequestRequestTypeDef",
     "ReloadTablesMessageRequestTypeDef",
     "ReplicationTaskAssessmentRunTypeDef",
     "ReplicationTaskTypeDef",
     "SchemaResponseTypeDef",
     "ReplicationSubnetGroupTypeDef",
     "DescribeFleetAdvisorCollectorsResponseTypeDef",
+    "DescribeFleetAdvisorDatabasesResponseTypeDef",
     "CreateEndpointResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ModifyEndpointResponseTypeDef",
-    "DescribeFleetAdvisorDatabasesResponseTypeDef",
     "ApplyPendingMaintenanceActionResponseTypeDef",
     "DescribePendingMaintenanceActionsResponseTypeDef",
     "RecommendationDataTypeDef",
     "BatchStartRecommendationsRequestRequestTypeDef",
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
@@ -314,14 +317,25 @@
     {
         "ReplicationInstanceArn": str,
         "ApplyAction": str,
         "OptInType": str,
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
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -332,14 +346,15 @@
         "DatabaseId": str,
         "Message": str,
         "Code": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelReplicationTaskAssessmentRunMessageRequestTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
     },
 )
 
@@ -449,21 +464,19 @@
         "FullLoadErrorPercentage": int,
         "ErrorRetryDuration": int,
         "UseNewMappingType": bool,
     },
     total=False,
 )
 
-
 class ElasticsearchSettingsTypeDef(
     _RequiredElasticsearchSettingsTypeDef, _OptionalElasticsearchSettingsTypeDef
 ):
     pass
 
-
 GcpMySQLSettingsTypeDef = TypedDict(
     "GcpMySQLSettingsTypeDef",
     {
         "AfterConnectScript": str,
         "CleanSourceMetadataOnMismatch": bool,
         "DatabaseName": str,
         "EventsPollInterval": int,
@@ -622,19 +635,17 @@
         "MaxFileSize": int,
         "MaxRetryCount": int,
         "IamAuthEnabled": bool,
     },
     total=False,
 )
 
-
 class NeptuneSettingsTypeDef(_RequiredNeptuneSettingsTypeDef, _OptionalNeptuneSettingsTypeDef):
     pass
 
-
 OracleSettingsTypeDef = TypedDict(
     "OracleSettingsTypeDef",
     {
         "AddSupplementalLogging": bool,
         "ArchivedLogDestId": int,
         "AdditionalArchivedLogDestId": int,
         "ExtraArchivedLogDestIds": Sequence[int],
@@ -722,19 +733,17 @@
         "AuthUserName": str,
         "AuthPassword": str,
         "SslCaCertificateArn": str,
     },
     total=False,
 )
 
-
 class RedisSettingsTypeDef(_RequiredRedisSettingsTypeDef, _OptionalRedisSettingsTypeDef):
     pass
 
-
 RedshiftSettingsTypeDef = TypedDict(
     "RedshiftSettingsTypeDef",
     {
         "AcceptAnyDate": bool,
         "AfterConnectScript": str,
         "BucketFolder": str,
         "BucketName": str,
@@ -859,34 +868,21 @@
     "_OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateFleetAdvisorCollectorRequestRequestTypeDef(
     _RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef,
     _OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef,
 ):
     pass
 
-
-CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
-    "CreateFleetAdvisorCollectorResponseTypeDef",
-    {
-        "CollectorReferencedId": str,
-        "CollectorName": str,
-        "Description": str,
-        "ServiceAccessRoleArn": str,
-        "S3BucketName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 DatabaseInstanceSoftwareDetailsResponseTypeDef = TypedDict(
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "EngineEdition": str,
         "ServicePack": str,
@@ -957,22 +953,14 @@
 DeleteFleetAdvisorDatabasesRequestRequestTypeDef = TypedDict(
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
     {
         "DatabaseIds": Sequence[str],
     },
 )
 
-DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
-    {
-        "DatabaseIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteReplicationInstanceMessageRequestTypeDef = TypedDict(
     "DeleteReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
 )
 
@@ -1007,31 +995,32 @@
         "MigrationType": MigrationTypeValueType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
-    {
-        "IndividualAssessmentNames": List[str],
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FilterTypeDef = TypedDict(
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
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1048,22 +1037,20 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeEndpointSettingsMessageRequestTypeDef(
     _RequiredDescribeEndpointSettingsMessageRequestTypeDef,
     _OptionalDescribeEndpointSettingsMessageRequestTypeDef,
 ):
     pass
 
-
 EndpointSettingTypeDef = TypedDict(
     "EndpointSettingTypeDef",
     {
         "Name": str,
         "Type": EndpointSettingTypeValueType,
         "EnumValues": List[str],
         "Sensitive": bool,
@@ -1135,22 +1122,14 @@
         "NumberOfObjects": int,
         "CodeLineCount": int,
         "CodeSize": int,
     },
     total=False,
 )
 
-DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = TypedDict(
-    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrderableReplicationInstancesMessageRequestTypeDef = TypedDict(
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
@@ -1215,41 +1194,30 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeReplicationInstanceTaskLogsMessageRequestTypeDef(
     _RequiredDescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     _OptionalDescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
 ):
     pass
 
-
 ReplicationInstanceTaskLogTypeDef = TypedDict(
     "ReplicationInstanceTaskLogTypeDef",
     {
         "ReplicationTaskName": str,
         "ReplicationTaskArn": str,
         "ReplicationInstanceTaskLogSize": int,
     },
     total=False,
 )
 
-DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
-    {
-        "ReplicationTaskArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1278,36 +1246,14 @@
         "IndividualAssessmentName": str,
         "Status": str,
         "ReplicationTaskIndividualAssessmentStartDate": datetime,
     },
     total=False,
 )
 
-_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
-    {
-        "EndpointArn": str,
-    },
-)
-_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
-    _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
-    _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeSchemasMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemasMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 _OptionalDescribeSchemasMessageRequestTypeDef = TypedDict(
@@ -1315,30 +1261,19 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeSchemasMessageRequestTypeDef(
     _RequiredDescribeSchemasMessageRequestTypeDef, _OptionalDescribeSchemasMessageRequestTypeDef
 ):
     pass
 
-
-DescribeSchemasResponseTypeDef = TypedDict(
-    "DescribeSchemasResponseTypeDef",
-    {
-        "Marker": str,
-        "Schemas": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TableStatisticsTypeDef = TypedDict(
     "TableStatisticsTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
         "Inserts": int,
         "Deletes": int,
@@ -1361,19 +1296,61 @@
         "ValidationSuspendedRecords": int,
         "ValidationState": str,
         "ValidationStateDetails": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+OracleSettingsOutputTypeDef = TypedDict(
+    "OracleSettingsOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AddSupplementalLogging": bool,
+        "ArchivedLogDestId": int,
+        "AdditionalArchivedLogDestId": int,
+        "ExtraArchivedLogDestIds": List[int],
+        "AllowSelectNestedTables": bool,
+        "ParallelAsmReadThreads": int,
+        "ReadAheadBlocks": int,
+        "AccessAlternateDirectly": bool,
+        "UseAlternateFolderForOnline": bool,
+        "OraclePathPrefix": str,
+        "UsePathPrefix": str,
+        "ReplacePathPrefix": bool,
+        "EnableHomogenousTablespace": bool,
+        "DirectPathNoLog": bool,
+        "ArchivedLogsOnly": bool,
+        "AsmPassword": str,
+        "AsmServer": str,
+        "AsmUser": str,
+        "CharLengthSemantics": CharLengthSemanticsType,
+        "DatabaseName": str,
+        "DirectPathParallelLoad": bool,
+        "FailTasksOnLobTruncation": bool,
+        "NumberDatatypeScale": int,
+        "Password": str,
+        "Port": int,
+        "ReadTableSpaceName": bool,
+        "RetryInterval": int,
+        "SecurityDbEncryption": str,
+        "SecurityDbEncryptionName": str,
+        "ServerName": str,
+        "SpatialDataOptionToGeoJsonFunctionName": str,
+        "StandbyDelayTime": int,
+        "Username": str,
+        "UseBFile": bool,
+        "UseDirectPathFullLoad": bool,
+        "UseLogminerReader": bool,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "SecretsManagerOracleAsmAccessRoleArn": str,
+        "SecretsManagerOracleAsmSecretId": str,
+        "TrimSpaceInChar": bool,
+        "ConvertTimestampWithZoneToUTC": bool,
     },
+    total=False,
 )
 
 ListTagsForResourceMessageRequestTypeDef = TypedDict(
     "ListTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceArnList": Sequence[str],
@@ -1394,22 +1371,20 @@
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
 _RequiredModifyReplicationInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
 )
 _OptionalModifyReplicationInstanceMessageRequestTypeDef = TypedDict(
@@ -1426,22 +1401,20 @@
         "AutoMinorVersionUpgrade": bool,
         "ReplicationInstanceIdentifier": str,
         "NetworkType": str,
     },
     total=False,
 )
 
-
 class ModifyReplicationInstanceMessageRequestTypeDef(
     _RequiredModifyReplicationInstanceMessageRequestTypeDef,
     _OptionalModifyReplicationInstanceMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyReplicationSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationSubnetGroupMessageRequestTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -1449,69 +1422,28 @@
     "_OptionalModifyReplicationSubnetGroupMessageRequestTypeDef",
     {
         "ReplicationSubnetGroupDescription": str,
     },
     total=False,
 )
 
-
 class ModifyReplicationSubnetGroupMessageRequestTypeDef(
     _RequiredModifyReplicationSubnetGroupMessageRequestTypeDef,
     _OptionalModifyReplicationSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
-_RequiredModifyReplicationTaskMessageRequestTypeDef = TypedDict(
-    "_RequiredModifyReplicationTaskMessageRequestTypeDef",
-    {
-        "ReplicationTaskArn": str,
-    },
-)
-_OptionalModifyReplicationTaskMessageRequestTypeDef = TypedDict(
-    "_OptionalModifyReplicationTaskMessageRequestTypeDef",
-    {
-        "ReplicationTaskIdentifier": str,
-        "MigrationType": MigrationTypeValueType,
-        "TableMappings": str,
-        "ReplicationTaskSettings": str,
-        "CdcStartTime": Union[datetime, str],
-        "CdcStartPosition": str,
-        "CdcStopPosition": str,
-        "TaskData": str,
-    },
-    total=False,
-)
-
-
-class ModifyReplicationTaskMessageRequestTypeDef(
-    _RequiredModifyReplicationTaskMessageRequestTypeDef,
-    _OptionalModifyReplicationTaskMessageRequestTypeDef,
-):
-    pass
-
-
 MoveReplicationTaskMessageRequestTypeDef = TypedDict(
     "MoveReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "TargetReplicationInstanceArn": str,
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
@@ -1560,22 +1492,20 @@
     {
         "ForceFailover": bool,
         "ForcePlannedFailover": bool,
     },
     total=False,
 )
 
-
 class RebootReplicationInstanceMessageRequestTypeDef(
     _RequiredRebootReplicationInstanceMessageRequestTypeDef,
     _OptionalRebootReplicationInstanceMessageRequestTypeDef,
 ):
     pass
 
-
 RecommendationSettingsTypeDef = TypedDict(
     "RecommendationSettingsTypeDef",
     {
         "InstanceSizingType": str,
         "WorkloadType": str,
     },
 )
@@ -1592,22 +1522,14 @@
     "TableToReloadTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
     },
 )
 
-ReloadTablesResponseTypeDef = TypedDict(
-    "ReloadTablesResponseTypeDef",
-    {
-        "ReplicationTaskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromResourceMessageRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1656,34 +1578,14 @@
         "StopDate": datetime,
         "FullLoadStartDate": datetime,
         "FullLoadFinishDate": datetime,
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
-RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
-    {
-        "LsaAnalysisId": str,
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SchemaShortInfoResponseTypeDef = TypedDict(
     "SchemaShortInfoResponseTypeDef",
     {
         "SchemaId": str,
         "SchemaName": str,
         "DatabaseId": str,
         "DatabaseName": str,
@@ -1716,47 +1618,20 @@
         "ResultKmsKeyArn": str,
         "IncludeOnly": Sequence[str],
         "Exclude": Sequence[str],
     },
     total=False,
 )
 
-
 class StartReplicationTaskAssessmentRunMessageRequestTypeDef(
     _RequiredStartReplicationTaskAssessmentRunMessageRequestTypeDef,
     _OptionalStartReplicationTaskAssessmentRunMessageRequestTypeDef,
 ):
     pass
 
-
-_RequiredStartReplicationTaskMessageRequestTypeDef = TypedDict(
-    "_RequiredStartReplicationTaskMessageRequestTypeDef",
-    {
-        "ReplicationTaskArn": str,
-        "StartReplicationTaskType": StartReplicationTaskTypeValueType,
-    },
-)
-_OptionalStartReplicationTaskMessageRequestTypeDef = TypedDict(
-    "_OptionalStartReplicationTaskMessageRequestTypeDef",
-    {
-        "CdcStartTime": Union[datetime, str],
-        "CdcStartPosition": str,
-        "CdcStopPosition": str,
-    },
-    total=False,
-)
-
-
-class StartReplicationTaskMessageRequestTypeDef(
-    _RequiredStartReplicationTaskMessageRequestTypeDef,
-    _OptionalStartReplicationTaskMessageRequestTypeDef,
-):
-    pass
-
-
 StopReplicationTaskMessageRequestTypeDef = TypedDict(
     "StopReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
 
@@ -1772,31 +1647,14 @@
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
     {
         "ForceMove": bool,
     },
     total=False,
 )
 
-UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
-    {
-        "Result": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
-    {
-        "AccountQuotas": List[AccountQuotaTypeDef],
-        "UniqueAccountIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1816,22 +1674,20 @@
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
 _RequiredCreateReplicationInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
         "ReplicationInstanceClass": str,
     },
 )
@@ -1852,22 +1708,20 @@
         "DnsNameServers": str,
         "ResourceIdentifier": str,
         "NetworkType": str,
     },
     total=False,
 )
 
-
 class CreateReplicationInstanceMessageRequestTypeDef(
     _RequiredCreateReplicationInstanceMessageRequestTypeDef,
     _OptionalCreateReplicationInstanceMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateReplicationSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationSubnetGroupMessageRequestTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "ReplicationSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -1876,83 +1730,104 @@
     "_OptionalCreateReplicationSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateReplicationSubnetGroupMessageRequestTypeDef(
     _RequiredCreateReplicationSubnetGroupMessageRequestTypeDef,
     _OptionalCreateReplicationSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
-_RequiredCreateReplicationTaskMessageRequestTypeDef = TypedDict(
-    "_RequiredCreateReplicationTaskMessageRequestTypeDef",
+CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
+    "CreateFleetAdvisorCollectorResponseTypeDef",
     {
-        "ReplicationTaskIdentifier": str,
-        "SourceEndpointArn": str,
-        "TargetEndpointArn": str,
-        "ReplicationInstanceArn": str,
-        "MigrationType": MigrationTypeValueType,
-        "TableMappings": str,
+        "CollectorReferencedId": str,
+        "CollectorName": str,
+        "Description": str,
+        "ServiceAccessRoleArn": str,
+        "S3BucketName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateReplicationTaskMessageRequestTypeDef = TypedDict(
-    "_OptionalCreateReplicationTaskMessageRequestTypeDef",
+
+DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
     {
-        "ReplicationTaskSettings": str,
-        "CdcStartTime": Union[datetime, str],
-        "CdcStartPosition": str,
-        "CdcStopPosition": str,
-        "Tags": Sequence[TagTypeDef],
-        "TaskData": str,
-        "ResourceIdentifier": str,
+        "DatabaseIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateReplicationTaskMessageRequestTypeDef(
-    _RequiredCreateReplicationTaskMessageRequestTypeDef,
-    _OptionalCreateReplicationTaskMessageRequestTypeDef,
-):
-    pass
-
-
-_RequiredImportCertificateMessageRequestTypeDef = TypedDict(
-    "_RequiredImportCertificateMessageRequestTypeDef",
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
     {
-        "CertificateIdentifier": str,
+        "AccountQuotas": List[AccountQuotaTypeDef],
+        "UniqueAccountIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalImportCertificateMessageRequestTypeDef = TypedDict(
-    "_OptionalImportCertificateMessageRequestTypeDef",
+
+DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     {
-        "CertificatePem": str,
-        "CertificateWallet": Union[str, bytes, IO[Any], StreamingBody],
-        "Tags": Sequence[TagTypeDef],
+        "IndividualAssessmentNames": List[str],
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+DescribeSchemasResponseTypeDef = TypedDict(
+    "DescribeSchemasResponseTypeDef",
+    {
+        "Marker": str,
+        "Schemas": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ImportCertificateMessageRequestTypeDef(
-    _RequiredImportCertificateMessageRequestTypeDef, _OptionalImportCertificateMessageRequestTypeDef
-):
-    pass
-
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReloadTablesResponseTypeDef = TypedDict(
+    "ReloadTablesResponseTypeDef",
+    {
+        "ReplicationTaskArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
+    {
+        "LsaAnalysisId": str,
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
@@ -1962,40 +1837,61 @@
     total=False,
 )
 
 BatchStartRecommendationsResponseTypeDef = TypedDict(
     "BatchStartRecommendationsResponseTypeDef",
     {
         "ErrorEntries": List[BatchStartRecommendationsErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredImportCertificateMessageRequestTypeDef = TypedDict(
+    "_RequiredImportCertificateMessageRequestTypeDef",
+    {
+        "CertificateIdentifier": str,
+    },
+)
+_OptionalImportCertificateMessageRequestTypeDef = TypedDict(
+    "_OptionalImportCertificateMessageRequestTypeDef",
+    {
+        "CertificatePem": str,
+        "CertificateWallet": BlobTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class ImportCertificateMessageRequestTypeDef(
+    _RequiredImportCertificateMessageRequestTypeDef, _OptionalImportCertificateMessageRequestTypeDef
+):
+    pass
+
 DeleteCertificateResponseTypeDef = TypedDict(
     "DeleteCertificateResponseTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificatesResponseTypeDef = TypedDict(
     "DescribeCertificatesResponseTypeDef",
     {
         "Marker": str,
         "Certificates": List[CertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportCertificateResponseTypeDef = TypedDict(
     "ImportCertificateResponseTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CollectorResponseTypeDef = TypedDict(
     "CollectorResponseTypeDef",
     {
         "CollectorReferencedId": str,
@@ -2015,32 +1911,32 @@
     total=False,
 )
 
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectionsResponseTypeDef = TypedDict(
     "DescribeConnectionsResponseTypeDef",
     {
         "Marker": str,
         "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestConnectionResponseTypeDef = TypedDict(
     "TestConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointMessageRequestTypeDef",
     {
         "EndpointIdentifier": str,
@@ -2082,63 +1978,19 @@
         "DocDbSettings": DocDbSettingsTypeDef,
         "RedisSettings": RedisSettingsTypeDef,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
     },
     total=False,
 )
 
-
 class CreateEndpointMessageRequestTypeDef(
     _RequiredCreateEndpointMessageRequestTypeDef, _OptionalCreateEndpointMessageRequestTypeDef
 ):
     pass
 
-
-EndpointTypeDef = TypedDict(
-    "EndpointTypeDef",
-    {
-        "EndpointIdentifier": str,
-        "EndpointType": ReplicationEndpointTypeValueType,
-        "EngineName": str,
-        "EngineDisplayName": str,
-        "Username": str,
-        "ServerName": str,
-        "Port": int,
-        "DatabaseName": str,
-        "ExtraConnectionAttributes": str,
-        "Status": str,
-        "KmsKeyId": str,
-        "EndpointArn": str,
-        "CertificateArn": str,
-        "SslMode": DmsSslModeValueType,
-        "ServiceAccessRoleArn": str,
-        "ExternalTableDefinition": str,
-        "ExternalId": str,
-        "DynamoDbSettings": DynamoDbSettingsTypeDef,
-        "S3Settings": S3SettingsTypeDef,
-        "DmsTransferSettings": DmsTransferSettingsTypeDef,
-        "MongoDbSettings": MongoDbSettingsTypeDef,
-        "KinesisSettings": KinesisSettingsTypeDef,
-        "KafkaSettings": KafkaSettingsTypeDef,
-        "ElasticsearchSettings": ElasticsearchSettingsTypeDef,
-        "NeptuneSettings": NeptuneSettingsTypeDef,
-        "RedshiftSettings": RedshiftSettingsTypeDef,
-        "PostgreSQLSettings": PostgreSQLSettingsTypeDef,
-        "MySQLSettings": MySQLSettingsTypeDef,
-        "OracleSettings": OracleSettingsTypeDef,
-        "SybaseSettings": SybaseSettingsTypeDef,
-        "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
-        "IBMDb2Settings": IBMDb2SettingsTypeDef,
-        "DocDbSettings": DocDbSettingsTypeDef,
-        "RedisSettings": RedisSettingsTypeDef,
-        "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredModifyEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 _OptionalModifyEndpointMessageRequestTypeDef = TypedDict(
@@ -2176,134 +2028,177 @@
         "RedisSettings": RedisSettingsTypeDef,
         "ExactSettings": bool,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
     },
     total=False,
 )
 
-
 class ModifyEndpointMessageRequestTypeDef(
     _RequiredModifyEndpointMessageRequestTypeDef, _OptionalModifyEndpointMessageRequestTypeDef
 ):
     pass
 
-
 CreateEventSubscriptionResponseTypeDef = TypedDict(
     "CreateEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventSubscriptionResponseTypeDef = TypedDict(
     "DeleteEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventSubscriptionsResponseTypeDef = TypedDict(
     "DescribeEventSubscriptionsResponseTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyEventSubscriptionResponseTypeDef = TypedDict(
     "ModifyEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DatabaseResponseTypeDef = TypedDict(
-    "DatabaseResponseTypeDef",
+_RequiredCreateReplicationTaskMessageRequestTypeDef = TypedDict(
+    "_RequiredCreateReplicationTaskMessageRequestTypeDef",
     {
-        "DatabaseId": str,
-        "DatabaseName": str,
-        "IpAddress": str,
-        "NumberOfSchemas": int,
-        "Server": ServerShortInfoResponseTypeDef,
-        "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseTypeDef,
-        "Collectors": List[CollectorShortInfoResponseTypeDef],
+        "ReplicationTaskIdentifier": str,
+        "SourceEndpointArn": str,
+        "TargetEndpointArn": str,
+        "ReplicationInstanceArn": str,
+        "MigrationType": MigrationTypeValueType,
+        "TableMappings": str,
+    },
+)
+_OptionalCreateReplicationTaskMessageRequestTypeDef = TypedDict(
+    "_OptionalCreateReplicationTaskMessageRequestTypeDef",
+    {
+        "ReplicationTaskSettings": str,
+        "CdcStartTime": TimestampTypeDef,
+        "CdcStartPosition": str,
+        "CdcStopPosition": str,
+        "Tags": Sequence[TagTypeDef],
+        "TaskData": str,
+        "ResourceIdentifier": str,
     },
     total=False,
 )
 
-DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+class CreateReplicationTaskMessageRequestTypeDef(
+    _RequiredCreateReplicationTaskMessageRequestTypeDef,
+    _OptionalCreateReplicationTaskMessageRequestTypeDef,
+):
+    pass
+
+_RequiredModifyReplicationTaskMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyReplicationTaskMessageRequestTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ReplicationTaskArn": str,
+    },
+)
+_OptionalModifyReplicationTaskMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyReplicationTaskMessageRequestTypeDef",
+    {
+        "ReplicationTaskIdentifier": str,
+        "MigrationType": MigrationTypeValueType,
+        "TableMappings": str,
+        "ReplicationTaskSettings": str,
+        "CdcStartTime": TimestampTypeDef,
+        "CdcStartPosition": str,
+        "CdcStopPosition": str,
+        "TaskData": str,
     },
     total=False,
 )
 
-DescribeCertificatesMessageRequestTypeDef = TypedDict(
-    "DescribeCertificatesMessageRequestTypeDef",
+class ModifyReplicationTaskMessageRequestTypeDef(
+    _RequiredModifyReplicationTaskMessageRequestTypeDef,
+    _OptionalModifyReplicationTaskMessageRequestTypeDef,
+):
+    pass
+
+_RequiredStartReplicationTaskMessageRequestTypeDef = TypedDict(
+    "_RequiredStartReplicationTaskMessageRequestTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "ReplicationTaskArn": str,
+        "StartReplicationTaskType": StartReplicationTaskTypeValueType,
+    },
+)
+_OptionalStartReplicationTaskMessageRequestTypeDef = TypedDict(
+    "_OptionalStartReplicationTaskMessageRequestTypeDef",
+    {
+        "CdcStartTime": TimestampTypeDef,
+        "CdcStartPosition": str,
+        "CdcStopPosition": str,
     },
     total=False,
 )
 
-DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = TypedDict(
-    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
+class StartReplicationTaskMessageRequestTypeDef(
+    _RequiredStartReplicationTaskMessageRequestTypeDef,
+    _OptionalStartReplicationTaskMessageRequestTypeDef,
+):
+    pass
+
+DatabaseResponseTypeDef = TypedDict(
+    "DatabaseResponseTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "DatabaseId": str,
+        "DatabaseName": str,
+        "IpAddress": str,
+        "NumberOfSchemas": int,
+        "Server": ServerShortInfoResponseTypeDef,
+        "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseTypeDef,
+        "Collectors": List[CollectorShortInfoResponseTypeDef],
     },
     total=False,
 )
 
-DescribeConnectionsMessageRequestTypeDef = TypedDict(
-    "DescribeConnectionsMessageRequestTypeDef",
+DescribeCertificatesMessageRequestTypeDef = TypedDict(
+    "DescribeCertificatesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = TypedDict(
-    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
+DescribeConnectionsMessageRequestTypeDef = TypedDict(
+    "DescribeConnectionsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
 DescribeEndpointTypesMessageRequestTypeDef = TypedDict(
     "DescribeEndpointTypesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeEndpointsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2315,57 +2210,32 @@
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": Literal["replication-instance"],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": Literal["replication-instance"],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Duration": int,
         "EventCategories": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
@@ -2438,139 +2308,233 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = TypedDict(
-    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
+DescribeReplicationInstancesMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationInstancesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationInstancesMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationInstancesMessageRequestTypeDef",
+DescribeReplicationSubnetGroupsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
+DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationSubnetGroupsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
+DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
+DescribeReplicationTasksMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTasksMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
+        "WithoutSettings": bool,
     },
     total=False,
 )
 
-DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
+_RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
+    {
+        "ReplicationTaskArn": str,
+    },
+)
+_OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeTableStatisticsMessageRequestTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
+        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = TypedDict(
-    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
+class DescribeTableStatisticsMessageRequestTypeDef(
+    _RequiredDescribeTableStatisticsMessageRequestTypeDef,
+    _OptionalDescribeTableStatisticsMessageRequestTypeDef,
+):
+    pass
+
+DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "WithoutSettings": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeReplicationTasksMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTasksMessageRequestTypeDef",
+DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = TypedDict(
+    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-        "WithoutSettings": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = TypedDict(
+    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     {
-        "ReplicationTaskArn": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+
+DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
-    _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
-    _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
-):
-    pass
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": Literal["replication-instance"],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Duration": int,
+        "EventCategories": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
+DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = TypedDict(
+    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-_RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
+DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = TypedDict(
+    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     {
         "ReplicationTaskArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeTableStatisticsMessageRequestTypeDef",
+
+DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = TypedDict(
+    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
     {
-        "MaxRecords": int,
-        "Marker": str,
         "Filters": Sequence[FilterTypeDef],
+        "WithoutSettings": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    {
+        "EndpointArn": str,
+    },
+)
+_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class DescribeTableStatisticsMessageRequestTypeDef(
-    _RequiredDescribeTableStatisticsMessageRequestTypeDef,
-    _OptionalDescribeTableStatisticsMessageRequestTypeDef,
+class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
+    _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+    _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
 ):
     pass
 
+_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+    {
+        "ReplicationTaskArn": str,
+    },
+)
+_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
+    _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+    _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+):
+    pass
 
 DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef = TypedDict(
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
@@ -2661,135 +2625,178 @@
 )
 
 DescribeEndpointSettingsResponseTypeDef = TypedDict(
     "DescribeEndpointSettingsResponseTypeDef",
     {
         "Marker": str,
         "EndpointSettings": List[EndpointSettingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointTypesResponseTypeDef = TypedDict(
     "DescribeEndpointTypesResponseTypeDef",
     {
         "Marker": str,
         "SupportedEndpointTypes": List[SupportedEndpointTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventCategoriesResponseTypeDef = TypedDict(
     "DescribeEventCategoriesResponseTypeDef",
     {
         "EventCategoryGroupList": List[EventCategoryGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
     {
         "Analysis": List[FleetAdvisorLsaAnalysisResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
     {
         "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrderableReplicationInstancesResponseTypeDef = TypedDict(
     "DescribeOrderableReplicationInstancesResponseTypeDef",
     {
         "OrderableReplicationInstances": List[OrderableReplicationInstanceTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecommendationLimitationsResponseTypeDef = TypedDict(
     "DescribeRecommendationLimitationsResponseTypeDef",
     {
         "NextToken": str,
         "Limitations": List[LimitationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRefreshSchemasStatusResponseTypeDef = TypedDict(
     "DescribeRefreshSchemasStatusResponseTypeDef",
     {
         "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RefreshSchemasResponseTypeDef = TypedDict(
     "RefreshSchemasResponseTypeDef",
     {
         "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationInstanceTaskLogsResponseTypeDef = TypedDict(
     "DescribeReplicationInstanceTaskLogsResponseTypeDef",
     {
         "ReplicationInstanceArn": str,
         "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationTaskAssessmentResultsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     {
         "Marker": str,
         "BucketName": str,
         "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationTaskIndividualAssessmentsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTaskIndividualAssessments": List[ReplicationTaskIndividualAssessmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableStatisticsResponseTypeDef = TypedDict(
     "DescribeTableStatisticsResponseTypeDef",
     {
         "ReplicationTaskArn": str,
         "TableStatistics": List[TableStatisticsTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EndpointTypeDef = TypedDict(
+    "EndpointTypeDef",
+    {
+        "EndpointIdentifier": str,
+        "EndpointType": ReplicationEndpointTypeValueType,
+        "EngineName": str,
+        "EngineDisplayName": str,
+        "Username": str,
+        "ServerName": str,
+        "Port": int,
+        "DatabaseName": str,
+        "ExtraConnectionAttributes": str,
+        "Status": str,
+        "KmsKeyId": str,
+        "EndpointArn": str,
+        "CertificateArn": str,
+        "SslMode": DmsSslModeValueType,
+        "ServiceAccessRoleArn": str,
+        "ExternalTableDefinition": str,
+        "ExternalId": str,
+        "DynamoDbSettings": DynamoDbSettingsTypeDef,
+        "S3Settings": S3SettingsTypeDef,
+        "DmsTransferSettings": DmsTransferSettingsTypeDef,
+        "MongoDbSettings": MongoDbSettingsTypeDef,
+        "KinesisSettings": KinesisSettingsTypeDef,
+        "KafkaSettings": KafkaSettingsTypeDef,
+        "ElasticsearchSettings": ElasticsearchSettingsTypeDef,
+        "NeptuneSettings": NeptuneSettingsTypeDef,
+        "RedshiftSettings": RedshiftSettingsTypeDef,
+        "PostgreSQLSettings": PostgreSQLSettingsTypeDef,
+        "MySQLSettings": MySQLSettingsTypeDef,
+        "OracleSettings": OracleSettingsOutputTypeDef,
+        "SybaseSettings": SybaseSettingsTypeDef,
+        "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
+        "IBMDb2Settings": IBMDb2SettingsTypeDef,
+        "DocDbSettings": DocDbSettingsTypeDef,
+        "RedisSettings": RedisSettingsTypeDef,
+        "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
+    },
+    total=False,
+)
+
+OracleSettingsUnionTypeDef = Union[OracleSettingsTypeDef, OracleSettingsOutputTypeDef]
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
     total=False,
@@ -2831,21 +2838,19 @@
     "_OptionalReloadTablesMessageRequestTypeDef",
     {
         "ReloadOption": ReloadOptionValueType,
     },
     total=False,
 )
 
-
 class ReloadTablesMessageRequestTypeDef(
     _RequiredReloadTablesMessageRequestTypeDef, _OptionalReloadTablesMessageRequestTypeDef
 ):
     pass
 
-
 ReplicationTaskAssessmentRunTypeDef = TypedDict(
     "ReplicationTaskAssessmentRunTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
         "ReplicationTaskArn": str,
         "Status": str,
         "ReplicationTaskAssessmentRunCreationDate": datetime,
@@ -2917,74 +2922,74 @@
 )
 
 DescribeFleetAdvisorCollectorsResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorCollectorsResponseTypeDef",
     {
         "Collectors": List[CollectorResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorDatabasesResponseTypeDef",
+    {
+        "Databases": List[DatabaseResponseTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Marker": str,
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyEndpointResponseTypeDef = TypedDict(
     "ModifyEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorDatabasesResponseTypeDef",
-    {
-        "Databases": List[DatabaseResponseTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplyPendingMaintenanceActionResponseTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResponseTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePendingMaintenanceActionsResponseTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsResponseTypeDef",
     {
         "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationDataTypeDef = TypedDict(
     "RecommendationDataTypeDef",
     {
         "RdsEngine": RdsRecommendationTypeDef,
@@ -3000,139 +3005,139 @@
     total=False,
 )
 
 CancelReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationTaskAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "StartReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateReplicationTaskResponseTypeDef = TypedDict(
     "CreateReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteReplicationTaskResponseTypeDef = TypedDict(
     "DeleteReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationTasksResponseTypeDef = TypedDict(
     "DescribeReplicationTasksResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTasks": List[ReplicationTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationTaskResponseTypeDef = TypedDict(
     "ModifyReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MoveReplicationTaskResponseTypeDef = TypedDict(
     "MoveReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartReplicationTaskAssessmentResponseTypeDef = TypedDict(
     "StartReplicationTaskAssessmentResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartReplicationTaskResponseTypeDef = TypedDict(
     "StartReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopReplicationTaskResponseTypeDef = TypedDict(
     "StopReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFleetAdvisorSchemasResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorSchemasResponseTypeDef",
     {
         "FleetAdvisorSchemas": List[SchemaResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateReplicationSubnetGroupResponseTypeDef = TypedDict(
     "CreateReplicationSubnetGroupResponseTypeDef",
     {
         "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationSubnetGroupsResponseTypeDef = TypedDict(
     "DescribeReplicationSubnetGroupsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationSubnetGroups": List[ReplicationSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationSubnetGroupResponseTypeDef = TypedDict(
     "ModifyReplicationSubnetGroupResponseTypeDef",
     {
         "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicationInstanceTypeDef = TypedDict(
     "ReplicationInstanceTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
@@ -3178,52 +3183,52 @@
     total=False,
 )
 
 CreateReplicationInstanceResponseTypeDef = TypedDict(
     "CreateReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteReplicationInstanceResponseTypeDef = TypedDict(
     "DeleteReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationInstancesResponseTypeDef = TypedDict(
     "DescribeReplicationInstancesResponseTypeDef",
     {
         "Marker": str,
         "ReplicationInstances": List[ReplicationInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationInstanceResponseTypeDef = TypedDict(
     "ModifyReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootReplicationInstanceResponseTypeDef = TypedDict(
     "RebootReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecommendationsResponseTypeDef = TypedDict(
     "DescribeRecommendationsResponseTypeDef",
     {
         "NextToken": str,
         "Recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/type_defs.pyi` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_dms.type_defs import AccountQuotaTypeDef
 
-    data: AccountQuotaTypeDef = {...}
+    data: AccountQuotaTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -56,20 +56,23 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountQuotaTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchStartRecommendationsErrorEntryTypeDef",
+    "BlobTypeDef",
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     "CertificateTypeDef",
     "CollectorHealthCheckTypeDef",
     "InventoryDataTypeDef",
     "CollectorShortInfoResponseTypeDef",
     "ConnectionTypeDef",
     "DmsTransferSettingsTypeDef",
@@ -88,143 +91,143 @@
     "PostgreSQLSettingsTypeDef",
     "RedisSettingsTypeDef",
     "RedshiftSettingsTypeDef",
     "S3SettingsTypeDef",
     "SybaseSettingsTypeDef",
     "EventSubscriptionTypeDef",
     "CreateFleetAdvisorCollectorRequestRequestTypeDef",
-    "CreateFleetAdvisorCollectorResponseTypeDef",
+    "TimestampTypeDef",
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     "ServerShortInfoResponseTypeDef",
     "DatabaseShortInfoResponseTypeDef",
     "DeleteCertificateMessageRequestTypeDef",
     "DeleteCollectorRequestRequestTypeDef",
     "DeleteConnectionMessageRequestTypeDef",
     "DeleteEndpointMessageRequestTypeDef",
     "DeleteEventSubscriptionMessageRequestTypeDef",
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
     "DeleteReplicationInstanceMessageRequestTypeDef",
     "DeleteReplicationSubnetGroupMessageRequestTypeDef",
     "DeleteReplicationTaskAssessmentRunMessageRequestTypeDef",
     "DeleteReplicationTaskMessageRequestTypeDef",
     "DescribeApplicableIndividualAssessmentsMessageRequestTypeDef",
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "DescribeEndpointSettingsMessageRequestTypeDef",
     "EndpointSettingTypeDef",
     "SupportedEndpointTypeTypeDef",
     "EventCategoryGroupTypeDef",
     "EventTypeDef",
     "DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef",
     "FleetAdvisorLsaAnalysisResponseTypeDef",
     "FleetAdvisorSchemaObjectResponseTypeDef",
-    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     "OrderableReplicationInstanceTypeDef",
     "LimitationTypeDef",
     "DescribeRefreshSchemasStatusMessageRequestTypeDef",
     "RefreshSchemasStatusTypeDef",
     "DescribeReplicationInstanceTaskLogsMessageRequestTypeDef",
     "ReplicationInstanceTaskLogTypeDef",
-    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     "ReplicationTaskAssessmentResultTypeDef",
     "ReplicationTaskIndividualAssessmentTypeDef",
-    "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
     "DescribeSchemasMessageRequestTypeDef",
-    "DescribeSchemasResponseTypeDef",
     "TableStatisticsTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "OracleSettingsOutputTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifyReplicationInstanceMessageRequestTypeDef",
     "ModifyReplicationSubnetGroupMessageRequestTypeDef",
-    "ModifyReplicationTaskMessageRequestTypeDef",
     "MoveReplicationTaskMessageRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "RdsConfigurationTypeDef",
     "RdsRequirementsTypeDef",
     "RebootReplicationInstanceMessageRequestTypeDef",
     "RecommendationSettingsTypeDef",
     "RefreshSchemasMessageRequestTypeDef",
     "TableToReloadTypeDef",
-    "ReloadTablesResponseTypeDef",
     "RemoveTagsFromResourceMessageRequestTypeDef",
     "ReplicationPendingModifiedValuesTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ReplicationTaskAssessmentRunProgressTypeDef",
     "ReplicationTaskStatsTypeDef",
-    "ResponseMetadataTypeDef",
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
     "SchemaShortInfoResponseTypeDef",
     "StartReplicationTaskAssessmentMessageRequestTypeDef",
     "StartReplicationTaskAssessmentRunMessageRequestTypeDef",
-    "StartReplicationTaskMessageRequestTypeDef",
     "StopReplicationTaskMessageRequestTypeDef",
     "TestConnectionMessageRequestTypeDef",
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
     "AddTagsToResourceMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateReplicationInstanceMessageRequestTypeDef",
     "CreateReplicationSubnetGroupMessageRequestTypeDef",
-    "CreateReplicationTaskMessageRequestTypeDef",
-    "ImportCertificateMessageRequestTypeDef",
+    "CreateFleetAdvisorCollectorResponseTypeDef",
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
+    "DescribeSchemasResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ReloadTablesResponseTypeDef",
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
     "SubnetTypeDef",
     "BatchStartRecommendationsResponseTypeDef",
+    "ImportCertificateMessageRequestTypeDef",
     "DeleteCertificateResponseTypeDef",
     "DescribeCertificatesResponseTypeDef",
     "ImportCertificateResponseTypeDef",
     "CollectorResponseTypeDef",
     "DeleteConnectionResponseTypeDef",
     "DescribeConnectionsResponseTypeDef",
     "TestConnectionResponseTypeDef",
     "CreateEndpointMessageRequestTypeDef",
-    "EndpointTypeDef",
     "ModifyEndpointMessageRequestTypeDef",
     "CreateEventSubscriptionResponseTypeDef",
     "DeleteEventSubscriptionResponseTypeDef",
     "DescribeEventSubscriptionsResponseTypeDef",
     "ModifyEventSubscriptionResponseTypeDef",
+    "CreateReplicationTaskMessageRequestTypeDef",
+    "ModifyReplicationTaskMessageRequestTypeDef",
+    "StartReplicationTaskMessageRequestTypeDef",
     "DatabaseResponseTypeDef",
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     "DescribeCertificatesMessageRequestTypeDef",
-    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     "DescribeConnectionsMessageRequestTypeDef",
-    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
     "DescribeEndpointTypesMessageRequestTypeDef",
-    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
     "DescribeEndpointsMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
     "DescribeEventsMessageRequestTypeDef",
     "DescribeFleetAdvisorCollectorsRequestRequestTypeDef",
     "DescribeFleetAdvisorDatabasesRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef",
     "DescribeFleetAdvisorSchemasRequestRequestTypeDef",
     "DescribePendingMaintenanceActionsMessageRequestTypeDef",
     "DescribeRecommendationLimitationsRequestRequestTypeDef",
     "DescribeRecommendationsRequestRequestTypeDef",
-    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
     "DescribeReplicationInstancesMessageRequestTypeDef",
-    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
     "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
     "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
-    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
     "DescribeReplicationTasksMessageRequestTypeDef",
-    "DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     "DescribeTableStatisticsMessageRequestTypeDef",
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
+    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
+    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
+    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
+    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
+    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
+    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
+    "DescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    "DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     "DescribeEndpointsMessageEndpointDeletedWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef",
     "DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef",
     "DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef",
@@ -239,29 +242,31 @@
     "DescribeRecommendationLimitationsResponseTypeDef",
     "DescribeRefreshSchemasStatusResponseTypeDef",
     "RefreshSchemasResponseTypeDef",
     "DescribeReplicationInstanceTaskLogsResponseTypeDef",
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
     "DescribeTableStatisticsResponseTypeDef",
+    "EndpointTypeDef",
+    "OracleSettingsUnionTypeDef",
     "ResourcePendingMaintenanceActionsTypeDef",
     "RdsRecommendationTypeDef",
     "StartRecommendationsRequestEntryTypeDef",
     "StartRecommendationsRequestRequestTypeDef",
     "ReloadTablesMessageRequestTypeDef",
     "ReplicationTaskAssessmentRunTypeDef",
     "ReplicationTaskTypeDef",
     "SchemaResponseTypeDef",
     "ReplicationSubnetGroupTypeDef",
     "DescribeFleetAdvisorCollectorsResponseTypeDef",
+    "DescribeFleetAdvisorDatabasesResponseTypeDef",
     "CreateEndpointResponseTypeDef",
     "DeleteEndpointResponseTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ModifyEndpointResponseTypeDef",
-    "DescribeFleetAdvisorDatabasesResponseTypeDef",
     "ApplyPendingMaintenanceActionResponseTypeDef",
     "DescribePendingMaintenanceActionsResponseTypeDef",
     "RecommendationDataTypeDef",
     "BatchStartRecommendationsRequestRequestTypeDef",
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
@@ -313,14 +318,25 @@
     {
         "ReplicationInstanceArn": str,
         "ApplyAction": str,
         "OptInType": str,
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
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -331,14 +347,15 @@
         "DatabaseId": str,
         "Message": str,
         "Code": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelReplicationTaskAssessmentRunMessageRequestTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunMessageRequestTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
     },
 )
 
@@ -448,19 +465,21 @@
         "FullLoadErrorPercentage": int,
         "ErrorRetryDuration": int,
         "UseNewMappingType": bool,
     },
     total=False,
 )
 
+
 class ElasticsearchSettingsTypeDef(
     _RequiredElasticsearchSettingsTypeDef, _OptionalElasticsearchSettingsTypeDef
 ):
     pass
 
+
 GcpMySQLSettingsTypeDef = TypedDict(
     "GcpMySQLSettingsTypeDef",
     {
         "AfterConnectScript": str,
         "CleanSourceMetadataOnMismatch": bool,
         "DatabaseName": str,
         "EventsPollInterval": int,
@@ -619,17 +638,19 @@
         "MaxFileSize": int,
         "MaxRetryCount": int,
         "IamAuthEnabled": bool,
     },
     total=False,
 )
 
+
 class NeptuneSettingsTypeDef(_RequiredNeptuneSettingsTypeDef, _OptionalNeptuneSettingsTypeDef):
     pass
 
+
 OracleSettingsTypeDef = TypedDict(
     "OracleSettingsTypeDef",
     {
         "AddSupplementalLogging": bool,
         "ArchivedLogDestId": int,
         "AdditionalArchivedLogDestId": int,
         "ExtraArchivedLogDestIds": Sequence[int],
@@ -717,17 +738,19 @@
         "AuthUserName": str,
         "AuthPassword": str,
         "SslCaCertificateArn": str,
     },
     total=False,
 )
 
+
 class RedisSettingsTypeDef(_RequiredRedisSettingsTypeDef, _OptionalRedisSettingsTypeDef):
     pass
 
+
 RedshiftSettingsTypeDef = TypedDict(
     "RedshiftSettingsTypeDef",
     {
         "AcceptAnyDate": bool,
         "AfterConnectScript": str,
         "BucketFolder": str,
         "BucketName": str,
@@ -852,32 +875,23 @@
     "_OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateFleetAdvisorCollectorRequestRequestTypeDef(
     _RequiredCreateFleetAdvisorCollectorRequestRequestTypeDef,
     _OptionalCreateFleetAdvisorCollectorRequestRequestTypeDef,
 ):
     pass
 
-CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
-    "CreateFleetAdvisorCollectorResponseTypeDef",
-    {
-        "CollectorReferencedId": str,
-        "CollectorName": str,
-        "Description": str,
-        "ServiceAccessRoleArn": str,
-        "S3BucketName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
+TimestampTypeDef = Union[datetime, str]
 DatabaseInstanceSoftwareDetailsResponseTypeDef = TypedDict(
     "DatabaseInstanceSoftwareDetailsResponseTypeDef",
     {
         "Engine": str,
         "EngineVersion": str,
         "EngineEdition": str,
         "ServicePack": str,
@@ -948,22 +962,14 @@
 DeleteFleetAdvisorDatabasesRequestRequestTypeDef = TypedDict(
     "DeleteFleetAdvisorDatabasesRequestRequestTypeDef",
     {
         "DatabaseIds": Sequence[str],
     },
 )
 
-DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DeleteFleetAdvisorDatabasesResponseTypeDef",
-    {
-        "DatabaseIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteReplicationInstanceMessageRequestTypeDef = TypedDict(
     "DeleteReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
 )
 
@@ -998,31 +1004,32 @@
         "MigrationType": MigrationTypeValueType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
-    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
-    {
-        "IndividualAssessmentNames": List[str],
-        "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FilterTypeDef = TypedDict(
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
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1039,20 +1046,22 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeEndpointSettingsMessageRequestTypeDef(
     _RequiredDescribeEndpointSettingsMessageRequestTypeDef,
     _OptionalDescribeEndpointSettingsMessageRequestTypeDef,
 ):
     pass
 
+
 EndpointSettingTypeDef = TypedDict(
     "EndpointSettingTypeDef",
     {
         "Name": str,
         "Type": EndpointSettingTypeValueType,
         "EnumValues": List[str],
         "Sensitive": bool,
@@ -1124,22 +1133,14 @@
         "NumberOfObjects": int,
         "CodeLineCount": int,
         "CodeSize": int,
     },
     total=False,
 )
 
-DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = TypedDict(
-    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrderableReplicationInstancesMessageRequestTypeDef = TypedDict(
     "DescribeOrderableReplicationInstancesMessageRequestTypeDef",
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
@@ -1204,39 +1205,32 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeReplicationInstanceTaskLogsMessageRequestTypeDef(
     _RequiredDescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     _OptionalDescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
 ):
     pass
 
+
 ReplicationInstanceTaskLogTypeDef = TypedDict(
     "ReplicationInstanceTaskLogTypeDef",
     {
         "ReplicationTaskName": str,
         "ReplicationTaskArn": str,
         "ReplicationInstanceTaskLogSize": int,
     },
     total=False,
 )
 
-DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
-    {
-        "ReplicationTaskArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1265,34 +1259,14 @@
         "IndividualAssessmentName": str,
         "Status": str,
         "ReplicationTaskIndividualAssessmentStartDate": datetime,
     },
     total=False,
 )
 
-_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
-    {
-        "EndpointArn": str,
-    },
-)
-_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
-    _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
-    _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeSchemasMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemasMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
 _OptionalDescribeSchemasMessageRequestTypeDef = TypedDict(
@@ -1300,27 +1274,20 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeSchemasMessageRequestTypeDef(
     _RequiredDescribeSchemasMessageRequestTypeDef, _OptionalDescribeSchemasMessageRequestTypeDef
 ):
     pass
 
-DescribeSchemasResponseTypeDef = TypedDict(
-    "DescribeSchemasResponseTypeDef",
-    {
-        "Marker": str,
-        "Schemas": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TableStatisticsTypeDef = TypedDict(
     "TableStatisticsTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
         "Inserts": int,
@@ -1344,19 +1311,61 @@
         "ValidationSuspendedRecords": int,
         "ValidationState": str,
         "ValidationStateDetails": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+OracleSettingsOutputTypeDef = TypedDict(
+    "OracleSettingsOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AddSupplementalLogging": bool,
+        "ArchivedLogDestId": int,
+        "AdditionalArchivedLogDestId": int,
+        "ExtraArchivedLogDestIds": List[int],
+        "AllowSelectNestedTables": bool,
+        "ParallelAsmReadThreads": int,
+        "ReadAheadBlocks": int,
+        "AccessAlternateDirectly": bool,
+        "UseAlternateFolderForOnline": bool,
+        "OraclePathPrefix": str,
+        "UsePathPrefix": str,
+        "ReplacePathPrefix": bool,
+        "EnableHomogenousTablespace": bool,
+        "DirectPathNoLog": bool,
+        "ArchivedLogsOnly": bool,
+        "AsmPassword": str,
+        "AsmServer": str,
+        "AsmUser": str,
+        "CharLengthSemantics": CharLengthSemanticsType,
+        "DatabaseName": str,
+        "DirectPathParallelLoad": bool,
+        "FailTasksOnLobTruncation": bool,
+        "NumberDatatypeScale": int,
+        "Password": str,
+        "Port": int,
+        "ReadTableSpaceName": bool,
+        "RetryInterval": int,
+        "SecurityDbEncryption": str,
+        "SecurityDbEncryptionName": str,
+        "ServerName": str,
+        "SpatialDataOptionToGeoJsonFunctionName": str,
+        "StandbyDelayTime": int,
+        "Username": str,
+        "UseBFile": bool,
+        "UseDirectPathFullLoad": bool,
+        "UseLogminerReader": bool,
+        "SecretsManagerAccessRoleArn": str,
+        "SecretsManagerSecretId": str,
+        "SecretsManagerOracleAsmAccessRoleArn": str,
+        "SecretsManagerOracleAsmSecretId": str,
+        "TrimSpaceInChar": bool,
+        "ConvertTimestampWithZoneToUTC": bool,
     },
+    total=False,
 )
 
 ListTagsForResourceMessageRequestTypeDef = TypedDict(
     "ListTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceArnList": Sequence[str],
@@ -1377,20 +1386,22 @@
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
 _RequiredModifyReplicationInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceArn": str,
     },
 )
 _OptionalModifyReplicationInstanceMessageRequestTypeDef = TypedDict(
@@ -1407,20 +1418,22 @@
         "AutoMinorVersionUpgrade": bool,
         "ReplicationInstanceIdentifier": str,
         "NetworkType": str,
     },
     total=False,
 )
 
+
 class ModifyReplicationInstanceMessageRequestTypeDef(
     _RequiredModifyReplicationInstanceMessageRequestTypeDef,
     _OptionalModifyReplicationInstanceMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyReplicationSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyReplicationSubnetGroupMessageRequestTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -1428,65 +1441,30 @@
     "_OptionalModifyReplicationSubnetGroupMessageRequestTypeDef",
     {
         "ReplicationSubnetGroupDescription": str,
     },
     total=False,
 )
 
+
 class ModifyReplicationSubnetGroupMessageRequestTypeDef(
     _RequiredModifyReplicationSubnetGroupMessageRequestTypeDef,
     _OptionalModifyReplicationSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-_RequiredModifyReplicationTaskMessageRequestTypeDef = TypedDict(
-    "_RequiredModifyReplicationTaskMessageRequestTypeDef",
-    {
-        "ReplicationTaskArn": str,
-    },
-)
-_OptionalModifyReplicationTaskMessageRequestTypeDef = TypedDict(
-    "_OptionalModifyReplicationTaskMessageRequestTypeDef",
-    {
-        "ReplicationTaskIdentifier": str,
-        "MigrationType": MigrationTypeValueType,
-        "TableMappings": str,
-        "ReplicationTaskSettings": str,
-        "CdcStartTime": Union[datetime, str],
-        "CdcStartPosition": str,
-        "CdcStopPosition": str,
-        "TaskData": str,
-    },
-    total=False,
-)
-
-class ModifyReplicationTaskMessageRequestTypeDef(
-    _RequiredModifyReplicationTaskMessageRequestTypeDef,
-    _OptionalModifyReplicationTaskMessageRequestTypeDef,
-):
-    pass
 
 MoveReplicationTaskMessageRequestTypeDef = TypedDict(
     "MoveReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
         "TargetReplicationInstanceArn": str,
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "Action": str,
         "AutoAppliedAfterDate": datetime,
         "ForcedApplyDate": datetime,
         "OptInStatus": str,
@@ -1535,20 +1513,22 @@
     {
         "ForceFailover": bool,
         "ForcePlannedFailover": bool,
     },
     total=False,
 )
 
+
 class RebootReplicationInstanceMessageRequestTypeDef(
     _RequiredRebootReplicationInstanceMessageRequestTypeDef,
     _OptionalRebootReplicationInstanceMessageRequestTypeDef,
 ):
     pass
 
+
 RecommendationSettingsTypeDef = TypedDict(
     "RecommendationSettingsTypeDef",
     {
         "InstanceSizingType": str,
         "WorkloadType": str,
     },
 )
@@ -1565,22 +1545,14 @@
     "TableToReloadTypeDef",
     {
         "SchemaName": str,
         "TableName": str,
     },
 )
 
-ReloadTablesResponseTypeDef = TypedDict(
-    "ReloadTablesResponseTypeDef",
-    {
-        "ReplicationTaskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromResourceMessageRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1629,34 +1601,14 @@
         "StopDate": datetime,
         "FullLoadStartDate": datetime,
         "FullLoadFinishDate": datetime,
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
-RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
-    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
-    {
-        "LsaAnalysisId": str,
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SchemaShortInfoResponseTypeDef = TypedDict(
     "SchemaShortInfoResponseTypeDef",
     {
         "SchemaId": str,
         "SchemaName": str,
         "DatabaseId": str,
         "DatabaseName": str,
@@ -1689,42 +1641,21 @@
         "ResultKmsKeyArn": str,
         "IncludeOnly": Sequence[str],
         "Exclude": Sequence[str],
     },
     total=False,
 )
 
+
 class StartReplicationTaskAssessmentRunMessageRequestTypeDef(
     _RequiredStartReplicationTaskAssessmentRunMessageRequestTypeDef,
     _OptionalStartReplicationTaskAssessmentRunMessageRequestTypeDef,
 ):
     pass
 
-_RequiredStartReplicationTaskMessageRequestTypeDef = TypedDict(
-    "_RequiredStartReplicationTaskMessageRequestTypeDef",
-    {
-        "ReplicationTaskArn": str,
-        "StartReplicationTaskType": StartReplicationTaskTypeValueType,
-    },
-)
-_OptionalStartReplicationTaskMessageRequestTypeDef = TypedDict(
-    "_OptionalStartReplicationTaskMessageRequestTypeDef",
-    {
-        "CdcStartTime": Union[datetime, str],
-        "CdcStartPosition": str,
-        "CdcStopPosition": str,
-    },
-    total=False,
-)
-
-class StartReplicationTaskMessageRequestTypeDef(
-    _RequiredStartReplicationTaskMessageRequestTypeDef,
-    _OptionalStartReplicationTaskMessageRequestTypeDef,
-):
-    pass
 
 StopReplicationTaskMessageRequestTypeDef = TypedDict(
     "StopReplicationTaskMessageRequestTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
@@ -1741,31 +1672,14 @@
     "UpdateSubscriptionsToEventBridgeMessageRequestTypeDef",
     {
         "ForceMove": bool,
     },
     total=False,
 )
 
-UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
-    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
-    {
-        "Result": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
-    {
-        "AccountQuotas": List[AccountQuotaTypeDef],
-        "UniqueAccountIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddTagsToResourceMessageRequestTypeDef = TypedDict(
     "AddTagsToResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1785,20 +1699,22 @@
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
 _RequiredCreateReplicationInstanceMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationInstanceMessageRequestTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
         "ReplicationInstanceClass": str,
     },
 )
@@ -1819,20 +1735,22 @@
         "DnsNameServers": str,
         "ResourceIdentifier": str,
         "NetworkType": str,
     },
     total=False,
 )
 
+
 class CreateReplicationInstanceMessageRequestTypeDef(
     _RequiredCreateReplicationInstanceMessageRequestTypeDef,
     _OptionalCreateReplicationInstanceMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateReplicationSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateReplicationSubnetGroupMessageRequestTypeDef",
     {
         "ReplicationSubnetGroupIdentifier": str,
         "ReplicationSubnetGroupDescription": str,
         "SubnetIds": Sequence[str],
     },
@@ -1841,77 +1759,106 @@
     "_OptionalCreateReplicationSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateReplicationSubnetGroupMessageRequestTypeDef(
     _RequiredCreateReplicationSubnetGroupMessageRequestTypeDef,
     _OptionalCreateReplicationSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-_RequiredCreateReplicationTaskMessageRequestTypeDef = TypedDict(
-    "_RequiredCreateReplicationTaskMessageRequestTypeDef",
+
+CreateFleetAdvisorCollectorResponseTypeDef = TypedDict(
+    "CreateFleetAdvisorCollectorResponseTypeDef",
     {
-        "ReplicationTaskIdentifier": str,
-        "SourceEndpointArn": str,
-        "TargetEndpointArn": str,
-        "ReplicationInstanceArn": str,
-        "MigrationType": MigrationTypeValueType,
-        "TableMappings": str,
+        "CollectorReferencedId": str,
+        "CollectorName": str,
+        "Description": str,
+        "ServiceAccessRoleArn": str,
+        "S3BucketName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateReplicationTaskMessageRequestTypeDef = TypedDict(
-    "_OptionalCreateReplicationTaskMessageRequestTypeDef",
+
+DeleteFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DeleteFleetAdvisorDatabasesResponseTypeDef",
     {
-        "ReplicationTaskSettings": str,
-        "CdcStartTime": Union[datetime, str],
-        "CdcStartPosition": str,
-        "CdcStopPosition": str,
-        "Tags": Sequence[TagTypeDef],
-        "TaskData": str,
-        "ResourceIdentifier": str,
+        "DatabaseIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateReplicationTaskMessageRequestTypeDef(
-    _RequiredCreateReplicationTaskMessageRequestTypeDef,
-    _OptionalCreateReplicationTaskMessageRequestTypeDef,
-):
-    pass
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
+    {
+        "AccountQuotas": List[AccountQuotaTypeDef],
+        "UniqueAccountIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredImportCertificateMessageRequestTypeDef = TypedDict(
-    "_RequiredImportCertificateMessageRequestTypeDef",
+DescribeApplicableIndividualAssessmentsResponseTypeDef = TypedDict(
+    "DescribeApplicableIndividualAssessmentsResponseTypeDef",
     {
-        "CertificateIdentifier": str,
+        "IndividualAssessmentNames": List[str],
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalImportCertificateMessageRequestTypeDef = TypedDict(
-    "_OptionalImportCertificateMessageRequestTypeDef",
+
+DescribeSchemasResponseTypeDef = TypedDict(
+    "DescribeSchemasResponseTypeDef",
     {
-        "CertificatePem": str,
-        "CertificateWallet": Union[str, bytes, IO[Any], StreamingBody],
-        "Tags": Sequence[TagTypeDef],
+        "Marker": str,
+        "Schemas": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ImportCertificateMessageRequestTypeDef(
-    _RequiredImportCertificateMessageRequestTypeDef, _OptionalImportCertificateMessageRequestTypeDef
-):
-    pass
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReloadTablesResponseTypeDef = TypedDict(
+    "ReloadTablesResponseTypeDef",
+    {
+        "ReplicationTaskArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RunFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
+    "RunFleetAdvisorLsaAnalysisResponseTypeDef",
+    {
+        "LsaAnalysisId": str,
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSubscriptionsToEventBridgeResponseTypeDef = TypedDict(
+    "UpdateSubscriptionsToEventBridgeResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
@@ -1921,40 +1868,63 @@
     total=False,
 )
 
 BatchStartRecommendationsResponseTypeDef = TypedDict(
     "BatchStartRecommendationsResponseTypeDef",
     {
         "ErrorEntries": List[BatchStartRecommendationsErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredImportCertificateMessageRequestTypeDef = TypedDict(
+    "_RequiredImportCertificateMessageRequestTypeDef",
+    {
+        "CertificateIdentifier": str,
+    },
+)
+_OptionalImportCertificateMessageRequestTypeDef = TypedDict(
+    "_OptionalImportCertificateMessageRequestTypeDef",
+    {
+        "CertificatePem": str,
+        "CertificateWallet": BlobTypeDef,
+        "Tags": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
+
+class ImportCertificateMessageRequestTypeDef(
+    _RequiredImportCertificateMessageRequestTypeDef, _OptionalImportCertificateMessageRequestTypeDef
+):
+    pass
+
+
 DeleteCertificateResponseTypeDef = TypedDict(
     "DeleteCertificateResponseTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificatesResponseTypeDef = TypedDict(
     "DescribeCertificatesResponseTypeDef",
     {
         "Marker": str,
         "Certificates": List[CertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportCertificateResponseTypeDef = TypedDict(
     "ImportCertificateResponseTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CollectorResponseTypeDef = TypedDict(
     "CollectorResponseTypeDef",
     {
         "CollectorReferencedId": str,
@@ -1974,32 +1944,32 @@
     total=False,
 )
 
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectionsResponseTypeDef = TypedDict(
     "DescribeConnectionsResponseTypeDef",
     {
         "Marker": str,
         "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestConnectionResponseTypeDef = TypedDict(
     "TestConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointMessageRequestTypeDef",
     {
         "EndpointIdentifier": str,
@@ -2041,60 +2011,20 @@
         "DocDbSettings": DocDbSettingsTypeDef,
         "RedisSettings": RedisSettingsTypeDef,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
     },
     total=False,
 )
 
+
 class CreateEndpointMessageRequestTypeDef(
     _RequiredCreateEndpointMessageRequestTypeDef, _OptionalCreateEndpointMessageRequestTypeDef
 ):
     pass
 
-EndpointTypeDef = TypedDict(
-    "EndpointTypeDef",
-    {
-        "EndpointIdentifier": str,
-        "EndpointType": ReplicationEndpointTypeValueType,
-        "EngineName": str,
-        "EngineDisplayName": str,
-        "Username": str,
-        "ServerName": str,
-        "Port": int,
-        "DatabaseName": str,
-        "ExtraConnectionAttributes": str,
-        "Status": str,
-        "KmsKeyId": str,
-        "EndpointArn": str,
-        "CertificateArn": str,
-        "SslMode": DmsSslModeValueType,
-        "ServiceAccessRoleArn": str,
-        "ExternalTableDefinition": str,
-        "ExternalId": str,
-        "DynamoDbSettings": DynamoDbSettingsTypeDef,
-        "S3Settings": S3SettingsTypeDef,
-        "DmsTransferSettings": DmsTransferSettingsTypeDef,
-        "MongoDbSettings": MongoDbSettingsTypeDef,
-        "KinesisSettings": KinesisSettingsTypeDef,
-        "KafkaSettings": KafkaSettingsTypeDef,
-        "ElasticsearchSettings": ElasticsearchSettingsTypeDef,
-        "NeptuneSettings": NeptuneSettingsTypeDef,
-        "RedshiftSettings": RedshiftSettingsTypeDef,
-        "PostgreSQLSettings": PostgreSQLSettingsTypeDef,
-        "MySQLSettings": MySQLSettingsTypeDef,
-        "OracleSettings": OracleSettingsTypeDef,
-        "SybaseSettings": SybaseSettingsTypeDef,
-        "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
-        "IBMDb2Settings": IBMDb2SettingsTypeDef,
-        "DocDbSettings": DocDbSettingsTypeDef,
-        "RedisSettings": RedisSettingsTypeDef,
-        "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
-    },
-    total=False,
-)
 
 _RequiredModifyEndpointMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointMessageRequestTypeDef",
     {
         "EndpointArn": str,
     },
 )
@@ -2133,132 +2063,185 @@
         "RedisSettings": RedisSettingsTypeDef,
         "ExactSettings": bool,
         "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
     },
     total=False,
 )
 
+
 class ModifyEndpointMessageRequestTypeDef(
     _RequiredModifyEndpointMessageRequestTypeDef, _OptionalModifyEndpointMessageRequestTypeDef
 ):
     pass
 
+
 CreateEventSubscriptionResponseTypeDef = TypedDict(
     "CreateEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEventSubscriptionResponseTypeDef = TypedDict(
     "DeleteEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventSubscriptionsResponseTypeDef = TypedDict(
     "DescribeEventSubscriptionsResponseTypeDef",
     {
         "Marker": str,
         "EventSubscriptionsList": List[EventSubscriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyEventSubscriptionResponseTypeDef = TypedDict(
     "ModifyEventSubscriptionResponseTypeDef",
     {
         "EventSubscription": EventSubscriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DatabaseResponseTypeDef = TypedDict(
-    "DatabaseResponseTypeDef",
+_RequiredCreateReplicationTaskMessageRequestTypeDef = TypedDict(
+    "_RequiredCreateReplicationTaskMessageRequestTypeDef",
     {
-        "DatabaseId": str,
-        "DatabaseName": str,
-        "IpAddress": str,
-        "NumberOfSchemas": int,
-        "Server": ServerShortInfoResponseTypeDef,
-        "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseTypeDef,
-        "Collectors": List[CollectorShortInfoResponseTypeDef],
+        "ReplicationTaskIdentifier": str,
+        "SourceEndpointArn": str,
+        "TargetEndpointArn": str,
+        "ReplicationInstanceArn": str,
+        "MigrationType": MigrationTypeValueType,
+        "TableMappings": str,
+    },
+)
+_OptionalCreateReplicationTaskMessageRequestTypeDef = TypedDict(
+    "_OptionalCreateReplicationTaskMessageRequestTypeDef",
+    {
+        "ReplicationTaskSettings": str,
+        "CdcStartTime": TimestampTypeDef,
+        "CdcStartPosition": str,
+        "CdcStopPosition": str,
+        "Tags": Sequence[TagTypeDef],
+        "TaskData": str,
+        "ResourceIdentifier": str,
     },
     total=False,
 )
 
-DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
-    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
+
+class CreateReplicationTaskMessageRequestTypeDef(
+    _RequiredCreateReplicationTaskMessageRequestTypeDef,
+    _OptionalCreateReplicationTaskMessageRequestTypeDef,
+):
+    pass
+
+
+_RequiredModifyReplicationTaskMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyReplicationTaskMessageRequestTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ReplicationTaskArn": str,
+    },
+)
+_OptionalModifyReplicationTaskMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyReplicationTaskMessageRequestTypeDef",
+    {
+        "ReplicationTaskIdentifier": str,
+        "MigrationType": MigrationTypeValueType,
+        "TableMappings": str,
+        "ReplicationTaskSettings": str,
+        "CdcStartTime": TimestampTypeDef,
+        "CdcStartPosition": str,
+        "CdcStopPosition": str,
+        "TaskData": str,
     },
     total=False,
 )
 
-DescribeCertificatesMessageRequestTypeDef = TypedDict(
-    "DescribeCertificatesMessageRequestTypeDef",
+
+class ModifyReplicationTaskMessageRequestTypeDef(
+    _RequiredModifyReplicationTaskMessageRequestTypeDef,
+    _OptionalModifyReplicationTaskMessageRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartReplicationTaskMessageRequestTypeDef = TypedDict(
+    "_RequiredStartReplicationTaskMessageRequestTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
+        "ReplicationTaskArn": str,
+        "StartReplicationTaskType": StartReplicationTaskTypeValueType,
+    },
+)
+_OptionalStartReplicationTaskMessageRequestTypeDef = TypedDict(
+    "_OptionalStartReplicationTaskMessageRequestTypeDef",
+    {
+        "CdcStartTime": TimestampTypeDef,
+        "CdcStartPosition": str,
+        "CdcStopPosition": str,
     },
     total=False,
 )
 
-DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = TypedDict(
-    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
+
+class StartReplicationTaskMessageRequestTypeDef(
+    _RequiredStartReplicationTaskMessageRequestTypeDef,
+    _OptionalStartReplicationTaskMessageRequestTypeDef,
+):
+    pass
+
+
+DatabaseResponseTypeDef = TypedDict(
+    "DatabaseResponseTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "DatabaseId": str,
+        "DatabaseName": str,
+        "IpAddress": str,
+        "NumberOfSchemas": int,
+        "Server": ServerShortInfoResponseTypeDef,
+        "SoftwareDetails": DatabaseInstanceSoftwareDetailsResponseTypeDef,
+        "Collectors": List[CollectorShortInfoResponseTypeDef],
     },
     total=False,
 )
 
-DescribeConnectionsMessageRequestTypeDef = TypedDict(
-    "DescribeConnectionsMessageRequestTypeDef",
+DescribeCertificatesMessageRequestTypeDef = TypedDict(
+    "DescribeCertificatesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = TypedDict(
-    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
+DescribeConnectionsMessageRequestTypeDef = TypedDict(
+    "DescribeConnectionsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
 DescribeEndpointTypesMessageRequestTypeDef = TypedDict(
     "DescribeEndpointTypesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
-    {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEndpointsMessageRequestTypeDef = TypedDict(
     "DescribeEndpointsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
@@ -2270,57 +2253,32 @@
     {
         "SourceType": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "SourceIdentifier": str,
-        "SourceType": Literal["replication-instance"],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "EventCategories": Sequence[str],
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventsMessageRequestTypeDef = TypedDict(
     "DescribeEventsMessageRequestTypeDef",
     {
         "SourceIdentifier": str,
         "SourceType": Literal["replication-instance"],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Duration": int,
         "EventCategories": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
@@ -2393,136 +2351,240 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = TypedDict(
-    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
+DescribeReplicationInstancesMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationInstancesMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationInstancesMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationInstancesMessageRequestTypeDef",
+DescribeReplicationSubnetGroupsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
+DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxRecords": int,
+        "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationSubnetGroupsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationSubnetGroupsMessageRequestTypeDef",
+DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef",
+DescribeReplicationTasksMessageRequestTypeDef = TypedDict(
+    "DescribeReplicationTasksMessageRequestTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
+        "WithoutSettings": bool,
     },
     total=False,
 )
 
-DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef",
+_RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
+    {
+        "ReplicationTaskArn": str,
+    },
+)
+_OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
+    "_OptionalDescribeTableStatisticsMessageRequestTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
+        "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = TypedDict(
-    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
+
+class DescribeTableStatisticsMessageRequestTypeDef(
+    _RequiredDescribeTableStatisticsMessageRequestTypeDef,
+    _OptionalDescribeTableStatisticsMessageRequestTypeDef,
+):
+    pass
+
+
+DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef = TypedDict(
+    "DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "WithoutSettings": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeReplicationTasksMessageRequestTypeDef = TypedDict(
-    "DescribeReplicationTasksMessageRequestTypeDef",
+DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef = TypedDict(
+    "DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "MaxRecords": int,
-        "Marker": str,
-        "WithoutSettings": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef = TypedDict(
+    "DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef",
+    {
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
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceType": Literal["replication-instance"],
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
+DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef = TypedDict(
+    "DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef = TypedDict(
+    "DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef",
+    {
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef = TypedDict(
+    "DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef",
     {
         "ReplicationTaskArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
+
+DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef = TypedDict(
+    "DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "WithoutSettings": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
-    _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
-    _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    {
+        "EndpointArn": str,
+    },
+)
+_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeSchemasMessageDescribeSchemasPaginateTypeDef(
+    _RequiredDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+    _OptionalDescribeSchemasMessageDescribeSchemasPaginateTypeDef,
 ):
     pass
 
-_RequiredDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
-    "_RequiredDescribeTableStatisticsMessageRequestTypeDef",
+
+_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     {
         "ReplicationTaskArn": str,
     },
 )
-_OptionalDescribeTableStatisticsMessageRequestTypeDef = TypedDict(
-    "_OptionalDescribeTableStatisticsMessageRequestTypeDef",
+_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef",
     {
-        "MaxRecords": int,
-        "Marker": str,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class DescribeTableStatisticsMessageRequestTypeDef(
-    _RequiredDescribeTableStatisticsMessageRequestTypeDef,
-    _OptionalDescribeTableStatisticsMessageRequestTypeDef,
+
+class DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef(
+    _RequiredDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
+    _OptionalDescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
 ):
     pass
 
+
 DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef = TypedDict(
     "DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "MaxRecords": int,
         "Marker": str,
         "WaiterConfig": WaiterConfigTypeDef,
@@ -2612,135 +2674,178 @@
 )
 
 DescribeEndpointSettingsResponseTypeDef = TypedDict(
     "DescribeEndpointSettingsResponseTypeDef",
     {
         "Marker": str,
         "EndpointSettings": List[EndpointSettingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointTypesResponseTypeDef = TypedDict(
     "DescribeEndpointTypesResponseTypeDef",
     {
         "Marker": str,
         "SupportedEndpointTypes": List[SupportedEndpointTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventCategoriesResponseTypeDef = TypedDict(
     "DescribeEventCategoriesResponseTypeDef",
     {
         "EventCategoryGroupList": List[EventCategoryGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "Marker": str,
         "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFleetAdvisorLsaAnalysisResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorLsaAnalysisResponseTypeDef",
     {
         "Analysis": List[FleetAdvisorLsaAnalysisResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorSchemaObjectSummaryResponseTypeDef",
     {
         "FleetAdvisorSchemaObjects": List[FleetAdvisorSchemaObjectResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrderableReplicationInstancesResponseTypeDef = TypedDict(
     "DescribeOrderableReplicationInstancesResponseTypeDef",
     {
         "OrderableReplicationInstances": List[OrderableReplicationInstanceTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecommendationLimitationsResponseTypeDef = TypedDict(
     "DescribeRecommendationLimitationsResponseTypeDef",
     {
         "NextToken": str,
         "Limitations": List[LimitationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRefreshSchemasStatusResponseTypeDef = TypedDict(
     "DescribeRefreshSchemasStatusResponseTypeDef",
     {
         "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RefreshSchemasResponseTypeDef = TypedDict(
     "RefreshSchemasResponseTypeDef",
     {
         "RefreshSchemasStatus": RefreshSchemasStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationInstanceTaskLogsResponseTypeDef = TypedDict(
     "DescribeReplicationInstanceTaskLogsResponseTypeDef",
     {
         "ReplicationInstanceArn": str,
         "ReplicationInstanceTaskLogs": List[ReplicationInstanceTaskLogTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationTaskAssessmentResultsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentResultsResponseTypeDef",
     {
         "Marker": str,
         "BucketName": str,
         "ReplicationTaskAssessmentResults": List[ReplicationTaskAssessmentResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationTaskIndividualAssessmentsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskIndividualAssessmentsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTaskIndividualAssessments": List[ReplicationTaskIndividualAssessmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableStatisticsResponseTypeDef = TypedDict(
     "DescribeTableStatisticsResponseTypeDef",
     {
         "ReplicationTaskArn": str,
         "TableStatistics": List[TableStatisticsTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EndpointTypeDef = TypedDict(
+    "EndpointTypeDef",
+    {
+        "EndpointIdentifier": str,
+        "EndpointType": ReplicationEndpointTypeValueType,
+        "EngineName": str,
+        "EngineDisplayName": str,
+        "Username": str,
+        "ServerName": str,
+        "Port": int,
+        "DatabaseName": str,
+        "ExtraConnectionAttributes": str,
+        "Status": str,
+        "KmsKeyId": str,
+        "EndpointArn": str,
+        "CertificateArn": str,
+        "SslMode": DmsSslModeValueType,
+        "ServiceAccessRoleArn": str,
+        "ExternalTableDefinition": str,
+        "ExternalId": str,
+        "DynamoDbSettings": DynamoDbSettingsTypeDef,
+        "S3Settings": S3SettingsTypeDef,
+        "DmsTransferSettings": DmsTransferSettingsTypeDef,
+        "MongoDbSettings": MongoDbSettingsTypeDef,
+        "KinesisSettings": KinesisSettingsTypeDef,
+        "KafkaSettings": KafkaSettingsTypeDef,
+        "ElasticsearchSettings": ElasticsearchSettingsTypeDef,
+        "NeptuneSettings": NeptuneSettingsTypeDef,
+        "RedshiftSettings": RedshiftSettingsTypeDef,
+        "PostgreSQLSettings": PostgreSQLSettingsTypeDef,
+        "MySQLSettings": MySQLSettingsTypeDef,
+        "OracleSettings": OracleSettingsOutputTypeDef,
+        "SybaseSettings": SybaseSettingsTypeDef,
+        "MicrosoftSQLServerSettings": MicrosoftSQLServerSettingsTypeDef,
+        "IBMDb2Settings": IBMDb2SettingsTypeDef,
+        "DocDbSettings": DocDbSettingsTypeDef,
+        "RedisSettings": RedisSettingsTypeDef,
+        "GcpMySQLSettings": GcpMySQLSettingsTypeDef,
     },
+    total=False,
 )
 
+OracleSettingsUnionTypeDef = Union[OracleSettingsTypeDef, OracleSettingsOutputTypeDef]
 ResourcePendingMaintenanceActionsTypeDef = TypedDict(
     "ResourcePendingMaintenanceActionsTypeDef",
     {
         "ResourceIdentifier": str,
         "PendingMaintenanceActionDetails": List[PendingMaintenanceActionTypeDef],
     },
     total=False,
@@ -2782,19 +2887,21 @@
     "_OptionalReloadTablesMessageRequestTypeDef",
     {
         "ReloadOption": ReloadOptionValueType,
     },
     total=False,
 )
 
+
 class ReloadTablesMessageRequestTypeDef(
     _RequiredReloadTablesMessageRequestTypeDef, _OptionalReloadTablesMessageRequestTypeDef
 ):
     pass
 
+
 ReplicationTaskAssessmentRunTypeDef = TypedDict(
     "ReplicationTaskAssessmentRunTypeDef",
     {
         "ReplicationTaskAssessmentRunArn": str,
         "ReplicationTaskArn": str,
         "Status": str,
         "ReplicationTaskAssessmentRunCreationDate": datetime,
@@ -2866,74 +2973,74 @@
 )
 
 DescribeFleetAdvisorCollectorsResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorCollectorsResponseTypeDef",
     {
         "Collectors": List[CollectorResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
+    "DescribeFleetAdvisorDatabasesResponseTypeDef",
+    {
+        "Databases": List[DatabaseResponseTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEndpointResponseTypeDef = TypedDict(
     "CreateEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteEndpointResponseTypeDef = TypedDict(
     "DeleteEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Marker": str,
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyEndpointResponseTypeDef = TypedDict(
     "ModifyEndpointResponseTypeDef",
     {
         "Endpoint": EndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeFleetAdvisorDatabasesResponseTypeDef = TypedDict(
-    "DescribeFleetAdvisorDatabasesResponseTypeDef",
-    {
-        "Databases": List[DatabaseResponseTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplyPendingMaintenanceActionResponseTypeDef = TypedDict(
     "ApplyPendingMaintenanceActionResponseTypeDef",
     {
         "ResourcePendingMaintenanceActions": ResourcePendingMaintenanceActionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePendingMaintenanceActionsResponseTypeDef = TypedDict(
     "DescribePendingMaintenanceActionsResponseTypeDef",
     {
         "PendingMaintenanceActions": List[ResourcePendingMaintenanceActionsTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationDataTypeDef = TypedDict(
     "RecommendationDataTypeDef",
     {
         "RdsEngine": RdsRecommendationTypeDef,
@@ -2949,139 +3056,139 @@
     total=False,
 )
 
 CancelReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "CancelReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "DeleteReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationTaskAssessmentRunsResponseTypeDef = TypedDict(
     "DescribeReplicationTaskAssessmentRunsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTaskAssessmentRuns": List[ReplicationTaskAssessmentRunTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartReplicationTaskAssessmentRunResponseTypeDef = TypedDict(
     "StartReplicationTaskAssessmentRunResponseTypeDef",
     {
         "ReplicationTaskAssessmentRun": ReplicationTaskAssessmentRunTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateReplicationTaskResponseTypeDef = TypedDict(
     "CreateReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteReplicationTaskResponseTypeDef = TypedDict(
     "DeleteReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationTasksResponseTypeDef = TypedDict(
     "DescribeReplicationTasksResponseTypeDef",
     {
         "Marker": str,
         "ReplicationTasks": List[ReplicationTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationTaskResponseTypeDef = TypedDict(
     "ModifyReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MoveReplicationTaskResponseTypeDef = TypedDict(
     "MoveReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartReplicationTaskAssessmentResponseTypeDef = TypedDict(
     "StartReplicationTaskAssessmentResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartReplicationTaskResponseTypeDef = TypedDict(
     "StartReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopReplicationTaskResponseTypeDef = TypedDict(
     "StopReplicationTaskResponseTypeDef",
     {
         "ReplicationTask": ReplicationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFleetAdvisorSchemasResponseTypeDef = TypedDict(
     "DescribeFleetAdvisorSchemasResponseTypeDef",
     {
         "FleetAdvisorSchemas": List[SchemaResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateReplicationSubnetGroupResponseTypeDef = TypedDict(
     "CreateReplicationSubnetGroupResponseTypeDef",
     {
         "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationSubnetGroupsResponseTypeDef = TypedDict(
     "DescribeReplicationSubnetGroupsResponseTypeDef",
     {
         "Marker": str,
         "ReplicationSubnetGroups": List[ReplicationSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationSubnetGroupResponseTypeDef = TypedDict(
     "ModifyReplicationSubnetGroupResponseTypeDef",
     {
         "ReplicationSubnetGroup": ReplicationSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicationInstanceTypeDef = TypedDict(
     "ReplicationInstanceTypeDef",
     {
         "ReplicationInstanceIdentifier": str,
@@ -3127,52 +3234,52 @@
     total=False,
 )
 
 CreateReplicationInstanceResponseTypeDef = TypedDict(
     "CreateReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteReplicationInstanceResponseTypeDef = TypedDict(
     "DeleteReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReplicationInstancesResponseTypeDef = TypedDict(
     "DescribeReplicationInstancesResponseTypeDef",
     {
         "Marker": str,
         "ReplicationInstances": List[ReplicationInstanceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReplicationInstanceResponseTypeDef = TypedDict(
     "ModifyReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootReplicationInstanceResponseTypeDef = TypedDict(
     "RebootReplicationInstanceResponseTypeDef",
     {
         "ReplicationInstance": ReplicationInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRecommendationsResponseTypeDef = TypedDict(
     "DescribeRecommendationsResponseTypeDef",
     {
         "NextToken": str,
         "Recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/waiter.py` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms/waiter.pyi` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/PKG-INFO` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dms
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DatabaseMigrationService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore dms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore dms type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-dms"></a>
 
 # types-aiobotocore-dms
 
 [![PyPI - types-aiobotocore-dms](https://img.shields.io/pypi/v/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dms?color=blue)](https://pypistats.org/packages/types-aiobotocore-dms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dms)](https://pepy.tech/project/types-aiobotocore-dms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DatabaseMigrationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#DatabaseMigrationService)
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
 [types-aiobotocore-dms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dms/).
 
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
@@ -458,28 +457,30 @@
 )
 
 
 def check_value(value: AuthMechanismValueType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_dms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_dms.type_defs import (
     AccountQuotaTypeDef,
     TagTypeDef,
     ApplyPendingMaintenanceActionMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     AvailabilityZoneTypeDef,
     BatchStartRecommendationsErrorEntryTypeDef,
+    BlobTypeDef,
     CancelReplicationTaskAssessmentRunMessageRequestTypeDef,
     CertificateTypeDef,
     CollectorHealthCheckTypeDef,
     InventoryDataTypeDef,
     CollectorShortInfoResponseTypeDef,
     ConnectionTypeDef,
     DmsTransferSettingsTypeDef,
@@ -498,143 +499,143 @@
     PostgreSQLSettingsTypeDef,
     RedisSettingsTypeDef,
     RedshiftSettingsTypeDef,
     S3SettingsTypeDef,
     SybaseSettingsTypeDef,
     EventSubscriptionTypeDef,
     CreateFleetAdvisorCollectorRequestRequestTypeDef,
-    CreateFleetAdvisorCollectorResponseTypeDef,
+    TimestampTypeDef,
     DatabaseInstanceSoftwareDetailsResponseTypeDef,
     ServerShortInfoResponseTypeDef,
     DatabaseShortInfoResponseTypeDef,
     DeleteCertificateMessageRequestTypeDef,
     DeleteCollectorRequestRequestTypeDef,
     DeleteConnectionMessageRequestTypeDef,
     DeleteEndpointMessageRequestTypeDef,
     DeleteEventSubscriptionMessageRequestTypeDef,
     DeleteFleetAdvisorDatabasesRequestRequestTypeDef,
-    DeleteFleetAdvisorDatabasesResponseTypeDef,
     DeleteReplicationInstanceMessageRequestTypeDef,
     DeleteReplicationSubnetGroupMessageRequestTypeDef,
     DeleteReplicationTaskAssessmentRunMessageRequestTypeDef,
     DeleteReplicationTaskMessageRequestTypeDef,
     DescribeApplicableIndividualAssessmentsMessageRequestTypeDef,
-    DescribeApplicableIndividualAssessmentsResponseTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     DescribeEndpointSettingsMessageRequestTypeDef,
     EndpointSettingTypeDef,
     SupportedEndpointTypeTypeDef,
     EventCategoryGroupTypeDef,
     EventTypeDef,
     DescribeFleetAdvisorLsaAnalysisRequestRequestTypeDef,
     FleetAdvisorLsaAnalysisResponseTypeDef,
     FleetAdvisorSchemaObjectResponseTypeDef,
-    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
     DescribeOrderableReplicationInstancesMessageRequestTypeDef,
     OrderableReplicationInstanceTypeDef,
     LimitationTypeDef,
     DescribeRefreshSchemasStatusMessageRequestTypeDef,
     RefreshSchemasStatusTypeDef,
     DescribeReplicationInstanceTaskLogsMessageRequestTypeDef,
     ReplicationInstanceTaskLogTypeDef,
-    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
     DescribeReplicationTaskAssessmentResultsMessageRequestTypeDef,
     ReplicationTaskAssessmentResultTypeDef,
     ReplicationTaskIndividualAssessmentTypeDef,
-    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
     DescribeSchemasMessageRequestTypeDef,
-    DescribeSchemasResponseTypeDef,
     TableStatisticsTypeDef,
-    EmptyResponseMetadataTypeDef,
+    OracleSettingsOutputTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifyReplicationInstanceMessageRequestTypeDef,
     ModifyReplicationSubnetGroupMessageRequestTypeDef,
-    ModifyReplicationTaskMessageRequestTypeDef,
     MoveReplicationTaskMessageRequestTypeDef,
-    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     RdsConfigurationTypeDef,
     RdsRequirementsTypeDef,
     RebootReplicationInstanceMessageRequestTypeDef,
     RecommendationSettingsTypeDef,
     RefreshSchemasMessageRequestTypeDef,
     TableToReloadTypeDef,
-    ReloadTablesResponseTypeDef,
     RemoveTagsFromResourceMessageRequestTypeDef,
     ReplicationPendingModifiedValuesTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ReplicationTaskAssessmentRunProgressTypeDef,
     ReplicationTaskStatsTypeDef,
-    ResponseMetadataTypeDef,
-    RunFleetAdvisorLsaAnalysisResponseTypeDef,
     SchemaShortInfoResponseTypeDef,
     StartReplicationTaskAssessmentMessageRequestTypeDef,
     StartReplicationTaskAssessmentRunMessageRequestTypeDef,
-    StartReplicationTaskMessageRequestTypeDef,
     StopReplicationTaskMessageRequestTypeDef,
     TestConnectionMessageRequestTypeDef,
     UpdateSubscriptionsToEventBridgeMessageRequestTypeDef,
-    UpdateSubscriptionsToEventBridgeResponseTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
     AddTagsToResourceMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateReplicationInstanceMessageRequestTypeDef,
     CreateReplicationSubnetGroupMessageRequestTypeDef,
-    CreateReplicationTaskMessageRequestTypeDef,
-    ImportCertificateMessageRequestTypeDef,
+    CreateFleetAdvisorCollectorResponseTypeDef,
+    DeleteFleetAdvisorDatabasesResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
+    DescribeApplicableIndividualAssessmentsResponseTypeDef,
+    DescribeSchemasResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ReloadTablesResponseTypeDef,
+    RunFleetAdvisorLsaAnalysisResponseTypeDef,
+    UpdateSubscriptionsToEventBridgeResponseTypeDef,
     SubnetTypeDef,
     BatchStartRecommendationsResponseTypeDef,
+    ImportCertificateMessageRequestTypeDef,
     DeleteCertificateResponseTypeDef,
     DescribeCertificatesResponseTypeDef,
     ImportCertificateResponseTypeDef,
     CollectorResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     DescribeConnectionsResponseTypeDef,
     TestConnectionResponseTypeDef,
     CreateEndpointMessageRequestTypeDef,
-    EndpointTypeDef,
     ModifyEndpointMessageRequestTypeDef,
     CreateEventSubscriptionResponseTypeDef,
     DeleteEventSubscriptionResponseTypeDef,
     DescribeEventSubscriptionsResponseTypeDef,
     ModifyEventSubscriptionResponseTypeDef,
+    CreateReplicationTaskMessageRequestTypeDef,
+    ModifyReplicationTaskMessageRequestTypeDef,
+    StartReplicationTaskMessageRequestTypeDef,
     DatabaseResponseTypeDef,
-    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
     DescribeCertificatesMessageRequestTypeDef,
-    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
     DescribeConnectionsMessageRequestTypeDef,
-    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
     DescribeEndpointTypesMessageRequestTypeDef,
-    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
     DescribeEndpointsMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
     DescribeEventsMessageRequestTypeDef,
     DescribeFleetAdvisorCollectorsRequestRequestTypeDef,
     DescribeFleetAdvisorDatabasesRequestRequestTypeDef,
     DescribeFleetAdvisorSchemaObjectSummaryRequestRequestTypeDef,
     DescribeFleetAdvisorSchemasRequestRequestTypeDef,
     DescribePendingMaintenanceActionsMessageRequestTypeDef,
     DescribeRecommendationLimitationsRequestRequestTypeDef,
     DescribeRecommendationsRequestRequestTypeDef,
-    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
     DescribeReplicationInstancesMessageRequestTypeDef,
-    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
     DescribeReplicationSubnetGroupsMessageRequestTypeDef,
     DescribeReplicationTaskAssessmentRunsMessageRequestTypeDef,
     DescribeReplicationTaskIndividualAssessmentsMessageRequestTypeDef,
-    DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
     DescribeReplicationTasksMessageRequestTypeDef,
-    DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
     DescribeTableStatisticsMessageRequestTypeDef,
+    DescribeCertificatesMessageDescribeCertificatesPaginateTypeDef,
+    DescribeConnectionsMessageDescribeConnectionsPaginateTypeDef,
+    DescribeEndpointTypesMessageDescribeEndpointTypesPaginateTypeDef,
+    DescribeEndpointsMessageDescribeEndpointsPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeOrderableReplicationInstancesMessageDescribeOrderableReplicationInstancesPaginateTypeDef,
+    DescribeReplicationInstancesMessageDescribeReplicationInstancesPaginateTypeDef,
+    DescribeReplicationSubnetGroupsMessageDescribeReplicationSubnetGroupsPaginateTypeDef,
+    DescribeReplicationTaskAssessmentResultsMessageDescribeReplicationTaskAssessmentResultsPaginateTypeDef,
+    DescribeReplicationTasksMessageDescribeReplicationTasksPaginateTypeDef,
+    DescribeSchemasMessageDescribeSchemasPaginateTypeDef,
+    DescribeTableStatisticsMessageDescribeTableStatisticsPaginateTypeDef,
     DescribeConnectionsMessageTestConnectionSucceedsWaitTypeDef,
     DescribeEndpointsMessageEndpointDeletedWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceAvailableWaitTypeDef,
     DescribeReplicationInstancesMessageReplicationInstanceDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskDeletedWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskReadyWaitTypeDef,
     DescribeReplicationTasksMessageReplicationTaskRunningWaitTypeDef,
@@ -649,29 +650,31 @@
     DescribeRecommendationLimitationsResponseTypeDef,
     DescribeRefreshSchemasStatusResponseTypeDef,
     RefreshSchemasResponseTypeDef,
     DescribeReplicationInstanceTaskLogsResponseTypeDef,
     DescribeReplicationTaskAssessmentResultsResponseTypeDef,
     DescribeReplicationTaskIndividualAssessmentsResponseTypeDef,
     DescribeTableStatisticsResponseTypeDef,
+    EndpointTypeDef,
+    OracleSettingsUnionTypeDef,
     ResourcePendingMaintenanceActionsTypeDef,
     RdsRecommendationTypeDef,
     StartRecommendationsRequestEntryTypeDef,
     StartRecommendationsRequestRequestTypeDef,
     ReloadTablesMessageRequestTypeDef,
     ReplicationTaskAssessmentRunTypeDef,
     ReplicationTaskTypeDef,
     SchemaResponseTypeDef,
     ReplicationSubnetGroupTypeDef,
     DescribeFleetAdvisorCollectorsResponseTypeDef,
+    DescribeFleetAdvisorDatabasesResponseTypeDef,
     CreateEndpointResponseTypeDef,
     DeleteEndpointResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     ModifyEndpointResponseTypeDef,
-    DescribeFleetAdvisorDatabasesResponseTypeDef,
     ApplyPendingMaintenanceActionResponseTypeDef,
     DescribePendingMaintenanceActionsResponseTypeDef,
     RecommendationDataTypeDef,
     BatchStartRecommendationsRequestRequestTypeDef,
     CancelReplicationTaskAssessmentRunResponseTypeDef,
     DeleteReplicationTaskAssessmentRunResponseTypeDef,
     DescribeReplicationTaskAssessmentRunsResponseTypeDef,
@@ -695,15 +698,15 @@
     DescribeReplicationInstancesResponseTypeDef,
     ModifyReplicationInstanceResponseTypeDef,
     RebootReplicationInstanceResponseTypeDef,
     DescribeRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountQuotaTypeDef:
+def get_value() -> AccountQuotaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dms-2.5.2/types_aiobotocore_dms.egg-info/SOURCES.txt` & `types-aiobotocore-dms-2.5.2.post1/types_aiobotocore_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*


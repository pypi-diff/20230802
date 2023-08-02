# Comparing `tmp/types-aiobotocore-redshift-2.5.2.tar.gz` & `tmp/types-aiobotocore-redshift-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-redshift-2.5.2.tar", last modified: Sat Jul  8 01:44:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-redshift-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
```

## Comparing `types-aiobotocore-redshift-2.5.2.tar` & `types-aiobotocore-redshift-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.206760 types-aiobotocore-redshift-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:38:58.000000 types-aiobotocore-redshift-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-07-08 01:44:11.198759 types-aiobotocore-redshift-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36237 2023-07-08 01:38:58.000000 types-aiobotocore-redshift-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:11.206760 types-aiobotocore-redshift-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:38:58.000000 types-aiobotocore-redshift-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.198759 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-07-08 01:38:58.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-07-08 01:38:58.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:38:58.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   120218 2023-07-08 01:38:59.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   120049 2023-07-08 01:38:58.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-07-08 01:38:59.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-07-08 01:38:59.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    45221 2023-07-08 01:38:59.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    45186 2023-07-08 01:38:59.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:38:58.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   134465 2023-07-08 01:39:04.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   134346 2023-07-08 01:39:01.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:38:58.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-08 01:38:59.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-08 01:38:59.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.198759 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-07-08 01:44:11.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-08 01:44:11.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:11.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:11.000000 types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.237483 types-aiobotocore-redshift-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37716 2023-08-02 14:52:52.237483 types-aiobotocore-redshift-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36194 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.237483 types-aiobotocore-redshift-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.237483 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119965 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119796 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    45116 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45081 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   134049 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133930 2023-08-02 14:47:38.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.237483 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37716 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-redshift-2.5.2/LICENSE` & `types-aiobotocore-redshift-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2/PKG-INFO` & `types-aiobotocore-redshift-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Redshift 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Redshift 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore redshift type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore redshift type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-redshift"></a>
 
 # types-aiobotocore-redshift
 
 [![PyPI - types-aiobotocore-redshift](https://img.shields.io/pypi/v/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-redshift?color=blue)](https://pypistats.org/packages/types-aiobotocore-redshift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift)](https://pepy.tech/project/types-aiobotocore-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Redshift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [types-aiobotocore-redshift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/).
 
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
@@ -528,24 +527,25 @@
 )
 
 
 def check_value(value: ActionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_redshift.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_redshift.type_defs import (
     AcceptReservedNodeExchangeInputMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     AttributeValueTargetTypeDef,
     AccountWithRestoreAccessTypeDef,
     AquaConfigurationTypeDef,
     AssociateDataShareConsumerMessageRequestTypeDef,
     CertificateAssociationTypeDef,
     AuthenticationProfileTypeDef,
     AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
@@ -554,21 +554,18 @@
     AuthorizeSnapshotAccessMessageRequestTypeDef,
     SupportedPlatformTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     SnapshotErrorMessageTypeDef,
     BatchModifyClusterSnapshotsMessageRequestTypeDef,
     CancelResizeMessageRequestTypeDef,
     ClusterAssociatedToScheduleTypeDef,
-    ClusterCredentialsTypeDef,
     RevisionTargetTypeDef,
-    ClusterExtendedCredentialsTypeDef,
     ClusterIamRoleTypeDef,
     ClusterNodeTypeDef,
     ParameterTypeDef,
-    ClusterParameterGroupNameMessageTypeDef,
     ClusterParameterStatusTypeDef,
     TagTypeDef,
     ClusterSecurityGroupMembershipTypeDef,
     ClusterSnapshotCopyStatusTypeDef,
     DataTransferProgressTypeDef,
     DeferredMaintenanceWindowTypeDef,
     ElasticIpStatusTypeDef,
@@ -577,23 +574,20 @@
     ReservedNodeExchangeStatusTypeDef,
     ResizeInfoTypeDef,
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
-    CreateAuthenticationProfileResultTypeDef,
     CreateCustomDomainAssociationMessageRequestTypeDef,
-    CreateCustomDomainAssociationResultTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
-    CustomerStorageMessageTypeDef,
+    TimestampTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
-    DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
     DeleteClusterSecurityGroupMessageRequestTypeDef,
     DeleteClusterSnapshotMessageRequestTypeDef,
     DeleteClusterSubnetGroupMessageRequestTypeDef,
     DeleteCustomDomainAssociationMessageRequestTypeDef,
     DeleteEndpointAccessMessageRequestTypeDef,
@@ -603,139 +597,113 @@
     DeleteScheduledActionMessageRequestTypeDef,
     DeleteSnapshotCopyGrantMessageRequestTypeDef,
     DeleteSnapshotScheduleMessageRequestTypeDef,
     DeleteTagsMessageRequestTypeDef,
     DeleteUsageLimitMessageRequestTypeDef,
     DescribeAccountAttributesMessageRequestTypeDef,
     DescribeAuthenticationProfilesMessageRequestTypeDef,
-    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClusterDbRevisionsMessageRequestTypeDef,
-    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageRequestTypeDef,
-    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterParametersMessageRequestTypeDef,
-    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageRequestTypeDef,
     SnapshotSortingEntityTypeDef,
     WaiterConfigTypeDef,
-    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageRequestTypeDef,
-    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
     DescribeClusterTracksMessageRequestTypeDef,
-    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
     DescribeClusterVersionsMessageRequestTypeDef,
-    DescribeClustersMessageDescribeClustersPaginateTypeDef,
     DescribeClustersMessageRequestTypeDef,
-    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
     DescribeCustomDomainAssociationsMessageRequestTypeDef,
-    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
     DescribeDataSharesForConsumerMessageRequestTypeDef,
-    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
     DescribeDataSharesForProducerMessageRequestTypeDef,
-    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
     DescribeDataSharesMessageRequestTypeDef,
-    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
     DescribeDefaultClusterParametersMessageRequestTypeDef,
-    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
     DescribeEndpointAccessMessageRequestTypeDef,
-    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
     DescribeEndpointAuthorizationMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
     DescribeHsmClientCertificatesMessageRequestTypeDef,
-    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
     DescribeHsmConfigurationsMessageRequestTypeDef,
     DescribeLoggingStatusMessageRequestTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
-    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
     DescribeOrderableClusterOptionsMessageRequestTypeDef,
     DescribePartnersInputMessageRequestTypeDef,
     PartnerIntegrationInfoTypeDef,
-    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
     DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef,
-    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
     DescribeReservedNodeOfferingsMessageRequestTypeDef,
-    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
     DescribeReservedNodesMessageRequestTypeDef,
     DescribeResizeMessageRequestTypeDef,
     ScheduledActionFilterTypeDef,
-    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
     DescribeSnapshotCopyGrantsMessageRequestTypeDef,
-    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
     DescribeSnapshotSchedulesMessageRequestTypeDef,
-    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
     DescribeTableRestoreStatusMessageRequestTypeDef,
-    DescribeTagsMessageDescribeTagsPaginateTypeDef,
     DescribeTagsMessageRequestTypeDef,
-    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
     DescribeUsageLimitsMessageRequestTypeDef,
     DisableLoggingMessageRequestTypeDef,
     DisableSnapshotCopyMessageRequestTypeDef,
     DisassociateDataShareConsumerMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableLoggingMessageRequestTypeDef,
     EnableSnapshotCopyMessageRequestTypeDef,
     EndpointAuthorizationTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
     EventInfoMapTypeDef,
     EventTypeDef,
     GetClusterCredentialsMessageRequestTypeDef,
     GetClusterCredentialsWithIAMMessageRequestTypeDef,
-    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
     GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
-    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
-    LoggingStatusTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
-    ModifyAuthenticationProfileResultTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
-    ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
     ModifyCustomDomainAssociationMessageRequestTypeDef,
-    ModifyCustomDomainAssociationResultTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     ModifySnapshotScheduleMessageRequestTypeDef,
     ModifyUsageLimitMessageRequestTypeDef,
     NetworkInterfaceTypeDef,
     NodeConfigurationOptionTypeDef,
-    PaginatorConfigTypeDef,
     PartnerIntegrationInputMessageRequestTypeDef,
-    PartnerIntegrationOutputMessageTypeDef,
     PauseClusterMessageRequestTypeDef,
     PauseClusterMessageTypeDef,
     PurchaseReservedNodeOfferingMessageRequestTypeDef,
     RebootClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RejectDataShareMessageRequestTypeDef,
     ResizeClusterMessageRequestTypeDef,
     ResizeClusterMessageTypeDef,
-    ResizeProgressMessageTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromClusterSnapshotMessageRequestTypeDef,
     RestoreTableFromClusterSnapshotMessageRequestTypeDef,
     TableRestoreStatusTypeDef,
     ResumeClusterMessageRequestTypeDef,
     ResumeClusterMessageTypeDef,
     RevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     RevokeEndpointAccessMessageRequestTypeDef,
     RevokeSnapshotAccessMessageRequestTypeDef,
     RotateEncryptionKeyMessageRequestTypeDef,
     SupportedOperationTypeDef,
     UpdatePartnerStatusInputMessageRequestTypeDef,
+    ClusterCredentialsTypeDef,
+    ClusterExtendedCredentialsTypeDef,
+    ClusterParameterGroupNameMessageTypeDef,
+    CreateAuthenticationProfileResultTypeDef,
+    CreateCustomDomainAssociationResultTypeDef,
+    CustomerStorageMessageTypeDef,
+    DeleteAuthenticationProfileResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EndpointAuthorizationResponseTypeDef,
+    LoggingStatusTypeDef,
+    ModifyAuthenticationProfileResultTypeDef,
+    ModifyCustomDomainAssociationResultTypeDef,
+    PartnerIntegrationOutputMessageTypeDef,
+    ResizeProgressMessageTypeDef,
     AccountAttributeTypeDef,
     ModifyAquaOutputMessageTypeDef,
     AssociationTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     AvailabilityZoneTypeDef,
     BatchDeleteClusterSnapshotsRequestRequestTypeDef,
     BatchDeleteClusterSnapshotsResultTypeDef,
@@ -761,24 +729,56 @@
     CreateUsageLimitMessageRequestTypeDef,
     EC2SecurityGroupTypeDef,
     EventSubscriptionTypeDef,
     HsmClientCertificateTypeDef,
     HsmConfigurationTypeDef,
     IPRangeTypeDef,
     SnapshotCopyGrantTypeDef,
-    SnapshotScheduleResponseMetadataTypeDef,
+    SnapshotScheduleResponseTypeDef,
     SnapshotScheduleTypeDef,
     SnapshotTypeDef,
     TaggedResourceTypeDef,
-    UsageLimitResponseMetadataTypeDef,
+    UsageLimitResponseTypeDef,
     UsageLimitTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     ClusterVersionsMessageTypeDef,
-    DataShareResponseMetadataTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    ModifyClusterMaintenanceMessageRequestTypeDef,
+    DataShareResponseTypeDef,
     DataShareTypeDef,
+    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
+    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
+    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
+    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
+    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
+    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
+    DescribeClustersMessageDescribeClustersPaginateTypeDef,
+    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
+    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
+    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
+    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
+    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
+    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
+    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
+    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
+    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
+    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
+    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
+    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
+    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
+    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
+    DescribeTagsMessageDescribeTagsPaginateTypeDef,
+    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
+    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef,
     DescribeClusterSnapshotsMessageRequestTypeDef,
     DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef,
     DescribeClustersMessageClusterAvailableWaitTypeDef,
     DescribeClustersMessageClusterDeletedWaitTypeDef,
     DescribeClustersMessageClusterRestoredWaitTypeDef,
     DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
@@ -825,26 +825,26 @@
     SnapshotMessageTypeDef,
     TaggedResourceListMessageTypeDef,
     UsageLimitListTypeDef,
     DescribeDataSharesForConsumerResultTypeDef,
     DescribeDataSharesForProducerResultTypeDef,
     DescribeDataSharesResultTypeDef,
     EventCategoriesMessageTypeDef,
-    EndpointAccessResponseMetadataTypeDef,
+    EndpointAccessResponseTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     ReservedNodeOfferingsMessageTypeDef,
     AcceptReservedNodeExchangeOutputMessageTypeDef,
     PurchaseReservedNodeOfferingResultTypeDef,
     ReservedNodeConfigurationOptionTypeDef,
     ReservedNodesMessageTypeDef,
     CreateScheduledActionMessageRequestTypeDef,
     ModifyScheduledActionMessageRequestTypeDef,
-    ScheduledActionResponseMetadataTypeDef,
+    ScheduledActionResponseTypeDef,
     ScheduledActionTypeDef,
     MaintenanceTrackTypeDef,
     OrderableClusterOptionsMessageTypeDef,
     ClusterSubnetGroupTypeDef,
     AuthorizeClusterSecurityGroupIngressResultTypeDef,
     ClusterSecurityGroupMessageTypeDef,
     CreateClusterSecurityGroupResultTypeDef,
@@ -872,15 +872,15 @@
     ResizeClusterResultTypeDef,
     RestoreFromClusterSnapshotResultTypeDef,
     ResumeClusterResultTypeDef,
     RotateEncryptionKeyResultTypeDef,
 )
 
 
-def get_structure() -> AcceptReservedNodeExchangeInputMessageRequestTypeDef:
+def get_value() -> AcceptReservedNodeExchangeInputMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-redshift-2.5.2/README.md` & `types-aiobotocore-redshift-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-redshift"></a>
 
 # types-aiobotocore-redshift
 
 [![PyPI - types-aiobotocore-redshift](https://img.shields.io/pypi/v/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-redshift?color=blue)](https://pypistats.org/packages/types-aiobotocore-redshift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift)](https://pepy.tech/project/types-aiobotocore-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Redshift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [types-aiobotocore-redshift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/).
 
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
@@ -495,24 +495,25 @@
 )
 
 
 def check_value(value: ActionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_redshift.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_redshift.type_defs import (
     AcceptReservedNodeExchangeInputMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     AttributeValueTargetTypeDef,
     AccountWithRestoreAccessTypeDef,
     AquaConfigurationTypeDef,
     AssociateDataShareConsumerMessageRequestTypeDef,
     CertificateAssociationTypeDef,
     AuthenticationProfileTypeDef,
     AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
@@ -521,21 +522,18 @@
     AuthorizeSnapshotAccessMessageRequestTypeDef,
     SupportedPlatformTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     SnapshotErrorMessageTypeDef,
     BatchModifyClusterSnapshotsMessageRequestTypeDef,
     CancelResizeMessageRequestTypeDef,
     ClusterAssociatedToScheduleTypeDef,
-    ClusterCredentialsTypeDef,
     RevisionTargetTypeDef,
-    ClusterExtendedCredentialsTypeDef,
     ClusterIamRoleTypeDef,
     ClusterNodeTypeDef,
     ParameterTypeDef,
-    ClusterParameterGroupNameMessageTypeDef,
     ClusterParameterStatusTypeDef,
     TagTypeDef,
     ClusterSecurityGroupMembershipTypeDef,
     ClusterSnapshotCopyStatusTypeDef,
     DataTransferProgressTypeDef,
     DeferredMaintenanceWindowTypeDef,
     ElasticIpStatusTypeDef,
@@ -544,23 +542,20 @@
     ReservedNodeExchangeStatusTypeDef,
     ResizeInfoTypeDef,
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
-    CreateAuthenticationProfileResultTypeDef,
     CreateCustomDomainAssociationMessageRequestTypeDef,
-    CreateCustomDomainAssociationResultTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
-    CustomerStorageMessageTypeDef,
+    TimestampTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
-    DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
     DeleteClusterSecurityGroupMessageRequestTypeDef,
     DeleteClusterSnapshotMessageRequestTypeDef,
     DeleteClusterSubnetGroupMessageRequestTypeDef,
     DeleteCustomDomainAssociationMessageRequestTypeDef,
     DeleteEndpointAccessMessageRequestTypeDef,
@@ -570,139 +565,113 @@
     DeleteScheduledActionMessageRequestTypeDef,
     DeleteSnapshotCopyGrantMessageRequestTypeDef,
     DeleteSnapshotScheduleMessageRequestTypeDef,
     DeleteTagsMessageRequestTypeDef,
     DeleteUsageLimitMessageRequestTypeDef,
     DescribeAccountAttributesMessageRequestTypeDef,
     DescribeAuthenticationProfilesMessageRequestTypeDef,
-    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClusterDbRevisionsMessageRequestTypeDef,
-    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageRequestTypeDef,
-    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterParametersMessageRequestTypeDef,
-    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageRequestTypeDef,
     SnapshotSortingEntityTypeDef,
     WaiterConfigTypeDef,
-    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageRequestTypeDef,
-    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
     DescribeClusterTracksMessageRequestTypeDef,
-    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
     DescribeClusterVersionsMessageRequestTypeDef,
-    DescribeClustersMessageDescribeClustersPaginateTypeDef,
     DescribeClustersMessageRequestTypeDef,
-    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
     DescribeCustomDomainAssociationsMessageRequestTypeDef,
-    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
     DescribeDataSharesForConsumerMessageRequestTypeDef,
-    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
     DescribeDataSharesForProducerMessageRequestTypeDef,
-    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
     DescribeDataSharesMessageRequestTypeDef,
-    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
     DescribeDefaultClusterParametersMessageRequestTypeDef,
-    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
     DescribeEndpointAccessMessageRequestTypeDef,
-    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
     DescribeEndpointAuthorizationMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
     DescribeHsmClientCertificatesMessageRequestTypeDef,
-    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
     DescribeHsmConfigurationsMessageRequestTypeDef,
     DescribeLoggingStatusMessageRequestTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
-    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
     DescribeOrderableClusterOptionsMessageRequestTypeDef,
     DescribePartnersInputMessageRequestTypeDef,
     PartnerIntegrationInfoTypeDef,
-    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
     DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef,
-    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
     DescribeReservedNodeOfferingsMessageRequestTypeDef,
-    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
     DescribeReservedNodesMessageRequestTypeDef,
     DescribeResizeMessageRequestTypeDef,
     ScheduledActionFilterTypeDef,
-    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
     DescribeSnapshotCopyGrantsMessageRequestTypeDef,
-    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
     DescribeSnapshotSchedulesMessageRequestTypeDef,
-    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
     DescribeTableRestoreStatusMessageRequestTypeDef,
-    DescribeTagsMessageDescribeTagsPaginateTypeDef,
     DescribeTagsMessageRequestTypeDef,
-    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
     DescribeUsageLimitsMessageRequestTypeDef,
     DisableLoggingMessageRequestTypeDef,
     DisableSnapshotCopyMessageRequestTypeDef,
     DisassociateDataShareConsumerMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableLoggingMessageRequestTypeDef,
     EnableSnapshotCopyMessageRequestTypeDef,
     EndpointAuthorizationTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
     EventInfoMapTypeDef,
     EventTypeDef,
     GetClusterCredentialsMessageRequestTypeDef,
     GetClusterCredentialsWithIAMMessageRequestTypeDef,
-    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
     GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
-    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
-    LoggingStatusTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
-    ModifyAuthenticationProfileResultTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
-    ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
     ModifyCustomDomainAssociationMessageRequestTypeDef,
-    ModifyCustomDomainAssociationResultTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     ModifySnapshotScheduleMessageRequestTypeDef,
     ModifyUsageLimitMessageRequestTypeDef,
     NetworkInterfaceTypeDef,
     NodeConfigurationOptionTypeDef,
-    PaginatorConfigTypeDef,
     PartnerIntegrationInputMessageRequestTypeDef,
-    PartnerIntegrationOutputMessageTypeDef,
     PauseClusterMessageRequestTypeDef,
     PauseClusterMessageTypeDef,
     PurchaseReservedNodeOfferingMessageRequestTypeDef,
     RebootClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RejectDataShareMessageRequestTypeDef,
     ResizeClusterMessageRequestTypeDef,
     ResizeClusterMessageTypeDef,
-    ResizeProgressMessageTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromClusterSnapshotMessageRequestTypeDef,
     RestoreTableFromClusterSnapshotMessageRequestTypeDef,
     TableRestoreStatusTypeDef,
     ResumeClusterMessageRequestTypeDef,
     ResumeClusterMessageTypeDef,
     RevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     RevokeEndpointAccessMessageRequestTypeDef,
     RevokeSnapshotAccessMessageRequestTypeDef,
     RotateEncryptionKeyMessageRequestTypeDef,
     SupportedOperationTypeDef,
     UpdatePartnerStatusInputMessageRequestTypeDef,
+    ClusterCredentialsTypeDef,
+    ClusterExtendedCredentialsTypeDef,
+    ClusterParameterGroupNameMessageTypeDef,
+    CreateAuthenticationProfileResultTypeDef,
+    CreateCustomDomainAssociationResultTypeDef,
+    CustomerStorageMessageTypeDef,
+    DeleteAuthenticationProfileResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EndpointAuthorizationResponseTypeDef,
+    LoggingStatusTypeDef,
+    ModifyAuthenticationProfileResultTypeDef,
+    ModifyCustomDomainAssociationResultTypeDef,
+    PartnerIntegrationOutputMessageTypeDef,
+    ResizeProgressMessageTypeDef,
     AccountAttributeTypeDef,
     ModifyAquaOutputMessageTypeDef,
     AssociationTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     AvailabilityZoneTypeDef,
     BatchDeleteClusterSnapshotsRequestRequestTypeDef,
     BatchDeleteClusterSnapshotsResultTypeDef,
@@ -728,24 +697,56 @@
     CreateUsageLimitMessageRequestTypeDef,
     EC2SecurityGroupTypeDef,
     EventSubscriptionTypeDef,
     HsmClientCertificateTypeDef,
     HsmConfigurationTypeDef,
     IPRangeTypeDef,
     SnapshotCopyGrantTypeDef,
-    SnapshotScheduleResponseMetadataTypeDef,
+    SnapshotScheduleResponseTypeDef,
     SnapshotScheduleTypeDef,
     SnapshotTypeDef,
     TaggedResourceTypeDef,
-    UsageLimitResponseMetadataTypeDef,
+    UsageLimitResponseTypeDef,
     UsageLimitTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     ClusterVersionsMessageTypeDef,
-    DataShareResponseMetadataTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    ModifyClusterMaintenanceMessageRequestTypeDef,
+    DataShareResponseTypeDef,
     DataShareTypeDef,
+    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
+    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
+    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
+    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
+    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
+    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
+    DescribeClustersMessageDescribeClustersPaginateTypeDef,
+    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
+    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
+    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
+    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
+    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
+    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
+    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
+    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
+    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
+    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
+    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
+    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
+    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
+    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
+    DescribeTagsMessageDescribeTagsPaginateTypeDef,
+    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
+    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef,
     DescribeClusterSnapshotsMessageRequestTypeDef,
     DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef,
     DescribeClustersMessageClusterAvailableWaitTypeDef,
     DescribeClustersMessageClusterDeletedWaitTypeDef,
     DescribeClustersMessageClusterRestoredWaitTypeDef,
     DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
@@ -792,26 +793,26 @@
     SnapshotMessageTypeDef,
     TaggedResourceListMessageTypeDef,
     UsageLimitListTypeDef,
     DescribeDataSharesForConsumerResultTypeDef,
     DescribeDataSharesForProducerResultTypeDef,
     DescribeDataSharesResultTypeDef,
     EventCategoriesMessageTypeDef,
-    EndpointAccessResponseMetadataTypeDef,
+    EndpointAccessResponseTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     ReservedNodeOfferingsMessageTypeDef,
     AcceptReservedNodeExchangeOutputMessageTypeDef,
     PurchaseReservedNodeOfferingResultTypeDef,
     ReservedNodeConfigurationOptionTypeDef,
     ReservedNodesMessageTypeDef,
     CreateScheduledActionMessageRequestTypeDef,
     ModifyScheduledActionMessageRequestTypeDef,
-    ScheduledActionResponseMetadataTypeDef,
+    ScheduledActionResponseTypeDef,
     ScheduledActionTypeDef,
     MaintenanceTrackTypeDef,
     OrderableClusterOptionsMessageTypeDef,
     ClusterSubnetGroupTypeDef,
     AuthorizeClusterSecurityGroupIngressResultTypeDef,
     ClusterSecurityGroupMessageTypeDef,
     CreateClusterSecurityGroupResultTypeDef,
@@ -839,15 +840,15 @@
     ResizeClusterResultTypeDef,
     RestoreFromClusterSnapshotResultTypeDef,
     ResumeClusterResultTypeDef,
     RotateEncryptionKeyResultTypeDef,
 )
 
 
-def get_structure() -> AcceptReservedNodeExchangeInputMessageRequestTypeDef:
+def get_value() -> AcceptReservedNodeExchangeInputMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-redshift-2.5.2/setup.py` & `types-aiobotocore-redshift-2.5.2.post1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-redshift",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_redshift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Redshift 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore redshift type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore redshift type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_redshift": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/"
```

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/__init__.py` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/__init__.pyi` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/__main__.py` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Redshift 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Redshift 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift\nOther"
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

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/client.py` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("redshift") as client:
         client: RedshiftClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     ActionTypeType,
     AquaConfigurationStatusType,
@@ -98,15 +97,15 @@
     CreateCustomDomainAssociationResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     CreateHsmClientCertificateResultTypeDef,
     CreateHsmConfigurationResultTypeDef,
     CreateSnapshotCopyGrantResultTypeDef,
     CustomDomainAssociationsMessageTypeDef,
     CustomerStorageMessageTypeDef,
-    DataShareResponseMetadataTypeDef,
+    DataShareResponseTypeDef,
     DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterResultTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     DeleteClusterSnapshotResultTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     DescribeDataSharesForConsumerResultTypeDef,
     DescribeDataSharesForProducerResultTypeDef,
@@ -115,17 +114,17 @@
     DescribePartnersOutputMessageTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     DescribeSnapshotSchedulesOutputMessageTypeDef,
     DisableSnapshotCopyResultTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableSnapshotCopyResultTypeDef,
     EndpointAccessListTypeDef,
-    EndpointAccessResponseMetadataTypeDef,
+    EndpointAccessResponseTypeDef,
     EndpointAuthorizationListTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
+    EndpointAuthorizationResponseTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     EventSubscriptionsMessageTypeDef,
     GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     HsmClientCertificateMessageTypeDef,
     HsmConfigurationMessageTypeDef,
@@ -156,52 +155,50 @@
     RestoreFromClusterSnapshotResultTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     ResumeClusterResultTypeDef,
     RevokeClusterSecurityGroupIngressResultTypeDef,
     RevokeSnapshotAccessResultTypeDef,
     RotateEncryptionKeyResultTypeDef,
     ScheduledActionFilterTypeDef,
-    ScheduledActionResponseMetadataTypeDef,
+    ScheduledActionResponseTypeDef,
     ScheduledActionsMessageTypeDef,
     ScheduledActionTypeTypeDef,
     SnapshotCopyGrantMessageTypeDef,
     SnapshotMessageTypeDef,
-    SnapshotScheduleResponseMetadataTypeDef,
+    SnapshotScheduleResponseTypeDef,
     SnapshotSortingEntityTypeDef,
     TableRestoreStatusMessageTypeDef,
     TaggedResourceListMessageTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TrackListMessageTypeDef,
     UsageLimitListTypeDef,
-    UsageLimitResponseMetadataTypeDef,
+    UsageLimitResponseTypeDef,
 )
 from .waiter import (
     ClusterAvailableWaiter,
     ClusterDeletedWaiter,
     ClusterRestoredWaiter,
     SnapshotAvailableWaiter,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("RedshiftClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessToClusterDeniedFault: Type[BotocoreClientError]
     AccessToSnapshotDeniedFault: Type[BotocoreClientError]
     AuthenticationProfileAlreadyExistsFault: Type[BotocoreClientError]
     AuthenticationProfileNotFoundFault: Type[BotocoreClientError]
     AuthenticationProfileQuotaExceededFault: Type[BotocoreClientError]
     AuthorizationAlreadyExistsFault: Type[BotocoreClientError]
@@ -325,15 +322,14 @@
     UnauthorizedPartnerIntegrationFault: Type[BotocoreClientError]
     UnknownSnapshotCopyRegionFault: Type[BotocoreClientError]
     UnsupportedOperationFault: Type[BotocoreClientError]
     UnsupportedOptionFault: Type[BotocoreClientError]
     UsageLimitAlreadyExistsFault: Type[BotocoreClientError]
     UsageLimitNotFoundFault: Type[BotocoreClientError]
 
-
 class RedshiftClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/)
     """
 
     meta: ClientMeta
@@ -342,88 +338,81 @@
     def exceptions(self) -> Exceptions:
         """
         RedshiftClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#exceptions)
         """
-
     async def accept_reserved_node_exchange(
         self, *, ReservedNodeId: str, TargetReservedNodeOfferingId: str
     ) -> AcceptReservedNodeExchangeOutputMessageTypeDef:
         """
         Exchanges a DC1 Reserved Node for a DC2 Reserved Node with no changes to the
         configuration (term, payment type, or number of nodes) and no additional costs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.accept_reserved_node_exchange)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#accept_reserved_node_exchange)
         """
-
     async def add_partner(
         self, *, AccountId: str, ClusterIdentifier: str, DatabaseName: str, PartnerName: str
     ) -> PartnerIntegrationOutputMessageTypeDef:
         """
         Adds a partner integration to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.add_partner)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#add_partner)
         """
-
     async def associate_data_share_consumer(
         self,
         *,
         DataShareArn: str,
         AssociateEntireAccount: bool = ...,
         ConsumerArn: str = ...,
         ConsumerRegion: str = ...
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, associates a datashare with the account
         (AssociateEntireAccount) or the specified namespace (ConsumerArn).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.associate_data_share_consumer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#associate_data_share_consumer)
         """
-
     async def authorize_cluster_security_group_ingress(
         self,
         *,
         ClusterSecurityGroupName: str,
         CIDRIP: str = ...,
         EC2SecurityGroupName: str = ...,
         EC2SecurityGroupOwnerId: str = ...
     ) -> AuthorizeClusterSecurityGroupIngressResultTypeDef:
         """
         Adds an inbound (ingress) rule to an Amazon Redshift security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_cluster_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#authorize_cluster_security_group_ingress)
         """
-
     async def authorize_data_share(
         self, *, DataShareArn: str, ConsumerIdentifier: str
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a data producer account, authorizes the sharing of a datashare with one or
         more consumer accounts or managing entities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_data_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#authorize_data_share)
         """
-
     async def authorize_endpoint_access(
         self, *, Account: str, ClusterIdentifier: str = ..., VpcIds: Sequence[str] = ...
-    ) -> EndpointAuthorizationResponseMetadataTypeDef:
+    ) -> EndpointAuthorizationResponseTypeDef:
         """
         Grants access to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#authorize_endpoint_access)
         """
-
     async def authorize_snapshot_access(
         self,
         *,
         AccountWithRestoreAccess: str,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotClusterIdentifier: str = ...
@@ -431,63 +420,57 @@
         """
         Authorizes the specified Amazon Web Services account to restore the specified
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_snapshot_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#authorize_snapshot_access)
         """
-
     async def batch_delete_cluster_snapshots(
         self, *, Identifiers: Sequence[DeleteClusterSnapshotMessageTypeDef]
     ) -> BatchDeleteClusterSnapshotsResultTypeDef:
         """
         Deletes a set of cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.batch_delete_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#batch_delete_cluster_snapshots)
         """
-
     async def batch_modify_cluster_snapshots(
         self,
         *,
         SnapshotIdentifierList: Sequence[str],
         ManualSnapshotRetentionPeriod: int = ...,
         Force: bool = ...
     ) -> BatchModifyClusterSnapshotsOutputMessageTypeDef:
         """
         Modifies the settings for a set of cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.batch_modify_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#batch_modify_cluster_snapshots)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#can_paginate)
         """
-
     async def cancel_resize(self, *, ClusterIdentifier: str) -> ResizeProgressMessageTypeDef:
         """
         Cancels a resize operation for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.cancel_resize)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#cancel_resize)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#close)
         """
-
     async def copy_cluster_snapshot(
         self,
         *,
         SourceSnapshotIdentifier: str,
         TargetSnapshotIdentifier: str,
         SourceSnapshotClusterIdentifier: str = ...,
         ManualSnapshotRetentionPeriod: int = ...
@@ -495,25 +478,23 @@
         """
         Copies the specified automated cluster snapshot to a new manual cluster
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.copy_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#copy_cluster_snapshot)
         """
-
     async def create_authentication_profile(
         self, *, AuthenticationProfileName: str, AuthenticationProfileContent: str
     ) -> CreateAuthenticationProfileResultTypeDef:
         """
         Creates an authentication profile with the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_authentication_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_authentication_profile)
         """
-
     async def create_cluster(
         self,
         *,
         ClusterIdentifier: str,
         NodeType: str,
         MasterUsername: str,
         MasterUserPassword: str,
@@ -550,96 +531,89 @@
     ) -> CreateClusterResultTypeDef:
         """
         Creates a new cluster with the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster)
         """
-
     async def create_cluster_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         ParameterGroupFamily: str,
         Description: str,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateClusterParameterGroupResultTypeDef:
         """
         Creates an Amazon Redshift parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_parameter_group)
         """
-
     async def create_cluster_security_group(
         self, *, ClusterSecurityGroupName: str, Description: str, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateClusterSecurityGroupResultTypeDef:
         """
         Creates a new Amazon Redshift security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_security_group)
         """
-
     async def create_cluster_snapshot(
         self,
         *,
         SnapshotIdentifier: str,
         ClusterIdentifier: str,
         ManualSnapshotRetentionPeriod: int = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateClusterSnapshotResultTypeDef:
         """
         Creates a manual snapshot of the specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_snapshot)
         """
-
     async def create_cluster_subnet_group(
         self,
         *,
         ClusterSubnetGroupName: str,
         Description: str,
         SubnetIds: Sequence[str],
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateClusterSubnetGroupResultTypeDef:
         """
         Creates a new Amazon Redshift subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_subnet_group)
         """
-
     async def create_custom_domain_association(
         self, *, CustomDomainName: str, CustomDomainCertificateArn: str, ClusterIdentifier: str
     ) -> CreateCustomDomainAssociationResultTypeDef:
         """
         Used to create a custom domain name for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_custom_domain_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_custom_domain_association)
         """
-
     async def create_endpoint_access(
         self,
         *,
         EndpointName: str,
         SubnetGroupName: str,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...
-    ) -> EndpointAccessResponseMetadataTypeDef:
+    ) -> EndpointAccessResponseTypeDef:
         """
         Creates a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_endpoint_access)
         """
-
     async def create_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         SourceIds: Sequence[str] = ...,
@@ -650,27 +624,25 @@
     ) -> CreateEventSubscriptionResultTypeDef:
         """
         Creates an Amazon Redshift event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_event_subscription)
         """
-
     async def create_hsm_client_certificate(
         self, *, HsmClientCertificateIdentifier: str, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateHsmClientCertificateResultTypeDef:
         """
         Creates an HSM client certificate that an Amazon Redshift cluster will use to
         connect to the client's HSM in order to store and retrieve the keys used to
         encrypt the cluster databases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_hsm_client_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_hsm_client_certificate)
         """
-
     async def create_hsm_configuration(
         self,
         *,
         HsmConfigurationIdentifier: str,
         Description: str,
         HsmIpAddress: str,
         HsmPartitionName: str,
@@ -682,113 +654,105 @@
         Creates an HSM configuration that contains the information required by an Amazon
         Redshift cluster to store and use database encryption keys in a Hardware
         Security Module (HSM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_hsm_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_hsm_configuration)
         """
-
     async def create_scheduled_action(
         self,
         *,
         ScheduledActionName: str,
         TargetAction: ScheduledActionTypeTypeDef,
         Schedule: str,
         IamRole: str,
         ScheduledActionDescription: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Enable: bool = ...
-    ) -> ScheduledActionResponseMetadataTypeDef:
+    ) -> ScheduledActionResponseTypeDef:
         """
         Creates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_scheduled_action)
         """
-
     async def create_snapshot_copy_grant(
         self, *, SnapshotCopyGrantName: str, KmsKeyId: str = ..., Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSnapshotCopyGrantResultTypeDef:
         """
         Creates a snapshot copy grant that permits Amazon Redshift to use an encrypted
         symmetric key from Key Management Service (KMS) to encrypt copied snapshots in a
         destination region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_snapshot_copy_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_snapshot_copy_grant)
         """
-
     async def create_snapshot_schedule(
         self,
         *,
         ScheduleDefinitions: Sequence[str] = ...,
         ScheduleIdentifier: str = ...,
         ScheduleDescription: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         NextInvocations: int = ...
-    ) -> SnapshotScheduleResponseMetadataTypeDef:
+    ) -> SnapshotScheduleResponseTypeDef:
         """
         Create a snapshot schedule that can be associated to a cluster and which
         overrides the default system backup schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_snapshot_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_snapshot_schedule)
         """
-
     async def create_tags(
         self, *, ResourceName: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds tags to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_tags)
         """
-
     async def create_usage_limit(
         self,
         *,
         ClusterIdentifier: str,
         FeatureType: UsageLimitFeatureTypeType,
         LimitType: UsageLimitLimitTypeType,
         Amount: int,
         Period: UsageLimitPeriodType = ...,
         BreachAction: UsageLimitBreachActionType = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> UsageLimitResponseMetadataTypeDef:
+    ) -> UsageLimitResponseTypeDef:
         """
         Creates a usage limit for a specified Amazon Redshift feature on a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_usage_limit)
         """
-
     async def deauthorize_data_share(
         self, *, DataShareArn: str, ConsumerIdentifier: str
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a datashare producer account, removes authorization from the specified
         datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.deauthorize_data_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#deauthorize_data_share)
         """
-
     async def delete_authentication_profile(
         self, *, AuthenticationProfileName: str
     ) -> DeleteAuthenticationProfileResultTypeDef:
         """
         Deletes an authentication profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_authentication_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_authentication_profile)
         """
-
     async def delete_cluster(
         self,
         *,
         ClusterIdentifier: str,
         SkipFinalClusterSnapshot: bool = ...,
         FinalClusterSnapshotIdentifier: str = ...,
         FinalClusterSnapshotRetentionPeriod: int = ...
@@ -796,194 +760,173 @@
         """
         Deletes a previously provisioned cluster without its final snapshot being
         created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_cluster)
         """
-
     async def delete_cluster_parameter_group(
         self, *, ParameterGroupName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a specified Amazon Redshift parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_cluster_parameter_group)
         """
-
     async def delete_cluster_security_group(
         self, *, ClusterSecurityGroupName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an Amazon Redshift security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_cluster_security_group)
         """
-
     async def delete_cluster_snapshot(
         self, *, SnapshotIdentifier: str, SnapshotClusterIdentifier: str = ...
     ) -> DeleteClusterSnapshotResultTypeDef:
         """
         Deletes the specified manual snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_cluster_snapshot)
         """
-
     async def delete_cluster_subnet_group(
         self, *, ClusterSubnetGroupName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified cluster subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_cluster_subnet_group)
         """
-
     async def delete_custom_domain_association(
         self, *, ClusterIdentifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Contains information about deleting a custom domain association for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_custom_domain_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_custom_domain_association)
         """
-
-    async def delete_endpoint_access(
-        self, *, EndpointName: str
-    ) -> EndpointAccessResponseMetadataTypeDef:
+    async def delete_endpoint_access(self, *, EndpointName: str) -> EndpointAccessResponseTypeDef:
         """
         Deletes a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_endpoint_access)
         """
-
     async def delete_event_subscription(
         self, *, SubscriptionName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an Amazon Redshift event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_event_subscription)
         """
-
     async def delete_hsm_client_certificate(
         self, *, HsmClientCertificateIdentifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified HSM client certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_hsm_client_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_hsm_client_certificate)
         """
-
     async def delete_hsm_configuration(
         self, *, HsmConfigurationIdentifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified Amazon Redshift HSM configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_hsm_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_hsm_configuration)
         """
-
     async def delete_partner(
         self, *, AccountId: str, ClusterIdentifier: str, DatabaseName: str, PartnerName: str
     ) -> PartnerIntegrationOutputMessageTypeDef:
         """
         Deletes a partner integration from a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_partner)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_partner)
         """
-
     async def delete_scheduled_action(
         self, *, ScheduledActionName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_scheduled_action)
         """
-
     async def delete_snapshot_copy_grant(
         self, *, SnapshotCopyGrantName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified snapshot copy grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_snapshot_copy_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_snapshot_copy_grant)
         """
-
     async def delete_snapshot_schedule(
         self, *, ScheduleIdentifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a snapshot schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_snapshot_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_snapshot_schedule)
         """
-
     async def delete_tags(
         self, *, ResourceName: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_tags)
         """
-
     async def delete_usage_limit(self, *, UsageLimitId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a usage limit from a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_usage_limit)
         """
-
     async def describe_account_attributes(
         self, *, AttributeNames: Sequence[str] = ...
     ) -> AccountAttributeListTypeDef:
         """
         Returns a list of attributes attached to an account See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/redshift-2012-12-01/DescribeAccountAttributes).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_account_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_account_attributes)
         """
-
     async def describe_authentication_profiles(
         self, *, AuthenticationProfileName: str = ...
     ) -> DescribeAuthenticationProfilesResultTypeDef:
         """
         Describes an authentication profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_authentication_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_authentication_profiles)
         """
-
     async def describe_cluster_db_revisions(
         self, *, ClusterIdentifier: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> ClusterDbRevisionsMessageTypeDef:
         """
         Returns an array of `ClusterDbRevision` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_db_revisions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_db_revisions)
         """
-
     async def describe_cluster_parameter_groups(
         self,
         *,
         ParameterGroupName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -992,15 +935,14 @@
         """
         Returns a list of Amazon Redshift parameter groups, including parameter groups
         you created and the default parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_parameter_groups)
         """
-
     async def describe_cluster_parameters(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...
@@ -1008,15 +950,14 @@
         """
         Returns a detailed list of parameters contained within the specified Amazon
         Redshift parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_parameters)
         """
-
     async def describe_cluster_security_groups(
         self,
         *,
         ClusterSecurityGroupName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1024,24 +965,23 @@
     ) -> ClusterSecurityGroupMessageTypeDef:
         """
         Returns information about Amazon Redshift security groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_security_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_security_groups)
         """
-
     async def describe_cluster_snapshots(
         self,
         *,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotType: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...
@@ -1049,15 +989,14 @@
         """
         Returns one or more snapshot objects, which contain metadata about your cluster
         snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_snapshots)
         """
-
     async def describe_cluster_subnet_groups(
         self,
         *,
         ClusterSubnetGroupName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1066,40 +1005,37 @@
         """
         Returns one or more cluster subnet group objects, which contain metadata about
         your cluster subnet groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_subnet_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_subnet_groups)
         """
-
     async def describe_cluster_tracks(
         self, *, MaintenanceTrackName: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> TrackListMessageTypeDef:
         """
         Returns a list of all the available maintenance tracks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_tracks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_tracks)
         """
-
     async def describe_cluster_versions(
         self,
         *,
         ClusterVersion: str = ...,
         ClusterParameterGroupFamily: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> ClusterVersionsMessageTypeDef:
         """
         Returns descriptions of the available Amazon Redshift cluster versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_versions)
         """
-
     async def describe_clusters(
         self,
         *,
         ClusterIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1109,41 +1045,38 @@
         Returns properties of provisioned clusters including general cluster properties,
         cluster database properties, maintenance and backup properties, and security and
         access properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_clusters)
         """
-
     async def describe_custom_domain_associations(
         self,
         *,
         CustomDomainName: str = ...,
         CustomDomainCertificateArn: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> CustomDomainAssociationsMessageTypeDef:
         """
         Contains information for custom domain associations for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_custom_domain_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_custom_domain_associations)
         """
-
     async def describe_data_shares(
         self, *, DataShareArn: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> DescribeDataSharesResultTypeDef:
         """
         Shows the status of any inbound or outbound datashares available in the
         specified account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_data_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_data_shares)
         """
-
     async def describe_data_shares_for_consumer(
         self,
         *,
         ConsumerArn: str = ...,
         Status: DataShareStatusForConsumerType = ...,
         MaxRecords: int = ...,
         Marker: str = ...
@@ -1151,15 +1084,14 @@
         """
         Returns a list of datashares where the account identifier being called is a
         consumer account identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_data_shares_for_consumer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_data_shares_for_consumer)
         """
-
     async def describe_data_shares_for_producer(
         self,
         *,
         ProducerArn: str = ...,
         Status: DataShareStatusForProducerType = ...,
         MaxRecords: int = ...,
         Marker: str = ...
@@ -1167,25 +1099,23 @@
         """
         Returns a list of datashares when the account identifier being called is a
         producer account identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_data_shares_for_producer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_data_shares_for_producer)
         """
-
     async def describe_default_cluster_parameters(
         self, *, ParameterGroupFamily: str, MaxRecords: int = ..., Marker: str = ...
     ) -> DescribeDefaultClusterParametersResultTypeDef:
         """
         Returns a list of parameter settings for the specified parameter group family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_default_cluster_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_default_cluster_parameters)
         """
-
     async def describe_endpoint_access(
         self,
         *,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         EndpointName: str = ...,
         VpcId: str = ...,
@@ -1194,15 +1124,14 @@
     ) -> EndpointAccessListTypeDef:
         """
         Describes a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_endpoint_access)
         """
-
     async def describe_endpoint_authorization(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         Grantee: bool = ...,
         MaxRecords: int = ...,
@@ -1210,26 +1139,24 @@
     ) -> EndpointAuthorizationListTypeDef:
         """
         Describes an endpoint authorization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_endpoint_authorization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_endpoint_authorization)
         """
-
     async def describe_event_categories(
         self, *, SourceType: str = ...
     ) -> EventCategoriesMessageTypeDef:
         """
         Displays a list of event categories for all event source types, or for a
         specified source type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_event_categories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_event_categories)
         """
-
     async def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1238,34 +1165,32 @@
         """
         Lists descriptions of all the Amazon Redshift event notification subscriptions
         for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_event_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_event_subscriptions)
         """
-
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
         Returns events related to clusters, security groups, snapshots, and parameter
         groups for the past 14 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_events)
         """
-
     async def describe_hsm_client_certificates(
         self,
         *,
         HsmClientCertificateIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1273,15 +1198,14 @@
     ) -> HsmClientCertificateMessageTypeDef:
         """
         Returns information about the specified HSM client certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_hsm_client_certificates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_hsm_client_certificates)
         """
-
     async def describe_hsm_configurations(
         self,
         *,
         HsmConfigurationIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1289,24 +1213,22 @@
     ) -> HsmConfigurationMessageTypeDef:
         """
         Returns information about the specified Amazon Redshift HSM configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_hsm_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_hsm_configurations)
         """
-
     async def describe_logging_status(self, *, ClusterIdentifier: str) -> LoggingStatusTypeDef:
         """
         Describes whether information, such as queries and connection attempts, is being
         logged for the specified Amazon Redshift cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_logging_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_logging_status)
         """
-
     async def describe_node_configuration_options(
         self,
         *,
         ActionType: ActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
@@ -1318,45 +1240,42 @@
         """
         Returns properties of possible node configurations such as node type, number of
         nodes, and disk usage for the specified action type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_node_configuration_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_node_configuration_options)
         """
-
     async def describe_orderable_cluster_options(
         self,
         *,
         ClusterVersion: str = ...,
         NodeType: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> OrderableClusterOptionsMessageTypeDef:
         """
         Returns a list of orderable cluster options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_orderable_cluster_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_orderable_cluster_options)
         """
-
     async def describe_partners(
         self,
         *,
         AccountId: str,
         ClusterIdentifier: str,
         DatabaseName: str = ...,
         PartnerName: str = ...
     ) -> DescribePartnersOutputMessageTypeDef:
         """
         Returns information about the partner integrations defined for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_partners)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_partners)
         """
-
     async def describe_reserved_node_exchange_status(
         self,
         *,
         ReservedNodeId: str = ...,
         ReservedNodeExchangeRequestId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...
@@ -1364,64 +1283,59 @@
         """
         Returns exchange status details and associated metadata for a reserved-node
         exchange.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_reserved_node_exchange_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_reserved_node_exchange_status)
         """
-
     async def describe_reserved_node_offerings(
         self, *, ReservedNodeOfferingId: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> ReservedNodeOfferingsMessageTypeDef:
         """
         Returns a list of the available reserved node offerings by Amazon Redshift with
         their descriptions including the node type, the fixed and recurring costs of
         reserving the node and duration the node will be reserved for you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_reserved_node_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_reserved_node_offerings)
         """
-
     async def describe_reserved_nodes(
         self, *, ReservedNodeId: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> ReservedNodesMessageTypeDef:
         """
         Returns the descriptions of the reserved nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_reserved_nodes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_reserved_nodes)
         """
-
     async def describe_resize(self, *, ClusterIdentifier: str) -> ResizeProgressMessageTypeDef:
         """
         Returns information about the last resize operation for the specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_resize)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_resize)
         """
-
     async def describe_scheduled_actions(
         self,
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...
     ) -> ScheduledActionsMessageTypeDef:
         """
         Describes properties of scheduled actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_scheduled_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_scheduled_actions)
         """
-
     async def describe_snapshot_copy_grants(
         self,
         *,
         SnapshotCopyGrantName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1430,15 +1344,14 @@
         """
         Returns a list of snapshot copy grants owned by the Amazon Web Services account
         in the destination region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_snapshot_copy_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_snapshot_copy_grants)
         """
-
     async def describe_snapshot_schedules(
         self,
         *,
         ClusterIdentifier: str = ...,
         ScheduleIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
@@ -1447,23 +1360,21 @@
     ) -> DescribeSnapshotSchedulesOutputMessageTypeDef:
         """
         Returns a list of snapshot schedules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_snapshot_schedules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_snapshot_schedules)
         """
-
     async def describe_storage(self) -> CustomerStorageMessageTypeDef:
         """
         Returns account level backups storage size and provisional storage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_storage)
         """
-
     async def describe_table_restore_status(
         self,
         *,
         ClusterIdentifier: str = ...,
         TableRestoreRequestId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...
@@ -1471,15 +1382,14 @@
         """
         Lists the status of one or more table restore requests made using the
         RestoreTableFromClusterSnapshot API action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_table_restore_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_table_restore_status)
         """
-
     async def describe_tags(
         self,
         *,
         ResourceName: str = ...,
         ResourceType: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
@@ -1488,15 +1398,14 @@
     ) -> TaggedResourceListMessageTypeDef:
         """
         Returns a list of tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_tags)
         """
-
     async def describe_usage_limits(
         self,
         *,
         UsageLimitId: str = ...,
         ClusterIdentifier: str = ...,
         FeatureType: UsageLimitFeatureTypeType = ...,
         MaxRecords: int = ...,
@@ -1506,51 +1415,47 @@
     ) -> UsageLimitListTypeDef:
         """
         Shows usage limits on a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_usage_limits)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_usage_limits)
         """
-
     async def disable_logging(self, *, ClusterIdentifier: str) -> LoggingStatusTypeDef:
         """
         Stops logging information, such as queries and connection attempts, for the
         specified Amazon Redshift cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.disable_logging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#disable_logging)
         """
-
     async def disable_snapshot_copy(
         self, *, ClusterIdentifier: str
     ) -> DisableSnapshotCopyResultTypeDef:
         """
         Disables the automatic copying of snapshots from one region to another region
         for a specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.disable_snapshot_copy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#disable_snapshot_copy)
         """
-
     async def disassociate_data_share_consumer(
         self,
         *,
         DataShareArn: str,
         DisassociateEntireAccount: bool = ...,
         ConsumerArn: str = ...,
         ConsumerRegion: str = ...
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, remove association for the specified
         datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.disassociate_data_share_consumer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#disassociate_data_share_consumer)
         """
-
     async def enable_logging(
         self,
         *,
         ClusterIdentifier: str,
         BucketName: str = ...,
         S3KeyPrefix: str = ...,
         LogDestinationType: LogDestinationTypeType = ...,
@@ -1559,15 +1464,14 @@
         """
         Starts logging information, such as queries and connection attempts, for the
         specified Amazon Redshift cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.enable_logging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#enable_logging)
         """
-
     async def enable_snapshot_copy(
         self,
         *,
         ClusterIdentifier: str,
         DestinationRegion: str,
         RetentionPeriod: int = ...,
         SnapshotCopyGrantName: str = ...,
@@ -1576,29 +1480,27 @@
         """
         Enables the automatic copy of snapshots from one region to another region for a
         specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.enable_snapshot_copy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#enable_snapshot_copy)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#generate_presigned_url)
         """
-
     async def get_cluster_credentials(
         self,
         *,
         DbUser: str,
         DbName: str = ...,
         ClusterIdentifier: str = ...,
         DurationSeconds: int = ...,
@@ -1609,15 +1511,14 @@
         """
         Returns a database user name and temporary password with temporary authorization
         to log on to an Amazon Redshift database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_cluster_credentials)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_cluster_credentials)
         """
-
     async def get_cluster_credentials_with_iam(
         self,
         *,
         DbName: str = ...,
         ClusterIdentifier: str = ...,
         DurationSeconds: int = ...,
         CustomDomainName: str = ...
@@ -1625,15 +1526,14 @@
         """
         Returns a database user name and temporary password with temporary authorization
         to log in to an Amazon Redshift database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_cluster_credentials_with_iam)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_cluster_credentials_with_iam)
         """
-
     async def get_reserved_node_exchange_configuration_options(
         self,
         *,
         ActionType: ReservedNodeExchangeActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         MaxRecords: int = ...,
@@ -1641,46 +1541,42 @@
     ) -> GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef:
         """
         Gets the configuration options for the reserved-node exchange.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_reserved_node_exchange_configuration_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_reserved_node_exchange_configuration_options)
         """
-
     async def get_reserved_node_exchange_offerings(
         self, *, ReservedNodeId: str, MaxRecords: int = ..., Marker: str = ...
     ) -> GetReservedNodeExchangeOfferingsOutputMessageTypeDef:
         """
         Returns an array of DC2 ReservedNodeOfferings that matches the payment type,
         term, and usage price of the given DC1 reserved node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_reserved_node_exchange_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_reserved_node_exchange_offerings)
         """
-
     async def modify_aqua_configuration(
         self, *, ClusterIdentifier: str, AquaConfigurationStatus: AquaConfigurationStatusType = ...
     ) -> ModifyAquaOutputMessageTypeDef:
         """
         This operation is retired.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_aqua_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_aqua_configuration)
         """
-
     async def modify_authentication_profile(
         self, *, AuthenticationProfileName: str, AuthenticationProfileContent: str
     ) -> ModifyAuthenticationProfileResultTypeDef:
         """
         Modifies an authentication profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_authentication_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_authentication_profile)
         """
-
     async def modify_cluster(
         self,
         *,
         ClusterIdentifier: str,
         ClusterType: str = ...,
         NodeType: str = ...,
         NumberOfNodes: int = ...,
@@ -1708,25 +1604,23 @@
     ) -> ModifyClusterResultTypeDef:
         """
         Modifies the settings for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster)
         """
-
     async def modify_cluster_db_revision(
         self, *, ClusterIdentifier: str, RevisionTarget: str
     ) -> ModifyClusterDbRevisionResultTypeDef:
         """
         Modifies the database revision of a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_db_revision)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_db_revision)
         """
-
     async def modify_cluster_iam_roles(
         self,
         *,
         ClusterIdentifier: str,
         AddIamRoles: Sequence[str] = ...,
         RemoveIamRoles: Sequence[str] = ...,
         DefaultIamRoleArn: str = ...
@@ -1734,104 +1628,96 @@
         """
         Modifies the list of Identity and Access Management (IAM) roles that can be used
         by the cluster to access other Amazon Web Services services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_iam_roles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_iam_roles)
         """
-
     async def modify_cluster_maintenance(
         self,
         *,
         ClusterIdentifier: str,
         DeferMaintenance: bool = ...,
         DeferMaintenanceIdentifier: str = ...,
-        DeferMaintenanceStartTime: Union[datetime, str] = ...,
-        DeferMaintenanceEndTime: Union[datetime, str] = ...,
+        DeferMaintenanceStartTime: TimestampTypeDef = ...,
+        DeferMaintenanceEndTime: TimestampTypeDef = ...,
         DeferMaintenanceDuration: int = ...
     ) -> ModifyClusterMaintenanceResultTypeDef:
         """
         Modifies the maintenance settings of a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_maintenance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_maintenance)
         """
-
     async def modify_cluster_parameter_group(
         self, *, ParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
     ) -> ClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_parameter_group)
         """
-
     async def modify_cluster_snapshot(
         self,
         *,
         SnapshotIdentifier: str,
         ManualSnapshotRetentionPeriod: int = ...,
         Force: bool = ...
     ) -> ModifyClusterSnapshotResultTypeDef:
         """
         Modifies the settings for a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_snapshot)
         """
-
     async def modify_cluster_snapshot_schedule(
         self,
         *,
         ClusterIdentifier: str,
         ScheduleIdentifier: str = ...,
         DisassociateSchedule: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Modifies a snapshot schedule for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_snapshot_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_snapshot_schedule)
         """
-
     async def modify_cluster_subnet_group(
         self, *, ClusterSubnetGroupName: str, SubnetIds: Sequence[str], Description: str = ...
     ) -> ModifyClusterSubnetGroupResultTypeDef:
         """
         Modifies a cluster subnet group to include the specified list of VPC subnets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_subnet_group)
         """
-
     async def modify_custom_domain_association(
         self,
         *,
         ClusterIdentifier: str,
         CustomDomainName: str = ...,
         CustomDomainCertificateArn: str = ...
     ) -> ModifyCustomDomainAssociationResultTypeDef:
         """
         Contains information for changing a custom domain association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_custom_domain_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_custom_domain_association)
         """
-
     async def modify_endpoint_access(
         self, *, EndpointName: str, VpcSecurityGroupIds: Sequence[str] = ...
-    ) -> EndpointAccessResponseMetadataTypeDef:
+    ) -> EndpointAccessResponseTypeDef:
         """
         Modifies a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_endpoint_access)
         """
-
     async def modify_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         SourceIds: Sequence[str] = ...,
@@ -1841,119 +1727,109 @@
     ) -> ModifyEventSubscriptionResultTypeDef:
         """
         Modifies an existing Amazon Redshift event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_event_subscription)
         """
-
     async def modify_scheduled_action(
         self,
         *,
         ScheduledActionName: str,
         TargetAction: ScheduledActionTypeTypeDef = ...,
         Schedule: str = ...,
         IamRole: str = ...,
         ScheduledActionDescription: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Enable: bool = ...
-    ) -> ScheduledActionResponseMetadataTypeDef:
+    ) -> ScheduledActionResponseTypeDef:
         """
         Modifies a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_scheduled_action)
         """
-
     async def modify_snapshot_copy_retention_period(
         self, *, ClusterIdentifier: str, RetentionPeriod: int, Manual: bool = ...
     ) -> ModifySnapshotCopyRetentionPeriodResultTypeDef:
         """
         Modifies the number of days to retain snapshots in the destination Amazon Web
         Services Region after they are copied from the source Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_snapshot_copy_retention_period)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_snapshot_copy_retention_period)
         """
-
     async def modify_snapshot_schedule(
         self, *, ScheduleIdentifier: str, ScheduleDefinitions: Sequence[str]
-    ) -> SnapshotScheduleResponseMetadataTypeDef:
+    ) -> SnapshotScheduleResponseTypeDef:
         """
         Modifies a snapshot schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_snapshot_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_snapshot_schedule)
         """
-
     async def modify_usage_limit(
         self,
         *,
         UsageLimitId: str,
         Amount: int = ...,
         BreachAction: UsageLimitBreachActionType = ...
-    ) -> UsageLimitResponseMetadataTypeDef:
+    ) -> UsageLimitResponseTypeDef:
         """
         Modifies a usage limit in a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_usage_limit)
         """
-
     async def pause_cluster(self, *, ClusterIdentifier: str) -> PauseClusterResultTypeDef:
         """
         Pauses a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.pause_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#pause_cluster)
         """
-
     async def purchase_reserved_node_offering(
         self, *, ReservedNodeOfferingId: str, NodeCount: int = ...
     ) -> PurchaseReservedNodeOfferingResultTypeDef:
         """
         Allows you to purchase reserved nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.purchase_reserved_node_offering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#purchase_reserved_node_offering)
         """
-
     async def reboot_cluster(self, *, ClusterIdentifier: str) -> RebootClusterResultTypeDef:
         """
         Reboots a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.reboot_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#reboot_cluster)
         """
-
-    async def reject_data_share(self, *, DataShareArn: str) -> DataShareResponseMetadataTypeDef:
+    async def reject_data_share(self, *, DataShareArn: str) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, rejects the specified datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.reject_data_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#reject_data_share)
         """
-
     async def reset_cluster_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         ResetAllParameters: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...
     ) -> ClusterParameterGroupNameMessageTypeDef:
         """
         Sets one or more parameters of the specified parameter group to their default
         values and sets the source values of the parameters to "engine-default".
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.reset_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#reset_cluster_parameter_group)
         """
-
     async def resize_cluster(
         self,
         *,
         ClusterIdentifier: str,
         ClusterType: str = ...,
         NodeType: str = ...,
         NumberOfNodes: int = ...,
@@ -1963,15 +1839,14 @@
     ) -> ResizeClusterResultTypeDef:
         """
         Changes the size of the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.resize_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#resize_cluster)
         """
-
     async def restore_from_cluster_snapshot(
         self,
         *,
         ClusterIdentifier: str,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotClusterIdentifier: str = ...,
@@ -2007,15 +1882,14 @@
     ) -> RestoreFromClusterSnapshotResultTypeDef:
         """
         Creates a new cluster from a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.restore_from_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#restore_from_cluster_snapshot)
         """
-
     async def restore_table_from_cluster_snapshot(
         self,
         *,
         ClusterIdentifier: str,
         SnapshotIdentifier: str,
         SourceDatabaseName: str,
         SourceTableName: str,
@@ -2027,23 +1901,21 @@
     ) -> RestoreTableFromClusterSnapshotResultTypeDef:
         """
         Creates a new table from a table in an Amazon Redshift cluster snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.restore_table_from_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#restore_table_from_cluster_snapshot)
         """
-
     async def resume_cluster(self, *, ClusterIdentifier: str) -> ResumeClusterResultTypeDef:
         """
         Resumes a paused cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.resume_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#resume_cluster)
         """
-
     async def revoke_cluster_security_group_ingress(
         self,
         *,
         ClusterSecurityGroupName: str,
         CIDRIP: str = ...,
         EC2SecurityGroupName: str = ...,
         EC2SecurityGroupOwnerId: str = ...
@@ -2051,30 +1923,28 @@
         """
         Revokes an ingress rule in an Amazon Redshift security group for a previously
         authorized IP range or Amazon EC2 security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_cluster_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#revoke_cluster_security_group_ingress)
         """
-
     async def revoke_endpoint_access(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         VpcIds: Sequence[str] = ...,
         Force: bool = ...
-    ) -> EndpointAuthorizationResponseMetadataTypeDef:
+    ) -> EndpointAuthorizationResponseTypeDef:
         """
         Revokes access to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#revoke_endpoint_access)
         """
-
     async def revoke_snapshot_access(
         self,
         *,
         AccountWithRestoreAccess: str,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotClusterIdentifier: str = ...
@@ -2082,25 +1952,23 @@
         """
         Removes the ability of the specified Amazon Web Services account to restore the
         specified snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_snapshot_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#revoke_snapshot_access)
         """
-
     async def rotate_encryption_key(
         self, *, ClusterIdentifier: str
     ) -> RotateEncryptionKeyResultTypeDef:
         """
         Rotates the encryption keys for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.rotate_encryption_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#rotate_encryption_key)
         """
-
     async def update_partner_status(
         self,
         *,
         AccountId: str,
         ClusterIdentifier: str,
         DatabaseName: str,
         PartnerName: str,
@@ -2109,340 +1977,301 @@
     ) -> PartnerIntegrationOutputMessageTypeDef:
         """
         Updates the status of a partner integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.update_partner_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#update_partner_status)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_db_revisions"]
     ) -> DescribeClusterDbRevisionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_parameter_groups"]
     ) -> DescribeClusterParameterGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_parameters"]
     ) -> DescribeClusterParametersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_security_groups"]
     ) -> DescribeClusterSecurityGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_snapshots"]
     ) -> DescribeClusterSnapshotsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_subnet_groups"]
     ) -> DescribeClusterSubnetGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_tracks"]
     ) -> DescribeClusterTracksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_versions"]
     ) -> DescribeClusterVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_clusters"]
     ) -> DescribeClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_custom_domain_associations"]
     ) -> DescribeCustomDomainAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_data_shares"]
     ) -> DescribeDataSharesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_data_shares_for_consumer"]
     ) -> DescribeDataSharesForConsumerPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_data_shares_for_producer"]
     ) -> DescribeDataSharesForProducerPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_default_cluster_parameters"]
     ) -> DescribeDefaultClusterParametersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_endpoint_access"]
     ) -> DescribeEndpointAccessPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_endpoint_authorization"]
     ) -> DescribeEndpointAuthorizationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_event_subscriptions"]
     ) -> DescribeEventSubscriptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["describe_events"]) -> DescribeEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_hsm_client_certificates"]
     ) -> DescribeHsmClientCertificatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_hsm_configurations"]
     ) -> DescribeHsmConfigurationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_node_configuration_options"]
     ) -> DescribeNodeConfigurationOptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_orderable_cluster_options"]
     ) -> DescribeOrderableClusterOptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_reserved_node_exchange_status"]
     ) -> DescribeReservedNodeExchangeStatusPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_reserved_node_offerings"]
     ) -> DescribeReservedNodeOfferingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_reserved_nodes"]
     ) -> DescribeReservedNodesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scheduled_actions"]
     ) -> DescribeScheduledActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_snapshot_copy_grants"]
     ) -> DescribeSnapshotCopyGrantsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_snapshot_schedules"]
     ) -> DescribeSnapshotSchedulesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_table_restore_status"]
     ) -> DescribeTableRestoreStatusPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["describe_tags"]) -> DescribeTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_usage_limits"]
     ) -> DescribeUsageLimitsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_reserved_node_exchange_configuration_options"]
     ) -> GetReservedNodeExchangeConfigurationOptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_reserved_node_exchange_offerings"]
     ) -> GetReservedNodeExchangeOfferingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["cluster_available"]) -> ClusterAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["cluster_deleted"]) -> ClusterDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["cluster_restored"]) -> ClusterRestoredWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_waiter)
         """
-
     @overload
     def get_waiter(self, waiter_name: Literal["snapshot_available"]) -> SnapshotAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_waiter)
         """
-
     async def __aenter__(self) -> "RedshiftClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/)
         """
```

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/client.pyi` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("redshift") as client:
         client: RedshiftClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     ActionTypeType,
     AquaConfigurationStatusType,
@@ -98,15 +97,15 @@
     CreateCustomDomainAssociationResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     CreateHsmClientCertificateResultTypeDef,
     CreateHsmConfigurationResultTypeDef,
     CreateSnapshotCopyGrantResultTypeDef,
     CustomDomainAssociationsMessageTypeDef,
     CustomerStorageMessageTypeDef,
-    DataShareResponseMetadataTypeDef,
+    DataShareResponseTypeDef,
     DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterResultTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     DeleteClusterSnapshotResultTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     DescribeDataSharesForConsumerResultTypeDef,
     DescribeDataSharesForProducerResultTypeDef,
@@ -115,17 +114,17 @@
     DescribePartnersOutputMessageTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     DescribeSnapshotSchedulesOutputMessageTypeDef,
     DisableSnapshotCopyResultTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableSnapshotCopyResultTypeDef,
     EndpointAccessListTypeDef,
-    EndpointAccessResponseMetadataTypeDef,
+    EndpointAccessResponseTypeDef,
     EndpointAuthorizationListTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
+    EndpointAuthorizationResponseTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     EventSubscriptionsMessageTypeDef,
     GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     HsmClientCertificateMessageTypeDef,
     HsmConfigurationMessageTypeDef,
@@ -156,49 +155,53 @@
     RestoreFromClusterSnapshotResultTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     ResumeClusterResultTypeDef,
     RevokeClusterSecurityGroupIngressResultTypeDef,
     RevokeSnapshotAccessResultTypeDef,
     RotateEncryptionKeyResultTypeDef,
     ScheduledActionFilterTypeDef,
-    ScheduledActionResponseMetadataTypeDef,
+    ScheduledActionResponseTypeDef,
     ScheduledActionsMessageTypeDef,
     ScheduledActionTypeTypeDef,
     SnapshotCopyGrantMessageTypeDef,
     SnapshotMessageTypeDef,
-    SnapshotScheduleResponseMetadataTypeDef,
+    SnapshotScheduleResponseTypeDef,
     SnapshotSortingEntityTypeDef,
     TableRestoreStatusMessageTypeDef,
     TaggedResourceListMessageTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TrackListMessageTypeDef,
     UsageLimitListTypeDef,
-    UsageLimitResponseMetadataTypeDef,
+    UsageLimitResponseTypeDef,
 )
 from .waiter import (
     ClusterAvailableWaiter,
     ClusterDeletedWaiter,
     ClusterRestoredWaiter,
     SnapshotAvailableWaiter,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("RedshiftClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessToClusterDeniedFault: Type[BotocoreClientError]
     AccessToSnapshotDeniedFault: Type[BotocoreClientError]
     AuthenticationProfileAlreadyExistsFault: Type[BotocoreClientError]
     AuthenticationProfileNotFoundFault: Type[BotocoreClientError]
     AuthenticationProfileQuotaExceededFault: Type[BotocoreClientError]
     AuthorizationAlreadyExistsFault: Type[BotocoreClientError]
@@ -322,14 +325,15 @@
     UnauthorizedPartnerIntegrationFault: Type[BotocoreClientError]
     UnknownSnapshotCopyRegionFault: Type[BotocoreClientError]
     UnsupportedOperationFault: Type[BotocoreClientError]
     UnsupportedOptionFault: Type[BotocoreClientError]
     UsageLimitAlreadyExistsFault: Type[BotocoreClientError]
     UsageLimitNotFoundFault: Type[BotocoreClientError]
 
+
 class RedshiftClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/)
     """
 
     meta: ClientMeta
@@ -338,81 +342,88 @@
     def exceptions(self) -> Exceptions:
         """
         RedshiftClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#exceptions)
         """
+
     async def accept_reserved_node_exchange(
         self, *, ReservedNodeId: str, TargetReservedNodeOfferingId: str
     ) -> AcceptReservedNodeExchangeOutputMessageTypeDef:
         """
         Exchanges a DC1 Reserved Node for a DC2 Reserved Node with no changes to the
         configuration (term, payment type, or number of nodes) and no additional costs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.accept_reserved_node_exchange)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#accept_reserved_node_exchange)
         """
+
     async def add_partner(
         self, *, AccountId: str, ClusterIdentifier: str, DatabaseName: str, PartnerName: str
     ) -> PartnerIntegrationOutputMessageTypeDef:
         """
         Adds a partner integration to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.add_partner)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#add_partner)
         """
+
     async def associate_data_share_consumer(
         self,
         *,
         DataShareArn: str,
         AssociateEntireAccount: bool = ...,
         ConsumerArn: str = ...,
         ConsumerRegion: str = ...
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, associates a datashare with the account
         (AssociateEntireAccount) or the specified namespace (ConsumerArn).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.associate_data_share_consumer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#associate_data_share_consumer)
         """
+
     async def authorize_cluster_security_group_ingress(
         self,
         *,
         ClusterSecurityGroupName: str,
         CIDRIP: str = ...,
         EC2SecurityGroupName: str = ...,
         EC2SecurityGroupOwnerId: str = ...
     ) -> AuthorizeClusterSecurityGroupIngressResultTypeDef:
         """
         Adds an inbound (ingress) rule to an Amazon Redshift security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_cluster_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#authorize_cluster_security_group_ingress)
         """
+
     async def authorize_data_share(
         self, *, DataShareArn: str, ConsumerIdentifier: str
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a data producer account, authorizes the sharing of a datashare with one or
         more consumer accounts or managing entities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_data_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#authorize_data_share)
         """
+
     async def authorize_endpoint_access(
         self, *, Account: str, ClusterIdentifier: str = ..., VpcIds: Sequence[str] = ...
-    ) -> EndpointAuthorizationResponseMetadataTypeDef:
+    ) -> EndpointAuthorizationResponseTypeDef:
         """
         Grants access to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#authorize_endpoint_access)
         """
+
     async def authorize_snapshot_access(
         self,
         *,
         AccountWithRestoreAccess: str,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotClusterIdentifier: str = ...
@@ -420,57 +431,63 @@
         """
         Authorizes the specified Amazon Web Services account to restore the specified
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_snapshot_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#authorize_snapshot_access)
         """
+
     async def batch_delete_cluster_snapshots(
         self, *, Identifiers: Sequence[DeleteClusterSnapshotMessageTypeDef]
     ) -> BatchDeleteClusterSnapshotsResultTypeDef:
         """
         Deletes a set of cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.batch_delete_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#batch_delete_cluster_snapshots)
         """
+
     async def batch_modify_cluster_snapshots(
         self,
         *,
         SnapshotIdentifierList: Sequence[str],
         ManualSnapshotRetentionPeriod: int = ...,
         Force: bool = ...
     ) -> BatchModifyClusterSnapshotsOutputMessageTypeDef:
         """
         Modifies the settings for a set of cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.batch_modify_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#batch_modify_cluster_snapshots)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#can_paginate)
         """
+
     async def cancel_resize(self, *, ClusterIdentifier: str) -> ResizeProgressMessageTypeDef:
         """
         Cancels a resize operation for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.cancel_resize)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#cancel_resize)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#close)
         """
+
     async def copy_cluster_snapshot(
         self,
         *,
         SourceSnapshotIdentifier: str,
         TargetSnapshotIdentifier: str,
         SourceSnapshotClusterIdentifier: str = ...,
         ManualSnapshotRetentionPeriod: int = ...
@@ -478,23 +495,25 @@
         """
         Copies the specified automated cluster snapshot to a new manual cluster
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.copy_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#copy_cluster_snapshot)
         """
+
     async def create_authentication_profile(
         self, *, AuthenticationProfileName: str, AuthenticationProfileContent: str
     ) -> CreateAuthenticationProfileResultTypeDef:
         """
         Creates an authentication profile with the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_authentication_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_authentication_profile)
         """
+
     async def create_cluster(
         self,
         *,
         ClusterIdentifier: str,
         NodeType: str,
         MasterUsername: str,
         MasterUserPassword: str,
@@ -531,89 +550,96 @@
     ) -> CreateClusterResultTypeDef:
         """
         Creates a new cluster with the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster)
         """
+
     async def create_cluster_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         ParameterGroupFamily: str,
         Description: str,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateClusterParameterGroupResultTypeDef:
         """
         Creates an Amazon Redshift parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_parameter_group)
         """
+
     async def create_cluster_security_group(
         self, *, ClusterSecurityGroupName: str, Description: str, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateClusterSecurityGroupResultTypeDef:
         """
         Creates a new Amazon Redshift security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_security_group)
         """
+
     async def create_cluster_snapshot(
         self,
         *,
         SnapshotIdentifier: str,
         ClusterIdentifier: str,
         ManualSnapshotRetentionPeriod: int = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateClusterSnapshotResultTypeDef:
         """
         Creates a manual snapshot of the specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_snapshot)
         """
+
     async def create_cluster_subnet_group(
         self,
         *,
         ClusterSubnetGroupName: str,
         Description: str,
         SubnetIds: Sequence[str],
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateClusterSubnetGroupResultTypeDef:
         """
         Creates a new Amazon Redshift subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_cluster_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_cluster_subnet_group)
         """
+
     async def create_custom_domain_association(
         self, *, CustomDomainName: str, CustomDomainCertificateArn: str, ClusterIdentifier: str
     ) -> CreateCustomDomainAssociationResultTypeDef:
         """
         Used to create a custom domain name for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_custom_domain_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_custom_domain_association)
         """
+
     async def create_endpoint_access(
         self,
         *,
         EndpointName: str,
         SubnetGroupName: str,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...
-    ) -> EndpointAccessResponseMetadataTypeDef:
+    ) -> EndpointAccessResponseTypeDef:
         """
         Creates a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_endpoint_access)
         """
+
     async def create_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         SourceIds: Sequence[str] = ...,
@@ -624,25 +650,27 @@
     ) -> CreateEventSubscriptionResultTypeDef:
         """
         Creates an Amazon Redshift event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_event_subscription)
         """
+
     async def create_hsm_client_certificate(
         self, *, HsmClientCertificateIdentifier: str, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateHsmClientCertificateResultTypeDef:
         """
         Creates an HSM client certificate that an Amazon Redshift cluster will use to
         connect to the client's HSM in order to store and retrieve the keys used to
         encrypt the cluster databases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_hsm_client_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_hsm_client_certificate)
         """
+
     async def create_hsm_configuration(
         self,
         *,
         HsmConfigurationIdentifier: str,
         Description: str,
         HsmIpAddress: str,
         HsmPartitionName: str,
@@ -654,105 +682,113 @@
         Creates an HSM configuration that contains the information required by an Amazon
         Redshift cluster to store and use database encryption keys in a Hardware
         Security Module (HSM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_hsm_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_hsm_configuration)
         """
+
     async def create_scheduled_action(
         self,
         *,
         ScheduledActionName: str,
         TargetAction: ScheduledActionTypeTypeDef,
         Schedule: str,
         IamRole: str,
         ScheduledActionDescription: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Enable: bool = ...
-    ) -> ScheduledActionResponseMetadataTypeDef:
+    ) -> ScheduledActionResponseTypeDef:
         """
         Creates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_scheduled_action)
         """
+
     async def create_snapshot_copy_grant(
         self, *, SnapshotCopyGrantName: str, KmsKeyId: str = ..., Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSnapshotCopyGrantResultTypeDef:
         """
         Creates a snapshot copy grant that permits Amazon Redshift to use an encrypted
         symmetric key from Key Management Service (KMS) to encrypt copied snapshots in a
         destination region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_snapshot_copy_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_snapshot_copy_grant)
         """
+
     async def create_snapshot_schedule(
         self,
         *,
         ScheduleDefinitions: Sequence[str] = ...,
         ScheduleIdentifier: str = ...,
         ScheduleDescription: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         NextInvocations: int = ...
-    ) -> SnapshotScheduleResponseMetadataTypeDef:
+    ) -> SnapshotScheduleResponseTypeDef:
         """
         Create a snapshot schedule that can be associated to a cluster and which
         overrides the default system backup schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_snapshot_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_snapshot_schedule)
         """
+
     async def create_tags(
         self, *, ResourceName: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds tags to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_tags)
         """
+
     async def create_usage_limit(
         self,
         *,
         ClusterIdentifier: str,
         FeatureType: UsageLimitFeatureTypeType,
         LimitType: UsageLimitLimitTypeType,
         Amount: int,
         Period: UsageLimitPeriodType = ...,
         BreachAction: UsageLimitBreachActionType = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> UsageLimitResponseMetadataTypeDef:
+    ) -> UsageLimitResponseTypeDef:
         """
         Creates a usage limit for a specified Amazon Redshift feature on a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#create_usage_limit)
         """
+
     async def deauthorize_data_share(
         self, *, DataShareArn: str, ConsumerIdentifier: str
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a datashare producer account, removes authorization from the specified
         datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.deauthorize_data_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#deauthorize_data_share)
         """
+
     async def delete_authentication_profile(
         self, *, AuthenticationProfileName: str
     ) -> DeleteAuthenticationProfileResultTypeDef:
         """
         Deletes an authentication profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_authentication_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_authentication_profile)
         """
+
     async def delete_cluster(
         self,
         *,
         ClusterIdentifier: str,
         SkipFinalClusterSnapshot: bool = ...,
         FinalClusterSnapshotIdentifier: str = ...,
         FinalClusterSnapshotRetentionPeriod: int = ...
@@ -760,175 +796,192 @@
         """
         Deletes a previously provisioned cluster without its final snapshot being
         created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_cluster)
         """
+
     async def delete_cluster_parameter_group(
         self, *, ParameterGroupName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a specified Amazon Redshift parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_cluster_parameter_group)
         """
+
     async def delete_cluster_security_group(
         self, *, ClusterSecurityGroupName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an Amazon Redshift security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_cluster_security_group)
         """
+
     async def delete_cluster_snapshot(
         self, *, SnapshotIdentifier: str, SnapshotClusterIdentifier: str = ...
     ) -> DeleteClusterSnapshotResultTypeDef:
         """
         Deletes the specified manual snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_cluster_snapshot)
         """
+
     async def delete_cluster_subnet_group(
         self, *, ClusterSubnetGroupName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified cluster subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_cluster_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_cluster_subnet_group)
         """
+
     async def delete_custom_domain_association(
         self, *, ClusterIdentifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Contains information about deleting a custom domain association for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_custom_domain_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_custom_domain_association)
         """
-    async def delete_endpoint_access(
-        self, *, EndpointName: str
-    ) -> EndpointAccessResponseMetadataTypeDef:
+
+    async def delete_endpoint_access(self, *, EndpointName: str) -> EndpointAccessResponseTypeDef:
         """
         Deletes a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_endpoint_access)
         """
+
     async def delete_event_subscription(
         self, *, SubscriptionName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an Amazon Redshift event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_event_subscription)
         """
+
     async def delete_hsm_client_certificate(
         self, *, HsmClientCertificateIdentifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified HSM client certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_hsm_client_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_hsm_client_certificate)
         """
+
     async def delete_hsm_configuration(
         self, *, HsmConfigurationIdentifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified Amazon Redshift HSM configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_hsm_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_hsm_configuration)
         """
+
     async def delete_partner(
         self, *, AccountId: str, ClusterIdentifier: str, DatabaseName: str, PartnerName: str
     ) -> PartnerIntegrationOutputMessageTypeDef:
         """
         Deletes a partner integration from a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_partner)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_partner)
         """
+
     async def delete_scheduled_action(
         self, *, ScheduledActionName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_scheduled_action)
         """
+
     async def delete_snapshot_copy_grant(
         self, *, SnapshotCopyGrantName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified snapshot copy grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_snapshot_copy_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_snapshot_copy_grant)
         """
+
     async def delete_snapshot_schedule(
         self, *, ScheduleIdentifier: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a snapshot schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_snapshot_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_snapshot_schedule)
         """
+
     async def delete_tags(
         self, *, ResourceName: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_tags)
         """
+
     async def delete_usage_limit(self, *, UsageLimitId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a usage limit from a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#delete_usage_limit)
         """
+
     async def describe_account_attributes(
         self, *, AttributeNames: Sequence[str] = ...
     ) -> AccountAttributeListTypeDef:
         """
         Returns a list of attributes attached to an account See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/redshift-2012-12-01/DescribeAccountAttributes).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_account_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_account_attributes)
         """
+
     async def describe_authentication_profiles(
         self, *, AuthenticationProfileName: str = ...
     ) -> DescribeAuthenticationProfilesResultTypeDef:
         """
         Describes an authentication profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_authentication_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_authentication_profiles)
         """
+
     async def describe_cluster_db_revisions(
         self, *, ClusterIdentifier: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> ClusterDbRevisionsMessageTypeDef:
         """
         Returns an array of `ClusterDbRevision` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_db_revisions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_db_revisions)
         """
+
     async def describe_cluster_parameter_groups(
         self,
         *,
         ParameterGroupName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -937,14 +990,15 @@
         """
         Returns a list of Amazon Redshift parameter groups, including parameter groups
         you created and the default parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_parameter_groups)
         """
+
     async def describe_cluster_parameters(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...
@@ -952,14 +1006,15 @@
         """
         Returns a detailed list of parameters contained within the specified Amazon
         Redshift parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_parameters)
         """
+
     async def describe_cluster_security_groups(
         self,
         *,
         ClusterSecurityGroupName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -967,23 +1022,24 @@
     ) -> ClusterSecurityGroupMessageTypeDef:
         """
         Returns information about Amazon Redshift security groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_security_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_security_groups)
         """
+
     async def describe_cluster_snapshots(
         self,
         *,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotType: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...
@@ -991,14 +1047,15 @@
         """
         Returns one or more snapshot objects, which contain metadata about your cluster
         snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_snapshots)
         """
+
     async def describe_cluster_subnet_groups(
         self,
         *,
         ClusterSubnetGroupName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1007,37 +1064,40 @@
         """
         Returns one or more cluster subnet group objects, which contain metadata about
         your cluster subnet groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_subnet_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_subnet_groups)
         """
+
     async def describe_cluster_tracks(
         self, *, MaintenanceTrackName: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> TrackListMessageTypeDef:
         """
         Returns a list of all the available maintenance tracks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_tracks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_tracks)
         """
+
     async def describe_cluster_versions(
         self,
         *,
         ClusterVersion: str = ...,
         ClusterParameterGroupFamily: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> ClusterVersionsMessageTypeDef:
         """
         Returns descriptions of the available Amazon Redshift cluster versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_cluster_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_cluster_versions)
         """
+
     async def describe_clusters(
         self,
         *,
         ClusterIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1047,38 +1107,41 @@
         Returns properties of provisioned clusters including general cluster properties,
         cluster database properties, maintenance and backup properties, and security and
         access properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_clusters)
         """
+
     async def describe_custom_domain_associations(
         self,
         *,
         CustomDomainName: str = ...,
         CustomDomainCertificateArn: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> CustomDomainAssociationsMessageTypeDef:
         """
         Contains information for custom domain associations for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_custom_domain_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_custom_domain_associations)
         """
+
     async def describe_data_shares(
         self, *, DataShareArn: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> DescribeDataSharesResultTypeDef:
         """
         Shows the status of any inbound or outbound datashares available in the
         specified account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_data_shares)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_data_shares)
         """
+
     async def describe_data_shares_for_consumer(
         self,
         *,
         ConsumerArn: str = ...,
         Status: DataShareStatusForConsumerType = ...,
         MaxRecords: int = ...,
         Marker: str = ...
@@ -1086,14 +1149,15 @@
         """
         Returns a list of datashares where the account identifier being called is a
         consumer account identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_data_shares_for_consumer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_data_shares_for_consumer)
         """
+
     async def describe_data_shares_for_producer(
         self,
         *,
         ProducerArn: str = ...,
         Status: DataShareStatusForProducerType = ...,
         MaxRecords: int = ...,
         Marker: str = ...
@@ -1101,23 +1165,25 @@
         """
         Returns a list of datashares when the account identifier being called is a
         producer account identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_data_shares_for_producer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_data_shares_for_producer)
         """
+
     async def describe_default_cluster_parameters(
         self, *, ParameterGroupFamily: str, MaxRecords: int = ..., Marker: str = ...
     ) -> DescribeDefaultClusterParametersResultTypeDef:
         """
         Returns a list of parameter settings for the specified parameter group family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_default_cluster_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_default_cluster_parameters)
         """
+
     async def describe_endpoint_access(
         self,
         *,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         EndpointName: str = ...,
         VpcId: str = ...,
@@ -1126,14 +1192,15 @@
     ) -> EndpointAccessListTypeDef:
         """
         Describes a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_endpoint_access)
         """
+
     async def describe_endpoint_authorization(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         Grantee: bool = ...,
         MaxRecords: int = ...,
@@ -1141,24 +1208,26 @@
     ) -> EndpointAuthorizationListTypeDef:
         """
         Describes an endpoint authorization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_endpoint_authorization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_endpoint_authorization)
         """
+
     async def describe_event_categories(
         self, *, SourceType: str = ...
     ) -> EventCategoriesMessageTypeDef:
         """
         Displays a list of event categories for all event source types, or for a
         specified source type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_event_categories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_event_categories)
         """
+
     async def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1167,32 +1236,34 @@
         """
         Lists descriptions of all the Amazon Redshift event notification subscriptions
         for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_event_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_event_subscriptions)
         """
+
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
         Returns events related to clusters, security groups, snapshots, and parameter
         groups for the past 14 days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_events)
         """
+
     async def describe_hsm_client_certificates(
         self,
         *,
         HsmClientCertificateIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1200,14 +1271,15 @@
     ) -> HsmClientCertificateMessageTypeDef:
         """
         Returns information about the specified HSM client certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_hsm_client_certificates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_hsm_client_certificates)
         """
+
     async def describe_hsm_configurations(
         self,
         *,
         HsmConfigurationIdentifier: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1215,22 +1287,24 @@
     ) -> HsmConfigurationMessageTypeDef:
         """
         Returns information about the specified Amazon Redshift HSM configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_hsm_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_hsm_configurations)
         """
+
     async def describe_logging_status(self, *, ClusterIdentifier: str) -> LoggingStatusTypeDef:
         """
         Describes whether information, such as queries and connection attempts, is being
         logged for the specified Amazon Redshift cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_logging_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_logging_status)
         """
+
     async def describe_node_configuration_options(
         self,
         *,
         ActionType: ActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
@@ -1242,42 +1316,45 @@
         """
         Returns properties of possible node configurations such as node type, number of
         nodes, and disk usage for the specified action type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_node_configuration_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_node_configuration_options)
         """
+
     async def describe_orderable_cluster_options(
         self,
         *,
         ClusterVersion: str = ...,
         NodeType: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...
     ) -> OrderableClusterOptionsMessageTypeDef:
         """
         Returns a list of orderable cluster options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_orderable_cluster_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_orderable_cluster_options)
         """
+
     async def describe_partners(
         self,
         *,
         AccountId: str,
         ClusterIdentifier: str,
         DatabaseName: str = ...,
         PartnerName: str = ...
     ) -> DescribePartnersOutputMessageTypeDef:
         """
         Returns information about the partner integrations defined for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_partners)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_partners)
         """
+
     async def describe_reserved_node_exchange_status(
         self,
         *,
         ReservedNodeId: str = ...,
         ReservedNodeExchangeRequestId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...
@@ -1285,59 +1362,64 @@
         """
         Returns exchange status details and associated metadata for a reserved-node
         exchange.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_reserved_node_exchange_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_reserved_node_exchange_status)
         """
+
     async def describe_reserved_node_offerings(
         self, *, ReservedNodeOfferingId: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> ReservedNodeOfferingsMessageTypeDef:
         """
         Returns a list of the available reserved node offerings by Amazon Redshift with
         their descriptions including the node type, the fixed and recurring costs of
         reserving the node and duration the node will be reserved for you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_reserved_node_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_reserved_node_offerings)
         """
+
     async def describe_reserved_nodes(
         self, *, ReservedNodeId: str = ..., MaxRecords: int = ..., Marker: str = ...
     ) -> ReservedNodesMessageTypeDef:
         """
         Returns the descriptions of the reserved nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_reserved_nodes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_reserved_nodes)
         """
+
     async def describe_resize(self, *, ClusterIdentifier: str) -> ResizeProgressMessageTypeDef:
         """
         Returns information about the last resize operation for the specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_resize)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_resize)
         """
+
     async def describe_scheduled_actions(
         self,
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
         Marker: str = ...,
         MaxRecords: int = ...
     ) -> ScheduledActionsMessageTypeDef:
         """
         Describes properties of scheduled actions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_scheduled_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_scheduled_actions)
         """
+
     async def describe_snapshot_copy_grants(
         self,
         *,
         SnapshotCopyGrantName: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         TagKeys: Sequence[str] = ...,
@@ -1346,14 +1428,15 @@
         """
         Returns a list of snapshot copy grants owned by the Amazon Web Services account
         in the destination region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_snapshot_copy_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_snapshot_copy_grants)
         """
+
     async def describe_snapshot_schedules(
         self,
         *,
         ClusterIdentifier: str = ...,
         ScheduleIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
@@ -1362,21 +1445,23 @@
     ) -> DescribeSnapshotSchedulesOutputMessageTypeDef:
         """
         Returns a list of snapshot schedules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_snapshot_schedules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_snapshot_schedules)
         """
+
     async def describe_storage(self) -> CustomerStorageMessageTypeDef:
         """
         Returns account level backups storage size and provisional storage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_storage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_storage)
         """
+
     async def describe_table_restore_status(
         self,
         *,
         ClusterIdentifier: str = ...,
         TableRestoreRequestId: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...
@@ -1384,14 +1469,15 @@
         """
         Lists the status of one or more table restore requests made using the
         RestoreTableFromClusterSnapshot API action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_table_restore_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_table_restore_status)
         """
+
     async def describe_tags(
         self,
         *,
         ResourceName: str = ...,
         ResourceType: str = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
@@ -1400,14 +1486,15 @@
     ) -> TaggedResourceListMessageTypeDef:
         """
         Returns a list of tags.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_tags)
         """
+
     async def describe_usage_limits(
         self,
         *,
         UsageLimitId: str = ...,
         ClusterIdentifier: str = ...,
         FeatureType: UsageLimitFeatureTypeType = ...,
         MaxRecords: int = ...,
@@ -1417,47 +1504,51 @@
     ) -> UsageLimitListTypeDef:
         """
         Shows usage limits on a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.describe_usage_limits)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#describe_usage_limits)
         """
+
     async def disable_logging(self, *, ClusterIdentifier: str) -> LoggingStatusTypeDef:
         """
         Stops logging information, such as queries and connection attempts, for the
         specified Amazon Redshift cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.disable_logging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#disable_logging)
         """
+
     async def disable_snapshot_copy(
         self, *, ClusterIdentifier: str
     ) -> DisableSnapshotCopyResultTypeDef:
         """
         Disables the automatic copying of snapshots from one region to another region
         for a specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.disable_snapshot_copy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#disable_snapshot_copy)
         """
+
     async def disassociate_data_share_consumer(
         self,
         *,
         DataShareArn: str,
         DisassociateEntireAccount: bool = ...,
         ConsumerArn: str = ...,
         ConsumerRegion: str = ...
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, remove association for the specified
         datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.disassociate_data_share_consumer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#disassociate_data_share_consumer)
         """
+
     async def enable_logging(
         self,
         *,
         ClusterIdentifier: str,
         BucketName: str = ...,
         S3KeyPrefix: str = ...,
         LogDestinationType: LogDestinationTypeType = ...,
@@ -1466,14 +1557,15 @@
         """
         Starts logging information, such as queries and connection attempts, for the
         specified Amazon Redshift cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.enable_logging)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#enable_logging)
         """
+
     async def enable_snapshot_copy(
         self,
         *,
         ClusterIdentifier: str,
         DestinationRegion: str,
         RetentionPeriod: int = ...,
         SnapshotCopyGrantName: str = ...,
@@ -1482,27 +1574,29 @@
         """
         Enables the automatic copy of snapshots from one region to another region for a
         specified cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.enable_snapshot_copy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#enable_snapshot_copy)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#generate_presigned_url)
         """
+
     async def get_cluster_credentials(
         self,
         *,
         DbUser: str,
         DbName: str = ...,
         ClusterIdentifier: str = ...,
         DurationSeconds: int = ...,
@@ -1513,14 +1607,15 @@
         """
         Returns a database user name and temporary password with temporary authorization
         to log on to an Amazon Redshift database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_cluster_credentials)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_cluster_credentials)
         """
+
     async def get_cluster_credentials_with_iam(
         self,
         *,
         DbName: str = ...,
         ClusterIdentifier: str = ...,
         DurationSeconds: int = ...,
         CustomDomainName: str = ...
@@ -1528,14 +1623,15 @@
         """
         Returns a database user name and temporary password with temporary authorization
         to log in to an Amazon Redshift database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_cluster_credentials_with_iam)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_cluster_credentials_with_iam)
         """
+
     async def get_reserved_node_exchange_configuration_options(
         self,
         *,
         ActionType: ReservedNodeExchangeActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         MaxRecords: int = ...,
@@ -1543,42 +1639,46 @@
     ) -> GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef:
         """
         Gets the configuration options for the reserved-node exchange.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_reserved_node_exchange_configuration_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_reserved_node_exchange_configuration_options)
         """
+
     async def get_reserved_node_exchange_offerings(
         self, *, ReservedNodeId: str, MaxRecords: int = ..., Marker: str = ...
     ) -> GetReservedNodeExchangeOfferingsOutputMessageTypeDef:
         """
         Returns an array of DC2 ReservedNodeOfferings that matches the payment type,
         term, and usage price of the given DC1 reserved node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_reserved_node_exchange_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_reserved_node_exchange_offerings)
         """
+
     async def modify_aqua_configuration(
         self, *, ClusterIdentifier: str, AquaConfigurationStatus: AquaConfigurationStatusType = ...
     ) -> ModifyAquaOutputMessageTypeDef:
         """
         This operation is retired.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_aqua_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_aqua_configuration)
         """
+
     async def modify_authentication_profile(
         self, *, AuthenticationProfileName: str, AuthenticationProfileContent: str
     ) -> ModifyAuthenticationProfileResultTypeDef:
         """
         Modifies an authentication profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_authentication_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_authentication_profile)
         """
+
     async def modify_cluster(
         self,
         *,
         ClusterIdentifier: str,
         ClusterType: str = ...,
         NodeType: str = ...,
         NumberOfNodes: int = ...,
@@ -1606,23 +1706,25 @@
     ) -> ModifyClusterResultTypeDef:
         """
         Modifies the settings for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster)
         """
+
     async def modify_cluster_db_revision(
         self, *, ClusterIdentifier: str, RevisionTarget: str
     ) -> ModifyClusterDbRevisionResultTypeDef:
         """
         Modifies the database revision of a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_db_revision)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_db_revision)
         """
+
     async def modify_cluster_iam_roles(
         self,
         *,
         ClusterIdentifier: str,
         AddIamRoles: Sequence[str] = ...,
         RemoveIamRoles: Sequence[str] = ...,
         DefaultIamRoleArn: str = ...
@@ -1630,96 +1732,104 @@
         """
         Modifies the list of Identity and Access Management (IAM) roles that can be used
         by the cluster to access other Amazon Web Services services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_iam_roles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_iam_roles)
         """
+
     async def modify_cluster_maintenance(
         self,
         *,
         ClusterIdentifier: str,
         DeferMaintenance: bool = ...,
         DeferMaintenanceIdentifier: str = ...,
-        DeferMaintenanceStartTime: Union[datetime, str] = ...,
-        DeferMaintenanceEndTime: Union[datetime, str] = ...,
+        DeferMaintenanceStartTime: TimestampTypeDef = ...,
+        DeferMaintenanceEndTime: TimestampTypeDef = ...,
         DeferMaintenanceDuration: int = ...
     ) -> ModifyClusterMaintenanceResultTypeDef:
         """
         Modifies the maintenance settings of a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_maintenance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_maintenance)
         """
+
     async def modify_cluster_parameter_group(
         self, *, ParameterGroupName: str, Parameters: Sequence[ParameterTypeDef]
     ) -> ClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_parameter_group)
         """
+
     async def modify_cluster_snapshot(
         self,
         *,
         SnapshotIdentifier: str,
         ManualSnapshotRetentionPeriod: int = ...,
         Force: bool = ...
     ) -> ModifyClusterSnapshotResultTypeDef:
         """
         Modifies the settings for a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_snapshot)
         """
+
     async def modify_cluster_snapshot_schedule(
         self,
         *,
         ClusterIdentifier: str,
         ScheduleIdentifier: str = ...,
         DisassociateSchedule: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Modifies a snapshot schedule for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_snapshot_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_snapshot_schedule)
         """
+
     async def modify_cluster_subnet_group(
         self, *, ClusterSubnetGroupName: str, SubnetIds: Sequence[str], Description: str = ...
     ) -> ModifyClusterSubnetGroupResultTypeDef:
         """
         Modifies a cluster subnet group to include the specified list of VPC subnets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_cluster_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_cluster_subnet_group)
         """
+
     async def modify_custom_domain_association(
         self,
         *,
         ClusterIdentifier: str,
         CustomDomainName: str = ...,
         CustomDomainCertificateArn: str = ...
     ) -> ModifyCustomDomainAssociationResultTypeDef:
         """
         Contains information for changing a custom domain association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_custom_domain_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_custom_domain_association)
         """
+
     async def modify_endpoint_access(
         self, *, EndpointName: str, VpcSecurityGroupIds: Sequence[str] = ...
-    ) -> EndpointAccessResponseMetadataTypeDef:
+    ) -> EndpointAccessResponseTypeDef:
         """
         Modifies a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_endpoint_access)
         """
+
     async def modify_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         SourceIds: Sequence[str] = ...,
@@ -1729,109 +1839,119 @@
     ) -> ModifyEventSubscriptionResultTypeDef:
         """
         Modifies an existing Amazon Redshift event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_event_subscription)
         """
+
     async def modify_scheduled_action(
         self,
         *,
         ScheduledActionName: str,
         TargetAction: ScheduledActionTypeTypeDef = ...,
         Schedule: str = ...,
         IamRole: str = ...,
         ScheduledActionDescription: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Enable: bool = ...
-    ) -> ScheduledActionResponseMetadataTypeDef:
+    ) -> ScheduledActionResponseTypeDef:
         """
         Modifies a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_scheduled_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_scheduled_action)
         """
+
     async def modify_snapshot_copy_retention_period(
         self, *, ClusterIdentifier: str, RetentionPeriod: int, Manual: bool = ...
     ) -> ModifySnapshotCopyRetentionPeriodResultTypeDef:
         """
         Modifies the number of days to retain snapshots in the destination Amazon Web
         Services Region after they are copied from the source Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_snapshot_copy_retention_period)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_snapshot_copy_retention_period)
         """
+
     async def modify_snapshot_schedule(
         self, *, ScheduleIdentifier: str, ScheduleDefinitions: Sequence[str]
-    ) -> SnapshotScheduleResponseMetadataTypeDef:
+    ) -> SnapshotScheduleResponseTypeDef:
         """
         Modifies a snapshot schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_snapshot_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_snapshot_schedule)
         """
+
     async def modify_usage_limit(
         self,
         *,
         UsageLimitId: str,
         Amount: int = ...,
         BreachAction: UsageLimitBreachActionType = ...
-    ) -> UsageLimitResponseMetadataTypeDef:
+    ) -> UsageLimitResponseTypeDef:
         """
         Modifies a usage limit in a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_usage_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#modify_usage_limit)
         """
+
     async def pause_cluster(self, *, ClusterIdentifier: str) -> PauseClusterResultTypeDef:
         """
         Pauses a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.pause_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#pause_cluster)
         """
+
     async def purchase_reserved_node_offering(
         self, *, ReservedNodeOfferingId: str, NodeCount: int = ...
     ) -> PurchaseReservedNodeOfferingResultTypeDef:
         """
         Allows you to purchase reserved nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.purchase_reserved_node_offering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#purchase_reserved_node_offering)
         """
+
     async def reboot_cluster(self, *, ClusterIdentifier: str) -> RebootClusterResultTypeDef:
         """
         Reboots a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.reboot_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#reboot_cluster)
         """
-    async def reject_data_share(self, *, DataShareArn: str) -> DataShareResponseMetadataTypeDef:
+
+    async def reject_data_share(self, *, DataShareArn: str) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, rejects the specified datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.reject_data_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#reject_data_share)
         """
+
     async def reset_cluster_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         ResetAllParameters: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...
     ) -> ClusterParameterGroupNameMessageTypeDef:
         """
         Sets one or more parameters of the specified parameter group to their default
         values and sets the source values of the parameters to "engine-default".
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.reset_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#reset_cluster_parameter_group)
         """
+
     async def resize_cluster(
         self,
         *,
         ClusterIdentifier: str,
         ClusterType: str = ...,
         NodeType: str = ...,
         NumberOfNodes: int = ...,
@@ -1841,14 +1961,15 @@
     ) -> ResizeClusterResultTypeDef:
         """
         Changes the size of the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.resize_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#resize_cluster)
         """
+
     async def restore_from_cluster_snapshot(
         self,
         *,
         ClusterIdentifier: str,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotClusterIdentifier: str = ...,
@@ -1884,14 +2005,15 @@
     ) -> RestoreFromClusterSnapshotResultTypeDef:
         """
         Creates a new cluster from a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.restore_from_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#restore_from_cluster_snapshot)
         """
+
     async def restore_table_from_cluster_snapshot(
         self,
         *,
         ClusterIdentifier: str,
         SnapshotIdentifier: str,
         SourceDatabaseName: str,
         SourceTableName: str,
@@ -1903,21 +2025,23 @@
     ) -> RestoreTableFromClusterSnapshotResultTypeDef:
         """
         Creates a new table from a table in an Amazon Redshift cluster snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.restore_table_from_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#restore_table_from_cluster_snapshot)
         """
+
     async def resume_cluster(self, *, ClusterIdentifier: str) -> ResumeClusterResultTypeDef:
         """
         Resumes a paused cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.resume_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#resume_cluster)
         """
+
     async def revoke_cluster_security_group_ingress(
         self,
         *,
         ClusterSecurityGroupName: str,
         CIDRIP: str = ...,
         EC2SecurityGroupName: str = ...,
         EC2SecurityGroupOwnerId: str = ...
@@ -1925,28 +2049,30 @@
         """
         Revokes an ingress rule in an Amazon Redshift security group for a previously
         authorized IP range or Amazon EC2 security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_cluster_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#revoke_cluster_security_group_ingress)
         """
+
     async def revoke_endpoint_access(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         VpcIds: Sequence[str] = ...,
         Force: bool = ...
-    ) -> EndpointAuthorizationResponseMetadataTypeDef:
+    ) -> EndpointAuthorizationResponseTypeDef:
         """
         Revokes access to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_endpoint_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#revoke_endpoint_access)
         """
+
     async def revoke_snapshot_access(
         self,
         *,
         AccountWithRestoreAccess: str,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotClusterIdentifier: str = ...
@@ -1954,23 +2080,25 @@
         """
         Removes the ability of the specified Amazon Web Services account to restore the
         specified snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_snapshot_access)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#revoke_snapshot_access)
         """
+
     async def rotate_encryption_key(
         self, *, ClusterIdentifier: str
     ) -> RotateEncryptionKeyResultTypeDef:
         """
         Rotates the encryption keys for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.rotate_encryption_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#rotate_encryption_key)
         """
+
     async def update_partner_status(
         self,
         *,
         AccountId: str,
         ClusterIdentifier: str,
         DatabaseName: str,
         PartnerName: str,
@@ -1979,301 +2107,340 @@
     ) -> PartnerIntegrationOutputMessageTypeDef:
         """
         Updates the status of a partner integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.update_partner_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#update_partner_status)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_db_revisions"]
     ) -> DescribeClusterDbRevisionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_parameter_groups"]
     ) -> DescribeClusterParameterGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_parameters"]
     ) -> DescribeClusterParametersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_security_groups"]
     ) -> DescribeClusterSecurityGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_snapshots"]
     ) -> DescribeClusterSnapshotsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_subnet_groups"]
     ) -> DescribeClusterSubnetGroupsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_tracks"]
     ) -> DescribeClusterTracksPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_cluster_versions"]
     ) -> DescribeClusterVersionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_clusters"]
     ) -> DescribeClustersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_custom_domain_associations"]
     ) -> DescribeCustomDomainAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_data_shares"]
     ) -> DescribeDataSharesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_data_shares_for_consumer"]
     ) -> DescribeDataSharesForConsumerPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_data_shares_for_producer"]
     ) -> DescribeDataSharesForProducerPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_default_cluster_parameters"]
     ) -> DescribeDefaultClusterParametersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_endpoint_access"]
     ) -> DescribeEndpointAccessPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_endpoint_authorization"]
     ) -> DescribeEndpointAuthorizationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_event_subscriptions"]
     ) -> DescribeEventSubscriptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["describe_events"]) -> DescribeEventsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_hsm_client_certificates"]
     ) -> DescribeHsmClientCertificatesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_hsm_configurations"]
     ) -> DescribeHsmConfigurationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_node_configuration_options"]
     ) -> DescribeNodeConfigurationOptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_orderable_cluster_options"]
     ) -> DescribeOrderableClusterOptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_reserved_node_exchange_status"]
     ) -> DescribeReservedNodeExchangeStatusPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_reserved_node_offerings"]
     ) -> DescribeReservedNodeOfferingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_reserved_nodes"]
     ) -> DescribeReservedNodesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_scheduled_actions"]
     ) -> DescribeScheduledActionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_snapshot_copy_grants"]
     ) -> DescribeSnapshotCopyGrantsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_snapshot_schedules"]
     ) -> DescribeSnapshotSchedulesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_table_restore_status"]
     ) -> DescribeTableRestoreStatusPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["describe_tags"]) -> DescribeTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_usage_limits"]
     ) -> DescribeUsageLimitsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_reserved_node_exchange_configuration_options"]
     ) -> GetReservedNodeExchangeConfigurationOptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_reserved_node_exchange_offerings"]
     ) -> GetReservedNodeExchangeOfferingsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_paginator)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["cluster_available"]) -> ClusterAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["cluster_deleted"]) -> ClusterDeletedWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["cluster_restored"]) -> ClusterRestoredWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_waiter)
         """
+
     @overload
     def get_waiter(self, waiter_name: Literal["snapshot_available"]) -> SnapshotAvailableWaiter:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.get_waiter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/#get_waiter)
         """
+
     async def __aenter__(self) -> "RedshiftClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/client/)
         """
```

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/literals.py` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/literals.pyi` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/paginator.py` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,15 @@
         describe_table_restore_status_paginator: DescribeTableRestoreStatusPaginator = client.get_paginator("describe_table_restore_status")
         describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
         describe_usage_limits_paginator: DescribeUsageLimitsPaginator = client.get_paginator("describe_usage_limits")
         get_reserved_node_exchange_configuration_options_paginator: GetReservedNodeExchangeConfigurationOptionsPaginator = client.get_paginator("get_reserved_node_exchange_configuration_options")
         get_reserved_node_exchange_offerings_paginator: GetReservedNodeExchangeOfferingsPaginator = client.get_paginator("get_reserved_node_exchange_offerings")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import (
     ActionTypeType,
     DataShareStatusForConsumerType,
@@ -131,14 +130,15 @@
     ScheduledActionFilterTypeDef,
     ScheduledActionsMessageTypeDef,
     SnapshotCopyGrantMessageTypeDef,
     SnapshotMessageTypeDef,
     SnapshotSortingEntityTypeDef,
     TableRestoreStatusMessageTypeDef,
     TaggedResourceListMessageTypeDef,
+    TimestampTypeDef,
     TrackListMessageTypeDef,
     UsageLimitListTypeDef,
 )
 
 __all__ = (
     "DescribeClusterDbRevisionsPaginator",
     "DescribeClusterParameterGroupsPaginator",
@@ -189,15 +189,15 @@
 class DescribeClusterDbRevisionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterdbrevisionspaginator)
     """
 
     def paginate(
-        self, *, ClusterIdentifier: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClusterDbRevisionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterdbrevisionspaginator)
         """
 
 
@@ -209,15 +209,15 @@
 
     def paginate(
         self,
         *,
         ParameterGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterparametergroupspaginator)
         """
 
 
@@ -228,15 +228,15 @@
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterparameterspaginator)
         """
 
 
@@ -248,15 +248,15 @@
 
     def paginate(
         self,
         *,
         ClusterSecurityGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClusterSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSecurityGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustersecuritygroupspaginator)
         """
 
 
@@ -269,22 +269,22 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotType: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustersnapshotspaginator)
         """
 
 
@@ -296,30 +296,30 @@
 
     def paginate(
         self,
         *,
         ClusterSubnetGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClusterSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustersubnetgroupspaginator)
         """
 
 
 class DescribeClusterTracksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustertrackspaginator)
     """
 
     def paginate(
-        self, *, MaintenanceTrackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, MaintenanceTrackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[TrackListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustertrackspaginator)
         """
 
 
@@ -330,15 +330,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         ClusterParameterGroupFamily: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClusterVersionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterversionspaginator)
         """
 
 
@@ -350,15 +350,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterspaginator)
         """
 
 
@@ -369,30 +369,30 @@
     """
 
     def paginate(
         self,
         *,
         CustomDomainName: str = ...,
         CustomDomainCertificateArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CustomDomainAssociationsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeCustomDomainAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describecustomdomainassociationspaginator)
         """
 
 
 class DescribeDataSharesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedatasharespaginator)
     """
 
     def paginate(
-        self, *, DataShareArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DataShareArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDataSharesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedatasharespaginator)
         """
 
 
@@ -403,15 +403,15 @@
     """
 
     def paginate(
         self,
         *,
         ConsumerArn: str = ...,
         Status: DataShareStatusForConsumerType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDataSharesForConsumerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForConsumer.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedatasharesforconsumerpaginator)
         """
 
 
@@ -422,30 +422,30 @@
     """
 
     def paginate(
         self,
         *,
         ProducerArn: str = ...,
         Status: DataShareStatusForProducerType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDataSharesForProducerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForProducer.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedatasharesforproducerpaginator)
         """
 
 
 class DescribeDefaultClusterParametersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedefaultclusterparameterspaginator)
     """
 
     def paginate(
-        self, *, ParameterGroupFamily: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ParameterGroupFamily: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDefaultClusterParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedefaultclusterparameterspaginator)
         """
 
 
@@ -458,15 +458,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         EndpointName: str = ...,
         VpcId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EndpointAccessListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAccess.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeendpointaccesspaginator)
         """
 
 
@@ -478,15 +478,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         Grantee: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EndpointAuthorizationListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAuthorization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeendpointauthorizationpaginator)
         """
 
 
@@ -498,15 +498,15 @@
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -517,18 +517,18 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeeventspaginator)
         """
 
 
@@ -540,15 +540,15 @@
 
     def paginate(
         self,
         *,
         HsmClientCertificateIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[HsmClientCertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmClientCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describehsmclientcertificatespaginator)
         """
 
 
@@ -560,15 +560,15 @@
 
     def paginate(
         self,
         *,
         HsmConfigurationIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[HsmConfigurationMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describehsmconfigurationspaginator)
         """
 
 
@@ -583,15 +583,15 @@
         *,
         ActionType: ActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         OwnerAccount: str = ...,
         Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[NodeConfigurationOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeNodeConfigurationOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describenodeconfigurationoptionspaginator)
         """
 
 
@@ -602,15 +602,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         NodeType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[OrderableClusterOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeOrderableClusterOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeorderableclusteroptionspaginator)
         """
 
 
@@ -621,45 +621,45 @@
     """
 
     def paginate(
         self,
         *,
         ReservedNodeId: str = ...,
         ReservedNodeExchangeRequestId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReservedNodeExchangeStatusOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeExchangeStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describereservednodeexchangestatuspaginator)
         """
 
 
 class DescribeReservedNodeOfferingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describereservednodeofferingspaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeOfferingId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReservedNodeOfferingId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ReservedNodeOfferingsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describereservednodeofferingspaginator)
         """
 
 
 class DescribeReservedNodesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describereservednodespaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReservedNodeId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ReservedNodesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describereservednodespaginator)
         """
 
 
@@ -670,19 +670,19 @@
     """
 
     def paginate(
         self,
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ScheduledActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeScheduledActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describescheduledactionspaginator)
         """
 
 
@@ -694,15 +694,15 @@
 
     def paginate(
         self,
         *,
         SnapshotCopyGrantName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SnapshotCopyGrantMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotCopyGrants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describesnapshotcopygrantspaginator)
         """
 
 
@@ -715,15 +715,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ScheduleIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSnapshotSchedulesOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotSchedules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describesnapshotschedulespaginator)
         """
 
 
@@ -734,15 +734,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TableRestoreRequestId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[TableRestoreStatusMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTableRestoreStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describetablerestorestatuspaginator)
         """
 
 
@@ -755,15 +755,15 @@
     def paginate(
         self,
         *,
         ResourceName: str = ...,
         ResourceType: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[TaggedResourceListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describetagspaginator)
         """
 
 
@@ -777,15 +777,15 @@
         self,
         *,
         UsageLimitId: str = ...,
         ClusterIdentifier: str = ...,
         FeatureType: UsageLimitFeatureTypeType = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[UsageLimitListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeUsageLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeusagelimitspaginator)
         """
 
 
@@ -797,28 +797,28 @@
 
     def paginate(
         self,
         *,
         ActionType: ReservedNodeExchangeActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeConfigurationOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#getreservednodeexchangeconfigurationoptionspaginator)
         """
 
 
 class GetReservedNodeExchangeOfferingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#getreservednodeexchangeofferingspaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReservedNodeId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetReservedNodeExchangeOfferingsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#getreservednodeexchangeofferingspaginator)
         """
```

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/paginator.pyi` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,15 @@
         describe_table_restore_status_paginator: DescribeTableRestoreStatusPaginator = client.get_paginator("describe_table_restore_status")
         describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
         describe_usage_limits_paginator: DescribeUsageLimitsPaginator = client.get_paginator("describe_usage_limits")
         get_reserved_node_exchange_configuration_options_paginator: GetReservedNodeExchangeConfigurationOptionsPaginator = client.get_paginator("get_reserved_node_exchange_configuration_options")
         get_reserved_node_exchange_offerings_paginator: GetReservedNodeExchangeOfferingsPaginator = client.get_paginator("get_reserved_node_exchange_offerings")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import (
     ActionTypeType,
     DataShareStatusForConsumerType,
@@ -131,14 +130,15 @@
     ScheduledActionFilterTypeDef,
     ScheduledActionsMessageTypeDef,
     SnapshotCopyGrantMessageTypeDef,
     SnapshotMessageTypeDef,
     SnapshotSortingEntityTypeDef,
     TableRestoreStatusMessageTypeDef,
     TaggedResourceListMessageTypeDef,
+    TimestampTypeDef,
     TrackListMessageTypeDef,
     UsageLimitListTypeDef,
 )
 
 __all__ = (
     "DescribeClusterDbRevisionsPaginator",
     "DescribeClusterParameterGroupsPaginator",
@@ -186,15 +186,15 @@
 class DescribeClusterDbRevisionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterdbrevisionspaginator)
     """
 
     def paginate(
-        self, *, ClusterIdentifier: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterIdentifier: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClusterDbRevisionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterDbRevisions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterdbrevisionspaginator)
         """
 
 class DescribeClusterParameterGroupsPaginator(AioPaginator):
@@ -205,15 +205,15 @@
 
     def paginate(
         self,
         *,
         ParameterGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterparametergroupspaginator)
         """
 
 class DescribeClusterParametersPaginator(AioPaginator):
@@ -223,15 +223,15 @@
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterparameterspaginator)
         """
 
 class DescribeClusterSecurityGroupsPaginator(AioPaginator):
@@ -242,15 +242,15 @@
 
     def paginate(
         self,
         *,
         ClusterSecurityGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClusterSecurityGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSecurityGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustersecuritygroupspaginator)
         """
 
 class DescribeClusterSnapshotsPaginator(AioPaginator):
@@ -262,22 +262,22 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotType: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustersnapshotspaginator)
         """
 
 class DescribeClusterSubnetGroupsPaginator(AioPaginator):
@@ -288,29 +288,29 @@
 
     def paginate(
         self,
         *,
         ClusterSubnetGroupName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClusterSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustersubnetgroupspaginator)
         """
 
 class DescribeClusterTracksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustertrackspaginator)
     """
 
     def paginate(
-        self, *, MaintenanceTrackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, MaintenanceTrackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[TrackListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterTracks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclustertrackspaginator)
         """
 
 class DescribeClusterVersionsPaginator(AioPaginator):
@@ -320,15 +320,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         ClusterParameterGroupFamily: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClusterVersionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusterVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterversionspaginator)
         """
 
 class DescribeClustersPaginator(AioPaginator):
@@ -339,15 +339,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeclusterspaginator)
         """
 
 class DescribeCustomDomainAssociationsPaginator(AioPaginator):
@@ -357,29 +357,29 @@
     """
 
     def paginate(
         self,
         *,
         CustomDomainName: str = ...,
         CustomDomainCertificateArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[CustomDomainAssociationsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeCustomDomainAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describecustomdomainassociationspaginator)
         """
 
 class DescribeDataSharesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedatasharespaginator)
     """
 
     def paginate(
-        self, *, DataShareArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DataShareArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDataSharesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataShares.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedatasharespaginator)
         """
 
 class DescribeDataSharesForConsumerPaginator(AioPaginator):
@@ -389,15 +389,15 @@
     """
 
     def paginate(
         self,
         *,
         ConsumerArn: str = ...,
         Status: DataShareStatusForConsumerType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDataSharesForConsumerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForConsumer.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedatasharesforconsumerpaginator)
         """
 
 class DescribeDataSharesForProducerPaginator(AioPaginator):
@@ -407,29 +407,29 @@
     """
 
     def paginate(
         self,
         *,
         ProducerArn: str = ...,
         Status: DataShareStatusForProducerType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDataSharesForProducerResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDataSharesForProducer.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedatasharesforproducerpaginator)
         """
 
 class DescribeDefaultClusterParametersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedefaultclusterparameterspaginator)
     """
 
     def paginate(
-        self, *, ParameterGroupFamily: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ParameterGroupFamily: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDefaultClusterParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeDefaultClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describedefaultclusterparameterspaginator)
         """
 
 class DescribeEndpointAccessPaginator(AioPaginator):
@@ -441,15 +441,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         EndpointName: str = ...,
         VpcId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EndpointAccessListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAccess.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeendpointaccesspaginator)
         """
 
 class DescribeEndpointAuthorizationPaginator(AioPaginator):
@@ -460,15 +460,15 @@
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         Grantee: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EndpointAuthorizationListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEndpointAuthorization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeendpointauthorizationpaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(AioPaginator):
@@ -479,15 +479,15 @@
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -497,18 +497,18 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeeventspaginator)
         """
 
 class DescribeHsmClientCertificatesPaginator(AioPaginator):
@@ -519,15 +519,15 @@
 
     def paginate(
         self,
         *,
         HsmClientCertificateIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[HsmClientCertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmClientCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describehsmclientcertificatespaginator)
         """
 
 class DescribeHsmConfigurationsPaginator(AioPaginator):
@@ -538,15 +538,15 @@
 
     def paginate(
         self,
         *,
         HsmConfigurationIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[HsmConfigurationMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeHsmConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describehsmconfigurationspaginator)
         """
 
 class DescribeNodeConfigurationOptionsPaginator(AioPaginator):
@@ -560,15 +560,15 @@
         *,
         ActionType: ActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         OwnerAccount: str = ...,
         Filters: Sequence[NodeConfigurationOptionsFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[NodeConfigurationOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeNodeConfigurationOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describenodeconfigurationoptionspaginator)
         """
 
 class DescribeOrderableClusterOptionsPaginator(AioPaginator):
@@ -578,15 +578,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterVersion: str = ...,
         NodeType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[OrderableClusterOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeOrderableClusterOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeorderableclusteroptionspaginator)
         """
 
 class DescribeReservedNodeExchangeStatusPaginator(AioPaginator):
@@ -596,43 +596,43 @@
     """
 
     def paginate(
         self,
         *,
         ReservedNodeId: str = ...,
         ReservedNodeExchangeRequestId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReservedNodeExchangeStatusOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeExchangeStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describereservednodeexchangestatuspaginator)
         """
 
 class DescribeReservedNodeOfferingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describereservednodeofferingspaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeOfferingId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReservedNodeOfferingId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ReservedNodeOfferingsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodeOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describereservednodeofferingspaginator)
         """
 
 class DescribeReservedNodesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describereservednodespaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReservedNodeId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ReservedNodesMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeReservedNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describereservednodespaginator)
         """
 
 class DescribeScheduledActionsPaginator(AioPaginator):
@@ -642,19 +642,19 @@
     """
 
     def paginate(
         self,
         *,
         ScheduledActionName: str = ...,
         TargetActionType: ScheduledActionTypeValuesType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Active: bool = ...,
         Filters: Sequence[ScheduledActionFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ScheduledActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeScheduledActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describescheduledactionspaginator)
         """
 
 class DescribeSnapshotCopyGrantsPaginator(AioPaginator):
@@ -665,15 +665,15 @@
 
     def paginate(
         self,
         *,
         SnapshotCopyGrantName: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SnapshotCopyGrantMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotCopyGrants.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describesnapshotcopygrantspaginator)
         """
 
 class DescribeSnapshotSchedulesPaginator(AioPaginator):
@@ -685,15 +685,15 @@
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         ScheduleIdentifier: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSnapshotSchedulesOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeSnapshotSchedules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describesnapshotschedulespaginator)
         """
 
 class DescribeTableRestoreStatusPaginator(AioPaginator):
@@ -703,15 +703,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterIdentifier: str = ...,
         TableRestoreRequestId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[TableRestoreStatusMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTableRestoreStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describetablerestorestatuspaginator)
         """
 
 class DescribeTagsPaginator(AioPaginator):
@@ -723,15 +723,15 @@
     def paginate(
         self,
         *,
         ResourceName: str = ...,
         ResourceType: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[TaggedResourceListMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describetagspaginator)
         """
 
 class DescribeUsageLimitsPaginator(AioPaginator):
@@ -744,15 +744,15 @@
         self,
         *,
         UsageLimitId: str = ...,
         ClusterIdentifier: str = ...,
         FeatureType: UsageLimitFeatureTypeType = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[UsageLimitListTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.DescribeUsageLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#describeusagelimitspaginator)
         """
 
 class GetReservedNodeExchangeConfigurationOptionsPaginator(AioPaginator):
@@ -763,27 +763,27 @@
 
     def paginate(
         self,
         *,
         ActionType: ReservedNodeExchangeActionTypeType,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeConfigurationOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#getreservednodeexchangeconfigurationoptionspaginator)
         """
 
 class GetReservedNodeExchangeOfferingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#getreservednodeexchangeofferingspaginator)
     """
 
     def paginate(
-        self, *, ReservedNodeId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ReservedNodeId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetReservedNodeExchangeOfferingsOutputMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Paginator.GetReservedNodeExchangeOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/paginators/#getreservednodeexchangeofferingspaginator)
         """
```

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/type_defs.py` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_redshift.type_defs import AcceptReservedNodeExchangeInputMessageRequestTypeDef
 
-    data: AcceptReservedNodeExchangeInputMessageRequestTypeDef = {...}
+    data: AcceptReservedNodeExchangeInputMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -47,17 +47,17 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AttributeValueTargetTypeDef",
     "AccountWithRestoreAccessTypeDef",
     "AquaConfigurationTypeDef",
     "AssociateDataShareConsumerMessageRequestTypeDef",
     "CertificateAssociationTypeDef",
     "AuthenticationProfileTypeDef",
     "AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef",
@@ -66,21 +66,18 @@
     "AuthorizeSnapshotAccessMessageRequestTypeDef",
     "SupportedPlatformTypeDef",
     "DeleteClusterSnapshotMessageTypeDef",
     "SnapshotErrorMessageTypeDef",
     "BatchModifyClusterSnapshotsMessageRequestTypeDef",
     "CancelResizeMessageRequestTypeDef",
     "ClusterAssociatedToScheduleTypeDef",
-    "ClusterCredentialsTypeDef",
     "RevisionTargetTypeDef",
-    "ClusterExtendedCredentialsTypeDef",
     "ClusterIamRoleTypeDef",
     "ClusterNodeTypeDef",
     "ParameterTypeDef",
-    "ClusterParameterGroupNameMessageTypeDef",
     "ClusterParameterStatusTypeDef",
     "TagTypeDef",
     "ClusterSecurityGroupMembershipTypeDef",
     "ClusterSnapshotCopyStatusTypeDef",
     "DataTransferProgressTypeDef",
     "DeferredMaintenanceWindowTypeDef",
     "ElasticIpStatusTypeDef",
@@ -89,23 +86,20 @@
     "ReservedNodeExchangeStatusTypeDef",
     "ResizeInfoTypeDef",
     "RestoreStatusTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ClusterVersionTypeDef",
     "CopyClusterSnapshotMessageRequestTypeDef",
     "CreateAuthenticationProfileMessageRequestTypeDef",
-    "CreateAuthenticationProfileResultTypeDef",
     "CreateCustomDomainAssociationMessageRequestTypeDef",
-    "CreateCustomDomainAssociationResultTypeDef",
     "CreateEndpointAccessMessageRequestTypeDef",
-    "CustomerStorageMessageTypeDef",
+    "TimestampTypeDef",
     "DataShareAssociationTypeDef",
     "DeauthorizeDataShareMessageRequestTypeDef",
     "DeleteAuthenticationProfileMessageRequestTypeDef",
-    "DeleteAuthenticationProfileResultTypeDef",
     "DeleteClusterMessageRequestTypeDef",
     "DeleteClusterParameterGroupMessageRequestTypeDef",
     "DeleteClusterSecurityGroupMessageRequestTypeDef",
     "DeleteClusterSnapshotMessageRequestTypeDef",
     "DeleteClusterSubnetGroupMessageRequestTypeDef",
     "DeleteCustomDomainAssociationMessageRequestTypeDef",
     "DeleteEndpointAccessMessageRequestTypeDef",
@@ -115,139 +109,113 @@
     "DeleteScheduledActionMessageRequestTypeDef",
     "DeleteSnapshotCopyGrantMessageRequestTypeDef",
     "DeleteSnapshotScheduleMessageRequestTypeDef",
     "DeleteTagsMessageRequestTypeDef",
     "DeleteUsageLimitMessageRequestTypeDef",
     "DescribeAccountAttributesMessageRequestTypeDef",
     "DescribeAuthenticationProfilesMessageRequestTypeDef",
-    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClusterDbRevisionsMessageRequestTypeDef",
-    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
     "DescribeClusterParameterGroupsMessageRequestTypeDef",
-    "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
     "DescribeClusterParametersMessageRequestTypeDef",
-    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
     "DescribeClusterSecurityGroupsMessageRequestTypeDef",
     "SnapshotSortingEntityTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
     "DescribeClusterSubnetGroupsMessageRequestTypeDef",
-    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
     "DescribeClusterTracksMessageRequestTypeDef",
-    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
     "DescribeClusterVersionsMessageRequestTypeDef",
-    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
     "DescribeClustersMessageRequestTypeDef",
-    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
     "DescribeCustomDomainAssociationsMessageRequestTypeDef",
-    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
     "DescribeDataSharesForConsumerMessageRequestTypeDef",
-    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
     "DescribeDataSharesForProducerMessageRequestTypeDef",
-    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
     "DescribeDataSharesMessageRequestTypeDef",
-    "DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
     "DescribeDefaultClusterParametersMessageRequestTypeDef",
-    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
     "DescribeEndpointAccessMessageRequestTypeDef",
-    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
-    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
-    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     "DescribeLoggingStatusMessageRequestTypeDef",
     "NodeConfigurationOptionsFilterTypeDef",
-    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     "DescribePartnersInputMessageRequestTypeDef",
     "PartnerIntegrationInfoTypeDef",
-    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
     "DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef",
-    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
     "DescribeReservedNodeOfferingsMessageRequestTypeDef",
-    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
     "DescribeReservedNodesMessageRequestTypeDef",
     "DescribeResizeMessageRequestTypeDef",
     "ScheduledActionFilterTypeDef",
-    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
     "DescribeSnapshotCopyGrantsMessageRequestTypeDef",
-    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
     "DescribeSnapshotSchedulesMessageRequestTypeDef",
-    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
     "DescribeTableRestoreStatusMessageRequestTypeDef",
-    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
     "DescribeTagsMessageRequestTypeDef",
-    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
     "DescribeUsageLimitsMessageRequestTypeDef",
     "DisableLoggingMessageRequestTypeDef",
     "DisableSnapshotCopyMessageRequestTypeDef",
     "DisassociateDataShareConsumerMessageRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableLoggingMessageRequestTypeDef",
     "EnableSnapshotCopyMessageRequestTypeDef",
     "EndpointAuthorizationTypeDef",
-    "EndpointAuthorizationResponseMetadataTypeDef",
     "EventInfoMapTypeDef",
     "EventTypeDef",
     "GetClusterCredentialsMessageRequestTypeDef",
     "GetClusterCredentialsWithIAMMessageRequestTypeDef",
-    "GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
     "GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
-    "GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     "GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
-    "LoggingStatusTypeDef",
     "ModifyAquaInputMessageRequestTypeDef",
     "ModifyAuthenticationProfileMessageRequestTypeDef",
-    "ModifyAuthenticationProfileResultTypeDef",
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     "ModifyClusterIamRolesMessageRequestTypeDef",
-    "ModifyClusterMaintenanceMessageRequestTypeDef",
     "ModifyClusterMessageRequestTypeDef",
     "ModifyClusterSnapshotMessageRequestTypeDef",
     "ModifyClusterSnapshotScheduleMessageRequestTypeDef",
     "ModifyClusterSubnetGroupMessageRequestTypeDef",
     "ModifyCustomDomainAssociationMessageRequestTypeDef",
-    "ModifyCustomDomainAssociationResultTypeDef",
     "ModifyEndpointAccessMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     "ModifySnapshotScheduleMessageRequestTypeDef",
     "ModifyUsageLimitMessageRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "NodeConfigurationOptionTypeDef",
-    "PaginatorConfigTypeDef",
     "PartnerIntegrationInputMessageRequestTypeDef",
-    "PartnerIntegrationOutputMessageTypeDef",
     "PauseClusterMessageRequestTypeDef",
     "PauseClusterMessageTypeDef",
     "PurchaseReservedNodeOfferingMessageRequestTypeDef",
     "RebootClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RejectDataShareMessageRequestTypeDef",
     "ResizeClusterMessageRequestTypeDef",
     "ResizeClusterMessageTypeDef",
-    "ResizeProgressMessageTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreFromClusterSnapshotMessageRequestTypeDef",
     "RestoreTableFromClusterSnapshotMessageRequestTypeDef",
     "TableRestoreStatusTypeDef",
     "ResumeClusterMessageRequestTypeDef",
     "ResumeClusterMessageTypeDef",
     "RevokeClusterSecurityGroupIngressMessageRequestTypeDef",
     "RevokeEndpointAccessMessageRequestTypeDef",
     "RevokeSnapshotAccessMessageRequestTypeDef",
     "RotateEncryptionKeyMessageRequestTypeDef",
     "SupportedOperationTypeDef",
     "UpdatePartnerStatusInputMessageRequestTypeDef",
+    "ClusterCredentialsTypeDef",
+    "ClusterExtendedCredentialsTypeDef",
+    "ClusterParameterGroupNameMessageTypeDef",
+    "CreateAuthenticationProfileResultTypeDef",
+    "CreateCustomDomainAssociationResultTypeDef",
+    "CustomerStorageMessageTypeDef",
+    "DeleteAuthenticationProfileResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EndpointAuthorizationResponseTypeDef",
+    "LoggingStatusTypeDef",
+    "ModifyAuthenticationProfileResultTypeDef",
+    "ModifyCustomDomainAssociationResultTypeDef",
+    "PartnerIntegrationOutputMessageTypeDef",
+    "ResizeProgressMessageTypeDef",
     "AccountAttributeTypeDef",
     "ModifyAquaOutputMessageTypeDef",
     "AssociationTypeDef",
     "DescribeAuthenticationProfilesResultTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchDeleteClusterSnapshotsRequestRequestTypeDef",
     "BatchDeleteClusterSnapshotsResultTypeDef",
@@ -273,24 +241,56 @@
     "CreateUsageLimitMessageRequestTypeDef",
     "EC2SecurityGroupTypeDef",
     "EventSubscriptionTypeDef",
     "HsmClientCertificateTypeDef",
     "HsmConfigurationTypeDef",
     "IPRangeTypeDef",
     "SnapshotCopyGrantTypeDef",
-    "SnapshotScheduleResponseMetadataTypeDef",
+    "SnapshotScheduleResponseTypeDef",
     "SnapshotScheduleTypeDef",
     "SnapshotTypeDef",
     "TaggedResourceTypeDef",
-    "UsageLimitResponseMetadataTypeDef",
+    "UsageLimitResponseTypeDef",
     "UsageLimitTypeDef",
     "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
     "ClusterVersionsMessageTypeDef",
-    "DataShareResponseMetadataTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
+    "ModifyClusterMaintenanceMessageRequestTypeDef",
+    "DataShareResponseTypeDef",
     "DataShareTypeDef",
+    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
+    "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
+    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
+    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
+    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
+    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
+    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
+    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
+    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
+    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
+    "DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
+    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
+    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
+    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
+    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
+    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
+    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
+    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
+    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
+    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
+    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
+    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
+    "GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
+    "GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     "DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef",
     "DescribeClustersMessageClusterAvailableWaitTypeDef",
     "DescribeClustersMessageClusterDeletedWaitTypeDef",
     "DescribeClustersMessageClusterRestoredWaitTypeDef",
     "DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef",
@@ -337,26 +337,26 @@
     "SnapshotMessageTypeDef",
     "TaggedResourceListMessageTypeDef",
     "UsageLimitListTypeDef",
     "DescribeDataSharesForConsumerResultTypeDef",
     "DescribeDataSharesForProducerResultTypeDef",
     "DescribeDataSharesResultTypeDef",
     "EventCategoriesMessageTypeDef",
-    "EndpointAccessResponseMetadataTypeDef",
+    "EndpointAccessResponseTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "GetReservedNodeExchangeOfferingsOutputMessageTypeDef",
     "ReservedNodeOfferingsMessageTypeDef",
     "AcceptReservedNodeExchangeOutputMessageTypeDef",
     "PurchaseReservedNodeOfferingResultTypeDef",
     "ReservedNodeConfigurationOptionTypeDef",
     "ReservedNodesMessageTypeDef",
     "CreateScheduledActionMessageRequestTypeDef",
     "ModifyScheduledActionMessageRequestTypeDef",
-    "ScheduledActionResponseMetadataTypeDef",
+    "ScheduledActionResponseTypeDef",
     "ScheduledActionTypeDef",
     "MaintenanceTrackTypeDef",
     "OrderableClusterOptionsMessageTypeDef",
     "ClusterSubnetGroupTypeDef",
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     "ClusterSecurityGroupMessageTypeDef",
     "CreateClusterSecurityGroupResultTypeDef",
@@ -391,14 +391,25 @@
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
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
 AttributeValueTargetTypeDef = TypedDict(
     "AttributeValueTargetTypeDef",
     {
         "AttributeValue": str,
     },
     total=False,
 )
@@ -433,22 +444,20 @@
         "AssociateEntireAccount": bool,
         "ConsumerArn": str,
         "ConsumerRegion": str,
     },
     total=False,
 )
 
-
 class AssociateDataShareConsumerMessageRequestTypeDef(
     _RequiredAssociateDataShareConsumerMessageRequestTypeDef,
     _OptionalAssociateDataShareConsumerMessageRequestTypeDef,
 ):
     pass
 
-
 CertificateAssociationTypeDef = TypedDict(
     "CertificateAssociationTypeDef",
     {
         "CustomDomainName": str,
         "ClusterIdentifier": str,
     },
     total=False,
@@ -475,22 +484,20 @@
         "CIDRIP": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
-
 class AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef(
     _RequiredAuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
     _OptionalAuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
-
 AuthorizeDataShareMessageRequestTypeDef = TypedDict(
     "AuthorizeDataShareMessageRequestTypeDef",
     {
         "DataShareArn": str,
         "ConsumerIdentifier": str,
     },
 )
@@ -506,22 +513,20 @@
     {
         "ClusterIdentifier": str,
         "VpcIds": Sequence[str],
     },
     total=False,
 )
 
-
 class AuthorizeEndpointAccessMessageRequestTypeDef(
     _RequiredAuthorizeEndpointAccessMessageRequestTypeDef,
     _OptionalAuthorizeEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredAuthorizeSnapshotAccessMessageRequestTypeDef = TypedDict(
     "_RequiredAuthorizeSnapshotAccessMessageRequestTypeDef",
     {
         "AccountWithRestoreAccess": str,
     },
 )
 _OptionalAuthorizeSnapshotAccessMessageRequestTypeDef = TypedDict(
@@ -530,22 +535,20 @@
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
-
 class AuthorizeSnapshotAccessMessageRequestTypeDef(
     _RequiredAuthorizeSnapshotAccessMessageRequestTypeDef,
     _OptionalAuthorizeSnapshotAccessMessageRequestTypeDef,
 ):
     pass
 
-
 SupportedPlatformTypeDef = TypedDict(
     "SupportedPlatformTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -560,21 +563,19 @@
     "_OptionalDeleteClusterSnapshotMessageTypeDef",
     {
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
-
 class DeleteClusterSnapshotMessageTypeDef(
     _RequiredDeleteClusterSnapshotMessageTypeDef, _OptionalDeleteClusterSnapshotMessageTypeDef
 ):
     pass
 
-
 SnapshotErrorMessageTypeDef = TypedDict(
     "SnapshotErrorMessageTypeDef",
     {
         "SnapshotIdentifier": str,
         "SnapshotClusterIdentifier": str,
         "FailureCode": str,
         "FailureReason": str,
@@ -593,22 +594,20 @@
     {
         "ManualSnapshotRetentionPeriod": int,
         "Force": bool,
     },
     total=False,
 )
 
-
 class BatchModifyClusterSnapshotsMessageRequestTypeDef(
     _RequiredBatchModifyClusterSnapshotsMessageRequestTypeDef,
     _OptionalBatchModifyClusterSnapshotsMessageRequestTypeDef,
 ):
     pass
 
-
 CancelResizeMessageRequestTypeDef = TypedDict(
     "CancelResizeMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -617,45 +616,24 @@
     {
         "ClusterIdentifier": str,
         "ScheduleAssociationState": ScheduleStateType,
     },
     total=False,
 )
 
-ClusterCredentialsTypeDef = TypedDict(
-    "ClusterCredentialsTypeDef",
-    {
-        "DbUser": str,
-        "DbPassword": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RevisionTargetTypeDef = TypedDict(
     "RevisionTargetTypeDef",
     {
         "DatabaseRevision": str,
         "Description": str,
         "DatabaseRevisionReleaseDate": datetime,
     },
     total=False,
 )
 
-ClusterExtendedCredentialsTypeDef = TypedDict(
-    "ClusterExtendedCredentialsTypeDef",
-    {
-        "DbUser": str,
-        "DbPassword": str,
-        "Expiration": datetime,
-        "NextRefreshTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ClusterIamRoleTypeDef = TypedDict(
     "ClusterIamRoleTypeDef",
     {
         "IamRoleArn": str,
         "ApplyStatus": str,
     },
     total=False,
@@ -683,23 +661,14 @@
         "ApplyType": ParameterApplyTypeType,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
     },
     total=False,
 )
 
-ClusterParameterGroupNameMessageTypeDef = TypedDict(
-    "ClusterParameterGroupNameMessageTypeDef",
-    {
-        "ParameterGroupName": str,
-        "ParameterGroupStatus": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ClusterParameterStatusTypeDef = TypedDict(
     "ClusterParameterStatusTypeDef",
     {
         "ParameterName": str,
         "ParameterApplyStatus": str,
         "ParameterApplyErrorDescription": str,
     },
@@ -864,59 +833,37 @@
     {
         "SourceSnapshotClusterIdentifier": str,
         "ManualSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
-
 class CopyClusterSnapshotMessageRequestTypeDef(
     _RequiredCopyClusterSnapshotMessageRequestTypeDef,
     _OptionalCopyClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 CreateAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "CreateAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
-CreateAuthenticationProfileResultTypeDef = TypedDict(
-    "CreateAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "AuthenticationProfileContent": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateCustomDomainAssociationMessageRequestTypeDef = TypedDict(
     "CreateCustomDomainAssociationMessageRequestTypeDef",
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
         "ClusterIdentifier": str,
     },
 )
 
-CreateCustomDomainAssociationResultTypeDef = TypedDict(
-    "CreateCustomDomainAssociationResultTypeDef",
-    {
-        "CustomDomainName": str,
-        "CustomDomainCertificateArn": str,
-        "ClusterIdentifier": str,
-        "CustomDomainCertExpiryTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateEndpointAccessMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
         "SubnetGroupName": str,
     },
 )
@@ -926,31 +873,21 @@
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateEndpointAccessMessageRequestTypeDef(
     _RequiredCreateEndpointAccessMessageRequestTypeDef,
     _OptionalCreateEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
-
-CustomerStorageMessageTypeDef = TypedDict(
-    "CustomerStorageMessageTypeDef",
-    {
-        "TotalBackupSizeInMegaBytes": float,
-        "TotalProvisionedStorageInMegaBytes": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 DataShareAssociationTypeDef = TypedDict(
     "DataShareAssociationTypeDef",
     {
         "ConsumerIdentifier": str,
         "Status": DataShareStatusType,
         "ConsumerRegion": str,
         "CreatedDate": datetime,
@@ -970,22 +907,14 @@
 DeleteAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "DeleteAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
     },
 )
 
-DeleteAuthenticationProfileResultTypeDef = TypedDict(
-    "DeleteAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalDeleteClusterMessageRequestTypeDef = TypedDict(
@@ -994,21 +923,19 @@
         "SkipFinalClusterSnapshot": bool,
         "FinalClusterSnapshotIdentifier": str,
         "FinalClusterSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
-
 class DeleteClusterMessageRequestTypeDef(
     _RequiredDeleteClusterMessageRequestTypeDef, _OptionalDeleteClusterMessageRequestTypeDef
 ):
     pass
 
-
 DeleteClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteClusterParameterGroupMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 
@@ -1029,22 +956,20 @@
     "_OptionalDeleteClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
-
 class DeleteClusterSnapshotMessageRequestTypeDef(
     _RequiredDeleteClusterSnapshotMessageRequestTypeDef,
     _OptionalDeleteClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 DeleteClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "DeleteClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
     },
 )
 
@@ -1131,79 +1056,46 @@
     "DescribeAuthenticationProfilesMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
     },
     total=False,
 )
 
-DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = TypedDict(
-    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ClusterIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeClusterDbRevisionsMessageRequestTypeDef = TypedDict(
     "DescribeClusterDbRevisionsMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterParameterGroupsMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef(
-    _RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-    _OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeClusterParametersMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1212,33 +1104,20 @@
         "Source": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeClusterParametersMessageRequestTypeDef(
     _RequiredDescribeClusterParametersMessageRequestTypeDef,
     _OptionalDescribeClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-
-DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
-    {
-        "ClusterSecurityGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSecurityGroupsMessageRequestTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
@@ -1257,220 +1136,116 @@
     "_OptionalSnapshotSortingEntityTypeDef",
     {
         "SortOrder": SortByOrderType,
     },
     total=False,
 )
 
-
 class SnapshotSortingEntityTypeDef(
     _RequiredSnapshotSortingEntityTypeDef, _OptionalSnapshotSortingEntityTypeDef
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
-    {
-        "ClusterSubnetGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSubnetGroupsMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = TypedDict(
-    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
-    {
-        "MaintenanceTrackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterTracksMessageRequestTypeDef = TypedDict(
     "DescribeClusterTracksMessageRequestTypeDef",
     {
         "MaintenanceTrackName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = TypedDict(
-    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
-    {
-        "ClusterVersion": str,
-        "ClusterParameterGroupFamily": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterVersionsMessageRequestTypeDef = TypedDict(
     "DescribeClusterVersionsMessageRequestTypeDef",
     {
         "ClusterVersion": str,
         "ClusterParameterGroupFamily": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeClustersMessageDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClustersMessageRequestTypeDef = TypedDict(
     "DescribeClustersMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef = TypedDict(
-    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
-    {
-        "CustomDomainName": str,
-        "CustomDomainCertificateArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCustomDomainAssociationsMessageRequestTypeDef = TypedDict(
     "DescribeCustomDomainAssociationsMessageRequestTypeDef",
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = TypedDict(
-    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
-    {
-        "ConsumerArn": str,
-        "Status": DataShareStatusForConsumerType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSharesForConsumerMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesForConsumerMessageRequestTypeDef",
     {
         "ConsumerArn": str,
         "Status": DataShareStatusForConsumerType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = TypedDict(
-    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
-    {
-        "ProducerArn": str,
-        "Status": DataShareStatusForProducerType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSharesForProducerMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesForProducerMessageRequestTypeDef",
     {
         "ProducerArn": str,
         "Status": DataShareStatusForProducerType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = TypedDict(
-    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
-    {
-        "DataShareArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSharesMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesMessageRequestTypeDef",
     {
         "DataShareArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    {
-        "ParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef(
-    _RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-    _OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeDefaultClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDefaultClusterParametersMessageRequestTypeDef",
     {
         "ParameterGroupFamily": str,
     },
 )
 _OptionalDescribeDefaultClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1478,58 +1253,33 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-
-DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = TypedDict(
-    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ResourceOwner": str,
-        "EndpointName": str,
-        "VpcId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEndpointAccessMessageRequestTypeDef = TypedDict(
     "DescribeEndpointAccessMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "EndpointName": str,
         "VpcId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = TypedDict(
-    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "Account": str,
-        "Grantee": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEndpointAuthorizationMessageRequestTypeDef = TypedDict(
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "Account": str,
         "Grantee": bool,
         "MaxRecords": int,
@@ -1542,98 +1292,38 @@
     "DescribeEventCategoriesMessageRequestTypeDef",
     {
         "SourceType": str,
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
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
-DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
-    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
-    {
-        "HsmClientCertificateIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeHsmClientCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
-    {
-        "HsmConfigurationIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeHsmConfigurationsMessageRequestTypeDef = TypedDict(
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     {
         "HsmConfigurationIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
@@ -1655,24 +1345,14 @@
         "Name": NodeConfigurationOptionsFilterNameType,
         "Operator": OperatorTypeType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = TypedDict(
-    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
-    {
-        "ClusterVersion": str,
-        "NodeType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrderableClusterOptionsMessageRequestTypeDef = TypedDict(
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     {
         "ClusterVersion": str,
         "NodeType": str,
         "MaxRecords": int,
         "Marker": str,
@@ -1692,84 +1372,54 @@
     {
         "DatabaseName": str,
         "PartnerName": str,
     },
     total=False,
 )
 
-
 class DescribePartnersInputMessageRequestTypeDef(
     _RequiredDescribePartnersInputMessageRequestTypeDef,
     _OptionalDescribePartnersInputMessageRequestTypeDef,
 ):
     pass
 
-
 PartnerIntegrationInfoTypeDef = TypedDict(
     "PartnerIntegrationInfoTypeDef",
     {
         "DatabaseName": str,
         "PartnerName": str,
         "Status": PartnerIntegrationStatusType,
         "StatusMessage": str,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
-DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = TypedDict(
-    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-        "ReservedNodeExchangeRequestId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "ReservedNodeExchangeRequestId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
-    {
-        "ReservedNodeOfferingId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedNodeOfferingsMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodeOfferingsMessageRequestTypeDef",
     {
         "ReservedNodeOfferingId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedNodesMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodesMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1787,121 +1437,63 @@
     "ScheduledActionFilterTypeDef",
     {
         "Name": ScheduledActionFilterNameType,
         "Values": Sequence[str],
     },
 )
 
-DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
-    {
-        "SnapshotCopyGrantName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotCopyGrantsMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotCopyGrantsMessageRequestTypeDef",
     {
         "SnapshotCopyGrantName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = TypedDict(
-    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ScheduleIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotSchedulesMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotSchedulesMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ScheduleIdentifier": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = TypedDict(
-    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "TableRestoreRequestId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTableRestoreStatusMessageRequestTypeDef = TypedDict(
     "DescribeTableRestoreStatusMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "TableRestoreRequestId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeTagsMessageDescribeTagsPaginateTypeDef = TypedDict(
-    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
-    {
-        "ResourceName": str,
-        "ResourceType": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTagsMessageRequestTypeDef = TypedDict(
     "DescribeTagsMessageRequestTypeDef",
     {
         "ResourceName": str,
         "ResourceType": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = TypedDict(
-    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
-    {
-        "UsageLimitId": str,
-        "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUsageLimitsMessageRequestTypeDef = TypedDict(
     "DescribeUsageLimitsMessageRequestTypeDef",
     {
         "UsageLimitId": str,
         "ClusterIdentifier": str,
         "FeatureType": UsageLimitFeatureTypeType,
         "MaxRecords": int,
@@ -1938,29 +1530,20 @@
         "DisassociateEntireAccount": bool,
         "ConsumerArn": str,
         "ConsumerRegion": str,
     },
     total=False,
 )
 
-
 class DisassociateDataShareConsumerMessageRequestTypeDef(
     _RequiredDisassociateDataShareConsumerMessageRequestTypeDef,
     _OptionalDisassociateDataShareConsumerMessageRequestTypeDef,
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
 _RequiredEnableLoggingMessageRequestTypeDef = TypedDict(
     "_RequiredEnableLoggingMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalEnableLoggingMessageRequestTypeDef = TypedDict(
@@ -1970,21 +1553,19 @@
         "S3KeyPrefix": str,
         "LogDestinationType": LogDestinationTypeType,
         "LogExports": Sequence[str],
     },
     total=False,
 )
 
-
 class EnableLoggingMessageRequestTypeDef(
     _RequiredEnableLoggingMessageRequestTypeDef, _OptionalEnableLoggingMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredEnableSnapshotCopyMessageRequestTypeDef = TypedDict(
     "_RequiredEnableSnapshotCopyMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "DestinationRegion": str,
     },
 )
@@ -1994,22 +1575,20 @@
         "RetentionPeriod": int,
         "SnapshotCopyGrantName": str,
         "ManualSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
-
 class EnableSnapshotCopyMessageRequestTypeDef(
     _RequiredEnableSnapshotCopyMessageRequestTypeDef,
     _OptionalEnableSnapshotCopyMessageRequestTypeDef,
 ):
     pass
 
-
 EndpointAuthorizationTypeDef = TypedDict(
     "EndpointAuthorizationTypeDef",
     {
         "Grantor": str,
         "Grantee": str,
         "ClusterIdentifier": str,
         "AuthorizeTime": datetime,
@@ -2018,30 +1597,14 @@
         "AllowedAllVPCs": bool,
         "AllowedVPCs": List[str],
         "EndpointCount": int,
     },
     total=False,
 )
 
-EndpointAuthorizationResponseMetadataTypeDef = TypedDict(
-    "EndpointAuthorizationResponseMetadataTypeDef",
-    {
-        "Grantor": str,
-        "Grantee": str,
-        "ClusterIdentifier": str,
-        "AuthorizeTime": datetime,
-        "ClusterStatus": str,
-        "Status": AuthorizationStatusType,
-        "AllowedAllVPCs": bool,
-        "AllowedVPCs": List[str],
-        "EndpointCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventInfoMapTypeDef = TypedDict(
     "EventInfoMapTypeDef",
     {
         "EventId": str,
         "EventCategories": List[str],
         "EventDescription": str,
         "Severity": str,
@@ -2078,57 +1641,31 @@
         "AutoCreate": bool,
         "DbGroups": Sequence[str],
         "CustomDomainName": str,
     },
     total=False,
 )
 
-
 class GetClusterCredentialsMessageRequestTypeDef(
     _RequiredGetClusterCredentialsMessageRequestTypeDef,
     _OptionalGetClusterCredentialsMessageRequestTypeDef,
 ):
     pass
 
-
 GetClusterCredentialsWithIAMMessageRequestTypeDef = TypedDict(
     "GetClusterCredentialsWithIAMMessageRequestTypeDef",
     {
         "DbName": str,
         "ClusterIdentifier": str,
         "DurationSeconds": int,
         "CustomDomainName": str,
     },
     total=False,
 )
 
-_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
-    "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    {
-        "ActionType": ReservedNodeExchangeActionTypeType,
-    },
-)
-_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
-    "_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "SnapshotIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef(
-    _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-    _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef = TypedDict(
     "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
     {
         "ActionType": ReservedNodeExchangeActionTypeType,
     },
 )
 _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef = TypedDict(
@@ -2138,44 +1675,20 @@
         "SnapshotIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef(
     _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
     _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
 ):
     pass
 
-
-_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
-    "_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-    },
-)
-_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
-    "_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef(
-    _RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
-    _OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef = TypedDict(
     "_RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
     },
 )
 _OptionalGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef = TypedDict(
@@ -2183,75 +1696,47 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef(
     _RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
     _OptionalGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
 ):
     pass
 
-
-LoggingStatusTypeDef = TypedDict(
-    "LoggingStatusTypeDef",
-    {
-        "LoggingEnabled": bool,
-        "BucketName": str,
-        "S3KeyPrefix": str,
-        "LastSuccessfulDeliveryTime": datetime,
-        "LastFailureTime": datetime,
-        "LastFailureMessage": str,
-        "LogDestinationType": LogDestinationTypeType,
-        "LogExports": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredModifyAquaInputMessageRequestTypeDef = TypedDict(
     "_RequiredModifyAquaInputMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyAquaInputMessageRequestTypeDef = TypedDict(
     "_OptionalModifyAquaInputMessageRequestTypeDef",
     {
         "AquaConfigurationStatus": AquaConfigurationStatusType,
     },
     total=False,
 )
 
-
 class ModifyAquaInputMessageRequestTypeDef(
     _RequiredModifyAquaInputMessageRequestTypeDef, _OptionalModifyAquaInputMessageRequestTypeDef
 ):
     pass
 
-
 ModifyAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "ModifyAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
-ModifyAuthenticationProfileResultTypeDef = TypedDict(
-    "ModifyAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "AuthenticationProfileContent": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ModifyClusterDbRevisionMessageRequestTypeDef = TypedDict(
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "RevisionTarget": str,
     },
 )
@@ -2268,48 +1753,20 @@
         "AddIamRoles": Sequence[str],
         "RemoveIamRoles": Sequence[str],
         "DefaultIamRoleArn": str,
     },
     total=False,
 )
 
-
 class ModifyClusterIamRolesMessageRequestTypeDef(
     _RequiredModifyClusterIamRolesMessageRequestTypeDef,
     _OptionalModifyClusterIamRolesMessageRequestTypeDef,
 ):
     pass
 
-
-_RequiredModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
-    "_RequiredModifyClusterMaintenanceMessageRequestTypeDef",
-    {
-        "ClusterIdentifier": str,
-    },
-)
-_OptionalModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
-    "_OptionalModifyClusterMaintenanceMessageRequestTypeDef",
-    {
-        "DeferMaintenance": bool,
-        "DeferMaintenanceIdentifier": str,
-        "DeferMaintenanceStartTime": Union[datetime, str],
-        "DeferMaintenanceEndTime": Union[datetime, str],
-        "DeferMaintenanceDuration": int,
-    },
-    total=False,
-)
-
-
-class ModifyClusterMaintenanceMessageRequestTypeDef(
-    _RequiredModifyClusterMaintenanceMessageRequestTypeDef,
-    _OptionalModifyClusterMaintenanceMessageRequestTypeDef,
-):
-    pass
-
-
 _RequiredModifyClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyClusterMessageRequestTypeDef = TypedDict(
@@ -2339,21 +1796,19 @@
         "AvailabilityZoneRelocation": bool,
         "AvailabilityZone": str,
         "Port": int,
     },
     total=False,
 )
 
-
 class ModifyClusterMessageRequestTypeDef(
     _RequiredModifyClusterMessageRequestTypeDef, _OptionalModifyClusterMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredModifyClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotIdentifier": str,
     },
 )
 _OptionalModifyClusterSnapshotMessageRequestTypeDef = TypedDict(
@@ -2361,22 +1816,20 @@
     {
         "ManualSnapshotRetentionPeriod": int,
         "Force": bool,
     },
     total=False,
 )
 
-
 class ModifyClusterSnapshotMessageRequestTypeDef(
     _RequiredModifyClusterSnapshotMessageRequestTypeDef,
     _OptionalModifyClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyClusterSnapshotScheduleMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSnapshotScheduleMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyClusterSnapshotScheduleMessageRequestTypeDef = TypedDict(
@@ -2384,22 +1837,20 @@
     {
         "ScheduleIdentifier": str,
         "DisassociateSchedule": bool,
     },
     total=False,
 )
 
-
 class ModifyClusterSnapshotScheduleMessageRequestTypeDef(
     _RequiredModifyClusterSnapshotScheduleMessageRequestTypeDef,
     _OptionalModifyClusterSnapshotScheduleMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -2407,22 +1858,20 @@
     "_OptionalModifyClusterSubnetGroupMessageRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class ModifyClusterSubnetGroupMessageRequestTypeDef(
     _RequiredModifyClusterSubnetGroupMessageRequestTypeDef,
     _OptionalModifyClusterSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyCustomDomainAssociationMessageRequestTypeDef = TypedDict(
     "_RequiredModifyCustomDomainAssociationMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyCustomDomainAssociationMessageRequestTypeDef = TypedDict(
@@ -2430,55 +1879,40 @@
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
     },
     total=False,
 )
 
-
 class ModifyCustomDomainAssociationMessageRequestTypeDef(
     _RequiredModifyCustomDomainAssociationMessageRequestTypeDef,
     _OptionalModifyCustomDomainAssociationMessageRequestTypeDef,
 ):
     pass
 
-
-ModifyCustomDomainAssociationResultTypeDef = TypedDict(
-    "ModifyCustomDomainAssociationResultTypeDef",
-    {
-        "CustomDomainName": str,
-        "CustomDomainCertificateArn": str,
-        "ClusterIdentifier": str,
-        "CustomDomainCertExpiryTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredModifyEndpointAccessMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
 _OptionalModifyEndpointAccessMessageRequestTypeDef = TypedDict(
     "_OptionalModifyEndpointAccessMessageRequestTypeDef",
     {
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyEndpointAccessMessageRequestTypeDef(
     _RequiredModifyEndpointAccessMessageRequestTypeDef,
     _OptionalModifyEndpointAccessMessageRequestTypeDef,
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
@@ -2490,22 +1924,20 @@
         "EventCategories": Sequence[str],
         "Severity": str,
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
 _RequiredModifySnapshotCopyRetentionPeriodMessageRequestTypeDef = TypedDict(
     "_RequiredModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "RetentionPeriod": int,
     },
 )
@@ -2513,22 +1945,20 @@
     "_OptionalModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     {
         "Manual": bool,
     },
     total=False,
 )
 
-
 class ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef(
     _RequiredModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     _OptionalModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
 ):
     pass
 
-
 ModifySnapshotScheduleMessageRequestTypeDef = TypedDict(
     "ModifySnapshotScheduleMessageRequestTypeDef",
     {
         "ScheduleIdentifier": str,
         "ScheduleDefinitions": Sequence[str],
     },
 )
@@ -2544,21 +1974,19 @@
     {
         "Amount": int,
         "BreachAction": UsageLimitBreachActionType,
     },
     total=False,
 )
 
-
 class ModifyUsageLimitMessageRequestTypeDef(
     _RequiredModifyUsageLimitMessageRequestTypeDef, _OptionalModifyUsageLimitMessageRequestTypeDef
 ):
     pass
 
-
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "NetworkInterfaceId": str,
         "SubnetId": str,
         "PrivateIpAddress": str,
         "AvailabilityZone": str,
@@ -2573,43 +2001,24 @@
         "NumberOfNodes": int,
         "EstimatedDiskUtilizationPercent": float,
         "Mode": ModeType,
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
 PartnerIntegrationInputMessageRequestTypeDef = TypedDict(
     "PartnerIntegrationInputMessageRequestTypeDef",
     {
         "AccountId": str,
         "ClusterIdentifier": str,
         "DatabaseName": str,
         "PartnerName": str,
     },
 )
 
-PartnerIntegrationOutputMessageTypeDef = TypedDict(
-    "PartnerIntegrationOutputMessageTypeDef",
-    {
-        "DatabaseName": str,
-        "PartnerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PauseClusterMessageRequestTypeDef = TypedDict(
     "PauseClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2630,22 +2039,20 @@
     "_OptionalPurchaseReservedNodeOfferingMessageRequestTypeDef",
     {
         "NodeCount": int,
     },
     total=False,
 )
 
-
 class PurchaseReservedNodeOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedNodeOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedNodeOfferingMessageRequestTypeDef,
 ):
     pass
 
-
 RebootClusterMessageRequestTypeDef = TypedDict(
     "RebootClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2680,21 +2087,19 @@
         "Classic": bool,
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
     },
     total=False,
 )
 
-
 class ResizeClusterMessageRequestTypeDef(
     _RequiredResizeClusterMessageRequestTypeDef, _OptionalResizeClusterMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredResizeClusterMessageTypeDef = TypedDict(
     "_RequiredResizeClusterMessageTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalResizeClusterMessageTypeDef = TypedDict(
@@ -2706,55 +2111,19 @@
         "Classic": bool,
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
     },
     total=False,
 )
 
-
 class ResizeClusterMessageTypeDef(
     _RequiredResizeClusterMessageTypeDef, _OptionalResizeClusterMessageTypeDef
 ):
     pass
 
-
-ResizeProgressMessageTypeDef = TypedDict(
-    "ResizeProgressMessageTypeDef",
-    {
-        "TargetNodeType": str,
-        "TargetNumberOfNodes": int,
-        "TargetClusterType": str,
-        "Status": str,
-        "ImportTablesCompleted": List[str],
-        "ImportTablesInProgress": List[str],
-        "ImportTablesNotStarted": List[str],
-        "AvgResizeRateInMegaBytesPerSecond": float,
-        "TotalResizeDataInMegaBytes": int,
-        "ProgressInMegaBytes": int,
-        "ElapsedTimeInSeconds": int,
-        "EstimatedTimeToCompletionInSeconds": int,
-        "ResizeType": str,
-        "Message": str,
-        "TargetEncryptionType": str,
-        "DataTransferProgressPercent": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 _RequiredRestoreFromClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreFromClusterSnapshotMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalRestoreFromClusterSnapshotMessageRequestTypeDef = TypedDict(
@@ -2792,22 +2161,20 @@
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
         "Encrypted": bool,
     },
     total=False,
 )
 
-
 class RestoreFromClusterSnapshotMessageRequestTypeDef(
     _RequiredRestoreFromClusterSnapshotMessageRequestTypeDef,
     _OptionalRestoreFromClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredRestoreTableFromClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreTableFromClusterSnapshotMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SourceDatabaseName": str,
         "SourceTableName": str,
@@ -2821,22 +2188,20 @@
         "TargetDatabaseName": str,
         "TargetSchemaName": str,
         "EnableCaseSensitiveIdentifier": bool,
     },
     total=False,
 )
 
-
 class RestoreTableFromClusterSnapshotMessageRequestTypeDef(
     _RequiredRestoreTableFromClusterSnapshotMessageRequestTypeDef,
     _OptionalRestoreTableFromClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 TableRestoreStatusTypeDef = TypedDict(
     "TableRestoreStatusTypeDef",
     {
         "TableRestoreRequestId": str,
         "Status": TableRestoreStatusTypeType,
         "Message": str,
         "RequestTime": datetime,
@@ -2880,22 +2245,20 @@
         "CIDRIP": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
-
 class RevokeClusterSecurityGroupIngressMessageRequestTypeDef(
     _RequiredRevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     _OptionalRevokeClusterSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
-
 RevokeEndpointAccessMessageRequestTypeDef = TypedDict(
     "RevokeEndpointAccessMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "Account": str,
         "VpcIds": Sequence[str],
         "Force": bool,
@@ -2915,22 +2278,20 @@
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
-
 class RevokeSnapshotAccessMessageRequestTypeDef(
     _RequiredRevokeSnapshotAccessMessageRequestTypeDef,
     _OptionalRevokeSnapshotAccessMessageRequestTypeDef,
 ):
     pass
 
-
 RotateEncryptionKeyMessageRequestTypeDef = TypedDict(
     "RotateEncryptionKeyMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2956,36 +2317,191 @@
     "_OptionalUpdatePartnerStatusInputMessageRequestTypeDef",
     {
         "StatusMessage": str,
     },
     total=False,
 )
 
-
 class UpdatePartnerStatusInputMessageRequestTypeDef(
     _RequiredUpdatePartnerStatusInputMessageRequestTypeDef,
     _OptionalUpdatePartnerStatusInputMessageRequestTypeDef,
 ):
     pass
 
+ClusterCredentialsTypeDef = TypedDict(
+    "ClusterCredentialsTypeDef",
+    {
+        "DbUser": str,
+        "DbPassword": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterExtendedCredentialsTypeDef = TypedDict(
+    "ClusterExtendedCredentialsTypeDef",
+    {
+        "DbUser": str,
+        "DbPassword": str,
+        "Expiration": datetime,
+        "NextRefreshTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterParameterGroupNameMessageTypeDef = TypedDict(
+    "ClusterParameterGroupNameMessageTypeDef",
+    {
+        "ParameterGroupName": str,
+        "ParameterGroupStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthenticationProfileResultTypeDef = TypedDict(
+    "CreateAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "AuthenticationProfileContent": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomDomainAssociationResultTypeDef = TypedDict(
+    "CreateCustomDomainAssociationResultTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+        "CustomDomainCertExpiryTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CustomerStorageMessageTypeDef = TypedDict(
+    "CustomerStorageMessageTypeDef",
+    {
+        "TotalBackupSizeInMegaBytes": float,
+        "TotalProvisionedStorageInMegaBytes": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAuthenticationProfileResultTypeDef = TypedDict(
+    "DeleteAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
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
+EndpointAuthorizationResponseTypeDef = TypedDict(
+    "EndpointAuthorizationResponseTypeDef",
+    {
+        "Grantor": str,
+        "Grantee": str,
+        "ClusterIdentifier": str,
+        "AuthorizeTime": datetime,
+        "ClusterStatus": str,
+        "Status": AuthorizationStatusType,
+        "AllowedAllVPCs": bool,
+        "AllowedVPCs": List[str],
+        "EndpointCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoggingStatusTypeDef = TypedDict(
+    "LoggingStatusTypeDef",
+    {
+        "LoggingEnabled": bool,
+        "BucketName": str,
+        "S3KeyPrefix": str,
+        "LastSuccessfulDeliveryTime": datetime,
+        "LastFailureTime": datetime,
+        "LastFailureMessage": str,
+        "LogDestinationType": LogDestinationTypeType,
+        "LogExports": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyAuthenticationProfileResultTypeDef = TypedDict(
+    "ModifyAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "AuthenticationProfileContent": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyCustomDomainAssociationResultTypeDef = TypedDict(
+    "ModifyCustomDomainAssociationResultTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+        "CustomDomainCertExpiryTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PartnerIntegrationOutputMessageTypeDef = TypedDict(
+    "PartnerIntegrationOutputMessageTypeDef",
+    {
+        "DatabaseName": str,
+        "PartnerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResizeProgressMessageTypeDef = TypedDict(
+    "ResizeProgressMessageTypeDef",
+    {
+        "TargetNodeType": str,
+        "TargetNumberOfNodes": int,
+        "TargetClusterType": str,
+        "Status": str,
+        "ImportTablesCompleted": List[str],
+        "ImportTablesInProgress": List[str],
+        "ImportTablesNotStarted": List[str],
+        "AvgResizeRateInMegaBytesPerSecond": float,
+        "TotalResizeDataInMegaBytes": int,
+        "ProgressInMegaBytes": int,
+        "ElapsedTimeInSeconds": int,
+        "EstimatedTimeToCompletionInSeconds": int,
+        "ResizeType": str,
+        "Message": str,
+        "TargetEncryptionType": str,
+        "DataTransferProgressPercent": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 AccountAttributeTypeDef = TypedDict(
     "AccountAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[AttributeValueTargetTypeDef],
     },
     total=False,
 )
 
 ModifyAquaOutputMessageTypeDef = TypedDict(
     "ModifyAquaOutputMessageTypeDef",
     {
         "AquaConfiguration": AquaConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociationTypeDef = TypedDict(
     "AssociationTypeDef",
     {
         "CustomDomainCertificateArn": str,
@@ -2995,15 +2511,15 @@
     total=False,
 )
 
 DescribeAuthenticationProfilesResultTypeDef = TypedDict(
     "DescribeAuthenticationProfilesResultTypeDef",
     {
         "AuthenticationProfiles": List[AuthenticationProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
@@ -3020,24 +2536,24 @@
 )
 
 BatchDeleteClusterSnapshotsResultTypeDef = TypedDict(
     "BatchDeleteClusterSnapshotsResultTypeDef",
     {
         "Resources": List[str],
         "Errors": List[SnapshotErrorMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchModifyClusterSnapshotsOutputMessageTypeDef = TypedDict(
     "BatchModifyClusterSnapshotsOutputMessageTypeDef",
     {
         "Resources": List[str],
         "Errors": List[SnapshotErrorMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterDbRevisionTypeDef = TypedDict(
     "ClusterDbRevisionTypeDef",
     {
         "ClusterIdentifier": str,
@@ -3049,15 +2565,15 @@
 )
 
 ClusterParameterGroupDetailsTypeDef = TypedDict(
     "ClusterParameterGroupDetailsTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefaultClusterParametersTypeDef = TypedDict(
     "DefaultClusterParametersTypeDef",
     {
         "ParameterGroupFamily": str,
@@ -3086,22 +2602,20 @@
     {
         "ResetAllParameters": bool,
         "Parameters": Sequence[ParameterTypeDef],
     },
     total=False,
 )
 
-
 class ResetClusterParameterGroupMessageRequestTypeDef(
     _RequiredResetClusterParameterGroupMessageRequestTypeDef,
     _OptionalResetClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 ClusterParameterGroupStatusTypeDef = TypedDict(
     "ClusterParameterGroupStatusTypeDef",
     {
         "ParameterGroupName": str,
         "ParameterApplyStatus": str,
         "ClusterParameterStatusList": List[ClusterParameterStatusTypeDef],
     },
@@ -3161,21 +2675,19 @@
         "AquaConfigurationStatus": AquaConfigurationStatusType,
         "DefaultIamRoleArn": str,
         "LoadSampleData": str,
     },
     total=False,
 )
 
-
 class CreateClusterMessageRequestTypeDef(
     _RequiredCreateClusterMessageRequestTypeDef, _OptionalCreateClusterMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterParameterGroupMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
         "ParameterGroupFamily": str,
         "Description": str,
     },
@@ -3184,22 +2696,20 @@
     "_OptionalCreateClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateClusterParameterGroupMessageRequestTypeDef(
     _RequiredCreateClusterParameterGroupMessageRequestTypeDef,
     _OptionalCreateClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateClusterSecurityGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSecurityGroupMessageRequestTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Description": str,
     },
 )
@@ -3207,22 +2717,20 @@
     "_OptionalCreateClusterSecurityGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateClusterSecurityGroupMessageRequestTypeDef(
     _RequiredCreateClusterSecurityGroupMessageRequestTypeDef,
     _OptionalCreateClusterSecurityGroupMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotIdentifier": str,
         "ClusterIdentifier": str,
     },
 )
@@ -3231,22 +2739,20 @@
     {
         "ManualSnapshotRetentionPeriod": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateClusterSnapshotMessageRequestTypeDef(
     _RequiredCreateClusterSnapshotMessageRequestTypeDef,
     _OptionalCreateClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "Description": str,
         "SubnetIds": Sequence[str],
     },
@@ -3255,22 +2761,20 @@
     "_OptionalCreateClusterSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateClusterSubnetGroupMessageRequestTypeDef(
     _RequiredCreateClusterSubnetGroupMessageRequestTypeDef,
     _OptionalCreateClusterSubnetGroupMessageRequestTypeDef,
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
@@ -3283,44 +2787,40 @@
         "Severity": str,
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
 _RequiredCreateHsmClientCertificateMessageRequestTypeDef = TypedDict(
     "_RequiredCreateHsmClientCertificateMessageRequestTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
     },
 )
 _OptionalCreateHsmClientCertificateMessageRequestTypeDef = TypedDict(
     "_OptionalCreateHsmClientCertificateMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateHsmClientCertificateMessageRequestTypeDef(
     _RequiredCreateHsmClientCertificateMessageRequestTypeDef,
     _OptionalCreateHsmClientCertificateMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateHsmConfigurationMessageRequestTypeDef = TypedDict(
     "_RequiredCreateHsmConfigurationMessageRequestTypeDef",
     {
         "HsmConfigurationIdentifier": str,
         "Description": str,
         "HsmIpAddress": str,
         "HsmPartitionName": str,
@@ -3332,22 +2832,20 @@
     "_OptionalCreateHsmConfigurationMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateHsmConfigurationMessageRequestTypeDef(
     _RequiredCreateHsmConfigurationMessageRequestTypeDef,
     _OptionalCreateHsmConfigurationMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSnapshotCopyGrantMessageRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotCopyGrantMessageRequestTypeDef",
     {
         "SnapshotCopyGrantName": str,
     },
 )
 _OptionalCreateSnapshotCopyGrantMessageRequestTypeDef = TypedDict(
@@ -3355,22 +2853,20 @@
     {
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSnapshotCopyGrantMessageRequestTypeDef(
     _RequiredCreateSnapshotCopyGrantMessageRequestTypeDef,
     _OptionalCreateSnapshotCopyGrantMessageRequestTypeDef,
 ):
     pass
 
-
 CreateSnapshotScheduleMessageRequestTypeDef = TypedDict(
     "CreateSnapshotScheduleMessageRequestTypeDef",
     {
         "ScheduleDefinitions": Sequence[str],
         "ScheduleIdentifier": str,
         "ScheduleDescription": str,
         "Tags": Sequence[TagTypeDef],
@@ -3403,21 +2899,19 @@
         "Period": UsageLimitPeriodType,
         "BreachAction": UsageLimitBreachActionType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateUsageLimitMessageRequestTypeDef(
     _RequiredCreateUsageLimitMessageRequestTypeDef, _OptionalCreateUsageLimitMessageRequestTypeDef
 ):
     pass
 
-
 EC2SecurityGroupTypeDef = TypedDict(
     "EC2SecurityGroupTypeDef",
     {
         "Status": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
         "Tags": List[TagTypeDef],
@@ -3481,25 +2975,25 @@
         "SnapshotCopyGrantName": str,
         "KmsKeyId": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-SnapshotScheduleResponseMetadataTypeDef = TypedDict(
-    "SnapshotScheduleResponseMetadataTypeDef",
+SnapshotScheduleResponseTypeDef = TypedDict(
+    "SnapshotScheduleResponseTypeDef",
     {
         "ScheduleDefinitions": List[str],
         "ScheduleIdentifier": str,
         "ScheduleDescription": str,
         "Tags": List[TagTypeDef],
         "NextInvocations": List[datetime],
         "AssociatedClusterCount": int,
         "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SnapshotScheduleTypeDef = TypedDict(
     "SnapshotScheduleTypeDef",
     {
         "ScheduleDefinitions": List[str],
@@ -3560,26 +3054,26 @@
         "Tag": TagTypeDef,
         "ResourceName": str,
         "ResourceType": str,
     },
     total=False,
 )
 
-UsageLimitResponseMetadataTypeDef = TypedDict(
-    "UsageLimitResponseMetadataTypeDef",
+UsageLimitResponseTypeDef = TypedDict(
+    "UsageLimitResponseTypeDef",
     {
         "UsageLimitId": str,
         "ClusterIdentifier": str,
         "FeatureType": UsageLimitFeatureTypeType,
         "LimitType": UsageLimitLimitTypeType,
         "Amount": int,
         "Period": UsageLimitPeriodType,
         "BreachAction": UsageLimitBreachActionType,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UsageLimitTypeDef = TypedDict(
     "UsageLimitTypeDef",
     {
         "UsageLimitId": str,
@@ -3595,36 +3089,74 @@
 )
 
 DescribeReservedNodeExchangeStatusOutputMessageTypeDef = TypedDict(
     "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
     {
         "ReservedNodeExchangeStatusDetails": List[ReservedNodeExchangeStatusTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterVersionsMessageTypeDef = TypedDict(
     "ClusterVersionsMessageTypeDef",
     {
         "Marker": str,
         "ClusterVersions": List[ClusterVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
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
+        "MaxRecords": int,
+        "Marker": str,
+    },
+    total=False,
+)
+
+_RequiredModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyClusterMaintenanceMessageRequestTypeDef",
+    {
+        "ClusterIdentifier": str,
     },
 )
+_OptionalModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyClusterMaintenanceMessageRequestTypeDef",
+    {
+        "DeferMaintenance": bool,
+        "DeferMaintenanceIdentifier": str,
+        "DeferMaintenanceStartTime": TimestampTypeDef,
+        "DeferMaintenanceEndTime": TimestampTypeDef,
+        "DeferMaintenanceDuration": int,
+    },
+    total=False,
+)
+
+class ModifyClusterMaintenanceMessageRequestTypeDef(
+    _RequiredModifyClusterMaintenanceMessageRequestTypeDef,
+    _OptionalModifyClusterMaintenanceMessageRequestTypeDef,
+):
+    pass
 
-DataShareResponseMetadataTypeDef = TypedDict(
-    "DataShareResponseMetadataTypeDef",
+DataShareResponseTypeDef = TypedDict(
+    "DataShareResponseTypeDef",
     {
         "DataShareArn": str,
         "ProducerArn": str,
         "AllowPubliclyAccessibleConsumers": bool,
         "DataShareAssociations": List[DataShareAssociationTypeDef],
         "ManagedBy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataShareTypeDef = TypedDict(
     "DataShareTypeDef",
     {
         "DataShareArn": str,
@@ -3632,42 +3164,401 @@
         "AllowPubliclyAccessibleConsumers": bool,
         "DataShareAssociations": List[DataShareAssociationTypeDef],
         "ManagedBy": str,
     },
     total=False,
 )
 
+DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = TypedDict(
+    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+    },
+)
+_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef(
+    _RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+    _OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+):
+    pass
+
+DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
+    {
+        "ClusterSecurityGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
+    {
+        "ClusterSubnetGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = TypedDict(
+    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
+    {
+        "MaintenanceTrackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = TypedDict(
+    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
+    {
+        "ClusterVersion": str,
+        "ClusterParameterGroupFamily": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClustersMessageDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef = TypedDict(
+    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = TypedDict(
+    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
+    {
+        "ConsumerArn": str,
+        "Status": DataShareStatusForConsumerType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = TypedDict(
+    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
+    {
+        "ProducerArn": str,
+        "Status": DataShareStatusForProducerType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = TypedDict(
+    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
+    {
+        "DataShareArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    {
+        "ParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef(
+    _RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+    _OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+):
+    pass
+
+DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = TypedDict(
+    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ResourceOwner": str,
+        "EndpointName": str,
+        "VpcId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = TypedDict(
+    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "Account": str,
+        "Grantee": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
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
+DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
+    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
+    {
+        "HsmClientCertificateIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
+    {
+        "HsmConfigurationIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = TypedDict(
+    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
+    {
+        "ClusterVersion": str,
+        "NodeType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = TypedDict(
+    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+        "ReservedNodeExchangeRequestId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
+    {
+        "ReservedNodeOfferingId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
+    {
+        "SnapshotCopyGrantName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = TypedDict(
+    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ScheduleIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = TypedDict(
+    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "TableRestoreRequestId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeTagsMessageDescribeTagsPaginateTypeDef = TypedDict(
+    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
+    {
+        "ResourceName": str,
+        "ResourceType": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = TypedDict(
+    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
+    {
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
+    "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
+    {
+        "ActionType": ReservedNodeExchangeActionTypeType,
+    },
+)
+_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
+    "_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "SnapshotIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef(
+    _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+    _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
+    "_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+    },
+)
+_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
+    "_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef(
+    _RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
+    _OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
+):
+    pass
+
 DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "MaxRecords": int,
         "Marker": str,
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
@@ -3678,16 +3569,16 @@
 DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "MaxRecords": int,
         "Marker": str,
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
@@ -3745,27 +3636,25 @@
     "_OptionalDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "OwnerAccount": str,
         "Filters": Sequence[NodeConfigurationOptionsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef(
     _RequiredDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
     _OptionalDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeNodeConfigurationOptionsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeConfigurationOptionsMessageRequestTypeDef",
     {
         "ActionType": ActionTypeType,
     },
 )
 _OptionalDescribeNodeConfigurationOptionsMessageRequestTypeDef = TypedDict(
@@ -3778,65 +3667,63 @@
         "Filters": Sequence[NodeConfigurationOptionsFilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-
 class DescribeNodeConfigurationOptionsMessageRequestTypeDef(
     _RequiredDescribeNodeConfigurationOptionsMessageRequestTypeDef,
     _OptionalDescribeNodeConfigurationOptionsMessageRequestTypeDef,
 ):
     pass
 
-
 DescribePartnersOutputMessageTypeDef = TypedDict(
     "DescribePartnersOutputMessageTypeDef",
     {
         "PartnerIntegrationInfoList": List[PartnerIntegrationInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef = TypedDict(
     "DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef",
     {
         "ScheduledActionName": str,
         "TargetActionType": ScheduledActionTypeValuesType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Active": bool,
         "Filters": Sequence[ScheduledActionFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeScheduledActionsMessageRequestTypeDef = TypedDict(
     "DescribeScheduledActionsMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
         "TargetActionType": ScheduledActionTypeValuesType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Active": bool,
         "Filters": Sequence[ScheduledActionFilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
 EndpointAuthorizationListTypeDef = TypedDict(
     "EndpointAuthorizationListTypeDef",
     {
         "EndpointAuthorizationList": List[EndpointAuthorizationTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
@@ -3846,15 +3733,15 @@
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
 
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "VpcEndpointId": str,
@@ -3865,15 +3752,15 @@
 )
 
 NodeConfigurationOptionsMessageTypeDef = TypedDict(
     "NodeConfigurationOptionsMessageTypeDef",
     {
         "NodeConfigurationOptionList": List[NodeConfigurationOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedNodeOfferingTypeDef = TypedDict(
     "ReservedNodeOfferingTypeDef",
     {
         "ReservedNodeOfferingId": str,
@@ -3909,24 +3796,24 @@
     total=False,
 )
 
 RestoreTableFromClusterSnapshotResultTypeDef = TypedDict(
     "RestoreTableFromClusterSnapshotResultTypeDef",
     {
         "TableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TableRestoreStatusMessageTypeDef = TypedDict(
     "TableRestoreStatusMessageTypeDef",
     {
         "TableRestoreStatusDetails": List[TableRestoreStatusTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScheduledActionTypeTypeDef = TypedDict(
     "ScheduledActionTypeTypeDef",
     {
         "ResizeCluster": ResizeClusterMessageTypeDef,
@@ -3946,24 +3833,24 @@
     total=False,
 )
 
 AccountAttributeListTypeDef = TypedDict(
     "AccountAttributeListTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomDomainAssociationsMessageTypeDef = TypedDict(
     "CustomDomainAssociationsMessageTypeDef",
     {
         "Marker": str,
         "Associations": List[AssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OrderableClusterOptionTypeDef = TypedDict(
     "OrderableClusterOptionTypeDef",
     {
         "ClusterVersion": str,
@@ -3985,99 +3872,99 @@
 )
 
 ClusterDbRevisionsMessageTypeDef = TypedDict(
     "ClusterDbRevisionsMessageTypeDef",
     {
         "Marker": str,
         "ClusterDbRevisions": List[ClusterDbRevisionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeDefaultClusterParametersResultTypeDef",
     {
         "DefaultClusterParameters": DefaultClusterParametersTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterParameterGroupsMessageTypeDef = TypedDict(
     "ClusterParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "ParameterGroups": List[ClusterParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterParameterGroupResultTypeDef = TypedDict(
     "CreateClusterParameterGroupResultTypeDef",
     {
         "ClusterParameterGroup": ClusterParameterGroupTypeDef,
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
 
 CreateHsmClientCertificateResultTypeDef = TypedDict(
     "CreateHsmClientCertificateResultTypeDef",
     {
         "HsmClientCertificate": HsmClientCertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HsmClientCertificateMessageTypeDef = TypedDict(
     "HsmClientCertificateMessageTypeDef",
     {
         "Marker": str,
         "HsmClientCertificates": List[HsmClientCertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHsmConfigurationResultTypeDef = TypedDict(
     "CreateHsmConfigurationResultTypeDef",
     {
         "HsmConfiguration": HsmConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HsmConfigurationMessageTypeDef = TypedDict(
     "HsmConfigurationMessageTypeDef",
     {
         "Marker": str,
         "HsmConfigurations": List[HsmConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSecurityGroupTypeDef = TypedDict(
     "ClusterSecurityGroupTypeDef",
     {
         "ClusterSecurityGroupName": str,
@@ -4089,160 +3976,160 @@
     total=False,
 )
 
 CreateSnapshotCopyGrantResultTypeDef = TypedDict(
     "CreateSnapshotCopyGrantResultTypeDef",
     {
         "SnapshotCopyGrant": SnapshotCopyGrantTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SnapshotCopyGrantMessageTypeDef = TypedDict(
     "SnapshotCopyGrantMessageTypeDef",
     {
         "Marker": str,
         "SnapshotCopyGrants": List[SnapshotCopyGrantTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSnapshotSchedulesOutputMessageTypeDef = TypedDict(
     "DescribeSnapshotSchedulesOutputMessageTypeDef",
     {
         "SnapshotSchedules": List[SnapshotScheduleTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthorizeSnapshotAccessResultTypeDef = TypedDict(
     "AuthorizeSnapshotAccessResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyClusterSnapshotResultTypeDef = TypedDict(
     "CopyClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSnapshotResultTypeDef = TypedDict(
     "CreateClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterSnapshotResultTypeDef = TypedDict(
     "DeleteClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterSnapshotResultTypeDef = TypedDict(
     "ModifyClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RevokeSnapshotAccessResultTypeDef = TypedDict(
     "RevokeSnapshotAccessResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SnapshotMessageTypeDef = TypedDict(
     "SnapshotMessageTypeDef",
     {
         "Marker": str,
         "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaggedResourceListMessageTypeDef = TypedDict(
     "TaggedResourceListMessageTypeDef",
     {
         "TaggedResources": List[TaggedResourceTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UsageLimitListTypeDef = TypedDict(
     "UsageLimitListTypeDef",
     {
         "UsageLimits": List[UsageLimitTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSharesForConsumerResultTypeDef = TypedDict(
     "DescribeDataSharesForConsumerResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSharesForProducerResultTypeDef = TypedDict(
     "DescribeDataSharesForProducerResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSharesResultTypeDef = TypedDict(
     "DescribeDataSharesResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointAccessResponseMetadataTypeDef = TypedDict(
-    "EndpointAccessResponseMetadataTypeDef",
+EndpointAccessResponseTypeDef = TypedDict(
+    "EndpointAccessResponseTypeDef",
     {
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "SubnetGroupName": str,
         "EndpointStatus": str,
         "EndpointName": str,
         "EndpointCreateTime": datetime,
         "Port": int,
         "Address": str,
         "VpcSecurityGroups": List[VpcSecurityGroupMembershipTypeDef],
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointAccessTypeDef = TypedDict(
     "EndpointAccessTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4270,40 +4157,40 @@
 )
 
 GetReservedNodeExchangeOfferingsOutputMessageTypeDef = TypedDict(
     "GetReservedNodeExchangeOfferingsOutputMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeOfferings": List[ReservedNodeOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedNodeOfferingsMessageTypeDef = TypedDict(
     "ReservedNodeOfferingsMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeOfferings": List[ReservedNodeOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptReservedNodeExchangeOutputMessageTypeDef = TypedDict(
     "AcceptReservedNodeExchangeOutputMessageTypeDef",
     {
         "ExchangedReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PurchaseReservedNodeOfferingResultTypeDef = TypedDict(
     "PurchaseReservedNodeOfferingResultTypeDef",
     {
         "ReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedNodeConfigurationOptionTypeDef = TypedDict(
     "ReservedNodeConfigurationOptionTypeDef",
     {
         "SourceReservedNode": ReservedNodeTypeDef,
@@ -4314,15 +4201,15 @@
 )
 
 ReservedNodesMessageTypeDef = TypedDict(
     "ReservedNodesMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodes": List[ReservedNodeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateScheduledActionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
@@ -4331,70 +4218,66 @@
         "IamRole": str,
     },
 )
 _OptionalCreateScheduledActionMessageRequestTypeDef = TypedDict(
     "_OptionalCreateScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionDescription": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Enable": bool,
     },
     total=False,
 )
 
-
 class CreateScheduledActionMessageRequestTypeDef(
     _RequiredCreateScheduledActionMessageRequestTypeDef,
     _OptionalCreateScheduledActionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyScheduledActionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
     },
 )
 _OptionalModifyScheduledActionMessageRequestTypeDef = TypedDict(
     "_OptionalModifyScheduledActionMessageRequestTypeDef",
     {
         "TargetAction": ScheduledActionTypeTypeDef,
         "Schedule": str,
         "IamRole": str,
         "ScheduledActionDescription": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Enable": bool,
     },
     total=False,
 )
 
-
 class ModifyScheduledActionMessageRequestTypeDef(
     _RequiredModifyScheduledActionMessageRequestTypeDef,
     _OptionalModifyScheduledActionMessageRequestTypeDef,
 ):
     pass
 
-
-ScheduledActionResponseMetadataTypeDef = TypedDict(
-    "ScheduledActionResponseMetadataTypeDef",
+ScheduledActionResponseTypeDef = TypedDict(
+    "ScheduledActionResponseTypeDef",
     {
         "ScheduledActionName": str,
         "TargetAction": ScheduledActionTypeTypeDef,
         "Schedule": str,
         "IamRole": str,
         "ScheduledActionDescription": str,
         "State": ScheduledActionStateType,
         "NextInvocations": List[datetime],
         "StartTime": datetime,
         "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScheduledActionTypeDef = TypedDict(
     "ScheduledActionTypeDef",
     {
         "ScheduledActionName": str,
@@ -4421,15 +4304,15 @@
 )
 
 OrderableClusterOptionsMessageTypeDef = TypedDict(
     "OrderableClusterOptionsMessageTypeDef",
     {
         "OrderableClusterOptions": List[OrderableClusterOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSubnetGroupTypeDef = TypedDict(
     "ClusterSubnetGroupTypeDef",
     {
         "ClusterSubnetGroupName": str,
@@ -4442,49 +4325,49 @@
     total=False,
 )
 
 AuthorizeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSecurityGroupMessageTypeDef = TypedDict(
     "ClusterSecurityGroupMessageTypeDef",
     {
         "Marker": str,
         "ClusterSecurityGroups": List[ClusterSecurityGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSecurityGroupResultTypeDef = TypedDict(
     "CreateClusterSecurityGroupResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RevokeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeClusterSecurityGroupIngressResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointAccessListTypeDef = TypedDict(
     "EndpointAccessListTypeDef",
     {
         "EndpointAccessList": List[EndpointAccessTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4547,182 +4430,182 @@
 )
 
 GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef = TypedDict(
     "GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeConfigurationOptionList": List[ReservedNodeConfigurationOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScheduledActionsMessageTypeDef = TypedDict(
     "ScheduledActionsMessageTypeDef",
     {
         "Marker": str,
         "ScheduledActions": List[ScheduledActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrackListMessageTypeDef = TypedDict(
     "TrackListMessageTypeDef",
     {
         "MaintenanceTracks": List[MaintenanceTrackTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSubnetGroupMessageTypeDef = TypedDict(
     "ClusterSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "ClusterSubnetGroups": List[ClusterSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSubnetGroupResultTypeDef = TypedDict(
     "CreateClusterSubnetGroupResultTypeDef",
     {
         "ClusterSubnetGroup": ClusterSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterSubnetGroupResultTypeDef = TypedDict(
     "ModifyClusterSubnetGroupResultTypeDef",
     {
         "ClusterSubnetGroup": ClusterSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClustersMessageTypeDef = TypedDict(
     "ClustersMessageTypeDef",
     {
         "Marker": str,
         "Clusters": List[ClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResultTypeDef = TypedDict(
     "DeleteClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisableSnapshotCopyResultTypeDef = TypedDict(
     "DisableSnapshotCopyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableSnapshotCopyResultTypeDef = TypedDict(
     "EnableSnapshotCopyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterDbRevisionResultTypeDef = TypedDict(
     "ModifyClusterDbRevisionResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterIamRolesResultTypeDef = TypedDict(
     "ModifyClusterIamRolesResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterMaintenanceResultTypeDef = TypedDict(
     "ModifyClusterMaintenanceResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterResultTypeDef = TypedDict(
     "ModifyClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifySnapshotCopyRetentionPeriodResultTypeDef = TypedDict(
     "ModifySnapshotCopyRetentionPeriodResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PauseClusterResultTypeDef = TypedDict(
     "PauseClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootClusterResultTypeDef = TypedDict(
     "RebootClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResizeClusterResultTypeDef = TypedDict(
     "ResizeClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreFromClusterSnapshotResultTypeDef = TypedDict(
     "RestoreFromClusterSnapshotResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResumeClusterResultTypeDef = TypedDict(
     "ResumeClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RotateEncryptionKeyResultTypeDef = TypedDict(
     "RotateEncryptionKeyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/type_defs.pyi` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/type_defs.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_redshift.type_defs import AcceptReservedNodeExchangeInputMessageRequestTypeDef
 
-    data: AcceptReservedNodeExchangeInputMessageRequestTypeDef = {...}
+    data: AcceptReservedNodeExchangeInputMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -47,16 +47,18 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AttributeValueTargetTypeDef",
     "AccountWithRestoreAccessTypeDef",
     "AquaConfigurationTypeDef",
     "AssociateDataShareConsumerMessageRequestTypeDef",
     "CertificateAssociationTypeDef",
     "AuthenticationProfileTypeDef",
     "AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef",
@@ -65,21 +67,18 @@
     "AuthorizeSnapshotAccessMessageRequestTypeDef",
     "SupportedPlatformTypeDef",
     "DeleteClusterSnapshotMessageTypeDef",
     "SnapshotErrorMessageTypeDef",
     "BatchModifyClusterSnapshotsMessageRequestTypeDef",
     "CancelResizeMessageRequestTypeDef",
     "ClusterAssociatedToScheduleTypeDef",
-    "ClusterCredentialsTypeDef",
     "RevisionTargetTypeDef",
-    "ClusterExtendedCredentialsTypeDef",
     "ClusterIamRoleTypeDef",
     "ClusterNodeTypeDef",
     "ParameterTypeDef",
-    "ClusterParameterGroupNameMessageTypeDef",
     "ClusterParameterStatusTypeDef",
     "TagTypeDef",
     "ClusterSecurityGroupMembershipTypeDef",
     "ClusterSnapshotCopyStatusTypeDef",
     "DataTransferProgressTypeDef",
     "DeferredMaintenanceWindowTypeDef",
     "ElasticIpStatusTypeDef",
@@ -88,23 +87,20 @@
     "ReservedNodeExchangeStatusTypeDef",
     "ResizeInfoTypeDef",
     "RestoreStatusTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ClusterVersionTypeDef",
     "CopyClusterSnapshotMessageRequestTypeDef",
     "CreateAuthenticationProfileMessageRequestTypeDef",
-    "CreateAuthenticationProfileResultTypeDef",
     "CreateCustomDomainAssociationMessageRequestTypeDef",
-    "CreateCustomDomainAssociationResultTypeDef",
     "CreateEndpointAccessMessageRequestTypeDef",
-    "CustomerStorageMessageTypeDef",
+    "TimestampTypeDef",
     "DataShareAssociationTypeDef",
     "DeauthorizeDataShareMessageRequestTypeDef",
     "DeleteAuthenticationProfileMessageRequestTypeDef",
-    "DeleteAuthenticationProfileResultTypeDef",
     "DeleteClusterMessageRequestTypeDef",
     "DeleteClusterParameterGroupMessageRequestTypeDef",
     "DeleteClusterSecurityGroupMessageRequestTypeDef",
     "DeleteClusterSnapshotMessageRequestTypeDef",
     "DeleteClusterSubnetGroupMessageRequestTypeDef",
     "DeleteCustomDomainAssociationMessageRequestTypeDef",
     "DeleteEndpointAccessMessageRequestTypeDef",
@@ -114,139 +110,113 @@
     "DeleteScheduledActionMessageRequestTypeDef",
     "DeleteSnapshotCopyGrantMessageRequestTypeDef",
     "DeleteSnapshotScheduleMessageRequestTypeDef",
     "DeleteTagsMessageRequestTypeDef",
     "DeleteUsageLimitMessageRequestTypeDef",
     "DescribeAccountAttributesMessageRequestTypeDef",
     "DescribeAuthenticationProfilesMessageRequestTypeDef",
-    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClusterDbRevisionsMessageRequestTypeDef",
-    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
     "DescribeClusterParameterGroupsMessageRequestTypeDef",
-    "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
     "DescribeClusterParametersMessageRequestTypeDef",
-    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
     "DescribeClusterSecurityGroupsMessageRequestTypeDef",
     "SnapshotSortingEntityTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
     "DescribeClusterSubnetGroupsMessageRequestTypeDef",
-    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
     "DescribeClusterTracksMessageRequestTypeDef",
-    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
     "DescribeClusterVersionsMessageRequestTypeDef",
-    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
     "DescribeClustersMessageRequestTypeDef",
-    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
     "DescribeCustomDomainAssociationsMessageRequestTypeDef",
-    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
     "DescribeDataSharesForConsumerMessageRequestTypeDef",
-    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
     "DescribeDataSharesForProducerMessageRequestTypeDef",
-    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
     "DescribeDataSharesMessageRequestTypeDef",
-    "DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
     "DescribeDefaultClusterParametersMessageRequestTypeDef",
-    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
     "DescribeEndpointAccessMessageRequestTypeDef",
-    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     "DescribeEventCategoriesMessageRequestTypeDef",
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
     "DescribeEventSubscriptionsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
-    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
-    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     "DescribeLoggingStatusMessageRequestTypeDef",
     "NodeConfigurationOptionsFilterTypeDef",
-    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     "DescribePartnersInputMessageRequestTypeDef",
     "PartnerIntegrationInfoTypeDef",
-    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
     "DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef",
-    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
     "DescribeReservedNodeOfferingsMessageRequestTypeDef",
-    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
     "DescribeReservedNodesMessageRequestTypeDef",
     "DescribeResizeMessageRequestTypeDef",
     "ScheduledActionFilterTypeDef",
-    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
     "DescribeSnapshotCopyGrantsMessageRequestTypeDef",
-    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
     "DescribeSnapshotSchedulesMessageRequestTypeDef",
-    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
     "DescribeTableRestoreStatusMessageRequestTypeDef",
-    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
     "DescribeTagsMessageRequestTypeDef",
-    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
     "DescribeUsageLimitsMessageRequestTypeDef",
     "DisableLoggingMessageRequestTypeDef",
     "DisableSnapshotCopyMessageRequestTypeDef",
     "DisassociateDataShareConsumerMessageRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableLoggingMessageRequestTypeDef",
     "EnableSnapshotCopyMessageRequestTypeDef",
     "EndpointAuthorizationTypeDef",
-    "EndpointAuthorizationResponseMetadataTypeDef",
     "EventInfoMapTypeDef",
     "EventTypeDef",
     "GetClusterCredentialsMessageRequestTypeDef",
     "GetClusterCredentialsWithIAMMessageRequestTypeDef",
-    "GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
     "GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
-    "GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     "GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
-    "LoggingStatusTypeDef",
     "ModifyAquaInputMessageRequestTypeDef",
     "ModifyAuthenticationProfileMessageRequestTypeDef",
-    "ModifyAuthenticationProfileResultTypeDef",
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     "ModifyClusterIamRolesMessageRequestTypeDef",
-    "ModifyClusterMaintenanceMessageRequestTypeDef",
     "ModifyClusterMessageRequestTypeDef",
     "ModifyClusterSnapshotMessageRequestTypeDef",
     "ModifyClusterSnapshotScheduleMessageRequestTypeDef",
     "ModifyClusterSubnetGroupMessageRequestTypeDef",
     "ModifyCustomDomainAssociationMessageRequestTypeDef",
-    "ModifyCustomDomainAssociationResultTypeDef",
     "ModifyEndpointAccessMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     "ModifySnapshotScheduleMessageRequestTypeDef",
     "ModifyUsageLimitMessageRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "NodeConfigurationOptionTypeDef",
-    "PaginatorConfigTypeDef",
     "PartnerIntegrationInputMessageRequestTypeDef",
-    "PartnerIntegrationOutputMessageTypeDef",
     "PauseClusterMessageRequestTypeDef",
     "PauseClusterMessageTypeDef",
     "PurchaseReservedNodeOfferingMessageRequestTypeDef",
     "RebootClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RejectDataShareMessageRequestTypeDef",
     "ResizeClusterMessageRequestTypeDef",
     "ResizeClusterMessageTypeDef",
-    "ResizeProgressMessageTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreFromClusterSnapshotMessageRequestTypeDef",
     "RestoreTableFromClusterSnapshotMessageRequestTypeDef",
     "TableRestoreStatusTypeDef",
     "ResumeClusterMessageRequestTypeDef",
     "ResumeClusterMessageTypeDef",
     "RevokeClusterSecurityGroupIngressMessageRequestTypeDef",
     "RevokeEndpointAccessMessageRequestTypeDef",
     "RevokeSnapshotAccessMessageRequestTypeDef",
     "RotateEncryptionKeyMessageRequestTypeDef",
     "SupportedOperationTypeDef",
     "UpdatePartnerStatusInputMessageRequestTypeDef",
+    "ClusterCredentialsTypeDef",
+    "ClusterExtendedCredentialsTypeDef",
+    "ClusterParameterGroupNameMessageTypeDef",
+    "CreateAuthenticationProfileResultTypeDef",
+    "CreateCustomDomainAssociationResultTypeDef",
+    "CustomerStorageMessageTypeDef",
+    "DeleteAuthenticationProfileResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EndpointAuthorizationResponseTypeDef",
+    "LoggingStatusTypeDef",
+    "ModifyAuthenticationProfileResultTypeDef",
+    "ModifyCustomDomainAssociationResultTypeDef",
+    "PartnerIntegrationOutputMessageTypeDef",
+    "ResizeProgressMessageTypeDef",
     "AccountAttributeTypeDef",
     "ModifyAquaOutputMessageTypeDef",
     "AssociationTypeDef",
     "DescribeAuthenticationProfilesResultTypeDef",
     "AvailabilityZoneTypeDef",
     "BatchDeleteClusterSnapshotsRequestRequestTypeDef",
     "BatchDeleteClusterSnapshotsResultTypeDef",
@@ -272,24 +242,56 @@
     "CreateUsageLimitMessageRequestTypeDef",
     "EC2SecurityGroupTypeDef",
     "EventSubscriptionTypeDef",
     "HsmClientCertificateTypeDef",
     "HsmConfigurationTypeDef",
     "IPRangeTypeDef",
     "SnapshotCopyGrantTypeDef",
-    "SnapshotScheduleResponseMetadataTypeDef",
+    "SnapshotScheduleResponseTypeDef",
     "SnapshotScheduleTypeDef",
     "SnapshotTypeDef",
     "TaggedResourceTypeDef",
-    "UsageLimitResponseMetadataTypeDef",
+    "UsageLimitResponseTypeDef",
     "UsageLimitTypeDef",
     "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
     "ClusterVersionsMessageTypeDef",
-    "DataShareResponseMetadataTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
+    "ModifyClusterMaintenanceMessageRequestTypeDef",
+    "DataShareResponseTypeDef",
     "DataShareTypeDef",
+    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
+    "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
+    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
+    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
+    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
+    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
+    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
+    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
+    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
+    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
+    "DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
+    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
+    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
+    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
+    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
+    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
+    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
+    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
+    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
+    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
+    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
+    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
+    "GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
+    "GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     "DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef",
     "DescribeClustersMessageClusterAvailableWaitTypeDef",
     "DescribeClustersMessageClusterDeletedWaitTypeDef",
     "DescribeClustersMessageClusterRestoredWaitTypeDef",
     "DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef",
@@ -336,26 +338,26 @@
     "SnapshotMessageTypeDef",
     "TaggedResourceListMessageTypeDef",
     "UsageLimitListTypeDef",
     "DescribeDataSharesForConsumerResultTypeDef",
     "DescribeDataSharesForProducerResultTypeDef",
     "DescribeDataSharesResultTypeDef",
     "EventCategoriesMessageTypeDef",
-    "EndpointAccessResponseMetadataTypeDef",
+    "EndpointAccessResponseTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "GetReservedNodeExchangeOfferingsOutputMessageTypeDef",
     "ReservedNodeOfferingsMessageTypeDef",
     "AcceptReservedNodeExchangeOutputMessageTypeDef",
     "PurchaseReservedNodeOfferingResultTypeDef",
     "ReservedNodeConfigurationOptionTypeDef",
     "ReservedNodesMessageTypeDef",
     "CreateScheduledActionMessageRequestTypeDef",
     "ModifyScheduledActionMessageRequestTypeDef",
-    "ScheduledActionResponseMetadataTypeDef",
+    "ScheduledActionResponseTypeDef",
     "ScheduledActionTypeDef",
     "MaintenanceTrackTypeDef",
     "OrderableClusterOptionsMessageTypeDef",
     "ClusterSubnetGroupTypeDef",
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     "ClusterSecurityGroupMessageTypeDef",
     "CreateClusterSecurityGroupResultTypeDef",
@@ -390,14 +392,25 @@
     "AcceptReservedNodeExchangeInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
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
 AttributeValueTargetTypeDef = TypedDict(
     "AttributeValueTargetTypeDef",
     {
         "AttributeValue": str,
     },
     total=False,
 )
@@ -432,20 +445,22 @@
         "AssociateEntireAccount": bool,
         "ConsumerArn": str,
         "ConsumerRegion": str,
     },
     total=False,
 )
 
+
 class AssociateDataShareConsumerMessageRequestTypeDef(
     _RequiredAssociateDataShareConsumerMessageRequestTypeDef,
     _OptionalAssociateDataShareConsumerMessageRequestTypeDef,
 ):
     pass
 
+
 CertificateAssociationTypeDef = TypedDict(
     "CertificateAssociationTypeDef",
     {
         "CustomDomainName": str,
         "ClusterIdentifier": str,
     },
     total=False,
@@ -472,20 +487,22 @@
         "CIDRIP": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+
 class AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef(
     _RequiredAuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
     _OptionalAuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
+
 AuthorizeDataShareMessageRequestTypeDef = TypedDict(
     "AuthorizeDataShareMessageRequestTypeDef",
     {
         "DataShareArn": str,
         "ConsumerIdentifier": str,
     },
 )
@@ -501,20 +518,22 @@
     {
         "ClusterIdentifier": str,
         "VpcIds": Sequence[str],
     },
     total=False,
 )
 
+
 class AuthorizeEndpointAccessMessageRequestTypeDef(
     _RequiredAuthorizeEndpointAccessMessageRequestTypeDef,
     _OptionalAuthorizeEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredAuthorizeSnapshotAccessMessageRequestTypeDef = TypedDict(
     "_RequiredAuthorizeSnapshotAccessMessageRequestTypeDef",
     {
         "AccountWithRestoreAccess": str,
     },
 )
 _OptionalAuthorizeSnapshotAccessMessageRequestTypeDef = TypedDict(
@@ -523,20 +542,22 @@
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
+
 class AuthorizeSnapshotAccessMessageRequestTypeDef(
     _RequiredAuthorizeSnapshotAccessMessageRequestTypeDef,
     _OptionalAuthorizeSnapshotAccessMessageRequestTypeDef,
 ):
     pass
 
+
 SupportedPlatformTypeDef = TypedDict(
     "SupportedPlatformTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -551,19 +572,21 @@
     "_OptionalDeleteClusterSnapshotMessageTypeDef",
     {
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
+
 class DeleteClusterSnapshotMessageTypeDef(
     _RequiredDeleteClusterSnapshotMessageTypeDef, _OptionalDeleteClusterSnapshotMessageTypeDef
 ):
     pass
 
+
 SnapshotErrorMessageTypeDef = TypedDict(
     "SnapshotErrorMessageTypeDef",
     {
         "SnapshotIdentifier": str,
         "SnapshotClusterIdentifier": str,
         "FailureCode": str,
         "FailureReason": str,
@@ -582,20 +605,22 @@
     {
         "ManualSnapshotRetentionPeriod": int,
         "Force": bool,
     },
     total=False,
 )
 
+
 class BatchModifyClusterSnapshotsMessageRequestTypeDef(
     _RequiredBatchModifyClusterSnapshotsMessageRequestTypeDef,
     _OptionalBatchModifyClusterSnapshotsMessageRequestTypeDef,
 ):
     pass
 
+
 CancelResizeMessageRequestTypeDef = TypedDict(
     "CancelResizeMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -604,45 +629,24 @@
     {
         "ClusterIdentifier": str,
         "ScheduleAssociationState": ScheduleStateType,
     },
     total=False,
 )
 
-ClusterCredentialsTypeDef = TypedDict(
-    "ClusterCredentialsTypeDef",
-    {
-        "DbUser": str,
-        "DbPassword": str,
-        "Expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RevisionTargetTypeDef = TypedDict(
     "RevisionTargetTypeDef",
     {
         "DatabaseRevision": str,
         "Description": str,
         "DatabaseRevisionReleaseDate": datetime,
     },
     total=False,
 )
 
-ClusterExtendedCredentialsTypeDef = TypedDict(
-    "ClusterExtendedCredentialsTypeDef",
-    {
-        "DbUser": str,
-        "DbPassword": str,
-        "Expiration": datetime,
-        "NextRefreshTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ClusterIamRoleTypeDef = TypedDict(
     "ClusterIamRoleTypeDef",
     {
         "IamRoleArn": str,
         "ApplyStatus": str,
     },
     total=False,
@@ -670,23 +674,14 @@
         "ApplyType": ParameterApplyTypeType,
         "IsModifiable": bool,
         "MinimumEngineVersion": str,
     },
     total=False,
 )
 
-ClusterParameterGroupNameMessageTypeDef = TypedDict(
-    "ClusterParameterGroupNameMessageTypeDef",
-    {
-        "ParameterGroupName": str,
-        "ParameterGroupStatus": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ClusterParameterStatusTypeDef = TypedDict(
     "ClusterParameterStatusTypeDef",
     {
         "ParameterName": str,
         "ParameterApplyStatus": str,
         "ParameterApplyErrorDescription": str,
     },
@@ -851,57 +846,39 @@
     {
         "SourceSnapshotClusterIdentifier": str,
         "ManualSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
+
 class CopyClusterSnapshotMessageRequestTypeDef(
     _RequiredCopyClusterSnapshotMessageRequestTypeDef,
     _OptionalCopyClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 CreateAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "CreateAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
-CreateAuthenticationProfileResultTypeDef = TypedDict(
-    "CreateAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "AuthenticationProfileContent": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateCustomDomainAssociationMessageRequestTypeDef = TypedDict(
     "CreateCustomDomainAssociationMessageRequestTypeDef",
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
         "ClusterIdentifier": str,
     },
 )
 
-CreateCustomDomainAssociationResultTypeDef = TypedDict(
-    "CreateCustomDomainAssociationResultTypeDef",
-    {
-        "CustomDomainName": str,
-        "CustomDomainCertificateArn": str,
-        "ClusterIdentifier": str,
-        "CustomDomainCertExpiryTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateEndpointAccessMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
         "SubnetGroupName": str,
     },
 )
@@ -911,29 +888,23 @@
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateEndpointAccessMessageRequestTypeDef(
     _RequiredCreateEndpointAccessMessageRequestTypeDef,
     _OptionalCreateEndpointAccessMessageRequestTypeDef,
 ):
     pass
 
-CustomerStorageMessageTypeDef = TypedDict(
-    "CustomerStorageMessageTypeDef",
-    {
-        "TotalBackupSizeInMegaBytes": float,
-        "TotalProvisionedStorageInMegaBytes": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
+TimestampTypeDef = Union[datetime, str]
 DataShareAssociationTypeDef = TypedDict(
     "DataShareAssociationTypeDef",
     {
         "ConsumerIdentifier": str,
         "Status": DataShareStatusType,
         "ConsumerRegion": str,
         "CreatedDate": datetime,
@@ -953,22 +924,14 @@
 DeleteAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "DeleteAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
     },
 )
 
-DeleteAuthenticationProfileResultTypeDef = TypedDict(
-    "DeleteAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteClusterMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalDeleteClusterMessageRequestTypeDef = TypedDict(
@@ -977,19 +940,21 @@
         "SkipFinalClusterSnapshot": bool,
         "FinalClusterSnapshotIdentifier": str,
         "FinalClusterSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
+
 class DeleteClusterMessageRequestTypeDef(
     _RequiredDeleteClusterMessageRequestTypeDef, _OptionalDeleteClusterMessageRequestTypeDef
 ):
     pass
 
+
 DeleteClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "DeleteClusterParameterGroupMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 
@@ -1010,20 +975,22 @@
     "_OptionalDeleteClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
+
 class DeleteClusterSnapshotMessageRequestTypeDef(
     _RequiredDeleteClusterSnapshotMessageRequestTypeDef,
     _OptionalDeleteClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 DeleteClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "DeleteClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
     },
 )
 
@@ -1110,77 +1077,46 @@
     "DescribeAuthenticationProfilesMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
     },
     total=False,
 )
 
-DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = TypedDict(
-    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ClusterIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeClusterDbRevisionsMessageRequestTypeDef = TypedDict(
     "DescribeClusterDbRevisionsMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterParameterGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterParameterGroupsMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef(
-    _RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-    _OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeClusterParametersMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1189,30 +1125,21 @@
         "Source": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeClusterParametersMessageRequestTypeDef(
     _RequiredDescribeClusterParametersMessageRequestTypeDef,
     _OptionalDescribeClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
-    {
-        "ClusterSecurityGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeClusterSecurityGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSecurityGroupsMessageRequestTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "MaxRecords": int,
         "Marker": str,
@@ -1232,216 +1159,118 @@
     "_OptionalSnapshotSortingEntityTypeDef",
     {
         "SortOrder": SortByOrderType,
     },
     total=False,
 )
 
+
 class SnapshotSortingEntityTypeDef(
     _RequiredSnapshotSortingEntityTypeDef, _OptionalSnapshotSortingEntityTypeDef
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
-    {
-        "ClusterSubnetGroupName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterSubnetGroupsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSubnetGroupsMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = TypedDict(
-    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
-    {
-        "MaintenanceTrackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterTracksMessageRequestTypeDef = TypedDict(
     "DescribeClusterTracksMessageRequestTypeDef",
     {
         "MaintenanceTrackName": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = TypedDict(
-    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
-    {
-        "ClusterVersion": str,
-        "ClusterParameterGroupFamily": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClusterVersionsMessageRequestTypeDef = TypedDict(
     "DescribeClusterVersionsMessageRequestTypeDef",
     {
         "ClusterVersion": str,
         "ClusterParameterGroupFamily": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeClustersMessageDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClustersMessageRequestTypeDef = TypedDict(
     "DescribeClustersMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef = TypedDict(
-    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
-    {
-        "CustomDomainName": str,
-        "CustomDomainCertificateArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeCustomDomainAssociationsMessageRequestTypeDef = TypedDict(
     "DescribeCustomDomainAssociationsMessageRequestTypeDef",
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = TypedDict(
-    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
-    {
-        "ConsumerArn": str,
-        "Status": DataShareStatusForConsumerType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSharesForConsumerMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesForConsumerMessageRequestTypeDef",
     {
         "ConsumerArn": str,
         "Status": DataShareStatusForConsumerType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = TypedDict(
-    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
-    {
-        "ProducerArn": str,
-        "Status": DataShareStatusForProducerType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSharesForProducerMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesForProducerMessageRequestTypeDef",
     {
         "ProducerArn": str,
         "Status": DataShareStatusForProducerType,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = TypedDict(
-    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
-    {
-        "DataShareArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSharesMessageRequestTypeDef = TypedDict(
     "DescribeDataSharesMessageRequestTypeDef",
     {
         "DataShareArn": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    {
-        "ParameterGroupFamily": str,
-    },
-)
-_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef(
-    _RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-    _OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeDefaultClusterParametersMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeDefaultClusterParametersMessageRequestTypeDef",
     {
         "ParameterGroupFamily": str,
     },
 )
 _OptionalDescribeDefaultClusterParametersMessageRequestTypeDef = TypedDict(
@@ -1449,56 +1278,35 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeDefaultClusterParametersMessageRequestTypeDef(
     _RequiredDescribeDefaultClusterParametersMessageRequestTypeDef,
     _OptionalDescribeDefaultClusterParametersMessageRequestTypeDef,
 ):
     pass
 
-DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = TypedDict(
-    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ResourceOwner": str,
-        "EndpointName": str,
-        "VpcId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeEndpointAccessMessageRequestTypeDef = TypedDict(
     "DescribeEndpointAccessMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "EndpointName": str,
         "VpcId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = TypedDict(
-    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "Account": str,
-        "Grantee": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEndpointAuthorizationMessageRequestTypeDef = TypedDict(
     "DescribeEndpointAuthorizationMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "Account": str,
         "Grantee": bool,
         "MaxRecords": int,
@@ -1511,98 +1319,38 @@
     "DescribeEventCategoriesMessageRequestTypeDef",
     {
         "SourceType": str,
     },
     total=False,
 )
 
-DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
-    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
-    {
-        "SubscriptionName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventSubscriptionsMessageRequestTypeDef = TypedDict(
     "DescribeEventSubscriptionsMessageRequestTypeDef",
     {
         "SubscriptionName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
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
-DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
-    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
-    {
-        "HsmClientCertificateIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeHsmClientCertificatesMessageRequestTypeDef = TypedDict(
     "DescribeHsmClientCertificatesMessageRequestTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
-    {
-        "HsmConfigurationIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeHsmConfigurationsMessageRequestTypeDef = TypedDict(
     "DescribeHsmConfigurationsMessageRequestTypeDef",
     {
         "HsmConfigurationIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
@@ -1624,24 +1372,14 @@
         "Name": NodeConfigurationOptionsFilterNameType,
         "Operator": OperatorTypeType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = TypedDict(
-    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
-    {
-        "ClusterVersion": str,
-        "NodeType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrderableClusterOptionsMessageRequestTypeDef = TypedDict(
     "DescribeOrderableClusterOptionsMessageRequestTypeDef",
     {
         "ClusterVersion": str,
         "NodeType": str,
         "MaxRecords": int,
         "Marker": str,
@@ -1661,82 +1399,56 @@
     {
         "DatabaseName": str,
         "PartnerName": str,
     },
     total=False,
 )
 
+
 class DescribePartnersInputMessageRequestTypeDef(
     _RequiredDescribePartnersInputMessageRequestTypeDef,
     _OptionalDescribePartnersInputMessageRequestTypeDef,
 ):
     pass
 
+
 PartnerIntegrationInfoTypeDef = TypedDict(
     "PartnerIntegrationInfoTypeDef",
     {
         "DatabaseName": str,
         "PartnerName": str,
         "Status": PartnerIntegrationStatusType,
         "StatusMessage": str,
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
-DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = TypedDict(
-    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-        "ReservedNodeExchangeRequestId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "ReservedNodeExchangeRequestId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = TypedDict(
-    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
-    {
-        "ReservedNodeOfferingId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedNodeOfferingsMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodeOfferingsMessageRequestTypeDef",
     {
         "ReservedNodeOfferingId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = TypedDict(
-    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeReservedNodesMessageRequestTypeDef = TypedDict(
     "DescribeReservedNodesMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
         "MaxRecords": int,
         "Marker": str,
     },
@@ -1754,121 +1466,63 @@
     "ScheduledActionFilterTypeDef",
     {
         "Name": ScheduledActionFilterNameType,
         "Values": Sequence[str],
     },
 )
 
-DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
-    {
-        "SnapshotCopyGrantName": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotCopyGrantsMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotCopyGrantsMessageRequestTypeDef",
     {
         "SnapshotCopyGrantName": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = TypedDict(
-    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ScheduleIdentifier": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotSchedulesMessageRequestTypeDef = TypedDict(
     "DescribeSnapshotSchedulesMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "ScheduleIdentifier": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = TypedDict(
-    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "TableRestoreRequestId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTableRestoreStatusMessageRequestTypeDef = TypedDict(
     "DescribeTableRestoreStatusMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "TableRestoreRequestId": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
-DescribeTagsMessageDescribeTagsPaginateTypeDef = TypedDict(
-    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
-    {
-        "ResourceName": str,
-        "ResourceType": str,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTagsMessageRequestTypeDef = TypedDict(
     "DescribeTagsMessageRequestTypeDef",
     {
         "ResourceName": str,
         "ResourceType": str,
         "MaxRecords": int,
         "Marker": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
     },
     total=False,
 )
 
-DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = TypedDict(
-    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
-    {
-        "UsageLimitId": str,
-        "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "TagKeys": Sequence[str],
-        "TagValues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeUsageLimitsMessageRequestTypeDef = TypedDict(
     "DescribeUsageLimitsMessageRequestTypeDef",
     {
         "UsageLimitId": str,
         "ClusterIdentifier": str,
         "FeatureType": UsageLimitFeatureTypeType,
         "MaxRecords": int,
@@ -1905,26 +1559,21 @@
         "DisassociateEntireAccount": bool,
         "ConsumerArn": str,
         "ConsumerRegion": str,
     },
     total=False,
 )
 
+
 class DisassociateDataShareConsumerMessageRequestTypeDef(
     _RequiredDisassociateDataShareConsumerMessageRequestTypeDef,
     _OptionalDisassociateDataShareConsumerMessageRequestTypeDef,
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredEnableLoggingMessageRequestTypeDef = TypedDict(
     "_RequiredEnableLoggingMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
@@ -1935,19 +1584,21 @@
         "S3KeyPrefix": str,
         "LogDestinationType": LogDestinationTypeType,
         "LogExports": Sequence[str],
     },
     total=False,
 )
 
+
 class EnableLoggingMessageRequestTypeDef(
     _RequiredEnableLoggingMessageRequestTypeDef, _OptionalEnableLoggingMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredEnableSnapshotCopyMessageRequestTypeDef = TypedDict(
     "_RequiredEnableSnapshotCopyMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "DestinationRegion": str,
     },
 )
@@ -1957,20 +1608,22 @@
         "RetentionPeriod": int,
         "SnapshotCopyGrantName": str,
         "ManualSnapshotRetentionPeriod": int,
     },
     total=False,
 )
 
+
 class EnableSnapshotCopyMessageRequestTypeDef(
     _RequiredEnableSnapshotCopyMessageRequestTypeDef,
     _OptionalEnableSnapshotCopyMessageRequestTypeDef,
 ):
     pass
 
+
 EndpointAuthorizationTypeDef = TypedDict(
     "EndpointAuthorizationTypeDef",
     {
         "Grantor": str,
         "Grantee": str,
         "ClusterIdentifier": str,
         "AuthorizeTime": datetime,
@@ -1979,30 +1632,14 @@
         "AllowedAllVPCs": bool,
         "AllowedVPCs": List[str],
         "EndpointCount": int,
     },
     total=False,
 )
 
-EndpointAuthorizationResponseMetadataTypeDef = TypedDict(
-    "EndpointAuthorizationResponseMetadataTypeDef",
-    {
-        "Grantor": str,
-        "Grantee": str,
-        "ClusterIdentifier": str,
-        "AuthorizeTime": datetime,
-        "ClusterStatus": str,
-        "Status": AuthorizationStatusType,
-        "AllowedAllVPCs": bool,
-        "AllowedVPCs": List[str],
-        "EndpointCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventInfoMapTypeDef = TypedDict(
     "EventInfoMapTypeDef",
     {
         "EventId": str,
         "EventCategories": List[str],
         "EventDescription": str,
         "Severity": str,
@@ -2039,53 +1676,33 @@
         "AutoCreate": bool,
         "DbGroups": Sequence[str],
         "CustomDomainName": str,
     },
     total=False,
 )
 
+
 class GetClusterCredentialsMessageRequestTypeDef(
     _RequiredGetClusterCredentialsMessageRequestTypeDef,
     _OptionalGetClusterCredentialsMessageRequestTypeDef,
 ):
     pass
 
+
 GetClusterCredentialsWithIAMMessageRequestTypeDef = TypedDict(
     "GetClusterCredentialsWithIAMMessageRequestTypeDef",
     {
         "DbName": str,
         "ClusterIdentifier": str,
         "DurationSeconds": int,
         "CustomDomainName": str,
     },
     total=False,
 )
 
-_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
-    "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    {
-        "ActionType": ReservedNodeExchangeActionTypeType,
-    },
-)
-_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
-    "_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "SnapshotIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef(
-    _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-    _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef = TypedDict(
     "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef",
     {
         "ActionType": ReservedNodeExchangeActionTypeType,
     },
 )
 _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef = TypedDict(
@@ -2095,39 +1712,21 @@
         "SnapshotIdentifier": str,
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef(
     _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
     _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
 ):
     pass
 
-_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
-    "_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
-    {
-        "ReservedNodeId": str,
-    },
-)
-_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
-    "_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef(
-    _RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
-    _OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
-):
-    pass
 
 _RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef = TypedDict(
     "_RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
     {
         "ReservedNodeId": str,
     },
 )
@@ -2136,34 +1735,21 @@
     {
         "MaxRecords": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef(
     _RequiredGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
     _OptionalGetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
 ):
     pass
 
-LoggingStatusTypeDef = TypedDict(
-    "LoggingStatusTypeDef",
-    {
-        "LoggingEnabled": bool,
-        "BucketName": str,
-        "S3KeyPrefix": str,
-        "LastSuccessfulDeliveryTime": datetime,
-        "LastFailureTime": datetime,
-        "LastFailureMessage": str,
-        "LogDestinationType": LogDestinationTypeType,
-        "LogExports": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredModifyAquaInputMessageRequestTypeDef = TypedDict(
     "_RequiredModifyAquaInputMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
@@ -2171,36 +1757,29 @@
     "_OptionalModifyAquaInputMessageRequestTypeDef",
     {
         "AquaConfigurationStatus": AquaConfigurationStatusType,
     },
     total=False,
 )
 
+
 class ModifyAquaInputMessageRequestTypeDef(
     _RequiredModifyAquaInputMessageRequestTypeDef, _OptionalModifyAquaInputMessageRequestTypeDef
 ):
     pass
 
+
 ModifyAuthenticationProfileMessageRequestTypeDef = TypedDict(
     "ModifyAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
-ModifyAuthenticationProfileResultTypeDef = TypedDict(
-    "ModifyAuthenticationProfileResultTypeDef",
-    {
-        "AuthenticationProfileName": str,
-        "AuthenticationProfileContent": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ModifyClusterDbRevisionMessageRequestTypeDef = TypedDict(
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "RevisionTarget": str,
     },
 )
@@ -2217,43 +1796,21 @@
         "AddIamRoles": Sequence[str],
         "RemoveIamRoles": Sequence[str],
         "DefaultIamRoleArn": str,
     },
     total=False,
 )
 
+
 class ModifyClusterIamRolesMessageRequestTypeDef(
     _RequiredModifyClusterIamRolesMessageRequestTypeDef,
     _OptionalModifyClusterIamRolesMessageRequestTypeDef,
 ):
     pass
 
-_RequiredModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
-    "_RequiredModifyClusterMaintenanceMessageRequestTypeDef",
-    {
-        "ClusterIdentifier": str,
-    },
-)
-_OptionalModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
-    "_OptionalModifyClusterMaintenanceMessageRequestTypeDef",
-    {
-        "DeferMaintenance": bool,
-        "DeferMaintenanceIdentifier": str,
-        "DeferMaintenanceStartTime": Union[datetime, str],
-        "DeferMaintenanceEndTime": Union[datetime, str],
-        "DeferMaintenanceDuration": int,
-    },
-    total=False,
-)
-
-class ModifyClusterMaintenanceMessageRequestTypeDef(
-    _RequiredModifyClusterMaintenanceMessageRequestTypeDef,
-    _OptionalModifyClusterMaintenanceMessageRequestTypeDef,
-):
-    pass
 
 _RequiredModifyClusterMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
@@ -2284,19 +1841,21 @@
         "AvailabilityZoneRelocation": bool,
         "AvailabilityZone": str,
         "Port": int,
     },
     total=False,
 )
 
+
 class ModifyClusterMessageRequestTypeDef(
     _RequiredModifyClusterMessageRequestTypeDef, _OptionalModifyClusterMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredModifyClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotIdentifier": str,
     },
 )
 _OptionalModifyClusterSnapshotMessageRequestTypeDef = TypedDict(
@@ -2304,20 +1863,22 @@
     {
         "ManualSnapshotRetentionPeriod": int,
         "Force": bool,
     },
     total=False,
 )
 
+
 class ModifyClusterSnapshotMessageRequestTypeDef(
     _RequiredModifyClusterSnapshotMessageRequestTypeDef,
     _OptionalModifyClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyClusterSnapshotScheduleMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSnapshotScheduleMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyClusterSnapshotScheduleMessageRequestTypeDef = TypedDict(
@@ -2325,20 +1886,22 @@
     {
         "ScheduleIdentifier": str,
         "DisassociateSchedule": bool,
     },
     total=False,
 )
 
+
 class ModifyClusterSnapshotScheduleMessageRequestTypeDef(
     _RequiredModifyClusterSnapshotScheduleMessageRequestTypeDef,
     _OptionalModifyClusterSnapshotScheduleMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -2346,20 +1909,22 @@
     "_OptionalModifyClusterSubnetGroupMessageRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class ModifyClusterSubnetGroupMessageRequestTypeDef(
     _RequiredModifyClusterSubnetGroupMessageRequestTypeDef,
     _OptionalModifyClusterSubnetGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyCustomDomainAssociationMessageRequestTypeDef = TypedDict(
     "_RequiredModifyCustomDomainAssociationMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalModifyCustomDomainAssociationMessageRequestTypeDef = TypedDict(
@@ -2367,30 +1932,21 @@
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
     },
     total=False,
 )
 
+
 class ModifyCustomDomainAssociationMessageRequestTypeDef(
     _RequiredModifyCustomDomainAssociationMessageRequestTypeDef,
     _OptionalModifyCustomDomainAssociationMessageRequestTypeDef,
 ):
     pass
 
-ModifyCustomDomainAssociationResultTypeDef = TypedDict(
-    "ModifyCustomDomainAssociationResultTypeDef",
-    {
-        "CustomDomainName": str,
-        "CustomDomainCertificateArn": str,
-        "ClusterIdentifier": str,
-        "CustomDomainCertExpiryTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredModifyEndpointAccessMessageRequestTypeDef = TypedDict(
     "_RequiredModifyEndpointAccessMessageRequestTypeDef",
     {
         "EndpointName": str,
     },
 )
@@ -2398,20 +1954,22 @@
     "_OptionalModifyEndpointAccessMessageRequestTypeDef",
     {
         "VpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyEndpointAccessMessageRequestTypeDef(
     _RequiredModifyEndpointAccessMessageRequestTypeDef,
     _OptionalModifyEndpointAccessMessageRequestTypeDef,
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
@@ -2423,20 +1981,22 @@
         "EventCategories": Sequence[str],
         "Severity": str,
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
 _RequiredModifySnapshotCopyRetentionPeriodMessageRequestTypeDef = TypedDict(
     "_RequiredModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "RetentionPeriod": int,
     },
 )
@@ -2444,20 +2004,22 @@
     "_OptionalModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     {
         "Manual": bool,
     },
     total=False,
 )
 
+
 class ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef(
     _RequiredModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     _OptionalModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
 ):
     pass
 
+
 ModifySnapshotScheduleMessageRequestTypeDef = TypedDict(
     "ModifySnapshotScheduleMessageRequestTypeDef",
     {
         "ScheduleIdentifier": str,
         "ScheduleDefinitions": Sequence[str],
     },
 )
@@ -2473,19 +2035,21 @@
     {
         "Amount": int,
         "BreachAction": UsageLimitBreachActionType,
     },
     total=False,
 )
 
+
 class ModifyUsageLimitMessageRequestTypeDef(
     _RequiredModifyUsageLimitMessageRequestTypeDef, _OptionalModifyUsageLimitMessageRequestTypeDef
 ):
     pass
 
+
 NetworkInterfaceTypeDef = TypedDict(
     "NetworkInterfaceTypeDef",
     {
         "NetworkInterfaceId": str,
         "SubnetId": str,
         "PrivateIpAddress": str,
         "AvailabilityZone": str,
@@ -2500,43 +2064,24 @@
         "NumberOfNodes": int,
         "EstimatedDiskUtilizationPercent": float,
         "Mode": ModeType,
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
 PartnerIntegrationInputMessageRequestTypeDef = TypedDict(
     "PartnerIntegrationInputMessageRequestTypeDef",
     {
         "AccountId": str,
         "ClusterIdentifier": str,
         "DatabaseName": str,
         "PartnerName": str,
     },
 )
 
-PartnerIntegrationOutputMessageTypeDef = TypedDict(
-    "PartnerIntegrationOutputMessageTypeDef",
-    {
-        "DatabaseName": str,
-        "PartnerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PauseClusterMessageRequestTypeDef = TypedDict(
     "PauseClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2557,20 +2102,22 @@
     "_OptionalPurchaseReservedNodeOfferingMessageRequestTypeDef",
     {
         "NodeCount": int,
     },
     total=False,
 )
 
+
 class PurchaseReservedNodeOfferingMessageRequestTypeDef(
     _RequiredPurchaseReservedNodeOfferingMessageRequestTypeDef,
     _OptionalPurchaseReservedNodeOfferingMessageRequestTypeDef,
 ):
     pass
 
+
 RebootClusterMessageRequestTypeDef = TypedDict(
     "RebootClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2605,19 +2152,21 @@
         "Classic": bool,
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
     },
     total=False,
 )
 
+
 class ResizeClusterMessageRequestTypeDef(
     _RequiredResizeClusterMessageRequestTypeDef, _OptionalResizeClusterMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredResizeClusterMessageTypeDef = TypedDict(
     "_RequiredResizeClusterMessageTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalResizeClusterMessageTypeDef = TypedDict(
@@ -2629,52 +2178,20 @@
         "Classic": bool,
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
     },
     total=False,
 )
 
+
 class ResizeClusterMessageTypeDef(
     _RequiredResizeClusterMessageTypeDef, _OptionalResizeClusterMessageTypeDef
 ):
     pass
 
-ResizeProgressMessageTypeDef = TypedDict(
-    "ResizeProgressMessageTypeDef",
-    {
-        "TargetNodeType": str,
-        "TargetNumberOfNodes": int,
-        "TargetClusterType": str,
-        "Status": str,
-        "ImportTablesCompleted": List[str],
-        "ImportTablesInProgress": List[str],
-        "ImportTablesNotStarted": List[str],
-        "AvgResizeRateInMegaBytesPerSecond": float,
-        "TotalResizeDataInMegaBytes": int,
-        "ProgressInMegaBytes": int,
-        "ElapsedTimeInSeconds": int,
-        "EstimatedTimeToCompletionInSeconds": int,
-        "ResizeType": str,
-        "Message": str,
-        "TargetEncryptionType": str,
-        "DataTransferProgressPercent": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 
 _RequiredRestoreFromClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreFromClusterSnapshotMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
@@ -2713,20 +2230,22 @@
         "ReservedNodeId": str,
         "TargetReservedNodeOfferingId": str,
         "Encrypted": bool,
     },
     total=False,
 )
 
+
 class RestoreFromClusterSnapshotMessageRequestTypeDef(
     _RequiredRestoreFromClusterSnapshotMessageRequestTypeDef,
     _OptionalRestoreFromClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredRestoreTableFromClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredRestoreTableFromClusterSnapshotMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SourceDatabaseName": str,
         "SourceTableName": str,
@@ -2740,20 +2259,22 @@
         "TargetDatabaseName": str,
         "TargetSchemaName": str,
         "EnableCaseSensitiveIdentifier": bool,
     },
     total=False,
 )
 
+
 class RestoreTableFromClusterSnapshotMessageRequestTypeDef(
     _RequiredRestoreTableFromClusterSnapshotMessageRequestTypeDef,
     _OptionalRestoreTableFromClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 TableRestoreStatusTypeDef = TypedDict(
     "TableRestoreStatusTypeDef",
     {
         "TableRestoreRequestId": str,
         "Status": TableRestoreStatusTypeType,
         "Message": str,
         "RequestTime": datetime,
@@ -2797,20 +2318,22 @@
         "CIDRIP": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+
 class RevokeClusterSecurityGroupIngressMessageRequestTypeDef(
     _RequiredRevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     _OptionalRevokeClusterSecurityGroupIngressMessageRequestTypeDef,
 ):
     pass
 
+
 RevokeEndpointAccessMessageRequestTypeDef = TypedDict(
     "RevokeEndpointAccessMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "Account": str,
         "VpcIds": Sequence[str],
         "Force": bool,
@@ -2830,20 +2353,22 @@
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotClusterIdentifier": str,
     },
     total=False,
 )
 
+
 class RevokeSnapshotAccessMessageRequestTypeDef(
     _RequiredRevokeSnapshotAccessMessageRequestTypeDef,
     _OptionalRevokeSnapshotAccessMessageRequestTypeDef,
 ):
     pass
 
+
 RotateEncryptionKeyMessageRequestTypeDef = TypedDict(
     "RotateEncryptionKeyMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2869,34 +2394,193 @@
     "_OptionalUpdatePartnerStatusInputMessageRequestTypeDef",
     {
         "StatusMessage": str,
     },
     total=False,
 )
 
+
 class UpdatePartnerStatusInputMessageRequestTypeDef(
     _RequiredUpdatePartnerStatusInputMessageRequestTypeDef,
     _OptionalUpdatePartnerStatusInputMessageRequestTypeDef,
 ):
     pass
 
+
+ClusterCredentialsTypeDef = TypedDict(
+    "ClusterCredentialsTypeDef",
+    {
+        "DbUser": str,
+        "DbPassword": str,
+        "Expiration": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterExtendedCredentialsTypeDef = TypedDict(
+    "ClusterExtendedCredentialsTypeDef",
+    {
+        "DbUser": str,
+        "DbPassword": str,
+        "Expiration": datetime,
+        "NextRefreshTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterParameterGroupNameMessageTypeDef = TypedDict(
+    "ClusterParameterGroupNameMessageTypeDef",
+    {
+        "ParameterGroupName": str,
+        "ParameterGroupStatus": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthenticationProfileResultTypeDef = TypedDict(
+    "CreateAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "AuthenticationProfileContent": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomDomainAssociationResultTypeDef = TypedDict(
+    "CreateCustomDomainAssociationResultTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+        "CustomDomainCertExpiryTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CustomerStorageMessageTypeDef = TypedDict(
+    "CustomerStorageMessageTypeDef",
+    {
+        "TotalBackupSizeInMegaBytes": float,
+        "TotalProvisionedStorageInMegaBytes": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAuthenticationProfileResultTypeDef = TypedDict(
+    "DeleteAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
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
+EndpointAuthorizationResponseTypeDef = TypedDict(
+    "EndpointAuthorizationResponseTypeDef",
+    {
+        "Grantor": str,
+        "Grantee": str,
+        "ClusterIdentifier": str,
+        "AuthorizeTime": datetime,
+        "ClusterStatus": str,
+        "Status": AuthorizationStatusType,
+        "AllowedAllVPCs": bool,
+        "AllowedVPCs": List[str],
+        "EndpointCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoggingStatusTypeDef = TypedDict(
+    "LoggingStatusTypeDef",
+    {
+        "LoggingEnabled": bool,
+        "BucketName": str,
+        "S3KeyPrefix": str,
+        "LastSuccessfulDeliveryTime": datetime,
+        "LastFailureTime": datetime,
+        "LastFailureMessage": str,
+        "LogDestinationType": LogDestinationTypeType,
+        "LogExports": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyAuthenticationProfileResultTypeDef = TypedDict(
+    "ModifyAuthenticationProfileResultTypeDef",
+    {
+        "AuthenticationProfileName": str,
+        "AuthenticationProfileContent": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyCustomDomainAssociationResultTypeDef = TypedDict(
+    "ModifyCustomDomainAssociationResultTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "ClusterIdentifier": str,
+        "CustomDomainCertExpiryTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PartnerIntegrationOutputMessageTypeDef = TypedDict(
+    "PartnerIntegrationOutputMessageTypeDef",
+    {
+        "DatabaseName": str,
+        "PartnerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResizeProgressMessageTypeDef = TypedDict(
+    "ResizeProgressMessageTypeDef",
+    {
+        "TargetNodeType": str,
+        "TargetNumberOfNodes": int,
+        "TargetClusterType": str,
+        "Status": str,
+        "ImportTablesCompleted": List[str],
+        "ImportTablesInProgress": List[str],
+        "ImportTablesNotStarted": List[str],
+        "AvgResizeRateInMegaBytesPerSecond": float,
+        "TotalResizeDataInMegaBytes": int,
+        "ProgressInMegaBytes": int,
+        "ElapsedTimeInSeconds": int,
+        "EstimatedTimeToCompletionInSeconds": int,
+        "ResizeType": str,
+        "Message": str,
+        "TargetEncryptionType": str,
+        "DataTransferProgressPercent": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AccountAttributeTypeDef = TypedDict(
     "AccountAttributeTypeDef",
     {
         "AttributeName": str,
         "AttributeValues": List[AttributeValueTargetTypeDef],
     },
     total=False,
 )
 
 ModifyAquaOutputMessageTypeDef = TypedDict(
     "ModifyAquaOutputMessageTypeDef",
     {
         "AquaConfiguration": AquaConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociationTypeDef = TypedDict(
     "AssociationTypeDef",
     {
         "CustomDomainCertificateArn": str,
@@ -2906,15 +2590,15 @@
     total=False,
 )
 
 DescribeAuthenticationProfilesResultTypeDef = TypedDict(
     "DescribeAuthenticationProfilesResultTypeDef",
     {
         "AuthenticationProfiles": List[AuthenticationProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "Name": str,
@@ -2931,24 +2615,24 @@
 )
 
 BatchDeleteClusterSnapshotsResultTypeDef = TypedDict(
     "BatchDeleteClusterSnapshotsResultTypeDef",
     {
         "Resources": List[str],
         "Errors": List[SnapshotErrorMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchModifyClusterSnapshotsOutputMessageTypeDef = TypedDict(
     "BatchModifyClusterSnapshotsOutputMessageTypeDef",
     {
         "Resources": List[str],
         "Errors": List[SnapshotErrorMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterDbRevisionTypeDef = TypedDict(
     "ClusterDbRevisionTypeDef",
     {
         "ClusterIdentifier": str,
@@ -2960,15 +2644,15 @@
 )
 
 ClusterParameterGroupDetailsTypeDef = TypedDict(
     "ClusterParameterGroupDetailsTypeDef",
     {
         "Parameters": List[ParameterTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefaultClusterParametersTypeDef = TypedDict(
     "DefaultClusterParametersTypeDef",
     {
         "ParameterGroupFamily": str,
@@ -2997,20 +2681,22 @@
     {
         "ResetAllParameters": bool,
         "Parameters": Sequence[ParameterTypeDef],
     },
     total=False,
 )
 
+
 class ResetClusterParameterGroupMessageRequestTypeDef(
     _RequiredResetClusterParameterGroupMessageRequestTypeDef,
     _OptionalResetClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 ClusterParameterGroupStatusTypeDef = TypedDict(
     "ClusterParameterGroupStatusTypeDef",
     {
         "ParameterGroupName": str,
         "ParameterApplyStatus": str,
         "ClusterParameterStatusList": List[ClusterParameterStatusTypeDef],
     },
@@ -3070,19 +2756,21 @@
         "AquaConfigurationStatus": AquaConfigurationStatusType,
         "DefaultIamRoleArn": str,
         "LoadSampleData": str,
     },
     total=False,
 )
 
+
 class CreateClusterMessageRequestTypeDef(
     _RequiredCreateClusterMessageRequestTypeDef, _OptionalCreateClusterMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateClusterParameterGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterParameterGroupMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
         "ParameterGroupFamily": str,
         "Description": str,
     },
@@ -3091,20 +2779,22 @@
     "_OptionalCreateClusterParameterGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateClusterParameterGroupMessageRequestTypeDef(
     _RequiredCreateClusterParameterGroupMessageRequestTypeDef,
     _OptionalCreateClusterParameterGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateClusterSecurityGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSecurityGroupMessageRequestTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Description": str,
     },
 )
@@ -3112,20 +2802,22 @@
     "_OptionalCreateClusterSecurityGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateClusterSecurityGroupMessageRequestTypeDef(
     _RequiredCreateClusterSecurityGroupMessageRequestTypeDef,
     _OptionalCreateClusterSecurityGroupMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotIdentifier": str,
         "ClusterIdentifier": str,
     },
 )
@@ -3134,20 +2826,22 @@
     {
         "ManualSnapshotRetentionPeriod": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateClusterSnapshotMessageRequestTypeDef(
     _RequiredCreateClusterSnapshotMessageRequestTypeDef,
     _OptionalCreateClusterSnapshotMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateClusterSubnetGroupMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSubnetGroupMessageRequestTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "Description": str,
         "SubnetIds": Sequence[str],
     },
@@ -3156,20 +2850,22 @@
     "_OptionalCreateClusterSubnetGroupMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateClusterSubnetGroupMessageRequestTypeDef(
     _RequiredCreateClusterSubnetGroupMessageRequestTypeDef,
     _OptionalCreateClusterSubnetGroupMessageRequestTypeDef,
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
@@ -3182,40 +2878,44 @@
         "Severity": str,
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
 _RequiredCreateHsmClientCertificateMessageRequestTypeDef = TypedDict(
     "_RequiredCreateHsmClientCertificateMessageRequestTypeDef",
     {
         "HsmClientCertificateIdentifier": str,
     },
 )
 _OptionalCreateHsmClientCertificateMessageRequestTypeDef = TypedDict(
     "_OptionalCreateHsmClientCertificateMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateHsmClientCertificateMessageRequestTypeDef(
     _RequiredCreateHsmClientCertificateMessageRequestTypeDef,
     _OptionalCreateHsmClientCertificateMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateHsmConfigurationMessageRequestTypeDef = TypedDict(
     "_RequiredCreateHsmConfigurationMessageRequestTypeDef",
     {
         "HsmConfigurationIdentifier": str,
         "Description": str,
         "HsmIpAddress": str,
         "HsmPartitionName": str,
@@ -3227,20 +2927,22 @@
     "_OptionalCreateHsmConfigurationMessageRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateHsmConfigurationMessageRequestTypeDef(
     _RequiredCreateHsmConfigurationMessageRequestTypeDef,
     _OptionalCreateHsmConfigurationMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSnapshotCopyGrantMessageRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotCopyGrantMessageRequestTypeDef",
     {
         "SnapshotCopyGrantName": str,
     },
 )
 _OptionalCreateSnapshotCopyGrantMessageRequestTypeDef = TypedDict(
@@ -3248,20 +2950,22 @@
     {
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSnapshotCopyGrantMessageRequestTypeDef(
     _RequiredCreateSnapshotCopyGrantMessageRequestTypeDef,
     _OptionalCreateSnapshotCopyGrantMessageRequestTypeDef,
 ):
     pass
 
+
 CreateSnapshotScheduleMessageRequestTypeDef = TypedDict(
     "CreateSnapshotScheduleMessageRequestTypeDef",
     {
         "ScheduleDefinitions": Sequence[str],
         "ScheduleIdentifier": str,
         "ScheduleDescription": str,
         "Tags": Sequence[TagTypeDef],
@@ -3294,19 +2998,21 @@
         "Period": UsageLimitPeriodType,
         "BreachAction": UsageLimitBreachActionType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateUsageLimitMessageRequestTypeDef(
     _RequiredCreateUsageLimitMessageRequestTypeDef, _OptionalCreateUsageLimitMessageRequestTypeDef
 ):
     pass
 
+
 EC2SecurityGroupTypeDef = TypedDict(
     "EC2SecurityGroupTypeDef",
     {
         "Status": str,
         "EC2SecurityGroupName": str,
         "EC2SecurityGroupOwnerId": str,
         "Tags": List[TagTypeDef],
@@ -3370,25 +3076,25 @@
         "SnapshotCopyGrantName": str,
         "KmsKeyId": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-SnapshotScheduleResponseMetadataTypeDef = TypedDict(
-    "SnapshotScheduleResponseMetadataTypeDef",
+SnapshotScheduleResponseTypeDef = TypedDict(
+    "SnapshotScheduleResponseTypeDef",
     {
         "ScheduleDefinitions": List[str],
         "ScheduleIdentifier": str,
         "ScheduleDescription": str,
         "Tags": List[TagTypeDef],
         "NextInvocations": List[datetime],
         "AssociatedClusterCount": int,
         "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SnapshotScheduleTypeDef = TypedDict(
     "SnapshotScheduleTypeDef",
     {
         "ScheduleDefinitions": List[str],
@@ -3449,26 +3155,26 @@
         "Tag": TagTypeDef,
         "ResourceName": str,
         "ResourceType": str,
     },
     total=False,
 )
 
-UsageLimitResponseMetadataTypeDef = TypedDict(
-    "UsageLimitResponseMetadataTypeDef",
+UsageLimitResponseTypeDef = TypedDict(
+    "UsageLimitResponseTypeDef",
     {
         "UsageLimitId": str,
         "ClusterIdentifier": str,
         "FeatureType": UsageLimitFeatureTypeType,
         "LimitType": UsageLimitLimitTypeType,
         "Amount": int,
         "Period": UsageLimitPeriodType,
         "BreachAction": UsageLimitBreachActionType,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UsageLimitTypeDef = TypedDict(
     "UsageLimitTypeDef",
     {
         "UsageLimitId": str,
@@ -3484,36 +3190,76 @@
 )
 
 DescribeReservedNodeExchangeStatusOutputMessageTypeDef = TypedDict(
     "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
     {
         "ReservedNodeExchangeStatusDetails": List[ReservedNodeExchangeStatusTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterVersionsMessageTypeDef = TypedDict(
     "ClusterVersionsMessageTypeDef",
     {
         "Marker": str,
         "ClusterVersions": List[ClusterVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
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
+        "MaxRecords": int,
+        "Marker": str,
     },
+    total=False,
 )
 
-DataShareResponseMetadataTypeDef = TypedDict(
-    "DataShareResponseMetadataTypeDef",
+_RequiredModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
+    "_RequiredModifyClusterMaintenanceMessageRequestTypeDef",
+    {
+        "ClusterIdentifier": str,
+    },
+)
+_OptionalModifyClusterMaintenanceMessageRequestTypeDef = TypedDict(
+    "_OptionalModifyClusterMaintenanceMessageRequestTypeDef",
+    {
+        "DeferMaintenance": bool,
+        "DeferMaintenanceIdentifier": str,
+        "DeferMaintenanceStartTime": TimestampTypeDef,
+        "DeferMaintenanceEndTime": TimestampTypeDef,
+        "DeferMaintenanceDuration": int,
+    },
+    total=False,
+)
+
+
+class ModifyClusterMaintenanceMessageRequestTypeDef(
+    _RequiredModifyClusterMaintenanceMessageRequestTypeDef,
+    _OptionalModifyClusterMaintenanceMessageRequestTypeDef,
+):
+    pass
+
+
+DataShareResponseTypeDef = TypedDict(
+    "DataShareResponseTypeDef",
     {
         "DataShareArn": str,
         "ProducerArn": str,
         "AllowPubliclyAccessibleConsumers": bool,
         "DataShareAssociations": List[DataShareAssociationTypeDef],
         "ManagedBy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataShareTypeDef = TypedDict(
     "DataShareTypeDef",
     {
         "DataShareArn": str,
@@ -3521,42 +3267,409 @@
         "AllowPubliclyAccessibleConsumers": bool,
         "DataShareAssociations": List[DataShareAssociationTypeDef],
         "ManagedBy": str,
     },
     total=False,
 )
 
+DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef = TypedDict(
+    "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+    },
+)
+_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef(
+    _RequiredDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+    _OptionalDescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+):
+    pass
+
+
+DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
+    {
+        "ClusterSecurityGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
+    {
+        "ClusterSubnetGroupName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef = TypedDict(
+    "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
+    {
+        "MaintenanceTrackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef = TypedDict(
+    "DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef",
+    {
+        "ClusterVersion": str,
+        "ClusterParameterGroupFamily": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClustersMessageDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersMessageDescribeClustersPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef = TypedDict(
+    "DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef",
+    {
+        "CustomDomainName": str,
+        "CustomDomainCertificateArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef = TypedDict(
+    "DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef",
+    {
+        "ConsumerArn": str,
+        "Status": DataShareStatusForConsumerType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef = TypedDict(
+    "DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef",
+    {
+        "ProducerArn": str,
+        "Status": DataShareStatusForProducerType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef = TypedDict(
+    "DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef",
+    {
+        "DataShareArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    {
+        "ParameterGroupFamily": str,
+    },
+)
+_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef(
+    _RequiredDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+    _OptionalDescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+):
+    pass
+
+
+DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef = TypedDict(
+    "DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ResourceOwner": str,
+        "EndpointName": str,
+        "VpcId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef = TypedDict(
+    "DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "Account": str,
+        "Grantee": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef = TypedDict(
+    "DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef",
+    {
+        "SubscriptionName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
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
+DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef = TypedDict(
+    "DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef",
+    {
+        "HsmClientCertificateIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef",
+    {
+        "HsmConfigurationIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef = TypedDict(
+    "DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef",
+    {
+        "ClusterVersion": str,
+        "NodeType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef = TypedDict(
+    "DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+        "ReservedNodeExchangeRequestId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef = TypedDict(
+    "DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef",
+    {
+        "ReservedNodeOfferingId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef = TypedDict(
+    "DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef",
+    {
+        "SnapshotCopyGrantName": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef = TypedDict(
+    "DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ScheduleIdentifier": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef = TypedDict(
+    "DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "TableRestoreRequestId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeTagsMessageDescribeTagsPaginateTypeDef = TypedDict(
+    "DescribeTagsMessageDescribeTagsPaginateTypeDef",
+    {
+        "ResourceName": str,
+        "ResourceType": str,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef = TypedDict(
+    "DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef",
+    {
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "TagKeys": Sequence[str],
+        "TagValues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
+    "_RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
+    {
+        "ActionType": ReservedNodeExchangeActionTypeType,
+    },
+)
+_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef = TypedDict(
+    "_OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "SnapshotIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef(
+    _RequiredGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+    _OptionalGetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
+    "_RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
+    {
+        "ReservedNodeId": str,
+    },
+)
+_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef = TypedDict(
+    "_OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef(
+    _RequiredGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
+    _OptionalGetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
+):
+    pass
+
+
 DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeClusterSnapshotsMessageRequestTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "MaxRecords": int,
         "Marker": str,
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
@@ -3567,16 +3680,16 @@
 DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef = TypedDict(
     "DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "SnapshotType": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "MaxRecords": int,
         "Marker": str,
         "OwnerAccount": str,
         "TagKeys": Sequence[str],
         "TagValues": Sequence[str],
         "ClusterExists": bool,
         "SortingEntities": Sequence[SnapshotSortingEntityTypeDef],
@@ -3634,25 +3747,27 @@
     "_OptionalDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef",
     {
         "ClusterIdentifier": str,
         "SnapshotIdentifier": str,
         "SnapshotArn": str,
         "OwnerAccount": str,
         "Filters": Sequence[NodeConfigurationOptionsFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef(
     _RequiredDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
     _OptionalDescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeNodeConfigurationOptionsMessageRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeConfigurationOptionsMessageRequestTypeDef",
     {
         "ActionType": ActionTypeType,
     },
 )
 _OptionalDescribeNodeConfigurationOptionsMessageRequestTypeDef = TypedDict(
@@ -3665,63 +3780,65 @@
         "Filters": Sequence[NodeConfigurationOptionsFilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
+
 class DescribeNodeConfigurationOptionsMessageRequestTypeDef(
     _RequiredDescribeNodeConfigurationOptionsMessageRequestTypeDef,
     _OptionalDescribeNodeConfigurationOptionsMessageRequestTypeDef,
 ):
     pass
 
+
 DescribePartnersOutputMessageTypeDef = TypedDict(
     "DescribePartnersOutputMessageTypeDef",
     {
         "PartnerIntegrationInfoList": List[PartnerIntegrationInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef = TypedDict(
     "DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef",
     {
         "ScheduledActionName": str,
         "TargetActionType": ScheduledActionTypeValuesType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Active": bool,
         "Filters": Sequence[ScheduledActionFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeScheduledActionsMessageRequestTypeDef = TypedDict(
     "DescribeScheduledActionsMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
         "TargetActionType": ScheduledActionTypeValuesType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Active": bool,
         "Filters": Sequence[ScheduledActionFilterTypeDef],
         "Marker": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
 EndpointAuthorizationListTypeDef = TypedDict(
     "EndpointAuthorizationListTypeDef",
     {
         "EndpointAuthorizationList": List[EndpointAuthorizationTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventCategoriesMapTypeDef = TypedDict(
     "EventCategoriesMapTypeDef",
     {
         "SourceType": str,
@@ -3731,15 +3848,15 @@
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
 
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "VpcEndpointId": str,
@@ -3750,15 +3867,15 @@
 )
 
 NodeConfigurationOptionsMessageTypeDef = TypedDict(
     "NodeConfigurationOptionsMessageTypeDef",
     {
         "NodeConfigurationOptionList": List[NodeConfigurationOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedNodeOfferingTypeDef = TypedDict(
     "ReservedNodeOfferingTypeDef",
     {
         "ReservedNodeOfferingId": str,
@@ -3794,24 +3911,24 @@
     total=False,
 )
 
 RestoreTableFromClusterSnapshotResultTypeDef = TypedDict(
     "RestoreTableFromClusterSnapshotResultTypeDef",
     {
         "TableRestoreStatus": TableRestoreStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TableRestoreStatusMessageTypeDef = TypedDict(
     "TableRestoreStatusMessageTypeDef",
     {
         "TableRestoreStatusDetails": List[TableRestoreStatusTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScheduledActionTypeTypeDef = TypedDict(
     "ScheduledActionTypeTypeDef",
     {
         "ResizeCluster": ResizeClusterMessageTypeDef,
@@ -3831,24 +3948,24 @@
     total=False,
 )
 
 AccountAttributeListTypeDef = TypedDict(
     "AccountAttributeListTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomDomainAssociationsMessageTypeDef = TypedDict(
     "CustomDomainAssociationsMessageTypeDef",
     {
         "Marker": str,
         "Associations": List[AssociationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OrderableClusterOptionTypeDef = TypedDict(
     "OrderableClusterOptionTypeDef",
     {
         "ClusterVersion": str,
@@ -3870,99 +3987,99 @@
 )
 
 ClusterDbRevisionsMessageTypeDef = TypedDict(
     "ClusterDbRevisionsMessageTypeDef",
     {
         "Marker": str,
         "ClusterDbRevisions": List[ClusterDbRevisionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDefaultClusterParametersResultTypeDef = TypedDict(
     "DescribeDefaultClusterParametersResultTypeDef",
     {
         "DefaultClusterParameters": DefaultClusterParametersTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterParameterGroupsMessageTypeDef = TypedDict(
     "ClusterParameterGroupsMessageTypeDef",
     {
         "Marker": str,
         "ParameterGroups": List[ClusterParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterParameterGroupResultTypeDef = TypedDict(
     "CreateClusterParameterGroupResultTypeDef",
     {
         "ClusterParameterGroup": ClusterParameterGroupTypeDef,
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
 
 CreateHsmClientCertificateResultTypeDef = TypedDict(
     "CreateHsmClientCertificateResultTypeDef",
     {
         "HsmClientCertificate": HsmClientCertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HsmClientCertificateMessageTypeDef = TypedDict(
     "HsmClientCertificateMessageTypeDef",
     {
         "Marker": str,
         "HsmClientCertificates": List[HsmClientCertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHsmConfigurationResultTypeDef = TypedDict(
     "CreateHsmConfigurationResultTypeDef",
     {
         "HsmConfiguration": HsmConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HsmConfigurationMessageTypeDef = TypedDict(
     "HsmConfigurationMessageTypeDef",
     {
         "Marker": str,
         "HsmConfigurations": List[HsmConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSecurityGroupTypeDef = TypedDict(
     "ClusterSecurityGroupTypeDef",
     {
         "ClusterSecurityGroupName": str,
@@ -3974,160 +4091,160 @@
     total=False,
 )
 
 CreateSnapshotCopyGrantResultTypeDef = TypedDict(
     "CreateSnapshotCopyGrantResultTypeDef",
     {
         "SnapshotCopyGrant": SnapshotCopyGrantTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SnapshotCopyGrantMessageTypeDef = TypedDict(
     "SnapshotCopyGrantMessageTypeDef",
     {
         "Marker": str,
         "SnapshotCopyGrants": List[SnapshotCopyGrantTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSnapshotSchedulesOutputMessageTypeDef = TypedDict(
     "DescribeSnapshotSchedulesOutputMessageTypeDef",
     {
         "SnapshotSchedules": List[SnapshotScheduleTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthorizeSnapshotAccessResultTypeDef = TypedDict(
     "AuthorizeSnapshotAccessResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopyClusterSnapshotResultTypeDef = TypedDict(
     "CopyClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSnapshotResultTypeDef = TypedDict(
     "CreateClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterSnapshotResultTypeDef = TypedDict(
     "DeleteClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterSnapshotResultTypeDef = TypedDict(
     "ModifyClusterSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RevokeSnapshotAccessResultTypeDef = TypedDict(
     "RevokeSnapshotAccessResultTypeDef",
     {
         "Snapshot": SnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SnapshotMessageTypeDef = TypedDict(
     "SnapshotMessageTypeDef",
     {
         "Marker": str,
         "Snapshots": List[SnapshotTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaggedResourceListMessageTypeDef = TypedDict(
     "TaggedResourceListMessageTypeDef",
     {
         "TaggedResources": List[TaggedResourceTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UsageLimitListTypeDef = TypedDict(
     "UsageLimitListTypeDef",
     {
         "UsageLimits": List[UsageLimitTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSharesForConsumerResultTypeDef = TypedDict(
     "DescribeDataSharesForConsumerResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSharesForProducerResultTypeDef = TypedDict(
     "DescribeDataSharesForProducerResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSharesResultTypeDef = TypedDict(
     "DescribeDataSharesResultTypeDef",
     {
         "DataShares": List[DataShareTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventCategoriesMessageTypeDef = TypedDict(
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointAccessResponseMetadataTypeDef = TypedDict(
-    "EndpointAccessResponseMetadataTypeDef",
+EndpointAccessResponseTypeDef = TypedDict(
+    "EndpointAccessResponseTypeDef",
     {
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "SubnetGroupName": str,
         "EndpointStatus": str,
         "EndpointName": str,
         "EndpointCreateTime": datetime,
         "Port": int,
         "Address": str,
         "VpcSecurityGroups": List[VpcSecurityGroupMembershipTypeDef],
         "VpcEndpoint": VpcEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointAccessTypeDef = TypedDict(
     "EndpointAccessTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4155,40 +4272,40 @@
 )
 
 GetReservedNodeExchangeOfferingsOutputMessageTypeDef = TypedDict(
     "GetReservedNodeExchangeOfferingsOutputMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeOfferings": List[ReservedNodeOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedNodeOfferingsMessageTypeDef = TypedDict(
     "ReservedNodeOfferingsMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeOfferings": List[ReservedNodeOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptReservedNodeExchangeOutputMessageTypeDef = TypedDict(
     "AcceptReservedNodeExchangeOutputMessageTypeDef",
     {
         "ExchangedReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PurchaseReservedNodeOfferingResultTypeDef = TypedDict(
     "PurchaseReservedNodeOfferingResultTypeDef",
     {
         "ReservedNode": ReservedNodeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservedNodeConfigurationOptionTypeDef = TypedDict(
     "ReservedNodeConfigurationOptionTypeDef",
     {
         "SourceReservedNode": ReservedNodeTypeDef,
@@ -4199,15 +4316,15 @@
 )
 
 ReservedNodesMessageTypeDef = TypedDict(
     "ReservedNodesMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodes": List[ReservedNodeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateScheduledActionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
@@ -4216,66 +4333,70 @@
         "IamRole": str,
     },
 )
 _OptionalCreateScheduledActionMessageRequestTypeDef = TypedDict(
     "_OptionalCreateScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionDescription": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Enable": bool,
     },
     total=False,
 )
 
+
 class CreateScheduledActionMessageRequestTypeDef(
     _RequiredCreateScheduledActionMessageRequestTypeDef,
     _OptionalCreateScheduledActionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyScheduledActionMessageRequestTypeDef = TypedDict(
     "_RequiredModifyScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
     },
 )
 _OptionalModifyScheduledActionMessageRequestTypeDef = TypedDict(
     "_OptionalModifyScheduledActionMessageRequestTypeDef",
     {
         "TargetAction": ScheduledActionTypeTypeDef,
         "Schedule": str,
         "IamRole": str,
         "ScheduledActionDescription": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Enable": bool,
     },
     total=False,
 )
 
+
 class ModifyScheduledActionMessageRequestTypeDef(
     _RequiredModifyScheduledActionMessageRequestTypeDef,
     _OptionalModifyScheduledActionMessageRequestTypeDef,
 ):
     pass
 
-ScheduledActionResponseMetadataTypeDef = TypedDict(
-    "ScheduledActionResponseMetadataTypeDef",
+
+ScheduledActionResponseTypeDef = TypedDict(
+    "ScheduledActionResponseTypeDef",
     {
         "ScheduledActionName": str,
         "TargetAction": ScheduledActionTypeTypeDef,
         "Schedule": str,
         "IamRole": str,
         "ScheduledActionDescription": str,
         "State": ScheduledActionStateType,
         "NextInvocations": List[datetime],
         "StartTime": datetime,
         "EndTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScheduledActionTypeDef = TypedDict(
     "ScheduledActionTypeDef",
     {
         "ScheduledActionName": str,
@@ -4302,15 +4423,15 @@
 )
 
 OrderableClusterOptionsMessageTypeDef = TypedDict(
     "OrderableClusterOptionsMessageTypeDef",
     {
         "OrderableClusterOptions": List[OrderableClusterOptionTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSubnetGroupTypeDef = TypedDict(
     "ClusterSubnetGroupTypeDef",
     {
         "ClusterSubnetGroupName": str,
@@ -4323,49 +4444,49 @@
     total=False,
 )
 
 AuthorizeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSecurityGroupMessageTypeDef = TypedDict(
     "ClusterSecurityGroupMessageTypeDef",
     {
         "Marker": str,
         "ClusterSecurityGroups": List[ClusterSecurityGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSecurityGroupResultTypeDef = TypedDict(
     "CreateClusterSecurityGroupResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RevokeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "RevokeClusterSecurityGroupIngressResultTypeDef",
     {
         "ClusterSecurityGroup": ClusterSecurityGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EndpointAccessListTypeDef = TypedDict(
     "EndpointAccessListTypeDef",
     {
         "EndpointAccessList": List[EndpointAccessTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ClusterIdentifier": str,
@@ -4428,182 +4549,182 @@
 )
 
 GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef = TypedDict(
     "GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef",
     {
         "Marker": str,
         "ReservedNodeConfigurationOptionList": List[ReservedNodeConfigurationOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScheduledActionsMessageTypeDef = TypedDict(
     "ScheduledActionsMessageTypeDef",
     {
         "Marker": str,
         "ScheduledActions": List[ScheduledActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TrackListMessageTypeDef = TypedDict(
     "TrackListMessageTypeDef",
     {
         "MaintenanceTracks": List[MaintenanceTrackTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterSubnetGroupMessageTypeDef = TypedDict(
     "ClusterSubnetGroupMessageTypeDef",
     {
         "Marker": str,
         "ClusterSubnetGroups": List[ClusterSubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSubnetGroupResultTypeDef = TypedDict(
     "CreateClusterSubnetGroupResultTypeDef",
     {
         "ClusterSubnetGroup": ClusterSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterSubnetGroupResultTypeDef = TypedDict(
     "ModifyClusterSubnetGroupResultTypeDef",
     {
         "ClusterSubnetGroup": ClusterSubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClustersMessageTypeDef = TypedDict(
     "ClustersMessageTypeDef",
     {
         "Marker": str,
         "Clusters": List[ClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResultTypeDef = TypedDict(
     "DeleteClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisableSnapshotCopyResultTypeDef = TypedDict(
     "DisableSnapshotCopyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableSnapshotCopyResultTypeDef = TypedDict(
     "EnableSnapshotCopyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterDbRevisionResultTypeDef = TypedDict(
     "ModifyClusterDbRevisionResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterIamRolesResultTypeDef = TypedDict(
     "ModifyClusterIamRolesResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterMaintenanceResultTypeDef = TypedDict(
     "ModifyClusterMaintenanceResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterResultTypeDef = TypedDict(
     "ModifyClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifySnapshotCopyRetentionPeriodResultTypeDef = TypedDict(
     "ModifySnapshotCopyRetentionPeriodResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PauseClusterResultTypeDef = TypedDict(
     "PauseClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootClusterResultTypeDef = TypedDict(
     "RebootClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResizeClusterResultTypeDef = TypedDict(
     "ResizeClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreFromClusterSnapshotResultTypeDef = TypedDict(
     "RestoreFromClusterSnapshotResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResumeClusterResultTypeDef = TypedDict(
     "ResumeClusterResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RotateEncryptionKeyResultTypeDef = TypedDict(
     "RotateEncryptionKeyResultTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/waiter.py` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/waiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,19 @@
 
         cluster_available_waiter: ClusterAvailableWaiter = client.get_waiter("cluster_available")
         cluster_deleted_waiter: ClusterDeletedWaiter = client.get_waiter("cluster_deleted")
         cluster_restored_waiter: ClusterRestoredWaiter = client.get_waiter("cluster_restored")
         snapshot_available_waiter: SnapshotAvailableWaiter = client.get_waiter("snapshot_available")
     ```
 """
-from datetime import datetime
-from typing import Sequence, Union
+from typing import Sequence
 
 from aiobotocore.waiter import AIOWaiter
 
-from .type_defs import SnapshotSortingEntityTypeDef, WaiterConfigTypeDef
+from .type_defs import SnapshotSortingEntityTypeDef, TimestampTypeDef, WaiterConfigTypeDef
 
 __all__ = (
     "ClusterAvailableWaiter",
     "ClusterDeletedWaiter",
     "ClusterRestoredWaiter",
     "SnapshotAvailableWaiter",
 )
@@ -116,16 +115,16 @@
     async def wait(
         self,
         *,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotType: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
```

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift/waiter.pyi` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/waiter.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,19 @@
 
         cluster_available_waiter: ClusterAvailableWaiter = client.get_waiter("cluster_available")
         cluster_deleted_waiter: ClusterDeletedWaiter = client.get_waiter("cluster_deleted")
         cluster_restored_waiter: ClusterRestoredWaiter = client.get_waiter("cluster_restored")
         snapshot_available_waiter: SnapshotAvailableWaiter = client.get_waiter("snapshot_available")
     ```
 """
-from datetime import datetime
-from typing import Sequence, Union
+from typing import Sequence
 
 from aiobotocore.waiter import AIOWaiter
 
-from .type_defs import SnapshotSortingEntityTypeDef, WaiterConfigTypeDef
+from .type_defs import SnapshotSortingEntityTypeDef, TimestampTypeDef, WaiterConfigTypeDef
 
 __all__ = (
     "ClusterAvailableWaiter",
     "ClusterDeletedWaiter",
     "ClusterRestoredWaiter",
     "SnapshotAvailableWaiter",
 )
@@ -112,16 +111,16 @@
     async def wait(
         self,
         *,
         ClusterIdentifier: str = ...,
         SnapshotIdentifier: str = ...,
         SnapshotArn: str = ...,
         SnapshotType: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         OwnerAccount: str = ...,
         TagKeys: Sequence[str] = ...,
         TagValues: Sequence[str] = ...,
         ClusterExists: bool = ...,
         SortingEntities: Sequence[SnapshotSortingEntityTypeDef] = ...,
```

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift.egg-info/PKG-INFO` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Redshift 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Redshift 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore redshift type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore redshift type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-redshift"></a>
 
 # types-aiobotocore-redshift
 
 [![PyPI - types-aiobotocore-redshift](https://img.shields.io/pypi/v/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-redshift?color=blue)](https://pypistats.org/packages/types-aiobotocore-redshift)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift)](https://pepy.tech/project/types-aiobotocore-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Redshift 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [types-aiobotocore-redshift docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift/).
 
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
@@ -528,24 +527,25 @@
 )
 
 
 def check_value(value: ActionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_redshift.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_redshift.type_defs import (
     AcceptReservedNodeExchangeInputMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     AttributeValueTargetTypeDef,
     AccountWithRestoreAccessTypeDef,
     AquaConfigurationTypeDef,
     AssociateDataShareConsumerMessageRequestTypeDef,
     CertificateAssociationTypeDef,
     AuthenticationProfileTypeDef,
     AuthorizeClusterSecurityGroupIngressMessageRequestTypeDef,
@@ -554,21 +554,18 @@
     AuthorizeSnapshotAccessMessageRequestTypeDef,
     SupportedPlatformTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     SnapshotErrorMessageTypeDef,
     BatchModifyClusterSnapshotsMessageRequestTypeDef,
     CancelResizeMessageRequestTypeDef,
     ClusterAssociatedToScheduleTypeDef,
-    ClusterCredentialsTypeDef,
     RevisionTargetTypeDef,
-    ClusterExtendedCredentialsTypeDef,
     ClusterIamRoleTypeDef,
     ClusterNodeTypeDef,
     ParameterTypeDef,
-    ClusterParameterGroupNameMessageTypeDef,
     ClusterParameterStatusTypeDef,
     TagTypeDef,
     ClusterSecurityGroupMembershipTypeDef,
     ClusterSnapshotCopyStatusTypeDef,
     DataTransferProgressTypeDef,
     DeferredMaintenanceWindowTypeDef,
     ElasticIpStatusTypeDef,
@@ -577,23 +574,20 @@
     ReservedNodeExchangeStatusTypeDef,
     ResizeInfoTypeDef,
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
-    CreateAuthenticationProfileResultTypeDef,
     CreateCustomDomainAssociationMessageRequestTypeDef,
-    CreateCustomDomainAssociationResultTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
-    CustomerStorageMessageTypeDef,
+    TimestampTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
-    DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
     DeleteClusterSecurityGroupMessageRequestTypeDef,
     DeleteClusterSnapshotMessageRequestTypeDef,
     DeleteClusterSubnetGroupMessageRequestTypeDef,
     DeleteCustomDomainAssociationMessageRequestTypeDef,
     DeleteEndpointAccessMessageRequestTypeDef,
@@ -603,139 +597,113 @@
     DeleteScheduledActionMessageRequestTypeDef,
     DeleteSnapshotCopyGrantMessageRequestTypeDef,
     DeleteSnapshotScheduleMessageRequestTypeDef,
     DeleteTagsMessageRequestTypeDef,
     DeleteUsageLimitMessageRequestTypeDef,
     DescribeAccountAttributesMessageRequestTypeDef,
     DescribeAuthenticationProfilesMessageRequestTypeDef,
-    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClusterDbRevisionsMessageRequestTypeDef,
-    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageRequestTypeDef,
-    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterParametersMessageRequestTypeDef,
-    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageRequestTypeDef,
     SnapshotSortingEntityTypeDef,
     WaiterConfigTypeDef,
-    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageRequestTypeDef,
-    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
     DescribeClusterTracksMessageRequestTypeDef,
-    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
     DescribeClusterVersionsMessageRequestTypeDef,
-    DescribeClustersMessageDescribeClustersPaginateTypeDef,
     DescribeClustersMessageRequestTypeDef,
-    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
     DescribeCustomDomainAssociationsMessageRequestTypeDef,
-    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
     DescribeDataSharesForConsumerMessageRequestTypeDef,
-    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
     DescribeDataSharesForProducerMessageRequestTypeDef,
-    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
     DescribeDataSharesMessageRequestTypeDef,
-    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
     DescribeDefaultClusterParametersMessageRequestTypeDef,
-    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
     DescribeEndpointAccessMessageRequestTypeDef,
-    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
     DescribeEndpointAuthorizationMessageRequestTypeDef,
     DescribeEventCategoriesMessageRequestTypeDef,
-    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
     DescribeEventSubscriptionsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
-    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
     DescribeHsmClientCertificatesMessageRequestTypeDef,
-    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
     DescribeHsmConfigurationsMessageRequestTypeDef,
     DescribeLoggingStatusMessageRequestTypeDef,
     NodeConfigurationOptionsFilterTypeDef,
-    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
     DescribeOrderableClusterOptionsMessageRequestTypeDef,
     DescribePartnersInputMessageRequestTypeDef,
     PartnerIntegrationInfoTypeDef,
-    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
     DescribeReservedNodeExchangeStatusInputMessageRequestTypeDef,
-    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
     DescribeReservedNodeOfferingsMessageRequestTypeDef,
-    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
     DescribeReservedNodesMessageRequestTypeDef,
     DescribeResizeMessageRequestTypeDef,
     ScheduledActionFilterTypeDef,
-    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
     DescribeSnapshotCopyGrantsMessageRequestTypeDef,
-    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
     DescribeSnapshotSchedulesMessageRequestTypeDef,
-    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
     DescribeTableRestoreStatusMessageRequestTypeDef,
-    DescribeTagsMessageDescribeTagsPaginateTypeDef,
     DescribeTagsMessageRequestTypeDef,
-    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
     DescribeUsageLimitsMessageRequestTypeDef,
     DisableLoggingMessageRequestTypeDef,
     DisableSnapshotCopyMessageRequestTypeDef,
     DisassociateDataShareConsumerMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableLoggingMessageRequestTypeDef,
     EnableSnapshotCopyMessageRequestTypeDef,
     EndpointAuthorizationTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
     EventInfoMapTypeDef,
     EventTypeDef,
     GetClusterCredentialsMessageRequestTypeDef,
     GetClusterCredentialsWithIAMMessageRequestTypeDef,
-    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
     GetReservedNodeExchangeConfigurationOptionsInputMessageRequestTypeDef,
-    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
-    LoggingStatusTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
-    ModifyAuthenticationProfileResultTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
-    ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
     ModifyCustomDomainAssociationMessageRequestTypeDef,
-    ModifyCustomDomainAssociationResultTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     ModifySnapshotScheduleMessageRequestTypeDef,
     ModifyUsageLimitMessageRequestTypeDef,
     NetworkInterfaceTypeDef,
     NodeConfigurationOptionTypeDef,
-    PaginatorConfigTypeDef,
     PartnerIntegrationInputMessageRequestTypeDef,
-    PartnerIntegrationOutputMessageTypeDef,
     PauseClusterMessageRequestTypeDef,
     PauseClusterMessageTypeDef,
     PurchaseReservedNodeOfferingMessageRequestTypeDef,
     RebootClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RejectDataShareMessageRequestTypeDef,
     ResizeClusterMessageRequestTypeDef,
     ResizeClusterMessageTypeDef,
-    ResizeProgressMessageTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromClusterSnapshotMessageRequestTypeDef,
     RestoreTableFromClusterSnapshotMessageRequestTypeDef,
     TableRestoreStatusTypeDef,
     ResumeClusterMessageRequestTypeDef,
     ResumeClusterMessageTypeDef,
     RevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     RevokeEndpointAccessMessageRequestTypeDef,
     RevokeSnapshotAccessMessageRequestTypeDef,
     RotateEncryptionKeyMessageRequestTypeDef,
     SupportedOperationTypeDef,
     UpdatePartnerStatusInputMessageRequestTypeDef,
+    ClusterCredentialsTypeDef,
+    ClusterExtendedCredentialsTypeDef,
+    ClusterParameterGroupNameMessageTypeDef,
+    CreateAuthenticationProfileResultTypeDef,
+    CreateCustomDomainAssociationResultTypeDef,
+    CustomerStorageMessageTypeDef,
+    DeleteAuthenticationProfileResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EndpointAuthorizationResponseTypeDef,
+    LoggingStatusTypeDef,
+    ModifyAuthenticationProfileResultTypeDef,
+    ModifyCustomDomainAssociationResultTypeDef,
+    PartnerIntegrationOutputMessageTypeDef,
+    ResizeProgressMessageTypeDef,
     AccountAttributeTypeDef,
     ModifyAquaOutputMessageTypeDef,
     AssociationTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     AvailabilityZoneTypeDef,
     BatchDeleteClusterSnapshotsRequestRequestTypeDef,
     BatchDeleteClusterSnapshotsResultTypeDef,
@@ -761,24 +729,56 @@
     CreateUsageLimitMessageRequestTypeDef,
     EC2SecurityGroupTypeDef,
     EventSubscriptionTypeDef,
     HsmClientCertificateTypeDef,
     HsmConfigurationTypeDef,
     IPRangeTypeDef,
     SnapshotCopyGrantTypeDef,
-    SnapshotScheduleResponseMetadataTypeDef,
+    SnapshotScheduleResponseTypeDef,
     SnapshotScheduleTypeDef,
     SnapshotTypeDef,
     TaggedResourceTypeDef,
-    UsageLimitResponseMetadataTypeDef,
+    UsageLimitResponseTypeDef,
     UsageLimitTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     ClusterVersionsMessageTypeDef,
-    DataShareResponseMetadataTypeDef,
+    DescribeEventsMessageRequestTypeDef,
+    ModifyClusterMaintenanceMessageRequestTypeDef,
+    DataShareResponseTypeDef,
     DataShareTypeDef,
+    DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
+    DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
+    DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
+    DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
+    DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
+    DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
+    DescribeClusterVersionsMessageDescribeClusterVersionsPaginateTypeDef,
+    DescribeClustersMessageDescribeClustersPaginateTypeDef,
+    DescribeCustomDomainAssociationsMessageDescribeCustomDomainAssociationsPaginateTypeDef,
+    DescribeDataSharesForConsumerMessageDescribeDataSharesForConsumerPaginateTypeDef,
+    DescribeDataSharesForProducerMessageDescribeDataSharesForProducerPaginateTypeDef,
+    DescribeDataSharesMessageDescribeDataSharesPaginateTypeDef,
+    DescribeDefaultClusterParametersMessageDescribeDefaultClusterParametersPaginateTypeDef,
+    DescribeEndpointAccessMessageDescribeEndpointAccessPaginateTypeDef,
+    DescribeEndpointAuthorizationMessageDescribeEndpointAuthorizationPaginateTypeDef,
+    DescribeEventSubscriptionsMessageDescribeEventSubscriptionsPaginateTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeHsmClientCertificatesMessageDescribeHsmClientCertificatesPaginateTypeDef,
+    DescribeHsmConfigurationsMessageDescribeHsmConfigurationsPaginateTypeDef,
+    DescribeOrderableClusterOptionsMessageDescribeOrderableClusterOptionsPaginateTypeDef,
+    DescribeReservedNodeExchangeStatusInputMessageDescribeReservedNodeExchangeStatusPaginateTypeDef,
+    DescribeReservedNodeOfferingsMessageDescribeReservedNodeOfferingsPaginateTypeDef,
+    DescribeReservedNodesMessageDescribeReservedNodesPaginateTypeDef,
+    DescribeSnapshotCopyGrantsMessageDescribeSnapshotCopyGrantsPaginateTypeDef,
+    DescribeSnapshotSchedulesMessageDescribeSnapshotSchedulesPaginateTypeDef,
+    DescribeTableRestoreStatusMessageDescribeTableRestoreStatusPaginateTypeDef,
+    DescribeTagsMessageDescribeTagsPaginateTypeDef,
+    DescribeUsageLimitsMessageDescribeUsageLimitsPaginateTypeDef,
+    GetReservedNodeExchangeConfigurationOptionsInputMessageGetReservedNodeExchangeConfigurationOptionsPaginateTypeDef,
+    GetReservedNodeExchangeOfferingsInputMessageGetReservedNodeExchangeOfferingsPaginateTypeDef,
     DescribeClusterSnapshotsMessageDescribeClusterSnapshotsPaginateTypeDef,
     DescribeClusterSnapshotsMessageRequestTypeDef,
     DescribeClusterSnapshotsMessageSnapshotAvailableWaitTypeDef,
     DescribeClustersMessageClusterAvailableWaitTypeDef,
     DescribeClustersMessageClusterDeletedWaitTypeDef,
     DescribeClustersMessageClusterRestoredWaitTypeDef,
     DescribeNodeConfigurationOptionsMessageDescribeNodeConfigurationOptionsPaginateTypeDef,
@@ -825,26 +825,26 @@
     SnapshotMessageTypeDef,
     TaggedResourceListMessageTypeDef,
     UsageLimitListTypeDef,
     DescribeDataSharesForConsumerResultTypeDef,
     DescribeDataSharesForProducerResultTypeDef,
     DescribeDataSharesResultTypeDef,
     EventCategoriesMessageTypeDef,
-    EndpointAccessResponseMetadataTypeDef,
+    EndpointAccessResponseTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     ReservedNodeOfferingsMessageTypeDef,
     AcceptReservedNodeExchangeOutputMessageTypeDef,
     PurchaseReservedNodeOfferingResultTypeDef,
     ReservedNodeConfigurationOptionTypeDef,
     ReservedNodesMessageTypeDef,
     CreateScheduledActionMessageRequestTypeDef,
     ModifyScheduledActionMessageRequestTypeDef,
-    ScheduledActionResponseMetadataTypeDef,
+    ScheduledActionResponseTypeDef,
     ScheduledActionTypeDef,
     MaintenanceTrackTypeDef,
     OrderableClusterOptionsMessageTypeDef,
     ClusterSubnetGroupTypeDef,
     AuthorizeClusterSecurityGroupIngressResultTypeDef,
     ClusterSecurityGroupMessageTypeDef,
     CreateClusterSecurityGroupResultTypeDef,
@@ -872,15 +872,15 @@
     ResizeClusterResultTypeDef,
     RestoreFromClusterSnapshotResultTypeDef,
     ResumeClusterResultTypeDef,
     RotateEncryptionKeyResultTypeDef,
 )
 
 
-def get_structure() -> AcceptReservedNodeExchangeInputMessageRequestTypeDef:
+def get_value() -> AcceptReservedNodeExchangeInputMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-redshift-2.5.2/types_aiobotocore_redshift.egg-info/SOURCES.txt` & `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-ds-2.5.2.tar.gz` & `tmp/types-aiobotocore-ds-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ds-2.5.2.tar", last modified: Sat Jul  8 01:43:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-ds-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
```

## Comparing `types-aiobotocore-ds-2.5.2.tar` & `types-aiobotocore-ds-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.898042 types-aiobotocore-ds-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-07-08 01:43:32.894042 types-aiobotocore-ds-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20963 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:32.898042 types-aiobotocore-ds-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.894042 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54551 2023-07-08 01:29:04.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54461 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-07-08 01:29:04.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-07-08 01:29:04.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-07-08 01:29:04.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17759 2023-07-08 01:29:04.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57753 2023-07-08 01:29:05.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57680 2023-07-08 01:29:05.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:29:03.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:32.894042 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22522 2023-07-08 01:43:32.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-08 01:43:32.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:32.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 01:43:32.000000 types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.089601 types-aiobotocore-ds-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22600 2023-08-02 14:52:12.085601 types-aiobotocore-ds-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.089601 types-aiobotocore-ds-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-02 14:36:43.000000 types-aiobotocore-ds-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.085601 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54586 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54496 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-08-02 14:36:45.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-08-02 14:36:45.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-08-02 14:36:45.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58571 2023-08-02 14:36:46.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58498 2023-08-02 14:36:45.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.085601 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22600 2023-08-02 14:52:11.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 14:52:11.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:11.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 14:52:11.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ds-2.5.2/LICENSE` & `types-aiobotocore-ds-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2/PKG-INFO` & `types-aiobotocore-ds-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ds
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DirectoryService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DirectoryService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ds type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ds type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ds"></a>
 
 # types-aiobotocore-ds
 
 [![PyPI - types-aiobotocore-ds](https://img.shields.io/pypi/v/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ds?color=blue)](https://pypistats.org/packages/types-aiobotocore-ds)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ds)](https://pepy.tech/project/types-aiobotocore-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DirectoryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [types-aiobotocore-ds docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/).
 
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
@@ -398,184 +397,188 @@
 )
 
 
 def check_value(value: CertificateStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ds.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ds.type_defs import (
     AcceptSharedDirectoryRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SharedDirectoryTypeDef,
     IpRouteTypeDef,
     DirectoryVpcSettingsTypeDef,
     TagTypeDef,
     AttributeTypeDef,
     CancelSchemaExtensionRequestRequestTypeDef,
     CertificateInfoTypeDef,
     ClientCertAuthSettingsTypeDef,
     ClientAuthenticationSettingInfoTypeDef,
     ConditionalForwarderTypeDef,
     DirectoryConnectSettingsTypeDef,
-    ConnectDirectoryResultTypeDef,
     CreateAliasRequestRequestTypeDef,
-    CreateAliasResultTypeDef,
     CreateConditionalForwarderRequestRequestTypeDef,
-    CreateDirectoryResultTypeDef,
     CreateLogSubscriptionRequestRequestTypeDef,
-    CreateMicrosoftADResultTypeDef,
     CreateSnapshotRequestRequestTypeDef,
-    CreateSnapshotResultTypeDef,
     CreateTrustRequestRequestTypeDef,
-    CreateTrustResultTypeDef,
     DeleteConditionalForwarderRequestRequestTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
-    DeleteDirectoryResultTypeDef,
     DeleteLogSubscriptionRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
-    DeleteSnapshotResultTypeDef,
     DeleteTrustRequestRequestTypeDef,
-    DeleteTrustResultTypeDef,
     DeregisterCertificateRequestRequestTypeDef,
     DeregisterEventTopicRequestRequestTypeDef,
     DescribeCertificateRequestRequestTypeDef,
-    DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClientAuthenticationSettingsRequestRequestTypeDef,
     DescribeConditionalForwardersRequestRequestTypeDef,
-    DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef,
     DescribeDirectoriesRequestRequestTypeDef,
-    DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
     DescribeDomainControllersRequestRequestTypeDef,
     DomainControllerTypeDef,
     DescribeEventTopicsRequestRequestTypeDef,
     EventTopicTypeDef,
-    DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
     DescribeLDAPSSettingsRequestRequestTypeDef,
     LDAPSSettingInfoTypeDef,
-    DescribeRegionsRequestDescribeRegionsPaginateTypeDef,
     DescribeRegionsRequestRequestTypeDef,
     DescribeSettingsRequestRequestTypeDef,
     SettingEntryTypeDef,
-    DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
     DescribeSharedDirectoriesRequestRequestTypeDef,
-    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
-    DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
     DescribeTrustsRequestRequestTypeDef,
     TrustTypeDef,
-    DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
     DescribeUpdateDirectoryRequestRequestTypeDef,
     DirectoryConnectSettingsDescriptionTypeDef,
     DirectoryVpcSettingsDescriptionTypeDef,
-    RadiusSettingsTypeDef,
+    RadiusSettingsOutputTypeDef,
     RegionsInfoTypeDef,
     DirectoryLimitsTypeDef,
+    DirectoryVpcSettingsOutputTypeDef,
     DisableClientAuthenticationRequestRequestTypeDef,
     DisableLDAPSRequestRequestTypeDef,
     DisableRadiusRequestRequestTypeDef,
     DisableSsoRequestRequestTypeDef,
     EnableClientAuthenticationRequestRequestTypeDef,
     EnableLDAPSRequestRequestTypeDef,
+    RadiusSettingsTypeDef,
     EnableSsoRequestRequestTypeDef,
     GetSnapshotLimitsRequestRequestTypeDef,
     SnapshotLimitsTypeDef,
     IpRouteInfoTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
-    ListIpRoutesRequestListIpRoutesPaginateTypeDef,
     ListIpRoutesRequestRequestTypeDef,
-    ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef,
     ListLogSubscriptionsRequestRequestTypeDef,
     LogSubscriptionTypeDef,
-    ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
     ListSchemaExtensionsRequestRequestTypeDef,
     SchemaExtensionInfoTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     OSUpdateSettingsTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterCertificateResultTypeDef,
     RegisterEventTopicRequestRequestTypeDef,
     RejectSharedDirectoryRequestRequestTypeDef,
-    RejectSharedDirectoryResultTypeDef,
     RemoveIpRoutesRequestRequestTypeDef,
     RemoveRegionRequestRequestTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetUserPasswordRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     SettingTypeDef,
     ShareTargetTypeDef,
-    ShareDirectoryResultTypeDef,
     StartSchemaExtensionRequestRequestTypeDef,
-    StartSchemaExtensionResultTypeDef,
     UnshareTargetTypeDef,
-    UnshareDirectoryResultTypeDef,
     UpdateConditionalForwarderRequestRequestTypeDef,
     UpdateNumberOfDomainControllersRequestRequestTypeDef,
-    UpdateSettingsResultTypeDef,
     UpdateTrustRequestRequestTypeDef,
-    UpdateTrustResultTypeDef,
     VerifyTrustRequestRequestTypeDef,
+    ConnectDirectoryResultTypeDef,
+    CreateAliasResultTypeDef,
+    CreateDirectoryResultTypeDef,
+    CreateMicrosoftADResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    CreateTrustResultTypeDef,
+    DeleteDirectoryResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DeleteTrustResultTypeDef,
+    RegisterCertificateResultTypeDef,
+    RejectSharedDirectoryResultTypeDef,
+    ShareDirectoryResultTypeDef,
+    StartSchemaExtensionResultTypeDef,
+    UnshareDirectoryResultTypeDef,
+    UpdateSettingsResultTypeDef,
+    UpdateTrustResultTypeDef,
     VerifyTrustResultTypeDef,
     AcceptSharedDirectoryResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     AddIpRoutesRequestRequestTypeDef,
     AddRegionRequestRequestTypeDef,
-    RegionDescriptionTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateDirectoryRequestRequestTypeDef,
     CreateMicrosoftADRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     ComputerTypeDef,
     CreateComputerRequestRequestTypeDef,
     ListCertificatesResultTypeDef,
     CertificateTypeDef,
     RegisterCertificateRequestRequestTypeDef,
     DescribeClientAuthenticationSettingsResultTypeDef,
     DescribeConditionalForwardersResultTypeDef,
     ConnectDirectoryRequestRequestTypeDef,
+    DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef,
+    DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+    DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+    DescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+    DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
+    DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
+    DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListIpRoutesRequestListIpRoutesPaginateTypeDef,
+    ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef,
+    ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeDomainControllersResultTypeDef,
     DescribeEventTopicsResultTypeDef,
     DescribeLDAPSSettingsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
-    EnableRadiusRequestRequestTypeDef,
     OwnerDirectoryDescriptionTypeDef,
-    UpdateRadiusRequestRequestTypeDef,
     GetDirectoryLimitsResultTypeDef,
+    DirectoryVpcSettingsUnionTypeDef,
+    RegionDescriptionTypeDef,
+    EnableRadiusRequestRequestTypeDef,
+    RadiusSettingsUnionTypeDef,
+    UpdateRadiusRequestRequestTypeDef,
     GetSnapshotLimitsResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     UpdateDirectorySetupRequestRequestTypeDef,
     UpdateValueTypeDef,
     UpdateSettingsRequestRequestTypeDef,
     ShareDirectoryRequestRequestTypeDef,
     UnshareDirectoryRequestRequestTypeDef,
-    DescribeRegionsResultTypeDef,
     CreateComputerResultTypeDef,
     DescribeCertificateResultTypeDef,
     DirectoryDescriptionTypeDef,
+    DescribeRegionsResultTypeDef,
     UpdateInfoEntryTypeDef,
     DescribeDirectoriesResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
 )
 
 
-def get_structure() -> AcceptSharedDirectoryRequestRequestTypeDef:
+def get_value() -> AcceptSharedDirectoryRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ds-2.5.2/README.md` & `types-aiobotocore-ds-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-ds"></a>
 
 # types-aiobotocore-ds
 
 [![PyPI - types-aiobotocore-ds](https://img.shields.io/pypi/v/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ds?color=blue)](https://pypistats.org/packages/types-aiobotocore-ds)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ds)](https://pepy.tech/project/types-aiobotocore-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DirectoryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [types-aiobotocore-ds docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/).
 
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
@@ -365,184 +365,188 @@
 )
 
 
 def check_value(value: CertificateStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ds.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ds.type_defs import (
     AcceptSharedDirectoryRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SharedDirectoryTypeDef,
     IpRouteTypeDef,
     DirectoryVpcSettingsTypeDef,
     TagTypeDef,
     AttributeTypeDef,
     CancelSchemaExtensionRequestRequestTypeDef,
     CertificateInfoTypeDef,
     ClientCertAuthSettingsTypeDef,
     ClientAuthenticationSettingInfoTypeDef,
     ConditionalForwarderTypeDef,
     DirectoryConnectSettingsTypeDef,
-    ConnectDirectoryResultTypeDef,
     CreateAliasRequestRequestTypeDef,
-    CreateAliasResultTypeDef,
     CreateConditionalForwarderRequestRequestTypeDef,
-    CreateDirectoryResultTypeDef,
     CreateLogSubscriptionRequestRequestTypeDef,
-    CreateMicrosoftADResultTypeDef,
     CreateSnapshotRequestRequestTypeDef,
-    CreateSnapshotResultTypeDef,
     CreateTrustRequestRequestTypeDef,
-    CreateTrustResultTypeDef,
     DeleteConditionalForwarderRequestRequestTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
-    DeleteDirectoryResultTypeDef,
     DeleteLogSubscriptionRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
-    DeleteSnapshotResultTypeDef,
     DeleteTrustRequestRequestTypeDef,
-    DeleteTrustResultTypeDef,
     DeregisterCertificateRequestRequestTypeDef,
     DeregisterEventTopicRequestRequestTypeDef,
     DescribeCertificateRequestRequestTypeDef,
-    DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClientAuthenticationSettingsRequestRequestTypeDef,
     DescribeConditionalForwardersRequestRequestTypeDef,
-    DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef,
     DescribeDirectoriesRequestRequestTypeDef,
-    DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
     DescribeDomainControllersRequestRequestTypeDef,
     DomainControllerTypeDef,
     DescribeEventTopicsRequestRequestTypeDef,
     EventTopicTypeDef,
-    DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
     DescribeLDAPSSettingsRequestRequestTypeDef,
     LDAPSSettingInfoTypeDef,
-    DescribeRegionsRequestDescribeRegionsPaginateTypeDef,
     DescribeRegionsRequestRequestTypeDef,
     DescribeSettingsRequestRequestTypeDef,
     SettingEntryTypeDef,
-    DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
     DescribeSharedDirectoriesRequestRequestTypeDef,
-    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
-    DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
     DescribeTrustsRequestRequestTypeDef,
     TrustTypeDef,
-    DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
     DescribeUpdateDirectoryRequestRequestTypeDef,
     DirectoryConnectSettingsDescriptionTypeDef,
     DirectoryVpcSettingsDescriptionTypeDef,
-    RadiusSettingsTypeDef,
+    RadiusSettingsOutputTypeDef,
     RegionsInfoTypeDef,
     DirectoryLimitsTypeDef,
+    DirectoryVpcSettingsOutputTypeDef,
     DisableClientAuthenticationRequestRequestTypeDef,
     DisableLDAPSRequestRequestTypeDef,
     DisableRadiusRequestRequestTypeDef,
     DisableSsoRequestRequestTypeDef,
     EnableClientAuthenticationRequestRequestTypeDef,
     EnableLDAPSRequestRequestTypeDef,
+    RadiusSettingsTypeDef,
     EnableSsoRequestRequestTypeDef,
     GetSnapshotLimitsRequestRequestTypeDef,
     SnapshotLimitsTypeDef,
     IpRouteInfoTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
-    ListIpRoutesRequestListIpRoutesPaginateTypeDef,
     ListIpRoutesRequestRequestTypeDef,
-    ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef,
     ListLogSubscriptionsRequestRequestTypeDef,
     LogSubscriptionTypeDef,
-    ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
     ListSchemaExtensionsRequestRequestTypeDef,
     SchemaExtensionInfoTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     OSUpdateSettingsTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterCertificateResultTypeDef,
     RegisterEventTopicRequestRequestTypeDef,
     RejectSharedDirectoryRequestRequestTypeDef,
-    RejectSharedDirectoryResultTypeDef,
     RemoveIpRoutesRequestRequestTypeDef,
     RemoveRegionRequestRequestTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetUserPasswordRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     SettingTypeDef,
     ShareTargetTypeDef,
-    ShareDirectoryResultTypeDef,
     StartSchemaExtensionRequestRequestTypeDef,
-    StartSchemaExtensionResultTypeDef,
     UnshareTargetTypeDef,
-    UnshareDirectoryResultTypeDef,
     UpdateConditionalForwarderRequestRequestTypeDef,
     UpdateNumberOfDomainControllersRequestRequestTypeDef,
-    UpdateSettingsResultTypeDef,
     UpdateTrustRequestRequestTypeDef,
-    UpdateTrustResultTypeDef,
     VerifyTrustRequestRequestTypeDef,
+    ConnectDirectoryResultTypeDef,
+    CreateAliasResultTypeDef,
+    CreateDirectoryResultTypeDef,
+    CreateMicrosoftADResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    CreateTrustResultTypeDef,
+    DeleteDirectoryResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DeleteTrustResultTypeDef,
+    RegisterCertificateResultTypeDef,
+    RejectSharedDirectoryResultTypeDef,
+    ShareDirectoryResultTypeDef,
+    StartSchemaExtensionResultTypeDef,
+    UnshareDirectoryResultTypeDef,
+    UpdateSettingsResultTypeDef,
+    UpdateTrustResultTypeDef,
     VerifyTrustResultTypeDef,
     AcceptSharedDirectoryResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     AddIpRoutesRequestRequestTypeDef,
     AddRegionRequestRequestTypeDef,
-    RegionDescriptionTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateDirectoryRequestRequestTypeDef,
     CreateMicrosoftADRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     ComputerTypeDef,
     CreateComputerRequestRequestTypeDef,
     ListCertificatesResultTypeDef,
     CertificateTypeDef,
     RegisterCertificateRequestRequestTypeDef,
     DescribeClientAuthenticationSettingsResultTypeDef,
     DescribeConditionalForwardersResultTypeDef,
     ConnectDirectoryRequestRequestTypeDef,
+    DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef,
+    DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+    DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+    DescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+    DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
+    DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
+    DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListIpRoutesRequestListIpRoutesPaginateTypeDef,
+    ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef,
+    ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeDomainControllersResultTypeDef,
     DescribeEventTopicsResultTypeDef,
     DescribeLDAPSSettingsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
-    EnableRadiusRequestRequestTypeDef,
     OwnerDirectoryDescriptionTypeDef,
-    UpdateRadiusRequestRequestTypeDef,
     GetDirectoryLimitsResultTypeDef,
+    DirectoryVpcSettingsUnionTypeDef,
+    RegionDescriptionTypeDef,
+    EnableRadiusRequestRequestTypeDef,
+    RadiusSettingsUnionTypeDef,
+    UpdateRadiusRequestRequestTypeDef,
     GetSnapshotLimitsResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     UpdateDirectorySetupRequestRequestTypeDef,
     UpdateValueTypeDef,
     UpdateSettingsRequestRequestTypeDef,
     ShareDirectoryRequestRequestTypeDef,
     UnshareDirectoryRequestRequestTypeDef,
-    DescribeRegionsResultTypeDef,
     CreateComputerResultTypeDef,
     DescribeCertificateResultTypeDef,
     DirectoryDescriptionTypeDef,
+    DescribeRegionsResultTypeDef,
     UpdateInfoEntryTypeDef,
     DescribeDirectoriesResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
 )
 
 
-def get_structure() -> AcceptSharedDirectoryRequestRequestTypeDef:
+def get_value() -> AcceptSharedDirectoryRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ds-2.5.2/setup.py` & `types-aiobotocore-ds-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ds",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_ds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DirectoryService 2.5.2 service generated with"
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
-    keywords="aiobotocore ds type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore ds type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ds": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/__init__.py` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/__init__.pyi` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/__main__.py` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DirectoryService 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.DirectoryService 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService\nOther"
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

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/client.py` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,25 +71,25 @@
     DescribeRegionsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
     DirectoryConnectSettingsTypeDef,
-    DirectoryVpcSettingsTypeDef,
+    DirectoryVpcSettingsUnionTypeDef,
     GetDirectoryLimitsResultTypeDef,
     GetSnapshotLimitsResultTypeDef,
     IpRouteTypeDef,
     ListCertificatesResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     OSUpdateSettingsTypeDef,
-    RadiusSettingsTypeDef,
+    RadiusSettingsUnionTypeDef,
     RegisterCertificateResultTypeDef,
     RejectSharedDirectoryResultTypeDef,
     SettingTypeDef,
     ShareDirectoryResultTypeDef,
     ShareTargetTypeDef,
     StartSchemaExtensionResultTypeDef,
     TagTypeDef,
@@ -199,15 +199,15 @@
         from your Microsoft AD on Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_ip_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#add_ip_routes)
         """
 
     async def add_region(
-        self, *, DirectoryId: str, RegionName: str, VPCSettings: DirectoryVpcSettingsTypeDef
+        self, *, DirectoryId: str, RegionName: str, VPCSettings: DirectoryVpcSettingsUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Adds two domain controllers in the specified Region for the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_region)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#add_region)
         """
@@ -305,15 +305,15 @@
         self,
         *,
         Name: str,
         Password: str,
         Size: DirectorySizeType,
         ShortName: str = ...,
         Description: str = ...,
-        VpcSettings: DirectoryVpcSettingsTypeDef = ...,
+        VpcSettings: DirectoryVpcSettingsUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDirectoryResultTypeDef:
         """
         Creates a Simple AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_directory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_directory)
@@ -332,15 +332,15 @@
         """
 
     async def create_microsoft_ad(
         self,
         *,
         Name: str,
         Password: str,
-        VpcSettings: DirectoryVpcSettingsTypeDef,
+        VpcSettings: DirectoryVpcSettingsUnionTypeDef,
         ShortName: str = ...,
         Description: str = ...,
         Edition: DirectoryEditionType = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMicrosoftADResultTypeDef:
         """
         Creates a Microsoft AD directory in the Amazon Web Services Cloud.
@@ -671,15 +671,15 @@
         Activates the switch for the specific directory to always use LDAP secure calls.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_ldaps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#enable_ldaps)
         """
 
     async def enable_radius(
-        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsTypeDef
+        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Enables multi-factor authentication (MFA) with the Remote Authentication Dial In
         User Service (RADIUS) server for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_radius)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#enable_radius)
@@ -931,15 +931,15 @@
         Adds or removes domain controllers to or from the directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_number_of_domain_controllers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#update_number_of_domain_controllers)
         """
 
     async def update_radius(
-        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsTypeDef
+        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the Remote Authentication Dial In User Service (RADIUS) server
         information for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_radius)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#update_radius)
```

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/client.pyi` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -71,25 +71,25 @@
     DescribeRegionsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
     DirectoryConnectSettingsTypeDef,
-    DirectoryVpcSettingsTypeDef,
+    DirectoryVpcSettingsUnionTypeDef,
     GetDirectoryLimitsResultTypeDef,
     GetSnapshotLimitsResultTypeDef,
     IpRouteTypeDef,
     ListCertificatesResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     OSUpdateSettingsTypeDef,
-    RadiusSettingsTypeDef,
+    RadiusSettingsUnionTypeDef,
     RegisterCertificateResultTypeDef,
     RejectSharedDirectoryResultTypeDef,
     SettingTypeDef,
     ShareDirectoryResultTypeDef,
     ShareTargetTypeDef,
     StartSchemaExtensionResultTypeDef,
     TagTypeDef,
@@ -192,15 +192,15 @@
         address, you must add a CIDR address block to correctly route traffic to and
         from your Microsoft AD on Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_ip_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#add_ip_routes)
         """
     async def add_region(
-        self, *, DirectoryId: str, RegionName: str, VPCSettings: DirectoryVpcSettingsTypeDef
+        self, *, DirectoryId: str, RegionName: str, VPCSettings: DirectoryVpcSettingsUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Adds two domain controllers in the specified Region for the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_region)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#add_region)
         """
@@ -289,15 +289,15 @@
         self,
         *,
         Name: str,
         Password: str,
         Size: DirectorySizeType,
         ShortName: str = ...,
         Description: str = ...,
-        VpcSettings: DirectoryVpcSettingsTypeDef = ...,
+        VpcSettings: DirectoryVpcSettingsUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDirectoryResultTypeDef:
         """
         Creates a Simple AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_directory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_directory)
@@ -314,15 +314,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_log_subscription)
         """
     async def create_microsoft_ad(
         self,
         *,
         Name: str,
         Password: str,
-        VpcSettings: DirectoryVpcSettingsTypeDef,
+        VpcSettings: DirectoryVpcSettingsUnionTypeDef,
         ShortName: str = ...,
         Description: str = ...,
         Edition: DirectoryEditionType = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMicrosoftADResultTypeDef:
         """
         Creates a Microsoft AD directory in the Amazon Web Services Cloud.
@@ -624,15 +624,15 @@
         """
         Activates the switch for the specific directory to always use LDAP secure calls.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_ldaps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#enable_ldaps)
         """
     async def enable_radius(
-        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsTypeDef
+        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Enables multi-factor authentication (MFA) with the Remote Authentication Dial In
         User Service (RADIUS) server for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_radius)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#enable_radius)
@@ -860,15 +860,15 @@
         """
         Adds or removes domain controllers to or from the directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_number_of_domain_controllers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#update_number_of_domain_controllers)
         """
     async def update_radius(
-        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsTypeDef
+        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the Remote Authentication Dial In User Service (RADIUS) server
         information for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_radius)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#update_radius)
```

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/literals.py` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/literals.pyi` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/paginator.py` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeClientAuthenticationSettingsPaginator",
     "DescribeDirectoriesPaginator",
     "DescribeDomainControllersPaginator",
     "DescribeLDAPSSettingsPaginator",
     "DescribeRegionsPaginator",
     "DescribeSharedDirectoriesPaginator",
@@ -90,259 +89,243 @@
     "ListCertificatesPaginator",
     "ListIpRoutesPaginator",
     "ListLogSubscriptionsPaginator",
     "ListSchemaExtensionsPaginator",
     "ListTagsForResourcePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeClientAuthenticationSettingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeClientAuthenticationSettings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeclientauthenticationsettingspaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         Type: ClientAuthenticationTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeClientAuthenticationSettingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeClientAuthenticationSettings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeclientauthenticationsettingspaginator)
         """
 
-
 class DescribeDirectoriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDirectories)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describedirectoriespaginator)
     """
 
     def paginate(
-        self, *, DirectoryIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDirectories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describedirectoriespaginator)
         """
 
-
 class DescribeDomainControllersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDomainControllers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describedomaincontrollerspaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         DomainControllerIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDomainControllersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDomainControllers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describedomaincontrollerspaginator)
         """
 
-
 class DescribeLDAPSSettingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeLDAPSSettings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeldapssettingspaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         Type: Literal["Client"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeLDAPSSettingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeLDAPSSettings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeldapssettingspaginator)
         """
 
-
 class DescribeRegionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeRegions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeregionspaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         RegionName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRegionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeRegions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeregionspaginator)
         """
 
-
 class DescribeSharedDirectoriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSharedDirectories)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeshareddirectoriespaginator)
     """
 
     def paginate(
         self,
         *,
         OwnerDirectoryId: str,
         SharedDirectoryIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSharedDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSharedDirectories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeshareddirectoriespaginator)
         """
 
-
 class DescribeSnapshotsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSnapshots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describesnapshotspaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str = ...,
         SnapshotIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describesnapshotspaginator)
         """
 
-
 class DescribeTrustsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeTrusts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describetrustspaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str = ...,
         TrustIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTrustsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeTrusts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describetrustspaginator)
         """
 
-
 class DescribeUpdateDirectoryPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeUpdateDirectory)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeupdatedirectorypaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         UpdateType: Literal["OS"],
         RegionName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeUpdateDirectoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeUpdateDirectory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeupdatedirectorypaginator)
         """
 
-
 class ListCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listcertificatespaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCertificatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listcertificatespaginator)
         """
 
-
 class ListIpRoutesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListIpRoutes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listiproutespaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIpRoutesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListIpRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listiproutespaginator)
         """
 
-
 class ListLogSubscriptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListLogSubscriptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listlogsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLogSubscriptionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListLogSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listlogsubscriptionspaginator)
         """
 
-
 class ListSchemaExtensionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListSchemaExtensions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listschemaextensionspaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSchemaExtensionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListSchemaExtensions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listschemaextensionspaginator)
         """
 
-
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/paginator.pyi` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DescribeClientAuthenticationSettingsPaginator",
     "DescribeDirectoriesPaginator",
     "DescribeDomainControllersPaginator",
     "DescribeLDAPSSettingsPaginator",
     "DescribeRegionsPaginator",
     "DescribeSharedDirectoriesPaginator",
@@ -89,243 +90,259 @@
     "ListCertificatesPaginator",
     "ListIpRoutesPaginator",
     "ListLogSubscriptionsPaginator",
     "ListSchemaExtensionsPaginator",
     "ListTagsForResourcePaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeClientAuthenticationSettingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeClientAuthenticationSettings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeclientauthenticationsettingspaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         Type: ClientAuthenticationTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeClientAuthenticationSettingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeClientAuthenticationSettings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeclientauthenticationsettingspaginator)
         """
 
+
 class DescribeDirectoriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDirectories)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describedirectoriespaginator)
     """
 
     def paginate(
-        self, *, DirectoryIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDirectories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describedirectoriespaginator)
         """
 
+
 class DescribeDomainControllersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDomainControllers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describedomaincontrollerspaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         DomainControllerIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDomainControllersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDomainControllers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describedomaincontrollerspaginator)
         """
 
+
 class DescribeLDAPSSettingsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeLDAPSSettings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeldapssettingspaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         Type: Literal["Client"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeLDAPSSettingsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeLDAPSSettings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeldapssettingspaginator)
         """
 
+
 class DescribeRegionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeRegions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeregionspaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         RegionName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRegionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeRegions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeregionspaginator)
         """
 
+
 class DescribeSharedDirectoriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSharedDirectories)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeshareddirectoriespaginator)
     """
 
     def paginate(
         self,
         *,
         OwnerDirectoryId: str,
         SharedDirectoryIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSharedDirectoriesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSharedDirectories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeshareddirectoriespaginator)
         """
 
+
 class DescribeSnapshotsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSnapshots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describesnapshotspaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str = ...,
         SnapshotIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describesnapshotspaginator)
         """
 
+
 class DescribeTrustsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeTrusts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describetrustspaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str = ...,
         TrustIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTrustsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeTrusts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describetrustspaginator)
         """
 
+
 class DescribeUpdateDirectoryPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeUpdateDirectory)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeupdatedirectorypaginator)
     """
 
     def paginate(
         self,
         *,
         DirectoryId: str,
         UpdateType: Literal["OS"],
         RegionName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeUpdateDirectoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeUpdateDirectory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#describeupdatedirectorypaginator)
         """
 
+
 class ListCertificatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListCertificates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listcertificatespaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCertificatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listcertificatespaginator)
         """
 
+
 class ListIpRoutesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListIpRoutes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listiproutespaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIpRoutesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListIpRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listiproutespaginator)
         """
 
+
 class ListLogSubscriptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListLogSubscriptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listlogsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLogSubscriptionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListLogSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listlogsubscriptionspaginator)
         """
 
+
 class ListSchemaExtensionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListSchemaExtensions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listschemaextensionspaginator)
     """
 
     def paginate(
-        self, *, DirectoryId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DirectoryId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSchemaExtensionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListSchemaExtensions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listschemaextensionspaginator)
         """
 
+
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/type_defs.py` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ds.type_defs import AcceptSharedDirectoryRequestRequestTypeDef
 
-    data: AcceptSharedDirectoryRequestRequestTypeDef = {...}
+    data: AcceptSharedDirectoryRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     CertificateStateType,
     CertificateTypeType,
     ClientAuthenticationStatusType,
     ClientAuthenticationTypeType,
     DirectoryConfigurationStatusType,
@@ -50,182 +50,196 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptSharedDirectoryRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SharedDirectoryTypeDef",
     "IpRouteTypeDef",
     "DirectoryVpcSettingsTypeDef",
     "TagTypeDef",
     "AttributeTypeDef",
     "CancelSchemaExtensionRequestRequestTypeDef",
     "CertificateInfoTypeDef",
     "ClientCertAuthSettingsTypeDef",
     "ClientAuthenticationSettingInfoTypeDef",
     "ConditionalForwarderTypeDef",
     "DirectoryConnectSettingsTypeDef",
-    "ConnectDirectoryResultTypeDef",
     "CreateAliasRequestRequestTypeDef",
-    "CreateAliasResultTypeDef",
     "CreateConditionalForwarderRequestRequestTypeDef",
-    "CreateDirectoryResultTypeDef",
     "CreateLogSubscriptionRequestRequestTypeDef",
-    "CreateMicrosoftADResultTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
-    "CreateSnapshotResultTypeDef",
     "CreateTrustRequestRequestTypeDef",
-    "CreateTrustResultTypeDef",
     "DeleteConditionalForwarderRequestRequestTypeDef",
     "DeleteDirectoryRequestRequestTypeDef",
-    "DeleteDirectoryResultTypeDef",
     "DeleteLogSubscriptionRequestRequestTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
-    "DeleteSnapshotResultTypeDef",
     "DeleteTrustRequestRequestTypeDef",
-    "DeleteTrustResultTypeDef",
     "DeregisterCertificateRequestRequestTypeDef",
     "DeregisterEventTopicRequestRequestTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
-    "DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClientAuthenticationSettingsRequestRequestTypeDef",
     "DescribeConditionalForwardersRequestRequestTypeDef",
-    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
     "DescribeDirectoriesRequestRequestTypeDef",
-    "DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
     "DescribeDomainControllersRequestRequestTypeDef",
     "DomainControllerTypeDef",
     "DescribeEventTopicsRequestRequestTypeDef",
     "EventTopicTypeDef",
-    "DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
     "DescribeLDAPSSettingsRequestRequestTypeDef",
     "LDAPSSettingInfoTypeDef",
-    "DescribeRegionsRequestDescribeRegionsPaginateTypeDef",
     "DescribeRegionsRequestRequestTypeDef",
     "DescribeSettingsRequestRequestTypeDef",
     "SettingEntryTypeDef",
-    "DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
     "DescribeSharedDirectoriesRequestRequestTypeDef",
-    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
-    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
     "DescribeTrustsRequestRequestTypeDef",
     "TrustTypeDef",
-    "DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
     "DescribeUpdateDirectoryRequestRequestTypeDef",
     "DirectoryConnectSettingsDescriptionTypeDef",
     "DirectoryVpcSettingsDescriptionTypeDef",
-    "RadiusSettingsTypeDef",
+    "RadiusSettingsOutputTypeDef",
     "RegionsInfoTypeDef",
     "DirectoryLimitsTypeDef",
+    "DirectoryVpcSettingsOutputTypeDef",
     "DisableClientAuthenticationRequestRequestTypeDef",
     "DisableLDAPSRequestRequestTypeDef",
     "DisableRadiusRequestRequestTypeDef",
     "DisableSsoRequestRequestTypeDef",
     "EnableClientAuthenticationRequestRequestTypeDef",
     "EnableLDAPSRequestRequestTypeDef",
+    "RadiusSettingsTypeDef",
     "EnableSsoRequestRequestTypeDef",
     "GetSnapshotLimitsRequestRequestTypeDef",
     "SnapshotLimitsTypeDef",
     "IpRouteInfoTypeDef",
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
-    "ListIpRoutesRequestListIpRoutesPaginateTypeDef",
     "ListIpRoutesRequestRequestTypeDef",
-    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
     "ListLogSubscriptionsRequestRequestTypeDef",
     "LogSubscriptionTypeDef",
-    "ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
     "ListSchemaExtensionsRequestRequestTypeDef",
     "SchemaExtensionInfoTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OSUpdateSettingsTypeDef",
-    "PaginatorConfigTypeDef",
-    "RegisterCertificateResultTypeDef",
     "RegisterEventTopicRequestRequestTypeDef",
     "RejectSharedDirectoryRequestRequestTypeDef",
-    "RejectSharedDirectoryResultTypeDef",
     "RemoveIpRoutesRequestRequestTypeDef",
     "RemoveRegionRequestRequestTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetUserPasswordRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "SettingTypeDef",
     "ShareTargetTypeDef",
-    "ShareDirectoryResultTypeDef",
     "StartSchemaExtensionRequestRequestTypeDef",
-    "StartSchemaExtensionResultTypeDef",
     "UnshareTargetTypeDef",
-    "UnshareDirectoryResultTypeDef",
     "UpdateConditionalForwarderRequestRequestTypeDef",
     "UpdateNumberOfDomainControllersRequestRequestTypeDef",
-    "UpdateSettingsResultTypeDef",
     "UpdateTrustRequestRequestTypeDef",
-    "UpdateTrustResultTypeDef",
     "VerifyTrustRequestRequestTypeDef",
+    "ConnectDirectoryResultTypeDef",
+    "CreateAliasResultTypeDef",
+    "CreateDirectoryResultTypeDef",
+    "CreateMicrosoftADResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "CreateTrustResultTypeDef",
+    "DeleteDirectoryResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DeleteTrustResultTypeDef",
+    "RegisterCertificateResultTypeDef",
+    "RejectSharedDirectoryResultTypeDef",
+    "ShareDirectoryResultTypeDef",
+    "StartSchemaExtensionResultTypeDef",
+    "UnshareDirectoryResultTypeDef",
+    "UpdateSettingsResultTypeDef",
+    "UpdateTrustResultTypeDef",
     "VerifyTrustResultTypeDef",
     "AcceptSharedDirectoryResultTypeDef",
     "DescribeSharedDirectoriesResultTypeDef",
     "AddIpRoutesRequestRequestTypeDef",
     "AddRegionRequestRequestTypeDef",
-    "RegionDescriptionTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
     "CreateMicrosoftADRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "ComputerTypeDef",
     "CreateComputerRequestRequestTypeDef",
     "ListCertificatesResultTypeDef",
     "CertificateTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
     "DescribeClientAuthenticationSettingsResultTypeDef",
     "DescribeConditionalForwardersResultTypeDef",
     "ConnectDirectoryRequestRequestTypeDef",
+    "DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
+    "DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
+    "DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
+    "DescribeRegionsRequestDescribeRegionsPaginateTypeDef",
+    "DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
+    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
+    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
+    "DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListIpRoutesRequestListIpRoutesPaginateTypeDef",
+    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
+    "ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeDomainControllersResultTypeDef",
     "DescribeEventTopicsResultTypeDef",
     "DescribeLDAPSSettingsResultTypeDef",
     "DescribeSettingsResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "DescribeTrustsResultTypeDef",
-    "EnableRadiusRequestRequestTypeDef",
     "OwnerDirectoryDescriptionTypeDef",
-    "UpdateRadiusRequestRequestTypeDef",
     "GetDirectoryLimitsResultTypeDef",
+    "DirectoryVpcSettingsUnionTypeDef",
+    "RegionDescriptionTypeDef",
+    "EnableRadiusRequestRequestTypeDef",
+    "RadiusSettingsUnionTypeDef",
+    "UpdateRadiusRequestRequestTypeDef",
     "GetSnapshotLimitsResultTypeDef",
     "ListIpRoutesResultTypeDef",
     "ListLogSubscriptionsResultTypeDef",
     "ListSchemaExtensionsResultTypeDef",
     "UpdateDirectorySetupRequestRequestTypeDef",
     "UpdateValueTypeDef",
     "UpdateSettingsRequestRequestTypeDef",
     "ShareDirectoryRequestRequestTypeDef",
     "UnshareDirectoryRequestRequestTypeDef",
-    "DescribeRegionsResultTypeDef",
     "CreateComputerResultTypeDef",
     "DescribeCertificateResultTypeDef",
     "DirectoryDescriptionTypeDef",
+    "DescribeRegionsResultTypeDef",
     "UpdateInfoEntryTypeDef",
     "DescribeDirectoriesResultTypeDef",
     "DescribeUpdateDirectoryResultTypeDef",
 )
 
 AcceptSharedDirectoryRequestRequestTypeDef = TypedDict(
     "AcceptSharedDirectoryRequestRequestTypeDef",
     {
         "SharedDirectoryId": str,
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
 SharedDirectoryTypeDef = TypedDict(
     "SharedDirectoryTypeDef",
     {
         "OwnerAccountId": str,
         "OwnerDirectoryId": str,
         "ShareMethod": ShareMethodType,
         "SharedAccountId": str,
@@ -326,101 +340,58 @@
         "VpcId": str,
         "SubnetIds": Sequence[str],
         "CustomerDnsIps": Sequence[str],
         "CustomerUserName": str,
     },
 )
 
-ConnectDirectoryResultTypeDef = TypedDict(
-    "ConnectDirectoryResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateAliasRequestRequestTypeDef = TypedDict(
     "CreateAliasRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Alias": str,
     },
 )
 
-CreateAliasResultTypeDef = TypedDict(
-    "CreateAliasResultTypeDef",
-    {
-        "DirectoryId": str,
-        "Alias": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateConditionalForwarderRequestRequestTypeDef = TypedDict(
     "CreateConditionalForwarderRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
         "DnsIpAddrs": Sequence[str],
     },
 )
 
-CreateDirectoryResultTypeDef = TypedDict(
-    "CreateDirectoryResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateLogSubscriptionRequestRequestTypeDef = TypedDict(
     "CreateLogSubscriptionRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "LogGroupName": str,
     },
 )
 
-CreateMicrosoftADResultTypeDef = TypedDict(
-    "CreateMicrosoftADResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSnapshotRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "SnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateTrustRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
         "TrustPassword": str,
         "TrustDirection": TrustDirectionType,
@@ -432,29 +403,19 @@
         "TrustType": TrustTypeType,
         "ConditionalForwarderIpAddrs": Sequence[str],
         "SelectiveAuth": SelectiveAuthType,
     },
     total=False,
 )
 
-
 class CreateTrustRequestRequestTypeDef(
     _RequiredCreateTrustRequestRequestTypeDef, _OptionalCreateTrustRequestRequestTypeDef
 ):
     pass
 
-
-CreateTrustResultTypeDef = TypedDict(
-    "CreateTrustResultTypeDef",
-    {
-        "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteConditionalForwarderRequestRequestTypeDef = TypedDict(
     "DeleteConditionalForwarderRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
     },
 )
@@ -462,73 +423,47 @@
 DeleteDirectoryRequestRequestTypeDef = TypedDict(
     "DeleteDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
-DeleteDirectoryResultTypeDef = TypedDict(
-    "DeleteDirectoryResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLogSubscriptionRequestRequestTypeDef = TypedDict(
     "DeleteLogSubscriptionRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
 DeleteSnapshotRequestRequestTypeDef = TypedDict(
     "DeleteSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "SnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTrustRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTrustRequestRequestTypeDef",
     {
         "TrustId": str,
     },
 )
 _OptionalDeleteTrustRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteTrustRequestRequestTypeDef",
     {
         "DeleteAssociatedConditionalForwarder": bool,
     },
     total=False,
 )
 
-
 class DeleteTrustRequestRequestTypeDef(
     _RequiredDeleteTrustRequestRequestTypeDef, _OptionalDeleteTrustRequestRequestTypeDef
 ):
     pass
 
-
-DeleteTrustResultTypeDef = TypedDict(
-    "DeleteTrustResultTypeDef",
-    {
-        "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeregisterCertificateRequestRequestTypeDef = TypedDict(
     "DeregisterCertificateRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CertificateId": str,
     },
 )
@@ -545,37 +480,24 @@
     "DescribeCertificateRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CertificateId": str,
     },
 )
 
-_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Type": ClientAuthenticationTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef(
-    _RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
-    _OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeClientAuthenticationSettingsRequestRequestTypeDef = TypedDict(
@@ -584,86 +506,50 @@
         "Type": ClientAuthenticationTypeType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class DescribeClientAuthenticationSettingsRequestRequestTypeDef(
     _RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef,
     _OptionalDescribeClientAuthenticationSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeConditionalForwardersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConditionalForwardersRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeConditionalForwardersRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeConditionalForwardersRequestRequestTypeDef",
     {
         "RemoteDomainNames": Sequence[str],
     },
     total=False,
 )
 
-
 class DescribeConditionalForwardersRequestRequestTypeDef(
     _RequiredDescribeConditionalForwardersRequestRequestTypeDef,
     _OptionalDescribeConditionalForwardersRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef = TypedDict(
-    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
-    {
-        "DirectoryIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDirectoriesRequestRequestTypeDef = TypedDict(
     "DescribeDirectoriesRequestRequestTypeDef",
     {
         "DirectoryIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
-    {
-        "DomainControllerIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef(
-    _RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
-    _OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeDomainControllersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDomainControllersRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeDomainControllersRequestRequestTypeDef = TypedDict(
@@ -672,22 +558,20 @@
         "DomainControllerIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class DescribeDomainControllersRequestRequestTypeDef(
     _RequiredDescribeDomainControllersRequestRequestTypeDef,
     _OptionalDescribeDomainControllersRequestRequestTypeDef,
 ):
     pass
 
-
 DomainControllerTypeDef = TypedDict(
     "DomainControllerTypeDef",
     {
         "DirectoryId": str,
         "DomainControllerId": str,
         "DnsIpAddr": str,
         "VpcId": str,
@@ -718,37 +602,14 @@
         "TopicArn": str,
         "CreatedDateTime": datetime,
         "Status": TopicStatusType,
     },
     total=False,
 )
 
-_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
-    {
-        "Type": Literal["Client"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef(
-    _RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
-    _OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeLDAPSSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLDAPSSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeLDAPSSettingsRequestRequestTypeDef = TypedDict(
@@ -757,55 +618,30 @@
         "Type": Literal["Client"],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class DescribeLDAPSSettingsRequestRequestTypeDef(
     _RequiredDescribeLDAPSSettingsRequestRequestTypeDef,
     _OptionalDescribeLDAPSSettingsRequestRequestTypeDef,
 ):
     pass
 
-
 LDAPSSettingInfoTypeDef = TypedDict(
     "LDAPSSettingInfoTypeDef",
     {
         "LDAPSStatus": LDAPSStatusType,
         "LDAPSStatusReason": str,
         "LastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
-    {
-        "RegionName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeRegionsRequestDescribeRegionsPaginateTypeDef(
-    _RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
-    _OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeRegionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRegionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeRegionsRequestRequestTypeDef = TypedDict(
@@ -813,21 +649,19 @@
     {
         "RegionName": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeRegionsRequestRequestTypeDef(
     _RequiredDescribeRegionsRequestRequestTypeDef, _OptionalDescribeRegionsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeSettingsRequestRequestTypeDef = TypedDict(
@@ -835,21 +669,19 @@
     {
         "Status": DirectoryConfigurationStatusType,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeSettingsRequestRequestTypeDef(
     _RequiredDescribeSettingsRequestRequestTypeDef, _OptionalDescribeSettingsRequestRequestTypeDef
 ):
     pass
 
-
 SettingEntryTypeDef = TypedDict(
     "SettingEntryTypeDef",
     {
         "Type": str,
         "Name": str,
         "AllowedValues": str,
         "AppliedValue": str,
@@ -860,37 +692,14 @@
         "LastUpdatedDateTime": datetime,
         "LastRequestedDateTime": datetime,
         "DataType": str,
     },
     total=False,
 )
 
-_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
-    {
-        "OwnerDirectoryId": str,
-    },
-)
-_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
-    {
-        "SharedDirectoryIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef(
-    _RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
-    _OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeSharedDirectoriesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSharedDirectoriesRequestRequestTypeDef",
     {
         "OwnerDirectoryId": str,
     },
 )
 _OptionalDescribeSharedDirectoriesRequestRequestTypeDef = TypedDict(
@@ -899,32 +708,20 @@
         "SharedDirectoryIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class DescribeSharedDirectoriesRequestRequestTypeDef(
     _RequiredDescribeSharedDirectoriesRequestRequestTypeDef,
     _OptionalDescribeSharedDirectoriesRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "SnapshotIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "SnapshotIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
@@ -941,24 +738,14 @@
         "Name": str,
         "Status": SnapshotStatusType,
         "StartTime": datetime,
     },
     total=False,
 )
 
-DescribeTrustsRequestDescribeTrustsPaginateTypeDef = TypedDict(
-    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "TrustIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTrustsRequestRequestTypeDef = TypedDict(
     "DescribeTrustsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "TrustIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
@@ -980,38 +767,14 @@
         "StateLastUpdatedDateTime": datetime,
         "TrustStateReason": str,
         "SelectiveAuth": SelectiveAuthType,
     },
     total=False,
 )
 
-_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
-    "_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "UpdateType": Literal["OS"],
-    },
-)
-_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
-    "_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
-    {
-        "RegionName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef(
-    _RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
-    _OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeUpdateDirectoryRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeUpdateDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UpdateType": Literal["OS"],
     },
 )
@@ -1020,22 +783,20 @@
     {
         "RegionName": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeUpdateDirectoryRequestRequestTypeDef(
     _RequiredDescribeUpdateDirectoryRequestRequestTypeDef,
     _OptionalDescribeUpdateDirectoryRequestRequestTypeDef,
 ):
     pass
 
-
 DirectoryConnectSettingsDescriptionTypeDef = TypedDict(
     "DirectoryConnectSettingsDescriptionTypeDef",
     {
         "VpcId": str,
         "SubnetIds": List[str],
         "CustomerUserName": str,
         "SecurityGroupId": str,
@@ -1052,16 +813,16 @@
         "SubnetIds": List[str],
         "SecurityGroupId": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
-RadiusSettingsTypeDef = TypedDict(
-    "RadiusSettingsTypeDef",
+RadiusSettingsOutputTypeDef = TypedDict(
+    "RadiusSettingsOutputTypeDef",
     {
         "RadiusServers": List[str],
         "RadiusPort": int,
         "RadiusTimeout": int,
         "RadiusRetries": int,
         "SharedSecret": str,
         "AuthenticationProtocol": RadiusAuthenticationProtocolType,
@@ -1092,14 +853,22 @@
         "ConnectedDirectoriesLimit": int,
         "ConnectedDirectoriesCurrentCount": int,
         "ConnectedDirectoriesLimitReached": bool,
     },
     total=False,
 )
 
+DirectoryVpcSettingsOutputTypeDef = TypedDict(
+    "DirectoryVpcSettingsOutputTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+    },
+)
+
 DisableClientAuthenticationRequestRequestTypeDef = TypedDict(
     "DisableClientAuthenticationRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": ClientAuthenticationTypeType,
     },
 )
@@ -1130,21 +899,19 @@
     {
         "UserName": str,
         "Password": str,
     },
     total=False,
 )
 
-
 class DisableSsoRequestRequestTypeDef(
     _RequiredDisableSsoRequestRequestTypeDef, _OptionalDisableSsoRequestRequestTypeDef
 ):
     pass
 
-
 EnableClientAuthenticationRequestRequestTypeDef = TypedDict(
     "EnableClientAuthenticationRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": ClientAuthenticationTypeType,
     },
 )
@@ -1153,14 +920,29 @@
     "EnableLDAPSRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": Literal["Client"],
     },
 )
 
+RadiusSettingsTypeDef = TypedDict(
+    "RadiusSettingsTypeDef",
+    {
+        "RadiusServers": Sequence[str],
+        "RadiusPort": int,
+        "RadiusTimeout": int,
+        "RadiusRetries": int,
+        "SharedSecret": str,
+        "AuthenticationProtocol": RadiusAuthenticationProtocolType,
+        "DisplayLabel": str,
+        "UseSameUsername": bool,
+    },
+    total=False,
+)
+
 _RequiredEnableSsoRequestRequestTypeDef = TypedDict(
     "_RequiredEnableSsoRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalEnableSsoRequestRequestTypeDef = TypedDict(
@@ -1168,21 +950,19 @@
     {
         "UserName": str,
         "Password": str,
     },
     total=False,
 )
 
-
 class EnableSsoRequestRequestTypeDef(
     _RequiredEnableSsoRequestRequestTypeDef, _OptionalEnableSsoRequestRequestTypeDef
 ):
     pass
 
-
 GetSnapshotLimitsRequestRequestTypeDef = TypedDict(
     "GetSnapshotLimitsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
@@ -1205,36 +985,14 @@
         "AddedDateTime": datetime,
         "IpRouteStatusReason": str,
         "Description": str,
     },
     total=False,
 )
 
-_RequiredListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "_RequiredListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "_OptionalListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListCertificatesRequestListCertificatesPaginateTypeDef(
-    _RequiredListCertificatesRequestListCertificatesPaginateTypeDef,
-    _OptionalListCertificatesRequestListCertificatesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCertificatesRequestRequestTypeDef = TypedDict(
     "_RequiredListCertificatesRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListCertificatesRequestRequestTypeDef = TypedDict(
@@ -1242,43 +1000,19 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListCertificatesRequestRequestTypeDef(
     _RequiredListCertificatesRequestRequestTypeDef, _OptionalListCertificatesRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListIpRoutesRequestListIpRoutesPaginateTypeDef(
-    _RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef,
-    _OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListIpRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredListIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListIpRoutesRequestRequestTypeDef = TypedDict(
@@ -1286,30 +1020,19 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListIpRoutesRequestRequestTypeDef(
     _RequiredListIpRoutesRequestRequestTypeDef, _OptionalListIpRoutesRequestRequestTypeDef
 ):
     pass
 
-
-ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef = TypedDict(
-    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLogSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListLogSubscriptionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "NextToken": str,
         "Limit": int,
     },
@@ -1322,36 +1045,14 @@
         "DirectoryId": str,
         "LogGroupName": str,
         "SubscriptionCreatedDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
-    "_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
-    "_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef(
-    _RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
-    _OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSchemaExtensionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemaExtensionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListSchemaExtensionsRequestRequestTypeDef = TypedDict(
@@ -1359,58 +1060,34 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListSchemaExtensionsRequestRequestTypeDef(
     _RequiredListSchemaExtensionsRequestRequestTypeDef,
     _OptionalListSchemaExtensionsRequestRequestTypeDef,
 ):
     pass
 
-
 SchemaExtensionInfoTypeDef = TypedDict(
     "SchemaExtensionInfoTypeDef",
     {
         "DirectoryId": str,
         "SchemaExtensionId": str,
         "Description": str,
         "SchemaExtensionStatus": SchemaExtensionStatusType,
         "SchemaExtensionStatusReason": str,
         "StartDateTime": datetime,
         "EndDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1418,48 +1095,28 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 OSUpdateSettingsTypeDef = TypedDict(
     "OSUpdateSettingsTypeDef",
     {
         "OSVersion": OSVersionType,
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
-RegisterCertificateResultTypeDef = TypedDict(
-    "RegisterCertificateResultTypeDef",
-    {
-        "CertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterEventTopicRequestRequestTypeDef = TypedDict(
     "RegisterEventTopicRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "TopicName": str,
     },
 )
@@ -1467,22 +1124,14 @@
 RejectSharedDirectoryRequestRequestTypeDef = TypedDict(
     "RejectSharedDirectoryRequestRequestTypeDef",
     {
         "SharedDirectoryId": str,
     },
 )
 
-RejectSharedDirectoryResultTypeDef = TypedDict(
-    "RejectSharedDirectoryResultTypeDef",
-    {
-        "SharedDirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveIpRoutesRequestRequestTypeDef = TypedDict(
     "RemoveIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CidrIps": Sequence[str],
     },
 )
@@ -1507,25 +1156,14 @@
     {
         "DirectoryId": str,
         "UserName": str,
         "NewPassword": str,
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
 RestoreFromSnapshotRequestRequestTypeDef = TypedDict(
     "RestoreFromSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 
@@ -1541,56 +1179,32 @@
     "ShareTargetTypeDef",
     {
         "Id": str,
         "Type": Literal["ACCOUNT"],
     },
 )
 
-ShareDirectoryResultTypeDef = TypedDict(
-    "ShareDirectoryResultTypeDef",
-    {
-        "SharedDirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartSchemaExtensionRequestRequestTypeDef = TypedDict(
     "StartSchemaExtensionRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CreateSnapshotBeforeSchemaExtension": bool,
         "LdifContent": str,
         "Description": str,
     },
 )
 
-StartSchemaExtensionResultTypeDef = TypedDict(
-    "StartSchemaExtensionResultTypeDef",
-    {
-        "SchemaExtensionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnshareTargetTypeDef = TypedDict(
     "UnshareTargetTypeDef",
     {
         "Id": str,
         "Type": Literal["ACCOUNT"],
     },
 )
 
-UnshareDirectoryResultTypeDef = TypedDict(
-    "UnshareDirectoryResultTypeDef",
-    {
-        "SharedDirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateConditionalForwarderRequestRequestTypeDef = TypedDict(
     "UpdateConditionalForwarderRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
         "DnsIpAddrs": Sequence[str],
     },
@@ -1600,81 +1214,192 @@
     "UpdateNumberOfDomainControllersRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "DesiredNumber": int,
     },
 )
 
-UpdateSettingsResultTypeDef = TypedDict(
-    "UpdateSettingsResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTrustRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrustRequestRequestTypeDef",
     {
         "TrustId": str,
     },
 )
 _OptionalUpdateTrustRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTrustRequestRequestTypeDef",
     {
         "SelectiveAuth": SelectiveAuthType,
     },
     total=False,
 )
 
-
 class UpdateTrustRequestRequestTypeDef(
     _RequiredUpdateTrustRequestRequestTypeDef, _OptionalUpdateTrustRequestRequestTypeDef
 ):
     pass
 
+VerifyTrustRequestRequestTypeDef = TypedDict(
+    "VerifyTrustRequestRequestTypeDef",
+    {
+        "TrustId": str,
+    },
+)
 
-UpdateTrustResultTypeDef = TypedDict(
-    "UpdateTrustResultTypeDef",
+ConnectDirectoryResultTypeDef = TypedDict(
+    "ConnectDirectoryResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAliasResultTypeDef = TypedDict(
+    "CreateAliasResultTypeDef",
+    {
+        "DirectoryId": str,
+        "Alias": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDirectoryResultTypeDef = TypedDict(
+    "CreateDirectoryResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMicrosoftADResultTypeDef = TypedDict(
+    "CreateMicrosoftADResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "SnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrustResultTypeDef = TypedDict(
+    "CreateTrustResultTypeDef",
     {
-        "RequestId": str,
         "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VerifyTrustRequestRequestTypeDef = TypedDict(
-    "VerifyTrustRequestRequestTypeDef",
+DeleteDirectoryResultTypeDef = TypedDict(
+    "DeleteDirectoryResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "SnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTrustResultTypeDef = TypedDict(
+    "DeleteTrustResultTypeDef",
     {
         "TrustId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCertificateResultTypeDef = TypedDict(
+    "RegisterCertificateResultTypeDef",
+    {
+        "CertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RejectSharedDirectoryResultTypeDef = TypedDict(
+    "RejectSharedDirectoryResultTypeDef",
+    {
+        "SharedDirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ShareDirectoryResultTypeDef = TypedDict(
+    "ShareDirectoryResultTypeDef",
+    {
+        "SharedDirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSchemaExtensionResultTypeDef = TypedDict(
+    "StartSchemaExtensionResultTypeDef",
+    {
+        "SchemaExtensionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnshareDirectoryResultTypeDef = TypedDict(
+    "UnshareDirectoryResultTypeDef",
+    {
+        "SharedDirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSettingsResultTypeDef = TypedDict(
+    "UpdateSettingsResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrustResultTypeDef = TypedDict(
+    "UpdateTrustResultTypeDef",
+    {
+        "RequestId": str,
+        "TrustId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VerifyTrustResultTypeDef = TypedDict(
     "VerifyTrustResultTypeDef",
     {
         "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptSharedDirectoryResultTypeDef = TypedDict(
     "AcceptSharedDirectoryResultTypeDef",
     {
         "SharedDirectory": SharedDirectoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSharedDirectoriesResultTypeDef = TypedDict(
     "DescribeSharedDirectoriesResultTypeDef",
     {
         "SharedDirectories": List[SharedDirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAddIpRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredAddIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
@@ -1685,46 +1410,28 @@
     "_OptionalAddIpRoutesRequestRequestTypeDef",
     {
         "UpdateSecurityGroupForDirectoryControllers": bool,
     },
     total=False,
 )
 
-
 class AddIpRoutesRequestRequestTypeDef(
     _RequiredAddIpRoutesRequestRequestTypeDef, _OptionalAddIpRoutesRequestRequestTypeDef
 ):
     pass
 
-
 AddRegionRequestRequestTypeDef = TypedDict(
     "AddRegionRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RegionName": str,
         "VPCSettings": DirectoryVpcSettingsTypeDef,
     },
 )
 
-RegionDescriptionTypeDef = TypedDict(
-    "RegionDescriptionTypeDef",
-    {
-        "DirectoryId": str,
-        "RegionName": str,
-        "RegionType": RegionTypeType,
-        "Status": DirectoryStageType,
-        "VpcSettings": DirectoryVpcSettingsTypeDef,
-        "DesiredNumberOfDomainControllers": int,
-        "LaunchTime": datetime,
-        "StatusLastUpdatedDateTime": datetime,
-        "LastUpdatedDateTime": datetime,
-    },
-    total=False,
-)
-
 AddTagsToResourceRequestRequestTypeDef = TypedDict(
     "AddTagsToResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1744,21 +1451,19 @@
         "Description": str,
         "VpcSettings": DirectoryVpcSettingsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDirectoryRequestRequestTypeDef(
     _RequiredCreateDirectoryRequestRequestTypeDef, _OptionalCreateDirectoryRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateMicrosoftADRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMicrosoftADRequestRequestTypeDef",
     {
         "Name": str,
         "Password": str,
         "VpcSettings": DirectoryVpcSettingsTypeDef,
     },
@@ -1770,27 +1475,25 @@
         "Description": str,
         "Edition": DirectoryEditionType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMicrosoftADRequestRequestTypeDef(
     _RequiredCreateMicrosoftADRequestRequestTypeDef, _OptionalCreateMicrosoftADRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComputerTypeDef = TypedDict(
     "ComputerTypeDef",
     {
         "ComputerId": str,
@@ -1813,27 +1516,25 @@
     {
         "OrganizationalUnitDistinguishedName": str,
         "ComputerAttributes": Sequence[AttributeTypeDef],
     },
     total=False,
 )
 
-
 class CreateComputerRequestRequestTypeDef(
     _RequiredCreateComputerRequestRequestTypeDef, _OptionalCreateComputerRequestRequestTypeDef
 ):
     pass
 
-
 ListCertificatesResultTypeDef = TypedDict(
     "ListCertificatesResultTypeDef",
     {
         "NextToken": str,
         "CertificatesInfo": List[CertificateInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateId": str,
@@ -1860,36 +1561,34 @@
     {
         "Type": CertificateTypeType,
         "ClientCertAuthSettings": ClientCertAuthSettingsTypeDef,
     },
     total=False,
 )
 
-
 class RegisterCertificateRequestRequestTypeDef(
     _RequiredRegisterCertificateRequestRequestTypeDef,
     _OptionalRegisterCertificateRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeClientAuthenticationSettingsResultTypeDef = TypedDict(
     "DescribeClientAuthenticationSettingsResultTypeDef",
     {
         "ClientAuthenticationSettingsInfo": List[ClientAuthenticationSettingInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConditionalForwardersResultTypeDef = TypedDict(
     "DescribeConditionalForwardersResultTypeDef",
     {
         "ConditionalForwarders": List[ConditionalForwarderTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConnectDirectoryRequestRequestTypeDef = TypedDict(
     "_RequiredConnectDirectoryRequestRequestTypeDef",
     {
         "Name": str,
@@ -1904,144 +1603,407 @@
         "ShortName": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ConnectDirectoryRequestRequestTypeDef(
     _RequiredConnectDirectoryRequestRequestTypeDef, _OptionalConnectDirectoryRequestRequestTypeDef
 ):
     pass
 
+_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    {
+        "Type": ClientAuthenticationTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef(
+    _RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    _OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+):
+    pass
+
+DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef = TypedDict(
+    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
+    {
+        "DirectoryIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
+    {
+        "DomainControllerIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef(
+    _RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+    _OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
+    {
+        "Type": Literal["Client"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef(
+    _RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+    _OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
+    {
+        "RegionName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeRegionsRequestDescribeRegionsPaginateTypeDef(
+    _RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+    _OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
+    {
+        "OwnerDirectoryId": str,
+    },
+)
+_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
+    {
+        "SharedDirectoryIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef(
+    _RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+    _OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+):
+    pass
+
+DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "SnapshotIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeTrustsRequestDescribeTrustsPaginateTypeDef = TypedDict(
+    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "TrustIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
+    "_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "UpdateType": Literal["OS"],
+    },
+)
+_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
+    "_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
+    {
+        "RegionName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef(
+    _RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+    _OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+):
+    pass
+
+_RequiredListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "_RequiredListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "_OptionalListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListCertificatesRequestListCertificatesPaginateTypeDef(
+    _RequiredListCertificatesRequestListCertificatesPaginateTypeDef,
+    _OptionalListCertificatesRequestListCertificatesPaginateTypeDef,
+):
+    pass
+
+_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListIpRoutesRequestListIpRoutesPaginateTypeDef(
+    _RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef,
+    _OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef,
+):
+    pass
+
+ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef = TypedDict(
+    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
+    "_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
+    "_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef(
+    _RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+    _OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
 
 DescribeDomainControllersResultTypeDef = TypedDict(
     "DescribeDomainControllersResultTypeDef",
     {
         "DomainControllers": List[DomainControllerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventTopicsResultTypeDef = TypedDict(
     "DescribeEventTopicsResultTypeDef",
     {
         "EventTopics": List[EventTopicTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLDAPSSettingsResultTypeDef = TypedDict(
     "DescribeLDAPSSettingsResultTypeDef",
     {
         "LDAPSSettingsInfo": List[LDAPSSettingInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSettingsResultTypeDef = TypedDict(
     "DescribeSettingsResultTypeDef",
     {
         "DirectoryId": str,
         "SettingEntries": List[SettingEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSnapshotsResultTypeDef = TypedDict(
     "DescribeSnapshotsResultTypeDef",
     {
         "Snapshots": List[SnapshotTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustsResultTypeDef = TypedDict(
     "DescribeTrustsResultTypeDef",
     {
         "Trusts": List[TrustTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EnableRadiusRequestRequestTypeDef = TypedDict(
-    "EnableRadiusRequestRequestTypeDef",
-    {
-        "DirectoryId": str,
-        "RadiusSettings": RadiusSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OwnerDirectoryDescriptionTypeDef = TypedDict(
     "OwnerDirectoryDescriptionTypeDef",
     {
         "DirectoryId": str,
         "AccountId": str,
         "DnsIpAddrs": List[str],
         "VpcSettings": DirectoryVpcSettingsDescriptionTypeDef,
-        "RadiusSettings": RadiusSettingsTypeDef,
+        "RadiusSettings": RadiusSettingsOutputTypeDef,
         "RadiusStatus": RadiusStatusType,
     },
     total=False,
 )
 
-UpdateRadiusRequestRequestTypeDef = TypedDict(
-    "UpdateRadiusRequestRequestTypeDef",
+GetDirectoryLimitsResultTypeDef = TypedDict(
+    "GetDirectoryLimitsResultTypeDef",
+    {
+        "DirectoryLimits": DirectoryLimitsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DirectoryVpcSettingsUnionTypeDef = Union[
+    DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef
+]
+RegionDescriptionTypeDef = TypedDict(
+    "RegionDescriptionTypeDef",
+    {
+        "DirectoryId": str,
+        "RegionName": str,
+        "RegionType": RegionTypeType,
+        "Status": DirectoryStageType,
+        "VpcSettings": DirectoryVpcSettingsOutputTypeDef,
+        "DesiredNumberOfDomainControllers": int,
+        "LaunchTime": datetime,
+        "StatusLastUpdatedDateTime": datetime,
+        "LastUpdatedDateTime": datetime,
+    },
+    total=False,
+)
+
+EnableRadiusRequestRequestTypeDef = TypedDict(
+    "EnableRadiusRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
 
-GetDirectoryLimitsResultTypeDef = TypedDict(
-    "GetDirectoryLimitsResultTypeDef",
+RadiusSettingsUnionTypeDef = Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
+UpdateRadiusRequestRequestTypeDef = TypedDict(
+    "UpdateRadiusRequestRequestTypeDef",
     {
-        "DirectoryLimits": DirectoryLimitsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DirectoryId": str,
+        "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
 
 GetSnapshotLimitsResultTypeDef = TypedDict(
     "GetSnapshotLimitsResultTypeDef",
     {
         "SnapshotLimits": SnapshotLimitsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIpRoutesResultTypeDef = TypedDict(
     "ListIpRoutesResultTypeDef",
     {
         "IpRoutesInfo": List[IpRouteInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogSubscriptionsResultTypeDef = TypedDict(
     "ListLogSubscriptionsResultTypeDef",
     {
         "LogSubscriptions": List[LogSubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemaExtensionsResultTypeDef = TypedDict(
     "ListSchemaExtensionsResultTypeDef",
     {
         "SchemaExtensionsInfo": List[SchemaExtensionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateDirectorySetupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDirectorySetupRequestRequestTypeDef",
     {
         "DirectoryId": str,
@@ -2053,22 +2015,20 @@
     {
         "OSUpdateSettings": OSUpdateSettingsTypeDef,
         "CreateSnapshotBeforeUpdate": bool,
     },
     total=False,
 )
 
-
 class UpdateDirectorySetupRequestRequestTypeDef(
     _RequiredUpdateDirectorySetupRequestRequestTypeDef,
     _OptionalUpdateDirectorySetupRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateValueTypeDef = TypedDict(
     "UpdateValueTypeDef",
     {
         "OSUpdateSettings": OSUpdateSettingsTypeDef,
     },
     total=False,
 )
@@ -2093,51 +2053,40 @@
     "_OptionalShareDirectoryRequestRequestTypeDef",
     {
         "ShareNotes": str,
     },
     total=False,
 )
 
-
 class ShareDirectoryRequestRequestTypeDef(
     _RequiredShareDirectoryRequestRequestTypeDef, _OptionalShareDirectoryRequestRequestTypeDef
 ):
     pass
 
-
 UnshareDirectoryRequestRequestTypeDef = TypedDict(
     "UnshareDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UnshareTarget": UnshareTargetTypeDef,
     },
 )
 
-DescribeRegionsResultTypeDef = TypedDict(
-    "DescribeRegionsResultTypeDef",
-    {
-        "RegionsDescription": List[RegionDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateComputerResultTypeDef = TypedDict(
     "CreateComputerResultTypeDef",
     {
         "Computer": ComputerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificateResultTypeDef = TypedDict(
     "DescribeCertificateResultTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DirectoryDescriptionTypeDef = TypedDict(
     "DirectoryDescriptionTypeDef",
     {
         "DirectoryId": str,
@@ -2154,26 +2103,35 @@
         "ShareMethod": ShareMethodType,
         "ShareNotes": str,
         "LaunchTime": datetime,
         "StageLastUpdatedDateTime": datetime,
         "Type": DirectoryTypeType,
         "VpcSettings": DirectoryVpcSettingsDescriptionTypeDef,
         "ConnectSettings": DirectoryConnectSettingsDescriptionTypeDef,
-        "RadiusSettings": RadiusSettingsTypeDef,
+        "RadiusSettings": RadiusSettingsOutputTypeDef,
         "RadiusStatus": RadiusStatusType,
         "StageReason": str,
         "SsoEnabled": bool,
         "DesiredNumberOfDomainControllers": int,
         "OwnerDirectoryDescription": OwnerDirectoryDescriptionTypeDef,
         "RegionsInfo": RegionsInfoTypeDef,
         "OsVersion": OSVersionType,
     },
     total=False,
 )
 
+DescribeRegionsResultTypeDef = TypedDict(
+    "DescribeRegionsResultTypeDef",
+    {
+        "RegionsDescription": List[RegionDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateInfoEntryTypeDef = TypedDict(
     "UpdateInfoEntryTypeDef",
     {
         "Region": str,
         "Status": UpdateStatusType,
         "StatusReason": str,
         "InitiatedBy": str,
@@ -2186,19 +2144,19 @@
 )
 
 DescribeDirectoriesResultTypeDef = TypedDict(
     "DescribeDirectoriesResultTypeDef",
     {
         "DirectoryDescriptions": List[DirectoryDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUpdateDirectoryResultTypeDef = TypedDict(
     "DescribeUpdateDirectoryResultTypeDef",
     {
         "UpdateActivities": List[UpdateInfoEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds/type_defs.pyi` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ds.type_defs import AcceptSharedDirectoryRequestRequestTypeDef
 
-    data: AcceptSharedDirectoryRequestRequestTypeDef = {...}
+    data: AcceptSharedDirectoryRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     CertificateStateType,
     CertificateTypeType,
     ClientAuthenticationStatusType,
     ClientAuthenticationTypeType,
     DirectoryConfigurationStatusType,
@@ -50,181 +50,197 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptSharedDirectoryRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SharedDirectoryTypeDef",
     "IpRouteTypeDef",
     "DirectoryVpcSettingsTypeDef",
     "TagTypeDef",
     "AttributeTypeDef",
     "CancelSchemaExtensionRequestRequestTypeDef",
     "CertificateInfoTypeDef",
     "ClientCertAuthSettingsTypeDef",
     "ClientAuthenticationSettingInfoTypeDef",
     "ConditionalForwarderTypeDef",
     "DirectoryConnectSettingsTypeDef",
-    "ConnectDirectoryResultTypeDef",
     "CreateAliasRequestRequestTypeDef",
-    "CreateAliasResultTypeDef",
     "CreateConditionalForwarderRequestRequestTypeDef",
-    "CreateDirectoryResultTypeDef",
     "CreateLogSubscriptionRequestRequestTypeDef",
-    "CreateMicrosoftADResultTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
-    "CreateSnapshotResultTypeDef",
     "CreateTrustRequestRequestTypeDef",
-    "CreateTrustResultTypeDef",
     "DeleteConditionalForwarderRequestRequestTypeDef",
     "DeleteDirectoryRequestRequestTypeDef",
-    "DeleteDirectoryResultTypeDef",
     "DeleteLogSubscriptionRequestRequestTypeDef",
     "DeleteSnapshotRequestRequestTypeDef",
-    "DeleteSnapshotResultTypeDef",
     "DeleteTrustRequestRequestTypeDef",
-    "DeleteTrustResultTypeDef",
     "DeregisterCertificateRequestRequestTypeDef",
     "DeregisterEventTopicRequestRequestTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
-    "DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClientAuthenticationSettingsRequestRequestTypeDef",
     "DescribeConditionalForwardersRequestRequestTypeDef",
-    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
     "DescribeDirectoriesRequestRequestTypeDef",
-    "DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
     "DescribeDomainControllersRequestRequestTypeDef",
     "DomainControllerTypeDef",
     "DescribeEventTopicsRequestRequestTypeDef",
     "EventTopicTypeDef",
-    "DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
     "DescribeLDAPSSettingsRequestRequestTypeDef",
     "LDAPSSettingInfoTypeDef",
-    "DescribeRegionsRequestDescribeRegionsPaginateTypeDef",
     "DescribeRegionsRequestRequestTypeDef",
     "DescribeSettingsRequestRequestTypeDef",
     "SettingEntryTypeDef",
-    "DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
     "DescribeSharedDirectoriesRequestRequestTypeDef",
-    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
     "DescribeSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
-    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
     "DescribeTrustsRequestRequestTypeDef",
     "TrustTypeDef",
-    "DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
     "DescribeUpdateDirectoryRequestRequestTypeDef",
     "DirectoryConnectSettingsDescriptionTypeDef",
     "DirectoryVpcSettingsDescriptionTypeDef",
-    "RadiusSettingsTypeDef",
+    "RadiusSettingsOutputTypeDef",
     "RegionsInfoTypeDef",
     "DirectoryLimitsTypeDef",
+    "DirectoryVpcSettingsOutputTypeDef",
     "DisableClientAuthenticationRequestRequestTypeDef",
     "DisableLDAPSRequestRequestTypeDef",
     "DisableRadiusRequestRequestTypeDef",
     "DisableSsoRequestRequestTypeDef",
     "EnableClientAuthenticationRequestRequestTypeDef",
     "EnableLDAPSRequestRequestTypeDef",
+    "RadiusSettingsTypeDef",
     "EnableSsoRequestRequestTypeDef",
     "GetSnapshotLimitsRequestRequestTypeDef",
     "SnapshotLimitsTypeDef",
     "IpRouteInfoTypeDef",
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
-    "ListIpRoutesRequestListIpRoutesPaginateTypeDef",
     "ListIpRoutesRequestRequestTypeDef",
-    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
     "ListLogSubscriptionsRequestRequestTypeDef",
     "LogSubscriptionTypeDef",
-    "ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
     "ListSchemaExtensionsRequestRequestTypeDef",
     "SchemaExtensionInfoTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "OSUpdateSettingsTypeDef",
-    "PaginatorConfigTypeDef",
-    "RegisterCertificateResultTypeDef",
     "RegisterEventTopicRequestRequestTypeDef",
     "RejectSharedDirectoryRequestRequestTypeDef",
-    "RejectSharedDirectoryResultTypeDef",
     "RemoveIpRoutesRequestRequestTypeDef",
     "RemoveRegionRequestRequestTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetUserPasswordRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "SettingTypeDef",
     "ShareTargetTypeDef",
-    "ShareDirectoryResultTypeDef",
     "StartSchemaExtensionRequestRequestTypeDef",
-    "StartSchemaExtensionResultTypeDef",
     "UnshareTargetTypeDef",
-    "UnshareDirectoryResultTypeDef",
     "UpdateConditionalForwarderRequestRequestTypeDef",
     "UpdateNumberOfDomainControllersRequestRequestTypeDef",
-    "UpdateSettingsResultTypeDef",
     "UpdateTrustRequestRequestTypeDef",
-    "UpdateTrustResultTypeDef",
     "VerifyTrustRequestRequestTypeDef",
+    "ConnectDirectoryResultTypeDef",
+    "CreateAliasResultTypeDef",
+    "CreateDirectoryResultTypeDef",
+    "CreateMicrosoftADResultTypeDef",
+    "CreateSnapshotResultTypeDef",
+    "CreateTrustResultTypeDef",
+    "DeleteDirectoryResultTypeDef",
+    "DeleteSnapshotResultTypeDef",
+    "DeleteTrustResultTypeDef",
+    "RegisterCertificateResultTypeDef",
+    "RejectSharedDirectoryResultTypeDef",
+    "ShareDirectoryResultTypeDef",
+    "StartSchemaExtensionResultTypeDef",
+    "UnshareDirectoryResultTypeDef",
+    "UpdateSettingsResultTypeDef",
+    "UpdateTrustResultTypeDef",
     "VerifyTrustResultTypeDef",
     "AcceptSharedDirectoryResultTypeDef",
     "DescribeSharedDirectoriesResultTypeDef",
     "AddIpRoutesRequestRequestTypeDef",
     "AddRegionRequestRequestTypeDef",
-    "RegionDescriptionTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
     "CreateMicrosoftADRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "ComputerTypeDef",
     "CreateComputerRequestRequestTypeDef",
     "ListCertificatesResultTypeDef",
     "CertificateTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
     "DescribeClientAuthenticationSettingsResultTypeDef",
     "DescribeConditionalForwardersResultTypeDef",
     "ConnectDirectoryRequestRequestTypeDef",
+    "DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
+    "DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
+    "DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
+    "DescribeRegionsRequestDescribeRegionsPaginateTypeDef",
+    "DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
+    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
+    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
+    "DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListIpRoutesRequestListIpRoutesPaginateTypeDef",
+    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
+    "ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeDomainControllersResultTypeDef",
     "DescribeEventTopicsResultTypeDef",
     "DescribeLDAPSSettingsResultTypeDef",
     "DescribeSettingsResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "DescribeTrustsResultTypeDef",
-    "EnableRadiusRequestRequestTypeDef",
     "OwnerDirectoryDescriptionTypeDef",
-    "UpdateRadiusRequestRequestTypeDef",
     "GetDirectoryLimitsResultTypeDef",
+    "DirectoryVpcSettingsUnionTypeDef",
+    "RegionDescriptionTypeDef",
+    "EnableRadiusRequestRequestTypeDef",
+    "RadiusSettingsUnionTypeDef",
+    "UpdateRadiusRequestRequestTypeDef",
     "GetSnapshotLimitsResultTypeDef",
     "ListIpRoutesResultTypeDef",
     "ListLogSubscriptionsResultTypeDef",
     "ListSchemaExtensionsResultTypeDef",
     "UpdateDirectorySetupRequestRequestTypeDef",
     "UpdateValueTypeDef",
     "UpdateSettingsRequestRequestTypeDef",
     "ShareDirectoryRequestRequestTypeDef",
     "UnshareDirectoryRequestRequestTypeDef",
-    "DescribeRegionsResultTypeDef",
     "CreateComputerResultTypeDef",
     "DescribeCertificateResultTypeDef",
     "DirectoryDescriptionTypeDef",
+    "DescribeRegionsResultTypeDef",
     "UpdateInfoEntryTypeDef",
     "DescribeDirectoriesResultTypeDef",
     "DescribeUpdateDirectoryResultTypeDef",
 )
 
 AcceptSharedDirectoryRequestRequestTypeDef = TypedDict(
     "AcceptSharedDirectoryRequestRequestTypeDef",
     {
         "SharedDirectoryId": str,
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
 SharedDirectoryTypeDef = TypedDict(
     "SharedDirectoryTypeDef",
     {
         "OwnerAccountId": str,
         "OwnerDirectoryId": str,
         "ShareMethod": ShareMethodType,
         "SharedAccountId": str,
@@ -325,98 +341,59 @@
         "VpcId": str,
         "SubnetIds": Sequence[str],
         "CustomerDnsIps": Sequence[str],
         "CustomerUserName": str,
     },
 )
 
-ConnectDirectoryResultTypeDef = TypedDict(
-    "ConnectDirectoryResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateAliasRequestRequestTypeDef = TypedDict(
     "CreateAliasRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Alias": str,
     },
 )
 
-CreateAliasResultTypeDef = TypedDict(
-    "CreateAliasResultTypeDef",
-    {
-        "DirectoryId": str,
-        "Alias": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateConditionalForwarderRequestRequestTypeDef = TypedDict(
     "CreateConditionalForwarderRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
         "DnsIpAddrs": Sequence[str],
     },
 )
 
-CreateDirectoryResultTypeDef = TypedDict(
-    "CreateDirectoryResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateLogSubscriptionRequestRequestTypeDef = TypedDict(
     "CreateLogSubscriptionRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "LogGroupName": str,
     },
 )
 
-CreateMicrosoftADResultTypeDef = TypedDict(
-    "CreateMicrosoftADResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSnapshotRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
-CreateSnapshotResultTypeDef = TypedDict(
-    "CreateSnapshotResultTypeDef",
-    {
-        "SnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateTrustRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrustRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
         "TrustPassword": str,
@@ -429,26 +406,20 @@
         "TrustType": TrustTypeType,
         "ConditionalForwarderIpAddrs": Sequence[str],
         "SelectiveAuth": SelectiveAuthType,
     },
     total=False,
 )
 
+
 class CreateTrustRequestRequestTypeDef(
     _RequiredCreateTrustRequestRequestTypeDef, _OptionalCreateTrustRequestRequestTypeDef
 ):
     pass
 
-CreateTrustResultTypeDef = TypedDict(
-    "CreateTrustResultTypeDef",
-    {
-        "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteConditionalForwarderRequestRequestTypeDef = TypedDict(
     "DeleteConditionalForwarderRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
     },
@@ -457,70 +428,48 @@
 DeleteDirectoryRequestRequestTypeDef = TypedDict(
     "DeleteDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
-DeleteDirectoryResultTypeDef = TypedDict(
-    "DeleteDirectoryResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLogSubscriptionRequestRequestTypeDef = TypedDict(
     "DeleteLogSubscriptionRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
 DeleteSnapshotRequestRequestTypeDef = TypedDict(
     "DeleteSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 
-DeleteSnapshotResultTypeDef = TypedDict(
-    "DeleteSnapshotResultTypeDef",
-    {
-        "SnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTrustRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteTrustRequestRequestTypeDef",
     {
         "TrustId": str,
     },
 )
 _OptionalDeleteTrustRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteTrustRequestRequestTypeDef",
     {
         "DeleteAssociatedConditionalForwarder": bool,
     },
     total=False,
 )
 
+
 class DeleteTrustRequestRequestTypeDef(
     _RequiredDeleteTrustRequestRequestTypeDef, _OptionalDeleteTrustRequestRequestTypeDef
 ):
     pass
 
-DeleteTrustResultTypeDef = TypedDict(
-    "DeleteTrustResultTypeDef",
-    {
-        "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeregisterCertificateRequestRequestTypeDef = TypedDict(
     "DeregisterCertificateRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CertificateId": str,
     },
@@ -538,35 +487,24 @@
     "DescribeCertificateRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CertificateId": str,
     },
 )
 
-_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Type": ClientAuthenticationTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef(
-    _RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
-    _OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeClientAuthenticationSettingsRequestRequestTypeDef = TypedDict(
@@ -575,80 +513,54 @@
         "Type": ClientAuthenticationTypeType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class DescribeClientAuthenticationSettingsRequestRequestTypeDef(
     _RequiredDescribeClientAuthenticationSettingsRequestRequestTypeDef,
     _OptionalDescribeClientAuthenticationSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeConditionalForwardersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConditionalForwardersRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeConditionalForwardersRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeConditionalForwardersRequestRequestTypeDef",
     {
         "RemoteDomainNames": Sequence[str],
     },
     total=False,
 )
 
+
 class DescribeConditionalForwardersRequestRequestTypeDef(
     _RequiredDescribeConditionalForwardersRequestRequestTypeDef,
     _OptionalDescribeConditionalForwardersRequestRequestTypeDef,
 ):
     pass
 
-DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef = TypedDict(
-    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
-    {
-        "DirectoryIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeDirectoriesRequestRequestTypeDef = TypedDict(
     "DescribeDirectoriesRequestRequestTypeDef",
     {
         "DirectoryIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
-    {
-        "DomainControllerIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef(
-    _RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
-    _OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeDomainControllersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDomainControllersRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeDomainControllersRequestRequestTypeDef = TypedDict(
@@ -657,20 +569,22 @@
         "DomainControllerIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class DescribeDomainControllersRequestRequestTypeDef(
     _RequiredDescribeDomainControllersRequestRequestTypeDef,
     _OptionalDescribeDomainControllersRequestRequestTypeDef,
 ):
     pass
 
+
 DomainControllerTypeDef = TypedDict(
     "DomainControllerTypeDef",
     {
         "DirectoryId": str,
         "DomainControllerId": str,
         "DnsIpAddr": str,
         "VpcId": str,
@@ -701,35 +615,14 @@
         "TopicArn": str,
         "CreatedDateTime": datetime,
         "Status": TopicStatusType,
     },
     total=False,
 )
 
-_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
-    {
-        "Type": Literal["Client"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef(
-    _RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
-    _OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeLDAPSSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLDAPSSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeLDAPSSettingsRequestRequestTypeDef = TypedDict(
@@ -738,51 +631,32 @@
         "Type": Literal["Client"],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class DescribeLDAPSSettingsRequestRequestTypeDef(
     _RequiredDescribeLDAPSSettingsRequestRequestTypeDef,
     _OptionalDescribeLDAPSSettingsRequestRequestTypeDef,
 ):
     pass
 
+
 LDAPSSettingInfoTypeDef = TypedDict(
     "LDAPSSettingInfoTypeDef",
     {
         "LDAPSStatus": LDAPSStatusType,
         "LDAPSStatusReason": str,
         "LastUpdatedDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
-    {
-        "RegionName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeRegionsRequestDescribeRegionsPaginateTypeDef(
-    _RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
-    _OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeRegionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRegionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeRegionsRequestRequestTypeDef = TypedDict(
@@ -790,19 +664,21 @@
     {
         "RegionName": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeRegionsRequestRequestTypeDef(
     _RequiredDescribeRegionsRequestRequestTypeDef, _OptionalDescribeRegionsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSettingsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalDescribeSettingsRequestRequestTypeDef = TypedDict(
@@ -810,19 +686,21 @@
     {
         "Status": DirectoryConfigurationStatusType,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeSettingsRequestRequestTypeDef(
     _RequiredDescribeSettingsRequestRequestTypeDef, _OptionalDescribeSettingsRequestRequestTypeDef
 ):
     pass
 
+
 SettingEntryTypeDef = TypedDict(
     "SettingEntryTypeDef",
     {
         "Type": str,
         "Name": str,
         "AllowedValues": str,
         "AppliedValue": str,
@@ -833,35 +711,14 @@
         "LastUpdatedDateTime": datetime,
         "LastRequestedDateTime": datetime,
         "DataType": str,
     },
     total=False,
 )
 
-_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
-    {
-        "OwnerDirectoryId": str,
-    },
-)
-_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
-    {
-        "SharedDirectoryIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef(
-    _RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
-    _OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeSharedDirectoriesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSharedDirectoriesRequestRequestTypeDef",
     {
         "OwnerDirectoryId": str,
     },
 )
 _OptionalDescribeSharedDirectoriesRequestRequestTypeDef = TypedDict(
@@ -870,29 +727,21 @@
         "SharedDirectoryIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class DescribeSharedDirectoriesRequestRequestTypeDef(
     _RequiredDescribeSharedDirectoriesRequestRequestTypeDef,
     _OptionalDescribeSharedDirectoriesRequestRequestTypeDef,
 ):
     pass
 
-DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
-    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "SnapshotIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeSnapshotsRequestRequestTypeDef = TypedDict(
     "DescribeSnapshotsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "SnapshotIds": Sequence[str],
         "NextToken": str,
@@ -910,24 +759,14 @@
         "Name": str,
         "Status": SnapshotStatusType,
         "StartTime": datetime,
     },
     total=False,
 )
 
-DescribeTrustsRequestDescribeTrustsPaginateTypeDef = TypedDict(
-    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "TrustIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeTrustsRequestRequestTypeDef = TypedDict(
     "DescribeTrustsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "TrustIds": Sequence[str],
         "NextToken": str,
         "Limit": int,
@@ -949,36 +788,14 @@
         "StateLastUpdatedDateTime": datetime,
         "TrustStateReason": str,
         "SelectiveAuth": SelectiveAuthType,
     },
     total=False,
 )
 
-_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
-    "_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "UpdateType": Literal["OS"],
-    },
-)
-_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
-    "_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
-    {
-        "RegionName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef(
-    _RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
-    _OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeUpdateDirectoryRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeUpdateDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UpdateType": Literal["OS"],
     },
 )
@@ -987,20 +804,22 @@
     {
         "RegionName": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeUpdateDirectoryRequestRequestTypeDef(
     _RequiredDescribeUpdateDirectoryRequestRequestTypeDef,
     _OptionalDescribeUpdateDirectoryRequestRequestTypeDef,
 ):
     pass
 
+
 DirectoryConnectSettingsDescriptionTypeDef = TypedDict(
     "DirectoryConnectSettingsDescriptionTypeDef",
     {
         "VpcId": str,
         "SubnetIds": List[str],
         "CustomerUserName": str,
         "SecurityGroupId": str,
@@ -1017,16 +836,16 @@
         "SubnetIds": List[str],
         "SecurityGroupId": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
-RadiusSettingsTypeDef = TypedDict(
-    "RadiusSettingsTypeDef",
+RadiusSettingsOutputTypeDef = TypedDict(
+    "RadiusSettingsOutputTypeDef",
     {
         "RadiusServers": List[str],
         "RadiusPort": int,
         "RadiusTimeout": int,
         "RadiusRetries": int,
         "SharedSecret": str,
         "AuthenticationProtocol": RadiusAuthenticationProtocolType,
@@ -1057,14 +876,22 @@
         "ConnectedDirectoriesLimit": int,
         "ConnectedDirectoriesCurrentCount": int,
         "ConnectedDirectoriesLimitReached": bool,
     },
     total=False,
 )
 
+DirectoryVpcSettingsOutputTypeDef = TypedDict(
+    "DirectoryVpcSettingsOutputTypeDef",
+    {
+        "VpcId": str,
+        "SubnetIds": List[str],
+    },
+)
+
 DisableClientAuthenticationRequestRequestTypeDef = TypedDict(
     "DisableClientAuthenticationRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": ClientAuthenticationTypeType,
     },
 )
@@ -1095,19 +922,21 @@
     {
         "UserName": str,
         "Password": str,
     },
     total=False,
 )
 
+
 class DisableSsoRequestRequestTypeDef(
     _RequiredDisableSsoRequestRequestTypeDef, _OptionalDisableSsoRequestRequestTypeDef
 ):
     pass
 
+
 EnableClientAuthenticationRequestRequestTypeDef = TypedDict(
     "EnableClientAuthenticationRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": ClientAuthenticationTypeType,
     },
 )
@@ -1116,14 +945,29 @@
     "EnableLDAPSRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": Literal["Client"],
     },
 )
 
+RadiusSettingsTypeDef = TypedDict(
+    "RadiusSettingsTypeDef",
+    {
+        "RadiusServers": Sequence[str],
+        "RadiusPort": int,
+        "RadiusTimeout": int,
+        "RadiusRetries": int,
+        "SharedSecret": str,
+        "AuthenticationProtocol": RadiusAuthenticationProtocolType,
+        "DisplayLabel": str,
+        "UseSameUsername": bool,
+    },
+    total=False,
+)
+
 _RequiredEnableSsoRequestRequestTypeDef = TypedDict(
     "_RequiredEnableSsoRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalEnableSsoRequestRequestTypeDef = TypedDict(
@@ -1131,19 +975,21 @@
     {
         "UserName": str,
         "Password": str,
     },
     total=False,
 )
 
+
 class EnableSsoRequestRequestTypeDef(
     _RequiredEnableSsoRequestRequestTypeDef, _OptionalEnableSsoRequestRequestTypeDef
 ):
     pass
 
+
 GetSnapshotLimitsRequestRequestTypeDef = TypedDict(
     "GetSnapshotLimitsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 
@@ -1166,34 +1012,14 @@
         "AddedDateTime": datetime,
         "IpRouteStatusReason": str,
         "Description": str,
     },
     total=False,
 )
 
-_RequiredListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "_RequiredListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "_OptionalListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListCertificatesRequestListCertificatesPaginateTypeDef(
-    _RequiredListCertificatesRequestListCertificatesPaginateTypeDef,
-    _OptionalListCertificatesRequestListCertificatesPaginateTypeDef,
-):
-    pass
-
 _RequiredListCertificatesRequestRequestTypeDef = TypedDict(
     "_RequiredListCertificatesRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListCertificatesRequestRequestTypeDef = TypedDict(
@@ -1201,38 +1027,20 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListCertificatesRequestRequestTypeDef(
     _RequiredListCertificatesRequestRequestTypeDef, _OptionalListCertificatesRequestRequestTypeDef
 ):
     pass
 
-_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListIpRoutesRequestListIpRoutesPaginateTypeDef(
-    _RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef,
-    _OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef,
-):
-    pass
 
 _RequiredListIpRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredListIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
@@ -1241,27 +1049,20 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListIpRoutesRequestRequestTypeDef(
     _RequiredListIpRoutesRequestRequestTypeDef, _OptionalListIpRoutesRequestRequestTypeDef
 ):
     pass
 
-ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef = TypedDict(
-    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListLogSubscriptionsRequestRequestTypeDef = TypedDict(
     "ListLogSubscriptionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "NextToken": str,
         "Limit": int,
@@ -1275,34 +1076,14 @@
         "DirectoryId": str,
         "LogGroupName": str,
         "SubscriptionCreatedDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
-    "_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
-    {
-        "DirectoryId": str,
-    },
-)
-_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
-    "_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef(
-    _RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
-    _OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListSchemaExtensionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemaExtensionsRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalListSchemaExtensionsRequestRequestTypeDef = TypedDict(
@@ -1310,54 +1091,36 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListSchemaExtensionsRequestRequestTypeDef(
     _RequiredListSchemaExtensionsRequestRequestTypeDef,
     _OptionalListSchemaExtensionsRequestRequestTypeDef,
 ):
     pass
 
+
 SchemaExtensionInfoTypeDef = TypedDict(
     "SchemaExtensionInfoTypeDef",
     {
         "DirectoryId": str,
         "SchemaExtensionId": str,
         "Description": str,
         "SchemaExtensionStatus": SchemaExtensionStatusType,
         "SchemaExtensionStatusReason": str,
         "StartDateTime": datetime,
         "EndDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1365,46 +1128,30 @@
     {
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 OSUpdateSettingsTypeDef = TypedDict(
     "OSUpdateSettingsTypeDef",
     {
         "OSVersion": OSVersionType,
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
-RegisterCertificateResultTypeDef = TypedDict(
-    "RegisterCertificateResultTypeDef",
-    {
-        "CertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterEventTopicRequestRequestTypeDef = TypedDict(
     "RegisterEventTopicRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "TopicName": str,
     },
 )
@@ -1412,22 +1159,14 @@
 RejectSharedDirectoryRequestRequestTypeDef = TypedDict(
     "RejectSharedDirectoryRequestRequestTypeDef",
     {
         "SharedDirectoryId": str,
     },
 )
 
-RejectSharedDirectoryResultTypeDef = TypedDict(
-    "RejectSharedDirectoryResultTypeDef",
-    {
-        "SharedDirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveIpRoutesRequestRequestTypeDef = TypedDict(
     "RemoveIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CidrIps": Sequence[str],
     },
 )
@@ -1452,25 +1191,14 @@
     {
         "DirectoryId": str,
         "UserName": str,
         "NewPassword": str,
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
 RestoreFromSnapshotRequestRequestTypeDef = TypedDict(
     "RestoreFromSnapshotRequestRequestTypeDef",
     {
         "SnapshotId": str,
     },
 )
 
@@ -1486,56 +1214,32 @@
     "ShareTargetTypeDef",
     {
         "Id": str,
         "Type": Literal["ACCOUNT"],
     },
 )
 
-ShareDirectoryResultTypeDef = TypedDict(
-    "ShareDirectoryResultTypeDef",
-    {
-        "SharedDirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartSchemaExtensionRequestRequestTypeDef = TypedDict(
     "StartSchemaExtensionRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "CreateSnapshotBeforeSchemaExtension": bool,
         "LdifContent": str,
         "Description": str,
     },
 )
 
-StartSchemaExtensionResultTypeDef = TypedDict(
-    "StartSchemaExtensionResultTypeDef",
-    {
-        "SchemaExtensionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnshareTargetTypeDef = TypedDict(
     "UnshareTargetTypeDef",
     {
         "Id": str,
         "Type": Literal["ACCOUNT"],
     },
 )
 
-UnshareDirectoryResultTypeDef = TypedDict(
-    "UnshareDirectoryResultTypeDef",
-    {
-        "SharedDirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateConditionalForwarderRequestRequestTypeDef = TypedDict(
     "UpdateConditionalForwarderRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RemoteDomainName": str,
         "DnsIpAddrs": Sequence[str],
     },
@@ -1545,79 +1249,194 @@
     "UpdateNumberOfDomainControllersRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "DesiredNumber": int,
     },
 )
 
-UpdateSettingsResultTypeDef = TypedDict(
-    "UpdateSettingsResultTypeDef",
-    {
-        "DirectoryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTrustRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrustRequestRequestTypeDef",
     {
         "TrustId": str,
     },
 )
 _OptionalUpdateTrustRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTrustRequestRequestTypeDef",
     {
         "SelectiveAuth": SelectiveAuthType,
     },
     total=False,
 )
 
+
 class UpdateTrustRequestRequestTypeDef(
     _RequiredUpdateTrustRequestRequestTypeDef, _OptionalUpdateTrustRequestRequestTypeDef
 ):
     pass
 
-UpdateTrustResultTypeDef = TypedDict(
-    "UpdateTrustResultTypeDef",
+
+VerifyTrustRequestRequestTypeDef = TypedDict(
+    "VerifyTrustRequestRequestTypeDef",
     {
-        "RequestId": str,
         "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VerifyTrustRequestRequestTypeDef = TypedDict(
-    "VerifyTrustRequestRequestTypeDef",
+ConnectDirectoryResultTypeDef = TypedDict(
+    "ConnectDirectoryResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAliasResultTypeDef = TypedDict(
+    "CreateAliasResultTypeDef",
+    {
+        "DirectoryId": str,
+        "Alias": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDirectoryResultTypeDef = TypedDict(
+    "CreateDirectoryResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMicrosoftADResultTypeDef = TypedDict(
+    "CreateMicrosoftADResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotResultTypeDef = TypedDict(
+    "CreateSnapshotResultTypeDef",
+    {
+        "SnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrustResultTypeDef = TypedDict(
+    "CreateTrustResultTypeDef",
     {
         "TrustId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDirectoryResultTypeDef = TypedDict(
+    "DeleteDirectoryResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotResultTypeDef = TypedDict(
+    "DeleteSnapshotResultTypeDef",
+    {
+        "SnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTrustResultTypeDef = TypedDict(
+    "DeleteTrustResultTypeDef",
+    {
+        "TrustId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCertificateResultTypeDef = TypedDict(
+    "RegisterCertificateResultTypeDef",
+    {
+        "CertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RejectSharedDirectoryResultTypeDef = TypedDict(
+    "RejectSharedDirectoryResultTypeDef",
+    {
+        "SharedDirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ShareDirectoryResultTypeDef = TypedDict(
+    "ShareDirectoryResultTypeDef",
+    {
+        "SharedDirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSchemaExtensionResultTypeDef = TypedDict(
+    "StartSchemaExtensionResultTypeDef",
+    {
+        "SchemaExtensionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnshareDirectoryResultTypeDef = TypedDict(
+    "UnshareDirectoryResultTypeDef",
+    {
+        "SharedDirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSettingsResultTypeDef = TypedDict(
+    "UpdateSettingsResultTypeDef",
+    {
+        "DirectoryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrustResultTypeDef = TypedDict(
+    "UpdateTrustResultTypeDef",
+    {
+        "RequestId": str,
+        "TrustId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VerifyTrustResultTypeDef = TypedDict(
     "VerifyTrustResultTypeDef",
     {
         "TrustId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptSharedDirectoryResultTypeDef = TypedDict(
     "AcceptSharedDirectoryResultTypeDef",
     {
         "SharedDirectory": SharedDirectoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSharedDirectoriesResultTypeDef = TypedDict(
     "DescribeSharedDirectoriesResultTypeDef",
     {
         "SharedDirectories": List[SharedDirectoryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAddIpRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredAddIpRoutesRequestRequestTypeDef",
     {
         "DirectoryId": str,
@@ -1628,44 +1447,30 @@
     "_OptionalAddIpRoutesRequestRequestTypeDef",
     {
         "UpdateSecurityGroupForDirectoryControllers": bool,
     },
     total=False,
 )
 
+
 class AddIpRoutesRequestRequestTypeDef(
     _RequiredAddIpRoutesRequestRequestTypeDef, _OptionalAddIpRoutesRequestRequestTypeDef
 ):
     pass
 
+
 AddRegionRequestRequestTypeDef = TypedDict(
     "AddRegionRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RegionName": str,
         "VPCSettings": DirectoryVpcSettingsTypeDef,
     },
 )
 
-RegionDescriptionTypeDef = TypedDict(
-    "RegionDescriptionTypeDef",
-    {
-        "DirectoryId": str,
-        "RegionName": str,
-        "RegionType": RegionTypeType,
-        "Status": DirectoryStageType,
-        "VpcSettings": DirectoryVpcSettingsTypeDef,
-        "DesiredNumberOfDomainControllers": int,
-        "LaunchTime": datetime,
-        "StatusLastUpdatedDateTime": datetime,
-        "LastUpdatedDateTime": datetime,
-    },
-    total=False,
-)
-
 AddTagsToResourceRequestRequestTypeDef = TypedDict(
     "AddTagsToResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1685,19 +1490,21 @@
         "Description": str,
         "VpcSettings": DirectoryVpcSettingsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDirectoryRequestRequestTypeDef(
     _RequiredCreateDirectoryRequestRequestTypeDef, _OptionalCreateDirectoryRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateMicrosoftADRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMicrosoftADRequestRequestTypeDef",
     {
         "Name": str,
         "Password": str,
         "VpcSettings": DirectoryVpcSettingsTypeDef,
     },
@@ -1709,25 +1516,27 @@
         "Description": str,
         "Edition": DirectoryEditionType,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMicrosoftADRequestRequestTypeDef(
     _RequiredCreateMicrosoftADRequestRequestTypeDef, _OptionalCreateMicrosoftADRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComputerTypeDef = TypedDict(
     "ComputerTypeDef",
     {
         "ComputerId": str,
@@ -1750,25 +1559,27 @@
     {
         "OrganizationalUnitDistinguishedName": str,
         "ComputerAttributes": Sequence[AttributeTypeDef],
     },
     total=False,
 )
 
+
 class CreateComputerRequestRequestTypeDef(
     _RequiredCreateComputerRequestRequestTypeDef, _OptionalCreateComputerRequestRequestTypeDef
 ):
     pass
 
+
 ListCertificatesResultTypeDef = TypedDict(
     "ListCertificatesResultTypeDef",
     {
         "NextToken": str,
         "CertificatesInfo": List[CertificateInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CertificateTypeDef = TypedDict(
     "CertificateTypeDef",
     {
         "CertificateId": str,
@@ -1795,34 +1606,36 @@
     {
         "Type": CertificateTypeType,
         "ClientCertAuthSettings": ClientCertAuthSettingsTypeDef,
     },
     total=False,
 )
 
+
 class RegisterCertificateRequestRequestTypeDef(
     _RequiredRegisterCertificateRequestRequestTypeDef,
     _OptionalRegisterCertificateRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeClientAuthenticationSettingsResultTypeDef = TypedDict(
     "DescribeClientAuthenticationSettingsResultTypeDef",
     {
         "ClientAuthenticationSettingsInfo": List[ClientAuthenticationSettingInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConditionalForwardersResultTypeDef = TypedDict(
     "DescribeConditionalForwardersResultTypeDef",
     {
         "ConditionalForwarders": List[ConditionalForwarderTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredConnectDirectoryRequestRequestTypeDef = TypedDict(
     "_RequiredConnectDirectoryRequestRequestTypeDef",
     {
         "Name": str,
@@ -1837,142 +1650,429 @@
         "ShortName": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ConnectDirectoryRequestRequestTypeDef(
     _RequiredConnectDirectoryRequestRequestTypeDef, _OptionalConnectDirectoryRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef",
+    {
+        "Type": ClientAuthenticationTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef(
+    _RequiredDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    _OptionalDescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+):
+    pass
+
+
+DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef = TypedDict(
+    "DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef",
+    {
+        "DirectoryIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef",
+    {
+        "DomainControllerIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef(
+    _RequiredDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+    _OptionalDescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef",
+    {
+        "Type": Literal["Client"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef(
+    _RequiredDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+    _OptionalDescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef",
+    {
+        "RegionName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeRegionsRequestDescribeRegionsPaginateTypeDef(
+    _RequiredDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+    _OptionalDescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
+    {
+        "OwnerDirectoryId": str,
+    },
+)
+_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef",
+    {
+        "SharedDirectoryIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef(
+    _RequiredDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+    _OptionalDescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+):
+    pass
+
+
+DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = TypedDict(
+    "DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "SnapshotIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeTrustsRequestDescribeTrustsPaginateTypeDef = TypedDict(
+    "DescribeTrustsRequestDescribeTrustsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "TrustIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
+    "_RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "UpdateType": Literal["OS"],
+    },
+)
+_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef = TypedDict(
+    "_OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef",
+    {
+        "RegionName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef(
+    _RequiredDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+    _OptionalDescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "_RequiredListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "_OptionalListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCertificatesRequestListCertificatesPaginateTypeDef(
+    _RequiredListCertificatesRequestListCertificatesPaginateTypeDef,
+    _OptionalListCertificatesRequestListCertificatesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListIpRoutesRequestListIpRoutesPaginateTypeDef(
+    _RequiredListIpRoutesRequestListIpRoutesPaginateTypeDef,
+    _OptionalListIpRoutesRequestListIpRoutesPaginateTypeDef,
+):
+    pass
+
+
+ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef = TypedDict(
+    "ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
+    "_RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
+    {
+        "DirectoryId": str,
+    },
+)
+_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = TypedDict(
+    "_OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef(
+    _RequiredListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+    _OptionalListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 DescribeDomainControllersResultTypeDef = TypedDict(
     "DescribeDomainControllersResultTypeDef",
     {
         "DomainControllers": List[DomainControllerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEventTopicsResultTypeDef = TypedDict(
     "DescribeEventTopicsResultTypeDef",
     {
         "EventTopics": List[EventTopicTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLDAPSSettingsResultTypeDef = TypedDict(
     "DescribeLDAPSSettingsResultTypeDef",
     {
         "LDAPSSettingsInfo": List[LDAPSSettingInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSettingsResultTypeDef = TypedDict(
     "DescribeSettingsResultTypeDef",
     {
         "DirectoryId": str,
         "SettingEntries": List[SettingEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSnapshotsResultTypeDef = TypedDict(
     "DescribeSnapshotsResultTypeDef",
     {
         "Snapshots": List[SnapshotTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTrustsResultTypeDef = TypedDict(
     "DescribeTrustsResultTypeDef",
     {
         "Trusts": List[TrustTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EnableRadiusRequestRequestTypeDef = TypedDict(
-    "EnableRadiusRequestRequestTypeDef",
-    {
-        "DirectoryId": str,
-        "RadiusSettings": RadiusSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OwnerDirectoryDescriptionTypeDef = TypedDict(
     "OwnerDirectoryDescriptionTypeDef",
     {
         "DirectoryId": str,
         "AccountId": str,
         "DnsIpAddrs": List[str],
         "VpcSettings": DirectoryVpcSettingsDescriptionTypeDef,
-        "RadiusSettings": RadiusSettingsTypeDef,
+        "RadiusSettings": RadiusSettingsOutputTypeDef,
         "RadiusStatus": RadiusStatusType,
     },
     total=False,
 )
 
-UpdateRadiusRequestRequestTypeDef = TypedDict(
-    "UpdateRadiusRequestRequestTypeDef",
+GetDirectoryLimitsResultTypeDef = TypedDict(
+    "GetDirectoryLimitsResultTypeDef",
+    {
+        "DirectoryLimits": DirectoryLimitsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DirectoryVpcSettingsUnionTypeDef = Union[
+    DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef
+]
+RegionDescriptionTypeDef = TypedDict(
+    "RegionDescriptionTypeDef",
+    {
+        "DirectoryId": str,
+        "RegionName": str,
+        "RegionType": RegionTypeType,
+        "Status": DirectoryStageType,
+        "VpcSettings": DirectoryVpcSettingsOutputTypeDef,
+        "DesiredNumberOfDomainControllers": int,
+        "LaunchTime": datetime,
+        "StatusLastUpdatedDateTime": datetime,
+        "LastUpdatedDateTime": datetime,
+    },
+    total=False,
+)
+
+EnableRadiusRequestRequestTypeDef = TypedDict(
+    "EnableRadiusRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
 
-GetDirectoryLimitsResultTypeDef = TypedDict(
-    "GetDirectoryLimitsResultTypeDef",
+RadiusSettingsUnionTypeDef = Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
+UpdateRadiusRequestRequestTypeDef = TypedDict(
+    "UpdateRadiusRequestRequestTypeDef",
     {
-        "DirectoryLimits": DirectoryLimitsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DirectoryId": str,
+        "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
 
 GetSnapshotLimitsResultTypeDef = TypedDict(
     "GetSnapshotLimitsResultTypeDef",
     {
         "SnapshotLimits": SnapshotLimitsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIpRoutesResultTypeDef = TypedDict(
     "ListIpRoutesResultTypeDef",
     {
         "IpRoutesInfo": List[IpRouteInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogSubscriptionsResultTypeDef = TypedDict(
     "ListLogSubscriptionsResultTypeDef",
     {
         "LogSubscriptions": List[LogSubscriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemaExtensionsResultTypeDef = TypedDict(
     "ListSchemaExtensionsResultTypeDef",
     {
         "SchemaExtensionsInfo": List[SchemaExtensionInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateDirectorySetupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDirectorySetupRequestRequestTypeDef",
     {
         "DirectoryId": str,
@@ -1984,20 +2084,22 @@
     {
         "OSUpdateSettings": OSUpdateSettingsTypeDef,
         "CreateSnapshotBeforeUpdate": bool,
     },
     total=False,
 )
 
+
 class UpdateDirectorySetupRequestRequestTypeDef(
     _RequiredUpdateDirectorySetupRequestRequestTypeDef,
     _OptionalUpdateDirectorySetupRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateValueTypeDef = TypedDict(
     "UpdateValueTypeDef",
     {
         "OSUpdateSettings": OSUpdateSettingsTypeDef,
     },
     total=False,
 )
@@ -2022,49 +2124,42 @@
     "_OptionalShareDirectoryRequestRequestTypeDef",
     {
         "ShareNotes": str,
     },
     total=False,
 )
 
+
 class ShareDirectoryRequestRequestTypeDef(
     _RequiredShareDirectoryRequestRequestTypeDef, _OptionalShareDirectoryRequestRequestTypeDef
 ):
     pass
 
+
 UnshareDirectoryRequestRequestTypeDef = TypedDict(
     "UnshareDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UnshareTarget": UnshareTargetTypeDef,
     },
 )
 
-DescribeRegionsResultTypeDef = TypedDict(
-    "DescribeRegionsResultTypeDef",
-    {
-        "RegionsDescription": List[RegionDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateComputerResultTypeDef = TypedDict(
     "CreateComputerResultTypeDef",
     {
         "Computer": ComputerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificateResultTypeDef = TypedDict(
     "DescribeCertificateResultTypeDef",
     {
         "Certificate": CertificateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DirectoryDescriptionTypeDef = TypedDict(
     "DirectoryDescriptionTypeDef",
     {
         "DirectoryId": str,
@@ -2081,26 +2176,35 @@
         "ShareMethod": ShareMethodType,
         "ShareNotes": str,
         "LaunchTime": datetime,
         "StageLastUpdatedDateTime": datetime,
         "Type": DirectoryTypeType,
         "VpcSettings": DirectoryVpcSettingsDescriptionTypeDef,
         "ConnectSettings": DirectoryConnectSettingsDescriptionTypeDef,
-        "RadiusSettings": RadiusSettingsTypeDef,
+        "RadiusSettings": RadiusSettingsOutputTypeDef,
         "RadiusStatus": RadiusStatusType,
         "StageReason": str,
         "SsoEnabled": bool,
         "DesiredNumberOfDomainControllers": int,
         "OwnerDirectoryDescription": OwnerDirectoryDescriptionTypeDef,
         "RegionsInfo": RegionsInfoTypeDef,
         "OsVersion": OSVersionType,
     },
     total=False,
 )
 
+DescribeRegionsResultTypeDef = TypedDict(
+    "DescribeRegionsResultTypeDef",
+    {
+        "RegionsDescription": List[RegionDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateInfoEntryTypeDef = TypedDict(
     "UpdateInfoEntryTypeDef",
     {
         "Region": str,
         "Status": UpdateStatusType,
         "StatusReason": str,
         "InitiatedBy": str,
@@ -2113,19 +2217,19 @@
 )
 
 DescribeDirectoriesResultTypeDef = TypedDict(
     "DescribeDirectoriesResultTypeDef",
     {
         "DirectoryDescriptions": List[DirectoryDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUpdateDirectoryResultTypeDef = TypedDict(
     "DescribeUpdateDirectoryResultTypeDef",
     {
         "UpdateActivities": List[UpdateInfoEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/PKG-INFO` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ds
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DirectoryService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DirectoryService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ds type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ds type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ds"></a>
 
 # types-aiobotocore-ds
 
 [![PyPI - types-aiobotocore-ds](https://img.shields.io/pypi/v/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ds.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ds)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ds?color=blue)](https://pypistats.org/packages/types-aiobotocore-ds)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ds)](https://pepy.tech/project/types-aiobotocore-ds)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DirectoryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
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
 [types-aiobotocore-ds docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/).
 
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
@@ -398,184 +397,188 @@
 )
 
 
 def check_value(value: CertificateStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ds.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ds.type_defs import (
     AcceptSharedDirectoryRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SharedDirectoryTypeDef,
     IpRouteTypeDef,
     DirectoryVpcSettingsTypeDef,
     TagTypeDef,
     AttributeTypeDef,
     CancelSchemaExtensionRequestRequestTypeDef,
     CertificateInfoTypeDef,
     ClientCertAuthSettingsTypeDef,
     ClientAuthenticationSettingInfoTypeDef,
     ConditionalForwarderTypeDef,
     DirectoryConnectSettingsTypeDef,
-    ConnectDirectoryResultTypeDef,
     CreateAliasRequestRequestTypeDef,
-    CreateAliasResultTypeDef,
     CreateConditionalForwarderRequestRequestTypeDef,
-    CreateDirectoryResultTypeDef,
     CreateLogSubscriptionRequestRequestTypeDef,
-    CreateMicrosoftADResultTypeDef,
     CreateSnapshotRequestRequestTypeDef,
-    CreateSnapshotResultTypeDef,
     CreateTrustRequestRequestTypeDef,
-    CreateTrustResultTypeDef,
     DeleteConditionalForwarderRequestRequestTypeDef,
     DeleteDirectoryRequestRequestTypeDef,
-    DeleteDirectoryResultTypeDef,
     DeleteLogSubscriptionRequestRequestTypeDef,
     DeleteSnapshotRequestRequestTypeDef,
-    DeleteSnapshotResultTypeDef,
     DeleteTrustRequestRequestTypeDef,
-    DeleteTrustResultTypeDef,
     DeregisterCertificateRequestRequestTypeDef,
     DeregisterEventTopicRequestRequestTypeDef,
     DescribeCertificateRequestRequestTypeDef,
-    DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClientAuthenticationSettingsRequestRequestTypeDef,
     DescribeConditionalForwardersRequestRequestTypeDef,
-    DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef,
     DescribeDirectoriesRequestRequestTypeDef,
-    DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
     DescribeDomainControllersRequestRequestTypeDef,
     DomainControllerTypeDef,
     DescribeEventTopicsRequestRequestTypeDef,
     EventTopicTypeDef,
-    DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
     DescribeLDAPSSettingsRequestRequestTypeDef,
     LDAPSSettingInfoTypeDef,
-    DescribeRegionsRequestDescribeRegionsPaginateTypeDef,
     DescribeRegionsRequestRequestTypeDef,
     DescribeSettingsRequestRequestTypeDef,
     SettingEntryTypeDef,
-    DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
     DescribeSharedDirectoriesRequestRequestTypeDef,
-    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
     DescribeSnapshotsRequestRequestTypeDef,
     SnapshotTypeDef,
-    DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
     DescribeTrustsRequestRequestTypeDef,
     TrustTypeDef,
-    DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
     DescribeUpdateDirectoryRequestRequestTypeDef,
     DirectoryConnectSettingsDescriptionTypeDef,
     DirectoryVpcSettingsDescriptionTypeDef,
-    RadiusSettingsTypeDef,
+    RadiusSettingsOutputTypeDef,
     RegionsInfoTypeDef,
     DirectoryLimitsTypeDef,
+    DirectoryVpcSettingsOutputTypeDef,
     DisableClientAuthenticationRequestRequestTypeDef,
     DisableLDAPSRequestRequestTypeDef,
     DisableRadiusRequestRequestTypeDef,
     DisableSsoRequestRequestTypeDef,
     EnableClientAuthenticationRequestRequestTypeDef,
     EnableLDAPSRequestRequestTypeDef,
+    RadiusSettingsTypeDef,
     EnableSsoRequestRequestTypeDef,
     GetSnapshotLimitsRequestRequestTypeDef,
     SnapshotLimitsTypeDef,
     IpRouteInfoTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
-    ListIpRoutesRequestListIpRoutesPaginateTypeDef,
     ListIpRoutesRequestRequestTypeDef,
-    ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef,
     ListLogSubscriptionsRequestRequestTypeDef,
     LogSubscriptionTypeDef,
-    ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
     ListSchemaExtensionsRequestRequestTypeDef,
     SchemaExtensionInfoTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     OSUpdateSettingsTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterCertificateResultTypeDef,
     RegisterEventTopicRequestRequestTypeDef,
     RejectSharedDirectoryRequestRequestTypeDef,
-    RejectSharedDirectoryResultTypeDef,
     RemoveIpRoutesRequestRequestTypeDef,
     RemoveRegionRequestRequestTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetUserPasswordRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     SettingTypeDef,
     ShareTargetTypeDef,
-    ShareDirectoryResultTypeDef,
     StartSchemaExtensionRequestRequestTypeDef,
-    StartSchemaExtensionResultTypeDef,
     UnshareTargetTypeDef,
-    UnshareDirectoryResultTypeDef,
     UpdateConditionalForwarderRequestRequestTypeDef,
     UpdateNumberOfDomainControllersRequestRequestTypeDef,
-    UpdateSettingsResultTypeDef,
     UpdateTrustRequestRequestTypeDef,
-    UpdateTrustResultTypeDef,
     VerifyTrustRequestRequestTypeDef,
+    ConnectDirectoryResultTypeDef,
+    CreateAliasResultTypeDef,
+    CreateDirectoryResultTypeDef,
+    CreateMicrosoftADResultTypeDef,
+    CreateSnapshotResultTypeDef,
+    CreateTrustResultTypeDef,
+    DeleteDirectoryResultTypeDef,
+    DeleteSnapshotResultTypeDef,
+    DeleteTrustResultTypeDef,
+    RegisterCertificateResultTypeDef,
+    RejectSharedDirectoryResultTypeDef,
+    ShareDirectoryResultTypeDef,
+    StartSchemaExtensionResultTypeDef,
+    UnshareDirectoryResultTypeDef,
+    UpdateSettingsResultTypeDef,
+    UpdateTrustResultTypeDef,
     VerifyTrustResultTypeDef,
     AcceptSharedDirectoryResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     AddIpRoutesRequestRequestTypeDef,
     AddRegionRequestRequestTypeDef,
-    RegionDescriptionTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
     CreateDirectoryRequestRequestTypeDef,
     CreateMicrosoftADRequestRequestTypeDef,
     ListTagsForResourceResultTypeDef,
     ComputerTypeDef,
     CreateComputerRequestRequestTypeDef,
     ListCertificatesResultTypeDef,
     CertificateTypeDef,
     RegisterCertificateRequestRequestTypeDef,
     DescribeClientAuthenticationSettingsResultTypeDef,
     DescribeConditionalForwardersResultTypeDef,
     ConnectDirectoryRequestRequestTypeDef,
+    DescribeClientAuthenticationSettingsRequestDescribeClientAuthenticationSettingsPaginateTypeDef,
+    DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef,
+    DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef,
+    DescribeLDAPSSettingsRequestDescribeLDAPSSettingsPaginateTypeDef,
+    DescribeRegionsRequestDescribeRegionsPaginateTypeDef,
+    DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef,
+    DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef,
+    DescribeTrustsRequestDescribeTrustsPaginateTypeDef,
+    DescribeUpdateDirectoryRequestDescribeUpdateDirectoryPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListIpRoutesRequestListIpRoutesPaginateTypeDef,
+    ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef,
+    ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeDomainControllersResultTypeDef,
     DescribeEventTopicsResultTypeDef,
     DescribeLDAPSSettingsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
-    EnableRadiusRequestRequestTypeDef,
     OwnerDirectoryDescriptionTypeDef,
-    UpdateRadiusRequestRequestTypeDef,
     GetDirectoryLimitsResultTypeDef,
+    DirectoryVpcSettingsUnionTypeDef,
+    RegionDescriptionTypeDef,
+    EnableRadiusRequestRequestTypeDef,
+    RadiusSettingsUnionTypeDef,
+    UpdateRadiusRequestRequestTypeDef,
     GetSnapshotLimitsResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     UpdateDirectorySetupRequestRequestTypeDef,
     UpdateValueTypeDef,
     UpdateSettingsRequestRequestTypeDef,
     ShareDirectoryRequestRequestTypeDef,
     UnshareDirectoryRequestRequestTypeDef,
-    DescribeRegionsResultTypeDef,
     CreateComputerResultTypeDef,
     DescribeCertificateResultTypeDef,
     DirectoryDescriptionTypeDef,
+    DescribeRegionsResultTypeDef,
     UpdateInfoEntryTypeDef,
     DescribeDirectoriesResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
 )
 
 
-def get_structure() -> AcceptSharedDirectoryRequestRequestTypeDef:
+def get_value() -> AcceptSharedDirectoryRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ds-2.5.2/types_aiobotocore_ds.egg-info/SOURCES.txt` & `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*


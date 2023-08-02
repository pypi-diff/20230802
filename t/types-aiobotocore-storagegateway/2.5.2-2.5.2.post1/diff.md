# Comparing `tmp/types-aiobotocore-storagegateway-2.5.2.tar.gz` & `tmp/types-aiobotocore-storagegateway-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-storagegateway-2.5.2.tar", last modified: Sat Jul  8 01:44:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-storagegateway-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:05 2023, max compression
```

## Comparing `types-aiobotocore-storagegateway-2.5.2.tar` & `types-aiobotocore-storagegateway-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:23.858968 types-aiobotocore-storagegateway-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:43.000000 types-aiobotocore-storagegateway-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24419 2023-07-08 01:44:23.850968 types-aiobotocore-storagegateway-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-07-08 01:41:43.000000 types-aiobotocore-storagegateway-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:23.858968 types-aiobotocore-storagegateway-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 01:41:43.000000 types-aiobotocore-storagegateway-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:23.850968 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-07-08 01:41:43.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-08 01:41:43.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:41:43.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71745 2023-07-08 01:41:44.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    71635 2023-07-08 01:41:44.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-07-08 01:41:44.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-07-08 01:41:44.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13783 2023-07-08 01:41:44.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-07-08 01:41:44.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:43.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    76948 2023-07-08 01:41:48.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    76871 2023-07-08 01:41:47.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:43.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:23.850968 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24419 2023-07-08 01:44:23.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:44:23.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:23.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:23.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:23.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:44:23.000000 types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.621444 types-aiobotocore-storagegateway-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-08-02 14:53:05.621444 types-aiobotocore-storagegateway-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23056 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:05.621444 types-aiobotocore-storagegateway-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.621444 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71775 2023-08-02 14:50:22.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71665 2023-08-02 14:50:22.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-08-02 14:50:22.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-08-02 14:50:22.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-08-02 14:50:22.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13748 2023-08-02 14:50:22.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    78425 2023-08-02 14:50:23.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78346 2023-08-02 14:50:23.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:21.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.621444 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-08-02 14:53:05.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:53:05.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:05.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:05.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:05.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:53:05.000000 types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-storagegateway-2.5.2/LICENSE` & `types-aiobotocore-storagegateway-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.5.2/PKG-INFO` & `types-aiobotocore-storagegateway-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-storagegateway
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.StorageGateway 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.StorageGateway 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore storagegateway type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore storagegateway type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-storagegateway"></a>
 
 # types-aiobotocore-storagegateway
 
 [![PyPI - types-aiobotocore-storagegateway](https://img.shields.io/pypi/v/types-aiobotocore-storagegateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-storagegateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-storagegateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-storagegateway?color=blue)](https://pypistats.org/packages/types-aiobotocore-storagegateway)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-storagegateway)](https://pepy.tech/project/types-aiobotocore-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.StorageGateway 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [types-aiobotocore-storagegateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/).
 
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
@@ -358,250 +357,256 @@
 )
 
 
 def check_value(value: ActiveDirectoryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_storagegateway.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_storagegateway.type_defs import (
     TagTypeDef,
-    ActivateGatewayOutputTypeDef,
+    ResponseMetadataTypeDef,
     AddCacheInputRequestTypeDef,
-    AddCacheOutputTypeDef,
-    AddTagsToResourceOutputTypeDef,
     AddUploadBufferInputRequestTypeDef,
-    AddUploadBufferOutputTypeDef,
     AddWorkingStorageInputRequestTypeDef,
-    AddWorkingStorageOutputTypeDef,
     AssignTapePoolInputRequestTypeDef,
-    AssignTapePoolOutputTypeDef,
     CacheAttributesTypeDef,
     EndpointNetworkConfigurationTypeDef,
-    AssociateFileSystemOutputTypeDef,
     AttachVolumeInputRequestTypeDef,
-    AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     VolumeiSCSIAttributesTypeDef,
     CancelArchivalInputRequestTypeDef,
-    CancelArchivalOutputTypeDef,
     CancelRetrievalInputRequestTypeDef,
-    CancelRetrievalOutputTypeDef,
     ChapInfoTypeDef,
-    CreateCachediSCSIVolumeOutputTypeDef,
     NFSFileShareDefaultsTypeDef,
-    CreateNFSFileShareOutputTypeDef,
-    CreateSMBFileShareOutputTypeDef,
-    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
-    CreateSnapshotOutputTypeDef,
-    CreateStorediSCSIVolumeOutputTypeDef,
-    CreateTapePoolOutputTypeDef,
-    CreateTapeWithBarcodeOutputTypeDef,
-    CreateTapesOutputTypeDef,
     DeleteAutomaticTapeCreationPolicyInputRequestTypeDef,
-    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
     DeleteBandwidthRateLimitInputRequestTypeDef,
-    DeleteBandwidthRateLimitOutputTypeDef,
     DeleteChapCredentialsInputRequestTypeDef,
-    DeleteChapCredentialsOutputTypeDef,
     DeleteFileShareInputRequestTypeDef,
-    DeleteFileShareOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
-    DeleteGatewayOutputTypeDef,
     DeleteSnapshotScheduleInputRequestTypeDef,
-    DeleteSnapshotScheduleOutputTypeDef,
     DeleteTapeArchiveInputRequestTypeDef,
-    DeleteTapeArchiveOutputTypeDef,
     DeleteTapeInputRequestTypeDef,
-    DeleteTapeOutputTypeDef,
     DeleteTapePoolInputRequestTypeDef,
-    DeleteTapePoolOutputTypeDef,
     DeleteVolumeInputRequestTypeDef,
-    DeleteVolumeOutputTypeDef,
     DescribeAvailabilityMonitorTestInputRequestTypeDef,
-    DescribeAvailabilityMonitorTestOutputTypeDef,
     DescribeBandwidthRateLimitInputRequestTypeDef,
-    DescribeBandwidthRateLimitOutputTypeDef,
     DescribeBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCacheInputRequestTypeDef,
-    DescribeCacheOutputTypeDef,
     DescribeCachediSCSIVolumesInputRequestTypeDef,
     DescribeChapCredentialsInputRequestTypeDef,
     DescribeFileSystemAssociationsInputRequestTypeDef,
     DescribeGatewayInformationInputRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeMaintenanceStartTimeInputRequestTypeDef,
-    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeNFSFileSharesInputRequestTypeDef,
     DescribeSMBFileSharesInputRequestTypeDef,
     DescribeSMBSettingsInputRequestTypeDef,
-    SMBLocalGroupsTypeDef,
+    SMBLocalGroupsOutputTypeDef,
     DescribeSnapshotScheduleInputRequestTypeDef,
     DescribeStorediSCSIVolumesInputRequestTypeDef,
-    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeTapeArchivesInputRequestTypeDef,
     TapeArchiveTypeDef,
-    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
     DescribeTapeRecoveryPointsInputRequestTypeDef,
     TapeRecoveryPointInfoTypeDef,
-    DescribeTapesInputDescribeTapesPaginateTypeDef,
     DescribeTapesInputRequestTypeDef,
     TapeTypeDef,
     DescribeUploadBufferInputRequestTypeDef,
-    DescribeUploadBufferOutputTypeDef,
-    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
     DescribeVTLDevicesInputRequestTypeDef,
     DescribeWorkingStorageInputRequestTypeDef,
-    DescribeWorkingStorageOutputTypeDef,
     DetachVolumeInputRequestTypeDef,
-    DetachVolumeOutputTypeDef,
     DeviceiSCSIAttributesTypeDef,
     DisableGatewayInputRequestTypeDef,
-    DisableGatewayOutputTypeDef,
     DisassociateFileSystemInputRequestTypeDef,
-    DisassociateFileSystemOutputTypeDef,
     DiskTypeDef,
+    EndpointNetworkConfigurationOutputTypeDef,
     FileShareInfoTypeDef,
     FileSystemAssociationStatusDetailTypeDef,
     FileSystemAssociationSummaryTypeDef,
     GatewayInfoTypeDef,
     JoinDomainInputRequestTypeDef,
-    JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesInputRequestTypeDef,
-    ListFileSharesInputListFileSharesPaginateTypeDef,
     ListFileSharesInputRequestTypeDef,
-    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
     ListFileSystemAssociationsInputRequestTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
     ListGatewaysInputRequestTypeDef,
     ListLocalDisksInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTapePoolsInputListTapePoolsPaginateTypeDef,
     ListTapePoolsInputRequestTypeDef,
     PoolInfoTypeDef,
-    ListTapesInputListTapesPaginateTypeDef,
     ListTapesInputRequestTypeDef,
     TapeInfoTypeDef,
     ListVolumeInitiatorsInputRequestTypeDef,
-    ListVolumeInitiatorsOutputTypeDef,
     ListVolumeRecoveryPointsInputRequestTypeDef,
     VolumeRecoveryPointInfoTypeDef,
-    ListVolumesInputListVolumesPaginateTypeDef,
     ListVolumesInputRequestTypeDef,
     VolumeInfoTypeDef,
     NotifyWhenUploadedInputRequestTypeDef,
-    NotifyWhenUploadedOutputTypeDef,
-    PaginatorConfigTypeDef,
     RefreshCacheInputRequestTypeDef,
-    RefreshCacheOutputTypeDef,
     RemoveTagsFromResourceInputRequestTypeDef,
-    RemoveTagsFromResourceOutputTypeDef,
     ResetCacheInputRequestTypeDef,
-    ResetCacheOutputTypeDef,
-    ResponseMetadataTypeDef,
     RetrieveTapeArchiveInputRequestTypeDef,
-    RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointInputRequestTypeDef,
-    RetrieveTapeRecoveryPointOutputTypeDef,
+    SMBLocalGroupsTypeDef,
     SetLocalConsolePasswordInputRequestTypeDef,
-    SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordInputRequestTypeDef,
-    SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayInputRequestTypeDef,
-    ShutdownGatewayOutputTypeDef,
     StartAvailabilityMonitorTestInputRequestTypeDef,
-    StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayInputRequestTypeDef,
-    StartGatewayOutputTypeDef,
-    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitInputRequestTypeDef,
-    UpdateBandwidthRateLimitOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsInputRequestTypeDef,
-    UpdateChapCredentialsOutputTypeDef,
-    UpdateFileSystemAssociationOutputTypeDef,
     UpdateGatewayInformationInputRequestTypeDef,
-    UpdateGatewayInformationOutputTypeDef,
     UpdateGatewaySoftwareNowInputRequestTypeDef,
-    UpdateGatewaySoftwareNowOutputTypeDef,
     UpdateMaintenanceStartTimeInputRequestTypeDef,
-    UpdateMaintenanceStartTimeOutputTypeDef,
-    UpdateNFSFileShareOutputTypeDef,
-    UpdateSMBFileShareOutputTypeDef,
     UpdateSMBFileShareVisibilityInputRequestTypeDef,
-    UpdateSMBFileShareVisibilityOutputTypeDef,
-    UpdateSMBLocalGroupsOutputTypeDef,
     UpdateSMBSecurityStrategyInputRequestTypeDef,
-    UpdateSMBSecurityStrategyOutputTypeDef,
-    UpdateSnapshotScheduleOutputTypeDef,
     UpdateVTLDeviceTypeInputRequestTypeDef,
-    UpdateVTLDeviceTypeOutputTypeDef,
     ActivateGatewayInputRequestTypeDef,
     AddTagsToResourceInputRequestTypeDef,
     CreateCachediSCSIVolumeInputRequestTypeDef,
     CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef,
     CreateSnapshotInputRequestTypeDef,
     CreateStorediSCSIVolumeInputRequestTypeDef,
     CreateTapePoolInputRequestTypeDef,
     CreateTapeWithBarcodeInputRequestTypeDef,
     CreateTapesInputRequestTypeDef,
+    UpdateSnapshotScheduleInputRequestTypeDef,
+    ActivateGatewayOutputTypeDef,
+    AddCacheOutputTypeDef,
+    AddTagsToResourceOutputTypeDef,
+    AddUploadBufferOutputTypeDef,
+    AddWorkingStorageOutputTypeDef,
+    AssignTapePoolOutputTypeDef,
+    AssociateFileSystemOutputTypeDef,
+    AttachVolumeOutputTypeDef,
+    CancelArchivalOutputTypeDef,
+    CancelRetrievalOutputTypeDef,
+    CreateCachediSCSIVolumeOutputTypeDef,
+    CreateNFSFileShareOutputTypeDef,
+    CreateSMBFileShareOutputTypeDef,
+    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
+    CreateSnapshotOutputTypeDef,
+    CreateStorediSCSIVolumeOutputTypeDef,
+    CreateTapePoolOutputTypeDef,
+    CreateTapeWithBarcodeOutputTypeDef,
+    CreateTapesOutputTypeDef,
+    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
+    DeleteBandwidthRateLimitOutputTypeDef,
+    DeleteChapCredentialsOutputTypeDef,
+    DeleteFileShareOutputTypeDef,
+    DeleteGatewayOutputTypeDef,
+    DeleteSnapshotScheduleOutputTypeDef,
+    DeleteTapeArchiveOutputTypeDef,
+    DeleteTapeOutputTypeDef,
+    DeleteTapePoolOutputTypeDef,
+    DeleteVolumeOutputTypeDef,
+    DescribeAvailabilityMonitorTestOutputTypeDef,
+    DescribeBandwidthRateLimitOutputTypeDef,
+    DescribeCacheOutputTypeDef,
+    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeSnapshotScheduleOutputTypeDef,
+    DescribeUploadBufferOutputTypeDef,
+    DescribeWorkingStorageOutputTypeDef,
+    DetachVolumeOutputTypeDef,
+    DisableGatewayOutputTypeDef,
+    DisassociateFileSystemOutputTypeDef,
+    JoinDomainOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    UpdateSnapshotScheduleInputRequestTypeDef,
+    ListVolumeInitiatorsOutputTypeDef,
+    NotifyWhenUploadedOutputTypeDef,
+    RefreshCacheOutputTypeDef,
+    RemoveTagsFromResourceOutputTypeDef,
+    ResetCacheOutputTypeDef,
+    RetrieveTapeArchiveOutputTypeDef,
+    RetrieveTapeRecoveryPointOutputTypeDef,
+    SetLocalConsolePasswordOutputTypeDef,
+    SetSMBGuestPasswordOutputTypeDef,
+    ShutdownGatewayOutputTypeDef,
+    StartAvailabilityMonitorTestOutputTypeDef,
+    StartGatewayOutputTypeDef,
+    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
+    UpdateBandwidthRateLimitOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleOutputTypeDef,
+    UpdateChapCredentialsOutputTypeDef,
+    UpdateFileSystemAssociationOutputTypeDef,
+    UpdateGatewayInformationOutputTypeDef,
+    UpdateGatewaySoftwareNowOutputTypeDef,
+    UpdateMaintenanceStartTimeOutputTypeDef,
+    UpdateNFSFileShareOutputTypeDef,
+    UpdateSMBFileShareOutputTypeDef,
+    UpdateSMBFileShareVisibilityOutputTypeDef,
+    UpdateSMBLocalGroupsOutputTypeDef,
+    UpdateSMBSecurityStrategyOutputTypeDef,
+    UpdateSnapshotScheduleOutputTypeDef,
+    UpdateVTLDeviceTypeOutputTypeDef,
     CreateSMBFileShareInputRequestTypeDef,
     SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
     DescribeBandwidthRateLimitScheduleOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CachediSCSIVolumeTypeDef,
     StorediSCSIVolumeTypeDef,
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
     NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
     DescribeSMBSettingsOutputTypeDef,
-    UpdateSMBLocalGroupsInputRequestTypeDef,
+    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
+    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+    DescribeTapesInputDescribeTapesPaginateTypeDef,
+    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+    ListFileSharesInputListFileSharesPaginateTypeDef,
+    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListTapePoolsInputListTapePoolsPaginateTypeDef,
+    ListTapesInputListTapesPaginateTypeDef,
+    ListVolumesInputListVolumesPaginateTypeDef,
     DescribeTapeArchivesOutputTypeDef,
     DescribeTapeRecoveryPointsOutputTypeDef,
     DescribeTapesOutputTypeDef,
     VTLDeviceTypeDef,
     ListLocalDisksOutputTypeDef,
+    EndpointNetworkConfigurationUnionTypeDef,
     ListFileSharesOutputTypeDef,
     FileSystemAssociationInfoTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListTapePoolsOutputTypeDef,
     ListTapesOutputTypeDef,
     ListVolumeRecoveryPointsOutputTypeDef,
     ListVolumesOutputTypeDef,
+    SMBLocalGroupsUnionTypeDef,
+    UpdateSMBLocalGroupsInputRequestTypeDef,
     DescribeSMBFileSharesOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCachediSCSIVolumesOutputTypeDef,
     DescribeStorediSCSIVolumesOutputTypeDef,
     DescribeNFSFileSharesOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeFileSystemAssociationsOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-storagegateway-2.5.2/README.md` & `types-aiobotocore-storagegateway-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-storagegateway"></a>
 
 # types-aiobotocore-storagegateway
 
 [![PyPI - types-aiobotocore-storagegateway](https://img.shields.io/pypi/v/types-aiobotocore-storagegateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-storagegateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-storagegateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-storagegateway?color=blue)](https://pypistats.org/packages/types-aiobotocore-storagegateway)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-storagegateway)](https://pepy.tech/project/types-aiobotocore-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.StorageGateway 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [types-aiobotocore-storagegateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/).
 
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
@@ -325,250 +325,256 @@
 )
 
 
 def check_value(value: ActiveDirectoryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_storagegateway.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_storagegateway.type_defs import (
     TagTypeDef,
-    ActivateGatewayOutputTypeDef,
+    ResponseMetadataTypeDef,
     AddCacheInputRequestTypeDef,
-    AddCacheOutputTypeDef,
-    AddTagsToResourceOutputTypeDef,
     AddUploadBufferInputRequestTypeDef,
-    AddUploadBufferOutputTypeDef,
     AddWorkingStorageInputRequestTypeDef,
-    AddWorkingStorageOutputTypeDef,
     AssignTapePoolInputRequestTypeDef,
-    AssignTapePoolOutputTypeDef,
     CacheAttributesTypeDef,
     EndpointNetworkConfigurationTypeDef,
-    AssociateFileSystemOutputTypeDef,
     AttachVolumeInputRequestTypeDef,
-    AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     VolumeiSCSIAttributesTypeDef,
     CancelArchivalInputRequestTypeDef,
-    CancelArchivalOutputTypeDef,
     CancelRetrievalInputRequestTypeDef,
-    CancelRetrievalOutputTypeDef,
     ChapInfoTypeDef,
-    CreateCachediSCSIVolumeOutputTypeDef,
     NFSFileShareDefaultsTypeDef,
-    CreateNFSFileShareOutputTypeDef,
-    CreateSMBFileShareOutputTypeDef,
-    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
-    CreateSnapshotOutputTypeDef,
-    CreateStorediSCSIVolumeOutputTypeDef,
-    CreateTapePoolOutputTypeDef,
-    CreateTapeWithBarcodeOutputTypeDef,
-    CreateTapesOutputTypeDef,
     DeleteAutomaticTapeCreationPolicyInputRequestTypeDef,
-    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
     DeleteBandwidthRateLimitInputRequestTypeDef,
-    DeleteBandwidthRateLimitOutputTypeDef,
     DeleteChapCredentialsInputRequestTypeDef,
-    DeleteChapCredentialsOutputTypeDef,
     DeleteFileShareInputRequestTypeDef,
-    DeleteFileShareOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
-    DeleteGatewayOutputTypeDef,
     DeleteSnapshotScheduleInputRequestTypeDef,
-    DeleteSnapshotScheduleOutputTypeDef,
     DeleteTapeArchiveInputRequestTypeDef,
-    DeleteTapeArchiveOutputTypeDef,
     DeleteTapeInputRequestTypeDef,
-    DeleteTapeOutputTypeDef,
     DeleteTapePoolInputRequestTypeDef,
-    DeleteTapePoolOutputTypeDef,
     DeleteVolumeInputRequestTypeDef,
-    DeleteVolumeOutputTypeDef,
     DescribeAvailabilityMonitorTestInputRequestTypeDef,
-    DescribeAvailabilityMonitorTestOutputTypeDef,
     DescribeBandwidthRateLimitInputRequestTypeDef,
-    DescribeBandwidthRateLimitOutputTypeDef,
     DescribeBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCacheInputRequestTypeDef,
-    DescribeCacheOutputTypeDef,
     DescribeCachediSCSIVolumesInputRequestTypeDef,
     DescribeChapCredentialsInputRequestTypeDef,
     DescribeFileSystemAssociationsInputRequestTypeDef,
     DescribeGatewayInformationInputRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeMaintenanceStartTimeInputRequestTypeDef,
-    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeNFSFileSharesInputRequestTypeDef,
     DescribeSMBFileSharesInputRequestTypeDef,
     DescribeSMBSettingsInputRequestTypeDef,
-    SMBLocalGroupsTypeDef,
+    SMBLocalGroupsOutputTypeDef,
     DescribeSnapshotScheduleInputRequestTypeDef,
     DescribeStorediSCSIVolumesInputRequestTypeDef,
-    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeTapeArchivesInputRequestTypeDef,
     TapeArchiveTypeDef,
-    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
     DescribeTapeRecoveryPointsInputRequestTypeDef,
     TapeRecoveryPointInfoTypeDef,
-    DescribeTapesInputDescribeTapesPaginateTypeDef,
     DescribeTapesInputRequestTypeDef,
     TapeTypeDef,
     DescribeUploadBufferInputRequestTypeDef,
-    DescribeUploadBufferOutputTypeDef,
-    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
     DescribeVTLDevicesInputRequestTypeDef,
     DescribeWorkingStorageInputRequestTypeDef,
-    DescribeWorkingStorageOutputTypeDef,
     DetachVolumeInputRequestTypeDef,
-    DetachVolumeOutputTypeDef,
     DeviceiSCSIAttributesTypeDef,
     DisableGatewayInputRequestTypeDef,
-    DisableGatewayOutputTypeDef,
     DisassociateFileSystemInputRequestTypeDef,
-    DisassociateFileSystemOutputTypeDef,
     DiskTypeDef,
+    EndpointNetworkConfigurationOutputTypeDef,
     FileShareInfoTypeDef,
     FileSystemAssociationStatusDetailTypeDef,
     FileSystemAssociationSummaryTypeDef,
     GatewayInfoTypeDef,
     JoinDomainInputRequestTypeDef,
-    JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesInputRequestTypeDef,
-    ListFileSharesInputListFileSharesPaginateTypeDef,
     ListFileSharesInputRequestTypeDef,
-    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
     ListFileSystemAssociationsInputRequestTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
     ListGatewaysInputRequestTypeDef,
     ListLocalDisksInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTapePoolsInputListTapePoolsPaginateTypeDef,
     ListTapePoolsInputRequestTypeDef,
     PoolInfoTypeDef,
-    ListTapesInputListTapesPaginateTypeDef,
     ListTapesInputRequestTypeDef,
     TapeInfoTypeDef,
     ListVolumeInitiatorsInputRequestTypeDef,
-    ListVolumeInitiatorsOutputTypeDef,
     ListVolumeRecoveryPointsInputRequestTypeDef,
     VolumeRecoveryPointInfoTypeDef,
-    ListVolumesInputListVolumesPaginateTypeDef,
     ListVolumesInputRequestTypeDef,
     VolumeInfoTypeDef,
     NotifyWhenUploadedInputRequestTypeDef,
-    NotifyWhenUploadedOutputTypeDef,
-    PaginatorConfigTypeDef,
     RefreshCacheInputRequestTypeDef,
-    RefreshCacheOutputTypeDef,
     RemoveTagsFromResourceInputRequestTypeDef,
-    RemoveTagsFromResourceOutputTypeDef,
     ResetCacheInputRequestTypeDef,
-    ResetCacheOutputTypeDef,
-    ResponseMetadataTypeDef,
     RetrieveTapeArchiveInputRequestTypeDef,
-    RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointInputRequestTypeDef,
-    RetrieveTapeRecoveryPointOutputTypeDef,
+    SMBLocalGroupsTypeDef,
     SetLocalConsolePasswordInputRequestTypeDef,
-    SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordInputRequestTypeDef,
-    SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayInputRequestTypeDef,
-    ShutdownGatewayOutputTypeDef,
     StartAvailabilityMonitorTestInputRequestTypeDef,
-    StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayInputRequestTypeDef,
-    StartGatewayOutputTypeDef,
-    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitInputRequestTypeDef,
-    UpdateBandwidthRateLimitOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsInputRequestTypeDef,
-    UpdateChapCredentialsOutputTypeDef,
-    UpdateFileSystemAssociationOutputTypeDef,
     UpdateGatewayInformationInputRequestTypeDef,
-    UpdateGatewayInformationOutputTypeDef,
     UpdateGatewaySoftwareNowInputRequestTypeDef,
-    UpdateGatewaySoftwareNowOutputTypeDef,
     UpdateMaintenanceStartTimeInputRequestTypeDef,
-    UpdateMaintenanceStartTimeOutputTypeDef,
-    UpdateNFSFileShareOutputTypeDef,
-    UpdateSMBFileShareOutputTypeDef,
     UpdateSMBFileShareVisibilityInputRequestTypeDef,
-    UpdateSMBFileShareVisibilityOutputTypeDef,
-    UpdateSMBLocalGroupsOutputTypeDef,
     UpdateSMBSecurityStrategyInputRequestTypeDef,
-    UpdateSMBSecurityStrategyOutputTypeDef,
-    UpdateSnapshotScheduleOutputTypeDef,
     UpdateVTLDeviceTypeInputRequestTypeDef,
-    UpdateVTLDeviceTypeOutputTypeDef,
     ActivateGatewayInputRequestTypeDef,
     AddTagsToResourceInputRequestTypeDef,
     CreateCachediSCSIVolumeInputRequestTypeDef,
     CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef,
     CreateSnapshotInputRequestTypeDef,
     CreateStorediSCSIVolumeInputRequestTypeDef,
     CreateTapePoolInputRequestTypeDef,
     CreateTapeWithBarcodeInputRequestTypeDef,
     CreateTapesInputRequestTypeDef,
+    UpdateSnapshotScheduleInputRequestTypeDef,
+    ActivateGatewayOutputTypeDef,
+    AddCacheOutputTypeDef,
+    AddTagsToResourceOutputTypeDef,
+    AddUploadBufferOutputTypeDef,
+    AddWorkingStorageOutputTypeDef,
+    AssignTapePoolOutputTypeDef,
+    AssociateFileSystemOutputTypeDef,
+    AttachVolumeOutputTypeDef,
+    CancelArchivalOutputTypeDef,
+    CancelRetrievalOutputTypeDef,
+    CreateCachediSCSIVolumeOutputTypeDef,
+    CreateNFSFileShareOutputTypeDef,
+    CreateSMBFileShareOutputTypeDef,
+    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
+    CreateSnapshotOutputTypeDef,
+    CreateStorediSCSIVolumeOutputTypeDef,
+    CreateTapePoolOutputTypeDef,
+    CreateTapeWithBarcodeOutputTypeDef,
+    CreateTapesOutputTypeDef,
+    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
+    DeleteBandwidthRateLimitOutputTypeDef,
+    DeleteChapCredentialsOutputTypeDef,
+    DeleteFileShareOutputTypeDef,
+    DeleteGatewayOutputTypeDef,
+    DeleteSnapshotScheduleOutputTypeDef,
+    DeleteTapeArchiveOutputTypeDef,
+    DeleteTapeOutputTypeDef,
+    DeleteTapePoolOutputTypeDef,
+    DeleteVolumeOutputTypeDef,
+    DescribeAvailabilityMonitorTestOutputTypeDef,
+    DescribeBandwidthRateLimitOutputTypeDef,
+    DescribeCacheOutputTypeDef,
+    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeSnapshotScheduleOutputTypeDef,
+    DescribeUploadBufferOutputTypeDef,
+    DescribeWorkingStorageOutputTypeDef,
+    DetachVolumeOutputTypeDef,
+    DisableGatewayOutputTypeDef,
+    DisassociateFileSystemOutputTypeDef,
+    JoinDomainOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    UpdateSnapshotScheduleInputRequestTypeDef,
+    ListVolumeInitiatorsOutputTypeDef,
+    NotifyWhenUploadedOutputTypeDef,
+    RefreshCacheOutputTypeDef,
+    RemoveTagsFromResourceOutputTypeDef,
+    ResetCacheOutputTypeDef,
+    RetrieveTapeArchiveOutputTypeDef,
+    RetrieveTapeRecoveryPointOutputTypeDef,
+    SetLocalConsolePasswordOutputTypeDef,
+    SetSMBGuestPasswordOutputTypeDef,
+    ShutdownGatewayOutputTypeDef,
+    StartAvailabilityMonitorTestOutputTypeDef,
+    StartGatewayOutputTypeDef,
+    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
+    UpdateBandwidthRateLimitOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleOutputTypeDef,
+    UpdateChapCredentialsOutputTypeDef,
+    UpdateFileSystemAssociationOutputTypeDef,
+    UpdateGatewayInformationOutputTypeDef,
+    UpdateGatewaySoftwareNowOutputTypeDef,
+    UpdateMaintenanceStartTimeOutputTypeDef,
+    UpdateNFSFileShareOutputTypeDef,
+    UpdateSMBFileShareOutputTypeDef,
+    UpdateSMBFileShareVisibilityOutputTypeDef,
+    UpdateSMBLocalGroupsOutputTypeDef,
+    UpdateSMBSecurityStrategyOutputTypeDef,
+    UpdateSnapshotScheduleOutputTypeDef,
+    UpdateVTLDeviceTypeOutputTypeDef,
     CreateSMBFileShareInputRequestTypeDef,
     SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
     DescribeBandwidthRateLimitScheduleOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CachediSCSIVolumeTypeDef,
     StorediSCSIVolumeTypeDef,
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
     NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
     DescribeSMBSettingsOutputTypeDef,
-    UpdateSMBLocalGroupsInputRequestTypeDef,
+    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
+    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+    DescribeTapesInputDescribeTapesPaginateTypeDef,
+    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+    ListFileSharesInputListFileSharesPaginateTypeDef,
+    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListTapePoolsInputListTapePoolsPaginateTypeDef,
+    ListTapesInputListTapesPaginateTypeDef,
+    ListVolumesInputListVolumesPaginateTypeDef,
     DescribeTapeArchivesOutputTypeDef,
     DescribeTapeRecoveryPointsOutputTypeDef,
     DescribeTapesOutputTypeDef,
     VTLDeviceTypeDef,
     ListLocalDisksOutputTypeDef,
+    EndpointNetworkConfigurationUnionTypeDef,
     ListFileSharesOutputTypeDef,
     FileSystemAssociationInfoTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListTapePoolsOutputTypeDef,
     ListTapesOutputTypeDef,
     ListVolumeRecoveryPointsOutputTypeDef,
     ListVolumesOutputTypeDef,
+    SMBLocalGroupsUnionTypeDef,
+    UpdateSMBLocalGroupsInputRequestTypeDef,
     DescribeSMBFileSharesOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCachediSCSIVolumesOutputTypeDef,
     DescribeStorediSCSIVolumesOutputTypeDef,
     DescribeNFSFileSharesOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeFileSystemAssociationsOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-storagegateway-2.5.2/setup.py` & `types-aiobotocore-storagegateway-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-storagegateway",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_storagegateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.StorageGateway 2.5.2 service generated with"
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
-    keywords="aiobotocore storagegateway type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore storagegateway type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_storagegateway": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/"
```

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/__init__.py` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/__init__.pyi` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/__main__.py` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.StorageGateway 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.StorageGateway 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway\nOther"
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

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/client.py` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     AddTagsToResourceOutputTypeDef,
     AddUploadBufferOutputTypeDef,
     AddWorkingStorageOutputTypeDef,
     AssignTapePoolOutputTypeDef,
     AssociateFileSystemOutputTypeDef,
     AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
-    BandwidthRateLimitIntervalTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CacheAttributesTypeDef,
     CancelArchivalOutputTypeDef,
     CancelRetrievalOutputTypeDef,
     CreateCachediSCSIVolumeOutputTypeDef,
     CreateNFSFileShareOutputTypeDef,
     CreateSMBFileShareOutputTypeDef,
     CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
@@ -93,15 +93,15 @@
     DescribeTapesOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
-    EndpointNetworkConfigurationTypeDef,
+    EndpointNetworkConfigurationUnionTypeDef,
     JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     ListFileSharesOutputTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListLocalDisksOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
@@ -116,15 +116,15 @@
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayOutputTypeDef,
-    SMBLocalGroupsTypeDef,
+    SMBLocalGroupsUnionTypeDef,
     StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayOutputTypeDef,
     TagTypeDef,
     UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitOutputTypeDef,
     UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsOutputTypeDef,
@@ -257,15 +257,15 @@
         Password: str,
         ClientToken: str,
         GatewayARN: str,
         LocationARN: str,
         Tags: Sequence[TagTypeDef] = ...,
         AuditDestinationARN: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
-        EndpointNetworkConfiguration: EndpointNetworkConfigurationTypeDef = ...
+        EndpointNetworkConfiguration: EndpointNetworkConfigurationUnionTypeDef = ...
     ) -> AssociateFileSystemOutputTypeDef:
         """
         Associate an Amazon FSx file system with the FSx File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.associate_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#associate_file_system)
         """
@@ -1121,15 +1121,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_bandwidth_rate_limit)
         """
 
     async def update_bandwidth_rate_limit_schedule(
         self,
         *,
         GatewayARN: str,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef]
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef]
     ) -> UpdateBandwidthRateLimitScheduleOutputTypeDef:
         """
         Updates the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_bandwidth_rate_limit_schedule)
         """
@@ -1273,15 +1273,15 @@
         browse list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_file_share_visibility)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_smb_file_share_visibility)
         """
 
     async def update_smb_local_groups(
-        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsTypeDef
+        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsUnionTypeDef
     ) -> UpdateSMBLocalGroupsOutputTypeDef:
         """
         Updates the list of Active Directory users and groups that have special
         permissions for SMB file shares on the gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_local_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_smb_local_groups)
```

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/client.pyi` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     AddTagsToResourceOutputTypeDef,
     AddUploadBufferOutputTypeDef,
     AddWorkingStorageOutputTypeDef,
     AssignTapePoolOutputTypeDef,
     AssociateFileSystemOutputTypeDef,
     AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
-    BandwidthRateLimitIntervalTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CacheAttributesTypeDef,
     CancelArchivalOutputTypeDef,
     CancelRetrievalOutputTypeDef,
     CreateCachediSCSIVolumeOutputTypeDef,
     CreateNFSFileShareOutputTypeDef,
     CreateSMBFileShareOutputTypeDef,
     CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
@@ -93,15 +93,15 @@
     DescribeTapesOutputTypeDef,
     DescribeUploadBufferOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeWorkingStorageOutputTypeDef,
     DetachVolumeOutputTypeDef,
     DisableGatewayOutputTypeDef,
     DisassociateFileSystemOutputTypeDef,
-    EndpointNetworkConfigurationTypeDef,
+    EndpointNetworkConfigurationUnionTypeDef,
     JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
     ListFileSharesOutputTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListLocalDisksOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
@@ -116,15 +116,15 @@
     RemoveTagsFromResourceOutputTypeDef,
     ResetCacheOutputTypeDef,
     RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointOutputTypeDef,
     SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayOutputTypeDef,
-    SMBLocalGroupsTypeDef,
+    SMBLocalGroupsUnionTypeDef,
     StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayOutputTypeDef,
     TagTypeDef,
     UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitOutputTypeDef,
     UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsOutputTypeDef,
@@ -246,15 +246,15 @@
         Password: str,
         ClientToken: str,
         GatewayARN: str,
         LocationARN: str,
         Tags: Sequence[TagTypeDef] = ...,
         AuditDestinationARN: str = ...,
         CacheAttributes: CacheAttributesTypeDef = ...,
-        EndpointNetworkConfiguration: EndpointNetworkConfigurationTypeDef = ...
+        EndpointNetworkConfiguration: EndpointNetworkConfigurationUnionTypeDef = ...
     ) -> AssociateFileSystemOutputTypeDef:
         """
         Associate an Amazon FSx file system with the FSx File Gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.associate_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#associate_file_system)
         """
@@ -1036,15 +1036,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_bandwidth_rate_limit)
         """
     async def update_bandwidth_rate_limit_schedule(
         self,
         *,
         GatewayARN: str,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef]
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef]
     ) -> UpdateBandwidthRateLimitScheduleOutputTypeDef:
         """
         Updates the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_bandwidth_rate_limit_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_bandwidth_rate_limit_schedule)
         """
@@ -1179,15 +1179,15 @@
         Controls whether the shares on an S3 File Gateway are visible in a net view or
         browse list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_file_share_visibility)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_smb_file_share_visibility)
         """
     async def update_smb_local_groups(
-        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsTypeDef
+        self, *, GatewayARN: str, SMBLocalGroups: SMBLocalGroupsUnionTypeDef
     ) -> UpdateSMBLocalGroupsOutputTypeDef:
         """
         Updates the list of Active Directory users and groups that have special
         permissions for SMB file shares on the gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Client.update_smb_local_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/client/#update_smb_local_groups)
```

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/literals.py` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/literals.pyi` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/paginator.py` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,30 +88,30 @@
 class DescribeTapeArchivesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describetapearchivespaginator)
     """
 
     def paginate(
-        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTapeArchivesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describetapearchivespaginator)
         """
 
 
 class DescribeTapeRecoveryPointsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describetaperecoverypointspaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTapeRecoveryPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describetaperecoverypointspaginator)
         """
 
 
@@ -122,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         TapeARNs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describetapespaginator)
         """
 
 
@@ -141,118 +141,118 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         VTLDeviceARNs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeVTLDevicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeVTLDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describevtldevicespaginator)
         """
 
 
 class ListFileSharesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listfilesharespaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFileSharesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listfilesharespaginator)
         """
 
 
 class ListFileSystemAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listfilesystemassociationspaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFileSystemAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listfilesystemassociationspaginator)
         """
 
 
 class ListGatewaysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listgatewayspaginator)
         """
 
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListTapePoolsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listtapepoolspaginator)
     """
 
     def paginate(
-        self, *, PoolARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PoolARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTapePoolsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listtapepoolspaginator)
         """
 
 
 class ListTapesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listtapespaginator)
     """
 
     def paginate(
-        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listtapespaginator)
         """
 
 
 class ListVolumesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listvolumespaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVolumesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listvolumespaginator)
         """
```

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/paginator.pyi` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -85,29 +85,29 @@
 class DescribeTapeArchivesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describetapearchivespaginator)
     """
 
     def paginate(
-        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTapeArchivesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describetapearchivespaginator)
         """
 
 class DescribeTapeRecoveryPointsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describetaperecoverypointspaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTapeRecoveryPointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describetaperecoverypointspaginator)
         """
 
 class DescribeTapesPaginator(AioPaginator):
@@ -117,15 +117,15 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         TapeARNs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describetapespaginator)
         """
 
 class DescribeVTLDevicesPaginator(AioPaginator):
@@ -135,111 +135,111 @@
     """
 
     def paginate(
         self,
         *,
         GatewayARN: str,
         VTLDeviceARNs: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeVTLDevicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeVTLDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#describevtldevicespaginator)
         """
 
 class ListFileSharesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listfilesharespaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFileSharesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listfilesharespaginator)
         """
 
 class ListFileSystemAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listfilesystemassociationspaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFileSystemAssociationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listfilesystemassociationspaginator)
         """
 
 class ListGatewaysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listgatewayspaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listtagsforresourcepaginator)
         """
 
 class ListTapePoolsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listtapepoolspaginator)
     """
 
     def paginate(
-        self, *, PoolARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PoolARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTapePoolsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listtapepoolspaginator)
         """
 
 class ListTapesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listtapespaginator)
     """
 
     def paginate(
-        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TapeARNs: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTapesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listtapespaginator)
         """
 
 class ListVolumesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listvolumespaginator)
     """
 
     def paginate(
-        self, *, GatewayARN: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GatewayARN: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVolumesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/paginators/#listvolumespaginator)
         """
```

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/type_defs.py` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_storagegateway.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ActiveDirectoryStatusType,
     AvailabilityMonitorTestStatusType,
     CaseSensitivityType,
     FileShareTypeType,
     GatewayCapacityType,
@@ -33,231 +33,237 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "ActivateGatewayOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AddCacheInputRequestTypeDef",
-    "AddCacheOutputTypeDef",
-    "AddTagsToResourceOutputTypeDef",
     "AddUploadBufferInputRequestTypeDef",
-    "AddUploadBufferOutputTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
-    "AddWorkingStorageOutputTypeDef",
     "AssignTapePoolInputRequestTypeDef",
-    "AssignTapePoolOutputTypeDef",
     "CacheAttributesTypeDef",
     "EndpointNetworkConfigurationTypeDef",
-    "AssociateFileSystemOutputTypeDef",
     "AttachVolumeInputRequestTypeDef",
-    "AttachVolumeOutputTypeDef",
     "AutomaticTapeCreationRuleTypeDef",
+    "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "VolumeiSCSIAttributesTypeDef",
     "CancelArchivalInputRequestTypeDef",
-    "CancelArchivalOutputTypeDef",
     "CancelRetrievalInputRequestTypeDef",
-    "CancelRetrievalOutputTypeDef",
     "ChapInfoTypeDef",
-    "CreateCachediSCSIVolumeOutputTypeDef",
     "NFSFileShareDefaultsTypeDef",
-    "CreateNFSFileShareOutputTypeDef",
-    "CreateSMBFileShareOutputTypeDef",
-    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
-    "CreateSnapshotOutputTypeDef",
-    "CreateStorediSCSIVolumeOutputTypeDef",
-    "CreateTapePoolOutputTypeDef",
-    "CreateTapeWithBarcodeOutputTypeDef",
-    "CreateTapesOutputTypeDef",
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
-    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
     "DeleteBandwidthRateLimitInputRequestTypeDef",
-    "DeleteBandwidthRateLimitOutputTypeDef",
     "DeleteChapCredentialsInputRequestTypeDef",
-    "DeleteChapCredentialsOutputTypeDef",
     "DeleteFileShareInputRequestTypeDef",
-    "DeleteFileShareOutputTypeDef",
     "DeleteGatewayInputRequestTypeDef",
-    "DeleteGatewayOutputTypeDef",
     "DeleteSnapshotScheduleInputRequestTypeDef",
-    "DeleteSnapshotScheduleOutputTypeDef",
     "DeleteTapeArchiveInputRequestTypeDef",
-    "DeleteTapeArchiveOutputTypeDef",
     "DeleteTapeInputRequestTypeDef",
-    "DeleteTapeOutputTypeDef",
     "DeleteTapePoolInputRequestTypeDef",
-    "DeleteTapePoolOutputTypeDef",
     "DeleteVolumeInputRequestTypeDef",
-    "DeleteVolumeOutputTypeDef",
     "DescribeAvailabilityMonitorTestInputRequestTypeDef",
-    "DescribeAvailabilityMonitorTestOutputTypeDef",
     "DescribeBandwidthRateLimitInputRequestTypeDef",
-    "DescribeBandwidthRateLimitOutputTypeDef",
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCacheInputRequestTypeDef",
-    "DescribeCacheOutputTypeDef",
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     "DescribeChapCredentialsInputRequestTypeDef",
     "DescribeFileSystemAssociationsInputRequestTypeDef",
     "DescribeGatewayInformationInputRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
-    "DescribeMaintenanceStartTimeOutputTypeDef",
     "DescribeNFSFileSharesInputRequestTypeDef",
     "DescribeSMBFileSharesInputRequestTypeDef",
     "DescribeSMBSettingsInputRequestTypeDef",
-    "SMBLocalGroupsTypeDef",
+    "SMBLocalGroupsOutputTypeDef",
     "DescribeSnapshotScheduleInputRequestTypeDef",
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
-    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeTapeArchivesInputRequestTypeDef",
     "TapeArchiveTypeDef",
-    "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     "DescribeTapeRecoveryPointsInputRequestTypeDef",
     "TapeRecoveryPointInfoTypeDef",
-    "DescribeTapesInputDescribeTapesPaginateTypeDef",
     "DescribeTapesInputRequestTypeDef",
     "TapeTypeDef",
     "DescribeUploadBufferInputRequestTypeDef",
-    "DescribeUploadBufferOutputTypeDef",
-    "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     "DescribeVTLDevicesInputRequestTypeDef",
     "DescribeWorkingStorageInputRequestTypeDef",
-    "DescribeWorkingStorageOutputTypeDef",
     "DetachVolumeInputRequestTypeDef",
-    "DetachVolumeOutputTypeDef",
     "DeviceiSCSIAttributesTypeDef",
     "DisableGatewayInputRequestTypeDef",
-    "DisableGatewayOutputTypeDef",
     "DisassociateFileSystemInputRequestTypeDef",
-    "DisassociateFileSystemOutputTypeDef",
     "DiskTypeDef",
+    "EndpointNetworkConfigurationOutputTypeDef",
     "FileShareInfoTypeDef",
     "FileSystemAssociationStatusDetailTypeDef",
     "FileSystemAssociationSummaryTypeDef",
     "GatewayInfoTypeDef",
     "JoinDomainInputRequestTypeDef",
-    "JoinDomainOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
-    "ListFileSharesInputListFileSharesPaginateTypeDef",
     "ListFileSharesInputRequestTypeDef",
-    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
     "ListFileSystemAssociationsInputRequestTypeDef",
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
     "ListGatewaysInputRequestTypeDef",
     "ListLocalDisksInputRequestTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
     "ListTapePoolsInputRequestTypeDef",
     "PoolInfoTypeDef",
-    "ListTapesInputListTapesPaginateTypeDef",
     "ListTapesInputRequestTypeDef",
     "TapeInfoTypeDef",
     "ListVolumeInitiatorsInputRequestTypeDef",
-    "ListVolumeInitiatorsOutputTypeDef",
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     "VolumeRecoveryPointInfoTypeDef",
-    "ListVolumesInputListVolumesPaginateTypeDef",
     "ListVolumesInputRequestTypeDef",
     "VolumeInfoTypeDef",
     "NotifyWhenUploadedInputRequestTypeDef",
-    "NotifyWhenUploadedOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "RefreshCacheInputRequestTypeDef",
-    "RefreshCacheOutputTypeDef",
     "RemoveTagsFromResourceInputRequestTypeDef",
-    "RemoveTagsFromResourceOutputTypeDef",
     "ResetCacheInputRequestTypeDef",
-    "ResetCacheOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "RetrieveTapeArchiveInputRequestTypeDef",
-    "RetrieveTapeArchiveOutputTypeDef",
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
-    "RetrieveTapeRecoveryPointOutputTypeDef",
+    "SMBLocalGroupsTypeDef",
     "SetLocalConsolePasswordInputRequestTypeDef",
-    "SetLocalConsolePasswordOutputTypeDef",
     "SetSMBGuestPasswordInputRequestTypeDef",
-    "SetSMBGuestPasswordOutputTypeDef",
     "ShutdownGatewayInputRequestTypeDef",
-    "ShutdownGatewayOutputTypeDef",
     "StartAvailabilityMonitorTestInputRequestTypeDef",
-    "StartAvailabilityMonitorTestOutputTypeDef",
     "StartGatewayInputRequestTypeDef",
-    "StartGatewayOutputTypeDef",
-    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
     "UpdateBandwidthRateLimitInputRequestTypeDef",
-    "UpdateBandwidthRateLimitOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
     "UpdateChapCredentialsInputRequestTypeDef",
-    "UpdateChapCredentialsOutputTypeDef",
-    "UpdateFileSystemAssociationOutputTypeDef",
     "UpdateGatewayInformationInputRequestTypeDef",
-    "UpdateGatewayInformationOutputTypeDef",
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
-    "UpdateGatewaySoftwareNowOutputTypeDef",
     "UpdateMaintenanceStartTimeInputRequestTypeDef",
-    "UpdateMaintenanceStartTimeOutputTypeDef",
-    "UpdateNFSFileShareOutputTypeDef",
-    "UpdateSMBFileShareOutputTypeDef",
     "UpdateSMBFileShareVisibilityInputRequestTypeDef",
-    "UpdateSMBFileShareVisibilityOutputTypeDef",
-    "UpdateSMBLocalGroupsOutputTypeDef",
     "UpdateSMBSecurityStrategyInputRequestTypeDef",
-    "UpdateSMBSecurityStrategyOutputTypeDef",
-    "UpdateSnapshotScheduleOutputTypeDef",
     "UpdateVTLDeviceTypeInputRequestTypeDef",
-    "UpdateVTLDeviceTypeOutputTypeDef",
     "ActivateGatewayInputRequestTypeDef",
     "AddTagsToResourceInputRequestTypeDef",
     "CreateCachediSCSIVolumeInputRequestTypeDef",
     "CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef",
     "CreateSnapshotInputRequestTypeDef",
     "CreateStorediSCSIVolumeInputRequestTypeDef",
     "CreateTapePoolInputRequestTypeDef",
     "CreateTapeWithBarcodeInputRequestTypeDef",
     "CreateTapesInputRequestTypeDef",
+    "UpdateSnapshotScheduleInputRequestTypeDef",
+    "ActivateGatewayOutputTypeDef",
+    "AddCacheOutputTypeDef",
+    "AddTagsToResourceOutputTypeDef",
+    "AddUploadBufferOutputTypeDef",
+    "AddWorkingStorageOutputTypeDef",
+    "AssignTapePoolOutputTypeDef",
+    "AssociateFileSystemOutputTypeDef",
+    "AttachVolumeOutputTypeDef",
+    "CancelArchivalOutputTypeDef",
+    "CancelRetrievalOutputTypeDef",
+    "CreateCachediSCSIVolumeOutputTypeDef",
+    "CreateNFSFileShareOutputTypeDef",
+    "CreateSMBFileShareOutputTypeDef",
+    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
+    "CreateSnapshotOutputTypeDef",
+    "CreateStorediSCSIVolumeOutputTypeDef",
+    "CreateTapePoolOutputTypeDef",
+    "CreateTapeWithBarcodeOutputTypeDef",
+    "CreateTapesOutputTypeDef",
+    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
+    "DeleteBandwidthRateLimitOutputTypeDef",
+    "DeleteChapCredentialsOutputTypeDef",
+    "DeleteFileShareOutputTypeDef",
+    "DeleteGatewayOutputTypeDef",
+    "DeleteSnapshotScheduleOutputTypeDef",
+    "DeleteTapeArchiveOutputTypeDef",
+    "DeleteTapeOutputTypeDef",
+    "DeleteTapePoolOutputTypeDef",
+    "DeleteVolumeOutputTypeDef",
+    "DescribeAvailabilityMonitorTestOutputTypeDef",
+    "DescribeBandwidthRateLimitOutputTypeDef",
+    "DescribeCacheOutputTypeDef",
+    "DescribeMaintenanceStartTimeOutputTypeDef",
     "DescribeSnapshotScheduleOutputTypeDef",
+    "DescribeUploadBufferOutputTypeDef",
+    "DescribeWorkingStorageOutputTypeDef",
+    "DetachVolumeOutputTypeDef",
+    "DisableGatewayOutputTypeDef",
+    "DisassociateFileSystemOutputTypeDef",
+    "JoinDomainOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "UpdateSnapshotScheduleInputRequestTypeDef",
+    "ListVolumeInitiatorsOutputTypeDef",
+    "NotifyWhenUploadedOutputTypeDef",
+    "RefreshCacheOutputTypeDef",
+    "RemoveTagsFromResourceOutputTypeDef",
+    "ResetCacheOutputTypeDef",
+    "RetrieveTapeArchiveOutputTypeDef",
+    "RetrieveTapeRecoveryPointOutputTypeDef",
+    "SetLocalConsolePasswordOutputTypeDef",
+    "SetSMBGuestPasswordOutputTypeDef",
+    "ShutdownGatewayOutputTypeDef",
+    "StartAvailabilityMonitorTestOutputTypeDef",
+    "StartGatewayOutputTypeDef",
+    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
+    "UpdateBandwidthRateLimitOutputTypeDef",
+    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
+    "UpdateChapCredentialsOutputTypeDef",
+    "UpdateFileSystemAssociationOutputTypeDef",
+    "UpdateGatewayInformationOutputTypeDef",
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    "UpdateMaintenanceStartTimeOutputTypeDef",
+    "UpdateNFSFileShareOutputTypeDef",
+    "UpdateSMBFileShareOutputTypeDef",
+    "UpdateSMBFileShareVisibilityOutputTypeDef",
+    "UpdateSMBLocalGroupsOutputTypeDef",
+    "UpdateSMBSecurityStrategyOutputTypeDef",
+    "UpdateSnapshotScheduleOutputTypeDef",
+    "UpdateVTLDeviceTypeOutputTypeDef",
     "CreateSMBFileShareInputRequestTypeDef",
     "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
+    "BandwidthRateLimitIntervalUnionTypeDef",
     "CachediSCSIVolumeTypeDef",
     "StorediSCSIVolumeTypeDef",
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
     "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
     "DescribeSMBSettingsOutputTypeDef",
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
+    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+    "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    "DescribeTapesInputDescribeTapesPaginateTypeDef",
+    "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    "ListFileSharesInputListFileSharesPaginateTypeDef",
+    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
+    "ListTapesInputListTapesPaginateTypeDef",
+    "ListVolumesInputListVolumesPaginateTypeDef",
     "DescribeTapeArchivesOutputTypeDef",
     "DescribeTapeRecoveryPointsOutputTypeDef",
     "DescribeTapesOutputTypeDef",
     "VTLDeviceTypeDef",
     "ListLocalDisksOutputTypeDef",
+    "EndpointNetworkConfigurationUnionTypeDef",
     "ListFileSharesOutputTypeDef",
     "FileSystemAssociationInfoTypeDef",
     "ListFileSystemAssociationsOutputTypeDef",
     "ListGatewaysOutputTypeDef",
     "ListTapePoolsOutputTypeDef",
     "ListTapesOutputTypeDef",
     "ListVolumeRecoveryPointsOutputTypeDef",
     "ListVolumesOutputTypeDef",
+    "SMBLocalGroupsUnionTypeDef",
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
     "DescribeSMBFileSharesOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCachediSCSIVolumesOutputTypeDef",
     "DescribeStorediSCSIVolumesOutputTypeDef",
     "DescribeNFSFileSharesOutputTypeDef",
     "DescribeVTLDevicesOutputTypeDef",
     "DescribeFileSystemAssociationsOutputTypeDef",
 )
 
@@ -265,78 +271,49 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ActivateGatewayOutputTypeDef = TypedDict(
-    "ActivateGatewayOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AddCacheInputRequestTypeDef = TypedDict(
     "AddCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
-AddCacheOutputTypeDef = TypedDict(
-    "AddCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AddTagsToResourceOutputTypeDef = TypedDict(
-    "AddTagsToResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddUploadBufferInputRequestTypeDef = TypedDict(
     "AddUploadBufferInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
-AddUploadBufferOutputTypeDef = TypedDict(
-    "AddUploadBufferOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddWorkingStorageInputRequestTypeDef = TypedDict(
     "AddWorkingStorageInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
-AddWorkingStorageOutputTypeDef = TypedDict(
-    "AddWorkingStorageOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssignTapePoolInputRequestTypeDef = TypedDict(
     "_RequiredAssignTapePoolInputRequestTypeDef",
     {
         "TapeARN": str,
         "PoolId": str,
     },
 )
@@ -351,22 +328,14 @@
 
 class AssignTapePoolInputRequestTypeDef(
     _RequiredAssignTapePoolInputRequestTypeDef, _OptionalAssignTapePoolInputRequestTypeDef
 ):
     pass
 
 
-AssignTapePoolOutputTypeDef = TypedDict(
-    "AssignTapePoolOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CacheAttributesTypeDef = TypedDict(
     "CacheAttributesTypeDef",
     {
         "CacheStaleTimeoutInSeconds": int,
     },
     total=False,
 )
@@ -375,22 +344,14 @@
     "EndpointNetworkConfigurationTypeDef",
     {
         "IpAddresses": Sequence[str],
     },
     total=False,
 )
 
-AssociateFileSystemOutputTypeDef = TypedDict(
-    "AssociateFileSystemOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAttachVolumeInputRequestTypeDef = TypedDict(
     "_RequiredAttachVolumeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "VolumeARN": str,
         "NetworkInterfaceId": str,
     },
@@ -407,23 +368,14 @@
 
 class AttachVolumeInputRequestTypeDef(
     _RequiredAttachVolumeInputRequestTypeDef, _OptionalAttachVolumeInputRequestTypeDef
 ):
     pass
 
 
-AttachVolumeOutputTypeDef = TypedDict(
-    "AttachVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "TargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAutomaticTapeCreationRuleTypeDef = TypedDict(
     "_RequiredAutomaticTapeCreationRuleTypeDef",
     {
         "TapeBarcodePrefix": str,
         "PoolId": str,
         "TapeSizeInBytes": int,
         "MinimumNumTapes": int,
@@ -440,22 +392,49 @@
 
 class AutomaticTapeCreationRuleTypeDef(
     _RequiredAutomaticTapeCreationRuleTypeDef, _OptionalAutomaticTapeCreationRuleTypeDef
 ):
     pass
 
 
+_RequiredBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
+    "_RequiredBandwidthRateLimitIntervalOutputTypeDef",
+    {
+        "StartHourOfDay": int,
+        "StartMinuteOfHour": int,
+        "EndHourOfDay": int,
+        "EndMinuteOfHour": int,
+        "DaysOfWeek": List[int],
+    },
+)
+_OptionalBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
+    "_OptionalBandwidthRateLimitIntervalOutputTypeDef",
+    {
+        "AverageUploadRateLimitInBitsPerSec": int,
+        "AverageDownloadRateLimitInBitsPerSec": int,
+    },
+    total=False,
+)
+
+
+class BandwidthRateLimitIntervalOutputTypeDef(
+    _RequiredBandwidthRateLimitIntervalOutputTypeDef,
+    _OptionalBandwidthRateLimitIntervalOutputTypeDef,
+):
+    pass
+
+
 _RequiredBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_RequiredBandwidthRateLimitIntervalTypeDef",
     {
         "StartHourOfDay": int,
         "StartMinuteOfHour": int,
         "EndHourOfDay": int,
         "EndMinuteOfHour": int,
-        "DaysOfWeek": List[int],
+        "DaysOfWeek": Sequence[int],
     },
 )
 _OptionalBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_OptionalBandwidthRateLimitIntervalTypeDef",
     {
         "AverageUploadRateLimitInBitsPerSec": int,
         "AverageDownloadRateLimitInBitsPerSec": int,
@@ -486,186 +465,67 @@
     "CancelArchivalInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
 
-CancelArchivalOutputTypeDef = TypedDict(
-    "CancelArchivalOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CancelRetrievalInputRequestTypeDef = TypedDict(
     "CancelRetrievalInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
 
-CancelRetrievalOutputTypeDef = TypedDict(
-    "CancelRetrievalOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ChapInfoTypeDef = TypedDict(
     "ChapInfoTypeDef",
     {
         "TargetARN": str,
         "SecretToAuthenticateInitiator": str,
         "InitiatorName": str,
         "SecretToAuthenticateTarget": str,
     },
     total=False,
 )
 
-CreateCachediSCSIVolumeOutputTypeDef = TypedDict(
-    "CreateCachediSCSIVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "TargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NFSFileShareDefaultsTypeDef = TypedDict(
     "NFSFileShareDefaultsTypeDef",
     {
         "FileMode": str,
         "DirectoryMode": str,
         "GroupId": int,
         "OwnerId": int,
     },
     total=False,
 )
 
-CreateNFSFileShareOutputTypeDef = TypedDict(
-    "CreateNFSFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSMBFileShareOutputTypeDef = TypedDict(
-    "CreateSMBFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSnapshotFromVolumeRecoveryPointOutputTypeDef = TypedDict(
-    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
-    {
-        "SnapshotId": str,
-        "VolumeARN": str,
-        "VolumeRecoveryPointTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSnapshotOutputTypeDef = TypedDict(
-    "CreateSnapshotOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "SnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStorediSCSIVolumeOutputTypeDef = TypedDict(
-    "CreateStorediSCSIVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "VolumeSizeInBytes": int,
-        "TargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTapePoolOutputTypeDef = TypedDict(
-    "CreateTapePoolOutputTypeDef",
-    {
-        "PoolARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTapeWithBarcodeOutputTypeDef = TypedDict(
-    "CreateTapeWithBarcodeOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTapesOutputTypeDef = TypedDict(
-    "CreateTapesOutputTypeDef",
-    {
-        "TapeARNs": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAutomaticTapeCreationPolicyInputRequestTypeDef = TypedDict(
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DeleteAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
-    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "DeleteBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
         "BandwidthType": str,
     },
 )
 
-DeleteBandwidthRateLimitOutputTypeDef = TypedDict(
-    "DeleteBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteChapCredentialsInputRequestTypeDef = TypedDict(
     "DeleteChapCredentialsInputRequestTypeDef",
     {
         "TargetARN": str,
         "InitiatorName": str,
     },
 )
 
-DeleteChapCredentialsOutputTypeDef = TypedDict(
-    "DeleteChapCredentialsOutputTypeDef",
-    {
-        "TargetARN": str,
-        "InitiatorName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteFileShareInputRequestTypeDef = TypedDict(
     "_RequiredDeleteFileShareInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalDeleteFileShareInputRequestTypeDef = TypedDict(
@@ -679,52 +539,28 @@
 
 class DeleteFileShareInputRequestTypeDef(
     _RequiredDeleteFileShareInputRequestTypeDef, _OptionalDeleteFileShareInputRequestTypeDef
 ):
     pass
 
 
-DeleteFileShareOutputTypeDef = TypedDict(
-    "DeleteFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGatewayInputRequestTypeDef = TypedDict(
     "DeleteGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DeleteGatewayOutputTypeDef = TypedDict(
-    "DeleteGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSnapshotScheduleInputRequestTypeDef = TypedDict(
     "DeleteSnapshotScheduleInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
-DeleteSnapshotScheduleOutputTypeDef = TypedDict(
-    "DeleteSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTapeArchiveInputRequestTypeDef = TypedDict(
     "_RequiredDeleteTapeArchiveInputRequestTypeDef",
     {
         "TapeARN": str,
     },
 )
 _OptionalDeleteTapeArchiveInputRequestTypeDef = TypedDict(
@@ -738,22 +574,14 @@
 
 class DeleteTapeArchiveInputRequestTypeDef(
     _RequiredDeleteTapeArchiveInputRequestTypeDef, _OptionalDeleteTapeArchiveInputRequestTypeDef
 ):
     pass
 
 
-DeleteTapeArchiveOutputTypeDef = TypedDict(
-    "DeleteTapeArchiveOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTapeInputRequestTypeDef = TypedDict(
     "_RequiredDeleteTapeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
@@ -768,114 +596,56 @@
 
 class DeleteTapeInputRequestTypeDef(
     _RequiredDeleteTapeInputRequestTypeDef, _OptionalDeleteTapeInputRequestTypeDef
 ):
     pass
 
 
-DeleteTapeOutputTypeDef = TypedDict(
-    "DeleteTapeOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTapePoolInputRequestTypeDef = TypedDict(
     "DeleteTapePoolInputRequestTypeDef",
     {
         "PoolARN": str,
     },
 )
 
-DeleteTapePoolOutputTypeDef = TypedDict(
-    "DeleteTapePoolOutputTypeDef",
-    {
-        "PoolARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVolumeInputRequestTypeDef = TypedDict(
     "DeleteVolumeInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
-DeleteVolumeOutputTypeDef = TypedDict(
-    "DeleteVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAvailabilityMonitorTestInputRequestTypeDef = TypedDict(
     "DescribeAvailabilityMonitorTestInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeAvailabilityMonitorTestOutputTypeDef = TypedDict(
-    "DescribeAvailabilityMonitorTestOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "Status": AvailabilityMonitorTestStatusType,
-        "StartTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "DescribeBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeBandwidthRateLimitOutputTypeDef = TypedDict(
-    "DescribeBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "AverageUploadRateLimitInBitsPerSec": int,
-        "AverageDownloadRateLimitInBitsPerSec": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
 DescribeCacheInputRequestTypeDef = TypedDict(
     "DescribeCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeCacheOutputTypeDef = TypedDict(
-    "DescribeCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "CacheAllocatedInBytes": int,
-        "CacheUsedPercentage": float,
-        "CacheDirtyPercentage": float,
-        "CacheHitPercentage": float,
-        "CacheMissPercentage": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeCachediSCSIVolumesInputRequestTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     {
         "VolumeARNs": Sequence[str],
     },
 )
 
@@ -913,27 +683,14 @@
 DescribeMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "DescribeMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "HourOfDay": int,
-        "MinuteOfHour": int,
-        "DayOfWeek": int,
-        "DayOfMonth": int,
-        "Timezone": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeNFSFileSharesInputRequestTypeDef = TypedDict(
     "DescribeNFSFileSharesInputRequestTypeDef",
     {
         "FileShareARNList": Sequence[str],
     },
 )
 
@@ -947,16 +704,16 @@
 DescribeSMBSettingsInputRequestTypeDef = TypedDict(
     "DescribeSMBSettingsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-SMBLocalGroupsTypeDef = TypedDict(
-    "SMBLocalGroupsTypeDef",
+SMBLocalGroupsOutputTypeDef = TypedDict(
+    "SMBLocalGroupsOutputTypeDef",
     {
         "GatewayAdmins": List[str],
     },
     total=False,
 )
 
 DescribeSnapshotScheduleInputRequestTypeDef = TypedDict(
@@ -969,19 +726,20 @@
 DescribeStorediSCSIVolumesInputRequestTypeDef = TypedDict(
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
     {
         "VolumeARNs": Sequence[str],
     },
 )
 
-DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
-    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeTapeArchivesInputRequestTypeDef = TypedDict(
     "DescribeTapeArchivesInputRequestTypeDef",
     {
@@ -1008,36 +766,14 @@
         "Worm": bool,
         "RetentionStartDate": datetime,
         "PoolEntryDate": datetime,
     },
     total=False,
 )
 
-_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef(
-    _RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-    _OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeTapeRecoveryPointsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTapeRecoveryPointsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeTapeRecoveryPointsInputRequestTypeDef = TypedDict(
@@ -1064,37 +800,14 @@
         "TapeRecoveryPointTime": datetime,
         "TapeSizeInBytes": int,
         "TapeStatus": str,
     },
     total=False,
 )
 
-_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeTapesInputDescribeTapesPaginateTypeDef(
-    _RequiredDescribeTapesInputDescribeTapesPaginateTypeDef,
-    _OptionalDescribeTapesInputDescribeTapesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeTapesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTapesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeTapesInputRequestTypeDef = TypedDict(
@@ -1137,48 +850,14 @@
 DescribeUploadBufferInputRequestTypeDef = TypedDict(
     "DescribeUploadBufferInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeUploadBufferOutputTypeDef = TypedDict(
-    "DescribeUploadBufferOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "UploadBufferUsedInBytes": int,
-        "UploadBufferAllocatedInBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    {
-        "VTLDeviceARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef(
-    _RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-    _OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeVTLDevicesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVTLDevicesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeVTLDevicesInputRequestTypeDef = TypedDict(
@@ -1201,25 +880,14 @@
 DescribeWorkingStorageInputRequestTypeDef = TypedDict(
     "DescribeWorkingStorageInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeWorkingStorageOutputTypeDef = TypedDict(
-    "DescribeWorkingStorageOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "WorkingStorageUsedInBytes": int,
-        "WorkingStorageAllocatedInBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDetachVolumeInputRequestTypeDef = TypedDict(
     "_RequiredDetachVolumeInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 _OptionalDetachVolumeInputRequestTypeDef = TypedDict(
@@ -1233,22 +901,14 @@
 
 class DetachVolumeInputRequestTypeDef(
     _RequiredDetachVolumeInputRequestTypeDef, _OptionalDetachVolumeInputRequestTypeDef
 ):
     pass
 
 
-DetachVolumeOutputTypeDef = TypedDict(
-    "DetachVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceiSCSIAttributesTypeDef = TypedDict(
     "DeviceiSCSIAttributesTypeDef",
     {
         "TargetARN": str,
         "NetworkInterfaceId": str,
         "NetworkInterfacePort": int,
         "ChapEnabled": bool,
@@ -1259,22 +919,14 @@
 DisableGatewayInputRequestTypeDef = TypedDict(
     "DisableGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DisableGatewayOutputTypeDef = TypedDict(
-    "DisableGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisassociateFileSystemInputRequestTypeDef = TypedDict(
     "_RequiredDisassociateFileSystemInputRequestTypeDef",
     {
         "FileSystemAssociationARN": str,
     },
 )
 _OptionalDisassociateFileSystemInputRequestTypeDef = TypedDict(
@@ -1289,22 +941,14 @@
 class DisassociateFileSystemInputRequestTypeDef(
     _RequiredDisassociateFileSystemInputRequestTypeDef,
     _OptionalDisassociateFileSystemInputRequestTypeDef,
 ):
     pass
 
 
-DisassociateFileSystemOutputTypeDef = TypedDict(
-    "DisassociateFileSystemOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DiskTypeDef = TypedDict(
     "DiskTypeDef",
     {
         "DiskId": str,
         "DiskPath": str,
         "DiskNode": str,
         "DiskStatus": str,
@@ -1312,14 +956,22 @@
         "DiskAllocationType": str,
         "DiskAllocationResource": str,
         "DiskAttributeList": List[str],
     },
     total=False,
 )
 
+EndpointNetworkConfigurationOutputTypeDef = TypedDict(
+    "EndpointNetworkConfigurationOutputTypeDef",
+    {
+        "IpAddresses": List[str],
+    },
+    total=False,
+)
+
 FileShareInfoTypeDef = TypedDict(
     "FileShareInfoTypeDef",
     {
         "FileShareType": FileShareTypeType,
         "FileShareARN": str,
         "FileShareId": str,
         "FileShareStatus": str,
@@ -1385,77 +1037,42 @@
 
 class JoinDomainInputRequestTypeDef(
     _RequiredJoinDomainInputRequestTypeDef, _OptionalJoinDomainInputRequestTypeDef
 ):
     pass
 
 
-JoinDomainOutputTypeDef = TypedDict(
-    "JoinDomainOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ActiveDirectoryStatus": ActiveDirectoryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListAutomaticTapeCreationPoliciesInputRequestTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
     total=False,
 )
 
-ListFileSharesInputListFileSharesPaginateTypeDef = TypedDict(
-    "ListFileSharesInputListFileSharesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFileSharesInputRequestTypeDef = TypedDict(
     "ListFileSharesInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef = TypedDict(
-    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFileSystemAssociationsInputRequestTypeDef = TypedDict(
     "ListFileSystemAssociationsInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGatewaysInputRequestTypeDef = TypedDict(
     "ListGatewaysInputRequestTypeDef",
     {
         "Marker": str,
         "Limit": int,
     },
     total=False,
@@ -1464,36 +1081,14 @@
 ListLocalDisksInputRequestTypeDef = TypedDict(
     "ListLocalDisksInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1508,23 +1103,14 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
-ListTapePoolsInputListTapePoolsPaginateTypeDef = TypedDict(
-    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
-    {
-        "PoolARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTapePoolsInputRequestTypeDef = TypedDict(
     "ListTapePoolsInputRequestTypeDef",
     {
         "PoolARNs": Sequence[str],
         "Marker": str,
         "Limit": int,
     },
@@ -1540,23 +1126,14 @@
         "RetentionLockType": RetentionLockTypeType,
         "RetentionLockTimeInDays": int,
         "PoolStatus": PoolStatusType,
     },
     total=False,
 )
 
-ListTapesInputListTapesPaginateTypeDef = TypedDict(
-    "ListTapesInputListTapesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTapesInputRequestTypeDef = TypedDict(
     "ListTapesInputRequestTypeDef",
     {
         "TapeARNs": Sequence[str],
         "Marker": str,
         "Limit": int,
     },
@@ -1581,22 +1158,14 @@
 ListVolumeInitiatorsInputRequestTypeDef = TypedDict(
     "ListVolumeInitiatorsInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
-ListVolumeInitiatorsOutputTypeDef = TypedDict(
-    "ListVolumeInitiatorsOutputTypeDef",
-    {
-        "Initiators": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListVolumeRecoveryPointsInputRequestTypeDef = TypedDict(
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
@@ -1607,23 +1176,14 @@
         "VolumeSizeInBytes": int,
         "VolumeUsageInBytes": int,
         "VolumeRecoveryPointTime": str,
     },
     total=False,
 )
 
-ListVolumesInputListVolumesPaginateTypeDef = TypedDict(
-    "ListVolumesInputListVolumesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVolumesInputRequestTypeDef = TypedDict(
     "ListVolumesInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Marker": str,
         "Limit": int,
     },
@@ -1647,33 +1207,14 @@
 NotifyWhenUploadedInputRequestTypeDef = TypedDict(
     "NotifyWhenUploadedInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 
-NotifyWhenUploadedOutputTypeDef = TypedDict(
-    "NotifyWhenUploadedOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "NotificationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 _RequiredRefreshCacheInputRequestTypeDef = TypedDict(
     "_RequiredRefreshCacheInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalRefreshCacheInputRequestTypeDef = TypedDict(
@@ -1688,182 +1229,90 @@
 
 class RefreshCacheInputRequestTypeDef(
     _RequiredRefreshCacheInputRequestTypeDef, _OptionalRefreshCacheInputRequestTypeDef
 ):
     pass
 
 
-RefreshCacheOutputTypeDef = TypedDict(
-    "RefreshCacheOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "NotificationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromResourceInputRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-RemoveTagsFromResourceOutputTypeDef = TypedDict(
-    "RemoveTagsFromResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResetCacheInputRequestTypeDef = TypedDict(
     "ResetCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-ResetCacheOutputTypeDef = TypedDict(
-    "ResetCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
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
 RetrieveTapeArchiveInputRequestTypeDef = TypedDict(
     "RetrieveTapeArchiveInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
-RetrieveTapeArchiveOutputTypeDef = TypedDict(
-    "RetrieveTapeArchiveOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RetrieveTapeRecoveryPointInputRequestTypeDef = TypedDict(
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
-RetrieveTapeRecoveryPointOutputTypeDef = TypedDict(
-    "RetrieveTapeRecoveryPointOutputTypeDef",
+SMBLocalGroupsTypeDef = TypedDict(
+    "SMBLocalGroupsTypeDef",
     {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "GatewayAdmins": Sequence[str],
     },
+    total=False,
 )
 
 SetLocalConsolePasswordInputRequestTypeDef = TypedDict(
     "SetLocalConsolePasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "LocalConsolePassword": str,
     },
 )
 
-SetLocalConsolePasswordOutputTypeDef = TypedDict(
-    "SetLocalConsolePasswordOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetSMBGuestPasswordInputRequestTypeDef = TypedDict(
     "SetSMBGuestPasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Password": str,
     },
 )
 
-SetSMBGuestPasswordOutputTypeDef = TypedDict(
-    "SetSMBGuestPasswordOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ShutdownGatewayInputRequestTypeDef = TypedDict(
     "ShutdownGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-ShutdownGatewayOutputTypeDef = TypedDict(
-    "ShutdownGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartAvailabilityMonitorTestInputRequestTypeDef = TypedDict(
     "StartAvailabilityMonitorTestInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-StartAvailabilityMonitorTestOutputTypeDef = TypedDict(
-    "StartAvailabilityMonitorTestOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartGatewayInputRequestTypeDef = TypedDict(
     "StartGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-StartGatewayOutputTypeDef = TypedDict(
-    "StartGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
-    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "_RequiredUpdateBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalUpdateBandwidthRateLimitInputRequestTypeDef = TypedDict(
@@ -1879,30 +1328,14 @@
 class UpdateBandwidthRateLimitInputRequestTypeDef(
     _RequiredUpdateBandwidthRateLimitInputRequestTypeDef,
     _OptionalUpdateBandwidthRateLimitInputRequestTypeDef,
 ):
     pass
 
 
-UpdateBandwidthRateLimitOutputTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChapCredentialsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateChapCredentialsInputRequestTypeDef",
     {
         "TargetARN": str,
         "SecretToAuthenticateInitiator": str,
         "InitiatorName": str,
     },
@@ -1919,31 +1352,14 @@
 class UpdateChapCredentialsInputRequestTypeDef(
     _RequiredUpdateChapCredentialsInputRequestTypeDef,
     _OptionalUpdateChapCredentialsInputRequestTypeDef,
 ):
     pass
 
 
-UpdateChapCredentialsOutputTypeDef = TypedDict(
-    "UpdateChapCredentialsOutputTypeDef",
-    {
-        "TargetARN": str,
-        "InitiatorName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateFileSystemAssociationOutputTypeDef = TypedDict(
-    "UpdateFileSystemAssociationOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalUpdateGatewayInformationInputRequestTypeDef = TypedDict(
@@ -1961,38 +1377,21 @@
 class UpdateGatewayInformationInputRequestTypeDef(
     _RequiredUpdateGatewayInformationInputRequestTypeDef,
     _OptionalUpdateGatewayInformationInputRequestTypeDef,
 ):
     pass
 
 
-UpdateGatewayInformationOutputTypeDef = TypedDict(
-    "UpdateGatewayInformationOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "GatewayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateGatewaySoftwareNowInputRequestTypeDef = TypedDict(
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
-    "UpdateGatewaySoftwareNowOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
@@ -2010,102 +1409,38 @@
 class UpdateMaintenanceStartTimeInputRequestTypeDef(
     _RequiredUpdateMaintenanceStartTimeInputRequestTypeDef,
     _OptionalUpdateMaintenanceStartTimeInputRequestTypeDef,
 ):
     pass
 
 
-UpdateMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "UpdateMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateNFSFileShareOutputTypeDef = TypedDict(
-    "UpdateNFSFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSMBFileShareOutputTypeDef = TypedDict(
-    "UpdateSMBFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSMBFileShareVisibilityInputRequestTypeDef = TypedDict(
     "UpdateSMBFileShareVisibilityInputRequestTypeDef",
     {
         "GatewayARN": str,
         "FileSharesVisible": bool,
     },
 )
 
-UpdateSMBFileShareVisibilityOutputTypeDef = TypedDict(
-    "UpdateSMBFileShareVisibilityOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSMBLocalGroupsOutputTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSMBSecurityStrategyInputRequestTypeDef = TypedDict(
     "UpdateSMBSecurityStrategyInputRequestTypeDef",
     {
         "GatewayARN": str,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
     },
 )
 
-UpdateSMBSecurityStrategyOutputTypeDef = TypedDict(
-    "UpdateSMBSecurityStrategyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSnapshotScheduleOutputTypeDef = TypedDict(
-    "UpdateSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateVTLDeviceTypeInputRequestTypeDef = TypedDict(
     "UpdateVTLDeviceTypeInputRequestTypeDef",
     {
         "VTLDeviceARN": str,
         "DeviceType": str,
     },
 )
 
-UpdateVTLDeviceTypeOutputTypeDef = TypedDict(
-    "UpdateVTLDeviceTypeOutputTypeDef",
-    {
-        "VTLDeviceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredActivateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredActivateGatewayInputRequestTypeDef",
     {
         "ActivationKey": str,
         "GatewayName": str,
         "GatewayTimezone": str,
         "GatewayRegion": str,
@@ -2318,61 +1653,623 @@
 
 class CreateTapesInputRequestTypeDef(
     _RequiredCreateTapesInputRequestTypeDef, _OptionalCreateTapesInputRequestTypeDef
 ):
     pass
 
 
+_RequiredUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateSnapshotScheduleInputRequestTypeDef",
+    {
+        "VolumeARN": str,
+        "StartAt": int,
+        "RecurrenceInHours": int,
+    },
+)
+_OptionalUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateSnapshotScheduleInputRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateSnapshotScheduleInputRequestTypeDef(
+    _RequiredUpdateSnapshotScheduleInputRequestTypeDef,
+    _OptionalUpdateSnapshotScheduleInputRequestTypeDef,
+):
+    pass
+
+
+ActivateGatewayOutputTypeDef = TypedDict(
+    "ActivateGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddCacheOutputTypeDef = TypedDict(
+    "AddCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddTagsToResourceOutputTypeDef = TypedDict(
+    "AddTagsToResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddUploadBufferOutputTypeDef = TypedDict(
+    "AddUploadBufferOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddWorkingStorageOutputTypeDef = TypedDict(
+    "AddWorkingStorageOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssignTapePoolOutputTypeDef = TypedDict(
+    "AssignTapePoolOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateFileSystemOutputTypeDef = TypedDict(
+    "AssociateFileSystemOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachVolumeOutputTypeDef = TypedDict(
+    "AttachVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "TargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelArchivalOutputTypeDef = TypedDict(
+    "CancelArchivalOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelRetrievalOutputTypeDef = TypedDict(
+    "CancelRetrievalOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCachediSCSIVolumeOutputTypeDef = TypedDict(
+    "CreateCachediSCSIVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "TargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNFSFileShareOutputTypeDef = TypedDict(
+    "CreateNFSFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSMBFileShareOutputTypeDef = TypedDict(
+    "CreateSMBFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotFromVolumeRecoveryPointOutputTypeDef = TypedDict(
+    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
+    {
+        "SnapshotId": str,
+        "VolumeARN": str,
+        "VolumeRecoveryPointTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotOutputTypeDef = TypedDict(
+    "CreateSnapshotOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "SnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStorediSCSIVolumeOutputTypeDef = TypedDict(
+    "CreateStorediSCSIVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "VolumeSizeInBytes": int,
+        "TargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTapePoolOutputTypeDef = TypedDict(
+    "CreateTapePoolOutputTypeDef",
+    {
+        "PoolARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTapeWithBarcodeOutputTypeDef = TypedDict(
+    "CreateTapeWithBarcodeOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTapesOutputTypeDef = TypedDict(
+    "CreateTapesOutputTypeDef",
+    {
+        "TapeARNs": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
+    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBandwidthRateLimitOutputTypeDef = TypedDict(
+    "DeleteBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteChapCredentialsOutputTypeDef = TypedDict(
+    "DeleteChapCredentialsOutputTypeDef",
+    {
+        "TargetARN": str,
+        "InitiatorName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFileShareOutputTypeDef = TypedDict(
+    "DeleteFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGatewayOutputTypeDef = TypedDict(
+    "DeleteGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotScheduleOutputTypeDef = TypedDict(
+    "DeleteSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTapeArchiveOutputTypeDef = TypedDict(
+    "DeleteTapeArchiveOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTapeOutputTypeDef = TypedDict(
+    "DeleteTapeOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTapePoolOutputTypeDef = TypedDict(
+    "DeleteTapePoolOutputTypeDef",
+    {
+        "PoolARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVolumeOutputTypeDef = TypedDict(
+    "DeleteVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAvailabilityMonitorTestOutputTypeDef = TypedDict(
+    "DescribeAvailabilityMonitorTestOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "Status": AvailabilityMonitorTestStatusType,
+        "StartTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBandwidthRateLimitOutputTypeDef = TypedDict(
+    "DescribeBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "AverageUploadRateLimitInBitsPerSec": int,
+        "AverageDownloadRateLimitInBitsPerSec": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCacheOutputTypeDef = TypedDict(
+    "DescribeCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "CacheAllocatedInBytes": int,
+        "CacheUsedPercentage": float,
+        "CacheDirtyPercentage": float,
+        "CacheHitPercentage": float,
+        "CacheMissPercentage": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "DescribeMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "HourOfDay": int,
+        "MinuteOfHour": int,
+        "DayOfWeek": int,
+        "DayOfMonth": int,
+        "Timezone": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeSnapshotScheduleOutputTypeDef = TypedDict(
     "DescribeSnapshotScheduleOutputTypeDef",
     {
         "VolumeARN": str,
         "StartAt": int,
         "RecurrenceInHours": int,
         "Description": str,
         "Timezone": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUploadBufferOutputTypeDef = TypedDict(
+    "DescribeUploadBufferOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "UploadBufferUsedInBytes": int,
+        "UploadBufferAllocatedInBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorkingStorageOutputTypeDef = TypedDict(
+    "DescribeWorkingStorageOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "WorkingStorageUsedInBytes": int,
+        "WorkingStorageAllocatedInBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachVolumeOutputTypeDef = TypedDict(
+    "DetachVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableGatewayOutputTypeDef = TypedDict(
+    "DisableGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateFileSystemOutputTypeDef = TypedDict(
+    "DisassociateFileSystemOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+JoinDomainOutputTypeDef = TypedDict(
+    "JoinDomainOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ActiveDirectoryStatus": ActiveDirectoryStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "ResourceARN": str,
         "Marker": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateSnapshotScheduleInputRequestTypeDef",
+ListVolumeInitiatorsOutputTypeDef = TypedDict(
+    "ListVolumeInitiatorsOutputTypeDef",
     {
-        "VolumeARN": str,
-        "StartAt": int,
-        "RecurrenceInHours": int,
+        "Initiators": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateSnapshotScheduleInputRequestTypeDef",
+
+NotifyWhenUploadedOutputTypeDef = TypedDict(
+    "NotifyWhenUploadedOutputTypeDef",
     {
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
+        "FileShareARN": str,
+        "NotificationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+RefreshCacheOutputTypeDef = TypedDict(
+    "RefreshCacheOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "NotificationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateSnapshotScheduleInputRequestTypeDef(
-    _RequiredUpdateSnapshotScheduleInputRequestTypeDef,
-    _OptionalUpdateSnapshotScheduleInputRequestTypeDef,
-):
-    pass
+RemoveTagsFromResourceOutputTypeDef = TypedDict(
+    "RemoveTagsFromResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResetCacheOutputTypeDef = TypedDict(
+    "ResetCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetrieveTapeArchiveOutputTypeDef = TypedDict(
+    "RetrieveTapeArchiveOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetrieveTapeRecoveryPointOutputTypeDef = TypedDict(
+    "RetrieveTapeRecoveryPointOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetLocalConsolePasswordOutputTypeDef = TypedDict(
+    "SetLocalConsolePasswordOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+SetSMBGuestPasswordOutputTypeDef = TypedDict(
+    "SetSMBGuestPasswordOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ShutdownGatewayOutputTypeDef = TypedDict(
+    "ShutdownGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAvailabilityMonitorTestOutputTypeDef = TypedDict(
+    "StartAvailabilityMonitorTestOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartGatewayOutputTypeDef = TypedDict(
+    "StartGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
+    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBandwidthRateLimitOutputTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChapCredentialsOutputTypeDef = TypedDict(
+    "UpdateChapCredentialsOutputTypeDef",
+    {
+        "TargetARN": str,
+        "InitiatorName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFileSystemAssociationOutputTypeDef = TypedDict(
+    "UpdateFileSystemAssociationOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewayInformationOutputTypeDef = TypedDict(
+    "UpdateGatewayInformationOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "GatewayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "UpdateMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateNFSFileShareOutputTypeDef = TypedDict(
+    "UpdateNFSFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBFileShareOutputTypeDef = TypedDict(
+    "UpdateSMBFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBFileShareVisibilityOutputTypeDef = TypedDict(
+    "UpdateSMBFileShareVisibilityOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBLocalGroupsOutputTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBSecurityStrategyOutputTypeDef = TypedDict(
+    "UpdateSMBSecurityStrategyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSnapshotScheduleOutputTypeDef = TypedDict(
+    "UpdateSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVTLDeviceTypeOutputTypeDef = TypedDict(
+    "UpdateVTLDeviceTypeOutputTypeDef",
+    {
+        "VTLDeviceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateSMBFileShareInputRequestTypeDef = TypedDict(
     "_RequiredCreateSMBFileShareInputRequestTypeDef",
     {
         "ClientToken": str,
         "GatewayARN": str,
         "Role": str,
@@ -2559,27 +2456,22 @@
     },
 )
 
 DescribeBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     {
         "GatewayARN": str,
-        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
-    {
-        "GatewayARN": str,
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BandwidthRateLimitIntervalUnionTypeDef = Union[
+    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
+]
 CachediSCSIVolumeTypeDef = TypedDict(
     "CachediSCSIVolumeTypeDef",
     {
         "VolumeARN": str,
         "VolumeId": str,
         "VolumeType": str,
         "VolumeStatus": str,
@@ -2618,15 +2510,15 @@
     total=False,
 )
 
 DescribeChapCredentialsOutputTypeDef = TypedDict(
     "DescribeChapCredentialsOutputTypeDef",
     {
         "ChapCredentials": List[ChapInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateNFSFileShareInputRequestTypeDef = TypedDict(
     "_RequiredCreateNFSFileShareInputRequestTypeDef",
     {
         "ClientToken": str,
@@ -2751,65 +2643,209 @@
         "HostEnvironment": HostEnvironmentType,
         "EndpointType": str,
         "SoftwareUpdatesEndDate": str,
         "DeprecationDate": str,
         "GatewayCapacity": GatewayCapacityType,
         "SupportedGatewayCapacities": List[GatewayCapacityType],
         "HostEnvironmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSMBSettingsOutputTypeDef = TypedDict(
     "DescribeSMBSettingsOutputTypeDef",
     {
         "GatewayARN": str,
         "DomainName": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "SMBGuestPasswordSet": bool,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
         "FileSharesVisible": bool,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SMBLocalGroups": SMBLocalGroupsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
+DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
+    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     {
         "GatewayARN": str,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
 )
+_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef(
+    _RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+    _OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeTapesInputDescribeTapesPaginateTypeDef(
+    _RequiredDescribeTapesInputDescribeTapesPaginateTypeDef,
+    _OptionalDescribeTapesInputDescribeTapesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    {
+        "VTLDeviceARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef(
+    _RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+    _OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+):
+    pass
+
+
+ListFileSharesInputListFileSharesPaginateTypeDef = TypedDict(
+    "ListFileSharesInputListFileSharesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef = TypedDict(
+    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+ListTapePoolsInputListTapePoolsPaginateTypeDef = TypedDict(
+    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
+    {
+        "PoolARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTapesInputListTapesPaginateTypeDef = TypedDict(
+    "ListTapesInputListTapesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListVolumesInputListVolumesPaginateTypeDef = TypedDict(
+    "ListVolumesInputListVolumesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 DescribeTapeArchivesOutputTypeDef = TypedDict(
     "DescribeTapeArchivesOutputTypeDef",
     {
         "TapeArchives": List[TapeArchiveTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTapeRecoveryPointsOutputTypeDef = TypedDict(
     "DescribeTapeRecoveryPointsOutputTypeDef",
     {
         "GatewayARN": str,
         "TapeRecoveryPointInfos": List[TapeRecoveryPointInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTapesOutputTypeDef = TypedDict(
     "DescribeTapesOutputTypeDef",
     {
         "Tapes": List[TapeTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VTLDeviceTypeDef = TypedDict(
     "VTLDeviceTypeDef",
     {
         "VTLDeviceARN": str,
@@ -2822,150 +2858,170 @@
 )
 
 ListLocalDisksOutputTypeDef = TypedDict(
     "ListLocalDisksOutputTypeDef",
     {
         "GatewayARN": str,
         "Disks": List[DiskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EndpointNetworkConfigurationUnionTypeDef = Union[
+    EndpointNetworkConfigurationTypeDef, EndpointNetworkConfigurationOutputTypeDef
+]
 ListFileSharesOutputTypeDef = TypedDict(
     "ListFileSharesOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileShareInfoList": List[FileShareInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FileSystemAssociationInfoTypeDef = TypedDict(
     "FileSystemAssociationInfoTypeDef",
     {
         "FileSystemAssociationARN": str,
         "LocationARN": str,
         "FileSystemAssociationStatus": str,
         "AuditDestinationARN": str,
         "GatewayARN": str,
         "Tags": List[TagTypeDef],
         "CacheAttributes": CacheAttributesTypeDef,
-        "EndpointNetworkConfiguration": EndpointNetworkConfigurationTypeDef,
+        "EndpointNetworkConfiguration": EndpointNetworkConfigurationOutputTypeDef,
         "FileSystemAssociationStatusDetails": List[FileSystemAssociationStatusDetailTypeDef],
     },
     total=False,
 )
 
 ListFileSystemAssociationsOutputTypeDef = TypedDict(
     "ListFileSystemAssociationsOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileSystemAssociationSummaryList": List[FileSystemAssociationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGatewaysOutputTypeDef = TypedDict(
     "ListGatewaysOutputTypeDef",
     {
         "Gateways": List[GatewayInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTapePoolsOutputTypeDef = TypedDict(
     "ListTapePoolsOutputTypeDef",
     {
         "PoolInfos": List[PoolInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTapesOutputTypeDef = TypedDict(
     "ListTapesOutputTypeDef",
     {
         "TapeInfos": List[TapeInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVolumeRecoveryPointsOutputTypeDef = TypedDict(
     "ListVolumeRecoveryPointsOutputTypeDef",
     {
         "GatewayARN": str,
         "VolumeRecoveryPointInfos": List[VolumeRecoveryPointInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVolumesOutputTypeDef = TypedDict(
     "ListVolumesOutputTypeDef",
     {
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SMBLocalGroupsUnionTypeDef = Union[SMBLocalGroupsTypeDef, SMBLocalGroupsOutputTypeDef]
+UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
 )
 
 DescribeSMBFileSharesOutputTypeDef = TypedDict(
     "DescribeSMBFileSharesOutputTypeDef",
     {
         "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAutomaticTapeCreationPoliciesOutputTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
     },
 )
 
 DescribeCachediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesOutputTypeDef",
     {
         "CachediSCSIVolumes": List[CachediSCSIVolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStorediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeStorediSCSIVolumesOutputTypeDef",
     {
         "StorediSCSIVolumes": List[StorediSCSIVolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNFSFileSharesOutputTypeDef = TypedDict(
     "DescribeNFSFileSharesOutputTypeDef",
     {
         "NFSFileShareInfoList": List[NFSFileShareInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVTLDevicesOutputTypeDef = TypedDict(
     "DescribeVTLDevicesOutputTypeDef",
     {
         "GatewayARN": str,
         "VTLDevices": List[VTLDeviceTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFileSystemAssociationsOutputTypeDef = TypedDict(
     "DescribeFileSystemAssociationsOutputTypeDef",
     {
         "FileSystemAssociationInfoList": List[FileSystemAssociationInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway/type_defs.pyi` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_storagegateway.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ActiveDirectoryStatusType,
     AvailabilityMonitorTestStatusType,
     CaseSensitivityType,
     FileShareTypeType,
     GatewayCapacityType,
@@ -32,231 +32,237 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "ActivateGatewayOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AddCacheInputRequestTypeDef",
-    "AddCacheOutputTypeDef",
-    "AddTagsToResourceOutputTypeDef",
     "AddUploadBufferInputRequestTypeDef",
-    "AddUploadBufferOutputTypeDef",
     "AddWorkingStorageInputRequestTypeDef",
-    "AddWorkingStorageOutputTypeDef",
     "AssignTapePoolInputRequestTypeDef",
-    "AssignTapePoolOutputTypeDef",
     "CacheAttributesTypeDef",
     "EndpointNetworkConfigurationTypeDef",
-    "AssociateFileSystemOutputTypeDef",
     "AttachVolumeInputRequestTypeDef",
-    "AttachVolumeOutputTypeDef",
     "AutomaticTapeCreationRuleTypeDef",
+    "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "VolumeiSCSIAttributesTypeDef",
     "CancelArchivalInputRequestTypeDef",
-    "CancelArchivalOutputTypeDef",
     "CancelRetrievalInputRequestTypeDef",
-    "CancelRetrievalOutputTypeDef",
     "ChapInfoTypeDef",
-    "CreateCachediSCSIVolumeOutputTypeDef",
     "NFSFileShareDefaultsTypeDef",
-    "CreateNFSFileShareOutputTypeDef",
-    "CreateSMBFileShareOutputTypeDef",
-    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
-    "CreateSnapshotOutputTypeDef",
-    "CreateStorediSCSIVolumeOutputTypeDef",
-    "CreateTapePoolOutputTypeDef",
-    "CreateTapeWithBarcodeOutputTypeDef",
-    "CreateTapesOutputTypeDef",
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
-    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
     "DeleteBandwidthRateLimitInputRequestTypeDef",
-    "DeleteBandwidthRateLimitOutputTypeDef",
     "DeleteChapCredentialsInputRequestTypeDef",
-    "DeleteChapCredentialsOutputTypeDef",
     "DeleteFileShareInputRequestTypeDef",
-    "DeleteFileShareOutputTypeDef",
     "DeleteGatewayInputRequestTypeDef",
-    "DeleteGatewayOutputTypeDef",
     "DeleteSnapshotScheduleInputRequestTypeDef",
-    "DeleteSnapshotScheduleOutputTypeDef",
     "DeleteTapeArchiveInputRequestTypeDef",
-    "DeleteTapeArchiveOutputTypeDef",
     "DeleteTapeInputRequestTypeDef",
-    "DeleteTapeOutputTypeDef",
     "DeleteTapePoolInputRequestTypeDef",
-    "DeleteTapePoolOutputTypeDef",
     "DeleteVolumeInputRequestTypeDef",
-    "DeleteVolumeOutputTypeDef",
     "DescribeAvailabilityMonitorTestInputRequestTypeDef",
-    "DescribeAvailabilityMonitorTestOutputTypeDef",
     "DescribeBandwidthRateLimitInputRequestTypeDef",
-    "DescribeBandwidthRateLimitOutputTypeDef",
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCacheInputRequestTypeDef",
-    "DescribeCacheOutputTypeDef",
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     "DescribeChapCredentialsInputRequestTypeDef",
     "DescribeFileSystemAssociationsInputRequestTypeDef",
     "DescribeGatewayInformationInputRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
-    "DescribeMaintenanceStartTimeOutputTypeDef",
     "DescribeNFSFileSharesInputRequestTypeDef",
     "DescribeSMBFileSharesInputRequestTypeDef",
     "DescribeSMBSettingsInputRequestTypeDef",
-    "SMBLocalGroupsTypeDef",
+    "SMBLocalGroupsOutputTypeDef",
     "DescribeSnapshotScheduleInputRequestTypeDef",
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
-    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeTapeArchivesInputRequestTypeDef",
     "TapeArchiveTypeDef",
-    "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
     "DescribeTapeRecoveryPointsInputRequestTypeDef",
     "TapeRecoveryPointInfoTypeDef",
-    "DescribeTapesInputDescribeTapesPaginateTypeDef",
     "DescribeTapesInputRequestTypeDef",
     "TapeTypeDef",
     "DescribeUploadBufferInputRequestTypeDef",
-    "DescribeUploadBufferOutputTypeDef",
-    "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     "DescribeVTLDevicesInputRequestTypeDef",
     "DescribeWorkingStorageInputRequestTypeDef",
-    "DescribeWorkingStorageOutputTypeDef",
     "DetachVolumeInputRequestTypeDef",
-    "DetachVolumeOutputTypeDef",
     "DeviceiSCSIAttributesTypeDef",
     "DisableGatewayInputRequestTypeDef",
-    "DisableGatewayOutputTypeDef",
     "DisassociateFileSystemInputRequestTypeDef",
-    "DisassociateFileSystemOutputTypeDef",
     "DiskTypeDef",
+    "EndpointNetworkConfigurationOutputTypeDef",
     "FileShareInfoTypeDef",
     "FileSystemAssociationStatusDetailTypeDef",
     "FileSystemAssociationSummaryTypeDef",
     "GatewayInfoTypeDef",
     "JoinDomainInputRequestTypeDef",
-    "JoinDomainOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
-    "ListFileSharesInputListFileSharesPaginateTypeDef",
     "ListFileSharesInputRequestTypeDef",
-    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
     "ListFileSystemAssociationsInputRequestTypeDef",
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
     "ListGatewaysInputRequestTypeDef",
     "ListLocalDisksInputRequestTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
     "ListTapePoolsInputRequestTypeDef",
     "PoolInfoTypeDef",
-    "ListTapesInputListTapesPaginateTypeDef",
     "ListTapesInputRequestTypeDef",
     "TapeInfoTypeDef",
     "ListVolumeInitiatorsInputRequestTypeDef",
-    "ListVolumeInitiatorsOutputTypeDef",
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     "VolumeRecoveryPointInfoTypeDef",
-    "ListVolumesInputListVolumesPaginateTypeDef",
     "ListVolumesInputRequestTypeDef",
     "VolumeInfoTypeDef",
     "NotifyWhenUploadedInputRequestTypeDef",
-    "NotifyWhenUploadedOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "RefreshCacheInputRequestTypeDef",
-    "RefreshCacheOutputTypeDef",
     "RemoveTagsFromResourceInputRequestTypeDef",
-    "RemoveTagsFromResourceOutputTypeDef",
     "ResetCacheInputRequestTypeDef",
-    "ResetCacheOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "RetrieveTapeArchiveInputRequestTypeDef",
-    "RetrieveTapeArchiveOutputTypeDef",
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
-    "RetrieveTapeRecoveryPointOutputTypeDef",
+    "SMBLocalGroupsTypeDef",
     "SetLocalConsolePasswordInputRequestTypeDef",
-    "SetLocalConsolePasswordOutputTypeDef",
     "SetSMBGuestPasswordInputRequestTypeDef",
-    "SetSMBGuestPasswordOutputTypeDef",
     "ShutdownGatewayInputRequestTypeDef",
-    "ShutdownGatewayOutputTypeDef",
     "StartAvailabilityMonitorTestInputRequestTypeDef",
-    "StartAvailabilityMonitorTestOutputTypeDef",
     "StartGatewayInputRequestTypeDef",
-    "StartGatewayOutputTypeDef",
-    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
     "UpdateBandwidthRateLimitInputRequestTypeDef",
-    "UpdateBandwidthRateLimitOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
     "UpdateChapCredentialsInputRequestTypeDef",
-    "UpdateChapCredentialsOutputTypeDef",
-    "UpdateFileSystemAssociationOutputTypeDef",
     "UpdateGatewayInformationInputRequestTypeDef",
-    "UpdateGatewayInformationOutputTypeDef",
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
-    "UpdateGatewaySoftwareNowOutputTypeDef",
     "UpdateMaintenanceStartTimeInputRequestTypeDef",
-    "UpdateMaintenanceStartTimeOutputTypeDef",
-    "UpdateNFSFileShareOutputTypeDef",
-    "UpdateSMBFileShareOutputTypeDef",
     "UpdateSMBFileShareVisibilityInputRequestTypeDef",
-    "UpdateSMBFileShareVisibilityOutputTypeDef",
-    "UpdateSMBLocalGroupsOutputTypeDef",
     "UpdateSMBSecurityStrategyInputRequestTypeDef",
-    "UpdateSMBSecurityStrategyOutputTypeDef",
-    "UpdateSnapshotScheduleOutputTypeDef",
     "UpdateVTLDeviceTypeInputRequestTypeDef",
-    "UpdateVTLDeviceTypeOutputTypeDef",
     "ActivateGatewayInputRequestTypeDef",
     "AddTagsToResourceInputRequestTypeDef",
     "CreateCachediSCSIVolumeInputRequestTypeDef",
     "CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef",
     "CreateSnapshotInputRequestTypeDef",
     "CreateStorediSCSIVolumeInputRequestTypeDef",
     "CreateTapePoolInputRequestTypeDef",
     "CreateTapeWithBarcodeInputRequestTypeDef",
     "CreateTapesInputRequestTypeDef",
+    "UpdateSnapshotScheduleInputRequestTypeDef",
+    "ActivateGatewayOutputTypeDef",
+    "AddCacheOutputTypeDef",
+    "AddTagsToResourceOutputTypeDef",
+    "AddUploadBufferOutputTypeDef",
+    "AddWorkingStorageOutputTypeDef",
+    "AssignTapePoolOutputTypeDef",
+    "AssociateFileSystemOutputTypeDef",
+    "AttachVolumeOutputTypeDef",
+    "CancelArchivalOutputTypeDef",
+    "CancelRetrievalOutputTypeDef",
+    "CreateCachediSCSIVolumeOutputTypeDef",
+    "CreateNFSFileShareOutputTypeDef",
+    "CreateSMBFileShareOutputTypeDef",
+    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
+    "CreateSnapshotOutputTypeDef",
+    "CreateStorediSCSIVolumeOutputTypeDef",
+    "CreateTapePoolOutputTypeDef",
+    "CreateTapeWithBarcodeOutputTypeDef",
+    "CreateTapesOutputTypeDef",
+    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
+    "DeleteBandwidthRateLimitOutputTypeDef",
+    "DeleteChapCredentialsOutputTypeDef",
+    "DeleteFileShareOutputTypeDef",
+    "DeleteGatewayOutputTypeDef",
+    "DeleteSnapshotScheduleOutputTypeDef",
+    "DeleteTapeArchiveOutputTypeDef",
+    "DeleteTapeOutputTypeDef",
+    "DeleteTapePoolOutputTypeDef",
+    "DeleteVolumeOutputTypeDef",
+    "DescribeAvailabilityMonitorTestOutputTypeDef",
+    "DescribeBandwidthRateLimitOutputTypeDef",
+    "DescribeCacheOutputTypeDef",
+    "DescribeMaintenanceStartTimeOutputTypeDef",
     "DescribeSnapshotScheduleOutputTypeDef",
+    "DescribeUploadBufferOutputTypeDef",
+    "DescribeWorkingStorageOutputTypeDef",
+    "DetachVolumeOutputTypeDef",
+    "DisableGatewayOutputTypeDef",
+    "DisassociateFileSystemOutputTypeDef",
+    "JoinDomainOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "UpdateSnapshotScheduleInputRequestTypeDef",
+    "ListVolumeInitiatorsOutputTypeDef",
+    "NotifyWhenUploadedOutputTypeDef",
+    "RefreshCacheOutputTypeDef",
+    "RemoveTagsFromResourceOutputTypeDef",
+    "ResetCacheOutputTypeDef",
+    "RetrieveTapeArchiveOutputTypeDef",
+    "RetrieveTapeRecoveryPointOutputTypeDef",
+    "SetLocalConsolePasswordOutputTypeDef",
+    "SetSMBGuestPasswordOutputTypeDef",
+    "ShutdownGatewayOutputTypeDef",
+    "StartAvailabilityMonitorTestOutputTypeDef",
+    "StartGatewayOutputTypeDef",
+    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
+    "UpdateBandwidthRateLimitOutputTypeDef",
+    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
+    "UpdateChapCredentialsOutputTypeDef",
+    "UpdateFileSystemAssociationOutputTypeDef",
+    "UpdateGatewayInformationOutputTypeDef",
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    "UpdateMaintenanceStartTimeOutputTypeDef",
+    "UpdateNFSFileShareOutputTypeDef",
+    "UpdateSMBFileShareOutputTypeDef",
+    "UpdateSMBFileShareVisibilityOutputTypeDef",
+    "UpdateSMBLocalGroupsOutputTypeDef",
+    "UpdateSMBSecurityStrategyOutputTypeDef",
+    "UpdateSnapshotScheduleOutputTypeDef",
+    "UpdateVTLDeviceTypeOutputTypeDef",
     "CreateSMBFileShareInputRequestTypeDef",
     "SMBFileShareInfoTypeDef",
     "UpdateFileSystemAssociationInputRequestTypeDef",
     "UpdateSMBFileShareInputRequestTypeDef",
     "AssociateFileSystemInputRequestTypeDef",
     "AutomaticTapeCreationPolicyInfoTypeDef",
     "UpdateAutomaticTapeCreationPolicyInputRequestTypeDef",
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
+    "BandwidthRateLimitIntervalUnionTypeDef",
     "CachediSCSIVolumeTypeDef",
     "StorediSCSIVolumeTypeDef",
     "DescribeChapCredentialsOutputTypeDef",
     "CreateNFSFileShareInputRequestTypeDef",
     "NFSFileShareInfoTypeDef",
     "UpdateNFSFileShareInputRequestTypeDef",
     "DescribeGatewayInformationOutputTypeDef",
     "DescribeSMBSettingsOutputTypeDef",
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
+    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+    "DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    "DescribeTapesInputDescribeTapesPaginateTypeDef",
+    "DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    "ListFileSharesInputListFileSharesPaginateTypeDef",
+    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
+    "ListTapesInputListTapesPaginateTypeDef",
+    "ListVolumesInputListVolumesPaginateTypeDef",
     "DescribeTapeArchivesOutputTypeDef",
     "DescribeTapeRecoveryPointsOutputTypeDef",
     "DescribeTapesOutputTypeDef",
     "VTLDeviceTypeDef",
     "ListLocalDisksOutputTypeDef",
+    "EndpointNetworkConfigurationUnionTypeDef",
     "ListFileSharesOutputTypeDef",
     "FileSystemAssociationInfoTypeDef",
     "ListFileSystemAssociationsOutputTypeDef",
     "ListGatewaysOutputTypeDef",
     "ListTapePoolsOutputTypeDef",
     "ListTapesOutputTypeDef",
     "ListVolumeRecoveryPointsOutputTypeDef",
     "ListVolumesOutputTypeDef",
+    "SMBLocalGroupsUnionTypeDef",
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
     "DescribeSMBFileSharesOutputTypeDef",
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
     "DescribeCachediSCSIVolumesOutputTypeDef",
     "DescribeStorediSCSIVolumesOutputTypeDef",
     "DescribeNFSFileSharesOutputTypeDef",
     "DescribeVTLDevicesOutputTypeDef",
     "DescribeFileSystemAssociationsOutputTypeDef",
 )
 
@@ -264,78 +270,49 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-ActivateGatewayOutputTypeDef = TypedDict(
-    "ActivateGatewayOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AddCacheInputRequestTypeDef = TypedDict(
     "AddCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
-AddCacheOutputTypeDef = TypedDict(
-    "AddCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AddTagsToResourceOutputTypeDef = TypedDict(
-    "AddTagsToResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddUploadBufferInputRequestTypeDef = TypedDict(
     "AddUploadBufferInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
-AddUploadBufferOutputTypeDef = TypedDict(
-    "AddUploadBufferOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AddWorkingStorageInputRequestTypeDef = TypedDict(
     "AddWorkingStorageInputRequestTypeDef",
     {
         "GatewayARN": str,
         "DiskIds": Sequence[str],
     },
 )
 
-AddWorkingStorageOutputTypeDef = TypedDict(
-    "AddWorkingStorageOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssignTapePoolInputRequestTypeDef = TypedDict(
     "_RequiredAssignTapePoolInputRequestTypeDef",
     {
         "TapeARN": str,
         "PoolId": str,
     },
 )
@@ -348,22 +325,14 @@
 )
 
 class AssignTapePoolInputRequestTypeDef(
     _RequiredAssignTapePoolInputRequestTypeDef, _OptionalAssignTapePoolInputRequestTypeDef
 ):
     pass
 
-AssignTapePoolOutputTypeDef = TypedDict(
-    "AssignTapePoolOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CacheAttributesTypeDef = TypedDict(
     "CacheAttributesTypeDef",
     {
         "CacheStaleTimeoutInSeconds": int,
     },
     total=False,
 )
@@ -372,22 +341,14 @@
     "EndpointNetworkConfigurationTypeDef",
     {
         "IpAddresses": Sequence[str],
     },
     total=False,
 )
 
-AssociateFileSystemOutputTypeDef = TypedDict(
-    "AssociateFileSystemOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAttachVolumeInputRequestTypeDef = TypedDict(
     "_RequiredAttachVolumeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "VolumeARN": str,
         "NetworkInterfaceId": str,
     },
@@ -402,23 +363,14 @@
 )
 
 class AttachVolumeInputRequestTypeDef(
     _RequiredAttachVolumeInputRequestTypeDef, _OptionalAttachVolumeInputRequestTypeDef
 ):
     pass
 
-AttachVolumeOutputTypeDef = TypedDict(
-    "AttachVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "TargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAutomaticTapeCreationRuleTypeDef = TypedDict(
     "_RequiredAutomaticTapeCreationRuleTypeDef",
     {
         "TapeBarcodePrefix": str,
         "PoolId": str,
         "TapeSizeInBytes": int,
         "MinimumNumTapes": int,
@@ -433,22 +385,47 @@
 )
 
 class AutomaticTapeCreationRuleTypeDef(
     _RequiredAutomaticTapeCreationRuleTypeDef, _OptionalAutomaticTapeCreationRuleTypeDef
 ):
     pass
 
+_RequiredBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
+    "_RequiredBandwidthRateLimitIntervalOutputTypeDef",
+    {
+        "StartHourOfDay": int,
+        "StartMinuteOfHour": int,
+        "EndHourOfDay": int,
+        "EndMinuteOfHour": int,
+        "DaysOfWeek": List[int],
+    },
+)
+_OptionalBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
+    "_OptionalBandwidthRateLimitIntervalOutputTypeDef",
+    {
+        "AverageUploadRateLimitInBitsPerSec": int,
+        "AverageDownloadRateLimitInBitsPerSec": int,
+    },
+    total=False,
+)
+
+class BandwidthRateLimitIntervalOutputTypeDef(
+    _RequiredBandwidthRateLimitIntervalOutputTypeDef,
+    _OptionalBandwidthRateLimitIntervalOutputTypeDef,
+):
+    pass
+
 _RequiredBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_RequiredBandwidthRateLimitIntervalTypeDef",
     {
         "StartHourOfDay": int,
         "StartMinuteOfHour": int,
         "EndHourOfDay": int,
         "EndMinuteOfHour": int,
-        "DaysOfWeek": List[int],
+        "DaysOfWeek": Sequence[int],
     },
 )
 _OptionalBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_OptionalBandwidthRateLimitIntervalTypeDef",
     {
         "AverageUploadRateLimitInBitsPerSec": int,
         "AverageDownloadRateLimitInBitsPerSec": int,
@@ -477,186 +454,67 @@
     "CancelArchivalInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
 
-CancelArchivalOutputTypeDef = TypedDict(
-    "CancelArchivalOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CancelRetrievalInputRequestTypeDef = TypedDict(
     "CancelRetrievalInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
 
-CancelRetrievalOutputTypeDef = TypedDict(
-    "CancelRetrievalOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ChapInfoTypeDef = TypedDict(
     "ChapInfoTypeDef",
     {
         "TargetARN": str,
         "SecretToAuthenticateInitiator": str,
         "InitiatorName": str,
         "SecretToAuthenticateTarget": str,
     },
     total=False,
 )
 
-CreateCachediSCSIVolumeOutputTypeDef = TypedDict(
-    "CreateCachediSCSIVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "TargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NFSFileShareDefaultsTypeDef = TypedDict(
     "NFSFileShareDefaultsTypeDef",
     {
         "FileMode": str,
         "DirectoryMode": str,
         "GroupId": int,
         "OwnerId": int,
     },
     total=False,
 )
 
-CreateNFSFileShareOutputTypeDef = TypedDict(
-    "CreateNFSFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSMBFileShareOutputTypeDef = TypedDict(
-    "CreateSMBFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSnapshotFromVolumeRecoveryPointOutputTypeDef = TypedDict(
-    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
-    {
-        "SnapshotId": str,
-        "VolumeARN": str,
-        "VolumeRecoveryPointTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSnapshotOutputTypeDef = TypedDict(
-    "CreateSnapshotOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "SnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStorediSCSIVolumeOutputTypeDef = TypedDict(
-    "CreateStorediSCSIVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "VolumeSizeInBytes": int,
-        "TargetARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTapePoolOutputTypeDef = TypedDict(
-    "CreateTapePoolOutputTypeDef",
-    {
-        "PoolARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTapeWithBarcodeOutputTypeDef = TypedDict(
-    "CreateTapeWithBarcodeOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateTapesOutputTypeDef = TypedDict(
-    "CreateTapesOutputTypeDef",
-    {
-        "TapeARNs": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAutomaticTapeCreationPolicyInputRequestTypeDef = TypedDict(
     "DeleteAutomaticTapeCreationPolicyInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DeleteAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
-    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "DeleteBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
         "BandwidthType": str,
     },
 )
 
-DeleteBandwidthRateLimitOutputTypeDef = TypedDict(
-    "DeleteBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteChapCredentialsInputRequestTypeDef = TypedDict(
     "DeleteChapCredentialsInputRequestTypeDef",
     {
         "TargetARN": str,
         "InitiatorName": str,
     },
 )
 
-DeleteChapCredentialsOutputTypeDef = TypedDict(
-    "DeleteChapCredentialsOutputTypeDef",
-    {
-        "TargetARN": str,
-        "InitiatorName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteFileShareInputRequestTypeDef = TypedDict(
     "_RequiredDeleteFileShareInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalDeleteFileShareInputRequestTypeDef = TypedDict(
@@ -668,52 +526,28 @@
 )
 
 class DeleteFileShareInputRequestTypeDef(
     _RequiredDeleteFileShareInputRequestTypeDef, _OptionalDeleteFileShareInputRequestTypeDef
 ):
     pass
 
-DeleteFileShareOutputTypeDef = TypedDict(
-    "DeleteFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGatewayInputRequestTypeDef = TypedDict(
     "DeleteGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DeleteGatewayOutputTypeDef = TypedDict(
-    "DeleteGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSnapshotScheduleInputRequestTypeDef = TypedDict(
     "DeleteSnapshotScheduleInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
-DeleteSnapshotScheduleOutputTypeDef = TypedDict(
-    "DeleteSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTapeArchiveInputRequestTypeDef = TypedDict(
     "_RequiredDeleteTapeArchiveInputRequestTypeDef",
     {
         "TapeARN": str,
     },
 )
 _OptionalDeleteTapeArchiveInputRequestTypeDef = TypedDict(
@@ -725,22 +559,14 @@
 )
 
 class DeleteTapeArchiveInputRequestTypeDef(
     _RequiredDeleteTapeArchiveInputRequestTypeDef, _OptionalDeleteTapeArchiveInputRequestTypeDef
 ):
     pass
 
-DeleteTapeArchiveOutputTypeDef = TypedDict(
-    "DeleteTapeArchiveOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteTapeInputRequestTypeDef = TypedDict(
     "_RequiredDeleteTapeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "TapeARN": str,
     },
 )
@@ -753,114 +579,56 @@
 )
 
 class DeleteTapeInputRequestTypeDef(
     _RequiredDeleteTapeInputRequestTypeDef, _OptionalDeleteTapeInputRequestTypeDef
 ):
     pass
 
-DeleteTapeOutputTypeDef = TypedDict(
-    "DeleteTapeOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTapePoolInputRequestTypeDef = TypedDict(
     "DeleteTapePoolInputRequestTypeDef",
     {
         "PoolARN": str,
     },
 )
 
-DeleteTapePoolOutputTypeDef = TypedDict(
-    "DeleteTapePoolOutputTypeDef",
-    {
-        "PoolARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVolumeInputRequestTypeDef = TypedDict(
     "DeleteVolumeInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
-DeleteVolumeOutputTypeDef = TypedDict(
-    "DeleteVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeAvailabilityMonitorTestInputRequestTypeDef = TypedDict(
     "DescribeAvailabilityMonitorTestInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeAvailabilityMonitorTestOutputTypeDef = TypedDict(
-    "DescribeAvailabilityMonitorTestOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "Status": AvailabilityMonitorTestStatusType,
-        "StartTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "DescribeBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeBandwidthRateLimitOutputTypeDef = TypedDict(
-    "DescribeBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "AverageUploadRateLimitInBitsPerSec": int,
-        "AverageDownloadRateLimitInBitsPerSec": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
 DescribeCacheInputRequestTypeDef = TypedDict(
     "DescribeCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeCacheOutputTypeDef = TypedDict(
-    "DescribeCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "CacheAllocatedInBytes": int,
-        "CacheUsedPercentage": float,
-        "CacheDirtyPercentage": float,
-        "CacheHitPercentage": float,
-        "CacheMissPercentage": float,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeCachediSCSIVolumesInputRequestTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesInputRequestTypeDef",
     {
         "VolumeARNs": Sequence[str],
     },
 )
 
@@ -898,27 +666,14 @@
 DescribeMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "DescribeMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "DescribeMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "HourOfDay": int,
-        "MinuteOfHour": int,
-        "DayOfWeek": int,
-        "DayOfMonth": int,
-        "Timezone": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeNFSFileSharesInputRequestTypeDef = TypedDict(
     "DescribeNFSFileSharesInputRequestTypeDef",
     {
         "FileShareARNList": Sequence[str],
     },
 )
 
@@ -932,16 +687,16 @@
 DescribeSMBSettingsInputRequestTypeDef = TypedDict(
     "DescribeSMBSettingsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-SMBLocalGroupsTypeDef = TypedDict(
-    "SMBLocalGroupsTypeDef",
+SMBLocalGroupsOutputTypeDef = TypedDict(
+    "SMBLocalGroupsOutputTypeDef",
     {
         "GatewayAdmins": List[str],
     },
     total=False,
 )
 
 DescribeSnapshotScheduleInputRequestTypeDef = TypedDict(
@@ -954,19 +709,20 @@
 DescribeStorediSCSIVolumesInputRequestTypeDef = TypedDict(
     "DescribeStorediSCSIVolumesInputRequestTypeDef",
     {
         "VolumeARNs": Sequence[str],
     },
 )
 
-DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
-    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeTapeArchivesInputRequestTypeDef = TypedDict(
     "DescribeTapeArchivesInputRequestTypeDef",
     {
@@ -993,34 +749,14 @@
         "Worm": bool,
         "RetentionStartDate": datetime,
         "PoolEntryDate": datetime,
     },
     total=False,
 )
 
-_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef(
-    _RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-    _OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeTapeRecoveryPointsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTapeRecoveryPointsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeTapeRecoveryPointsInputRequestTypeDef = TypedDict(
@@ -1045,35 +781,14 @@
         "TapeRecoveryPointTime": datetime,
         "TapeSizeInBytes": int,
         "TapeStatus": str,
     },
     total=False,
 )
 
-_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeTapesInputDescribeTapesPaginateTypeDef(
-    _RequiredDescribeTapesInputDescribeTapesPaginateTypeDef,
-    _OptionalDescribeTapesInputDescribeTapesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeTapesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTapesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeTapesInputRequestTypeDef = TypedDict(
@@ -1114,46 +829,14 @@
 DescribeUploadBufferInputRequestTypeDef = TypedDict(
     "DescribeUploadBufferInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeUploadBufferOutputTypeDef = TypedDict(
-    "DescribeUploadBufferOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "UploadBufferUsedInBytes": int,
-        "UploadBufferAllocatedInBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-    },
-)
-_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
-    {
-        "VTLDeviceARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef(
-    _RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-    _OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeVTLDevicesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVTLDevicesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalDescribeVTLDevicesInputRequestTypeDef = TypedDict(
@@ -1174,25 +857,14 @@
 DescribeWorkingStorageInputRequestTypeDef = TypedDict(
     "DescribeWorkingStorageInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DescribeWorkingStorageOutputTypeDef = TypedDict(
-    "DescribeWorkingStorageOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "DiskIds": List[str],
-        "WorkingStorageUsedInBytes": int,
-        "WorkingStorageAllocatedInBytes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDetachVolumeInputRequestTypeDef = TypedDict(
     "_RequiredDetachVolumeInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 _OptionalDetachVolumeInputRequestTypeDef = TypedDict(
@@ -1204,22 +876,14 @@
 )
 
 class DetachVolumeInputRequestTypeDef(
     _RequiredDetachVolumeInputRequestTypeDef, _OptionalDetachVolumeInputRequestTypeDef
 ):
     pass
 
-DetachVolumeOutputTypeDef = TypedDict(
-    "DetachVolumeOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceiSCSIAttributesTypeDef = TypedDict(
     "DeviceiSCSIAttributesTypeDef",
     {
         "TargetARN": str,
         "NetworkInterfaceId": str,
         "NetworkInterfacePort": int,
         "ChapEnabled": bool,
@@ -1230,22 +894,14 @@
 DisableGatewayInputRequestTypeDef = TypedDict(
     "DisableGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-DisableGatewayOutputTypeDef = TypedDict(
-    "DisableGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisassociateFileSystemInputRequestTypeDef = TypedDict(
     "_RequiredDisassociateFileSystemInputRequestTypeDef",
     {
         "FileSystemAssociationARN": str,
     },
 )
 _OptionalDisassociateFileSystemInputRequestTypeDef = TypedDict(
@@ -1258,22 +914,14 @@
 
 class DisassociateFileSystemInputRequestTypeDef(
     _RequiredDisassociateFileSystemInputRequestTypeDef,
     _OptionalDisassociateFileSystemInputRequestTypeDef,
 ):
     pass
 
-DisassociateFileSystemOutputTypeDef = TypedDict(
-    "DisassociateFileSystemOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DiskTypeDef = TypedDict(
     "DiskTypeDef",
     {
         "DiskId": str,
         "DiskPath": str,
         "DiskNode": str,
         "DiskStatus": str,
@@ -1281,14 +929,22 @@
         "DiskAllocationType": str,
         "DiskAllocationResource": str,
         "DiskAttributeList": List[str],
     },
     total=False,
 )
 
+EndpointNetworkConfigurationOutputTypeDef = TypedDict(
+    "EndpointNetworkConfigurationOutputTypeDef",
+    {
+        "IpAddresses": List[str],
+    },
+    total=False,
+)
+
 FileShareInfoTypeDef = TypedDict(
     "FileShareInfoTypeDef",
     {
         "FileShareType": FileShareTypeType,
         "FileShareARN": str,
         "FileShareId": str,
         "FileShareStatus": str,
@@ -1352,77 +1008,42 @@
 )
 
 class JoinDomainInputRequestTypeDef(
     _RequiredJoinDomainInputRequestTypeDef, _OptionalJoinDomainInputRequestTypeDef
 ):
     pass
 
-JoinDomainOutputTypeDef = TypedDict(
-    "JoinDomainOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ActiveDirectoryStatus": ActiveDirectoryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListAutomaticTapeCreationPoliciesInputRequestTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
     total=False,
 )
 
-ListFileSharesInputListFileSharesPaginateTypeDef = TypedDict(
-    "ListFileSharesInputListFileSharesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFileSharesInputRequestTypeDef = TypedDict(
     "ListFileSharesInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef = TypedDict(
-    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFileSystemAssociationsInputRequestTypeDef = TypedDict(
     "ListFileSystemAssociationsInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Limit": int,
         "Marker": str,
     },
     total=False,
 )
 
-ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGatewaysInputRequestTypeDef = TypedDict(
     "ListGatewaysInputRequestTypeDef",
     {
         "Marker": str,
         "Limit": int,
     },
     total=False,
@@ -1431,34 +1052,14 @@
 ListLocalDisksInputRequestTypeDef = TypedDict(
     "ListLocalDisksInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1471,23 +1072,14 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-ListTapePoolsInputListTapePoolsPaginateTypeDef = TypedDict(
-    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
-    {
-        "PoolARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTapePoolsInputRequestTypeDef = TypedDict(
     "ListTapePoolsInputRequestTypeDef",
     {
         "PoolARNs": Sequence[str],
         "Marker": str,
         "Limit": int,
     },
@@ -1503,23 +1095,14 @@
         "RetentionLockType": RetentionLockTypeType,
         "RetentionLockTimeInDays": int,
         "PoolStatus": PoolStatusType,
     },
     total=False,
 )
 
-ListTapesInputListTapesPaginateTypeDef = TypedDict(
-    "ListTapesInputListTapesPaginateTypeDef",
-    {
-        "TapeARNs": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTapesInputRequestTypeDef = TypedDict(
     "ListTapesInputRequestTypeDef",
     {
         "TapeARNs": Sequence[str],
         "Marker": str,
         "Limit": int,
     },
@@ -1544,22 +1127,14 @@
 ListVolumeInitiatorsInputRequestTypeDef = TypedDict(
     "ListVolumeInitiatorsInputRequestTypeDef",
     {
         "VolumeARN": str,
     },
 )
 
-ListVolumeInitiatorsOutputTypeDef = TypedDict(
-    "ListVolumeInitiatorsOutputTypeDef",
-    {
-        "Initiators": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListVolumeRecoveryPointsInputRequestTypeDef = TypedDict(
     "ListVolumeRecoveryPointsInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
@@ -1570,23 +1145,14 @@
         "VolumeSizeInBytes": int,
         "VolumeUsageInBytes": int,
         "VolumeRecoveryPointTime": str,
     },
     total=False,
 )
 
-ListVolumesInputListVolumesPaginateTypeDef = TypedDict(
-    "ListVolumesInputListVolumesPaginateTypeDef",
-    {
-        "GatewayARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVolumesInputRequestTypeDef = TypedDict(
     "ListVolumesInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Marker": str,
         "Limit": int,
     },
@@ -1610,33 +1176,14 @@
 NotifyWhenUploadedInputRequestTypeDef = TypedDict(
     "NotifyWhenUploadedInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 
-NotifyWhenUploadedOutputTypeDef = TypedDict(
-    "NotifyWhenUploadedOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "NotificationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 _RequiredRefreshCacheInputRequestTypeDef = TypedDict(
     "_RequiredRefreshCacheInputRequestTypeDef",
     {
         "FileShareARN": str,
     },
 )
 _OptionalRefreshCacheInputRequestTypeDef = TypedDict(
@@ -1649,182 +1196,90 @@
 )
 
 class RefreshCacheInputRequestTypeDef(
     _RequiredRefreshCacheInputRequestTypeDef, _OptionalRefreshCacheInputRequestTypeDef
 ):
     pass
 
-RefreshCacheOutputTypeDef = TypedDict(
-    "RefreshCacheOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "NotificationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromResourceInputRequestTypeDef = TypedDict(
     "RemoveTagsFromResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-RemoveTagsFromResourceOutputTypeDef = TypedDict(
-    "RemoveTagsFromResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResetCacheInputRequestTypeDef = TypedDict(
     "ResetCacheInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-ResetCacheOutputTypeDef = TypedDict(
-    "ResetCacheOutputTypeDef",
-    {
-        "GatewayARN": str,
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
 RetrieveTapeArchiveInputRequestTypeDef = TypedDict(
     "RetrieveTapeArchiveInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
-RetrieveTapeArchiveOutputTypeDef = TypedDict(
-    "RetrieveTapeArchiveOutputTypeDef",
-    {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RetrieveTapeRecoveryPointInputRequestTypeDef = TypedDict(
     "RetrieveTapeRecoveryPointInputRequestTypeDef",
     {
         "TapeARN": str,
         "GatewayARN": str,
     },
 )
 
-RetrieveTapeRecoveryPointOutputTypeDef = TypedDict(
-    "RetrieveTapeRecoveryPointOutputTypeDef",
+SMBLocalGroupsTypeDef = TypedDict(
+    "SMBLocalGroupsTypeDef",
     {
-        "TapeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "GatewayAdmins": Sequence[str],
     },
+    total=False,
 )
 
 SetLocalConsolePasswordInputRequestTypeDef = TypedDict(
     "SetLocalConsolePasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "LocalConsolePassword": str,
     },
 )
 
-SetLocalConsolePasswordOutputTypeDef = TypedDict(
-    "SetLocalConsolePasswordOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetSMBGuestPasswordInputRequestTypeDef = TypedDict(
     "SetSMBGuestPasswordInputRequestTypeDef",
     {
         "GatewayARN": str,
         "Password": str,
     },
 )
 
-SetSMBGuestPasswordOutputTypeDef = TypedDict(
-    "SetSMBGuestPasswordOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ShutdownGatewayInputRequestTypeDef = TypedDict(
     "ShutdownGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-ShutdownGatewayOutputTypeDef = TypedDict(
-    "ShutdownGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartAvailabilityMonitorTestInputRequestTypeDef = TypedDict(
     "StartAvailabilityMonitorTestInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-StartAvailabilityMonitorTestOutputTypeDef = TypedDict(
-    "StartAvailabilityMonitorTestOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartGatewayInputRequestTypeDef = TypedDict(
     "StartGatewayInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-StartGatewayOutputTypeDef = TypedDict(
-    "StartGatewayOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
-    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateBandwidthRateLimitInputRequestTypeDef = TypedDict(
     "_RequiredUpdateBandwidthRateLimitInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalUpdateBandwidthRateLimitInputRequestTypeDef = TypedDict(
@@ -1838,30 +1293,14 @@
 
 class UpdateBandwidthRateLimitInputRequestTypeDef(
     _RequiredUpdateBandwidthRateLimitInputRequestTypeDef,
     _OptionalUpdateBandwidthRateLimitInputRequestTypeDef,
 ):
     pass
 
-UpdateBandwidthRateLimitOutputTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChapCredentialsInputRequestTypeDef = TypedDict(
     "_RequiredUpdateChapCredentialsInputRequestTypeDef",
     {
         "TargetARN": str,
         "SecretToAuthenticateInitiator": str,
         "InitiatorName": str,
     },
@@ -1876,31 +1315,14 @@
 
 class UpdateChapCredentialsInputRequestTypeDef(
     _RequiredUpdateChapCredentialsInputRequestTypeDef,
     _OptionalUpdateChapCredentialsInputRequestTypeDef,
 ):
     pass
 
-UpdateChapCredentialsOutputTypeDef = TypedDict(
-    "UpdateChapCredentialsOutputTypeDef",
-    {
-        "TargetARN": str,
-        "InitiatorName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateFileSystemAssociationOutputTypeDef = TypedDict(
-    "UpdateFileSystemAssociationOutputTypeDef",
-    {
-        "FileSystemAssociationARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 _OptionalUpdateGatewayInformationInputRequestTypeDef = TypedDict(
@@ -1916,38 +1338,21 @@
 
 class UpdateGatewayInformationInputRequestTypeDef(
     _RequiredUpdateGatewayInformationInputRequestTypeDef,
     _OptionalUpdateGatewayInformationInputRequestTypeDef,
 ):
     pass
 
-UpdateGatewayInformationOutputTypeDef = TypedDict(
-    "UpdateGatewayInformationOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "GatewayName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateGatewaySoftwareNowInputRequestTypeDef = TypedDict(
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
     {
         "GatewayARN": str,
     },
 )
 
-UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
-    "UpdateGatewaySoftwareNowOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayARN": str,
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
@@ -1963,102 +1368,38 @@
 
 class UpdateMaintenanceStartTimeInputRequestTypeDef(
     _RequiredUpdateMaintenanceStartTimeInputRequestTypeDef,
     _OptionalUpdateMaintenanceStartTimeInputRequestTypeDef,
 ):
     pass
 
-UpdateMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "UpdateMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateNFSFileShareOutputTypeDef = TypedDict(
-    "UpdateNFSFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSMBFileShareOutputTypeDef = TypedDict(
-    "UpdateSMBFileShareOutputTypeDef",
-    {
-        "FileShareARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSMBFileShareVisibilityInputRequestTypeDef = TypedDict(
     "UpdateSMBFileShareVisibilityInputRequestTypeDef",
     {
         "GatewayARN": str,
         "FileSharesVisible": bool,
     },
 )
 
-UpdateSMBFileShareVisibilityOutputTypeDef = TypedDict(
-    "UpdateSMBFileShareVisibilityOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSMBLocalGroupsOutputTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateSMBSecurityStrategyInputRequestTypeDef = TypedDict(
     "UpdateSMBSecurityStrategyInputRequestTypeDef",
     {
         "GatewayARN": str,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
     },
 )
 
-UpdateSMBSecurityStrategyOutputTypeDef = TypedDict(
-    "UpdateSMBSecurityStrategyOutputTypeDef",
-    {
-        "GatewayARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSnapshotScheduleOutputTypeDef = TypedDict(
-    "UpdateSnapshotScheduleOutputTypeDef",
-    {
-        "VolumeARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateVTLDeviceTypeInputRequestTypeDef = TypedDict(
     "UpdateVTLDeviceTypeInputRequestTypeDef",
     {
         "VTLDeviceARN": str,
         "DeviceType": str,
     },
 )
 
-UpdateVTLDeviceTypeOutputTypeDef = TypedDict(
-    "UpdateVTLDeviceTypeOutputTypeDef",
-    {
-        "VTLDeviceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredActivateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredActivateGatewayInputRequestTypeDef",
     {
         "ActivationKey": str,
         "GatewayName": str,
         "GatewayTimezone": str,
         "GatewayRegion": str,
@@ -2255,59 +1596,621 @@
 )
 
 class CreateTapesInputRequestTypeDef(
     _RequiredCreateTapesInputRequestTypeDef, _OptionalCreateTapesInputRequestTypeDef
 ):
     pass
 
+_RequiredUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateSnapshotScheduleInputRequestTypeDef",
+    {
+        "VolumeARN": str,
+        "StartAt": int,
+        "RecurrenceInHours": int,
+    },
+)
+_OptionalUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateSnapshotScheduleInputRequestTypeDef",
+    {
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class UpdateSnapshotScheduleInputRequestTypeDef(
+    _RequiredUpdateSnapshotScheduleInputRequestTypeDef,
+    _OptionalUpdateSnapshotScheduleInputRequestTypeDef,
+):
+    pass
+
+ActivateGatewayOutputTypeDef = TypedDict(
+    "ActivateGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddCacheOutputTypeDef = TypedDict(
+    "AddCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddTagsToResourceOutputTypeDef = TypedDict(
+    "AddTagsToResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddUploadBufferOutputTypeDef = TypedDict(
+    "AddUploadBufferOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddWorkingStorageOutputTypeDef = TypedDict(
+    "AddWorkingStorageOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssignTapePoolOutputTypeDef = TypedDict(
+    "AssignTapePoolOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateFileSystemOutputTypeDef = TypedDict(
+    "AssociateFileSystemOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AttachVolumeOutputTypeDef = TypedDict(
+    "AttachVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "TargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelArchivalOutputTypeDef = TypedDict(
+    "CancelArchivalOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelRetrievalOutputTypeDef = TypedDict(
+    "CancelRetrievalOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCachediSCSIVolumeOutputTypeDef = TypedDict(
+    "CreateCachediSCSIVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "TargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNFSFileShareOutputTypeDef = TypedDict(
+    "CreateNFSFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSMBFileShareOutputTypeDef = TypedDict(
+    "CreateSMBFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotFromVolumeRecoveryPointOutputTypeDef = TypedDict(
+    "CreateSnapshotFromVolumeRecoveryPointOutputTypeDef",
+    {
+        "SnapshotId": str,
+        "VolumeARN": str,
+        "VolumeRecoveryPointTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSnapshotOutputTypeDef = TypedDict(
+    "CreateSnapshotOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "SnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStorediSCSIVolumeOutputTypeDef = TypedDict(
+    "CreateStorediSCSIVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "VolumeSizeInBytes": int,
+        "TargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTapePoolOutputTypeDef = TypedDict(
+    "CreateTapePoolOutputTypeDef",
+    {
+        "PoolARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTapeWithBarcodeOutputTypeDef = TypedDict(
+    "CreateTapeWithBarcodeOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTapesOutputTypeDef = TypedDict(
+    "CreateTapesOutputTypeDef",
+    {
+        "TapeARNs": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
+    "DeleteAutomaticTapeCreationPolicyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteBandwidthRateLimitOutputTypeDef = TypedDict(
+    "DeleteBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteChapCredentialsOutputTypeDef = TypedDict(
+    "DeleteChapCredentialsOutputTypeDef",
+    {
+        "TargetARN": str,
+        "InitiatorName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFileShareOutputTypeDef = TypedDict(
+    "DeleteFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGatewayOutputTypeDef = TypedDict(
+    "DeleteGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSnapshotScheduleOutputTypeDef = TypedDict(
+    "DeleteSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTapeArchiveOutputTypeDef = TypedDict(
+    "DeleteTapeArchiveOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTapeOutputTypeDef = TypedDict(
+    "DeleteTapeOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTapePoolOutputTypeDef = TypedDict(
+    "DeleteTapePoolOutputTypeDef",
+    {
+        "PoolARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVolumeOutputTypeDef = TypedDict(
+    "DeleteVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAvailabilityMonitorTestOutputTypeDef = TypedDict(
+    "DescribeAvailabilityMonitorTestOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "Status": AvailabilityMonitorTestStatusType,
+        "StartTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBandwidthRateLimitOutputTypeDef = TypedDict(
+    "DescribeBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "AverageUploadRateLimitInBitsPerSec": int,
+        "AverageDownloadRateLimitInBitsPerSec": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCacheOutputTypeDef = TypedDict(
+    "DescribeCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "CacheAllocatedInBytes": int,
+        "CacheUsedPercentage": float,
+        "CacheDirtyPercentage": float,
+        "CacheHitPercentage": float,
+        "CacheMissPercentage": float,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "DescribeMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "HourOfDay": int,
+        "MinuteOfHour": int,
+        "DayOfWeek": int,
+        "DayOfMonth": int,
+        "Timezone": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeSnapshotScheduleOutputTypeDef = TypedDict(
     "DescribeSnapshotScheduleOutputTypeDef",
     {
         "VolumeARN": str,
         "StartAt": int,
         "RecurrenceInHours": int,
         "Description": str,
         "Timezone": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUploadBufferOutputTypeDef = TypedDict(
+    "DescribeUploadBufferOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "UploadBufferUsedInBytes": int,
+        "UploadBufferAllocatedInBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorkingStorageOutputTypeDef = TypedDict(
+    "DescribeWorkingStorageOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "DiskIds": List[str],
+        "WorkingStorageUsedInBytes": int,
+        "WorkingStorageAllocatedInBytes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetachVolumeOutputTypeDef = TypedDict(
+    "DetachVolumeOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableGatewayOutputTypeDef = TypedDict(
+    "DisableGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateFileSystemOutputTypeDef = TypedDict(
+    "DisassociateFileSystemOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+JoinDomainOutputTypeDef = TypedDict(
+    "JoinDomainOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ActiveDirectoryStatus": ActiveDirectoryStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "ResourceARN": str,
         "Marker": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateSnapshotScheduleInputRequestTypeDef",
+ListVolumeInitiatorsOutputTypeDef = TypedDict(
+    "ListVolumeInitiatorsOutputTypeDef",
     {
-        "VolumeARN": str,
-        "StartAt": int,
-        "RecurrenceInHours": int,
+        "Initiators": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateSnapshotScheduleInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateSnapshotScheduleInputRequestTypeDef",
+
+NotifyWhenUploadedOutputTypeDef = TypedDict(
+    "NotifyWhenUploadedOutputTypeDef",
     {
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
+        "FileShareARN": str,
+        "NotificationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateSnapshotScheduleInputRequestTypeDef(
-    _RequiredUpdateSnapshotScheduleInputRequestTypeDef,
-    _OptionalUpdateSnapshotScheduleInputRequestTypeDef,
-):
-    pass
+RefreshCacheOutputTypeDef = TypedDict(
+    "RefreshCacheOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "NotificationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveTagsFromResourceOutputTypeDef = TypedDict(
+    "RemoveTagsFromResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResetCacheOutputTypeDef = TypedDict(
+    "ResetCacheOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetrieveTapeArchiveOutputTypeDef = TypedDict(
+    "RetrieveTapeArchiveOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetrieveTapeRecoveryPointOutputTypeDef = TypedDict(
+    "RetrieveTapeRecoveryPointOutputTypeDef",
+    {
+        "TapeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetLocalConsolePasswordOutputTypeDef = TypedDict(
+    "SetLocalConsolePasswordOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetSMBGuestPasswordOutputTypeDef = TypedDict(
+    "SetSMBGuestPasswordOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ShutdownGatewayOutputTypeDef = TypedDict(
+    "ShutdownGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAvailabilityMonitorTestOutputTypeDef = TypedDict(
+    "StartAvailabilityMonitorTestOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartGatewayOutputTypeDef = TypedDict(
+    "StartGatewayOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAutomaticTapeCreationPolicyOutputTypeDef = TypedDict(
+    "UpdateAutomaticTapeCreationPolicyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBandwidthRateLimitOutputTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChapCredentialsOutputTypeDef = TypedDict(
+    "UpdateChapCredentialsOutputTypeDef",
+    {
+        "TargetARN": str,
+        "InitiatorName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFileSystemAssociationOutputTypeDef = TypedDict(
+    "UpdateFileSystemAssociationOutputTypeDef",
+    {
+        "FileSystemAssociationARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewayInformationOutputTypeDef = TypedDict(
+    "UpdateGatewayInformationOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "GatewayName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "UpdateMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateNFSFileShareOutputTypeDef = TypedDict(
+    "UpdateNFSFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBFileShareOutputTypeDef = TypedDict(
+    "UpdateSMBFileShareOutputTypeDef",
+    {
+        "FileShareARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBFileShareVisibilityOutputTypeDef = TypedDict(
+    "UpdateSMBFileShareVisibilityOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBLocalGroupsOutputTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSMBSecurityStrategyOutputTypeDef = TypedDict(
+    "UpdateSMBSecurityStrategyOutputTypeDef",
+    {
+        "GatewayARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSnapshotScheduleOutputTypeDef = TypedDict(
+    "UpdateSnapshotScheduleOutputTypeDef",
+    {
+        "VolumeARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVTLDeviceTypeOutputTypeDef = TypedDict(
+    "UpdateVTLDeviceTypeOutputTypeDef",
+    {
+        "VTLDeviceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateSMBFileShareInputRequestTypeDef = TypedDict(
     "_RequiredCreateSMBFileShareInputRequestTypeDef",
     {
         "ClientToken": str,
         "GatewayARN": str,
         "Role": str,
@@ -2486,27 +2389,22 @@
     },
 )
 
 DescribeBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
     "DescribeBandwidthRateLimitScheduleOutputTypeDef",
     {
         "GatewayARN": str,
-        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
-    {
-        "GatewayARN": str,
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BandwidthRateLimitIntervalUnionTypeDef = Union[
+    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
+]
 CachediSCSIVolumeTypeDef = TypedDict(
     "CachediSCSIVolumeTypeDef",
     {
         "VolumeARN": str,
         "VolumeId": str,
         "VolumeType": str,
         "VolumeStatus": str,
@@ -2545,15 +2443,15 @@
     total=False,
 )
 
 DescribeChapCredentialsOutputTypeDef = TypedDict(
     "DescribeChapCredentialsOutputTypeDef",
     {
         "ChapCredentials": List[ChapInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateNFSFileShareInputRequestTypeDef = TypedDict(
     "_RequiredCreateNFSFileShareInputRequestTypeDef",
     {
         "ClientToken": str,
@@ -2674,65 +2572,201 @@
         "HostEnvironment": HostEnvironmentType,
         "EndpointType": str,
         "SoftwareUpdatesEndDate": str,
         "DeprecationDate": str,
         "GatewayCapacity": GatewayCapacityType,
         "SupportedGatewayCapacities": List[GatewayCapacityType],
         "HostEnvironmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSMBSettingsOutputTypeDef = TypedDict(
     "DescribeSMBSettingsOutputTypeDef",
     {
         "GatewayARN": str,
         "DomainName": str,
         "ActiveDirectoryStatus": ActiveDirectoryStatusType,
         "SMBGuestPasswordSet": bool,
         "SMBSecurityStrategy": SMBSecurityStrategyType,
         "FileSharesVisible": bool,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SMBLocalGroups": SMBLocalGroupsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
-    "UpdateSMBLocalGroupsInputRequestTypeDef",
+DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef = TypedDict(
+    "DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef(
+    _RequiredDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+    _OptionalDescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTapesInputDescribeTapesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+    },
+)
+_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTapesInputDescribeTapesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeTapesInputDescribeTapesPaginateTypeDef(
+    _RequiredDescribeTapesInputDescribeTapesPaginateTypeDef,
+    _OptionalDescribeTapesInputDescribeTapesPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
     {
         "GatewayARN": str,
-        "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
 )
+_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef",
+    {
+        "VTLDeviceARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef(
+    _RequiredDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+    _OptionalDescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+):
+    pass
+
+ListFileSharesInputListFileSharesPaginateTypeDef = TypedDict(
+    "ListFileSharesInputListFileSharesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef = TypedDict(
+    "ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+ListTapePoolsInputListTapePoolsPaginateTypeDef = TypedDict(
+    "ListTapePoolsInputListTapePoolsPaginateTypeDef",
+    {
+        "PoolARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTapesInputListTapesPaginateTypeDef = TypedDict(
+    "ListTapesInputListTapesPaginateTypeDef",
+    {
+        "TapeARNs": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListVolumesInputListVolumesPaginateTypeDef = TypedDict(
+    "ListVolumesInputListVolumesPaginateTypeDef",
+    {
+        "GatewayARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 DescribeTapeArchivesOutputTypeDef = TypedDict(
     "DescribeTapeArchivesOutputTypeDef",
     {
         "TapeArchives": List[TapeArchiveTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTapeRecoveryPointsOutputTypeDef = TypedDict(
     "DescribeTapeRecoveryPointsOutputTypeDef",
     {
         "GatewayARN": str,
         "TapeRecoveryPointInfos": List[TapeRecoveryPointInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTapesOutputTypeDef = TypedDict(
     "DescribeTapesOutputTypeDef",
     {
         "Tapes": List[TapeTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VTLDeviceTypeDef = TypedDict(
     "VTLDeviceTypeDef",
     {
         "VTLDeviceARN": str,
@@ -2745,150 +2779,170 @@
 )
 
 ListLocalDisksOutputTypeDef = TypedDict(
     "ListLocalDisksOutputTypeDef",
     {
         "GatewayARN": str,
         "Disks": List[DiskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EndpointNetworkConfigurationUnionTypeDef = Union[
+    EndpointNetworkConfigurationTypeDef, EndpointNetworkConfigurationOutputTypeDef
+]
 ListFileSharesOutputTypeDef = TypedDict(
     "ListFileSharesOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileShareInfoList": List[FileShareInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FileSystemAssociationInfoTypeDef = TypedDict(
     "FileSystemAssociationInfoTypeDef",
     {
         "FileSystemAssociationARN": str,
         "LocationARN": str,
         "FileSystemAssociationStatus": str,
         "AuditDestinationARN": str,
         "GatewayARN": str,
         "Tags": List[TagTypeDef],
         "CacheAttributes": CacheAttributesTypeDef,
-        "EndpointNetworkConfiguration": EndpointNetworkConfigurationTypeDef,
+        "EndpointNetworkConfiguration": EndpointNetworkConfigurationOutputTypeDef,
         "FileSystemAssociationStatusDetails": List[FileSystemAssociationStatusDetailTypeDef],
     },
     total=False,
 )
 
 ListFileSystemAssociationsOutputTypeDef = TypedDict(
     "ListFileSystemAssociationsOutputTypeDef",
     {
         "Marker": str,
         "NextMarker": str,
         "FileSystemAssociationSummaryList": List[FileSystemAssociationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGatewaysOutputTypeDef = TypedDict(
     "ListGatewaysOutputTypeDef",
     {
         "Gateways": List[GatewayInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTapePoolsOutputTypeDef = TypedDict(
     "ListTapePoolsOutputTypeDef",
     {
         "PoolInfos": List[PoolInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTapesOutputTypeDef = TypedDict(
     "ListTapesOutputTypeDef",
     {
         "TapeInfos": List[TapeInfoTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVolumeRecoveryPointsOutputTypeDef = TypedDict(
     "ListVolumeRecoveryPointsOutputTypeDef",
     {
         "GatewayARN": str,
         "VolumeRecoveryPointInfos": List[VolumeRecoveryPointInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVolumesOutputTypeDef = TypedDict(
     "ListVolumesOutputTypeDef",
     {
         "GatewayARN": str,
         "Marker": str,
         "VolumeInfos": List[VolumeInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SMBLocalGroupsUnionTypeDef = Union[SMBLocalGroupsTypeDef, SMBLocalGroupsOutputTypeDef]
+UpdateSMBLocalGroupsInputRequestTypeDef = TypedDict(
+    "UpdateSMBLocalGroupsInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "SMBLocalGroups": SMBLocalGroupsTypeDef,
     },
 )
 
 DescribeSMBFileSharesOutputTypeDef = TypedDict(
     "DescribeSMBFileSharesOutputTypeDef",
     {
         "SMBFileShareInfoList": List[SMBFileShareInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAutomaticTapeCreationPoliciesOutputTypeDef = TypedDict(
     "ListAutomaticTapeCreationPoliciesOutputTypeDef",
     {
         "AutomaticTapeCreationPolicyInfos": List[AutomaticTapeCreationPolicyInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "UpdateBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "GatewayARN": str,
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
     },
 )
 
 DescribeCachediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeCachediSCSIVolumesOutputTypeDef",
     {
         "CachediSCSIVolumes": List[CachediSCSIVolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStorediSCSIVolumesOutputTypeDef = TypedDict(
     "DescribeStorediSCSIVolumesOutputTypeDef",
     {
         "StorediSCSIVolumes": List[StorediSCSIVolumeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNFSFileSharesOutputTypeDef = TypedDict(
     "DescribeNFSFileSharesOutputTypeDef",
     {
         "NFSFileShareInfoList": List[NFSFileShareInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVTLDevicesOutputTypeDef = TypedDict(
     "DescribeVTLDevicesOutputTypeDef",
     {
         "GatewayARN": str,
         "VTLDevices": List[VTLDeviceTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFileSystemAssociationsOutputTypeDef = TypedDict(
     "DescribeFileSystemAssociationsOutputTypeDef",
     {
         "FileSystemAssociationInfoList": List[FileSystemAssociationInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway.egg-info/PKG-INFO` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-storagegateway
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.StorageGateway 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.StorageGateway 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore storagegateway type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore storagegateway type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-storagegateway"></a>
 
 # types-aiobotocore-storagegateway
 
 [![PyPI - types-aiobotocore-storagegateway](https://img.shields.io/pypi/v/types-aiobotocore-storagegateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-storagegateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-storagegateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-storagegateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-storagegateway?color=blue)](https://pypistats.org/packages/types-aiobotocore-storagegateway)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-storagegateway)](https://pepy.tech/project/types-aiobotocore-storagegateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.StorageGateway 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
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
 [types-aiobotocore-storagegateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_storagegateway/).
 
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
@@ -358,250 +357,256 @@
 )
 
 
 def check_value(value: ActiveDirectoryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_storagegateway.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_storagegateway.type_defs import (
     TagTypeDef,
-    ActivateGatewayOutputTypeDef,
+    ResponseMetadataTypeDef,
     AddCacheInputRequestTypeDef,
-    AddCacheOutputTypeDef,
-    AddTagsToResourceOutputTypeDef,
     AddUploadBufferInputRequestTypeDef,
-    AddUploadBufferOutputTypeDef,
     AddWorkingStorageInputRequestTypeDef,
-    AddWorkingStorageOutputTypeDef,
     AssignTapePoolInputRequestTypeDef,
-    AssignTapePoolOutputTypeDef,
     CacheAttributesTypeDef,
     EndpointNetworkConfigurationTypeDef,
-    AssociateFileSystemOutputTypeDef,
     AttachVolumeInputRequestTypeDef,
-    AttachVolumeOutputTypeDef,
     AutomaticTapeCreationRuleTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     VolumeiSCSIAttributesTypeDef,
     CancelArchivalInputRequestTypeDef,
-    CancelArchivalOutputTypeDef,
     CancelRetrievalInputRequestTypeDef,
-    CancelRetrievalOutputTypeDef,
     ChapInfoTypeDef,
-    CreateCachediSCSIVolumeOutputTypeDef,
     NFSFileShareDefaultsTypeDef,
-    CreateNFSFileShareOutputTypeDef,
-    CreateSMBFileShareOutputTypeDef,
-    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
-    CreateSnapshotOutputTypeDef,
-    CreateStorediSCSIVolumeOutputTypeDef,
-    CreateTapePoolOutputTypeDef,
-    CreateTapeWithBarcodeOutputTypeDef,
-    CreateTapesOutputTypeDef,
     DeleteAutomaticTapeCreationPolicyInputRequestTypeDef,
-    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
     DeleteBandwidthRateLimitInputRequestTypeDef,
-    DeleteBandwidthRateLimitOutputTypeDef,
     DeleteChapCredentialsInputRequestTypeDef,
-    DeleteChapCredentialsOutputTypeDef,
     DeleteFileShareInputRequestTypeDef,
-    DeleteFileShareOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
-    DeleteGatewayOutputTypeDef,
     DeleteSnapshotScheduleInputRequestTypeDef,
-    DeleteSnapshotScheduleOutputTypeDef,
     DeleteTapeArchiveInputRequestTypeDef,
-    DeleteTapeArchiveOutputTypeDef,
     DeleteTapeInputRequestTypeDef,
-    DeleteTapeOutputTypeDef,
     DeleteTapePoolInputRequestTypeDef,
-    DeleteTapePoolOutputTypeDef,
     DeleteVolumeInputRequestTypeDef,
-    DeleteVolumeOutputTypeDef,
     DescribeAvailabilityMonitorTestInputRequestTypeDef,
-    DescribeAvailabilityMonitorTestOutputTypeDef,
     DescribeBandwidthRateLimitInputRequestTypeDef,
-    DescribeBandwidthRateLimitOutputTypeDef,
     DescribeBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCacheInputRequestTypeDef,
-    DescribeCacheOutputTypeDef,
     DescribeCachediSCSIVolumesInputRequestTypeDef,
     DescribeChapCredentialsInputRequestTypeDef,
     DescribeFileSystemAssociationsInputRequestTypeDef,
     DescribeGatewayInformationInputRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeMaintenanceStartTimeInputRequestTypeDef,
-    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeNFSFileSharesInputRequestTypeDef,
     DescribeSMBFileSharesInputRequestTypeDef,
     DescribeSMBSettingsInputRequestTypeDef,
-    SMBLocalGroupsTypeDef,
+    SMBLocalGroupsOutputTypeDef,
     DescribeSnapshotScheduleInputRequestTypeDef,
     DescribeStorediSCSIVolumesInputRequestTypeDef,
-    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeTapeArchivesInputRequestTypeDef,
     TapeArchiveTypeDef,
-    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
     DescribeTapeRecoveryPointsInputRequestTypeDef,
     TapeRecoveryPointInfoTypeDef,
-    DescribeTapesInputDescribeTapesPaginateTypeDef,
     DescribeTapesInputRequestTypeDef,
     TapeTypeDef,
     DescribeUploadBufferInputRequestTypeDef,
-    DescribeUploadBufferOutputTypeDef,
-    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
     DescribeVTLDevicesInputRequestTypeDef,
     DescribeWorkingStorageInputRequestTypeDef,
-    DescribeWorkingStorageOutputTypeDef,
     DetachVolumeInputRequestTypeDef,
-    DetachVolumeOutputTypeDef,
     DeviceiSCSIAttributesTypeDef,
     DisableGatewayInputRequestTypeDef,
-    DisableGatewayOutputTypeDef,
     DisassociateFileSystemInputRequestTypeDef,
-    DisassociateFileSystemOutputTypeDef,
     DiskTypeDef,
+    EndpointNetworkConfigurationOutputTypeDef,
     FileShareInfoTypeDef,
     FileSystemAssociationStatusDetailTypeDef,
     FileSystemAssociationSummaryTypeDef,
     GatewayInfoTypeDef,
     JoinDomainInputRequestTypeDef,
-    JoinDomainOutputTypeDef,
     ListAutomaticTapeCreationPoliciesInputRequestTypeDef,
-    ListFileSharesInputListFileSharesPaginateTypeDef,
     ListFileSharesInputRequestTypeDef,
-    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
     ListFileSystemAssociationsInputRequestTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
     ListGatewaysInputRequestTypeDef,
     ListLocalDisksInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTapePoolsInputListTapePoolsPaginateTypeDef,
     ListTapePoolsInputRequestTypeDef,
     PoolInfoTypeDef,
-    ListTapesInputListTapesPaginateTypeDef,
     ListTapesInputRequestTypeDef,
     TapeInfoTypeDef,
     ListVolumeInitiatorsInputRequestTypeDef,
-    ListVolumeInitiatorsOutputTypeDef,
     ListVolumeRecoveryPointsInputRequestTypeDef,
     VolumeRecoveryPointInfoTypeDef,
-    ListVolumesInputListVolumesPaginateTypeDef,
     ListVolumesInputRequestTypeDef,
     VolumeInfoTypeDef,
     NotifyWhenUploadedInputRequestTypeDef,
-    NotifyWhenUploadedOutputTypeDef,
-    PaginatorConfigTypeDef,
     RefreshCacheInputRequestTypeDef,
-    RefreshCacheOutputTypeDef,
     RemoveTagsFromResourceInputRequestTypeDef,
-    RemoveTagsFromResourceOutputTypeDef,
     ResetCacheInputRequestTypeDef,
-    ResetCacheOutputTypeDef,
-    ResponseMetadataTypeDef,
     RetrieveTapeArchiveInputRequestTypeDef,
-    RetrieveTapeArchiveOutputTypeDef,
     RetrieveTapeRecoveryPointInputRequestTypeDef,
-    RetrieveTapeRecoveryPointOutputTypeDef,
+    SMBLocalGroupsTypeDef,
     SetLocalConsolePasswordInputRequestTypeDef,
-    SetLocalConsolePasswordOutputTypeDef,
     SetSMBGuestPasswordInputRequestTypeDef,
-    SetSMBGuestPasswordOutputTypeDef,
     ShutdownGatewayInputRequestTypeDef,
-    ShutdownGatewayOutputTypeDef,
     StartAvailabilityMonitorTestInputRequestTypeDef,
-    StartAvailabilityMonitorTestOutputTypeDef,
     StartGatewayInputRequestTypeDef,
-    StartGatewayOutputTypeDef,
-    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
     UpdateBandwidthRateLimitInputRequestTypeDef,
-    UpdateBandwidthRateLimitOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleOutputTypeDef,
     UpdateChapCredentialsInputRequestTypeDef,
-    UpdateChapCredentialsOutputTypeDef,
-    UpdateFileSystemAssociationOutputTypeDef,
     UpdateGatewayInformationInputRequestTypeDef,
-    UpdateGatewayInformationOutputTypeDef,
     UpdateGatewaySoftwareNowInputRequestTypeDef,
-    UpdateGatewaySoftwareNowOutputTypeDef,
     UpdateMaintenanceStartTimeInputRequestTypeDef,
-    UpdateMaintenanceStartTimeOutputTypeDef,
-    UpdateNFSFileShareOutputTypeDef,
-    UpdateSMBFileShareOutputTypeDef,
     UpdateSMBFileShareVisibilityInputRequestTypeDef,
-    UpdateSMBFileShareVisibilityOutputTypeDef,
-    UpdateSMBLocalGroupsOutputTypeDef,
     UpdateSMBSecurityStrategyInputRequestTypeDef,
-    UpdateSMBSecurityStrategyOutputTypeDef,
-    UpdateSnapshotScheduleOutputTypeDef,
     UpdateVTLDeviceTypeInputRequestTypeDef,
-    UpdateVTLDeviceTypeOutputTypeDef,
     ActivateGatewayInputRequestTypeDef,
     AddTagsToResourceInputRequestTypeDef,
     CreateCachediSCSIVolumeInputRequestTypeDef,
     CreateSnapshotFromVolumeRecoveryPointInputRequestTypeDef,
     CreateSnapshotInputRequestTypeDef,
     CreateStorediSCSIVolumeInputRequestTypeDef,
     CreateTapePoolInputRequestTypeDef,
     CreateTapeWithBarcodeInputRequestTypeDef,
     CreateTapesInputRequestTypeDef,
+    UpdateSnapshotScheduleInputRequestTypeDef,
+    ActivateGatewayOutputTypeDef,
+    AddCacheOutputTypeDef,
+    AddTagsToResourceOutputTypeDef,
+    AddUploadBufferOutputTypeDef,
+    AddWorkingStorageOutputTypeDef,
+    AssignTapePoolOutputTypeDef,
+    AssociateFileSystemOutputTypeDef,
+    AttachVolumeOutputTypeDef,
+    CancelArchivalOutputTypeDef,
+    CancelRetrievalOutputTypeDef,
+    CreateCachediSCSIVolumeOutputTypeDef,
+    CreateNFSFileShareOutputTypeDef,
+    CreateSMBFileShareOutputTypeDef,
+    CreateSnapshotFromVolumeRecoveryPointOutputTypeDef,
+    CreateSnapshotOutputTypeDef,
+    CreateStorediSCSIVolumeOutputTypeDef,
+    CreateTapePoolOutputTypeDef,
+    CreateTapeWithBarcodeOutputTypeDef,
+    CreateTapesOutputTypeDef,
+    DeleteAutomaticTapeCreationPolicyOutputTypeDef,
+    DeleteBandwidthRateLimitOutputTypeDef,
+    DeleteChapCredentialsOutputTypeDef,
+    DeleteFileShareOutputTypeDef,
+    DeleteGatewayOutputTypeDef,
+    DeleteSnapshotScheduleOutputTypeDef,
+    DeleteTapeArchiveOutputTypeDef,
+    DeleteTapeOutputTypeDef,
+    DeleteTapePoolOutputTypeDef,
+    DeleteVolumeOutputTypeDef,
+    DescribeAvailabilityMonitorTestOutputTypeDef,
+    DescribeBandwidthRateLimitOutputTypeDef,
+    DescribeCacheOutputTypeDef,
+    DescribeMaintenanceStartTimeOutputTypeDef,
     DescribeSnapshotScheduleOutputTypeDef,
+    DescribeUploadBufferOutputTypeDef,
+    DescribeWorkingStorageOutputTypeDef,
+    DetachVolumeOutputTypeDef,
+    DisableGatewayOutputTypeDef,
+    DisassociateFileSystemOutputTypeDef,
+    JoinDomainOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    UpdateSnapshotScheduleInputRequestTypeDef,
+    ListVolumeInitiatorsOutputTypeDef,
+    NotifyWhenUploadedOutputTypeDef,
+    RefreshCacheOutputTypeDef,
+    RemoveTagsFromResourceOutputTypeDef,
+    ResetCacheOutputTypeDef,
+    RetrieveTapeArchiveOutputTypeDef,
+    RetrieveTapeRecoveryPointOutputTypeDef,
+    SetLocalConsolePasswordOutputTypeDef,
+    SetSMBGuestPasswordOutputTypeDef,
+    ShutdownGatewayOutputTypeDef,
+    StartAvailabilityMonitorTestOutputTypeDef,
+    StartGatewayOutputTypeDef,
+    UpdateAutomaticTapeCreationPolicyOutputTypeDef,
+    UpdateBandwidthRateLimitOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleOutputTypeDef,
+    UpdateChapCredentialsOutputTypeDef,
+    UpdateFileSystemAssociationOutputTypeDef,
+    UpdateGatewayInformationOutputTypeDef,
+    UpdateGatewaySoftwareNowOutputTypeDef,
+    UpdateMaintenanceStartTimeOutputTypeDef,
+    UpdateNFSFileShareOutputTypeDef,
+    UpdateSMBFileShareOutputTypeDef,
+    UpdateSMBFileShareVisibilityOutputTypeDef,
+    UpdateSMBLocalGroupsOutputTypeDef,
+    UpdateSMBSecurityStrategyOutputTypeDef,
+    UpdateSnapshotScheduleOutputTypeDef,
+    UpdateVTLDeviceTypeOutputTypeDef,
     CreateSMBFileShareInputRequestTypeDef,
     SMBFileShareInfoTypeDef,
     UpdateFileSystemAssociationInputRequestTypeDef,
     UpdateSMBFileShareInputRequestTypeDef,
     AssociateFileSystemInputRequestTypeDef,
     AutomaticTapeCreationPolicyInfoTypeDef,
     UpdateAutomaticTapeCreationPolicyInputRequestTypeDef,
     DescribeBandwidthRateLimitScheduleOutputTypeDef,
-    UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CachediSCSIVolumeTypeDef,
     StorediSCSIVolumeTypeDef,
     DescribeChapCredentialsOutputTypeDef,
     CreateNFSFileShareInputRequestTypeDef,
     NFSFileShareInfoTypeDef,
     UpdateNFSFileShareInputRequestTypeDef,
     DescribeGatewayInformationOutputTypeDef,
     DescribeSMBSettingsOutputTypeDef,
-    UpdateSMBLocalGroupsInputRequestTypeDef,
+    DescribeTapeArchivesInputDescribeTapeArchivesPaginateTypeDef,
+    DescribeTapeRecoveryPointsInputDescribeTapeRecoveryPointsPaginateTypeDef,
+    DescribeTapesInputDescribeTapesPaginateTypeDef,
+    DescribeVTLDevicesInputDescribeVTLDevicesPaginateTypeDef,
+    ListFileSharesInputListFileSharesPaginateTypeDef,
+    ListFileSystemAssociationsInputListFileSystemAssociationsPaginateTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListTapePoolsInputListTapePoolsPaginateTypeDef,
+    ListTapesInputListTapesPaginateTypeDef,
+    ListVolumesInputListVolumesPaginateTypeDef,
     DescribeTapeArchivesOutputTypeDef,
     DescribeTapeRecoveryPointsOutputTypeDef,
     DescribeTapesOutputTypeDef,
     VTLDeviceTypeDef,
     ListLocalDisksOutputTypeDef,
+    EndpointNetworkConfigurationUnionTypeDef,
     ListFileSharesOutputTypeDef,
     FileSystemAssociationInfoTypeDef,
     ListFileSystemAssociationsOutputTypeDef,
     ListGatewaysOutputTypeDef,
     ListTapePoolsOutputTypeDef,
     ListTapesOutputTypeDef,
     ListVolumeRecoveryPointsOutputTypeDef,
     ListVolumesOutputTypeDef,
+    SMBLocalGroupsUnionTypeDef,
+    UpdateSMBLocalGroupsInputRequestTypeDef,
     DescribeSMBFileSharesOutputTypeDef,
     ListAutomaticTapeCreationPoliciesOutputTypeDef,
+    UpdateBandwidthRateLimitScheduleInputRequestTypeDef,
     DescribeCachediSCSIVolumesOutputTypeDef,
     DescribeStorediSCSIVolumesOutputTypeDef,
     DescribeNFSFileSharesOutputTypeDef,
     DescribeVTLDevicesOutputTypeDef,
     DescribeFileSystemAssociationsOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-storagegateway-2.5.2/types_aiobotocore_storagegateway.egg-info/SOURCES.txt` & `types-aiobotocore-storagegateway-2.5.2.post1/types_aiobotocore_storagegateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*


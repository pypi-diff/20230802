# Comparing `tmp/types-aiobotocore-backup-gateway-2.5.2.tar.gz` & `tmp/types-aiobotocore-backup-gateway-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-backup-gateway-2.5.2.tar", last modified: Sat Jul  8 01:43:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-backup-gateway-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
```

## Comparing `types-aiobotocore-backup-gateway-2.5.2.tar` & `types-aiobotocore-backup-gateway-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.909738 types-aiobotocore-backup-gateway-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:17.000000 types-aiobotocore-backup-gateway-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-08 01:43:16.909738 types-aiobotocore-backup-gateway-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14639 2023-07-08 01:26:17.000000 types-aiobotocore-backup-gateway-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:16.909738 types-aiobotocore-backup-gateway-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-08 01:26:17.000000 types-aiobotocore-backup-gateway-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.905738 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-08 01:26:17.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-08 01:26:17.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-08 01:26:17.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21669 2023-07-08 01:26:18.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21632 2023-07-08 01:26:17.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-07-08 01:26:18.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-07-08 01:26:18.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-08 01:26:18.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-08 01:26:18.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:17.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19710 2023-07-08 01:26:19.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19693 2023-07-08 01:26:18.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:17.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.909738 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-07-08 01:43:16.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:43:16.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:16.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:43:16.000000 types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.285648 types-aiobotocore-backup-gateway-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-08-02 14:51:55.281648 types-aiobotocore-backup-gateway-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14711 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.285648 types-aiobotocore-backup-gateway-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.273648 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21679 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21642 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8673 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20562 2023-08-02 14:33:46.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20543 2023-08-02 14:33:45.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:44.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.281648 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16256 2023-08-02 14:51:55.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:51:55.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:55.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:51:55.000000 types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2/LICENSE` & `types-aiobotocore-backup-gateway-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2/PKG-INFO` & `types-aiobotocore-backup-gateway-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backup-gateway
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.BackupGateway 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.BackupGateway 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore backup-gateway type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore backup-gateway type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-backup-gateway"></a>
 
 # types-aiobotocore-backup-gateway
 
 [![PyPI - types-aiobotocore-backup-gateway](https://img.shields.io/pypi/v/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-backup-gateway?color=blue)](https://pypistats.org/packages/types-aiobotocore-backup-gateway)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup-gateway)](https://pepy.tech/project/types-aiobotocore-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.BackupGateway 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
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
 [types-aiobotocore-backup-gateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/).
 
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
@@ -318,92 +317,94 @@
 )
 
 
 def check_value(value: GatewayTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_backup_gateway.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_backup_gateway.type_defs import (
     AssociateGatewayToServerInputRequestTypeDef,
-    AssociateGatewayToServerOutputTypeDef,
+    ResponseMetadataTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     TagTypeDef,
-    CreateGatewayOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
-    DeleteGatewayOutputTypeDef,
     DeleteHypervisorInputRequestTypeDef,
-    DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerInputRequestTypeDef,
-    DisassociateGatewayFromServerOutputTypeDef,
     MaintenanceStartTimeTypeDef,
     GatewayTypeDef,
     GetBandwidthRateLimitScheduleInputRequestTypeDef,
     GetGatewayInputRequestTypeDef,
     GetHypervisorInputRequestTypeDef,
     HypervisorDetailsTypeDef,
     GetHypervisorPropertyMappingsInputRequestTypeDef,
     VmwareToAwsTagMappingTypeDef,
     GetVirtualMachineInputRequestTypeDef,
     HypervisorTypeDef,
-    ImportHypervisorConfigurationOutputTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListGatewaysInputRequestTypeDef,
-    ListHypervisorsInputListHypervisorsPaginateTypeDef,
     ListHypervisorsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesInputRequestTypeDef,
     VirtualMachineTypeDef,
-    PaginatorConfigTypeDef,
+    PutMaintenanceStartTimeInputRequestTypeDef,
+    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
+    TestHypervisorConfigurationInputRequestTypeDef,
+    UntagResourceInputRequestTypeDef,
+    UpdateGatewayInformationInputRequestTypeDef,
+    UpdateGatewaySoftwareNowInputRequestTypeDef,
+    UpdateHypervisorInputRequestTypeDef,
+    VmwareTagTypeDef,
+    AssociateGatewayToServerOutputTypeDef,
+    CreateGatewayOutputTypeDef,
+    DeleteGatewayOutputTypeDef,
+    DeleteHypervisorOutputTypeDef,
+    DisassociateGatewayFromServerOutputTypeDef,
+    ImportHypervisorConfigurationOutputTypeDef,
     PutBandwidthRateLimitScheduleOutputTypeDef,
     PutHypervisorPropertyMappingsOutputTypeDef,
-    PutMaintenanceStartTimeInputRequestTypeDef,
     PutMaintenanceStartTimeOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
     StartVirtualMachinesMetadataSyncOutputTypeDef,
     TagResourceOutputTypeDef,
-    TestHypervisorConfigurationInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
     UntagResourceOutputTypeDef,
-    UpdateGatewayInformationInputRequestTypeDef,
     UpdateGatewayInformationOutputTypeDef,
-    UpdateGatewaySoftwareNowInputRequestTypeDef,
     UpdateGatewaySoftwareNowOutputTypeDef,
-    UpdateHypervisorInputRequestTypeDef,
     UpdateHypervisorOutputTypeDef,
-    VmwareTagTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
-    PutBandwidthRateLimitScheduleInputRequestTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CreateGatewayInputRequestTypeDef,
     ImportHypervisorConfigurationInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     GatewayDetailsTypeDef,
     ListGatewaysOutputTypeDef,
     GetHypervisorOutputTypeDef,
     GetHypervisorPropertyMappingsOutputTypeDef,
     PutHypervisorPropertyMappingsInputRequestTypeDef,
     ListHypervisorsOutputTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
+    ListHypervisorsInputListHypervisorsPaginateTypeDef,
+    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesOutputTypeDef,
     VirtualMachineDetailsTypeDef,
+    PutBandwidthRateLimitScheduleInputRequestTypeDef,
     GetGatewayOutputTypeDef,
     GetVirtualMachineOutputTypeDef,
 )
 
 
-def get_structure() -> AssociateGatewayToServerInputRequestTypeDef:
+def get_value() -> AssociateGatewayToServerInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2/README.md` & `types-aiobotocore-backup-gateway-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-backup-gateway"></a>
 
 # types-aiobotocore-backup-gateway
 
 [![PyPI - types-aiobotocore-backup-gateway](https://img.shields.io/pypi/v/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-backup-gateway?color=blue)](https://pypistats.org/packages/types-aiobotocore-backup-gateway)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup-gateway)](https://pepy.tech/project/types-aiobotocore-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.BackupGateway 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
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
 [types-aiobotocore-backup-gateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/).
 
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
@@ -285,92 +285,94 @@
 )
 
 
 def check_value(value: GatewayTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_backup_gateway.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_backup_gateway.type_defs import (
     AssociateGatewayToServerInputRequestTypeDef,
-    AssociateGatewayToServerOutputTypeDef,
+    ResponseMetadataTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     TagTypeDef,
-    CreateGatewayOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
-    DeleteGatewayOutputTypeDef,
     DeleteHypervisorInputRequestTypeDef,
-    DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerInputRequestTypeDef,
-    DisassociateGatewayFromServerOutputTypeDef,
     MaintenanceStartTimeTypeDef,
     GatewayTypeDef,
     GetBandwidthRateLimitScheduleInputRequestTypeDef,
     GetGatewayInputRequestTypeDef,
     GetHypervisorInputRequestTypeDef,
     HypervisorDetailsTypeDef,
     GetHypervisorPropertyMappingsInputRequestTypeDef,
     VmwareToAwsTagMappingTypeDef,
     GetVirtualMachineInputRequestTypeDef,
     HypervisorTypeDef,
-    ImportHypervisorConfigurationOutputTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListGatewaysInputRequestTypeDef,
-    ListHypervisorsInputListHypervisorsPaginateTypeDef,
     ListHypervisorsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesInputRequestTypeDef,
     VirtualMachineTypeDef,
-    PaginatorConfigTypeDef,
+    PutMaintenanceStartTimeInputRequestTypeDef,
+    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
+    TestHypervisorConfigurationInputRequestTypeDef,
+    UntagResourceInputRequestTypeDef,
+    UpdateGatewayInformationInputRequestTypeDef,
+    UpdateGatewaySoftwareNowInputRequestTypeDef,
+    UpdateHypervisorInputRequestTypeDef,
+    VmwareTagTypeDef,
+    AssociateGatewayToServerOutputTypeDef,
+    CreateGatewayOutputTypeDef,
+    DeleteGatewayOutputTypeDef,
+    DeleteHypervisorOutputTypeDef,
+    DisassociateGatewayFromServerOutputTypeDef,
+    ImportHypervisorConfigurationOutputTypeDef,
     PutBandwidthRateLimitScheduleOutputTypeDef,
     PutHypervisorPropertyMappingsOutputTypeDef,
-    PutMaintenanceStartTimeInputRequestTypeDef,
     PutMaintenanceStartTimeOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
     StartVirtualMachinesMetadataSyncOutputTypeDef,
     TagResourceOutputTypeDef,
-    TestHypervisorConfigurationInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
     UntagResourceOutputTypeDef,
-    UpdateGatewayInformationInputRequestTypeDef,
     UpdateGatewayInformationOutputTypeDef,
-    UpdateGatewaySoftwareNowInputRequestTypeDef,
     UpdateGatewaySoftwareNowOutputTypeDef,
-    UpdateHypervisorInputRequestTypeDef,
     UpdateHypervisorOutputTypeDef,
-    VmwareTagTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
-    PutBandwidthRateLimitScheduleInputRequestTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CreateGatewayInputRequestTypeDef,
     ImportHypervisorConfigurationInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     GatewayDetailsTypeDef,
     ListGatewaysOutputTypeDef,
     GetHypervisorOutputTypeDef,
     GetHypervisorPropertyMappingsOutputTypeDef,
     PutHypervisorPropertyMappingsInputRequestTypeDef,
     ListHypervisorsOutputTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
+    ListHypervisorsInputListHypervisorsPaginateTypeDef,
+    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesOutputTypeDef,
     VirtualMachineDetailsTypeDef,
+    PutBandwidthRateLimitScheduleInputRequestTypeDef,
     GetGatewayOutputTypeDef,
     GetVirtualMachineOutputTypeDef,
 )
 
 
-def get_structure() -> AssociateGatewayToServerInputRequestTypeDef:
+def get_value() -> AssociateGatewayToServerInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2/setup.py` & `types-aiobotocore-backup-gateway-2.5.2.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-backup-gateway",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_backup_gateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.BackupGateway 2.5.2 service generated with"
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
-    keywords="aiobotocore backup-gateway type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore backup-gateway type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_backup_gateway": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/"
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/__init__.py` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/__init__.pyi` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/__main__.py` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.BackupGateway 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.BackupGateway 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway\nOther"
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

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/client.py` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import ListGatewaysPaginator, ListHypervisorsPaginator, ListVirtualMachinesPaginator
 from .type_defs import (
     AssociateGatewayToServerOutputTypeDef,
-    BandwidthRateLimitIntervalTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CreateGatewayOutputTypeDef,
     DeleteGatewayOutputTypeDef,
     DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerOutputTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
     GetGatewayOutputTypeDef,
     GetHypervisorOutputTypeDef,
@@ -278,15 +278,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.list_virtual_machines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#list_virtual_machines)
         """
 
     async def put_bandwidth_rate_limit_schedule(
         self,
         *,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef],
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef],
         GatewayArn: str
     ) -> PutBandwidthRateLimitScheduleOutputTypeDef:
         """
         This action sets the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_bandwidth_rate_limit_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#put_bandwidth_rate_limit_schedule)
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/client.pyi` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import ListGatewaysPaginator, ListHypervisorsPaginator, ListVirtualMachinesPaginator
 from .type_defs import (
     AssociateGatewayToServerOutputTypeDef,
-    BandwidthRateLimitIntervalTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CreateGatewayOutputTypeDef,
     DeleteGatewayOutputTypeDef,
     DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerOutputTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
     GetGatewayOutputTypeDef,
     GetHypervisorOutputTypeDef,
@@ -255,15 +255,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.list_virtual_machines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#list_virtual_machines)
         """
     async def put_bandwidth_rate_limit_schedule(
         self,
         *,
-        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalTypeDef],
+        BandwidthRateLimitIntervals: Sequence[BandwidthRateLimitIntervalUnionTypeDef],
         GatewayArn: str
     ) -> PutBandwidthRateLimitScheduleOutputTypeDef:
         """
         This action sets the bandwidth rate limit schedule for a specified gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_bandwidth_rate_limit_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/client/#put_bandwidth_rate_limit_schedule)
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/literals.py` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/literals.pyi` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/paginator.py` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,43 +52,43 @@
 class ListGatewaysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListGateways)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListGateways.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/paginators/#listgatewayspaginator)
         """
 
 
 class ListHypervisorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListHypervisors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/paginators/#listhypervisorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHypervisorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListHypervisors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/paginators/#listhypervisorspaginator)
         """
 
 
 class ListVirtualMachinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListVirtualMachines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/paginators/#listvirtualmachinespaginator)
     """
 
     def paginate(
-        self, *, HypervisorArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, HypervisorArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVirtualMachinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListVirtualMachines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/paginators/#listvirtualmachinespaginator)
         """
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/paginator.pyi` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,41 +49,41 @@
 class ListGatewaysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListGateways)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/paginators/#listgatewayspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListGateways.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/paginators/#listgatewayspaginator)
         """
 
 class ListHypervisorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListHypervisors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/paginators/#listhypervisorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHypervisorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListHypervisors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/paginators/#listhypervisorspaginator)
         """
 
 class ListVirtualMachinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListVirtualMachines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/paginators/#listvirtualmachinespaginator)
     """
 
     def paginate(
-        self, *, HypervisorArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, HypervisorArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVirtualMachinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListVirtualMachines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/paginators/#listvirtualmachinespaginator)
         """
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/type_defs.py` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,203 +4,197 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_backup_gateway.type_defs import AssociateGatewayToServerInputRequestTypeDef
 
-    data: AssociateGatewayToServerInputRequestTypeDef = {...}
+    data: AssociateGatewayToServerInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import HypervisorStateType, SyncMetadataStatusType
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateGatewayToServerInputRequestTypeDef",
-    "AssociateGatewayToServerOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "TagTypeDef",
-    "CreateGatewayOutputTypeDef",
     "DeleteGatewayInputRequestTypeDef",
-    "DeleteGatewayOutputTypeDef",
     "DeleteHypervisorInputRequestTypeDef",
-    "DeleteHypervisorOutputTypeDef",
     "DisassociateGatewayFromServerInputRequestTypeDef",
-    "DisassociateGatewayFromServerOutputTypeDef",
     "MaintenanceStartTimeTypeDef",
     "GatewayTypeDef",
     "GetBandwidthRateLimitScheduleInputRequestTypeDef",
     "GetGatewayInputRequestTypeDef",
     "GetHypervisorInputRequestTypeDef",
     "HypervisorDetailsTypeDef",
     "GetHypervisorPropertyMappingsInputRequestTypeDef",
     "VmwareToAwsTagMappingTypeDef",
     "GetVirtualMachineInputRequestTypeDef",
     "HypervisorTypeDef",
-    "ImportHypervisorConfigurationOutputTypeDef",
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListGatewaysInputRequestTypeDef",
-    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
     "ListHypervisorsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
     "ListVirtualMachinesInputRequestTypeDef",
     "VirtualMachineTypeDef",
-    "PaginatorConfigTypeDef",
+    "PutMaintenanceStartTimeInputRequestTypeDef",
+    "StartVirtualMachinesMetadataSyncInputRequestTypeDef",
+    "TestHypervisorConfigurationInputRequestTypeDef",
+    "UntagResourceInputRequestTypeDef",
+    "UpdateGatewayInformationInputRequestTypeDef",
+    "UpdateGatewaySoftwareNowInputRequestTypeDef",
+    "UpdateHypervisorInputRequestTypeDef",
+    "VmwareTagTypeDef",
+    "AssociateGatewayToServerOutputTypeDef",
+    "CreateGatewayOutputTypeDef",
+    "DeleteGatewayOutputTypeDef",
+    "DeleteHypervisorOutputTypeDef",
+    "DisassociateGatewayFromServerOutputTypeDef",
+    "ImportHypervisorConfigurationOutputTypeDef",
     "PutBandwidthRateLimitScheduleOutputTypeDef",
     "PutHypervisorPropertyMappingsOutputTypeDef",
-    "PutMaintenanceStartTimeInputRequestTypeDef",
     "PutMaintenanceStartTimeOutputTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartVirtualMachinesMetadataSyncInputRequestTypeDef",
     "StartVirtualMachinesMetadataSyncOutputTypeDef",
     "TagResourceOutputTypeDef",
-    "TestHypervisorConfigurationInputRequestTypeDef",
-    "UntagResourceInputRequestTypeDef",
     "UntagResourceOutputTypeDef",
-    "UpdateGatewayInformationInputRequestTypeDef",
     "UpdateGatewayInformationOutputTypeDef",
-    "UpdateGatewaySoftwareNowInputRequestTypeDef",
     "UpdateGatewaySoftwareNowOutputTypeDef",
-    "UpdateHypervisorInputRequestTypeDef",
     "UpdateHypervisorOutputTypeDef",
-    "VmwareTagTypeDef",
     "GetBandwidthRateLimitScheduleOutputTypeDef",
-    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
+    "BandwidthRateLimitIntervalUnionTypeDef",
     "CreateGatewayInputRequestTypeDef",
     "ImportHypervisorConfigurationInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "GatewayDetailsTypeDef",
     "ListGatewaysOutputTypeDef",
     "GetHypervisorOutputTypeDef",
     "GetHypervisorPropertyMappingsOutputTypeDef",
     "PutHypervisorPropertyMappingsInputRequestTypeDef",
     "ListHypervisorsOutputTypeDef",
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
+    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
     "ListVirtualMachinesOutputTypeDef",
     "VirtualMachineDetailsTypeDef",
+    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     "GetGatewayOutputTypeDef",
     "GetVirtualMachineOutputTypeDef",
 )
 
 AssociateGatewayToServerInputRequestTypeDef = TypedDict(
     "AssociateGatewayToServerInputRequestTypeDef",
     {
         "GatewayArn": str,
         "ServerArn": str,
     },
 )
 
-AssociateGatewayToServerOutputTypeDef = TypedDict(
-    "AssociateGatewayToServerOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+_RequiredBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
+    "_RequiredBandwidthRateLimitIntervalOutputTypeDef",
+    {
+        "DaysOfWeek": List[int],
+        "EndHourOfDay": int,
+        "EndMinuteOfHour": int,
+        "StartHourOfDay": int,
+        "StartMinuteOfHour": int,
+    },
+)
+_OptionalBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
+    "_OptionalBandwidthRateLimitIntervalOutputTypeDef",
+    {
+        "AverageUploadRateLimitInBitsPerSec": int,
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
-        "DaysOfWeek": List[int],
+        "DaysOfWeek": Sequence[int],
         "EndHourOfDay": int,
         "EndMinuteOfHour": int,
         "StartHourOfDay": int,
         "StartMinuteOfHour": int,
     },
 )
 _OptionalBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_OptionalBandwidthRateLimitIntervalTypeDef",
     {
         "AverageUploadRateLimitInBitsPerSec": int,
     },
     total=False,
 )
 
-
 class BandwidthRateLimitIntervalTypeDef(
     _RequiredBandwidthRateLimitIntervalTypeDef, _OptionalBandwidthRateLimitIntervalTypeDef
 ):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateGatewayOutputTypeDef = TypedDict(
-    "CreateGatewayOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGatewayInputRequestTypeDef = TypedDict(
     "DeleteGatewayInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
-DeleteGatewayOutputTypeDef = TypedDict(
-    "DeleteGatewayOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteHypervisorInputRequestTypeDef = TypedDict(
     "DeleteHypervisorInputRequestTypeDef",
     {
         "HypervisorArn": str,
     },
 )
 
-DeleteHypervisorOutputTypeDef = TypedDict(
-    "DeleteHypervisorOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateGatewayFromServerInputRequestTypeDef = TypedDict(
     "DisassociateGatewayFromServerInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
-DisassociateGatewayFromServerOutputTypeDef = TypedDict(
-    "DisassociateGatewayFromServerOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMaintenanceStartTimeTypeDef = TypedDict(
     "_RequiredMaintenanceStartTimeTypeDef",
     {
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
 )
@@ -209,21 +203,19 @@
     {
         "DayOfMonth": int,
         "DayOfWeek": int,
     },
     total=False,
 )
 
-
 class MaintenanceStartTimeTypeDef(
     _RequiredMaintenanceStartTimeTypeDef, _OptionalMaintenanceStartTimeTypeDef
 ):
     pass
 
-
 GatewayTypeDef = TypedDict(
     "GatewayTypeDef",
     {
         "GatewayArn": str,
         "GatewayDisplayName": str,
         "GatewayType": Literal["BACKUP_VM"],
         "HypervisorId": str,
@@ -301,47 +293,33 @@
         "KmsKeyArn": str,
         "Name": str,
         "State": HypervisorStateType,
     },
     total=False,
 )
 
-ImportHypervisorConfigurationOutputTypeDef = TypedDict(
-    "ImportHypervisorConfigurationOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
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
 
 ListGatewaysInputRequestTypeDef = TypedDict(
     "ListGatewaysInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListHypervisorsInputListHypervisorsPaginateTypeDef = TypedDict(
-    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHypervisorsInputRequestTypeDef = TypedDict(
     "ListHypervisorsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -350,23 +328,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef = TypedDict(
-    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
-    {
-        "HypervisorArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVirtualMachinesInputRequestTypeDef = TypedDict(
     "ListVirtualMachinesInputRequestTypeDef",
     {
         "HypervisorArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -382,40 +351,14 @@
         "Name": str,
         "Path": str,
         "ResourceArn": str,
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
-PutBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
-    "PutBandwidthRateLimitScheduleOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutHypervisorPropertyMappingsOutputTypeDef = TypedDict(
-    "PutHypervisorPropertyMappingsOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "_RequiredPutMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayArn": str,
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
@@ -425,64 +368,27 @@
     {
         "DayOfMonth": int,
         "DayOfWeek": int,
     },
     total=False,
 )
 
-
 class PutMaintenanceStartTimeInputRequestTypeDef(
     _RequiredPutMaintenanceStartTimeInputRequestTypeDef,
     _OptionalPutMaintenanceStartTimeInputRequestTypeDef,
 ):
     pass
 
-
-PutMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "PutMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayArn": str,
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
 StartVirtualMachinesMetadataSyncInputRequestTypeDef = TypedDict(
     "StartVirtualMachinesMetadataSyncInputRequestTypeDef",
     {
         "HypervisorArn": str,
     },
 )
 
-StartVirtualMachinesMetadataSyncOutputTypeDef = TypedDict(
-    "StartVirtualMachinesMetadataSyncOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagResourceOutputTypeDef = TypedDict(
-    "TagResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTestHypervisorConfigurationInputRequestTypeDef = TypedDict(
     "_RequiredTestHypervisorConfigurationInputRequestTypeDef",
     {
         "GatewayArn": str,
         "Host": str,
     },
 )
@@ -491,83 +397,55 @@
     {
         "Password": str,
         "Username": str,
     },
     total=False,
 )
 
-
 class TestHypervisorConfigurationInputRequestTypeDef(
     _RequiredTestHypervisorConfigurationInputRequestTypeDef,
     _OptionalTestHypervisorConfigurationInputRequestTypeDef,
 ):
     pass
 
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UntagResourceOutputTypeDef = TypedDict(
-    "UntagResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 _OptionalUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_OptionalUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayDisplayName": str,
     },
     total=False,
 )
 
-
 class UpdateGatewayInformationInputRequestTypeDef(
     _RequiredUpdateGatewayInformationInputRequestTypeDef,
     _OptionalUpdateGatewayInformationInputRequestTypeDef,
 ):
     pass
 
-
-UpdateGatewayInformationOutputTypeDef = TypedDict(
-    "UpdateGatewayInformationOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateGatewaySoftwareNowInputRequestTypeDef = TypedDict(
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
-UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
-    "UpdateGatewaySoftwareNowOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateHypervisorInputRequestTypeDef = TypedDict(
     "_RequiredUpdateHypervisorInputRequestTypeDef",
     {
         "HypervisorArn": str,
     },
 )
 _OptionalUpdateHypervisorInputRequestTypeDef = TypedDict(
@@ -578,56 +456,161 @@
         "Name": str,
         "Password": str,
         "Username": str,
     },
     total=False,
 )
 
-
 class UpdateHypervisorInputRequestTypeDef(
     _RequiredUpdateHypervisorInputRequestTypeDef, _OptionalUpdateHypervisorInputRequestTypeDef
 ):
     pass
 
-
-UpdateHypervisorOutputTypeDef = TypedDict(
-    "UpdateHypervisorOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VmwareTagTypeDef = TypedDict(
     "VmwareTagTypeDef",
     {
         "VmwareCategory": str,
         "VmwareTagDescription": str,
         "VmwareTagName": str,
     },
     total=False,
 )
 
-GetBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
-    "GetBandwidthRateLimitScheduleOutputTypeDef",
+AssociateGatewayToServerOutputTypeDef = TypedDict(
+    "AssociateGatewayToServerOutputTypeDef",
     {
-        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
         "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
+CreateGatewayOutputTypeDef = TypedDict(
+    "CreateGatewayOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGatewayOutputTypeDef = TypedDict(
+    "DeleteGatewayOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteHypervisorOutputTypeDef = TypedDict(
+    "DeleteHypervisorOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateGatewayFromServerOutputTypeDef = TypedDict(
+    "DisassociateGatewayFromServerOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportHypervisorConfigurationOutputTypeDef = TypedDict(
+    "ImportHypervisorConfigurationOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
+    "PutBandwidthRateLimitScheduleOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutHypervisorPropertyMappingsOutputTypeDef = TypedDict(
+    "PutHypervisorPropertyMappingsOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "PutMaintenanceStartTimeOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartVirtualMachinesMetadataSyncOutputTypeDef = TypedDict(
+    "StartVirtualMachinesMetadataSyncOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceOutputTypeDef = TypedDict(
+    "TagResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UntagResourceOutputTypeDef = TypedDict(
+    "UntagResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewayInformationOutputTypeDef = TypedDict(
+    "UpdateGatewayInformationOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateHypervisorOutputTypeDef = TypedDict(
+    "UpdateHypervisorOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
+    "GetBandwidthRateLimitScheduleOutputTypeDef",
     {
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
+        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
         "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BandwidthRateLimitIntervalUnionTypeDef = Union[
+    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
+]
 _RequiredCreateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayInputRequestTypeDef",
     {
         "ActivationKey": str,
         "GatewayDisplayName": str,
         "GatewayType": Literal["BACKUP_VM"],
     },
@@ -636,21 +619,19 @@
     "_OptionalCreateGatewayInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateGatewayInputRequestTypeDef(
     _RequiredCreateGatewayInputRequestTypeDef, _OptionalCreateGatewayInputRequestTypeDef
 ):
     pass
 
-
 _RequiredImportHypervisorConfigurationInputRequestTypeDef = TypedDict(
     "_RequiredImportHypervisorConfigurationInputRequestTypeDef",
     {
         "Host": str,
         "Name": str,
     },
 )
@@ -661,28 +642,26 @@
         "Password": str,
         "Tags": Sequence[TagTypeDef],
         "Username": str,
     },
     total=False,
 )
 
-
 class ImportHypervisorConfigurationInputRequestTypeDef(
     _RequiredImportHypervisorConfigurationInputRequestTypeDef,
     _OptionalImportHypervisorConfigurationInputRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
@@ -706,33 +685,33 @@
 )
 
 ListGatewaysOutputTypeDef = TypedDict(
     "ListGatewaysOutputTypeDef",
     {
         "Gateways": List[GatewayTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHypervisorOutputTypeDef = TypedDict(
     "GetHypervisorOutputTypeDef",
     {
         "Hypervisor": HypervisorDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHypervisorPropertyMappingsOutputTypeDef = TypedDict(
     "GetHypervisorPropertyMappingsOutputTypeDef",
     {
         "HypervisorArn": str,
         "IamRoleArn": str,
         "VmwareToAwsTagMappings": List[VmwareToAwsTagMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutHypervisorPropertyMappingsInputRequestTypeDef = TypedDict(
     "PutHypervisorPropertyMappingsInputRequestTypeDef",
     {
         "HypervisorArn": str,
@@ -742,24 +721,49 @@
 )
 
 ListHypervisorsOutputTypeDef = TypedDict(
     "ListHypervisorsOutputTypeDef",
     {
         "Hypervisors": List[HypervisorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListHypervisorsInputListHypervisorsPaginateTypeDef = TypedDict(
+    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef = TypedDict(
+    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
+    {
+        "HypervisorArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListVirtualMachinesOutputTypeDef = TypedDict(
     "ListVirtualMachinesOutputTypeDef",
     {
         "NextToken": str,
         "VirtualMachines": List[VirtualMachineTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualMachineDetailsTypeDef = TypedDict(
     "VirtualMachineDetailsTypeDef",
     {
         "HostName": str,
@@ -769,22 +773,30 @@
         "Path": str,
         "ResourceArn": str,
         "VmwareTags": List[VmwareTagTypeDef],
     },
     total=False,
 )
 
+PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
+        "GatewayArn": str,
+    },
+)
+
 GetGatewayOutputTypeDef = TypedDict(
     "GetGatewayOutputTypeDef",
     {
         "Gateway": GatewayDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVirtualMachineOutputTypeDef = TypedDict(
     "GetVirtualMachineOutputTypeDef",
     {
         "VirtualMachine": VirtualMachineDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway/type_defs.pyi` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,200 +4,202 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_backup_gateway.type_defs import AssociateGatewayToServerInputRequestTypeDef
 
-    data: AssociateGatewayToServerInputRequestTypeDef = {...}
+    data: AssociateGatewayToServerInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import HypervisorStateType, SyncMetadataStatusType
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateGatewayToServerInputRequestTypeDef",
-    "AssociateGatewayToServerOutputTypeDef",
+    "ResponseMetadataTypeDef",
+    "BandwidthRateLimitIntervalOutputTypeDef",
     "BandwidthRateLimitIntervalTypeDef",
     "TagTypeDef",
-    "CreateGatewayOutputTypeDef",
     "DeleteGatewayInputRequestTypeDef",
-    "DeleteGatewayOutputTypeDef",
     "DeleteHypervisorInputRequestTypeDef",
-    "DeleteHypervisorOutputTypeDef",
     "DisassociateGatewayFromServerInputRequestTypeDef",
-    "DisassociateGatewayFromServerOutputTypeDef",
     "MaintenanceStartTimeTypeDef",
     "GatewayTypeDef",
     "GetBandwidthRateLimitScheduleInputRequestTypeDef",
     "GetGatewayInputRequestTypeDef",
     "GetHypervisorInputRequestTypeDef",
     "HypervisorDetailsTypeDef",
     "GetHypervisorPropertyMappingsInputRequestTypeDef",
     "VmwareToAwsTagMappingTypeDef",
     "GetVirtualMachineInputRequestTypeDef",
     "HypervisorTypeDef",
-    "ImportHypervisorConfigurationOutputTypeDef",
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListGatewaysInputRequestTypeDef",
-    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
     "ListHypervisorsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
     "ListVirtualMachinesInputRequestTypeDef",
     "VirtualMachineTypeDef",
-    "PaginatorConfigTypeDef",
+    "PutMaintenanceStartTimeInputRequestTypeDef",
+    "StartVirtualMachinesMetadataSyncInputRequestTypeDef",
+    "TestHypervisorConfigurationInputRequestTypeDef",
+    "UntagResourceInputRequestTypeDef",
+    "UpdateGatewayInformationInputRequestTypeDef",
+    "UpdateGatewaySoftwareNowInputRequestTypeDef",
+    "UpdateHypervisorInputRequestTypeDef",
+    "VmwareTagTypeDef",
+    "AssociateGatewayToServerOutputTypeDef",
+    "CreateGatewayOutputTypeDef",
+    "DeleteGatewayOutputTypeDef",
+    "DeleteHypervisorOutputTypeDef",
+    "DisassociateGatewayFromServerOutputTypeDef",
+    "ImportHypervisorConfigurationOutputTypeDef",
     "PutBandwidthRateLimitScheduleOutputTypeDef",
     "PutHypervisorPropertyMappingsOutputTypeDef",
-    "PutMaintenanceStartTimeInputRequestTypeDef",
     "PutMaintenanceStartTimeOutputTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartVirtualMachinesMetadataSyncInputRequestTypeDef",
     "StartVirtualMachinesMetadataSyncOutputTypeDef",
     "TagResourceOutputTypeDef",
-    "TestHypervisorConfigurationInputRequestTypeDef",
-    "UntagResourceInputRequestTypeDef",
     "UntagResourceOutputTypeDef",
-    "UpdateGatewayInformationInputRequestTypeDef",
     "UpdateGatewayInformationOutputTypeDef",
-    "UpdateGatewaySoftwareNowInputRequestTypeDef",
     "UpdateGatewaySoftwareNowOutputTypeDef",
-    "UpdateHypervisorInputRequestTypeDef",
     "UpdateHypervisorOutputTypeDef",
-    "VmwareTagTypeDef",
     "GetBandwidthRateLimitScheduleOutputTypeDef",
-    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
+    "BandwidthRateLimitIntervalUnionTypeDef",
     "CreateGatewayInputRequestTypeDef",
     "ImportHypervisorConfigurationInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "GatewayDetailsTypeDef",
     "ListGatewaysOutputTypeDef",
     "GetHypervisorOutputTypeDef",
     "GetHypervisorPropertyMappingsOutputTypeDef",
     "PutHypervisorPropertyMappingsInputRequestTypeDef",
     "ListHypervisorsOutputTypeDef",
+    "ListGatewaysInputListGatewaysPaginateTypeDef",
+    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
+    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
     "ListVirtualMachinesOutputTypeDef",
     "VirtualMachineDetailsTypeDef",
+    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
     "GetGatewayOutputTypeDef",
     "GetVirtualMachineOutputTypeDef",
 )
 
 AssociateGatewayToServerInputRequestTypeDef = TypedDict(
     "AssociateGatewayToServerInputRequestTypeDef",
     {
         "GatewayArn": str,
         "ServerArn": str,
     },
 )
 
-AssociateGatewayToServerOutputTypeDef = TypedDict(
-    "AssociateGatewayToServerOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+_RequiredBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
+    "_RequiredBandwidthRateLimitIntervalOutputTypeDef",
+    {
+        "DaysOfWeek": List[int],
+        "EndHourOfDay": int,
+        "EndMinuteOfHour": int,
+        "StartHourOfDay": int,
+        "StartMinuteOfHour": int,
+    },
+)
+_OptionalBandwidthRateLimitIntervalOutputTypeDef = TypedDict(
+    "_OptionalBandwidthRateLimitIntervalOutputTypeDef",
+    {
+        "AverageUploadRateLimitInBitsPerSec": int,
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
-        "DaysOfWeek": List[int],
+        "DaysOfWeek": Sequence[int],
         "EndHourOfDay": int,
         "EndMinuteOfHour": int,
         "StartHourOfDay": int,
         "StartMinuteOfHour": int,
     },
 )
 _OptionalBandwidthRateLimitIntervalTypeDef = TypedDict(
     "_OptionalBandwidthRateLimitIntervalTypeDef",
     {
         "AverageUploadRateLimitInBitsPerSec": int,
     },
     total=False,
 )
 
+
 class BandwidthRateLimitIntervalTypeDef(
     _RequiredBandwidthRateLimitIntervalTypeDef, _OptionalBandwidthRateLimitIntervalTypeDef
 ):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateGatewayOutputTypeDef = TypedDict(
-    "CreateGatewayOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGatewayInputRequestTypeDef = TypedDict(
     "DeleteGatewayInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
-DeleteGatewayOutputTypeDef = TypedDict(
-    "DeleteGatewayOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteHypervisorInputRequestTypeDef = TypedDict(
     "DeleteHypervisorInputRequestTypeDef",
     {
         "HypervisorArn": str,
     },
 )
 
-DeleteHypervisorOutputTypeDef = TypedDict(
-    "DeleteHypervisorOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateGatewayFromServerInputRequestTypeDef = TypedDict(
     "DisassociateGatewayFromServerInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
-DisassociateGatewayFromServerOutputTypeDef = TypedDict(
-    "DisassociateGatewayFromServerOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMaintenanceStartTimeTypeDef = TypedDict(
     "_RequiredMaintenanceStartTimeTypeDef",
     {
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
 )
@@ -206,19 +208,21 @@
     {
         "DayOfMonth": int,
         "DayOfWeek": int,
     },
     total=False,
 )
 
+
 class MaintenanceStartTimeTypeDef(
     _RequiredMaintenanceStartTimeTypeDef, _OptionalMaintenanceStartTimeTypeDef
 ):
     pass
 
+
 GatewayTypeDef = TypedDict(
     "GatewayTypeDef",
     {
         "GatewayArn": str,
         "GatewayDisplayName": str,
         "GatewayType": Literal["BACKUP_VM"],
         "HypervisorId": str,
@@ -296,47 +300,33 @@
         "KmsKeyArn": str,
         "Name": str,
         "State": HypervisorStateType,
     },
     total=False,
 )
 
-ImportHypervisorConfigurationOutputTypeDef = TypedDict(
-    "ImportHypervisorConfigurationOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListGatewaysInputListGatewaysPaginateTypeDef = TypedDict(
-    "ListGatewaysInputListGatewaysPaginateTypeDef",
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
 
 ListGatewaysInputRequestTypeDef = TypedDict(
     "ListGatewaysInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListHypervisorsInputListHypervisorsPaginateTypeDef = TypedDict(
-    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHypervisorsInputRequestTypeDef = TypedDict(
     "ListHypervisorsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -345,23 +335,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef = TypedDict(
-    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
-    {
-        "HypervisorArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVirtualMachinesInputRequestTypeDef = TypedDict(
     "ListVirtualMachinesInputRequestTypeDef",
     {
         "HypervisorArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -377,40 +358,14 @@
         "Name": str,
         "Path": str,
         "ResourceArn": str,
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
-PutBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
-    "PutBandwidthRateLimitScheduleOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutHypervisorPropertyMappingsOutputTypeDef = TypedDict(
-    "PutHypervisorPropertyMappingsOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutMaintenanceStartTimeInputRequestTypeDef = TypedDict(
     "_RequiredPutMaintenanceStartTimeInputRequestTypeDef",
     {
         "GatewayArn": str,
         "HourOfDay": int,
         "MinuteOfHour": int,
     },
@@ -420,62 +375,29 @@
     {
         "DayOfMonth": int,
         "DayOfWeek": int,
     },
     total=False,
 )
 
+
 class PutMaintenanceStartTimeInputRequestTypeDef(
     _RequiredPutMaintenanceStartTimeInputRequestTypeDef,
     _OptionalPutMaintenanceStartTimeInputRequestTypeDef,
 ):
     pass
 
-PutMaintenanceStartTimeOutputTypeDef = TypedDict(
-    "PutMaintenanceStartTimeOutputTypeDef",
-    {
-        "GatewayArn": str,
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
 
 StartVirtualMachinesMetadataSyncInputRequestTypeDef = TypedDict(
     "StartVirtualMachinesMetadataSyncInputRequestTypeDef",
     {
         "HypervisorArn": str,
     },
 )
 
-StartVirtualMachinesMetadataSyncOutputTypeDef = TypedDict(
-    "StartVirtualMachinesMetadataSyncOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagResourceOutputTypeDef = TypedDict(
-    "TagResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTestHypervisorConfigurationInputRequestTypeDef = TypedDict(
     "_RequiredTestHypervisorConfigurationInputRequestTypeDef",
     {
         "GatewayArn": str,
         "Host": str,
     },
 )
@@ -484,79 +406,59 @@
     {
         "Password": str,
         "Username": str,
     },
     total=False,
 )
 
+
 class TestHypervisorConfigurationInputRequestTypeDef(
     _RequiredTestHypervisorConfigurationInputRequestTypeDef,
     _OptionalTestHypervisorConfigurationInputRequestTypeDef,
 ):
     pass
 
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UntagResourceOutputTypeDef = TypedDict(
-    "UntagResourceOutputTypeDef",
-    {
-        "ResourceARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 _OptionalUpdateGatewayInformationInputRequestTypeDef = TypedDict(
     "_OptionalUpdateGatewayInformationInputRequestTypeDef",
     {
         "GatewayDisplayName": str,
     },
     total=False,
 )
 
+
 class UpdateGatewayInformationInputRequestTypeDef(
     _RequiredUpdateGatewayInformationInputRequestTypeDef,
     _OptionalUpdateGatewayInformationInputRequestTypeDef,
 ):
     pass
 
-UpdateGatewayInformationOutputTypeDef = TypedDict(
-    "UpdateGatewayInformationOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UpdateGatewaySoftwareNowInputRequestTypeDef = TypedDict(
     "UpdateGatewaySoftwareNowInputRequestTypeDef",
     {
         "GatewayArn": str,
     },
 )
 
-UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
-    "UpdateGatewaySoftwareNowOutputTypeDef",
-    {
-        "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateHypervisorInputRequestTypeDef = TypedDict(
     "_RequiredUpdateHypervisorInputRequestTypeDef",
     {
         "HypervisorArn": str,
     },
 )
 _OptionalUpdateHypervisorInputRequestTypeDef = TypedDict(
@@ -567,54 +469,163 @@
         "Name": str,
         "Password": str,
         "Username": str,
     },
     total=False,
 )
 
+
 class UpdateHypervisorInputRequestTypeDef(
     _RequiredUpdateHypervisorInputRequestTypeDef, _OptionalUpdateHypervisorInputRequestTypeDef
 ):
     pass
 
-UpdateHypervisorOutputTypeDef = TypedDict(
-    "UpdateHypervisorOutputTypeDef",
-    {
-        "HypervisorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 VmwareTagTypeDef = TypedDict(
     "VmwareTagTypeDef",
     {
         "VmwareCategory": str,
         "VmwareTagDescription": str,
         "VmwareTagName": str,
     },
     total=False,
 )
 
-GetBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
-    "GetBandwidthRateLimitScheduleOutputTypeDef",
+AssociateGatewayToServerOutputTypeDef = TypedDict(
+    "AssociateGatewayToServerOutputTypeDef",
     {
-        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalTypeDef],
         "GatewayArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
-    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
+CreateGatewayOutputTypeDef = TypedDict(
+    "CreateGatewayOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGatewayOutputTypeDef = TypedDict(
+    "DeleteGatewayOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteHypervisorOutputTypeDef = TypedDict(
+    "DeleteHypervisorOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateGatewayFromServerOutputTypeDef = TypedDict(
+    "DisassociateGatewayFromServerOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportHypervisorConfigurationOutputTypeDef = TypedDict(
+    "ImportHypervisorConfigurationOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
+    "PutBandwidthRateLimitScheduleOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutHypervisorPropertyMappingsOutputTypeDef = TypedDict(
+    "PutHypervisorPropertyMappingsOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutMaintenanceStartTimeOutputTypeDef = TypedDict(
+    "PutMaintenanceStartTimeOutputTypeDef",
     {
-        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalTypeDef],
         "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StartVirtualMachinesMetadataSyncOutputTypeDef = TypedDict(
+    "StartVirtualMachinesMetadataSyncOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceOutputTypeDef = TypedDict(
+    "TagResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UntagResourceOutputTypeDef = TypedDict(
+    "UntagResourceOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewayInformationOutputTypeDef = TypedDict(
+    "UpdateGatewayInformationOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGatewaySoftwareNowOutputTypeDef = TypedDict(
+    "UpdateGatewaySoftwareNowOutputTypeDef",
+    {
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateHypervisorOutputTypeDef = TypedDict(
+    "UpdateHypervisorOutputTypeDef",
+    {
+        "HypervisorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBandwidthRateLimitScheduleOutputTypeDef = TypedDict(
+    "GetBandwidthRateLimitScheduleOutputTypeDef",
+    {
+        "BandwidthRateLimitIntervals": List[BandwidthRateLimitIntervalOutputTypeDef],
+        "GatewayArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BandwidthRateLimitIntervalUnionTypeDef = Union[
+    BandwidthRateLimitIntervalTypeDef, BandwidthRateLimitIntervalOutputTypeDef
+]
 _RequiredCreateGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayInputRequestTypeDef",
     {
         "ActivationKey": str,
         "GatewayDisplayName": str,
         "GatewayType": Literal["BACKUP_VM"],
     },
@@ -623,19 +634,21 @@
     "_OptionalCreateGatewayInputRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateGatewayInputRequestTypeDef(
     _RequiredCreateGatewayInputRequestTypeDef, _OptionalCreateGatewayInputRequestTypeDef
 ):
     pass
 
+
 _RequiredImportHypervisorConfigurationInputRequestTypeDef = TypedDict(
     "_RequiredImportHypervisorConfigurationInputRequestTypeDef",
     {
         "Host": str,
         "Name": str,
     },
 )
@@ -646,26 +659,28 @@
         "Password": str,
         "Tags": Sequence[TagTypeDef],
         "Username": str,
     },
     total=False,
 )
 
+
 class ImportHypervisorConfigurationInputRequestTypeDef(
     _RequiredImportHypervisorConfigurationInputRequestTypeDef,
     _OptionalImportHypervisorConfigurationInputRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
@@ -689,33 +704,33 @@
 )
 
 ListGatewaysOutputTypeDef = TypedDict(
     "ListGatewaysOutputTypeDef",
     {
         "Gateways": List[GatewayTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHypervisorOutputTypeDef = TypedDict(
     "GetHypervisorOutputTypeDef",
     {
         "Hypervisor": HypervisorDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHypervisorPropertyMappingsOutputTypeDef = TypedDict(
     "GetHypervisorPropertyMappingsOutputTypeDef",
     {
         "HypervisorArn": str,
         "IamRoleArn": str,
         "VmwareToAwsTagMappings": List[VmwareToAwsTagMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutHypervisorPropertyMappingsInputRequestTypeDef = TypedDict(
     "PutHypervisorPropertyMappingsInputRequestTypeDef",
     {
         "HypervisorArn": str,
@@ -725,24 +740,49 @@
 )
 
 ListHypervisorsOutputTypeDef = TypedDict(
     "ListHypervisorsOutputTypeDef",
     {
         "Hypervisors": List[HypervisorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
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
+ListHypervisorsInputListHypervisorsPaginateTypeDef = TypedDict(
+    "ListHypervisorsInputListHypervisorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef = TypedDict(
+    "ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef",
+    {
+        "HypervisorArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListVirtualMachinesOutputTypeDef = TypedDict(
     "ListVirtualMachinesOutputTypeDef",
     {
         "NextToken": str,
         "VirtualMachines": List[VirtualMachineTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualMachineDetailsTypeDef = TypedDict(
     "VirtualMachineDetailsTypeDef",
     {
         "HostName": str,
@@ -752,22 +792,30 @@
         "Path": str,
         "ResourceArn": str,
         "VmwareTags": List[VmwareTagTypeDef],
     },
     total=False,
 )
 
+PutBandwidthRateLimitScheduleInputRequestTypeDef = TypedDict(
+    "PutBandwidthRateLimitScheduleInputRequestTypeDef",
+    {
+        "BandwidthRateLimitIntervals": Sequence[BandwidthRateLimitIntervalUnionTypeDef],
+        "GatewayArn": str,
+    },
+)
+
 GetGatewayOutputTypeDef = TypedDict(
     "GetGatewayOutputTypeDef",
     {
         "Gateway": GatewayDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVirtualMachineOutputTypeDef = TypedDict(
     "GetVirtualMachineOutputTypeDef",
     {
         "VirtualMachine": VirtualMachineDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway.egg-info/PKG-INFO` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backup-gateway
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.BackupGateway 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.BackupGateway 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore backup-gateway type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore backup-gateway type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-backup-gateway"></a>
 
 # types-aiobotocore-backup-gateway
 
 [![PyPI - types-aiobotocore-backup-gateway](https://img.shields.io/pypi/v/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backup-gateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backup-gateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-backup-gateway?color=blue)](https://pypistats.org/packages/types-aiobotocore-backup-gateway)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backup-gateway)](https://pepy.tech/project/types-aiobotocore-backup-gateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.BackupGateway 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
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
 [types-aiobotocore-backup-gateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backup_gateway/).
 
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
@@ -318,92 +317,94 @@
 )
 
 
 def check_value(value: GatewayTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_backup_gateway.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_backup_gateway.type_defs import (
     AssociateGatewayToServerInputRequestTypeDef,
-    AssociateGatewayToServerOutputTypeDef,
+    ResponseMetadataTypeDef,
+    BandwidthRateLimitIntervalOutputTypeDef,
     BandwidthRateLimitIntervalTypeDef,
     TagTypeDef,
-    CreateGatewayOutputTypeDef,
     DeleteGatewayInputRequestTypeDef,
-    DeleteGatewayOutputTypeDef,
     DeleteHypervisorInputRequestTypeDef,
-    DeleteHypervisorOutputTypeDef,
     DisassociateGatewayFromServerInputRequestTypeDef,
-    DisassociateGatewayFromServerOutputTypeDef,
     MaintenanceStartTimeTypeDef,
     GatewayTypeDef,
     GetBandwidthRateLimitScheduleInputRequestTypeDef,
     GetGatewayInputRequestTypeDef,
     GetHypervisorInputRequestTypeDef,
     HypervisorDetailsTypeDef,
     GetHypervisorPropertyMappingsInputRequestTypeDef,
     VmwareToAwsTagMappingTypeDef,
     GetVirtualMachineInputRequestTypeDef,
     HypervisorTypeDef,
-    ImportHypervisorConfigurationOutputTypeDef,
-    ListGatewaysInputListGatewaysPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListGatewaysInputRequestTypeDef,
-    ListHypervisorsInputListHypervisorsPaginateTypeDef,
     ListHypervisorsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesInputRequestTypeDef,
     VirtualMachineTypeDef,
-    PaginatorConfigTypeDef,
+    PutMaintenanceStartTimeInputRequestTypeDef,
+    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
+    TestHypervisorConfigurationInputRequestTypeDef,
+    UntagResourceInputRequestTypeDef,
+    UpdateGatewayInformationInputRequestTypeDef,
+    UpdateGatewaySoftwareNowInputRequestTypeDef,
+    UpdateHypervisorInputRequestTypeDef,
+    VmwareTagTypeDef,
+    AssociateGatewayToServerOutputTypeDef,
+    CreateGatewayOutputTypeDef,
+    DeleteGatewayOutputTypeDef,
+    DeleteHypervisorOutputTypeDef,
+    DisassociateGatewayFromServerOutputTypeDef,
+    ImportHypervisorConfigurationOutputTypeDef,
     PutBandwidthRateLimitScheduleOutputTypeDef,
     PutHypervisorPropertyMappingsOutputTypeDef,
-    PutMaintenanceStartTimeInputRequestTypeDef,
     PutMaintenanceStartTimeOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartVirtualMachinesMetadataSyncInputRequestTypeDef,
     StartVirtualMachinesMetadataSyncOutputTypeDef,
     TagResourceOutputTypeDef,
-    TestHypervisorConfigurationInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
     UntagResourceOutputTypeDef,
-    UpdateGatewayInformationInputRequestTypeDef,
     UpdateGatewayInformationOutputTypeDef,
-    UpdateGatewaySoftwareNowInputRequestTypeDef,
     UpdateGatewaySoftwareNowOutputTypeDef,
-    UpdateHypervisorInputRequestTypeDef,
     UpdateHypervisorOutputTypeDef,
-    VmwareTagTypeDef,
     GetBandwidthRateLimitScheduleOutputTypeDef,
-    PutBandwidthRateLimitScheduleInputRequestTypeDef,
+    BandwidthRateLimitIntervalUnionTypeDef,
     CreateGatewayInputRequestTypeDef,
     ImportHypervisorConfigurationInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     GatewayDetailsTypeDef,
     ListGatewaysOutputTypeDef,
     GetHypervisorOutputTypeDef,
     GetHypervisorPropertyMappingsOutputTypeDef,
     PutHypervisorPropertyMappingsInputRequestTypeDef,
     ListHypervisorsOutputTypeDef,
+    ListGatewaysInputListGatewaysPaginateTypeDef,
+    ListHypervisorsInputListHypervisorsPaginateTypeDef,
+    ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef,
     ListVirtualMachinesOutputTypeDef,
     VirtualMachineDetailsTypeDef,
+    PutBandwidthRateLimitScheduleInputRequestTypeDef,
     GetGatewayOutputTypeDef,
     GetVirtualMachineOutputTypeDef,
 )
 
 
-def get_structure() -> AssociateGatewayToServerInputRequestTypeDef:
+def get_value() -> AssociateGatewayToServerInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-backup-gateway-2.5.2/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt` & `types-aiobotocore-backup-gateway-2.5.2.post1/types_aiobotocore_backup_gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*


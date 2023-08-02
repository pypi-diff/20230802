# Comparing `tmp/types-aiobotocore-iotwireless-2.5.2.tar.gz` & `tmp/types-aiobotocore-iotwireless-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotwireless-2.5.2.tar", last modified: Sat Jul  8 01:43:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotwireless-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:28 2023, max compression
```

## Comparing `types-aiobotocore-iotwireless-2.5.2.tar` & `types-aiobotocore-iotwireless-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:48.790342 types-aiobotocore-iotwireless-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:00.000000 types-aiobotocore-iotwireless-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25602 2023-07-08 01:43:48.786342 types-aiobotocore-iotwireless-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24021 2023-07-08 01:33:00.000000 types-aiobotocore-iotwireless-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:48.790342 types-aiobotocore-iotwireless-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-08 01:33:00.000000 types-aiobotocore-iotwireless-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:48.786342 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-08 01:33:00.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-08 01:33:00.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-08 01:33:00.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    75909 2023-07-08 01:33:02.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    75791 2023-07-08 01:33:01.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-08 01:33:02.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-07-08 01:33:02.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:00.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97162 2023-07-08 01:33:04.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97073 2023-07-08 01:33:03.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:00.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:48.786342 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25602 2023-07-08 01:43:48.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:48.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:48.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:48.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:48.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:43:48.000000 types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.889556 types-aiobotocore-iotwireless-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-08-02 14:52:28.889556 types-aiobotocore-iotwireless-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24634 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:28.889556 types-aiobotocore-iotwireless-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.889556 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75886 2023-08-02 14:41:05.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75768 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-08-02 14:41:05.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-08-02 14:41:05.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   102175 2023-08-02 14:41:09.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102082 2023-08-02 14:41:08.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:04.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.889556 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-08-02 14:52:28.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:28.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:28.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:28.000000 types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotwireless-2.5.2/LICENSE` & `types-aiobotocore-iotwireless-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotwireless-2.5.2/PKG-INFO` & `types-aiobotocore-iotwireless-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotwireless
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTWireless 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTWireless 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotwireless type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotwireless type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotwireless"></a>
 
 # types-aiobotocore-iotwireless
 
 [![PyPI - types-aiobotocore-iotwireless](https://img.shields.io/pypi/v/types-aiobotocore-iotwireless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotwireless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotwireless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotwireless?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotwireless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotwireless)](https://pepy.tech/project/types-aiobotocore-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTWireless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [types-aiobotocore-iotwireless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -320,60 +319,52 @@
 )
 
 
 def check_value(value: ApplicationConfigTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotwireless.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotwireless.type_defs import (
     SessionKeysAbpV10XTypeDef,
     SessionKeysAbpV11TypeDef,
     AccuracyTypeDef,
     ApplicationConfigTypeDef,
     SidewalkAccountInfoTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     AssociateWirelessDeviceWithThingRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateRequestRequestTypeDef,
-    AssociateWirelessGatewayWithCertificateResponseTypeDef,
     AssociateWirelessGatewayWithThingRequestRequestTypeDef,
+    BeaconingOutputTypeDef,
     BeaconingTypeDef,
+    BlobTypeDef,
     CancelMulticastGroupSessionRequestRequestTypeDef,
     CdmaLocalIdTypeDef,
     CdmaNmrObjTypeDef,
     CertificateListTypeDef,
     LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
     LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
-    CreateDestinationResponseTypeDef,
     LoRaWANDeviceProfileTypeDef,
-    CreateDeviceProfileResponseTypeDef,
     LoRaWANFuotaTaskTypeDef,
-    CreateFuotaTaskResponseTypeDef,
     LoRaWANMulticastTypeDef,
-    CreateMulticastGroupResponseTypeDef,
     TraceContentTypeDef,
-    CreateNetworkAnalyzerConfigurationResponseTypeDef,
     LoRaWANServiceProfileTypeDef,
-    CreateServiceProfileResponseTypeDef,
     SidewalkCreateWirelessDeviceTypeDef,
-    CreateWirelessDeviceResponseTypeDef,
-    CreateWirelessGatewayResponseTypeDef,
-    CreateWirelessGatewayTaskDefinitionResponseTypeDef,
     CreateWirelessGatewayTaskRequestRequestTypeDef,
-    CreateWirelessGatewayTaskResponseTypeDef,
     DakCertificateMetadataTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteDeviceProfileRequestRequestTypeDef,
     DeleteFuotaTaskRequestRequestTypeDef,
     DeleteMulticastGroupRequestRequestTypeDef,
     DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef,
     DeleteQueuedMessagesRequestRequestTypeDef,
@@ -395,54 +386,48 @@
     DisassociateWirelessDeviceFromThingRequestRequestTypeDef,
     DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef,
     DisassociateWirelessGatewayFromThingRequestRequestTypeDef,
     PositioningTypeDef,
     FuotaTaskTypeDef,
     GatewayListItemTypeDef,
     GetDestinationRequestRequestTypeDef,
-    GetDestinationResponseTypeDef,
     GetDeviceProfileRequestRequestTypeDef,
+    LoRaWANDeviceProfileOutputTypeDef,
     GetFuotaTaskRequestRequestTypeDef,
     LoRaWANFuotaTaskGetInfoTypeDef,
     GetMulticastGroupRequestRequestTypeDef,
     LoRaWANMulticastGetTypeDef,
     GetMulticastGroupSessionRequestRequestTypeDef,
-    LoRaWANMulticastSessionTypeDef,
+    LoRaWANMulticastSessionOutputTypeDef,
     GetNetworkAnalyzerConfigurationRequestRequestTypeDef,
     GetPartnerAccountRequestRequestTypeDef,
     SidewalkAccountInfoWithFingerprintTypeDef,
     GetPositionConfigurationRequestRequestTypeDef,
     GnssTypeDef,
     IpTypeDef,
+    TimestampTypeDef,
     WiFiAccessPointTypeDef,
-    GetPositionEstimateResponseTypeDef,
     GetPositionRequestRequestTypeDef,
     GetResourceEventConfigurationRequestRequestTypeDef,
     GetResourceLogLevelRequestRequestTypeDef,
-    GetResourceLogLevelResponseTypeDef,
     GetResourcePositionRequestRequestTypeDef,
-    GetResourcePositionResponseTypeDef,
     GetServiceEndpointRequestRequestTypeDef,
-    GetServiceEndpointResponseTypeDef,
     GetServiceProfileRequestRequestTypeDef,
     LoRaWANGetServiceProfileInfoTypeDef,
     GetWirelessDeviceImportTaskRequestRequestTypeDef,
     SidewalkGetStartImportInfoTypeDef,
     GetWirelessDeviceRequestRequestTypeDef,
     GetWirelessDeviceStatisticsRequestRequestTypeDef,
     SidewalkDeviceMetadataTypeDef,
     GetWirelessGatewayCertificateRequestRequestTypeDef,
-    GetWirelessGatewayCertificateResponseTypeDef,
     GetWirelessGatewayFirmwareInformationRequestRequestTypeDef,
     GetWirelessGatewayRequestRequestTypeDef,
     GetWirelessGatewayStatisticsRequestRequestTypeDef,
-    GetWirelessGatewayStatisticsResponseTypeDef,
     GetWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskRequestRequestTypeDef,
-    GetWirelessGatewayTaskResponseTypeDef,
     GlobalIdentityTypeDef,
     GsmLocalIdTypeDef,
     ImportedSidewalkDeviceTypeDef,
     LoRaWANJoinEventNotificationConfigurationsTypeDef,
     LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     ListDestinationsRequestRequestTypeDef,
     ListDeviceProfilesRequestRequestTypeDef,
@@ -467,57 +452,75 @@
     ListWirelessGatewaysRequestRequestTypeDef,
     LoRaWANGatewayMetadataTypeDef,
     OtaaV10XTypeDef,
     OtaaV11TypeDef,
     LoRaWANGatewayVersionTypeDef,
     LoRaWANListDeviceTypeDef,
     LoRaWANMulticastMetadataTypeDef,
-    LoRaWANStartFuotaTaskTypeDef,
     UpdateAbpV10XTypeDef,
     UpdateAbpV11TypeDef,
     LteLocalIdTypeDef,
     LteNmrObjTypeDef,
     SemtechGnssConfigurationTypeDef,
     SemtechGnssDetailTypeDef,
     PutResourceLogLevelRequestRequestTypeDef,
     ResetResourceLogLevelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendDataToMulticastGroupResponseTypeDef,
-    SendDataToWirelessDeviceResponseTypeDef,
     SidewalkSendDataToDeviceTypeDef,
     SidewalkSingleStartImportInfoTypeDef,
     SidewalkStartImportInfoTypeDef,
     SidewalkUpdateAccountTypeDef,
     SidewalkUpdateImportInfoTypeDef,
-    StartSingleWirelessDeviceImportTaskResponseTypeDef,
-    StartWirelessDeviceImportTaskResponseTypeDef,
     TdscdmaLocalIdTypeDef,
     TdscdmaNmrObjTypeDef,
     TestWirelessDeviceRequestRequestTypeDef,
-    TestWirelessDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdatePositionRequestRequestTypeDef,
-    UpdateResourcePositionRequestRequestTypeDef,
     UpdateWirelessGatewayRequestRequestTypeDef,
     WcdmaLocalIdTypeDef,
     WcdmaNmrObjTypeDef,
     WirelessDeviceEventLogOptionTypeDef,
     WirelessGatewayEventLogOptionTypeDef,
     AbpV10XTypeDef,
     AbpV11TypeDef,
-    GetPositionResponseTypeDef,
-    AssociateAwsAccountWithPartnerAccountResponseTypeDef,
     AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    AssociateAwsAccountWithPartnerAccountResponseTypeDef,
+    AssociateWirelessGatewayWithCertificateResponseTypeDef,
+    CreateDestinationResponseTypeDef,
+    CreateDeviceProfileResponseTypeDef,
+    CreateFuotaTaskResponseTypeDef,
+    CreateMulticastGroupResponseTypeDef,
+    CreateNetworkAnalyzerConfigurationResponseTypeDef,
+    CreateServiceProfileResponseTypeDef,
+    CreateWirelessDeviceResponseTypeDef,
+    CreateWirelessGatewayResponseTypeDef,
+    CreateWirelessGatewayTaskDefinitionResponseTypeDef,
+    CreateWirelessGatewayTaskResponseTypeDef,
+    GetDestinationResponseTypeDef,
+    GetPositionEstimateResponseTypeDef,
+    GetPositionResponseTypeDef,
+    GetResourceLogLevelResponseTypeDef,
+    GetResourcePositionResponseTypeDef,
+    GetServiceEndpointResponseTypeDef,
+    GetWirelessGatewayCertificateResponseTypeDef,
+    GetWirelessGatewayStatisticsResponseTypeDef,
+    GetWirelessGatewayTaskResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SendDataToMulticastGroupResponseTypeDef,
+    SendDataToWirelessDeviceResponseTypeDef,
+    StartSingleWirelessDeviceImportTaskResponseTypeDef,
+    StartWirelessDeviceImportTaskResponseTypeDef,
+    TestWirelessDeviceResponseTypeDef,
+    LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
+    UpdateResourcePositionRequestRequestTypeDef,
     CdmaObjTypeDef,
     SidewalkDeviceTypeDef,
     SidewalkListDeviceTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDeviceProfileRequestRequestTypeDef,
     CreateFuotaTaskRequestRequestTypeDef,
@@ -533,24 +536,28 @@
     ListDeviceProfilesResponseTypeDef,
     DeviceRegistrationStateEventConfigurationTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     ProximityEventConfigurationTypeDef,
     DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     ProximityResourceTypeEventConfigurationTypeDef,
+    FPortsOutputTypeDef,
     FPortsTypeDef,
     UpdateFPortsTypeDef,
     ListFuotaTasksResponseTypeDef,
+    ParticipatingGatewaysOutputTypeDef,
     ParticipatingGatewaysTypeDef,
+    LoRaWANDeviceProfileUnionTypeDef,
     GetFuotaTaskResponseTypeDef,
     GetMulticastGroupResponseTypeDef,
     GetMulticastGroupSessionResponseTypeDef,
-    StartMulticastGroupSessionRequestRequestTypeDef,
     GetPartnerAccountResponseTypeDef,
     ListPartnerAccountsResponseTypeDef,
+    LoRaWANMulticastSessionTypeDef,
+    LoRaWANStartFuotaTaskTypeDef,
     GetServiceProfileResponseTypeDef,
     GetWirelessDeviceImportTaskResponseTypeDef,
     WirelessDeviceImportTaskTypeDef,
     GsmNmrObjTypeDef,
     ImportedWirelessDeviceTypeDef,
     JoinEventConfigurationTypeDef,
     JoinResourceTypeEventConfigurationTypeDef,
@@ -559,34 +566,41 @@
     ListNetworkAnalyzerConfigurationsResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     LoRaWANDeviceMetadataTypeDef,
     LoRaWANGatewayCurrentVersionTypeDef,
     LoRaWANUpdateGatewayTaskCreateTypeDef,
     LoRaWANUpdateGatewayTaskEntryTypeDef,
     MulticastWirelessMetadataTypeDef,
-    StartFuotaTaskRequestRequestTypeDef,
     LteObjTypeDef,
     PositionSolverConfigurationsTypeDef,
     PositionSolverDetailsTypeDef,
     StartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     StartWirelessDeviceImportTaskRequestRequestTypeDef,
     UpdatePartnerAccountRequestRequestTypeDef,
     UpdateWirelessDeviceImportTaskRequestRequestTypeDef,
     TdscdmaObjTypeDef,
     WcdmaObjTypeDef,
+    WirelessDeviceLogOptionOutputTypeDef,
     WirelessDeviceLogOptionTypeDef,
+    WirelessGatewayLogOptionOutputTypeDef,
     WirelessGatewayLogOptionTypeDef,
-    CreateWirelessGatewayRequestRequestTypeDef,
     GetWirelessGatewayResponseTypeDef,
     WirelessGatewayStatisticsTypeDef,
+    CreateWirelessGatewayRequestRequestTypeDef,
+    LoRaWANGatewayUnionTypeDef,
     WirelessDeviceStatisticsTypeDef,
     GetDeviceProfileResponseTypeDef,
+    LoRaWANDeviceOutputTypeDef,
     LoRaWANDeviceTypeDef,
     LoRaWANUpdateDeviceTypeDef,
+    LoRaWANSendDataToDeviceOutputTypeDef,
     LoRaWANSendDataToDeviceTypeDef,
+    LoRaWANMulticastSessionUnionTypeDef,
+    StartMulticastGroupSessionRequestRequestTypeDef,
+    StartFuotaTaskRequestRequestTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     GsmObjTypeDef,
     ListDevicesForWirelessDeviceImportTaskResponseTypeDef,
     EventNotificationItemConfigurationsTypeDef,
     GetResourceEventConfigurationResponseTypeDef,
     UpdateResourceEventConfigurationRequestRequestTypeDef,
     GetEventConfigurationByResourceTypesResponseTypeDef,
@@ -595,37 +609,40 @@
     GetWirelessGatewayFirmwareInformationResponseTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     UpdateWirelessGatewayTaskEntryTypeDef,
     SendDataToMulticastGroupRequestRequestTypeDef,
     PutPositionConfigurationRequestRequestTypeDef,
     GetPositionConfigurationResponseTypeDef,
     PositionConfigurationItemTypeDef,
+    WirelessDeviceLogOptionUnionTypeDef,
     GetLogLevelsByResourceTypesResponseTypeDef,
-    UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
+    WirelessGatewayLogOptionUnionTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
-    CreateWirelessDeviceRequestRequestTypeDef,
     GetWirelessDeviceResponseTypeDef,
+    CreateWirelessDeviceRequestRequestTypeDef,
+    LoRaWANDeviceUnionTypeDef,
     UpdateWirelessDeviceRequestRequestTypeDef,
     DownlinkQueueMessageTypeDef,
     WirelessMetadataTypeDef,
     CellTowersTypeDef,
     EventConfigurationItemTypeDef,
     CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskDefinitionResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
     ListPositionConfigurationsResponseTypeDef,
+    UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
     ListQueuedMessagesResponseTypeDef,
     SendDataToWirelessDeviceRequestRequestTypeDef,
     GetPositionEstimateRequestRequestTypeDef,
     ListEventConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> SessionKeysAbpV10XTypeDef:
+def get_value() -> SessionKeysAbpV10XTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotwireless-2.5.2/README.md` & `types-aiobotocore-iotwireless-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iotwireless"></a>
 
 # types-aiobotocore-iotwireless
 
 [![PyPI - types-aiobotocore-iotwireless](https://img.shields.io/pypi/v/types-aiobotocore-iotwireless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotwireless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotwireless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotwireless?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotwireless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotwireless)](https://pepy.tech/project/types-aiobotocore-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTWireless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [types-aiobotocore-iotwireless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,15 +40,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -287,60 +287,52 @@
 )
 
 
 def check_value(value: ApplicationConfigTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotwireless.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotwireless.type_defs import (
     SessionKeysAbpV10XTypeDef,
     SessionKeysAbpV11TypeDef,
     AccuracyTypeDef,
     ApplicationConfigTypeDef,
     SidewalkAccountInfoTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     AssociateWirelessDeviceWithThingRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateRequestRequestTypeDef,
-    AssociateWirelessGatewayWithCertificateResponseTypeDef,
     AssociateWirelessGatewayWithThingRequestRequestTypeDef,
+    BeaconingOutputTypeDef,
     BeaconingTypeDef,
+    BlobTypeDef,
     CancelMulticastGroupSessionRequestRequestTypeDef,
     CdmaLocalIdTypeDef,
     CdmaNmrObjTypeDef,
     CertificateListTypeDef,
     LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
     LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
-    CreateDestinationResponseTypeDef,
     LoRaWANDeviceProfileTypeDef,
-    CreateDeviceProfileResponseTypeDef,
     LoRaWANFuotaTaskTypeDef,
-    CreateFuotaTaskResponseTypeDef,
     LoRaWANMulticastTypeDef,
-    CreateMulticastGroupResponseTypeDef,
     TraceContentTypeDef,
-    CreateNetworkAnalyzerConfigurationResponseTypeDef,
     LoRaWANServiceProfileTypeDef,
-    CreateServiceProfileResponseTypeDef,
     SidewalkCreateWirelessDeviceTypeDef,
-    CreateWirelessDeviceResponseTypeDef,
-    CreateWirelessGatewayResponseTypeDef,
-    CreateWirelessGatewayTaskDefinitionResponseTypeDef,
     CreateWirelessGatewayTaskRequestRequestTypeDef,
-    CreateWirelessGatewayTaskResponseTypeDef,
     DakCertificateMetadataTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteDeviceProfileRequestRequestTypeDef,
     DeleteFuotaTaskRequestRequestTypeDef,
     DeleteMulticastGroupRequestRequestTypeDef,
     DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef,
     DeleteQueuedMessagesRequestRequestTypeDef,
@@ -362,54 +354,48 @@
     DisassociateWirelessDeviceFromThingRequestRequestTypeDef,
     DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef,
     DisassociateWirelessGatewayFromThingRequestRequestTypeDef,
     PositioningTypeDef,
     FuotaTaskTypeDef,
     GatewayListItemTypeDef,
     GetDestinationRequestRequestTypeDef,
-    GetDestinationResponseTypeDef,
     GetDeviceProfileRequestRequestTypeDef,
+    LoRaWANDeviceProfileOutputTypeDef,
     GetFuotaTaskRequestRequestTypeDef,
     LoRaWANFuotaTaskGetInfoTypeDef,
     GetMulticastGroupRequestRequestTypeDef,
     LoRaWANMulticastGetTypeDef,
     GetMulticastGroupSessionRequestRequestTypeDef,
-    LoRaWANMulticastSessionTypeDef,
+    LoRaWANMulticastSessionOutputTypeDef,
     GetNetworkAnalyzerConfigurationRequestRequestTypeDef,
     GetPartnerAccountRequestRequestTypeDef,
     SidewalkAccountInfoWithFingerprintTypeDef,
     GetPositionConfigurationRequestRequestTypeDef,
     GnssTypeDef,
     IpTypeDef,
+    TimestampTypeDef,
     WiFiAccessPointTypeDef,
-    GetPositionEstimateResponseTypeDef,
     GetPositionRequestRequestTypeDef,
     GetResourceEventConfigurationRequestRequestTypeDef,
     GetResourceLogLevelRequestRequestTypeDef,
-    GetResourceLogLevelResponseTypeDef,
     GetResourcePositionRequestRequestTypeDef,
-    GetResourcePositionResponseTypeDef,
     GetServiceEndpointRequestRequestTypeDef,
-    GetServiceEndpointResponseTypeDef,
     GetServiceProfileRequestRequestTypeDef,
     LoRaWANGetServiceProfileInfoTypeDef,
     GetWirelessDeviceImportTaskRequestRequestTypeDef,
     SidewalkGetStartImportInfoTypeDef,
     GetWirelessDeviceRequestRequestTypeDef,
     GetWirelessDeviceStatisticsRequestRequestTypeDef,
     SidewalkDeviceMetadataTypeDef,
     GetWirelessGatewayCertificateRequestRequestTypeDef,
-    GetWirelessGatewayCertificateResponseTypeDef,
     GetWirelessGatewayFirmwareInformationRequestRequestTypeDef,
     GetWirelessGatewayRequestRequestTypeDef,
     GetWirelessGatewayStatisticsRequestRequestTypeDef,
-    GetWirelessGatewayStatisticsResponseTypeDef,
     GetWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskRequestRequestTypeDef,
-    GetWirelessGatewayTaskResponseTypeDef,
     GlobalIdentityTypeDef,
     GsmLocalIdTypeDef,
     ImportedSidewalkDeviceTypeDef,
     LoRaWANJoinEventNotificationConfigurationsTypeDef,
     LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     ListDestinationsRequestRequestTypeDef,
     ListDeviceProfilesRequestRequestTypeDef,
@@ -434,57 +420,75 @@
     ListWirelessGatewaysRequestRequestTypeDef,
     LoRaWANGatewayMetadataTypeDef,
     OtaaV10XTypeDef,
     OtaaV11TypeDef,
     LoRaWANGatewayVersionTypeDef,
     LoRaWANListDeviceTypeDef,
     LoRaWANMulticastMetadataTypeDef,
-    LoRaWANStartFuotaTaskTypeDef,
     UpdateAbpV10XTypeDef,
     UpdateAbpV11TypeDef,
     LteLocalIdTypeDef,
     LteNmrObjTypeDef,
     SemtechGnssConfigurationTypeDef,
     SemtechGnssDetailTypeDef,
     PutResourceLogLevelRequestRequestTypeDef,
     ResetResourceLogLevelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendDataToMulticastGroupResponseTypeDef,
-    SendDataToWirelessDeviceResponseTypeDef,
     SidewalkSendDataToDeviceTypeDef,
     SidewalkSingleStartImportInfoTypeDef,
     SidewalkStartImportInfoTypeDef,
     SidewalkUpdateAccountTypeDef,
     SidewalkUpdateImportInfoTypeDef,
-    StartSingleWirelessDeviceImportTaskResponseTypeDef,
-    StartWirelessDeviceImportTaskResponseTypeDef,
     TdscdmaLocalIdTypeDef,
     TdscdmaNmrObjTypeDef,
     TestWirelessDeviceRequestRequestTypeDef,
-    TestWirelessDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdatePositionRequestRequestTypeDef,
-    UpdateResourcePositionRequestRequestTypeDef,
     UpdateWirelessGatewayRequestRequestTypeDef,
     WcdmaLocalIdTypeDef,
     WcdmaNmrObjTypeDef,
     WirelessDeviceEventLogOptionTypeDef,
     WirelessGatewayEventLogOptionTypeDef,
     AbpV10XTypeDef,
     AbpV11TypeDef,
-    GetPositionResponseTypeDef,
-    AssociateAwsAccountWithPartnerAccountResponseTypeDef,
     AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    AssociateAwsAccountWithPartnerAccountResponseTypeDef,
+    AssociateWirelessGatewayWithCertificateResponseTypeDef,
+    CreateDestinationResponseTypeDef,
+    CreateDeviceProfileResponseTypeDef,
+    CreateFuotaTaskResponseTypeDef,
+    CreateMulticastGroupResponseTypeDef,
+    CreateNetworkAnalyzerConfigurationResponseTypeDef,
+    CreateServiceProfileResponseTypeDef,
+    CreateWirelessDeviceResponseTypeDef,
+    CreateWirelessGatewayResponseTypeDef,
+    CreateWirelessGatewayTaskDefinitionResponseTypeDef,
+    CreateWirelessGatewayTaskResponseTypeDef,
+    GetDestinationResponseTypeDef,
+    GetPositionEstimateResponseTypeDef,
+    GetPositionResponseTypeDef,
+    GetResourceLogLevelResponseTypeDef,
+    GetResourcePositionResponseTypeDef,
+    GetServiceEndpointResponseTypeDef,
+    GetWirelessGatewayCertificateResponseTypeDef,
+    GetWirelessGatewayStatisticsResponseTypeDef,
+    GetWirelessGatewayTaskResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SendDataToMulticastGroupResponseTypeDef,
+    SendDataToWirelessDeviceResponseTypeDef,
+    StartSingleWirelessDeviceImportTaskResponseTypeDef,
+    StartWirelessDeviceImportTaskResponseTypeDef,
+    TestWirelessDeviceResponseTypeDef,
+    LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
+    UpdateResourcePositionRequestRequestTypeDef,
     CdmaObjTypeDef,
     SidewalkDeviceTypeDef,
     SidewalkListDeviceTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDeviceProfileRequestRequestTypeDef,
     CreateFuotaTaskRequestRequestTypeDef,
@@ -500,24 +504,28 @@
     ListDeviceProfilesResponseTypeDef,
     DeviceRegistrationStateEventConfigurationTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     ProximityEventConfigurationTypeDef,
     DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     ProximityResourceTypeEventConfigurationTypeDef,
+    FPortsOutputTypeDef,
     FPortsTypeDef,
     UpdateFPortsTypeDef,
     ListFuotaTasksResponseTypeDef,
+    ParticipatingGatewaysOutputTypeDef,
     ParticipatingGatewaysTypeDef,
+    LoRaWANDeviceProfileUnionTypeDef,
     GetFuotaTaskResponseTypeDef,
     GetMulticastGroupResponseTypeDef,
     GetMulticastGroupSessionResponseTypeDef,
-    StartMulticastGroupSessionRequestRequestTypeDef,
     GetPartnerAccountResponseTypeDef,
     ListPartnerAccountsResponseTypeDef,
+    LoRaWANMulticastSessionTypeDef,
+    LoRaWANStartFuotaTaskTypeDef,
     GetServiceProfileResponseTypeDef,
     GetWirelessDeviceImportTaskResponseTypeDef,
     WirelessDeviceImportTaskTypeDef,
     GsmNmrObjTypeDef,
     ImportedWirelessDeviceTypeDef,
     JoinEventConfigurationTypeDef,
     JoinResourceTypeEventConfigurationTypeDef,
@@ -526,34 +534,41 @@
     ListNetworkAnalyzerConfigurationsResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     LoRaWANDeviceMetadataTypeDef,
     LoRaWANGatewayCurrentVersionTypeDef,
     LoRaWANUpdateGatewayTaskCreateTypeDef,
     LoRaWANUpdateGatewayTaskEntryTypeDef,
     MulticastWirelessMetadataTypeDef,
-    StartFuotaTaskRequestRequestTypeDef,
     LteObjTypeDef,
     PositionSolverConfigurationsTypeDef,
     PositionSolverDetailsTypeDef,
     StartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     StartWirelessDeviceImportTaskRequestRequestTypeDef,
     UpdatePartnerAccountRequestRequestTypeDef,
     UpdateWirelessDeviceImportTaskRequestRequestTypeDef,
     TdscdmaObjTypeDef,
     WcdmaObjTypeDef,
+    WirelessDeviceLogOptionOutputTypeDef,
     WirelessDeviceLogOptionTypeDef,
+    WirelessGatewayLogOptionOutputTypeDef,
     WirelessGatewayLogOptionTypeDef,
-    CreateWirelessGatewayRequestRequestTypeDef,
     GetWirelessGatewayResponseTypeDef,
     WirelessGatewayStatisticsTypeDef,
+    CreateWirelessGatewayRequestRequestTypeDef,
+    LoRaWANGatewayUnionTypeDef,
     WirelessDeviceStatisticsTypeDef,
     GetDeviceProfileResponseTypeDef,
+    LoRaWANDeviceOutputTypeDef,
     LoRaWANDeviceTypeDef,
     LoRaWANUpdateDeviceTypeDef,
+    LoRaWANSendDataToDeviceOutputTypeDef,
     LoRaWANSendDataToDeviceTypeDef,
+    LoRaWANMulticastSessionUnionTypeDef,
+    StartMulticastGroupSessionRequestRequestTypeDef,
+    StartFuotaTaskRequestRequestTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     GsmObjTypeDef,
     ListDevicesForWirelessDeviceImportTaskResponseTypeDef,
     EventNotificationItemConfigurationsTypeDef,
     GetResourceEventConfigurationResponseTypeDef,
     UpdateResourceEventConfigurationRequestRequestTypeDef,
     GetEventConfigurationByResourceTypesResponseTypeDef,
@@ -562,37 +577,40 @@
     GetWirelessGatewayFirmwareInformationResponseTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     UpdateWirelessGatewayTaskEntryTypeDef,
     SendDataToMulticastGroupRequestRequestTypeDef,
     PutPositionConfigurationRequestRequestTypeDef,
     GetPositionConfigurationResponseTypeDef,
     PositionConfigurationItemTypeDef,
+    WirelessDeviceLogOptionUnionTypeDef,
     GetLogLevelsByResourceTypesResponseTypeDef,
-    UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
+    WirelessGatewayLogOptionUnionTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
-    CreateWirelessDeviceRequestRequestTypeDef,
     GetWirelessDeviceResponseTypeDef,
+    CreateWirelessDeviceRequestRequestTypeDef,
+    LoRaWANDeviceUnionTypeDef,
     UpdateWirelessDeviceRequestRequestTypeDef,
     DownlinkQueueMessageTypeDef,
     WirelessMetadataTypeDef,
     CellTowersTypeDef,
     EventConfigurationItemTypeDef,
     CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskDefinitionResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
     ListPositionConfigurationsResponseTypeDef,
+    UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
     ListQueuedMessagesResponseTypeDef,
     SendDataToWirelessDeviceRequestRequestTypeDef,
     GetPositionEstimateRequestRequestTypeDef,
     ListEventConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> SessionKeysAbpV10XTypeDef:
+def get_value() -> SessionKeysAbpV10XTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotwireless-2.5.2/setup.py` & `types-aiobotocore-iotwireless-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotwireless",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iotwireless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTWireless 2.5.2 service generated with"
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
-    keywords="aiobotocore iotwireless type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore iotwireless type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotwireless": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/"
```

### Comparing `types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/__main__.py` & `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTWireless 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IoTWireless 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless\nOther"
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

### Comparing `types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/client.py` & `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 
     session = get_session()
     async with session.create_client("iotwireless") as client:
         client: IoTWirelessClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     DeviceProfileTypeType,
     EventNotificationResourceTypeType,
     ExpressionTypeType,
     IdentifierTypeType,
@@ -35,14 +33,15 @@
     WirelessDeviceTypeType,
     WirelessGatewayIdTypeType,
     WirelessGatewayServiceTypeType,
 )
 from .type_defs import (
     AssociateAwsAccountWithPartnerAccountResponseTypeDef,
     AssociateWirelessGatewayWithCertificateResponseTypeDef,
+    BlobTypeDef,
     CellTowersTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDestinationResponseTypeDef,
     CreateDeviceProfileResponseTypeDef,
     CreateFuotaTaskResponseTypeDef,
     CreateMulticastGroupResponseTypeDef,
@@ -97,19 +96,19 @@
     ListQueuedMessagesResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
-    LoRaWANDeviceProfileTypeDef,
-    LoRaWANDeviceTypeDef,
+    LoRaWANDeviceProfileUnionTypeDef,
+    LoRaWANDeviceUnionTypeDef,
     LoRaWANFuotaTaskTypeDef,
-    LoRaWANGatewayTypeDef,
-    LoRaWANMulticastSessionTypeDef,
+    LoRaWANGatewayUnionTypeDef,
+    LoRaWANMulticastSessionUnionTypeDef,
     LoRaWANMulticastTypeDef,
     LoRaWANServiceProfileTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     LoRaWANUpdateDeviceTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     MulticastWirelessMetadataTypeDef,
@@ -124,19 +123,20 @@
     SidewalkStartImportInfoTypeDef,
     SidewalkUpdateAccountTypeDef,
     SidewalkUpdateImportInfoTypeDef,
     StartSingleWirelessDeviceImportTaskResponseTypeDef,
     StartWirelessDeviceImportTaskResponseTypeDef,
     TagTypeDef,
     TestWirelessDeviceResponseTypeDef,
+    TimestampTypeDef,
     TraceContentTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     WiFiAccessPointTypeDef,
-    WirelessDeviceLogOptionTypeDef,
-    WirelessGatewayLogOptionTypeDef,
+    WirelessDeviceLogOptionUnionTypeDef,
+    WirelessGatewayLogOptionUnionTypeDef,
     WirelessMetadataTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -297,15 +297,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_destination)
         """
 
     async def create_device_profile(
         self,
         *,
         Name: str = ...,
-        LoRaWAN: LoRaWANDeviceProfileTypeDef = ...,
+        LoRaWAN: LoRaWANDeviceProfileUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         Sidewalk: Mapping[str, Any] = ...
     ) -> CreateDeviceProfileResponseTypeDef:
         """
         Creates a new device profile.
 
@@ -388,30 +388,30 @@
         self,
         *,
         Type: WirelessDeviceTypeType,
         DestinationName: str,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        LoRaWAN: LoRaWANDeviceTypeDef = ...,
+        LoRaWAN: LoRaWANDeviceUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Positioning: PositioningConfigStatusType = ...,
         Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...
     ) -> CreateWirelessDeviceResponseTypeDef:
         """
         Provisions a wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_wireless_device)
         """
 
     async def create_wireless_gateway(
         self,
         *,
-        LoRaWAN: LoRaWANGatewayTypeDef,
+        LoRaWAN: LoRaWANGatewayUnionTypeDef,
         Name: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateWirelessGatewayResponseTypeDef:
         """
         Provisions a wireless gateway.
@@ -737,15 +737,15 @@
     async def get_position_estimate(
         self,
         *,
         WiFiAccessPoints: Sequence[WiFiAccessPointTypeDef] = ...,
         CellTowers: CellTowersTypeDef = ...,
         Ip: IpTypeDef = ...,
         Gnss: GnssTypeDef = ...,
-        Timestamp: Union[datetime, str] = ...
+        Timestamp: TimestampTypeDef = ...
     ) -> GetPositionEstimateResponseTypeDef:
         """
         Get estimated position information as a payload in GeoJSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_position_estimate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#get_position_estimate)
         """
@@ -1199,15 +1199,15 @@
         Starts a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_fuota_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#start_fuota_task)
         """
 
     async def start_multicast_group_session(
-        self, *, Id: str, LoRaWAN: LoRaWANMulticastSessionTypeDef
+        self, *, Id: str, LoRaWAN: LoRaWANMulticastSessionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Starts a multicast group session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_multicast_group_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#start_multicast_group_session)
         """
@@ -1320,16 +1320,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_fuota_task)
         """
 
     async def update_log_levels_by_resource_types(
         self,
         *,
         DefaultLogLevel: LogLevelType = ...,
-        WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionTypeDef] = ...,
-        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionTypeDef] = ...
+        WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionUnionTypeDef] = ...,
+        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Set default log level, or log levels by resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_log_levels_by_resource_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_log_levels_by_resource_types)
         """
@@ -1417,15 +1417,15 @@
         """
 
     async def update_resource_position(
         self,
         *,
         ResourceIdentifier: str,
         ResourceType: PositionResourceTypeType,
-        GeoJsonPayload: Union[str, bytes, IO[Any], StreamingBody] = ...
+        GeoJsonPayload: BlobTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Update the position information of a given wireless device or a wireless gateway
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_resource_position)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_resource_position)
```

### Comparing `types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/client.pyi` & `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,17 @@
 
     session = get_session()
     async with session.create_client("iotwireless") as client:
         client: IoTWirelessClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     DeviceProfileTypeType,
     EventNotificationResourceTypeType,
     ExpressionTypeType,
     IdentifierTypeType,
@@ -35,14 +33,15 @@
     WirelessDeviceTypeType,
     WirelessGatewayIdTypeType,
     WirelessGatewayServiceTypeType,
 )
 from .type_defs import (
     AssociateAwsAccountWithPartnerAccountResponseTypeDef,
     AssociateWirelessGatewayWithCertificateResponseTypeDef,
+    BlobTypeDef,
     CellTowersTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDestinationResponseTypeDef,
     CreateDeviceProfileResponseTypeDef,
     CreateFuotaTaskResponseTypeDef,
     CreateMulticastGroupResponseTypeDef,
@@ -97,19 +96,19 @@
     ListQueuedMessagesResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
-    LoRaWANDeviceProfileTypeDef,
-    LoRaWANDeviceTypeDef,
+    LoRaWANDeviceProfileUnionTypeDef,
+    LoRaWANDeviceUnionTypeDef,
     LoRaWANFuotaTaskTypeDef,
-    LoRaWANGatewayTypeDef,
-    LoRaWANMulticastSessionTypeDef,
+    LoRaWANGatewayUnionTypeDef,
+    LoRaWANMulticastSessionUnionTypeDef,
     LoRaWANMulticastTypeDef,
     LoRaWANServiceProfileTypeDef,
     LoRaWANStartFuotaTaskTypeDef,
     LoRaWANUpdateDeviceTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     MulticastWirelessMetadataTypeDef,
@@ -124,19 +123,20 @@
     SidewalkStartImportInfoTypeDef,
     SidewalkUpdateAccountTypeDef,
     SidewalkUpdateImportInfoTypeDef,
     StartSingleWirelessDeviceImportTaskResponseTypeDef,
     StartWirelessDeviceImportTaskResponseTypeDef,
     TagTypeDef,
     TestWirelessDeviceResponseTypeDef,
+    TimestampTypeDef,
     TraceContentTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     WiFiAccessPointTypeDef,
-    WirelessDeviceLogOptionTypeDef,
-    WirelessGatewayLogOptionTypeDef,
+    WirelessDeviceLogOptionUnionTypeDef,
+    WirelessGatewayLogOptionUnionTypeDef,
     WirelessMetadataTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -281,15 +281,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_destination)
         """
     async def create_device_profile(
         self,
         *,
         Name: str = ...,
-        LoRaWAN: LoRaWANDeviceProfileTypeDef = ...,
+        LoRaWAN: LoRaWANDeviceProfileUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         Sidewalk: Mapping[str, Any] = ...
     ) -> CreateDeviceProfileResponseTypeDef:
         """
         Creates a new device profile.
 
@@ -367,29 +367,29 @@
         self,
         *,
         Type: WirelessDeviceTypeType,
         DestinationName: str,
         Name: str = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        LoRaWAN: LoRaWANDeviceTypeDef = ...,
+        LoRaWAN: LoRaWANDeviceUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Positioning: PositioningConfigStatusType = ...,
         Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...
     ) -> CreateWirelessDeviceResponseTypeDef:
         """
         Provisions a wireless device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#create_wireless_device)
         """
     async def create_wireless_gateway(
         self,
         *,
-        LoRaWAN: LoRaWANGatewayTypeDef,
+        LoRaWAN: LoRaWANGatewayUnionTypeDef,
         Name: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateWirelessGatewayResponseTypeDef:
         """
         Provisions a wireless gateway.
@@ -680,15 +680,15 @@
     async def get_position_estimate(
         self,
         *,
         WiFiAccessPoints: Sequence[WiFiAccessPointTypeDef] = ...,
         CellTowers: CellTowersTypeDef = ...,
         Ip: IpTypeDef = ...,
         Gnss: GnssTypeDef = ...,
-        Timestamp: Union[datetime, str] = ...
+        Timestamp: TimestampTypeDef = ...
     ) -> GetPositionEstimateResponseTypeDef:
         """
         Get estimated position information as a payload in GeoJSON format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_position_estimate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#get_position_estimate)
         """
@@ -1101,15 +1101,15 @@
         """
         Starts a FUOTA task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_fuota_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#start_fuota_task)
         """
     async def start_multicast_group_session(
-        self, *, Id: str, LoRaWAN: LoRaWANMulticastSessionTypeDef
+        self, *, Id: str, LoRaWAN: LoRaWANMulticastSessionUnionTypeDef
     ) -> Dict[str, Any]:
         """
         Starts a multicast group session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_multicast_group_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#start_multicast_group_session)
         """
@@ -1213,16 +1213,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_fuota_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_fuota_task)
         """
     async def update_log_levels_by_resource_types(
         self,
         *,
         DefaultLogLevel: LogLevelType = ...,
-        WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionTypeDef] = ...,
-        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionTypeDef] = ...
+        WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionUnionTypeDef] = ...,
+        WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Set default log level, or log levels by resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_log_levels_by_resource_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_log_levels_by_resource_types)
         """
@@ -1304,15 +1304,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_resource_event_configuration)
         """
     async def update_resource_position(
         self,
         *,
         ResourceIdentifier: str,
         ResourceType: PositionResourceTypeType,
-        GeoJsonPayload: Union[str, bytes, IO[Any], StreamingBody] = ...
+        GeoJsonPayload: BlobTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Update the position information of a given wireless device or a wireless gateway
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_resource_position)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/client/#update_resource_position)
```

### Comparing `types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/literals.py` & `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/literals.pyi` & `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/type_defs.py` & `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iotwireless.type_defs import SessionKeysAbpV10XTypeDef
 
-    data: SessionKeysAbpV10XTypeDef = {...}
+    data: SessionKeysAbpV10XTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -66,45 +66,37 @@
 __all__ = (
     "SessionKeysAbpV10XTypeDef",
     "SessionKeysAbpV11TypeDef",
     "AccuracyTypeDef",
     "ApplicationConfigTypeDef",
     "SidewalkAccountInfoTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "AssociateWirelessDeviceWithThingRequestRequestTypeDef",
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
-    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
+    "BeaconingOutputTypeDef",
     "BeaconingTypeDef",
+    "BlobTypeDef",
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     "CdmaLocalIdTypeDef",
     "CdmaNmrObjTypeDef",
     "CertificateListTypeDef",
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
-    "CreateDestinationResponseTypeDef",
     "LoRaWANDeviceProfileTypeDef",
-    "CreateDeviceProfileResponseTypeDef",
     "LoRaWANFuotaTaskTypeDef",
-    "CreateFuotaTaskResponseTypeDef",
     "LoRaWANMulticastTypeDef",
-    "CreateMulticastGroupResponseTypeDef",
     "TraceContentTypeDef",
-    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
     "LoRaWANServiceProfileTypeDef",
-    "CreateServiceProfileResponseTypeDef",
     "SidewalkCreateWirelessDeviceTypeDef",
-    "CreateWirelessDeviceResponseTypeDef",
-    "CreateWirelessGatewayResponseTypeDef",
-    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
     "CreateWirelessGatewayTaskRequestRequestTypeDef",
-    "CreateWirelessGatewayTaskResponseTypeDef",
     "DakCertificateMetadataTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteDeviceProfileRequestRequestTypeDef",
     "DeleteFuotaTaskRequestRequestTypeDef",
     "DeleteMulticastGroupRequestRequestTypeDef",
     "DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "DeleteQueuedMessagesRequestRequestTypeDef",
@@ -126,54 +118,48 @@
     "DisassociateWirelessDeviceFromThingRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromThingRequestRequestTypeDef",
     "PositioningTypeDef",
     "FuotaTaskTypeDef",
     "GatewayListItemTypeDef",
     "GetDestinationRequestRequestTypeDef",
-    "GetDestinationResponseTypeDef",
     "GetDeviceProfileRequestRequestTypeDef",
+    "LoRaWANDeviceProfileOutputTypeDef",
     "GetFuotaTaskRequestRequestTypeDef",
     "LoRaWANFuotaTaskGetInfoTypeDef",
     "GetMulticastGroupRequestRequestTypeDef",
     "LoRaWANMulticastGetTypeDef",
     "GetMulticastGroupSessionRequestRequestTypeDef",
-    "LoRaWANMulticastSessionTypeDef",
+    "LoRaWANMulticastSessionOutputTypeDef",
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "GetPartnerAccountRequestRequestTypeDef",
     "SidewalkAccountInfoWithFingerprintTypeDef",
     "GetPositionConfigurationRequestRequestTypeDef",
     "GnssTypeDef",
     "IpTypeDef",
+    "TimestampTypeDef",
     "WiFiAccessPointTypeDef",
-    "GetPositionEstimateResponseTypeDef",
     "GetPositionRequestRequestTypeDef",
     "GetResourceEventConfigurationRequestRequestTypeDef",
     "GetResourceLogLevelRequestRequestTypeDef",
-    "GetResourceLogLevelResponseTypeDef",
     "GetResourcePositionRequestRequestTypeDef",
-    "GetResourcePositionResponseTypeDef",
     "GetServiceEndpointRequestRequestTypeDef",
-    "GetServiceEndpointResponseTypeDef",
     "GetServiceProfileRequestRequestTypeDef",
     "LoRaWANGetServiceProfileInfoTypeDef",
     "GetWirelessDeviceImportTaskRequestRequestTypeDef",
     "SidewalkGetStartImportInfoTypeDef",
     "GetWirelessDeviceRequestRequestTypeDef",
     "GetWirelessDeviceStatisticsRequestRequestTypeDef",
     "SidewalkDeviceMetadataTypeDef",
     "GetWirelessGatewayCertificateRequestRequestTypeDef",
-    "GetWirelessGatewayCertificateResponseTypeDef",
     "GetWirelessGatewayFirmwareInformationRequestRequestTypeDef",
     "GetWirelessGatewayRequestRequestTypeDef",
     "GetWirelessGatewayStatisticsRequestRequestTypeDef",
-    "GetWirelessGatewayStatisticsResponseTypeDef",
     "GetWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskRequestRequestTypeDef",
-    "GetWirelessGatewayTaskResponseTypeDef",
     "GlobalIdentityTypeDef",
     "GsmLocalIdTypeDef",
     "ImportedSidewalkDeviceTypeDef",
     "LoRaWANJoinEventNotificationConfigurationsTypeDef",
     "LoRaWANJoinResourceTypeEventConfigurationTypeDef",
     "ListDestinationsRequestRequestTypeDef",
     "ListDeviceProfilesRequestRequestTypeDef",
@@ -198,57 +184,75 @@
     "ListWirelessGatewaysRequestRequestTypeDef",
     "LoRaWANGatewayMetadataTypeDef",
     "OtaaV10XTypeDef",
     "OtaaV11TypeDef",
     "LoRaWANGatewayVersionTypeDef",
     "LoRaWANListDeviceTypeDef",
     "LoRaWANMulticastMetadataTypeDef",
-    "LoRaWANStartFuotaTaskTypeDef",
     "UpdateAbpV10XTypeDef",
     "UpdateAbpV11TypeDef",
     "LteLocalIdTypeDef",
     "LteNmrObjTypeDef",
     "SemtechGnssConfigurationTypeDef",
     "SemtechGnssDetailTypeDef",
     "PutResourceLogLevelRequestRequestTypeDef",
     "ResetResourceLogLevelRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SendDataToMulticastGroupResponseTypeDef",
-    "SendDataToWirelessDeviceResponseTypeDef",
     "SidewalkSendDataToDeviceTypeDef",
     "SidewalkSingleStartImportInfoTypeDef",
     "SidewalkStartImportInfoTypeDef",
     "SidewalkUpdateAccountTypeDef",
     "SidewalkUpdateImportInfoTypeDef",
-    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
-    "StartWirelessDeviceImportTaskResponseTypeDef",
     "TdscdmaLocalIdTypeDef",
     "TdscdmaNmrObjTypeDef",
     "TestWirelessDeviceRequestRequestTypeDef",
-    "TestWirelessDeviceResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
     "UpdatePositionRequestRequestTypeDef",
-    "UpdateResourcePositionRequestRequestTypeDef",
     "UpdateWirelessGatewayRequestRequestTypeDef",
     "WcdmaLocalIdTypeDef",
     "WcdmaNmrObjTypeDef",
     "WirelessDeviceEventLogOptionTypeDef",
     "WirelessGatewayEventLogOptionTypeDef",
     "AbpV10XTypeDef",
     "AbpV11TypeDef",
-    "GetPositionResponseTypeDef",
-    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
     "AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef",
     "CreateDestinationRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
+    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
+    "CreateDestinationResponseTypeDef",
+    "CreateDeviceProfileResponseTypeDef",
+    "CreateFuotaTaskResponseTypeDef",
+    "CreateMulticastGroupResponseTypeDef",
+    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
+    "CreateServiceProfileResponseTypeDef",
+    "CreateWirelessDeviceResponseTypeDef",
+    "CreateWirelessGatewayResponseTypeDef",
+    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
+    "CreateWirelessGatewayTaskResponseTypeDef",
+    "GetDestinationResponseTypeDef",
+    "GetPositionEstimateResponseTypeDef",
+    "GetPositionResponseTypeDef",
+    "GetResourceLogLevelResponseTypeDef",
+    "GetResourcePositionResponseTypeDef",
+    "GetServiceEndpointResponseTypeDef",
+    "GetWirelessGatewayCertificateResponseTypeDef",
+    "GetWirelessGatewayStatisticsResponseTypeDef",
+    "GetWirelessGatewayTaskResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SendDataToMulticastGroupResponseTypeDef",
+    "SendDataToWirelessDeviceResponseTypeDef",
+    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
+    "StartWirelessDeviceImportTaskResponseTypeDef",
+    "TestWirelessDeviceResponseTypeDef",
+    "LoRaWANGatewayOutputTypeDef",
     "LoRaWANGatewayTypeDef",
+    "UpdateResourcePositionRequestRequestTypeDef",
     "CdmaObjTypeDef",
     "SidewalkDeviceTypeDef",
     "SidewalkListDeviceTypeDef",
     "ConnectionStatusEventConfigurationTypeDef",
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
     "CreateDeviceProfileRequestRequestTypeDef",
     "CreateFuotaTaskRequestRequestTypeDef",
@@ -264,24 +268,28 @@
     "ListDeviceProfilesResponseTypeDef",
     "DeviceRegistrationStateEventConfigurationTypeDef",
     "MessageDeliveryStatusEventConfigurationTypeDef",
     "ProximityEventConfigurationTypeDef",
     "DeviceRegistrationStateResourceTypeEventConfigurationTypeDef",
     "MessageDeliveryStatusResourceTypeEventConfigurationTypeDef",
     "ProximityResourceTypeEventConfigurationTypeDef",
+    "FPortsOutputTypeDef",
     "FPortsTypeDef",
     "UpdateFPortsTypeDef",
     "ListFuotaTasksResponseTypeDef",
+    "ParticipatingGatewaysOutputTypeDef",
     "ParticipatingGatewaysTypeDef",
+    "LoRaWANDeviceProfileUnionTypeDef",
     "GetFuotaTaskResponseTypeDef",
     "GetMulticastGroupResponseTypeDef",
     "GetMulticastGroupSessionResponseTypeDef",
-    "StartMulticastGroupSessionRequestRequestTypeDef",
     "GetPartnerAccountResponseTypeDef",
     "ListPartnerAccountsResponseTypeDef",
+    "LoRaWANMulticastSessionTypeDef",
+    "LoRaWANStartFuotaTaskTypeDef",
     "GetServiceProfileResponseTypeDef",
     "GetWirelessDeviceImportTaskResponseTypeDef",
     "WirelessDeviceImportTaskTypeDef",
     "GsmNmrObjTypeDef",
     "ImportedWirelessDeviceTypeDef",
     "JoinEventConfigurationTypeDef",
     "JoinResourceTypeEventConfigurationTypeDef",
@@ -290,34 +298,41 @@
     "ListNetworkAnalyzerConfigurationsResponseTypeDef",
     "ListServiceProfilesResponseTypeDef",
     "LoRaWANDeviceMetadataTypeDef",
     "LoRaWANGatewayCurrentVersionTypeDef",
     "LoRaWANUpdateGatewayTaskCreateTypeDef",
     "LoRaWANUpdateGatewayTaskEntryTypeDef",
     "MulticastWirelessMetadataTypeDef",
-    "StartFuotaTaskRequestRequestTypeDef",
     "LteObjTypeDef",
     "PositionSolverConfigurationsTypeDef",
     "PositionSolverDetailsTypeDef",
     "StartSingleWirelessDeviceImportTaskRequestRequestTypeDef",
     "StartWirelessDeviceImportTaskRequestRequestTypeDef",
     "UpdatePartnerAccountRequestRequestTypeDef",
     "UpdateWirelessDeviceImportTaskRequestRequestTypeDef",
     "TdscdmaObjTypeDef",
     "WcdmaObjTypeDef",
+    "WirelessDeviceLogOptionOutputTypeDef",
     "WirelessDeviceLogOptionTypeDef",
+    "WirelessGatewayLogOptionOutputTypeDef",
     "WirelessGatewayLogOptionTypeDef",
-    "CreateWirelessGatewayRequestRequestTypeDef",
     "GetWirelessGatewayResponseTypeDef",
     "WirelessGatewayStatisticsTypeDef",
+    "CreateWirelessGatewayRequestRequestTypeDef",
+    "LoRaWANGatewayUnionTypeDef",
     "WirelessDeviceStatisticsTypeDef",
     "GetDeviceProfileResponseTypeDef",
+    "LoRaWANDeviceOutputTypeDef",
     "LoRaWANDeviceTypeDef",
     "LoRaWANUpdateDeviceTypeDef",
+    "LoRaWANSendDataToDeviceOutputTypeDef",
     "LoRaWANSendDataToDeviceTypeDef",
+    "LoRaWANMulticastSessionUnionTypeDef",
+    "StartMulticastGroupSessionRequestRequestTypeDef",
+    "StartFuotaTaskRequestRequestTypeDef",
     "ListWirelessDeviceImportTasksResponseTypeDef",
     "GsmObjTypeDef",
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     "EventNotificationItemConfigurationsTypeDef",
     "GetResourceEventConfigurationResponseTypeDef",
     "UpdateResourceEventConfigurationRequestRequestTypeDef",
     "GetEventConfigurationByResourceTypesResponseTypeDef",
@@ -326,29 +341,32 @@
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
     "UpdateWirelessGatewayTaskCreateTypeDef",
     "UpdateWirelessGatewayTaskEntryTypeDef",
     "SendDataToMulticastGroupRequestRequestTypeDef",
     "PutPositionConfigurationRequestRequestTypeDef",
     "GetPositionConfigurationResponseTypeDef",
     "PositionConfigurationItemTypeDef",
+    "WirelessDeviceLogOptionUnionTypeDef",
     "GetLogLevelsByResourceTypesResponseTypeDef",
-    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
+    "WirelessGatewayLogOptionUnionTypeDef",
     "ListWirelessGatewaysResponseTypeDef",
     "ListWirelessDevicesResponseTypeDef",
-    "CreateWirelessDeviceRequestRequestTypeDef",
     "GetWirelessDeviceResponseTypeDef",
+    "CreateWirelessDeviceRequestRequestTypeDef",
+    "LoRaWANDeviceUnionTypeDef",
     "UpdateWirelessDeviceRequestRequestTypeDef",
     "DownlinkQueueMessageTypeDef",
     "WirelessMetadataTypeDef",
     "CellTowersTypeDef",
     "EventConfigurationItemTypeDef",
     "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
     "ListPositionConfigurationsResponseTypeDef",
+    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     "ListQueuedMessagesResponseTypeDef",
     "SendDataToWirelessDeviceRequestRequestTypeDef",
     "GetPositionEstimateRequestRequestTypeDef",
     "ListEventConfigurationsResponseTypeDef",
 )
 
 SessionKeysAbpV10XTypeDef = TypedDict(
@@ -403,14 +421,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef = TypedDict(
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
         "MulticastGroupId": str,
     },
 )
@@ -443,39 +472,41 @@
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
     {
         "Id": str,
         "IotCertificateId": str,
     },
 )
 
-AssociateWirelessGatewayWithCertificateResponseTypeDef = TypedDict(
-    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
-    {
-        "IotCertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateWirelessGatewayWithThingRequestRequestTypeDef = TypedDict(
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
     {
         "Id": str,
         "ThingArn": str,
     },
 )
 
+BeaconingOutputTypeDef = TypedDict(
+    "BeaconingOutputTypeDef",
+    {
+        "DataRate": int,
+        "Frequencies": List[int],
+    },
+    total=False,
+)
+
 BeaconingTypeDef = TypedDict(
     "BeaconingTypeDef",
     {
         "DataRate": int,
         "Frequencies": Sequence[int],
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelMulticastGroupSessionRequestRequestTypeDef = TypedDict(
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -528,23 +559,14 @@
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
     {
         "WirelessGatewayEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-CreateDestinationResponseTypeDef = TypedDict(
-    "CreateDestinationResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANDeviceProfileTypeDef = TypedDict(
     "LoRaWANDeviceProfileTypeDef",
     {
         "SupportsClassB": bool,
         "ClassBTimeout": int,
         "PingSlotPeriod": int,
         "PingSlotDr": int,
@@ -563,150 +585,69 @@
         "RfRegion": str,
         "SupportsJoin": bool,
         "Supports32BitFCnt": bool,
     },
     total=False,
 )
 
-CreateDeviceProfileResponseTypeDef = TypedDict(
-    "CreateDeviceProfileResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANFuotaTaskTypeDef = TypedDict(
     "LoRaWANFuotaTaskTypeDef",
     {
         "RfRegion": SupportedRfRegionType,
     },
     total=False,
 )
 
-CreateFuotaTaskResponseTypeDef = TypedDict(
-    "CreateFuotaTaskResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANMulticastTypeDef = TypedDict(
     "LoRaWANMulticastTypeDef",
     {
         "RfRegion": SupportedRfRegionType,
         "DlClass": DlClassType,
     },
     total=False,
 )
 
-CreateMulticastGroupResponseTypeDef = TypedDict(
-    "CreateMulticastGroupResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TraceContentTypeDef = TypedDict(
     "TraceContentTypeDef",
     {
         "WirelessDeviceFrameInfo": WirelessDeviceFrameInfoType,
         "LogLevel": LogLevelType,
         "MulticastFrameInfo": MulticastFrameInfoType,
     },
     total=False,
 )
 
-CreateNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
-    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANServiceProfileTypeDef = TypedDict(
     "LoRaWANServiceProfileTypeDef",
     {
         "AddGwMetadata": bool,
         "DrMin": int,
         "DrMax": int,
         "PrAllowed": bool,
         "RaAllowed": bool,
     },
     total=False,
 )
 
-CreateServiceProfileResponseTypeDef = TypedDict(
-    "CreateServiceProfileResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SidewalkCreateWirelessDeviceTypeDef = TypedDict(
     "SidewalkCreateWirelessDeviceTypeDef",
     {
         "DeviceProfileId": str,
     },
     total=False,
 )
 
-CreateWirelessDeviceResponseTypeDef = TypedDict(
-    "CreateWirelessDeviceResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWirelessGatewayResponseTypeDef = TypedDict(
-    "CreateWirelessGatewayResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
-    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateWirelessGatewayTaskRequestRequestTypeDef = TypedDict(
     "CreateWirelessGatewayTaskRequestRequestTypeDef",
     {
         "Id": str,
         "WirelessGatewayTaskDefinitionId": str,
     },
 )
 
-CreateWirelessGatewayTaskResponseTypeDef = TypedDict(
-    "CreateWirelessGatewayTaskResponseTypeDef",
-    {
-        "WirelessGatewayTaskDefinitionId": str,
-        "Status": WirelessGatewayTaskStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDakCertificateMetadataTypeDef = TypedDict(
     "_RequiredDakCertificateMetadataTypeDef",
     {
         "CertificateId": str,
     },
 )
 _OptionalDakCertificateMetadataTypeDef = TypedDict(
@@ -972,32 +913,45 @@
 GetDestinationRequestRequestTypeDef = TypedDict(
     "GetDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-GetDestinationResponseTypeDef = TypedDict(
-    "GetDestinationResponseTypeDef",
+GetDeviceProfileRequestRequestTypeDef = TypedDict(
+    "GetDeviceProfileRequestRequestTypeDef",
     {
-        "Arn": str,
-        "Name": str,
-        "Expression": str,
-        "ExpressionType": ExpressionTypeType,
-        "Description": str,
-        "RoleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Id": str,
     },
 )
 
-GetDeviceProfileRequestRequestTypeDef = TypedDict(
-    "GetDeviceProfileRequestRequestTypeDef",
+LoRaWANDeviceProfileOutputTypeDef = TypedDict(
+    "LoRaWANDeviceProfileOutputTypeDef",
     {
-        "Id": str,
+        "SupportsClassB": bool,
+        "ClassBTimeout": int,
+        "PingSlotPeriod": int,
+        "PingSlotDr": int,
+        "PingSlotFreq": int,
+        "SupportsClassC": bool,
+        "ClassCTimeout": int,
+        "MacVersion": str,
+        "RegParamsRevision": str,
+        "RxDelay1": int,
+        "RxDrOffset1": int,
+        "RxDataRate2": int,
+        "RxFreq2": int,
+        "FactoryPresetFreqsList": List[int],
+        "MaxEirp": int,
+        "MaxDutyCycle": int,
+        "RfRegion": str,
+        "SupportsJoin": bool,
+        "Supports32BitFCnt": bool,
     },
+    total=False,
 )
 
 GetFuotaTaskRequestRequestTypeDef = TypedDict(
     "GetFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
@@ -1033,16 +987,16 @@
 GetMulticastGroupSessionRequestRequestTypeDef = TypedDict(
     "GetMulticastGroupSessionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-LoRaWANMulticastSessionTypeDef = TypedDict(
-    "LoRaWANMulticastSessionTypeDef",
+LoRaWANMulticastSessionOutputTypeDef = TypedDict(
+    "LoRaWANMulticastSessionOutputTypeDef",
     {
         "DlDr": int,
         "DlFreq": int,
         "SessionStartTime": datetime,
         "SessionTimeout": int,
         "PingSlotPeriod": int,
     },
@@ -1108,30 +1062,23 @@
 IpTypeDef = TypedDict(
     "IpTypeDef",
     {
         "IpAddress": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 WiFiAccessPointTypeDef = TypedDict(
     "WiFiAccessPointTypeDef",
     {
         "MacAddress": str,
         "Rss": int,
     },
 )
 
-GetPositionEstimateResponseTypeDef = TypedDict(
-    "GetPositionEstimateResponseTypeDef",
-    {
-        "GeoJsonPayload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPositionRequestRequestTypeDef = TypedDict(
     "GetPositionRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
     },
 )
@@ -1163,56 +1110,30 @@
     "GetResourceLogLevelRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": str,
     },
 )
 
-GetResourceLogLevelResponseTypeDef = TypedDict(
-    "GetResourceLogLevelResponseTypeDef",
-    {
-        "LogLevel": LogLevelType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourcePositionRequestRequestTypeDef = TypedDict(
     "GetResourcePositionRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
     },
 )
 
-GetResourcePositionResponseTypeDef = TypedDict(
-    "GetResourcePositionResponseTypeDef",
-    {
-        "GeoJsonPayload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceEndpointRequestRequestTypeDef = TypedDict(
     "GetServiceEndpointRequestRequestTypeDef",
     {
         "ServiceType": WirelessGatewayServiceTypeType,
     },
     total=False,
 )
 
-GetServiceEndpointResponseTypeDef = TypedDict(
-    "GetServiceEndpointResponseTypeDef",
-    {
-        "ServiceType": WirelessGatewayServiceTypeType,
-        "ServiceEndpoint": str,
-        "ServerTrust": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceProfileRequestRequestTypeDef = TypedDict(
     "GetServiceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1287,23 +1208,14 @@
 GetWirelessGatewayCertificateRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayCertificateRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetWirelessGatewayCertificateResponseTypeDef = TypedDict(
-    "GetWirelessGatewayCertificateResponseTypeDef",
-    {
-        "IotCertificateId": str,
-        "LoRaWANNetworkServerCertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWirelessGatewayFirmwareInformationRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayFirmwareInformationRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1318,50 +1230,28 @@
 GetWirelessGatewayStatisticsRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayStatisticsRequestRequestTypeDef",
     {
         "WirelessGatewayId": str,
     },
 )
 
-GetWirelessGatewayStatisticsResponseTypeDef = TypedDict(
-    "GetWirelessGatewayStatisticsResponseTypeDef",
-    {
-        "WirelessGatewayId": str,
-        "LastUplinkReceivedAt": str,
-        "ConnectionStatus": ConnectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWirelessGatewayTaskDefinitionRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
 GetWirelessGatewayTaskRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetWirelessGatewayTaskResponseTypeDef = TypedDict(
-    "GetWirelessGatewayTaskResponseTypeDef",
-    {
-        "WirelessGatewayId": str,
-        "WirelessGatewayTaskDefinitionId": str,
-        "LastUplinkReceivedAt": str,
-        "TaskCreatedAt": str,
-        "Status": WirelessGatewayTaskStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GlobalIdentityTypeDef = TypedDict(
     "GlobalIdentityTypeDef",
     {
         "Lac": int,
         "GeranCid": int,
     },
 )
@@ -1708,22 +1598,14 @@
     "LoRaWANMulticastMetadataTypeDef",
     {
         "FPort": int,
     },
     total=False,
 )
 
-LoRaWANStartFuotaTaskTypeDef = TypedDict(
-    "LoRaWANStartFuotaTaskTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 UpdateAbpV10XTypeDef = TypedDict(
     "UpdateAbpV10XTypeDef",
     {
         "FCntStart": int,
     },
     total=False,
 )
@@ -1798,41 +1680,14 @@
     "ResetResourceLogLevelRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": str,
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
-SendDataToMulticastGroupResponseTypeDef = TypedDict(
-    "SendDataToMulticastGroupResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SendDataToWirelessDeviceResponseTypeDef = TypedDict(
-    "SendDataToWirelessDeviceResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SidewalkSendDataToDeviceTypeDef = TypedDict(
     "SidewalkSendDataToDeviceTypeDef",
     {
         "Seq": int,
         "MessageType": MessageTypeType,
         "AckModeRetryDurationSecs": int,
     },
@@ -1868,32 +1723,14 @@
     "SidewalkUpdateImportInfoTypeDef",
     {
         "DeviceCreationFile": str,
     },
     total=False,
 )
 
-StartSingleWirelessDeviceImportTaskResponseTypeDef = TypedDict(
-    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartWirelessDeviceImportTaskResponseTypeDef = TypedDict(
-    "StartWirelessDeviceImportTaskResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TdscdmaLocalIdTypeDef = TypedDict(
     "TdscdmaLocalIdTypeDef",
     {
         "Uarfcn": int,
         "CellParams": int,
     },
 )
@@ -1923,22 +1760,14 @@
 TestWirelessDeviceRequestRequestTypeDef = TypedDict(
     "TestWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-TestWirelessDeviceResponseTypeDef = TypedDict(
-    "TestWirelessDeviceResponseTypeDef",
-    {
-        "Result": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1972,37 +1801,14 @@
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
         "Position": Sequence[float],
     },
 )
 
-_RequiredUpdateResourcePositionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateResourcePositionRequestRequestTypeDef",
-    {
-        "ResourceIdentifier": str,
-        "ResourceType": PositionResourceTypeType,
-    },
-)
-_OptionalUpdateResourcePositionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateResourcePositionRequestRequestTypeDef",
-    {
-        "GeoJsonPayload": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-
-class UpdateResourcePositionRequestRequestTypeDef(
-    _RequiredUpdateResourcePositionRequestRequestTypeDef,
-    _OptionalUpdateResourcePositionRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredUpdateWirelessGatewayRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessGatewayRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessGatewayRequestRequestTypeDef = TypedDict(
@@ -2087,36 +1893,14 @@
         "DevAddr": str,
         "SessionKeys": SessionKeysAbpV11TypeDef,
         "FCntStart": int,
     },
     total=False,
 )
 
-GetPositionResponseTypeDef = TypedDict(
-    "GetPositionResponseTypeDef",
-    {
-        "Position": List[float],
-        "Accuracy": AccuracyTypeDef,
-        "SolverType": Literal["GNSS"],
-        "SolverProvider": Literal["Semtech"],
-        "SolverVersion": str,
-        "Timestamp": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AssociateAwsAccountWithPartnerAccountResponseTypeDef = TypedDict(
-    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
-    {
-        "Sidewalk": SidewalkAccountInfoTypeDef,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoTypeDef,
     },
 )
 _OptionalAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = TypedDict(
@@ -2158,22 +1942,14 @@
 
 class CreateDestinationRequestRequestTypeDef(
     _RequiredCreateDestinationRequestRequestTypeDef, _OptionalCreateDestinationRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2220,28 +1996,313 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+AssociateAwsAccountWithPartnerAccountResponseTypeDef = TypedDict(
+    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
+    {
+        "Sidewalk": SidewalkAccountInfoTypeDef,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateWirelessGatewayWithCertificateResponseTypeDef = TypedDict(
+    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
+    {
+        "IotCertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDestinationResponseTypeDef = TypedDict(
+    "CreateDestinationResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeviceProfileResponseTypeDef = TypedDict(
+    "CreateDeviceProfileResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFuotaTaskResponseTypeDef = TypedDict(
+    "CreateFuotaTaskResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMulticastGroupResponseTypeDef = TypedDict(
+    "CreateMulticastGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
+    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateServiceProfileResponseTypeDef = TypedDict(
+    "CreateServiceProfileResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessDeviceResponseTypeDef = TypedDict(
+    "CreateWirelessDeviceResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessGatewayResponseTypeDef = TypedDict(
+    "CreateWirelessGatewayResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
+    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessGatewayTaskResponseTypeDef = TypedDict(
+    "CreateWirelessGatewayTaskResponseTypeDef",
+    {
+        "WirelessGatewayTaskDefinitionId": str,
+        "Status": WirelessGatewayTaskStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDestinationResponseTypeDef = TypedDict(
+    "GetDestinationResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Expression": str,
+        "ExpressionType": ExpressionTypeType,
+        "Description": str,
+        "RoleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPositionEstimateResponseTypeDef = TypedDict(
+    "GetPositionEstimateResponseTypeDef",
+    {
+        "GeoJsonPayload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPositionResponseTypeDef = TypedDict(
+    "GetPositionResponseTypeDef",
+    {
+        "Position": List[float],
+        "Accuracy": AccuracyTypeDef,
+        "SolverType": Literal["GNSS"],
+        "SolverProvider": Literal["Semtech"],
+        "SolverVersion": str,
+        "Timestamp": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourceLogLevelResponseTypeDef = TypedDict(
+    "GetResourceLogLevelResponseTypeDef",
+    {
+        "LogLevel": LogLevelType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePositionResponseTypeDef = TypedDict(
+    "GetResourcePositionResponseTypeDef",
+    {
+        "GeoJsonPayload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceEndpointResponseTypeDef = TypedDict(
+    "GetServiceEndpointResponseTypeDef",
+    {
+        "ServiceType": WirelessGatewayServiceTypeType,
+        "ServiceEndpoint": str,
+        "ServerTrust": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessGatewayCertificateResponseTypeDef = TypedDict(
+    "GetWirelessGatewayCertificateResponseTypeDef",
+    {
+        "IotCertificateId": str,
+        "LoRaWANNetworkServerCertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessGatewayStatisticsResponseTypeDef = TypedDict(
+    "GetWirelessGatewayStatisticsResponseTypeDef",
+    {
+        "WirelessGatewayId": str,
+        "LastUplinkReceivedAt": str,
+        "ConnectionStatus": ConnectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessGatewayTaskResponseTypeDef = TypedDict(
+    "GetWirelessGatewayTaskResponseTypeDef",
+    {
+        "WirelessGatewayId": str,
+        "WirelessGatewayTaskDefinitionId": str,
+        "LastUplinkReceivedAt": str,
+        "TaskCreatedAt": str,
+        "Status": WirelessGatewayTaskStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendDataToMulticastGroupResponseTypeDef = TypedDict(
+    "SendDataToMulticastGroupResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendDataToWirelessDeviceResponseTypeDef = TypedDict(
+    "SendDataToWirelessDeviceResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSingleWirelessDeviceImportTaskResponseTypeDef = TypedDict(
+    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartWirelessDeviceImportTaskResponseTypeDef = TypedDict(
+    "StartWirelessDeviceImportTaskResponseTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestWirelessDeviceResponseTypeDef = TypedDict(
+    "TestWirelessDeviceResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoRaWANGatewayOutputTypeDef = TypedDict(
+    "LoRaWANGatewayOutputTypeDef",
+    {
+        "GatewayEui": str,
+        "RfRegion": str,
+        "JoinEuiFilters": List[List[str]],
+        "NetIdFilters": List[str],
+        "SubBands": List[int],
+        "Beaconing": BeaconingOutputTypeDef,
+        "MaxEirp": float,
+    },
+    total=False,
+)
+
 LoRaWANGatewayTypeDef = TypedDict(
     "LoRaWANGatewayTypeDef",
     {
         "GatewayEui": str,
         "RfRegion": str,
         "JoinEuiFilters": Sequence[Sequence[str]],
         "NetIdFilters": Sequence[str],
         "SubBands": Sequence[int],
         "Beaconing": BeaconingTypeDef,
         "MaxEirp": float,
     },
     total=False,
 )
 
+_RequiredUpdateResourcePositionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateResourcePositionRequestRequestTypeDef",
+    {
+        "ResourceIdentifier": str,
+        "ResourceType": PositionResourceTypeType,
+    },
+)
+_OptionalUpdateResourcePositionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateResourcePositionRequestRequestTypeDef",
+    {
+        "GeoJsonPayload": BlobTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateResourcePositionRequestRequestTypeDef(
+    _RequiredUpdateResourcePositionRequestRequestTypeDef,
+    _OptionalUpdateResourcePositionRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCdmaObjTypeDef = TypedDict(
     "_RequiredCdmaObjTypeDef",
     {
         "SystemId": int,
         "NetworkId": int,
         "BaseStationId": int,
     },
@@ -2461,15 +2522,15 @@
         "TraceContent": TraceContentTypeDef,
         "WirelessDevices": List[str],
         "WirelessGateways": List[str],
         "Description": str,
         "Arn": str,
         "Name": str,
         "MulticastGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "ConfigurationName": str,
@@ -2520,24 +2581,24 @@
 )
 
 ListDestinationsResponseTypeDef = TypedDict(
     "ListDestinationsResponseTypeDef",
     {
         "NextToken": str,
         "DestinationList": List[DestinationsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeviceProfilesResponseTypeDef = TypedDict(
     "ListDeviceProfilesResponseTypeDef",
     {
         "NextToken": str,
         "DeviceProfileList": List[DeviceProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceRegistrationStateEventConfigurationTypeDef = TypedDict(
     "DeviceRegistrationStateEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkEventNotificationConfigurationsTypeDef,
@@ -2584,14 +2645,26 @@
     "ProximityResourceTypeEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
 
+FPortsOutputTypeDef = TypedDict(
+    "FPortsOutputTypeDef",
+    {
+        "Fuota": int,
+        "Multicast": int,
+        "ClockSync": int,
+        "Positioning": PositioningTypeDef,
+        "Applications": List[ApplicationConfigTypeDef],
+    },
+    total=False,
+)
+
 FPortsTypeDef = TypedDict(
     "FPortsTypeDef",
     {
         "Fuota": int,
         "Multicast": int,
         "ClockSync": int,
         "Positioning": PositioningTypeDef,
@@ -2610,27 +2683,39 @@
 )
 
 ListFuotaTasksResponseTypeDef = TypedDict(
     "ListFuotaTasksResponseTypeDef",
     {
         "NextToken": str,
         "FuotaTaskList": List[FuotaTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ParticipatingGatewaysOutputTypeDef = TypedDict(
+    "ParticipatingGatewaysOutputTypeDef",
+    {
+        "DownlinkMode": DownlinkModeType,
+        "GatewayList": List[GatewayListItemTypeDef],
+        "TransmissionInterval": int,
     },
 )
 
 ParticipatingGatewaysTypeDef = TypedDict(
     "ParticipatingGatewaysTypeDef",
     {
         "DownlinkMode": DownlinkModeType,
-        "GatewayList": List[GatewayListItemTypeDef],
+        "GatewayList": Sequence[GatewayListItemTypeDef],
         "TransmissionInterval": int,
     },
 )
 
+LoRaWANDeviceProfileUnionTypeDef = Union[
+    LoRaWANDeviceProfileTypeDef, LoRaWANDeviceProfileOutputTypeDef
+]
 GetFuotaTaskResponseTypeDef = TypedDict(
     "GetFuotaTaskResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Status": FuotaTaskStatusType,
         "Name": str,
@@ -2638,74 +2723,86 @@
         "LoRaWAN": LoRaWANFuotaTaskGetInfoTypeDef,
         "FirmwareUpdateImage": str,
         "FirmwareUpdateRole": str,
         "CreatedAt": datetime,
         "RedundancyPercent": int,
         "FragmentSizeBytes": int,
         "FragmentIntervalMS": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMulticastGroupResponseTypeDef = TypedDict(
     "GetMulticastGroupResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "Status": str,
         "LoRaWAN": LoRaWANMulticastGetTypeDef,
         "CreatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMulticastGroupSessionResponseTypeDef = TypedDict(
     "GetMulticastGroupSessionResponseTypeDef",
     {
-        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
-    "StartMulticastGroupSessionRequestRequestTypeDef",
-    {
-        "Id": str,
-        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+        "LoRaWAN": LoRaWANMulticastSessionOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPartnerAccountResponseTypeDef = TypedDict(
     "GetPartnerAccountResponseTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoWithFingerprintTypeDef,
         "AccountLinked": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPartnerAccountsResponseTypeDef = TypedDict(
     "ListPartnerAccountsResponseTypeDef",
     {
         "NextToken": str,
         "Sidewalk": List[SidewalkAccountInfoWithFingerprintTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoRaWANMulticastSessionTypeDef = TypedDict(
+    "LoRaWANMulticastSessionTypeDef",
+    {
+        "DlDr": int,
+        "DlFreq": int,
+        "SessionStartTime": TimestampTypeDef,
+        "SessionTimeout": int,
+        "PingSlotPeriod": int,
+    },
+    total=False,
+)
+
+LoRaWANStartFuotaTaskTypeDef = TypedDict(
+    "LoRaWANStartFuotaTaskTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 GetServiceProfileResponseTypeDef = TypedDict(
     "GetServiceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
         "LoRaWAN": LoRaWANGetServiceProfileInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWirelessDeviceImportTaskResponseTypeDef = TypedDict(
     "GetWirelessDeviceImportTaskResponseTypeDef",
     {
         "Id": str,
@@ -2715,15 +2812,15 @@
         "CreationTime": datetime,
         "Status": ImportTaskStatusType,
         "StatusReason": str,
         "InitializedImportedDeviceCount": int,
         "PendingImportedDeviceCount": int,
         "OnboardedImportedDeviceCount": int,
         "FailedImportedDeviceCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WirelessDeviceImportTaskTypeDef = TypedDict(
     "WirelessDeviceImportTaskTypeDef",
     {
         "Id": str,
@@ -2788,42 +2885,42 @@
 )
 
 ListMulticastGroupsByFuotaTaskResponseTypeDef = TypedDict(
     "ListMulticastGroupsByFuotaTaskResponseTypeDef",
     {
         "NextToken": str,
         "MulticastGroupList": List[MulticastGroupByFuotaTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMulticastGroupsResponseTypeDef = TypedDict(
     "ListMulticastGroupsResponseTypeDef",
     {
         "NextToken": str,
         "MulticastGroupList": List[MulticastGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworkAnalyzerConfigurationsResponseTypeDef = TypedDict(
     "ListNetworkAnalyzerConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "NetworkAnalyzerConfigurationList": List[NetworkAnalyzerConfigurationsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceProfilesResponseTypeDef = TypedDict(
     "ListServiceProfilesResponseTypeDef",
     {
         "NextToken": str,
         "ServiceProfileList": List[ServiceProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoRaWANDeviceMetadataTypeDef = TypedDict(
     "LoRaWANDeviceMetadataTypeDef",
     {
         "DevEui": str,
@@ -2868,35 +2965,14 @@
     "MulticastWirelessMetadataTypeDef",
     {
         "LoRaWAN": LoRaWANMulticastMetadataTypeDef,
     },
     total=False,
 )
 
-_RequiredStartFuotaTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFuotaTaskRequestRequestTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalStartFuotaTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFuotaTaskRequestRequestTypeDef",
-    {
-        "LoRaWAN": LoRaWANStartFuotaTaskTypeDef,
-    },
-    total=False,
-)
-
-
-class StartFuotaTaskRequestRequestTypeDef(
-    _RequiredStartFuotaTaskRequestRequestTypeDef, _OptionalStartFuotaTaskRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredLteObjTypeDef = TypedDict(
     "_RequiredLteObjTypeDef",
     {
         "Mcc": int,
         "Mnc": int,
         "EutranCid": int,
     },
@@ -3049,110 +3125,155 @@
 )
 
 
 class WcdmaObjTypeDef(_RequiredWcdmaObjTypeDef, _OptionalWcdmaObjTypeDef):
     pass
 
 
+_RequiredWirelessDeviceLogOptionOutputTypeDef = TypedDict(
+    "_RequiredWirelessDeviceLogOptionOutputTypeDef",
+    {
+        "Type": WirelessDeviceTypeType,
+        "LogLevel": LogLevelType,
+    },
+)
+_OptionalWirelessDeviceLogOptionOutputTypeDef = TypedDict(
+    "_OptionalWirelessDeviceLogOptionOutputTypeDef",
+    {
+        "Events": List[WirelessDeviceEventLogOptionTypeDef],
+    },
+    total=False,
+)
+
+
+class WirelessDeviceLogOptionOutputTypeDef(
+    _RequiredWirelessDeviceLogOptionOutputTypeDef, _OptionalWirelessDeviceLogOptionOutputTypeDef
+):
+    pass
+
+
 _RequiredWirelessDeviceLogOptionTypeDef = TypedDict(
     "_RequiredWirelessDeviceLogOptionTypeDef",
     {
         "Type": WirelessDeviceTypeType,
         "LogLevel": LogLevelType,
     },
 )
 _OptionalWirelessDeviceLogOptionTypeDef = TypedDict(
     "_OptionalWirelessDeviceLogOptionTypeDef",
     {
-        "Events": List[WirelessDeviceEventLogOptionTypeDef],
+        "Events": Sequence[WirelessDeviceEventLogOptionTypeDef],
     },
     total=False,
 )
 
 
 class WirelessDeviceLogOptionTypeDef(
     _RequiredWirelessDeviceLogOptionTypeDef, _OptionalWirelessDeviceLogOptionTypeDef
 ):
     pass
 
 
-_RequiredWirelessGatewayLogOptionTypeDef = TypedDict(
-    "_RequiredWirelessGatewayLogOptionTypeDef",
+_RequiredWirelessGatewayLogOptionOutputTypeDef = TypedDict(
+    "_RequiredWirelessGatewayLogOptionOutputTypeDef",
     {
         "Type": Literal["LoRaWAN"],
         "LogLevel": LogLevelType,
     },
 )
-_OptionalWirelessGatewayLogOptionTypeDef = TypedDict(
-    "_OptionalWirelessGatewayLogOptionTypeDef",
+_OptionalWirelessGatewayLogOptionOutputTypeDef = TypedDict(
+    "_OptionalWirelessGatewayLogOptionOutputTypeDef",
     {
         "Events": List[WirelessGatewayEventLogOptionTypeDef],
     },
     total=False,
 )
 
 
-class WirelessGatewayLogOptionTypeDef(
-    _RequiredWirelessGatewayLogOptionTypeDef, _OptionalWirelessGatewayLogOptionTypeDef
+class WirelessGatewayLogOptionOutputTypeDef(
+    _RequiredWirelessGatewayLogOptionOutputTypeDef, _OptionalWirelessGatewayLogOptionOutputTypeDef
 ):
     pass
 
 
-_RequiredCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWirelessGatewayRequestRequestTypeDef",
+_RequiredWirelessGatewayLogOptionTypeDef = TypedDict(
+    "_RequiredWirelessGatewayLogOptionTypeDef",
     {
-        "LoRaWAN": LoRaWANGatewayTypeDef,
+        "Type": Literal["LoRaWAN"],
+        "LogLevel": LogLevelType,
     },
 )
-_OptionalCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWirelessGatewayRequestRequestTypeDef",
+_OptionalWirelessGatewayLogOptionTypeDef = TypedDict(
+    "_OptionalWirelessGatewayLogOptionTypeDef",
     {
-        "Name": str,
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-        "ClientRequestToken": str,
+        "Events": Sequence[WirelessGatewayEventLogOptionTypeDef],
     },
     total=False,
 )
 
 
-class CreateWirelessGatewayRequestRequestTypeDef(
-    _RequiredCreateWirelessGatewayRequestRequestTypeDef,
-    _OptionalCreateWirelessGatewayRequestRequestTypeDef,
+class WirelessGatewayLogOptionTypeDef(
+    _RequiredWirelessGatewayLogOptionTypeDef, _OptionalWirelessGatewayLogOptionTypeDef
 ):
     pass
 
 
 GetWirelessGatewayResponseTypeDef = TypedDict(
     "GetWirelessGatewayResponseTypeDef",
     {
         "Name": str,
         "Id": str,
         "Description": str,
-        "LoRaWAN": LoRaWANGatewayTypeDef,
+        "LoRaWAN": LoRaWANGatewayOutputTypeDef,
         "Arn": str,
         "ThingName": str,
         "ThingArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WirelessGatewayStatisticsTypeDef = TypedDict(
     "WirelessGatewayStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
-        "LoRaWAN": LoRaWANGatewayTypeDef,
+        "LoRaWAN": LoRaWANGatewayOutputTypeDef,
         "LastUplinkReceivedAt": str,
     },
     total=False,
 )
 
+_RequiredCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWirelessGatewayRequestRequestTypeDef",
+    {
+        "LoRaWAN": LoRaWANGatewayTypeDef,
+    },
+)
+_OptionalCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWirelessGatewayRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class CreateWirelessGatewayRequestRequestTypeDef(
+    _RequiredCreateWirelessGatewayRequestRequestTypeDef,
+    _OptionalCreateWirelessGatewayRequestRequestTypeDef,
+):
+    pass
+
+
+LoRaWANGatewayUnionTypeDef = Union[LoRaWANGatewayTypeDef, LoRaWANGatewayOutputTypeDef]
 WirelessDeviceStatisticsTypeDef = TypedDict(
     "WirelessDeviceStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Type": WirelessDeviceTypeType,
         "Name": str,
@@ -3169,20 +3290,35 @@
 
 GetDeviceProfileResponseTypeDef = TypedDict(
     "GetDeviceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
-        "LoRaWAN": LoRaWANDeviceProfileTypeDef,
+        "LoRaWAN": LoRaWANDeviceProfileOutputTypeDef,
         "Sidewalk": SidewalkGetDeviceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoRaWANDeviceOutputTypeDef = TypedDict(
+    "LoRaWANDeviceOutputTypeDef",
+    {
+        "DevEui": str,
+        "DeviceProfileId": str,
+        "ServiceProfileId": str,
+        "OtaaV1_1": OtaaV11TypeDef,
+        "OtaaV1_0_x": OtaaV10XTypeDef,
+        "AbpV1_1": AbpV11TypeDef,
+        "AbpV1_0_x": AbpV10XTypeDef,
+        "FPorts": FPortsOutputTypeDef,
+    },
+    total=False,
+)
+
 LoRaWANDeviceTypeDef = TypedDict(
     "LoRaWANDeviceTypeDef",
     {
         "DevEui": str,
         "DeviceProfileId": str,
         "ServiceProfileId": str,
         "OtaaV1_1": OtaaV11TypeDef,
@@ -3202,29 +3338,70 @@
         "AbpV1_1": UpdateAbpV11TypeDef,
         "AbpV1_0_x": UpdateAbpV10XTypeDef,
         "FPorts": UpdateFPortsTypeDef,
     },
     total=False,
 )
 
+LoRaWANSendDataToDeviceOutputTypeDef = TypedDict(
+    "LoRaWANSendDataToDeviceOutputTypeDef",
+    {
+        "FPort": int,
+        "ParticipatingGateways": ParticipatingGatewaysOutputTypeDef,
+    },
+    total=False,
+)
+
 LoRaWANSendDataToDeviceTypeDef = TypedDict(
     "LoRaWANSendDataToDeviceTypeDef",
     {
         "FPort": int,
         "ParticipatingGateways": ParticipatingGatewaysTypeDef,
     },
     total=False,
 )
 
+LoRaWANMulticastSessionUnionTypeDef = Union[
+    LoRaWANMulticastSessionTypeDef, LoRaWANMulticastSessionOutputTypeDef
+]
+StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
+    "StartMulticastGroupSessionRequestRequestTypeDef",
+    {
+        "Id": str,
+        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+    },
+)
+
+_RequiredStartFuotaTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFuotaTaskRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalStartFuotaTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFuotaTaskRequestRequestTypeDef",
+    {
+        "LoRaWAN": LoRaWANStartFuotaTaskTypeDef,
+    },
+    total=False,
+)
+
+
+class StartFuotaTaskRequestRequestTypeDef(
+    _RequiredStartFuotaTaskRequestRequestTypeDef, _OptionalStartFuotaTaskRequestRequestTypeDef
+):
+    pass
+
+
 ListWirelessDeviceImportTasksResponseTypeDef = TypedDict(
     "ListWirelessDeviceImportTasksResponseTypeDef",
     {
         "NextToken": str,
         "WirelessDeviceImportTaskList": List[WirelessDeviceImportTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGsmObjTypeDef = TypedDict(
     "_RequiredGsmObjTypeDef",
     {
         "Mcc": int,
@@ -3251,15 +3428,15 @@
 
 ListDevicesForWirelessDeviceImportTaskResponseTypeDef = TypedDict(
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     {
         "NextToken": str,
         "DestinationName": str,
         "ImportedWirelessDeviceList": List[ImportedWirelessDeviceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventNotificationItemConfigurationsTypeDef = TypedDict(
     "EventNotificationItemConfigurationsTypeDef",
     {
         "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationTypeDef,
@@ -3275,15 +3452,15 @@
     "GetResourceEventConfigurationResponseTypeDef",
     {
         "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationTypeDef,
         "Proximity": ProximityEventConfigurationTypeDef,
         "Join": JoinEventConfigurationTypeDef,
         "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
         "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateResourceEventConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceEventConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
@@ -3315,15 +3492,15 @@
     "GetEventConfigurationByResourceTypesResponseTypeDef",
     {
         "DeviceRegistrationState": DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
         "Proximity": ProximityResourceTypeEventConfigurationTypeDef,
         "Join": JoinResourceTypeEventConfigurationTypeDef,
         "ConnectionStatus": ConnectionStatusResourceTypeEventConfigurationTypeDef,
         "MessageDeliveryStatus": MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventConfigurationByResourceTypesRequestRequestTypeDef = TypedDict(
     "UpdateEventConfigurationByResourceTypesRequestRequestTypeDef",
     {
         "DeviceRegistrationState": DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
@@ -3338,23 +3515,23 @@
 GetWirelessDeviceStatisticsResponseTypeDef = TypedDict(
     "GetWirelessDeviceStatisticsResponseTypeDef",
     {
         "WirelessDeviceId": str,
         "LastUplinkReceivedAt": str,
         "LoRaWAN": LoRaWANDeviceMetadataTypeDef,
         "Sidewalk": SidewalkDeviceMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWirelessGatewayFirmwareInformationResponseTypeDef = TypedDict(
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
     {
         "LoRaWAN": LoRaWANGatewayCurrentVersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWirelessGatewayTaskCreateTypeDef = TypedDict(
     "UpdateWirelessGatewayTaskCreateTypeDef",
     {
         "UpdateDataSource": str,
@@ -3408,64 +3585,78 @@
 
 
 GetPositionConfigurationResponseTypeDef = TypedDict(
     "GetPositionConfigurationResponseTypeDef",
     {
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PositionConfigurationItemTypeDef = TypedDict(
     "PositionConfigurationItemTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
     },
     total=False,
 )
 
+WirelessDeviceLogOptionUnionTypeDef = Union[
+    WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef
+]
 GetLogLevelsByResourceTypesResponseTypeDef = TypedDict(
     "GetLogLevelsByResourceTypesResponseTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
-        "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionTypeDef],
-        "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
-    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
-    {
-        "DefaultLogLevel": LogLevelType,
-        "WirelessDeviceLogOptions": Sequence[WirelessDeviceLogOptionTypeDef],
-        "WirelessGatewayLogOptions": Sequence[WirelessGatewayLogOptionTypeDef],
+        "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionOutputTypeDef],
+        "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+WirelessGatewayLogOptionUnionTypeDef = Union[
+    WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef
+]
 ListWirelessGatewaysResponseTypeDef = TypedDict(
     "ListWirelessGatewaysResponseTypeDef",
     {
         "NextToken": str,
         "WirelessGatewayList": List[WirelessGatewayStatisticsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWirelessDevicesResponseTypeDef = TypedDict(
     "ListWirelessDevicesResponseTypeDef",
     {
         "NextToken": str,
         "WirelessDeviceList": List[WirelessDeviceStatisticsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessDeviceResponseTypeDef = TypedDict(
+    "GetWirelessDeviceResponseTypeDef",
+    {
+        "Type": WirelessDeviceTypeType,
+        "Name": str,
+        "Description": str,
+        "DestinationName": str,
+        "Id": str,
+        "Arn": str,
+        "ThingName": str,
+        "ThingArn": str,
+        "LoRaWAN": LoRaWANDeviceOutputTypeDef,
+        "Sidewalk": SidewalkDeviceTypeDef,
+        "Positioning": PositioningConfigStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWirelessDeviceRequestRequestTypeDef",
     {
         "Type": WirelessDeviceTypeType,
@@ -3490,32 +3681,15 @@
 class CreateWirelessDeviceRequestRequestTypeDef(
     _RequiredCreateWirelessDeviceRequestRequestTypeDef,
     _OptionalCreateWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
 
-GetWirelessDeviceResponseTypeDef = TypedDict(
-    "GetWirelessDeviceResponseTypeDef",
-    {
-        "Type": WirelessDeviceTypeType,
-        "Name": str,
-        "Description": str,
-        "DestinationName": str,
-        "Id": str,
-        "Arn": str,
-        "ThingName": str,
-        "ThingArn": str,
-        "LoRaWAN": LoRaWANDeviceTypeDef,
-        "Sidewalk": SidewalkDeviceTypeDef,
-        "Positioning": PositioningConfigStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+LoRaWANDeviceUnionTypeDef = Union[LoRaWANDeviceTypeDef, LoRaWANDeviceOutputTypeDef]
 _RequiredUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
@@ -3540,15 +3714,15 @@
 
 DownlinkQueueMessageTypeDef = TypedDict(
     "DownlinkQueueMessageTypeDef",
     {
         "MessageId": str,
         "TransmitMode": int,
         "ReceivedAt": str,
-        "LoRaWAN": LoRaWANSendDataToDeviceTypeDef,
+        "LoRaWAN": LoRaWANSendDataToDeviceOutputTypeDef,
     },
     total=False,
 )
 
 WirelessMetadataTypeDef = TypedDict(
     "WirelessMetadataTypeDef",
     {
@@ -3609,42 +3783,52 @@
 GetWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     {
         "AutoCreateTasks": bool,
         "Name": str,
         "Update": UpdateWirelessGatewayTaskCreateTypeDef,
         "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWirelessGatewayTaskDefinitionsResponseTypeDef = TypedDict(
     "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
     {
         "NextToken": str,
         "TaskDefinitions": List[UpdateWirelessGatewayTaskEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPositionConfigurationsResponseTypeDef = TypedDict(
     "ListPositionConfigurationsResponseTypeDef",
     {
         "PositionConfigurationList": List[PositionConfigurationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
+    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
+    {
+        "DefaultLogLevel": LogLevelType,
+        "WirelessDeviceLogOptions": Sequence[WirelessDeviceLogOptionUnionTypeDef],
+        "WirelessGatewayLogOptions": Sequence[WirelessGatewayLogOptionUnionTypeDef],
+    },
+    total=False,
+)
+
 ListQueuedMessagesResponseTypeDef = TypedDict(
     "ListQueuedMessagesResponseTypeDef",
     {
         "NextToken": str,
         "DownlinkQueueMessagesList": List[DownlinkQueueMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendDataToWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredSendDataToWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
@@ -3671,20 +3855,20 @@
 GetPositionEstimateRequestRequestTypeDef = TypedDict(
     "GetPositionEstimateRequestRequestTypeDef",
     {
         "WiFiAccessPoints": Sequence[WiFiAccessPointTypeDef],
         "CellTowers": CellTowersTypeDef,
         "Ip": IpTypeDef,
         "Gnss": GnssTypeDef,
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
     },
     total=False,
 )
 
 ListEventConfigurationsResponseTypeDef = TypedDict(
     "ListEventConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "EventConfigurationsList": List[EventConfigurationItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless/type_defs.pyi` & `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iotwireless.type_defs import SessionKeysAbpV10XTypeDef
 
-    data: SessionKeysAbpV10XTypeDef = {...}
+    data: SessionKeysAbpV10XTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -65,45 +65,37 @@
 __all__ = (
     "SessionKeysAbpV10XTypeDef",
     "SessionKeysAbpV11TypeDef",
     "AccuracyTypeDef",
     "ApplicationConfigTypeDef",
     "SidewalkAccountInfoTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef",
     "AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "AssociateWirelessDeviceWithThingRequestRequestTypeDef",
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
-    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
+    "BeaconingOutputTypeDef",
     "BeaconingTypeDef",
+    "BlobTypeDef",
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     "CdmaLocalIdTypeDef",
     "CdmaNmrObjTypeDef",
     "CertificateListTypeDef",
     "LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef",
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
-    "CreateDestinationResponseTypeDef",
     "LoRaWANDeviceProfileTypeDef",
-    "CreateDeviceProfileResponseTypeDef",
     "LoRaWANFuotaTaskTypeDef",
-    "CreateFuotaTaskResponseTypeDef",
     "LoRaWANMulticastTypeDef",
-    "CreateMulticastGroupResponseTypeDef",
     "TraceContentTypeDef",
-    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
     "LoRaWANServiceProfileTypeDef",
-    "CreateServiceProfileResponseTypeDef",
     "SidewalkCreateWirelessDeviceTypeDef",
-    "CreateWirelessDeviceResponseTypeDef",
-    "CreateWirelessGatewayResponseTypeDef",
-    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
     "CreateWirelessGatewayTaskRequestRequestTypeDef",
-    "CreateWirelessGatewayTaskResponseTypeDef",
     "DakCertificateMetadataTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteDeviceProfileRequestRequestTypeDef",
     "DeleteFuotaTaskRequestRequestTypeDef",
     "DeleteMulticastGroupRequestRequestTypeDef",
     "DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "DeleteQueuedMessagesRequestRequestTypeDef",
@@ -125,54 +117,48 @@
     "DisassociateWirelessDeviceFromThingRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef",
     "DisassociateWirelessGatewayFromThingRequestRequestTypeDef",
     "PositioningTypeDef",
     "FuotaTaskTypeDef",
     "GatewayListItemTypeDef",
     "GetDestinationRequestRequestTypeDef",
-    "GetDestinationResponseTypeDef",
     "GetDeviceProfileRequestRequestTypeDef",
+    "LoRaWANDeviceProfileOutputTypeDef",
     "GetFuotaTaskRequestRequestTypeDef",
     "LoRaWANFuotaTaskGetInfoTypeDef",
     "GetMulticastGroupRequestRequestTypeDef",
     "LoRaWANMulticastGetTypeDef",
     "GetMulticastGroupSessionRequestRequestTypeDef",
-    "LoRaWANMulticastSessionTypeDef",
+    "LoRaWANMulticastSessionOutputTypeDef",
     "GetNetworkAnalyzerConfigurationRequestRequestTypeDef",
     "GetPartnerAccountRequestRequestTypeDef",
     "SidewalkAccountInfoWithFingerprintTypeDef",
     "GetPositionConfigurationRequestRequestTypeDef",
     "GnssTypeDef",
     "IpTypeDef",
+    "TimestampTypeDef",
     "WiFiAccessPointTypeDef",
-    "GetPositionEstimateResponseTypeDef",
     "GetPositionRequestRequestTypeDef",
     "GetResourceEventConfigurationRequestRequestTypeDef",
     "GetResourceLogLevelRequestRequestTypeDef",
-    "GetResourceLogLevelResponseTypeDef",
     "GetResourcePositionRequestRequestTypeDef",
-    "GetResourcePositionResponseTypeDef",
     "GetServiceEndpointRequestRequestTypeDef",
-    "GetServiceEndpointResponseTypeDef",
     "GetServiceProfileRequestRequestTypeDef",
     "LoRaWANGetServiceProfileInfoTypeDef",
     "GetWirelessDeviceImportTaskRequestRequestTypeDef",
     "SidewalkGetStartImportInfoTypeDef",
     "GetWirelessDeviceRequestRequestTypeDef",
     "GetWirelessDeviceStatisticsRequestRequestTypeDef",
     "SidewalkDeviceMetadataTypeDef",
     "GetWirelessGatewayCertificateRequestRequestTypeDef",
-    "GetWirelessGatewayCertificateResponseTypeDef",
     "GetWirelessGatewayFirmwareInformationRequestRequestTypeDef",
     "GetWirelessGatewayRequestRequestTypeDef",
     "GetWirelessGatewayStatisticsRequestRequestTypeDef",
-    "GetWirelessGatewayStatisticsResponseTypeDef",
     "GetWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskRequestRequestTypeDef",
-    "GetWirelessGatewayTaskResponseTypeDef",
     "GlobalIdentityTypeDef",
     "GsmLocalIdTypeDef",
     "ImportedSidewalkDeviceTypeDef",
     "LoRaWANJoinEventNotificationConfigurationsTypeDef",
     "LoRaWANJoinResourceTypeEventConfigurationTypeDef",
     "ListDestinationsRequestRequestTypeDef",
     "ListDeviceProfilesRequestRequestTypeDef",
@@ -197,57 +183,75 @@
     "ListWirelessGatewaysRequestRequestTypeDef",
     "LoRaWANGatewayMetadataTypeDef",
     "OtaaV10XTypeDef",
     "OtaaV11TypeDef",
     "LoRaWANGatewayVersionTypeDef",
     "LoRaWANListDeviceTypeDef",
     "LoRaWANMulticastMetadataTypeDef",
-    "LoRaWANStartFuotaTaskTypeDef",
     "UpdateAbpV10XTypeDef",
     "UpdateAbpV11TypeDef",
     "LteLocalIdTypeDef",
     "LteNmrObjTypeDef",
     "SemtechGnssConfigurationTypeDef",
     "SemtechGnssDetailTypeDef",
     "PutResourceLogLevelRequestRequestTypeDef",
     "ResetResourceLogLevelRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "SendDataToMulticastGroupResponseTypeDef",
-    "SendDataToWirelessDeviceResponseTypeDef",
     "SidewalkSendDataToDeviceTypeDef",
     "SidewalkSingleStartImportInfoTypeDef",
     "SidewalkStartImportInfoTypeDef",
     "SidewalkUpdateAccountTypeDef",
     "SidewalkUpdateImportInfoTypeDef",
-    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
-    "StartWirelessDeviceImportTaskResponseTypeDef",
     "TdscdmaLocalIdTypeDef",
     "TdscdmaNmrObjTypeDef",
     "TestWirelessDeviceRequestRequestTypeDef",
-    "TestWirelessDeviceResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
     "UpdatePositionRequestRequestTypeDef",
-    "UpdateResourcePositionRequestRequestTypeDef",
     "UpdateWirelessGatewayRequestRequestTypeDef",
     "WcdmaLocalIdTypeDef",
     "WcdmaNmrObjTypeDef",
     "WirelessDeviceEventLogOptionTypeDef",
     "WirelessGatewayEventLogOptionTypeDef",
     "AbpV10XTypeDef",
     "AbpV11TypeDef",
-    "GetPositionResponseTypeDef",
-    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
     "AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef",
     "CreateDestinationRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     "StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
+    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
+    "CreateDestinationResponseTypeDef",
+    "CreateDeviceProfileResponseTypeDef",
+    "CreateFuotaTaskResponseTypeDef",
+    "CreateMulticastGroupResponseTypeDef",
+    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
+    "CreateServiceProfileResponseTypeDef",
+    "CreateWirelessDeviceResponseTypeDef",
+    "CreateWirelessGatewayResponseTypeDef",
+    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
+    "CreateWirelessGatewayTaskResponseTypeDef",
+    "GetDestinationResponseTypeDef",
+    "GetPositionEstimateResponseTypeDef",
+    "GetPositionResponseTypeDef",
+    "GetResourceLogLevelResponseTypeDef",
+    "GetResourcePositionResponseTypeDef",
+    "GetServiceEndpointResponseTypeDef",
+    "GetWirelessGatewayCertificateResponseTypeDef",
+    "GetWirelessGatewayStatisticsResponseTypeDef",
+    "GetWirelessGatewayTaskResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SendDataToMulticastGroupResponseTypeDef",
+    "SendDataToWirelessDeviceResponseTypeDef",
+    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
+    "StartWirelessDeviceImportTaskResponseTypeDef",
+    "TestWirelessDeviceResponseTypeDef",
+    "LoRaWANGatewayOutputTypeDef",
     "LoRaWANGatewayTypeDef",
+    "UpdateResourcePositionRequestRequestTypeDef",
     "CdmaObjTypeDef",
     "SidewalkDeviceTypeDef",
     "SidewalkListDeviceTypeDef",
     "ConnectionStatusEventConfigurationTypeDef",
     "ConnectionStatusResourceTypeEventConfigurationTypeDef",
     "CreateDeviceProfileRequestRequestTypeDef",
     "CreateFuotaTaskRequestRequestTypeDef",
@@ -263,24 +267,28 @@
     "ListDeviceProfilesResponseTypeDef",
     "DeviceRegistrationStateEventConfigurationTypeDef",
     "MessageDeliveryStatusEventConfigurationTypeDef",
     "ProximityEventConfigurationTypeDef",
     "DeviceRegistrationStateResourceTypeEventConfigurationTypeDef",
     "MessageDeliveryStatusResourceTypeEventConfigurationTypeDef",
     "ProximityResourceTypeEventConfigurationTypeDef",
+    "FPortsOutputTypeDef",
     "FPortsTypeDef",
     "UpdateFPortsTypeDef",
     "ListFuotaTasksResponseTypeDef",
+    "ParticipatingGatewaysOutputTypeDef",
     "ParticipatingGatewaysTypeDef",
+    "LoRaWANDeviceProfileUnionTypeDef",
     "GetFuotaTaskResponseTypeDef",
     "GetMulticastGroupResponseTypeDef",
     "GetMulticastGroupSessionResponseTypeDef",
-    "StartMulticastGroupSessionRequestRequestTypeDef",
     "GetPartnerAccountResponseTypeDef",
     "ListPartnerAccountsResponseTypeDef",
+    "LoRaWANMulticastSessionTypeDef",
+    "LoRaWANStartFuotaTaskTypeDef",
     "GetServiceProfileResponseTypeDef",
     "GetWirelessDeviceImportTaskResponseTypeDef",
     "WirelessDeviceImportTaskTypeDef",
     "GsmNmrObjTypeDef",
     "ImportedWirelessDeviceTypeDef",
     "JoinEventConfigurationTypeDef",
     "JoinResourceTypeEventConfigurationTypeDef",
@@ -289,34 +297,41 @@
     "ListNetworkAnalyzerConfigurationsResponseTypeDef",
     "ListServiceProfilesResponseTypeDef",
     "LoRaWANDeviceMetadataTypeDef",
     "LoRaWANGatewayCurrentVersionTypeDef",
     "LoRaWANUpdateGatewayTaskCreateTypeDef",
     "LoRaWANUpdateGatewayTaskEntryTypeDef",
     "MulticastWirelessMetadataTypeDef",
-    "StartFuotaTaskRequestRequestTypeDef",
     "LteObjTypeDef",
     "PositionSolverConfigurationsTypeDef",
     "PositionSolverDetailsTypeDef",
     "StartSingleWirelessDeviceImportTaskRequestRequestTypeDef",
     "StartWirelessDeviceImportTaskRequestRequestTypeDef",
     "UpdatePartnerAccountRequestRequestTypeDef",
     "UpdateWirelessDeviceImportTaskRequestRequestTypeDef",
     "TdscdmaObjTypeDef",
     "WcdmaObjTypeDef",
+    "WirelessDeviceLogOptionOutputTypeDef",
     "WirelessDeviceLogOptionTypeDef",
+    "WirelessGatewayLogOptionOutputTypeDef",
     "WirelessGatewayLogOptionTypeDef",
-    "CreateWirelessGatewayRequestRequestTypeDef",
     "GetWirelessGatewayResponseTypeDef",
     "WirelessGatewayStatisticsTypeDef",
+    "CreateWirelessGatewayRequestRequestTypeDef",
+    "LoRaWANGatewayUnionTypeDef",
     "WirelessDeviceStatisticsTypeDef",
     "GetDeviceProfileResponseTypeDef",
+    "LoRaWANDeviceOutputTypeDef",
     "LoRaWANDeviceTypeDef",
     "LoRaWANUpdateDeviceTypeDef",
+    "LoRaWANSendDataToDeviceOutputTypeDef",
     "LoRaWANSendDataToDeviceTypeDef",
+    "LoRaWANMulticastSessionUnionTypeDef",
+    "StartMulticastGroupSessionRequestRequestTypeDef",
+    "StartFuotaTaskRequestRequestTypeDef",
     "ListWirelessDeviceImportTasksResponseTypeDef",
     "GsmObjTypeDef",
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     "EventNotificationItemConfigurationsTypeDef",
     "GetResourceEventConfigurationResponseTypeDef",
     "UpdateResourceEventConfigurationRequestRequestTypeDef",
     "GetEventConfigurationByResourceTypesResponseTypeDef",
@@ -325,29 +340,32 @@
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
     "UpdateWirelessGatewayTaskCreateTypeDef",
     "UpdateWirelessGatewayTaskEntryTypeDef",
     "SendDataToMulticastGroupRequestRequestTypeDef",
     "PutPositionConfigurationRequestRequestTypeDef",
     "GetPositionConfigurationResponseTypeDef",
     "PositionConfigurationItemTypeDef",
+    "WirelessDeviceLogOptionUnionTypeDef",
     "GetLogLevelsByResourceTypesResponseTypeDef",
-    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
+    "WirelessGatewayLogOptionUnionTypeDef",
     "ListWirelessGatewaysResponseTypeDef",
     "ListWirelessDevicesResponseTypeDef",
-    "CreateWirelessDeviceRequestRequestTypeDef",
     "GetWirelessDeviceResponseTypeDef",
+    "CreateWirelessDeviceRequestRequestTypeDef",
+    "LoRaWANDeviceUnionTypeDef",
     "UpdateWirelessDeviceRequestRequestTypeDef",
     "DownlinkQueueMessageTypeDef",
     "WirelessMetadataTypeDef",
     "CellTowersTypeDef",
     "EventConfigurationItemTypeDef",
     "CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
     "ListPositionConfigurationsResponseTypeDef",
+    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
     "ListQueuedMessagesResponseTypeDef",
     "SendDataToWirelessDeviceRequestRequestTypeDef",
     "GetPositionEstimateRequestRequestTypeDef",
     "ListEventConfigurationsResponseTypeDef",
 )
 
 SessionKeysAbpV10XTypeDef = TypedDict(
@@ -402,14 +420,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
 AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef = TypedDict(
     "AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
         "MulticastGroupId": str,
     },
 )
@@ -442,39 +471,41 @@
     "AssociateWirelessGatewayWithCertificateRequestRequestTypeDef",
     {
         "Id": str,
         "IotCertificateId": str,
     },
 )
 
-AssociateWirelessGatewayWithCertificateResponseTypeDef = TypedDict(
-    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
-    {
-        "IotCertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateWirelessGatewayWithThingRequestRequestTypeDef = TypedDict(
     "AssociateWirelessGatewayWithThingRequestRequestTypeDef",
     {
         "Id": str,
         "ThingArn": str,
     },
 )
 
+BeaconingOutputTypeDef = TypedDict(
+    "BeaconingOutputTypeDef",
+    {
+        "DataRate": int,
+        "Frequencies": List[int],
+    },
+    total=False,
+)
+
 BeaconingTypeDef = TypedDict(
     "BeaconingTypeDef",
     {
         "DataRate": int,
         "Frequencies": Sequence[int],
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelMulticastGroupSessionRequestRequestTypeDef = TypedDict(
     "CancelMulticastGroupSessionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -525,23 +556,14 @@
     "LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef",
     {
         "WirelessGatewayEventTopic": EventNotificationTopicStatusType,
     },
     total=False,
 )
 
-CreateDestinationResponseTypeDef = TypedDict(
-    "CreateDestinationResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANDeviceProfileTypeDef = TypedDict(
     "LoRaWANDeviceProfileTypeDef",
     {
         "SupportsClassB": bool,
         "ClassBTimeout": int,
         "PingSlotPeriod": int,
         "PingSlotDr": int,
@@ -560,150 +582,69 @@
         "RfRegion": str,
         "SupportsJoin": bool,
         "Supports32BitFCnt": bool,
     },
     total=False,
 )
 
-CreateDeviceProfileResponseTypeDef = TypedDict(
-    "CreateDeviceProfileResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANFuotaTaskTypeDef = TypedDict(
     "LoRaWANFuotaTaskTypeDef",
     {
         "RfRegion": SupportedRfRegionType,
     },
     total=False,
 )
 
-CreateFuotaTaskResponseTypeDef = TypedDict(
-    "CreateFuotaTaskResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANMulticastTypeDef = TypedDict(
     "LoRaWANMulticastTypeDef",
     {
         "RfRegion": SupportedRfRegionType,
         "DlClass": DlClassType,
     },
     total=False,
 )
 
-CreateMulticastGroupResponseTypeDef = TypedDict(
-    "CreateMulticastGroupResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TraceContentTypeDef = TypedDict(
     "TraceContentTypeDef",
     {
         "WirelessDeviceFrameInfo": WirelessDeviceFrameInfoType,
         "LogLevel": LogLevelType,
         "MulticastFrameInfo": MulticastFrameInfoType,
     },
     total=False,
 )
 
-CreateNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
-    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LoRaWANServiceProfileTypeDef = TypedDict(
     "LoRaWANServiceProfileTypeDef",
     {
         "AddGwMetadata": bool,
         "DrMin": int,
         "DrMax": int,
         "PrAllowed": bool,
         "RaAllowed": bool,
     },
     total=False,
 )
 
-CreateServiceProfileResponseTypeDef = TypedDict(
-    "CreateServiceProfileResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SidewalkCreateWirelessDeviceTypeDef = TypedDict(
     "SidewalkCreateWirelessDeviceTypeDef",
     {
         "DeviceProfileId": str,
     },
     total=False,
 )
 
-CreateWirelessDeviceResponseTypeDef = TypedDict(
-    "CreateWirelessDeviceResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWirelessGatewayResponseTypeDef = TypedDict(
-    "CreateWirelessGatewayResponseTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
-    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateWirelessGatewayTaskRequestRequestTypeDef = TypedDict(
     "CreateWirelessGatewayTaskRequestRequestTypeDef",
     {
         "Id": str,
         "WirelessGatewayTaskDefinitionId": str,
     },
 )
 
-CreateWirelessGatewayTaskResponseTypeDef = TypedDict(
-    "CreateWirelessGatewayTaskResponseTypeDef",
-    {
-        "WirelessGatewayTaskDefinitionId": str,
-        "Status": WirelessGatewayTaskStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDakCertificateMetadataTypeDef = TypedDict(
     "_RequiredDakCertificateMetadataTypeDef",
     {
         "CertificateId": str,
     },
 )
 _OptionalDakCertificateMetadataTypeDef = TypedDict(
@@ -963,32 +904,45 @@
 GetDestinationRequestRequestTypeDef = TypedDict(
     "GetDestinationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-GetDestinationResponseTypeDef = TypedDict(
-    "GetDestinationResponseTypeDef",
+GetDeviceProfileRequestRequestTypeDef = TypedDict(
+    "GetDeviceProfileRequestRequestTypeDef",
     {
-        "Arn": str,
-        "Name": str,
-        "Expression": str,
-        "ExpressionType": ExpressionTypeType,
-        "Description": str,
-        "RoleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Id": str,
     },
 )
 
-GetDeviceProfileRequestRequestTypeDef = TypedDict(
-    "GetDeviceProfileRequestRequestTypeDef",
+LoRaWANDeviceProfileOutputTypeDef = TypedDict(
+    "LoRaWANDeviceProfileOutputTypeDef",
     {
-        "Id": str,
+        "SupportsClassB": bool,
+        "ClassBTimeout": int,
+        "PingSlotPeriod": int,
+        "PingSlotDr": int,
+        "PingSlotFreq": int,
+        "SupportsClassC": bool,
+        "ClassCTimeout": int,
+        "MacVersion": str,
+        "RegParamsRevision": str,
+        "RxDelay1": int,
+        "RxDrOffset1": int,
+        "RxDataRate2": int,
+        "RxFreq2": int,
+        "FactoryPresetFreqsList": List[int],
+        "MaxEirp": int,
+        "MaxDutyCycle": int,
+        "RfRegion": str,
+        "SupportsJoin": bool,
+        "Supports32BitFCnt": bool,
     },
+    total=False,
 )
 
 GetFuotaTaskRequestRequestTypeDef = TypedDict(
     "GetFuotaTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
@@ -1024,16 +978,16 @@
 GetMulticastGroupSessionRequestRequestTypeDef = TypedDict(
     "GetMulticastGroupSessionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-LoRaWANMulticastSessionTypeDef = TypedDict(
-    "LoRaWANMulticastSessionTypeDef",
+LoRaWANMulticastSessionOutputTypeDef = TypedDict(
+    "LoRaWANMulticastSessionOutputTypeDef",
     {
         "DlDr": int,
         "DlFreq": int,
         "SessionStartTime": datetime,
         "SessionTimeout": int,
         "PingSlotPeriod": int,
     },
@@ -1097,30 +1051,23 @@
 IpTypeDef = TypedDict(
     "IpTypeDef",
     {
         "IpAddress": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 WiFiAccessPointTypeDef = TypedDict(
     "WiFiAccessPointTypeDef",
     {
         "MacAddress": str,
         "Rss": int,
     },
 )
 
-GetPositionEstimateResponseTypeDef = TypedDict(
-    "GetPositionEstimateResponseTypeDef",
-    {
-        "GeoJsonPayload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPositionRequestRequestTypeDef = TypedDict(
     "GetPositionRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
     },
 )
@@ -1150,56 +1097,30 @@
     "GetResourceLogLevelRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": str,
     },
 )
 
-GetResourceLogLevelResponseTypeDef = TypedDict(
-    "GetResourceLogLevelResponseTypeDef",
-    {
-        "LogLevel": LogLevelType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourcePositionRequestRequestTypeDef = TypedDict(
     "GetResourcePositionRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
     },
 )
 
-GetResourcePositionResponseTypeDef = TypedDict(
-    "GetResourcePositionResponseTypeDef",
-    {
-        "GeoJsonPayload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceEndpointRequestRequestTypeDef = TypedDict(
     "GetServiceEndpointRequestRequestTypeDef",
     {
         "ServiceType": WirelessGatewayServiceTypeType,
     },
     total=False,
 )
 
-GetServiceEndpointResponseTypeDef = TypedDict(
-    "GetServiceEndpointResponseTypeDef",
-    {
-        "ServiceType": WirelessGatewayServiceTypeType,
-        "ServiceEndpoint": str,
-        "ServerTrust": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceProfileRequestRequestTypeDef = TypedDict(
     "GetServiceProfileRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1274,23 +1195,14 @@
 GetWirelessGatewayCertificateRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayCertificateRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetWirelessGatewayCertificateResponseTypeDef = TypedDict(
-    "GetWirelessGatewayCertificateResponseTypeDef",
-    {
-        "IotCertificateId": str,
-        "LoRaWANNetworkServerCertificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWirelessGatewayFirmwareInformationRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayFirmwareInformationRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -1305,50 +1217,28 @@
 GetWirelessGatewayStatisticsRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayStatisticsRequestRequestTypeDef",
     {
         "WirelessGatewayId": str,
     },
 )
 
-GetWirelessGatewayStatisticsResponseTypeDef = TypedDict(
-    "GetWirelessGatewayStatisticsResponseTypeDef",
-    {
-        "WirelessGatewayId": str,
-        "LastUplinkReceivedAt": str,
-        "ConnectionStatus": ConnectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWirelessGatewayTaskDefinitionRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayTaskDefinitionRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
 GetWirelessGatewayTaskRequestRequestTypeDef = TypedDict(
     "GetWirelessGatewayTaskRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetWirelessGatewayTaskResponseTypeDef = TypedDict(
-    "GetWirelessGatewayTaskResponseTypeDef",
-    {
-        "WirelessGatewayId": str,
-        "WirelessGatewayTaskDefinitionId": str,
-        "LastUplinkReceivedAt": str,
-        "TaskCreatedAt": str,
-        "Status": WirelessGatewayTaskStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GlobalIdentityTypeDef = TypedDict(
     "GlobalIdentityTypeDef",
     {
         "Lac": int,
         "GeranCid": int,
     },
 )
@@ -1687,22 +1577,14 @@
     "LoRaWANMulticastMetadataTypeDef",
     {
         "FPort": int,
     },
     total=False,
 )
 
-LoRaWANStartFuotaTaskTypeDef = TypedDict(
-    "LoRaWANStartFuotaTaskTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 UpdateAbpV10XTypeDef = TypedDict(
     "UpdateAbpV10XTypeDef",
     {
         "FCntStart": int,
     },
     total=False,
 )
@@ -1775,41 +1657,14 @@
     "ResetResourceLogLevelRequestRequestTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": str,
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
-SendDataToMulticastGroupResponseTypeDef = TypedDict(
-    "SendDataToMulticastGroupResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SendDataToWirelessDeviceResponseTypeDef = TypedDict(
-    "SendDataToWirelessDeviceResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SidewalkSendDataToDeviceTypeDef = TypedDict(
     "SidewalkSendDataToDeviceTypeDef",
     {
         "Seq": int,
         "MessageType": MessageTypeType,
         "AckModeRetryDurationSecs": int,
     },
@@ -1845,32 +1700,14 @@
     "SidewalkUpdateImportInfoTypeDef",
     {
         "DeviceCreationFile": str,
     },
     total=False,
 )
 
-StartSingleWirelessDeviceImportTaskResponseTypeDef = TypedDict(
-    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartWirelessDeviceImportTaskResponseTypeDef = TypedDict(
-    "StartWirelessDeviceImportTaskResponseTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TdscdmaLocalIdTypeDef = TypedDict(
     "TdscdmaLocalIdTypeDef",
     {
         "Uarfcn": int,
         "CellParams": int,
     },
 )
@@ -1898,22 +1735,14 @@
 TestWirelessDeviceRequestRequestTypeDef = TypedDict(
     "TestWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-TestWirelessDeviceResponseTypeDef = TypedDict(
-    "TestWirelessDeviceResponseTypeDef",
-    {
-        "Result": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1945,35 +1774,14 @@
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
         "Position": Sequence[float],
     },
 )
 
-_RequiredUpdateResourcePositionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateResourcePositionRequestRequestTypeDef",
-    {
-        "ResourceIdentifier": str,
-        "ResourceType": PositionResourceTypeType,
-    },
-)
-_OptionalUpdateResourcePositionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateResourcePositionRequestRequestTypeDef",
-    {
-        "GeoJsonPayload": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-class UpdateResourcePositionRequestRequestTypeDef(
-    _RequiredUpdateResourcePositionRequestRequestTypeDef,
-    _OptionalUpdateResourcePositionRequestRequestTypeDef,
-):
-    pass
-
 _RequiredUpdateWirelessGatewayRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessGatewayRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessGatewayRequestRequestTypeDef = TypedDict(
@@ -2054,36 +1862,14 @@
         "DevAddr": str,
         "SessionKeys": SessionKeysAbpV11TypeDef,
         "FCntStart": int,
     },
     total=False,
 )
 
-GetPositionResponseTypeDef = TypedDict(
-    "GetPositionResponseTypeDef",
-    {
-        "Position": List[float],
-        "Accuracy": AccuracyTypeDef,
-        "SolverType": Literal["GNSS"],
-        "SolverProvider": Literal["Semtech"],
-        "SolverVersion": str,
-        "Timestamp": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AssociateAwsAccountWithPartnerAccountResponseTypeDef = TypedDict(
-    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
-    {
-        "Sidewalk": SidewalkAccountInfoTypeDef,
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoTypeDef,
     },
 )
 _OptionalAssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = TypedDict(
@@ -2121,22 +1907,14 @@
 )
 
 class CreateDestinationRequestRequestTypeDef(
     _RequiredCreateDestinationRequestRequestTypeDef, _OptionalCreateDestinationRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = TypedDict(
     "_RequiredStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = TypedDict(
@@ -2179,28 +1957,311 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+AssociateAwsAccountWithPartnerAccountResponseTypeDef = TypedDict(
+    "AssociateAwsAccountWithPartnerAccountResponseTypeDef",
+    {
+        "Sidewalk": SidewalkAccountInfoTypeDef,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociateWirelessGatewayWithCertificateResponseTypeDef = TypedDict(
+    "AssociateWirelessGatewayWithCertificateResponseTypeDef",
+    {
+        "IotCertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDestinationResponseTypeDef = TypedDict(
+    "CreateDestinationResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeviceProfileResponseTypeDef = TypedDict(
+    "CreateDeviceProfileResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFuotaTaskResponseTypeDef = TypedDict(
+    "CreateFuotaTaskResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMulticastGroupResponseTypeDef = TypedDict(
+    "CreateMulticastGroupResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNetworkAnalyzerConfigurationResponseTypeDef = TypedDict(
+    "CreateNetworkAnalyzerConfigurationResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateServiceProfileResponseTypeDef = TypedDict(
+    "CreateServiceProfileResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessDeviceResponseTypeDef = TypedDict(
+    "CreateWirelessDeviceResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessGatewayResponseTypeDef = TypedDict(
+    "CreateWirelessGatewayResponseTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
+    "CreateWirelessGatewayTaskDefinitionResponseTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWirelessGatewayTaskResponseTypeDef = TypedDict(
+    "CreateWirelessGatewayTaskResponseTypeDef",
+    {
+        "WirelessGatewayTaskDefinitionId": str,
+        "Status": WirelessGatewayTaskStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDestinationResponseTypeDef = TypedDict(
+    "GetDestinationResponseTypeDef",
+    {
+        "Arn": str,
+        "Name": str,
+        "Expression": str,
+        "ExpressionType": ExpressionTypeType,
+        "Description": str,
+        "RoleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPositionEstimateResponseTypeDef = TypedDict(
+    "GetPositionEstimateResponseTypeDef",
+    {
+        "GeoJsonPayload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPositionResponseTypeDef = TypedDict(
+    "GetPositionResponseTypeDef",
+    {
+        "Position": List[float],
+        "Accuracy": AccuracyTypeDef,
+        "SolverType": Literal["GNSS"],
+        "SolverProvider": Literal["Semtech"],
+        "SolverVersion": str,
+        "Timestamp": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourceLogLevelResponseTypeDef = TypedDict(
+    "GetResourceLogLevelResponseTypeDef",
+    {
+        "LogLevel": LogLevelType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePositionResponseTypeDef = TypedDict(
+    "GetResourcePositionResponseTypeDef",
+    {
+        "GeoJsonPayload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceEndpointResponseTypeDef = TypedDict(
+    "GetServiceEndpointResponseTypeDef",
+    {
+        "ServiceType": WirelessGatewayServiceTypeType,
+        "ServiceEndpoint": str,
+        "ServerTrust": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessGatewayCertificateResponseTypeDef = TypedDict(
+    "GetWirelessGatewayCertificateResponseTypeDef",
+    {
+        "IotCertificateId": str,
+        "LoRaWANNetworkServerCertificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessGatewayStatisticsResponseTypeDef = TypedDict(
+    "GetWirelessGatewayStatisticsResponseTypeDef",
+    {
+        "WirelessGatewayId": str,
+        "LastUplinkReceivedAt": str,
+        "ConnectionStatus": ConnectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessGatewayTaskResponseTypeDef = TypedDict(
+    "GetWirelessGatewayTaskResponseTypeDef",
+    {
+        "WirelessGatewayId": str,
+        "WirelessGatewayTaskDefinitionId": str,
+        "LastUplinkReceivedAt": str,
+        "TaskCreatedAt": str,
+        "Status": WirelessGatewayTaskStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendDataToMulticastGroupResponseTypeDef = TypedDict(
+    "SendDataToMulticastGroupResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendDataToWirelessDeviceResponseTypeDef = TypedDict(
+    "SendDataToWirelessDeviceResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSingleWirelessDeviceImportTaskResponseTypeDef = TypedDict(
+    "StartSingleWirelessDeviceImportTaskResponseTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartWirelessDeviceImportTaskResponseTypeDef = TypedDict(
+    "StartWirelessDeviceImportTaskResponseTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestWirelessDeviceResponseTypeDef = TypedDict(
+    "TestWirelessDeviceResponseTypeDef",
+    {
+        "Result": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoRaWANGatewayOutputTypeDef = TypedDict(
+    "LoRaWANGatewayOutputTypeDef",
+    {
+        "GatewayEui": str,
+        "RfRegion": str,
+        "JoinEuiFilters": List[List[str]],
+        "NetIdFilters": List[str],
+        "SubBands": List[int],
+        "Beaconing": BeaconingOutputTypeDef,
+        "MaxEirp": float,
+    },
+    total=False,
+)
+
 LoRaWANGatewayTypeDef = TypedDict(
     "LoRaWANGatewayTypeDef",
     {
         "GatewayEui": str,
         "RfRegion": str,
         "JoinEuiFilters": Sequence[Sequence[str]],
         "NetIdFilters": Sequence[str],
         "SubBands": Sequence[int],
         "Beaconing": BeaconingTypeDef,
         "MaxEirp": float,
     },
     total=False,
 )
 
+_RequiredUpdateResourcePositionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateResourcePositionRequestRequestTypeDef",
+    {
+        "ResourceIdentifier": str,
+        "ResourceType": PositionResourceTypeType,
+    },
+)
+_OptionalUpdateResourcePositionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateResourcePositionRequestRequestTypeDef",
+    {
+        "GeoJsonPayload": BlobTypeDef,
+    },
+    total=False,
+)
+
+class UpdateResourcePositionRequestRequestTypeDef(
+    _RequiredUpdateResourcePositionRequestRequestTypeDef,
+    _OptionalUpdateResourcePositionRequestRequestTypeDef,
+):
+    pass
+
 _RequiredCdmaObjTypeDef = TypedDict(
     "_RequiredCdmaObjTypeDef",
     {
         "SystemId": int,
         "NetworkId": int,
         "BaseStationId": int,
     },
@@ -2408,15 +2469,15 @@
         "TraceContent": TraceContentTypeDef,
         "WirelessDevices": List[str],
         "WirelessGateways": List[str],
         "Description": str,
         "Arn": str,
         "Name": str,
         "MulticastGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNetworkAnalyzerConfigurationRequestRequestTypeDef",
     {
         "ConfigurationName": str,
@@ -2465,24 +2526,24 @@
 )
 
 ListDestinationsResponseTypeDef = TypedDict(
     "ListDestinationsResponseTypeDef",
     {
         "NextToken": str,
         "DestinationList": List[DestinationsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeviceProfilesResponseTypeDef = TypedDict(
     "ListDeviceProfilesResponseTypeDef",
     {
         "NextToken": str,
         "DeviceProfileList": List[DeviceProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceRegistrationStateEventConfigurationTypeDef = TypedDict(
     "DeviceRegistrationStateEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkEventNotificationConfigurationsTypeDef,
@@ -2529,14 +2590,26 @@
     "ProximityResourceTypeEventConfigurationTypeDef",
     {
         "Sidewalk": SidewalkResourceTypeEventConfigurationTypeDef,
     },
     total=False,
 )
 
+FPortsOutputTypeDef = TypedDict(
+    "FPortsOutputTypeDef",
+    {
+        "Fuota": int,
+        "Multicast": int,
+        "ClockSync": int,
+        "Positioning": PositioningTypeDef,
+        "Applications": List[ApplicationConfigTypeDef],
+    },
+    total=False,
+)
+
 FPortsTypeDef = TypedDict(
     "FPortsTypeDef",
     {
         "Fuota": int,
         "Multicast": int,
         "ClockSync": int,
         "Positioning": PositioningTypeDef,
@@ -2555,27 +2628,39 @@
 )
 
 ListFuotaTasksResponseTypeDef = TypedDict(
     "ListFuotaTasksResponseTypeDef",
     {
         "NextToken": str,
         "FuotaTaskList": List[FuotaTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ParticipatingGatewaysOutputTypeDef = TypedDict(
+    "ParticipatingGatewaysOutputTypeDef",
+    {
+        "DownlinkMode": DownlinkModeType,
+        "GatewayList": List[GatewayListItemTypeDef],
+        "TransmissionInterval": int,
     },
 )
 
 ParticipatingGatewaysTypeDef = TypedDict(
     "ParticipatingGatewaysTypeDef",
     {
         "DownlinkMode": DownlinkModeType,
-        "GatewayList": List[GatewayListItemTypeDef],
+        "GatewayList": Sequence[GatewayListItemTypeDef],
         "TransmissionInterval": int,
     },
 )
 
+LoRaWANDeviceProfileUnionTypeDef = Union[
+    LoRaWANDeviceProfileTypeDef, LoRaWANDeviceProfileOutputTypeDef
+]
 GetFuotaTaskResponseTypeDef = TypedDict(
     "GetFuotaTaskResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Status": FuotaTaskStatusType,
         "Name": str,
@@ -2583,74 +2668,86 @@
         "LoRaWAN": LoRaWANFuotaTaskGetInfoTypeDef,
         "FirmwareUpdateImage": str,
         "FirmwareUpdateRole": str,
         "CreatedAt": datetime,
         "RedundancyPercent": int,
         "FragmentSizeBytes": int,
         "FragmentIntervalMS": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMulticastGroupResponseTypeDef = TypedDict(
     "GetMulticastGroupResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "Status": str,
         "LoRaWAN": LoRaWANMulticastGetTypeDef,
         "CreatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMulticastGroupSessionResponseTypeDef = TypedDict(
     "GetMulticastGroupSessionResponseTypeDef",
     {
-        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
-    "StartMulticastGroupSessionRequestRequestTypeDef",
-    {
-        "Id": str,
-        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+        "LoRaWAN": LoRaWANMulticastSessionOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPartnerAccountResponseTypeDef = TypedDict(
     "GetPartnerAccountResponseTypeDef",
     {
         "Sidewalk": SidewalkAccountInfoWithFingerprintTypeDef,
         "AccountLinked": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPartnerAccountsResponseTypeDef = TypedDict(
     "ListPartnerAccountsResponseTypeDef",
     {
         "NextToken": str,
         "Sidewalk": List[SidewalkAccountInfoWithFingerprintTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoRaWANMulticastSessionTypeDef = TypedDict(
+    "LoRaWANMulticastSessionTypeDef",
+    {
+        "DlDr": int,
+        "DlFreq": int,
+        "SessionStartTime": TimestampTypeDef,
+        "SessionTimeout": int,
+        "PingSlotPeriod": int,
+    },
+    total=False,
+)
+
+LoRaWANStartFuotaTaskTypeDef = TypedDict(
+    "LoRaWANStartFuotaTaskTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
 GetServiceProfileResponseTypeDef = TypedDict(
     "GetServiceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
         "LoRaWAN": LoRaWANGetServiceProfileInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWirelessDeviceImportTaskResponseTypeDef = TypedDict(
     "GetWirelessDeviceImportTaskResponseTypeDef",
     {
         "Id": str,
@@ -2660,15 +2757,15 @@
         "CreationTime": datetime,
         "Status": ImportTaskStatusType,
         "StatusReason": str,
         "InitializedImportedDeviceCount": int,
         "PendingImportedDeviceCount": int,
         "OnboardedImportedDeviceCount": int,
         "FailedImportedDeviceCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WirelessDeviceImportTaskTypeDef = TypedDict(
     "WirelessDeviceImportTaskTypeDef",
     {
         "Id": str,
@@ -2731,42 +2828,42 @@
 )
 
 ListMulticastGroupsByFuotaTaskResponseTypeDef = TypedDict(
     "ListMulticastGroupsByFuotaTaskResponseTypeDef",
     {
         "NextToken": str,
         "MulticastGroupList": List[MulticastGroupByFuotaTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMulticastGroupsResponseTypeDef = TypedDict(
     "ListMulticastGroupsResponseTypeDef",
     {
         "NextToken": str,
         "MulticastGroupList": List[MulticastGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNetworkAnalyzerConfigurationsResponseTypeDef = TypedDict(
     "ListNetworkAnalyzerConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "NetworkAnalyzerConfigurationList": List[NetworkAnalyzerConfigurationsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceProfilesResponseTypeDef = TypedDict(
     "ListServiceProfilesResponseTypeDef",
     {
         "NextToken": str,
         "ServiceProfileList": List[ServiceProfileTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoRaWANDeviceMetadataTypeDef = TypedDict(
     "LoRaWANDeviceMetadataTypeDef",
     {
         "DevEui": str,
@@ -2811,33 +2908,14 @@
     "MulticastWirelessMetadataTypeDef",
     {
         "LoRaWAN": LoRaWANMulticastMetadataTypeDef,
     },
     total=False,
 )
 
-_RequiredStartFuotaTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFuotaTaskRequestRequestTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalStartFuotaTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFuotaTaskRequestRequestTypeDef",
-    {
-        "LoRaWAN": LoRaWANStartFuotaTaskTypeDef,
-    },
-    total=False,
-)
-
-class StartFuotaTaskRequestRequestTypeDef(
-    _RequiredStartFuotaTaskRequestRequestTypeDef, _OptionalStartFuotaTaskRequestRequestTypeDef
-):
-    pass
-
 _RequiredLteObjTypeDef = TypedDict(
     "_RequiredLteObjTypeDef",
     {
         "Mcc": int,
         "Mnc": int,
         "EutranCid": int,
     },
@@ -2980,104 +3058,145 @@
     },
     total=False,
 )
 
 class WcdmaObjTypeDef(_RequiredWcdmaObjTypeDef, _OptionalWcdmaObjTypeDef):
     pass
 
+_RequiredWirelessDeviceLogOptionOutputTypeDef = TypedDict(
+    "_RequiredWirelessDeviceLogOptionOutputTypeDef",
+    {
+        "Type": WirelessDeviceTypeType,
+        "LogLevel": LogLevelType,
+    },
+)
+_OptionalWirelessDeviceLogOptionOutputTypeDef = TypedDict(
+    "_OptionalWirelessDeviceLogOptionOutputTypeDef",
+    {
+        "Events": List[WirelessDeviceEventLogOptionTypeDef],
+    },
+    total=False,
+)
+
+class WirelessDeviceLogOptionOutputTypeDef(
+    _RequiredWirelessDeviceLogOptionOutputTypeDef, _OptionalWirelessDeviceLogOptionOutputTypeDef
+):
+    pass
+
 _RequiredWirelessDeviceLogOptionTypeDef = TypedDict(
     "_RequiredWirelessDeviceLogOptionTypeDef",
     {
         "Type": WirelessDeviceTypeType,
         "LogLevel": LogLevelType,
     },
 )
 _OptionalWirelessDeviceLogOptionTypeDef = TypedDict(
     "_OptionalWirelessDeviceLogOptionTypeDef",
     {
-        "Events": List[WirelessDeviceEventLogOptionTypeDef],
+        "Events": Sequence[WirelessDeviceEventLogOptionTypeDef],
     },
     total=False,
 )
 
 class WirelessDeviceLogOptionTypeDef(
     _RequiredWirelessDeviceLogOptionTypeDef, _OptionalWirelessDeviceLogOptionTypeDef
 ):
     pass
 
-_RequiredWirelessGatewayLogOptionTypeDef = TypedDict(
-    "_RequiredWirelessGatewayLogOptionTypeDef",
+_RequiredWirelessGatewayLogOptionOutputTypeDef = TypedDict(
+    "_RequiredWirelessGatewayLogOptionOutputTypeDef",
     {
         "Type": Literal["LoRaWAN"],
         "LogLevel": LogLevelType,
     },
 )
-_OptionalWirelessGatewayLogOptionTypeDef = TypedDict(
-    "_OptionalWirelessGatewayLogOptionTypeDef",
+_OptionalWirelessGatewayLogOptionOutputTypeDef = TypedDict(
+    "_OptionalWirelessGatewayLogOptionOutputTypeDef",
     {
         "Events": List[WirelessGatewayEventLogOptionTypeDef],
     },
     total=False,
 )
 
-class WirelessGatewayLogOptionTypeDef(
-    _RequiredWirelessGatewayLogOptionTypeDef, _OptionalWirelessGatewayLogOptionTypeDef
+class WirelessGatewayLogOptionOutputTypeDef(
+    _RequiredWirelessGatewayLogOptionOutputTypeDef, _OptionalWirelessGatewayLogOptionOutputTypeDef
 ):
     pass
 
-_RequiredCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWirelessGatewayRequestRequestTypeDef",
+_RequiredWirelessGatewayLogOptionTypeDef = TypedDict(
+    "_RequiredWirelessGatewayLogOptionTypeDef",
     {
-        "LoRaWAN": LoRaWANGatewayTypeDef,
+        "Type": Literal["LoRaWAN"],
+        "LogLevel": LogLevelType,
     },
 )
-_OptionalCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWirelessGatewayRequestRequestTypeDef",
+_OptionalWirelessGatewayLogOptionTypeDef = TypedDict(
+    "_OptionalWirelessGatewayLogOptionTypeDef",
     {
-        "Name": str,
-        "Description": str,
-        "Tags": Sequence[TagTypeDef],
-        "ClientRequestToken": str,
+        "Events": Sequence[WirelessGatewayEventLogOptionTypeDef],
     },
     total=False,
 )
 
-class CreateWirelessGatewayRequestRequestTypeDef(
-    _RequiredCreateWirelessGatewayRequestRequestTypeDef,
-    _OptionalCreateWirelessGatewayRequestRequestTypeDef,
+class WirelessGatewayLogOptionTypeDef(
+    _RequiredWirelessGatewayLogOptionTypeDef, _OptionalWirelessGatewayLogOptionTypeDef
 ):
     pass
 
 GetWirelessGatewayResponseTypeDef = TypedDict(
     "GetWirelessGatewayResponseTypeDef",
     {
         "Name": str,
         "Id": str,
         "Description": str,
-        "LoRaWAN": LoRaWANGatewayTypeDef,
+        "LoRaWAN": LoRaWANGatewayOutputTypeDef,
         "Arn": str,
         "ThingName": str,
         "ThingArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WirelessGatewayStatisticsTypeDef = TypedDict(
     "WirelessGatewayStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
-        "LoRaWAN": LoRaWANGatewayTypeDef,
+        "LoRaWAN": LoRaWANGatewayOutputTypeDef,
         "LastUplinkReceivedAt": str,
     },
     total=False,
 )
 
+_RequiredCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWirelessGatewayRequestRequestTypeDef",
+    {
+        "LoRaWAN": LoRaWANGatewayTypeDef,
+    },
+)
+_OptionalCreateWirelessGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWirelessGatewayRequestRequestTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Tags": Sequence[TagTypeDef],
+        "ClientRequestToken": str,
+    },
+    total=False,
+)
+
+class CreateWirelessGatewayRequestRequestTypeDef(
+    _RequiredCreateWirelessGatewayRequestRequestTypeDef,
+    _OptionalCreateWirelessGatewayRequestRequestTypeDef,
+):
+    pass
+
+LoRaWANGatewayUnionTypeDef = Union[LoRaWANGatewayTypeDef, LoRaWANGatewayOutputTypeDef]
 WirelessDeviceStatisticsTypeDef = TypedDict(
     "WirelessDeviceStatisticsTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Type": WirelessDeviceTypeType,
         "Name": str,
@@ -3094,20 +3213,35 @@
 
 GetDeviceProfileResponseTypeDef = TypedDict(
     "GetDeviceProfileResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Id": str,
-        "LoRaWAN": LoRaWANDeviceProfileTypeDef,
+        "LoRaWAN": LoRaWANDeviceProfileOutputTypeDef,
         "Sidewalk": SidewalkGetDeviceProfileTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoRaWANDeviceOutputTypeDef = TypedDict(
+    "LoRaWANDeviceOutputTypeDef",
+    {
+        "DevEui": str,
+        "DeviceProfileId": str,
+        "ServiceProfileId": str,
+        "OtaaV1_1": OtaaV11TypeDef,
+        "OtaaV1_0_x": OtaaV10XTypeDef,
+        "AbpV1_1": AbpV11TypeDef,
+        "AbpV1_0_x": AbpV10XTypeDef,
+        "FPorts": FPortsOutputTypeDef,
+    },
+    total=False,
+)
+
 LoRaWANDeviceTypeDef = TypedDict(
     "LoRaWANDeviceTypeDef",
     {
         "DevEui": str,
         "DeviceProfileId": str,
         "ServiceProfileId": str,
         "OtaaV1_1": OtaaV11TypeDef,
@@ -3127,29 +3261,68 @@
         "AbpV1_1": UpdateAbpV11TypeDef,
         "AbpV1_0_x": UpdateAbpV10XTypeDef,
         "FPorts": UpdateFPortsTypeDef,
     },
     total=False,
 )
 
+LoRaWANSendDataToDeviceOutputTypeDef = TypedDict(
+    "LoRaWANSendDataToDeviceOutputTypeDef",
+    {
+        "FPort": int,
+        "ParticipatingGateways": ParticipatingGatewaysOutputTypeDef,
+    },
+    total=False,
+)
+
 LoRaWANSendDataToDeviceTypeDef = TypedDict(
     "LoRaWANSendDataToDeviceTypeDef",
     {
         "FPort": int,
         "ParticipatingGateways": ParticipatingGatewaysTypeDef,
     },
     total=False,
 )
 
+LoRaWANMulticastSessionUnionTypeDef = Union[
+    LoRaWANMulticastSessionTypeDef, LoRaWANMulticastSessionOutputTypeDef
+]
+StartMulticastGroupSessionRequestRequestTypeDef = TypedDict(
+    "StartMulticastGroupSessionRequestRequestTypeDef",
+    {
+        "Id": str,
+        "LoRaWAN": LoRaWANMulticastSessionTypeDef,
+    },
+)
+
+_RequiredStartFuotaTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFuotaTaskRequestRequestTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalStartFuotaTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFuotaTaskRequestRequestTypeDef",
+    {
+        "LoRaWAN": LoRaWANStartFuotaTaskTypeDef,
+    },
+    total=False,
+)
+
+class StartFuotaTaskRequestRequestTypeDef(
+    _RequiredStartFuotaTaskRequestRequestTypeDef, _OptionalStartFuotaTaskRequestRequestTypeDef
+):
+    pass
+
 ListWirelessDeviceImportTasksResponseTypeDef = TypedDict(
     "ListWirelessDeviceImportTasksResponseTypeDef",
     {
         "NextToken": str,
         "WirelessDeviceImportTaskList": List[WirelessDeviceImportTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGsmObjTypeDef = TypedDict(
     "_RequiredGsmObjTypeDef",
     {
         "Mcc": int,
@@ -3174,15 +3347,15 @@
 
 ListDevicesForWirelessDeviceImportTaskResponseTypeDef = TypedDict(
     "ListDevicesForWirelessDeviceImportTaskResponseTypeDef",
     {
         "NextToken": str,
         "DestinationName": str,
         "ImportedWirelessDeviceList": List[ImportedWirelessDeviceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventNotificationItemConfigurationsTypeDef = TypedDict(
     "EventNotificationItemConfigurationsTypeDef",
     {
         "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationTypeDef,
@@ -3198,15 +3371,15 @@
     "GetResourceEventConfigurationResponseTypeDef",
     {
         "DeviceRegistrationState": DeviceRegistrationStateEventConfigurationTypeDef,
         "Proximity": ProximityEventConfigurationTypeDef,
         "Join": JoinEventConfigurationTypeDef,
         "ConnectionStatus": ConnectionStatusEventConfigurationTypeDef,
         "MessageDeliveryStatus": MessageDeliveryStatusEventConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateResourceEventConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceEventConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
@@ -3236,15 +3409,15 @@
     "GetEventConfigurationByResourceTypesResponseTypeDef",
     {
         "DeviceRegistrationState": DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
         "Proximity": ProximityResourceTypeEventConfigurationTypeDef,
         "Join": JoinResourceTypeEventConfigurationTypeDef,
         "ConnectionStatus": ConnectionStatusResourceTypeEventConfigurationTypeDef,
         "MessageDeliveryStatus": MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventConfigurationByResourceTypesRequestRequestTypeDef = TypedDict(
     "UpdateEventConfigurationByResourceTypesRequestRequestTypeDef",
     {
         "DeviceRegistrationState": DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
@@ -3259,23 +3432,23 @@
 GetWirelessDeviceStatisticsResponseTypeDef = TypedDict(
     "GetWirelessDeviceStatisticsResponseTypeDef",
     {
         "WirelessDeviceId": str,
         "LastUplinkReceivedAt": str,
         "LoRaWAN": LoRaWANDeviceMetadataTypeDef,
         "Sidewalk": SidewalkDeviceMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWirelessGatewayFirmwareInformationResponseTypeDef = TypedDict(
     "GetWirelessGatewayFirmwareInformationResponseTypeDef",
     {
         "LoRaWAN": LoRaWANGatewayCurrentVersionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWirelessGatewayTaskCreateTypeDef = TypedDict(
     "UpdateWirelessGatewayTaskCreateTypeDef",
     {
         "UpdateDataSource": str,
@@ -3327,64 +3500,78 @@
     pass
 
 GetPositionConfigurationResponseTypeDef = TypedDict(
     "GetPositionConfigurationResponseTypeDef",
     {
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PositionConfigurationItemTypeDef = TypedDict(
     "PositionConfigurationItemTypeDef",
     {
         "ResourceIdentifier": str,
         "ResourceType": PositionResourceTypeType,
         "Solvers": PositionSolverDetailsTypeDef,
         "Destination": str,
     },
     total=False,
 )
 
+WirelessDeviceLogOptionUnionTypeDef = Union[
+    WirelessDeviceLogOptionTypeDef, WirelessDeviceLogOptionOutputTypeDef
+]
 GetLogLevelsByResourceTypesResponseTypeDef = TypedDict(
     "GetLogLevelsByResourceTypesResponseTypeDef",
     {
         "DefaultLogLevel": LogLevelType,
-        "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionTypeDef],
-        "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "WirelessGatewayLogOptions": List[WirelessGatewayLogOptionOutputTypeDef],
+        "WirelessDeviceLogOptions": List[WirelessDeviceLogOptionOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
-    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
-    {
-        "DefaultLogLevel": LogLevelType,
-        "WirelessDeviceLogOptions": Sequence[WirelessDeviceLogOptionTypeDef],
-        "WirelessGatewayLogOptions": Sequence[WirelessGatewayLogOptionTypeDef],
-    },
-    total=False,
-)
-
+WirelessGatewayLogOptionUnionTypeDef = Union[
+    WirelessGatewayLogOptionTypeDef, WirelessGatewayLogOptionOutputTypeDef
+]
 ListWirelessGatewaysResponseTypeDef = TypedDict(
     "ListWirelessGatewaysResponseTypeDef",
     {
         "NextToken": str,
         "WirelessGatewayList": List[WirelessGatewayStatisticsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWirelessDevicesResponseTypeDef = TypedDict(
     "ListWirelessDevicesResponseTypeDef",
     {
         "NextToken": str,
         "WirelessDeviceList": List[WirelessDeviceStatisticsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWirelessDeviceResponseTypeDef = TypedDict(
+    "GetWirelessDeviceResponseTypeDef",
+    {
+        "Type": WirelessDeviceTypeType,
+        "Name": str,
+        "Description": str,
+        "DestinationName": str,
+        "Id": str,
+        "Arn": str,
+        "ThingName": str,
+        "ThingArn": str,
+        "LoRaWAN": LoRaWANDeviceOutputTypeDef,
+        "Sidewalk": SidewalkDeviceTypeDef,
+        "Positioning": PositioningConfigStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWirelessDeviceRequestRequestTypeDef",
     {
         "Type": WirelessDeviceTypeType,
@@ -3407,32 +3594,15 @@
 
 class CreateWirelessDeviceRequestRequestTypeDef(
     _RequiredCreateWirelessDeviceRequestRequestTypeDef,
     _OptionalCreateWirelessDeviceRequestRequestTypeDef,
 ):
     pass
 
-GetWirelessDeviceResponseTypeDef = TypedDict(
-    "GetWirelessDeviceResponseTypeDef",
-    {
-        "Type": WirelessDeviceTypeType,
-        "Name": str,
-        "Description": str,
-        "DestinationName": str,
-        "Id": str,
-        "Arn": str,
-        "ThingName": str,
-        "ThingArn": str,
-        "LoRaWAN": LoRaWANDeviceTypeDef,
-        "Sidewalk": SidewalkDeviceTypeDef,
-        "Positioning": PositioningConfigStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+LoRaWANDeviceUnionTypeDef = Union[LoRaWANDeviceTypeDef, LoRaWANDeviceOutputTypeDef]
 _RequiredUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateWirelessDeviceRequestRequestTypeDef = TypedDict(
@@ -3455,15 +3625,15 @@
 
 DownlinkQueueMessageTypeDef = TypedDict(
     "DownlinkQueueMessageTypeDef",
     {
         "MessageId": str,
         "TransmitMode": int,
         "ReceivedAt": str,
-        "LoRaWAN": LoRaWANSendDataToDeviceTypeDef,
+        "LoRaWAN": LoRaWANSendDataToDeviceOutputTypeDef,
     },
     total=False,
 )
 
 WirelessMetadataTypeDef = TypedDict(
     "WirelessMetadataTypeDef",
     {
@@ -3522,42 +3692,52 @@
 GetWirelessGatewayTaskDefinitionResponseTypeDef = TypedDict(
     "GetWirelessGatewayTaskDefinitionResponseTypeDef",
     {
         "AutoCreateTasks": bool,
         "Name": str,
         "Update": UpdateWirelessGatewayTaskCreateTypeDef,
         "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWirelessGatewayTaskDefinitionsResponseTypeDef = TypedDict(
     "ListWirelessGatewayTaskDefinitionsResponseTypeDef",
     {
         "NextToken": str,
         "TaskDefinitions": List[UpdateWirelessGatewayTaskEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPositionConfigurationsResponseTypeDef = TypedDict(
     "ListPositionConfigurationsResponseTypeDef",
     {
         "PositionConfigurationList": List[PositionConfigurationItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateLogLevelsByResourceTypesRequestRequestTypeDef = TypedDict(
+    "UpdateLogLevelsByResourceTypesRequestRequestTypeDef",
+    {
+        "DefaultLogLevel": LogLevelType,
+        "WirelessDeviceLogOptions": Sequence[WirelessDeviceLogOptionUnionTypeDef],
+        "WirelessGatewayLogOptions": Sequence[WirelessGatewayLogOptionUnionTypeDef],
+    },
+    total=False,
+)
+
 ListQueuedMessagesResponseTypeDef = TypedDict(
     "ListQueuedMessagesResponseTypeDef",
     {
         "NextToken": str,
         "DownlinkQueueMessagesList": List[DownlinkQueueMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSendDataToWirelessDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredSendDataToWirelessDeviceRequestRequestTypeDef",
     {
         "Id": str,
@@ -3582,20 +3762,20 @@
 GetPositionEstimateRequestRequestTypeDef = TypedDict(
     "GetPositionEstimateRequestRequestTypeDef",
     {
         "WiFiAccessPoints": Sequence[WiFiAccessPointTypeDef],
         "CellTowers": CellTowersTypeDef,
         "Ip": IpTypeDef,
         "Gnss": GnssTypeDef,
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
     },
     total=False,
 )
 
 ListEventConfigurationsResponseTypeDef = TypedDict(
     "ListEventConfigurationsResponseTypeDef",
     {
         "NextToken": str,
         "EventConfigurationsList": List[EventConfigurationItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless.egg-info/PKG-INFO` & `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotwireless
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTWireless 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTWireless 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotwireless type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotwireless type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotwireless"></a>
 
 # types-aiobotocore-iotwireless
 
 [![PyPI - types-aiobotocore-iotwireless](https://img.shields.io/pypi/v/types-aiobotocore-iotwireless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotwireless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotwireless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotwireless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotwireless?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotwireless)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotwireless)](https://pepy.tech/project/types-aiobotocore-iotwireless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTWireless 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
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
 [types-aiobotocore-iotwireless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotwireless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -320,60 +319,52 @@
 )
 
 
 def check_value(value: ApplicationConfigTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotwireless.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotwireless.type_defs import (
     SessionKeysAbpV10XTypeDef,
     SessionKeysAbpV11TypeDef,
     AccuracyTypeDef,
     ApplicationConfigTypeDef,
     SidewalkAccountInfoTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef,
     AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     AssociateWirelessDeviceWithThingRequestRequestTypeDef,
     AssociateWirelessGatewayWithCertificateRequestRequestTypeDef,
-    AssociateWirelessGatewayWithCertificateResponseTypeDef,
     AssociateWirelessGatewayWithThingRequestRequestTypeDef,
+    BeaconingOutputTypeDef,
     BeaconingTypeDef,
+    BlobTypeDef,
     CancelMulticastGroupSessionRequestRequestTypeDef,
     CdmaLocalIdTypeDef,
     CdmaNmrObjTypeDef,
     CertificateListTypeDef,
     LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef,
     LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef,
-    CreateDestinationResponseTypeDef,
     LoRaWANDeviceProfileTypeDef,
-    CreateDeviceProfileResponseTypeDef,
     LoRaWANFuotaTaskTypeDef,
-    CreateFuotaTaskResponseTypeDef,
     LoRaWANMulticastTypeDef,
-    CreateMulticastGroupResponseTypeDef,
     TraceContentTypeDef,
-    CreateNetworkAnalyzerConfigurationResponseTypeDef,
     LoRaWANServiceProfileTypeDef,
-    CreateServiceProfileResponseTypeDef,
     SidewalkCreateWirelessDeviceTypeDef,
-    CreateWirelessDeviceResponseTypeDef,
-    CreateWirelessGatewayResponseTypeDef,
-    CreateWirelessGatewayTaskDefinitionResponseTypeDef,
     CreateWirelessGatewayTaskRequestRequestTypeDef,
-    CreateWirelessGatewayTaskResponseTypeDef,
     DakCertificateMetadataTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteDeviceProfileRequestRequestTypeDef,
     DeleteFuotaTaskRequestRequestTypeDef,
     DeleteMulticastGroupRequestRequestTypeDef,
     DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef,
     DeleteQueuedMessagesRequestRequestTypeDef,
@@ -395,54 +386,48 @@
     DisassociateWirelessDeviceFromThingRequestRequestTypeDef,
     DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef,
     DisassociateWirelessGatewayFromThingRequestRequestTypeDef,
     PositioningTypeDef,
     FuotaTaskTypeDef,
     GatewayListItemTypeDef,
     GetDestinationRequestRequestTypeDef,
-    GetDestinationResponseTypeDef,
     GetDeviceProfileRequestRequestTypeDef,
+    LoRaWANDeviceProfileOutputTypeDef,
     GetFuotaTaskRequestRequestTypeDef,
     LoRaWANFuotaTaskGetInfoTypeDef,
     GetMulticastGroupRequestRequestTypeDef,
     LoRaWANMulticastGetTypeDef,
     GetMulticastGroupSessionRequestRequestTypeDef,
-    LoRaWANMulticastSessionTypeDef,
+    LoRaWANMulticastSessionOutputTypeDef,
     GetNetworkAnalyzerConfigurationRequestRequestTypeDef,
     GetPartnerAccountRequestRequestTypeDef,
     SidewalkAccountInfoWithFingerprintTypeDef,
     GetPositionConfigurationRequestRequestTypeDef,
     GnssTypeDef,
     IpTypeDef,
+    TimestampTypeDef,
     WiFiAccessPointTypeDef,
-    GetPositionEstimateResponseTypeDef,
     GetPositionRequestRequestTypeDef,
     GetResourceEventConfigurationRequestRequestTypeDef,
     GetResourceLogLevelRequestRequestTypeDef,
-    GetResourceLogLevelResponseTypeDef,
     GetResourcePositionRequestRequestTypeDef,
-    GetResourcePositionResponseTypeDef,
     GetServiceEndpointRequestRequestTypeDef,
-    GetServiceEndpointResponseTypeDef,
     GetServiceProfileRequestRequestTypeDef,
     LoRaWANGetServiceProfileInfoTypeDef,
     GetWirelessDeviceImportTaskRequestRequestTypeDef,
     SidewalkGetStartImportInfoTypeDef,
     GetWirelessDeviceRequestRequestTypeDef,
     GetWirelessDeviceStatisticsRequestRequestTypeDef,
     SidewalkDeviceMetadataTypeDef,
     GetWirelessGatewayCertificateRequestRequestTypeDef,
-    GetWirelessGatewayCertificateResponseTypeDef,
     GetWirelessGatewayFirmwareInformationRequestRequestTypeDef,
     GetWirelessGatewayRequestRequestTypeDef,
     GetWirelessGatewayStatisticsRequestRequestTypeDef,
-    GetWirelessGatewayStatisticsResponseTypeDef,
     GetWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskRequestRequestTypeDef,
-    GetWirelessGatewayTaskResponseTypeDef,
     GlobalIdentityTypeDef,
     GsmLocalIdTypeDef,
     ImportedSidewalkDeviceTypeDef,
     LoRaWANJoinEventNotificationConfigurationsTypeDef,
     LoRaWANJoinResourceTypeEventConfigurationTypeDef,
     ListDestinationsRequestRequestTypeDef,
     ListDeviceProfilesRequestRequestTypeDef,
@@ -467,57 +452,75 @@
     ListWirelessGatewaysRequestRequestTypeDef,
     LoRaWANGatewayMetadataTypeDef,
     OtaaV10XTypeDef,
     OtaaV11TypeDef,
     LoRaWANGatewayVersionTypeDef,
     LoRaWANListDeviceTypeDef,
     LoRaWANMulticastMetadataTypeDef,
-    LoRaWANStartFuotaTaskTypeDef,
     UpdateAbpV10XTypeDef,
     UpdateAbpV11TypeDef,
     LteLocalIdTypeDef,
     LteNmrObjTypeDef,
     SemtechGnssConfigurationTypeDef,
     SemtechGnssDetailTypeDef,
     PutResourceLogLevelRequestRequestTypeDef,
     ResetResourceLogLevelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    SendDataToMulticastGroupResponseTypeDef,
-    SendDataToWirelessDeviceResponseTypeDef,
     SidewalkSendDataToDeviceTypeDef,
     SidewalkSingleStartImportInfoTypeDef,
     SidewalkStartImportInfoTypeDef,
     SidewalkUpdateAccountTypeDef,
     SidewalkUpdateImportInfoTypeDef,
-    StartSingleWirelessDeviceImportTaskResponseTypeDef,
-    StartWirelessDeviceImportTaskResponseTypeDef,
     TdscdmaLocalIdTypeDef,
     TdscdmaNmrObjTypeDef,
     TestWirelessDeviceRequestRequestTypeDef,
-    TestWirelessDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDestinationRequestRequestTypeDef,
     UpdatePositionRequestRequestTypeDef,
-    UpdateResourcePositionRequestRequestTypeDef,
     UpdateWirelessGatewayRequestRequestTypeDef,
     WcdmaLocalIdTypeDef,
     WcdmaNmrObjTypeDef,
     WirelessDeviceEventLogOptionTypeDef,
     WirelessGatewayEventLogOptionTypeDef,
     AbpV10XTypeDef,
     AbpV11TypeDef,
-    GetPositionResponseTypeDef,
-    AssociateAwsAccountWithPartnerAccountResponseTypeDef,
     AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef,
     StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    AssociateAwsAccountWithPartnerAccountResponseTypeDef,
+    AssociateWirelessGatewayWithCertificateResponseTypeDef,
+    CreateDestinationResponseTypeDef,
+    CreateDeviceProfileResponseTypeDef,
+    CreateFuotaTaskResponseTypeDef,
+    CreateMulticastGroupResponseTypeDef,
+    CreateNetworkAnalyzerConfigurationResponseTypeDef,
+    CreateServiceProfileResponseTypeDef,
+    CreateWirelessDeviceResponseTypeDef,
+    CreateWirelessGatewayResponseTypeDef,
+    CreateWirelessGatewayTaskDefinitionResponseTypeDef,
+    CreateWirelessGatewayTaskResponseTypeDef,
+    GetDestinationResponseTypeDef,
+    GetPositionEstimateResponseTypeDef,
+    GetPositionResponseTypeDef,
+    GetResourceLogLevelResponseTypeDef,
+    GetResourcePositionResponseTypeDef,
+    GetServiceEndpointResponseTypeDef,
+    GetWirelessGatewayCertificateResponseTypeDef,
+    GetWirelessGatewayStatisticsResponseTypeDef,
+    GetWirelessGatewayTaskResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SendDataToMulticastGroupResponseTypeDef,
+    SendDataToWirelessDeviceResponseTypeDef,
+    StartSingleWirelessDeviceImportTaskResponseTypeDef,
+    StartWirelessDeviceImportTaskResponseTypeDef,
+    TestWirelessDeviceResponseTypeDef,
+    LoRaWANGatewayOutputTypeDef,
     LoRaWANGatewayTypeDef,
+    UpdateResourcePositionRequestRequestTypeDef,
     CdmaObjTypeDef,
     SidewalkDeviceTypeDef,
     SidewalkListDeviceTypeDef,
     ConnectionStatusEventConfigurationTypeDef,
     ConnectionStatusResourceTypeEventConfigurationTypeDef,
     CreateDeviceProfileRequestRequestTypeDef,
     CreateFuotaTaskRequestRequestTypeDef,
@@ -533,24 +536,28 @@
     ListDeviceProfilesResponseTypeDef,
     DeviceRegistrationStateEventConfigurationTypeDef,
     MessageDeliveryStatusEventConfigurationTypeDef,
     ProximityEventConfigurationTypeDef,
     DeviceRegistrationStateResourceTypeEventConfigurationTypeDef,
     MessageDeliveryStatusResourceTypeEventConfigurationTypeDef,
     ProximityResourceTypeEventConfigurationTypeDef,
+    FPortsOutputTypeDef,
     FPortsTypeDef,
     UpdateFPortsTypeDef,
     ListFuotaTasksResponseTypeDef,
+    ParticipatingGatewaysOutputTypeDef,
     ParticipatingGatewaysTypeDef,
+    LoRaWANDeviceProfileUnionTypeDef,
     GetFuotaTaskResponseTypeDef,
     GetMulticastGroupResponseTypeDef,
     GetMulticastGroupSessionResponseTypeDef,
-    StartMulticastGroupSessionRequestRequestTypeDef,
     GetPartnerAccountResponseTypeDef,
     ListPartnerAccountsResponseTypeDef,
+    LoRaWANMulticastSessionTypeDef,
+    LoRaWANStartFuotaTaskTypeDef,
     GetServiceProfileResponseTypeDef,
     GetWirelessDeviceImportTaskResponseTypeDef,
     WirelessDeviceImportTaskTypeDef,
     GsmNmrObjTypeDef,
     ImportedWirelessDeviceTypeDef,
     JoinEventConfigurationTypeDef,
     JoinResourceTypeEventConfigurationTypeDef,
@@ -559,34 +566,41 @@
     ListNetworkAnalyzerConfigurationsResponseTypeDef,
     ListServiceProfilesResponseTypeDef,
     LoRaWANDeviceMetadataTypeDef,
     LoRaWANGatewayCurrentVersionTypeDef,
     LoRaWANUpdateGatewayTaskCreateTypeDef,
     LoRaWANUpdateGatewayTaskEntryTypeDef,
     MulticastWirelessMetadataTypeDef,
-    StartFuotaTaskRequestRequestTypeDef,
     LteObjTypeDef,
     PositionSolverConfigurationsTypeDef,
     PositionSolverDetailsTypeDef,
     StartSingleWirelessDeviceImportTaskRequestRequestTypeDef,
     StartWirelessDeviceImportTaskRequestRequestTypeDef,
     UpdatePartnerAccountRequestRequestTypeDef,
     UpdateWirelessDeviceImportTaskRequestRequestTypeDef,
     TdscdmaObjTypeDef,
     WcdmaObjTypeDef,
+    WirelessDeviceLogOptionOutputTypeDef,
     WirelessDeviceLogOptionTypeDef,
+    WirelessGatewayLogOptionOutputTypeDef,
     WirelessGatewayLogOptionTypeDef,
-    CreateWirelessGatewayRequestRequestTypeDef,
     GetWirelessGatewayResponseTypeDef,
     WirelessGatewayStatisticsTypeDef,
+    CreateWirelessGatewayRequestRequestTypeDef,
+    LoRaWANGatewayUnionTypeDef,
     WirelessDeviceStatisticsTypeDef,
     GetDeviceProfileResponseTypeDef,
+    LoRaWANDeviceOutputTypeDef,
     LoRaWANDeviceTypeDef,
     LoRaWANUpdateDeviceTypeDef,
+    LoRaWANSendDataToDeviceOutputTypeDef,
     LoRaWANSendDataToDeviceTypeDef,
+    LoRaWANMulticastSessionUnionTypeDef,
+    StartMulticastGroupSessionRequestRequestTypeDef,
+    StartFuotaTaskRequestRequestTypeDef,
     ListWirelessDeviceImportTasksResponseTypeDef,
     GsmObjTypeDef,
     ListDevicesForWirelessDeviceImportTaskResponseTypeDef,
     EventNotificationItemConfigurationsTypeDef,
     GetResourceEventConfigurationResponseTypeDef,
     UpdateResourceEventConfigurationRequestRequestTypeDef,
     GetEventConfigurationByResourceTypesResponseTypeDef,
@@ -595,37 +609,40 @@
     GetWirelessGatewayFirmwareInformationResponseTypeDef,
     UpdateWirelessGatewayTaskCreateTypeDef,
     UpdateWirelessGatewayTaskEntryTypeDef,
     SendDataToMulticastGroupRequestRequestTypeDef,
     PutPositionConfigurationRequestRequestTypeDef,
     GetPositionConfigurationResponseTypeDef,
     PositionConfigurationItemTypeDef,
+    WirelessDeviceLogOptionUnionTypeDef,
     GetLogLevelsByResourceTypesResponseTypeDef,
-    UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
+    WirelessGatewayLogOptionUnionTypeDef,
     ListWirelessGatewaysResponseTypeDef,
     ListWirelessDevicesResponseTypeDef,
-    CreateWirelessDeviceRequestRequestTypeDef,
     GetWirelessDeviceResponseTypeDef,
+    CreateWirelessDeviceRequestRequestTypeDef,
+    LoRaWANDeviceUnionTypeDef,
     UpdateWirelessDeviceRequestRequestTypeDef,
     DownlinkQueueMessageTypeDef,
     WirelessMetadataTypeDef,
     CellTowersTypeDef,
     EventConfigurationItemTypeDef,
     CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef,
     GetWirelessGatewayTaskDefinitionResponseTypeDef,
     ListWirelessGatewayTaskDefinitionsResponseTypeDef,
     ListPositionConfigurationsResponseTypeDef,
+    UpdateLogLevelsByResourceTypesRequestRequestTypeDef,
     ListQueuedMessagesResponseTypeDef,
     SendDataToWirelessDeviceRequestRequestTypeDef,
     GetPositionEstimateRequestRequestTypeDef,
     ListEventConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> SessionKeysAbpV10XTypeDef:
+def get_value() -> SessionKeysAbpV10XTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotwireless-2.5.2/types_aiobotocore_iotwireless.egg-info/SOURCES.txt` & `types-aiobotocore-iotwireless-2.5.2.post1/types_aiobotocore_iotwireless.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-iotfleetwise-2.5.2.tar.gz` & `tmp/types-aiobotocore-iotfleetwise-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotfleetwise-2.5.2.tar", last modified: Sat Jul  8 01:43:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotfleetwise-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
```

## Comparing `types-aiobotocore-iotfleetwise-2.5.2.tar` & `types-aiobotocore-iotfleetwise-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.834305 types-aiobotocore-iotfleetwise-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:47.000000 types-aiobotocore-iotfleetwise-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21868 2023-07-08 01:43:46.830305 types-aiobotocore-iotfleetwise-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20283 2023-07-08 01:32:47.000000 types-aiobotocore-iotfleetwise-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:46.834305 types-aiobotocore-iotfleetwise-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:32:47.000000 types-aiobotocore-iotfleetwise-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.822305 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-08 01:32:47.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-08 01:32:47.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:32:47.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43363 2023-07-08 01:32:48.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43291 2023-07-08 01:32:48.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-08 01:32:48.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-07-08 01:32:48.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-07-08 01:32:48.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16204 2023-07-08 01:32:48.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:47.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58211 2023-07-08 01:32:49.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58111 2023-07-08 01:32:49.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:47.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.830305 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21868 2023-07-08 01:43:46.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:46.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:46.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:46.000000 types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.745562 types-aiobotocore-iotfleetwise-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-08-02 14:52:26.745562 types-aiobotocore-iotfleetwise-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.745562 types-aiobotocore-iotfleetwise-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.741562 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43360 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43288 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16193 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16178 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60490 2023-08-02 14:40:51.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60384 2023-08-02 14:40:51.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:50.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.745562 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:26.000000 types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/LICENSE` & `types-aiobotocore-iotfleetwise-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/PKG-INFO` & `types-aiobotocore-iotfleetwise-2.5.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotfleetwise
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTFleetWise 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTFleetWise 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotfleetwise type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotfleetwise type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotfleetwise"></a>
 
 # types-aiobotocore-iotfleetwise
 
 [![PyPI - types-aiobotocore-iotfleetwise](https://img.shields.io/pypi/v/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotfleetwise?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotfleetwise)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotfleetwise)](https://pepy.tech/project/types-aiobotocore-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTFleetWise 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [types-aiobotocore-iotfleetwise docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/).
 
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
@@ -380,136 +379,127 @@
 )
 
 
 def check_value(value: CampaignStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotfleetwise.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotfleetwise.type_defs import (
+    ActuatorOutputTypeDef,
     ActuatorTypeDef,
     AssociateVehicleFleetRequestRequestTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateVehicleErrorTypeDef,
     CreateVehicleResponseItemTypeDef,
+    ResponseMetadataTypeDef,
     UpdateVehicleRequestItemTypeDef,
     UpdateVehicleErrorTypeDef,
     UpdateVehicleResponseItemTypeDef,
+    BlobTypeDef,
     BranchTypeDef,
     CampaignSummaryTypeDef,
-    CanDbcDefinitionTypeDef,
     CanInterfaceTypeDef,
     CanSignalTypeDef,
     CloudWatchLogDeliveryOptionsTypeDef,
     ConditionBasedCollectionSchemeTypeDef,
     TimeBasedCollectionSchemeTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDecoderManifestResponseTypeDef,
-    CreateFleetResponseTypeDef,
-    CreateModelManifestResponseTypeDef,
-    CreateSignalCatalogResponseTypeDef,
-    CreateVehicleResponseTypeDef,
+    TimestampTypeDef,
     S3ConfigTypeDef,
     TimestreamConfigTypeDef,
     DecoderManifestSummaryTypeDef,
     DeleteCampaignRequestRequestTypeDef,
-    DeleteCampaignResponseTypeDef,
     DeleteDecoderManifestRequestRequestTypeDef,
-    DeleteDecoderManifestResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
-    DeleteFleetResponseTypeDef,
     DeleteModelManifestRequestRequestTypeDef,
-    DeleteModelManifestResponseTypeDef,
     DeleteSignalCatalogRequestRequestTypeDef,
-    DeleteSignalCatalogResponseTypeDef,
     DeleteVehicleRequestRequestTypeDef,
-    DeleteVehicleResponseTypeDef,
     DisassociateVehicleFleetRequestRequestTypeDef,
     FleetSummaryTypeDef,
     FormattedVssTypeDef,
     GetCampaignRequestRequestTypeDef,
     GetDecoderManifestRequestRequestTypeDef,
-    GetDecoderManifestResponseTypeDef,
     GetFleetRequestRequestTypeDef,
-    GetFleetResponseTypeDef,
     GetModelManifestRequestRequestTypeDef,
-    GetModelManifestResponseTypeDef,
     IamRegistrationResponseTypeDef,
     TimestreamRegistrationResponseTypeDef,
     GetSignalCatalogRequestRequestTypeDef,
     NodeCountsTypeDef,
     GetVehicleRequestRequestTypeDef,
-    GetVehicleResponseTypeDef,
-    GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetVehicleStatusRequestRequestTypeDef,
     VehicleStatusTypeDef,
     IamResourcesTypeDef,
-    ImportDecoderManifestResponseTypeDef,
-    ImportSignalCatalogResponseTypeDef,
-    ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
-    ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
     ListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
-    ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
     ListDecoderManifestSignalsRequestRequestTypeDef,
-    ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef,
     ListDecoderManifestsRequestRequestTypeDef,
-    ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
     ListFleetsForVehicleRequestRequestTypeDef,
-    ListFleetsForVehicleResponseTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
-    ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
     ListModelManifestNodesRequestRequestTypeDef,
-    ListModelManifestsRequestListModelManifestsPaginateTypeDef,
     ListModelManifestsRequestRequestTypeDef,
     ModelManifestSummaryTypeDef,
-    ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
     ListSignalCatalogNodesRequestRequestTypeDef,
-    ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
     ListSignalCatalogsRequestRequestTypeDef,
     SignalCatalogSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
     ListVehiclesInFleetRequestRequestTypeDef,
-    ListVehiclesInFleetResponseTypeDef,
-    ListVehiclesRequestListVehiclesPaginateTypeDef,
     ListVehiclesRequestRequestTypeDef,
     VehicleSummaryTypeDef,
     ObdInterfaceTypeDef,
+    SensorOutputTypeDef,
     SensorTypeDef,
     ObdSignalTypeDef,
-    PaginatorConfigTypeDef,
     TimestreamResourcesTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignRequestRequestTypeDef,
+    UpdateFleetRequestRequestTypeDef,
+    UpdateModelManifestRequestRequestTypeDef,
+    UpdateVehicleRequestRequestTypeDef,
+    BatchCreateVehicleResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDecoderManifestResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    CreateModelManifestResponseTypeDef,
+    CreateSignalCatalogResponseTypeDef,
+    CreateVehicleResponseTypeDef,
+    DeleteCampaignResponseTypeDef,
+    DeleteDecoderManifestResponseTypeDef,
+    DeleteFleetResponseTypeDef,
+    DeleteModelManifestResponseTypeDef,
+    DeleteSignalCatalogResponseTypeDef,
+    DeleteVehicleResponseTypeDef,
+    GetDecoderManifestResponseTypeDef,
+    GetFleetResponseTypeDef,
+    GetModelManifestResponseTypeDef,
+    GetVehicleResponseTypeDef,
+    ImportDecoderManifestResponseTypeDef,
+    ImportSignalCatalogResponseTypeDef,
+    ListFleetsForVehicleResponseTypeDef,
+    ListVehiclesInFleetResponseTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
-    UpdateFleetRequestRequestTypeDef,
     UpdateFleetResponseTypeDef,
-    UpdateModelManifestRequestRequestTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
-    UpdateVehicleRequestRequestTypeDef,
     UpdateVehicleResponseTypeDef,
-    BatchCreateVehicleResponseTypeDef,
     BatchUpdateVehicleRequestRequestTypeDef,
     BatchUpdateVehicleResponseTypeDef,
+    CanDbcDefinitionTypeDef,
     ListCampaignsResponseTypeDef,
-    NetworkFileDefinitionTypeDef,
     GetLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     CollectionSchemeTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateModelManifestRequestRequestTypeDef,
     CreateVehicleRequestItemTypeDef,
     CreateVehicleRequestRequestTypeDef,
@@ -517,39 +507,55 @@
     TagResourceRequestRequestTypeDef,
     DataDestinationConfigTypeDef,
     ListDecoderManifestsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ImportSignalCatalogRequestRequestTypeDef,
     GetRegisterAccountStatusResponseTypeDef,
     GetSignalCatalogResponseTypeDef,
+    GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    ListCampaignsRequestListCampaignsPaginateTypeDef,
+    ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+    ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+    ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef,
+    ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
+    ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+    ListModelManifestsRequestListModelManifestsPaginateTypeDef,
+    ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+    ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
+    ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+    ListVehiclesRequestListVehiclesPaginateTypeDef,
     GetVehicleStatusResponseTypeDef,
     ListModelManifestsResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
     ListVehiclesResponseTypeDef,
     NetworkInterfaceTypeDef,
+    NodeOutputTypeDef,
     NodeTypeDef,
     SignalDecoderTypeDef,
     RegisterAccountRequestRequestTypeDef,
     RegisterAccountResponseTypeDef,
-    ImportDecoderManifestRequestRequestTypeDef,
+    NetworkFileDefinitionTypeDef,
     BatchCreateVehicleRequestRequestTypeDef,
     CreateCampaignRequestRequestTypeDef,
     GetCampaignResponseTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
-    CreateSignalCatalogRequestRequestTypeDef,
     ListModelManifestNodesResponseTypeDef,
     ListSignalCatalogNodesResponseTypeDef,
-    UpdateSignalCatalogRequestRequestTypeDef,
+    NodeUnionTypeDef,
     CreateDecoderManifestRequestRequestTypeDef,
     ListDecoderManifestSignalsResponseTypeDef,
     UpdateDecoderManifestRequestRequestTypeDef,
+    ImportDecoderManifestRequestRequestTypeDef,
+    CreateSignalCatalogRequestRequestTypeDef,
+    UpdateSignalCatalogRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActuatorTypeDef:
+def get_value() -> ActuatorOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/README.md` & `types-aiobotocore-iotfleetwise-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iotfleetwise"></a>
 
 # types-aiobotocore-iotfleetwise
 
 [![PyPI - types-aiobotocore-iotfleetwise](https://img.shields.io/pypi/v/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotfleetwise?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotfleetwise)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotfleetwise)](https://pepy.tech/project/types-aiobotocore-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTFleetWise 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [types-aiobotocore-iotfleetwise docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/).
 
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
@@ -347,136 +347,127 @@
 )
 
 
 def check_value(value: CampaignStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotfleetwise.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotfleetwise.type_defs import (
+    ActuatorOutputTypeDef,
     ActuatorTypeDef,
     AssociateVehicleFleetRequestRequestTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateVehicleErrorTypeDef,
     CreateVehicleResponseItemTypeDef,
+    ResponseMetadataTypeDef,
     UpdateVehicleRequestItemTypeDef,
     UpdateVehicleErrorTypeDef,
     UpdateVehicleResponseItemTypeDef,
+    BlobTypeDef,
     BranchTypeDef,
     CampaignSummaryTypeDef,
-    CanDbcDefinitionTypeDef,
     CanInterfaceTypeDef,
     CanSignalTypeDef,
     CloudWatchLogDeliveryOptionsTypeDef,
     ConditionBasedCollectionSchemeTypeDef,
     TimeBasedCollectionSchemeTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDecoderManifestResponseTypeDef,
-    CreateFleetResponseTypeDef,
-    CreateModelManifestResponseTypeDef,
-    CreateSignalCatalogResponseTypeDef,
-    CreateVehicleResponseTypeDef,
+    TimestampTypeDef,
     S3ConfigTypeDef,
     TimestreamConfigTypeDef,
     DecoderManifestSummaryTypeDef,
     DeleteCampaignRequestRequestTypeDef,
-    DeleteCampaignResponseTypeDef,
     DeleteDecoderManifestRequestRequestTypeDef,
-    DeleteDecoderManifestResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
-    DeleteFleetResponseTypeDef,
     DeleteModelManifestRequestRequestTypeDef,
-    DeleteModelManifestResponseTypeDef,
     DeleteSignalCatalogRequestRequestTypeDef,
-    DeleteSignalCatalogResponseTypeDef,
     DeleteVehicleRequestRequestTypeDef,
-    DeleteVehicleResponseTypeDef,
     DisassociateVehicleFleetRequestRequestTypeDef,
     FleetSummaryTypeDef,
     FormattedVssTypeDef,
     GetCampaignRequestRequestTypeDef,
     GetDecoderManifestRequestRequestTypeDef,
-    GetDecoderManifestResponseTypeDef,
     GetFleetRequestRequestTypeDef,
-    GetFleetResponseTypeDef,
     GetModelManifestRequestRequestTypeDef,
-    GetModelManifestResponseTypeDef,
     IamRegistrationResponseTypeDef,
     TimestreamRegistrationResponseTypeDef,
     GetSignalCatalogRequestRequestTypeDef,
     NodeCountsTypeDef,
     GetVehicleRequestRequestTypeDef,
-    GetVehicleResponseTypeDef,
-    GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetVehicleStatusRequestRequestTypeDef,
     VehicleStatusTypeDef,
     IamResourcesTypeDef,
-    ImportDecoderManifestResponseTypeDef,
-    ImportSignalCatalogResponseTypeDef,
-    ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
-    ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
     ListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
-    ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
     ListDecoderManifestSignalsRequestRequestTypeDef,
-    ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef,
     ListDecoderManifestsRequestRequestTypeDef,
-    ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
     ListFleetsForVehicleRequestRequestTypeDef,
-    ListFleetsForVehicleResponseTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
-    ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
     ListModelManifestNodesRequestRequestTypeDef,
-    ListModelManifestsRequestListModelManifestsPaginateTypeDef,
     ListModelManifestsRequestRequestTypeDef,
     ModelManifestSummaryTypeDef,
-    ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
     ListSignalCatalogNodesRequestRequestTypeDef,
-    ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
     ListSignalCatalogsRequestRequestTypeDef,
     SignalCatalogSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
     ListVehiclesInFleetRequestRequestTypeDef,
-    ListVehiclesInFleetResponseTypeDef,
-    ListVehiclesRequestListVehiclesPaginateTypeDef,
     ListVehiclesRequestRequestTypeDef,
     VehicleSummaryTypeDef,
     ObdInterfaceTypeDef,
+    SensorOutputTypeDef,
     SensorTypeDef,
     ObdSignalTypeDef,
-    PaginatorConfigTypeDef,
     TimestreamResourcesTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignRequestRequestTypeDef,
+    UpdateFleetRequestRequestTypeDef,
+    UpdateModelManifestRequestRequestTypeDef,
+    UpdateVehicleRequestRequestTypeDef,
+    BatchCreateVehicleResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDecoderManifestResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    CreateModelManifestResponseTypeDef,
+    CreateSignalCatalogResponseTypeDef,
+    CreateVehicleResponseTypeDef,
+    DeleteCampaignResponseTypeDef,
+    DeleteDecoderManifestResponseTypeDef,
+    DeleteFleetResponseTypeDef,
+    DeleteModelManifestResponseTypeDef,
+    DeleteSignalCatalogResponseTypeDef,
+    DeleteVehicleResponseTypeDef,
+    GetDecoderManifestResponseTypeDef,
+    GetFleetResponseTypeDef,
+    GetModelManifestResponseTypeDef,
+    GetVehicleResponseTypeDef,
+    ImportDecoderManifestResponseTypeDef,
+    ImportSignalCatalogResponseTypeDef,
+    ListFleetsForVehicleResponseTypeDef,
+    ListVehiclesInFleetResponseTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
-    UpdateFleetRequestRequestTypeDef,
     UpdateFleetResponseTypeDef,
-    UpdateModelManifestRequestRequestTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
-    UpdateVehicleRequestRequestTypeDef,
     UpdateVehicleResponseTypeDef,
-    BatchCreateVehicleResponseTypeDef,
     BatchUpdateVehicleRequestRequestTypeDef,
     BatchUpdateVehicleResponseTypeDef,
+    CanDbcDefinitionTypeDef,
     ListCampaignsResponseTypeDef,
-    NetworkFileDefinitionTypeDef,
     GetLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     CollectionSchemeTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateModelManifestRequestRequestTypeDef,
     CreateVehicleRequestItemTypeDef,
     CreateVehicleRequestRequestTypeDef,
@@ -484,39 +475,55 @@
     TagResourceRequestRequestTypeDef,
     DataDestinationConfigTypeDef,
     ListDecoderManifestsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ImportSignalCatalogRequestRequestTypeDef,
     GetRegisterAccountStatusResponseTypeDef,
     GetSignalCatalogResponseTypeDef,
+    GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    ListCampaignsRequestListCampaignsPaginateTypeDef,
+    ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+    ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+    ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef,
+    ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
+    ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+    ListModelManifestsRequestListModelManifestsPaginateTypeDef,
+    ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+    ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
+    ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+    ListVehiclesRequestListVehiclesPaginateTypeDef,
     GetVehicleStatusResponseTypeDef,
     ListModelManifestsResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
     ListVehiclesResponseTypeDef,
     NetworkInterfaceTypeDef,
+    NodeOutputTypeDef,
     NodeTypeDef,
     SignalDecoderTypeDef,
     RegisterAccountRequestRequestTypeDef,
     RegisterAccountResponseTypeDef,
-    ImportDecoderManifestRequestRequestTypeDef,
+    NetworkFileDefinitionTypeDef,
     BatchCreateVehicleRequestRequestTypeDef,
     CreateCampaignRequestRequestTypeDef,
     GetCampaignResponseTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
-    CreateSignalCatalogRequestRequestTypeDef,
     ListModelManifestNodesResponseTypeDef,
     ListSignalCatalogNodesResponseTypeDef,
-    UpdateSignalCatalogRequestRequestTypeDef,
+    NodeUnionTypeDef,
     CreateDecoderManifestRequestRequestTypeDef,
     ListDecoderManifestSignalsResponseTypeDef,
     UpdateDecoderManifestRequestRequestTypeDef,
+    ImportDecoderManifestRequestRequestTypeDef,
+    CreateSignalCatalogRequestRequestTypeDef,
+    UpdateSignalCatalogRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActuatorTypeDef:
+def get_value() -> ActuatorOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/setup.py` & `types-aiobotocore-iotfleetwise-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotfleetwise",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iotfleetwise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTFleetWise 2.5.2 service generated with"
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
-    keywords="aiobotocore iotfleetwise type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore iotfleetwise type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotfleetwise": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/"
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/__init__.py` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/__init__.pyi` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/__main__.py` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTFleetWise 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IoTFleetWise 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise\nOther"
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

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/client.py` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("iotfleetwise") as client:
         client: IoTFleetWiseClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     CompressionType,
     DiagnosticsModeType,
@@ -88,19 +87,20 @@
     ListSignalCatalogNodesResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVehiclesInFleetResponseTypeDef,
     ListVehiclesResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     NetworkInterfaceTypeDef,
-    NodeTypeDef,
+    NodeUnionTypeDef,
     RegisterAccountResponseTypeDef,
     SignalDecoderTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TimestreamResourcesTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
     UpdateFleetResponseTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
     UpdateVehicleRequestItemTypeDef,
@@ -203,16 +203,16 @@
         self,
         *,
         name: str,
         signalCatalogArn: str,
         targetArn: str,
         collectionScheme: CollectionSchemeTypeDef,
         description: str = ...,
-        startTime: Union[datetime, str] = ...,
-        expiryTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        expiryTime: TimestampTypeDef = ...,
         postTriggerCollectionDuration: int = ...,
         diagnosticsMode: DiagnosticsModeType = ...,
         spoolingMode: SpoolingModeType = ...,
         compression: CompressionType = ...,
         priority: int = ...,
         signalsToCollect: Sequence[SignalInformationTypeDef] = ...,
         dataExtraDimensions: Sequence[str] = ...,
@@ -276,15 +276,15 @@
         """
 
     async def create_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodes: Sequence[NodeTypeDef] = ...,
+        nodes: Sequence[NodeUnionTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSignalCatalogResponseTypeDef:
         """
         Creates a collection of standardized signals that can be reused to create
         vehicle models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_signal_catalog)
@@ -713,16 +713,16 @@
         """
 
     async def update_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodesToAdd: Sequence[NodeTypeDef] = ...,
-        nodesToUpdate: Sequence[NodeTypeDef] = ...,
+        nodesToAdd: Sequence[NodeUnionTypeDef] = ...,
+        nodesToUpdate: Sequence[NodeUnionTypeDef] = ...,
         nodesToRemove: Sequence[str] = ...
     ) -> UpdateSignalCatalogResponseTypeDef:
         """
         Updates a signal catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_signal_catalog)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_signal_catalog)
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/client.pyi` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("iotfleetwise") as client:
         client: IoTFleetWiseClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     CompressionType,
     DiagnosticsModeType,
@@ -88,19 +87,20 @@
     ListSignalCatalogNodesResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVehiclesInFleetResponseTypeDef,
     ListVehiclesResponseTypeDef,
     NetworkFileDefinitionTypeDef,
     NetworkInterfaceTypeDef,
-    NodeTypeDef,
+    NodeUnionTypeDef,
     RegisterAccountResponseTypeDef,
     SignalDecoderTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     TimestreamResourcesTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
     UpdateFleetResponseTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
     UpdateVehicleRequestItemTypeDef,
@@ -193,16 +193,16 @@
         self,
         *,
         name: str,
         signalCatalogArn: str,
         targetArn: str,
         collectionScheme: CollectionSchemeTypeDef,
         description: str = ...,
-        startTime: Union[datetime, str] = ...,
-        expiryTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        expiryTime: TimestampTypeDef = ...,
         postTriggerCollectionDuration: int = ...,
         diagnosticsMode: DiagnosticsModeType = ...,
         spoolingMode: SpoolingModeType = ...,
         compression: CompressionType = ...,
         priority: int = ...,
         signalsToCollect: Sequence[SignalInformationTypeDef] = ...,
         dataExtraDimensions: Sequence[str] = ...,
@@ -262,15 +262,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#create_model_manifest)
         """
     async def create_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodes: Sequence[NodeTypeDef] = ...,
+        nodes: Sequence[NodeUnionTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateSignalCatalogResponseTypeDef:
         """
         Creates a collection of standardized signals that can be reused to create
         vehicle models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.create_signal_catalog)
@@ -657,16 +657,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_model_manifest)
         """
     async def update_signal_catalog(
         self,
         *,
         name: str,
         description: str = ...,
-        nodesToAdd: Sequence[NodeTypeDef] = ...,
-        nodesToUpdate: Sequence[NodeTypeDef] = ...,
+        nodesToAdd: Sequence[NodeUnionTypeDef] = ...,
+        nodesToUpdate: Sequence[NodeUnionTypeDef] = ...,
         nodesToRemove: Sequence[str] = ...
     ) -> UpdateSignalCatalogResponseTypeDef:
         """
         Updates a signal catalog.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client.update_signal_catalog)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/client/#update_signal_catalog)
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/literals.py` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/literals.pyi` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/paginator.py` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,193 +96,193 @@
 class GetVehicleStatusPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.GetVehicleStatus)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#getvehiclestatuspaginator)
     """
 
     def paginate(
-        self, *, vehicleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, vehicleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetVehicleStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.GetVehicleStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#getvehiclestatuspaginator)
         """
 
 
 class ListCampaignsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListCampaigns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listcampaignspaginator)
     """
 
     def paginate(
-        self, *, status: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListCampaigns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listcampaignspaginator)
         """
 
 
 class ListDecoderManifestNetworkInterfacesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestNetworkInterfaces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listdecodermanifestnetworkinterfacespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDecoderManifestNetworkInterfacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestNetworkInterfaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listdecodermanifestnetworkinterfacespaginator)
         """
 
 
 class ListDecoderManifestSignalsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestSignals)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listdecodermanifestsignalspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDecoderManifestSignalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestSignals.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listdecodermanifestsignalspaginator)
         """
 
 
 class ListDecoderManifestsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifests)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listdecodermanifestspaginator)
     """
 
     def paginate(
-        self, *, modelManifestArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, modelManifestArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDecoderManifestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listdecodermanifestspaginator)
         """
 
 
 class ListFleetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listfleetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listfleetspaginator)
         """
 
 
 class ListFleetsForVehiclePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleetsForVehicle)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listfleetsforvehiclepaginator)
     """
 
     def paginate(
-        self, *, vehicleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, vehicleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFleetsForVehicleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleetsForVehicle.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listfleetsforvehiclepaginator)
         """
 
 
 class ListModelManifestNodesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifestNodes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listmodelmanifestnodespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListModelManifestNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifestNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listmodelmanifestnodespaginator)
         """
 
 
 class ListModelManifestsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifests)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listmodelmanifestspaginator)
     """
 
     def paginate(
-        self, *, signalCatalogArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, signalCatalogArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListModelManifestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listmodelmanifestspaginator)
         """
 
 
 class ListSignalCatalogNodesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listsignalcatalognodespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSignalCatalogNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listsignalcatalognodespaginator)
         """
 
 
 class ListSignalCatalogsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listsignalcatalogspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSignalCatalogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listsignalcatalogspaginator)
         """
 
 
 class ListVehiclesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehicles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listvehiclespaginator)
     """
 
     def paginate(
-        self, *, modelManifestArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, modelManifestArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVehiclesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehicles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listvehiclespaginator)
         """
 
 
 class ListVehiclesInFleetPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehiclesInFleet)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listvehiclesinfleetpaginator)
     """
 
     def paginate(
-        self, *, fleetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, fleetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVehiclesInFleetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehiclesInFleet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listvehiclesinfleetpaginator)
         """
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/paginator.pyi` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -93,181 +93,181 @@
 class GetVehicleStatusPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.GetVehicleStatus)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#getvehiclestatuspaginator)
     """
 
     def paginate(
-        self, *, vehicleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, vehicleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetVehicleStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.GetVehicleStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#getvehiclestatuspaginator)
         """
 
 class ListCampaignsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListCampaigns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listcampaignspaginator)
     """
 
     def paginate(
-        self, *, status: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCampaignsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListCampaigns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listcampaignspaginator)
         """
 
 class ListDecoderManifestNetworkInterfacesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestNetworkInterfaces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listdecodermanifestnetworkinterfacespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDecoderManifestNetworkInterfacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestNetworkInterfaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listdecodermanifestnetworkinterfacespaginator)
         """
 
 class ListDecoderManifestSignalsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestSignals)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listdecodermanifestsignalspaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDecoderManifestSignalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestSignals.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listdecodermanifestsignalspaginator)
         """
 
 class ListDecoderManifestsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifests)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listdecodermanifestspaginator)
     """
 
     def paginate(
-        self, *, modelManifestArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, modelManifestArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDecoderManifestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listdecodermanifestspaginator)
         """
 
 class ListFleetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listfleetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listfleetspaginator)
         """
 
 class ListFleetsForVehiclePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleetsForVehicle)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listfleetsforvehiclepaginator)
     """
 
     def paginate(
-        self, *, vehicleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, vehicleName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFleetsForVehicleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleetsForVehicle.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listfleetsforvehiclepaginator)
         """
 
 class ListModelManifestNodesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifestNodes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listmodelmanifestnodespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListModelManifestNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifestNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listmodelmanifestnodespaginator)
         """
 
 class ListModelManifestsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifests)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listmodelmanifestspaginator)
     """
 
     def paginate(
-        self, *, signalCatalogArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, signalCatalogArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListModelManifestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listmodelmanifestspaginator)
         """
 
 class ListSignalCatalogNodesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listsignalcatalognodespaginator)
     """
 
     def paginate(
-        self, *, name: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSignalCatalogNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listsignalcatalognodespaginator)
         """
 
 class ListSignalCatalogsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listsignalcatalogspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSignalCatalogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listsignalcatalogspaginator)
         """
 
 class ListVehiclesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehicles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listvehiclespaginator)
     """
 
     def paginate(
-        self, *, modelManifestArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, modelManifestArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVehiclesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehicles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listvehiclespaginator)
         """
 
 class ListVehiclesInFleetPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehiclesInFleet)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listvehiclesinfleetpaginator)
     """
 
     def paginate(
-        self, *, fleetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, fleetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVehiclesInFleetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehiclesInFleet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/paginators/#listvehiclesinfleetpaginator)
         """
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/type_defs.py` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotfleetwise service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_iotfleetwise.type_defs import ActuatorTypeDef
+    from types_aiobotocore_iotfleetwise.type_defs import ActuatorOutputTypeDef
 
-    data: ActuatorTypeDef = {...}
+    data: ActuatorOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -40,127 +40,118 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ActuatorOutputTypeDef",
     "ActuatorTypeDef",
     "AssociateVehicleFleetRequestRequestTypeDef",
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CreateVehicleErrorTypeDef",
     "CreateVehicleResponseItemTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateVehicleRequestItemTypeDef",
     "UpdateVehicleErrorTypeDef",
     "UpdateVehicleResponseItemTypeDef",
+    "BlobTypeDef",
     "BranchTypeDef",
     "CampaignSummaryTypeDef",
-    "CanDbcDefinitionTypeDef",
     "CanInterfaceTypeDef",
     "CanSignalTypeDef",
     "CloudWatchLogDeliveryOptionsTypeDef",
     "ConditionBasedCollectionSchemeTypeDef",
     "TimeBasedCollectionSchemeTypeDef",
     "SignalInformationTypeDef",
     "TagTypeDef",
-    "CreateCampaignResponseTypeDef",
-    "CreateDecoderManifestResponseTypeDef",
-    "CreateFleetResponseTypeDef",
-    "CreateModelManifestResponseTypeDef",
-    "CreateSignalCatalogResponseTypeDef",
-    "CreateVehicleResponseTypeDef",
+    "TimestampTypeDef",
     "S3ConfigTypeDef",
     "TimestreamConfigTypeDef",
     "DecoderManifestSummaryTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
-    "DeleteCampaignResponseTypeDef",
     "DeleteDecoderManifestRequestRequestTypeDef",
-    "DeleteDecoderManifestResponseTypeDef",
     "DeleteFleetRequestRequestTypeDef",
-    "DeleteFleetResponseTypeDef",
     "DeleteModelManifestRequestRequestTypeDef",
-    "DeleteModelManifestResponseTypeDef",
     "DeleteSignalCatalogRequestRequestTypeDef",
-    "DeleteSignalCatalogResponseTypeDef",
     "DeleteVehicleRequestRequestTypeDef",
-    "DeleteVehicleResponseTypeDef",
     "DisassociateVehicleFleetRequestRequestTypeDef",
     "FleetSummaryTypeDef",
     "FormattedVssTypeDef",
     "GetCampaignRequestRequestTypeDef",
     "GetDecoderManifestRequestRequestTypeDef",
-    "GetDecoderManifestResponseTypeDef",
     "GetFleetRequestRequestTypeDef",
-    "GetFleetResponseTypeDef",
     "GetModelManifestRequestRequestTypeDef",
-    "GetModelManifestResponseTypeDef",
     "IamRegistrationResponseTypeDef",
     "TimestreamRegistrationResponseTypeDef",
     "GetSignalCatalogRequestRequestTypeDef",
     "NodeCountsTypeDef",
     "GetVehicleRequestRequestTypeDef",
-    "GetVehicleResponseTypeDef",
-    "GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetVehicleStatusRequestRequestTypeDef",
     "VehicleStatusTypeDef",
     "IamResourcesTypeDef",
-    "ImportDecoderManifestResponseTypeDef",
-    "ImportSignalCatalogResponseTypeDef",
-    "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
-    "ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
     "ListDecoderManifestNetworkInterfacesRequestRequestTypeDef",
-    "ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
     "ListDecoderManifestSignalsRequestRequestTypeDef",
-    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
     "ListDecoderManifestsRequestRequestTypeDef",
-    "ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
     "ListFleetsForVehicleRequestRequestTypeDef",
-    "ListFleetsForVehicleResponseTypeDef",
-    "ListFleetsRequestListFleetsPaginateTypeDef",
     "ListFleetsRequestRequestTypeDef",
-    "ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
     "ListModelManifestNodesRequestRequestTypeDef",
-    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
     "ListModelManifestsRequestRequestTypeDef",
     "ModelManifestSummaryTypeDef",
-    "ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
     "ListSignalCatalogNodesRequestRequestTypeDef",
-    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
     "ListSignalCatalogsRequestRequestTypeDef",
     "SignalCatalogSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
     "ListVehiclesInFleetRequestRequestTypeDef",
-    "ListVehiclesInFleetResponseTypeDef",
-    "ListVehiclesRequestListVehiclesPaginateTypeDef",
     "ListVehiclesRequestRequestTypeDef",
     "VehicleSummaryTypeDef",
     "ObdInterfaceTypeDef",
+    "SensorOutputTypeDef",
     "SensorTypeDef",
     "ObdSignalTypeDef",
-    "PaginatorConfigTypeDef",
     "TimestreamResourcesTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
+    "UpdateFleetRequestRequestTypeDef",
+    "UpdateModelManifestRequestRequestTypeDef",
+    "UpdateVehicleRequestRequestTypeDef",
+    "BatchCreateVehicleResponseTypeDef",
+    "CreateCampaignResponseTypeDef",
+    "CreateDecoderManifestResponseTypeDef",
+    "CreateFleetResponseTypeDef",
+    "CreateModelManifestResponseTypeDef",
+    "CreateSignalCatalogResponseTypeDef",
+    "CreateVehicleResponseTypeDef",
+    "DeleteCampaignResponseTypeDef",
+    "DeleteDecoderManifestResponseTypeDef",
+    "DeleteFleetResponseTypeDef",
+    "DeleteModelManifestResponseTypeDef",
+    "DeleteSignalCatalogResponseTypeDef",
+    "DeleteVehicleResponseTypeDef",
+    "GetDecoderManifestResponseTypeDef",
+    "GetFleetResponseTypeDef",
+    "GetModelManifestResponseTypeDef",
+    "GetVehicleResponseTypeDef",
+    "ImportDecoderManifestResponseTypeDef",
+    "ImportSignalCatalogResponseTypeDef",
+    "ListFleetsForVehicleResponseTypeDef",
+    "ListVehiclesInFleetResponseTypeDef",
     "UpdateCampaignResponseTypeDef",
     "UpdateDecoderManifestResponseTypeDef",
-    "UpdateFleetRequestRequestTypeDef",
     "UpdateFleetResponseTypeDef",
-    "UpdateModelManifestRequestRequestTypeDef",
     "UpdateModelManifestResponseTypeDef",
     "UpdateSignalCatalogResponseTypeDef",
-    "UpdateVehicleRequestRequestTypeDef",
     "UpdateVehicleResponseTypeDef",
-    "BatchCreateVehicleResponseTypeDef",
     "BatchUpdateVehicleRequestRequestTypeDef",
     "BatchUpdateVehicleResponseTypeDef",
+    "CanDbcDefinitionTypeDef",
     "ListCampaignsResponseTypeDef",
-    "NetworkFileDefinitionTypeDef",
     "GetLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "CollectionSchemeTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateModelManifestRequestRequestTypeDef",
     "CreateVehicleRequestItemTypeDef",
     "CreateVehicleRequestRequestTypeDef",
@@ -168,37 +159,80 @@
     "TagResourceRequestRequestTypeDef",
     "DataDestinationConfigTypeDef",
     "ListDecoderManifestsResponseTypeDef",
     "ListFleetsResponseTypeDef",
     "ImportSignalCatalogRequestRequestTypeDef",
     "GetRegisterAccountStatusResponseTypeDef",
     "GetSignalCatalogResponseTypeDef",
+    "GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    "ListCampaignsRequestListCampaignsPaginateTypeDef",
+    "ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
+    "ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
+    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
+    "ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
+    "ListFleetsRequestListFleetsPaginateTypeDef",
+    "ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
+    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
+    "ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
+    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
+    "ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
+    "ListVehiclesRequestListVehiclesPaginateTypeDef",
     "GetVehicleStatusResponseTypeDef",
     "ListModelManifestsResponseTypeDef",
     "ListSignalCatalogsResponseTypeDef",
     "ListVehiclesResponseTypeDef",
     "NetworkInterfaceTypeDef",
+    "NodeOutputTypeDef",
     "NodeTypeDef",
     "SignalDecoderTypeDef",
     "RegisterAccountRequestRequestTypeDef",
     "RegisterAccountResponseTypeDef",
-    "ImportDecoderManifestRequestRequestTypeDef",
+    "NetworkFileDefinitionTypeDef",
     "BatchCreateVehicleRequestRequestTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "GetCampaignResponseTypeDef",
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
-    "CreateSignalCatalogRequestRequestTypeDef",
     "ListModelManifestNodesResponseTypeDef",
     "ListSignalCatalogNodesResponseTypeDef",
-    "UpdateSignalCatalogRequestRequestTypeDef",
+    "NodeUnionTypeDef",
     "CreateDecoderManifestRequestRequestTypeDef",
     "ListDecoderManifestSignalsResponseTypeDef",
     "UpdateDecoderManifestRequestRequestTypeDef",
+    "ImportDecoderManifestRequestRequestTypeDef",
+    "CreateSignalCatalogRequestRequestTypeDef",
+    "UpdateSignalCatalogRequestRequestTypeDef",
 )
 
+_RequiredActuatorOutputTypeDef = TypedDict(
+    "_RequiredActuatorOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "dataType": NodeDataTypeType,
+    },
+)
+_OptionalActuatorOutputTypeDef = TypedDict(
+    "_OptionalActuatorOutputTypeDef",
+    {
+        "description": str,
+        "unit": str,
+        "allowedValues": List[str],
+        "min": float,
+        "max": float,
+        "assignedValue": str,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+
+class ActuatorOutputTypeDef(_RequiredActuatorOutputTypeDef, _OptionalActuatorOutputTypeDef):
+    pass
+
+
 _RequiredActuatorTypeDef = TypedDict(
     "_RequiredActuatorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -226,14 +260,42 @@
     "AssociateVehicleFleetRequestRequestTypeDef",
     {
         "vehicleName": str,
         "fleetId": str,
     },
 )
 
+_RequiredAttributeOutputTypeDef = TypedDict(
+    "_RequiredAttributeOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "dataType": NodeDataTypeType,
+    },
+)
+_OptionalAttributeOutputTypeDef = TypedDict(
+    "_OptionalAttributeOutputTypeDef",
+    {
+        "description": str,
+        "unit": str,
+        "allowedValues": List[str],
+        "min": float,
+        "max": float,
+        "assignedValue": str,
+        "defaultValue": str,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+
+class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
+    pass
+
+
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -274,14 +336,25 @@
         "vehicleName": str,
         "arn": str,
         "thingArn": str,
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
 _RequiredUpdateVehicleRequestItemTypeDef = TypedDict(
     "_RequiredUpdateVehicleRequestItemTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalUpdateVehicleRequestItemTypeDef = TypedDict(
@@ -317,14 +390,15 @@
     {
         "vehicleName": str,
         "arn": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredBranchTypeDef = TypedDict(
     "_RequiredBranchTypeDef",
     {
         "fullyQualifiedName": str,
     },
 )
 _OptionalBranchTypeDef = TypedDict(
@@ -363,34 +437,14 @@
 )
 
 
 class CampaignSummaryTypeDef(_RequiredCampaignSummaryTypeDef, _OptionalCampaignSummaryTypeDef):
     pass
 
 
-_RequiredCanDbcDefinitionTypeDef = TypedDict(
-    "_RequiredCanDbcDefinitionTypeDef",
-    {
-        "networkInterface": str,
-        "canDbcFiles": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-    },
-)
-_OptionalCanDbcDefinitionTypeDef = TypedDict(
-    "_OptionalCanDbcDefinitionTypeDef",
-    {
-        "signalsMap": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CanDbcDefinitionTypeDef(_RequiredCanDbcDefinitionTypeDef, _OptionalCanDbcDefinitionTypeDef):
-    pass
-
-
 _RequiredCanInterfaceTypeDef = TypedDict(
     "_RequiredCanInterfaceTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCanInterfaceTypeDef = TypedDict(
@@ -509,69 +563,15 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDecoderManifestResponseTypeDef = TypedDict(
-    "CreateDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateModelManifestResponseTypeDef = TypedDict(
-    "CreateModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSignalCatalogResponseTypeDef = TypedDict(
-    "CreateSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVehicleResponseTypeDef = TypedDict(
-    "CreateVehicleResponseTypeDef",
-    {
-        "vehicleName": str,
-        "arn": str,
-        "thingArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "bucketArn": str,
     },
 )
 _OptionalS3ConfigTypeDef = TypedDict(
@@ -626,103 +626,49 @@
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteCampaignResponseTypeDef = TypedDict(
-    "DeleteCampaignResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDecoderManifestRequestRequestTypeDef = TypedDict(
     "DeleteDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteDecoderManifestResponseTypeDef = TypedDict(
-    "DeleteDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFleetRequestRequestTypeDef = TypedDict(
     "DeleteFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 
-DeleteFleetResponseTypeDef = TypedDict(
-    "DeleteFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteModelManifestRequestRequestTypeDef = TypedDict(
     "DeleteModelManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteModelManifestResponseTypeDef = TypedDict(
-    "DeleteModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSignalCatalogRequestRequestTypeDef = TypedDict(
     "DeleteSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteSignalCatalogResponseTypeDef = TypedDict(
-    "DeleteSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVehicleRequestRequestTypeDef = TypedDict(
     "DeleteVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 
-DeleteVehicleResponseTypeDef = TypedDict(
-    "DeleteVehicleResponseTypeDef",
-    {
-        "vehicleName": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateVehicleFleetRequestRequestTypeDef = TypedDict(
     "DisassociateVehicleFleetRequestRequestTypeDef",
     {
         "vehicleName": str,
         "fleetId": str,
     },
 )
@@ -768,69 +714,28 @@
 GetDecoderManifestRequestRequestTypeDef = TypedDict(
     "GetDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetDecoderManifestResponseTypeDef = TypedDict(
-    "GetDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "modelManifestArn": str,
-        "status": ManifestStatusType,
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFleetRequestRequestTypeDef = TypedDict(
     "GetFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 
-GetFleetResponseTypeDef = TypedDict(
-    "GetFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "description": str,
-        "signalCatalogArn": str,
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetModelManifestRequestRequestTypeDef = TypedDict(
     "GetModelManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetModelManifestResponseTypeDef = TypedDict(
-    "GetModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "signalCatalogArn": str,
-        "status": ManifestStatusType,
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredIamRegistrationResponseTypeDef = TypedDict(
     "_RequiredIamRegistrationResponseTypeDef",
     {
         "roleArn": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -896,50 +801,24 @@
 GetVehicleRequestRequestTypeDef = TypedDict(
     "GetVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 
-GetVehicleResponseTypeDef = TypedDict(
-    "GetVehicleResponseTypeDef",
-    {
-        "vehicleName": str,
-        "arn": str,
-        "modelManifestArn": str,
-        "decoderManifestArn": str,
-        "attributes": Dict[str, str],
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
-    "_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
-    {
-        "vehicleName": str,
-    },
-)
-_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
-    "_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
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
-class GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef(
-    _RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
-    _OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetVehicleStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetVehicleStatusRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalGetVehicleStatusRequestRequestTypeDef = TypedDict(
@@ -971,73 +850,24 @@
 IamResourcesTypeDef = TypedDict(
     "IamResourcesTypeDef",
     {
         "roleArn": str,
     },
 )
 
-ImportDecoderManifestResponseTypeDef = TypedDict(
-    "ImportDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportSignalCatalogResponseTypeDef = TypedDict(
-    "ImportSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
-    "ListCampaignsRequestListCampaignsPaginateTypeDef",
-    {
-        "status": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCampaignsRequestRequestTypeDef = TypedDict(
     "ListCampaignsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": str,
     },
     total=False,
 )
 
-_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
-    "_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
-    "_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef(
-    _RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
-    _OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDecoderManifestNetworkInterfacesRequestRequestTypeDef = TypedDict(
     "_RequiredListDecoderManifestNetworkInterfacesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListDecoderManifestNetworkInterfacesRequestRequestTypeDef = TypedDict(
@@ -1053,36 +883,14 @@
 class ListDecoderManifestNetworkInterfacesRequestRequestTypeDef(
     _RequiredListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
     _OptionalListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
-    "_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
-    "_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef(
-    _RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
-    _OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDecoderManifestSignalsRequestRequestTypeDef = TypedDict(
     "_RequiredListDecoderManifestSignalsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListDecoderManifestSignalsRequestRequestTypeDef = TypedDict(
@@ -1098,55 +906,24 @@
 class ListDecoderManifestSignalsRequestRequestTypeDef(
     _RequiredListDecoderManifestSignalsRequestRequestTypeDef,
     _OptionalListDecoderManifestSignalsRequestRequestTypeDef,
 ):
     pass
 
 
-ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef = TypedDict(
-    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
-    {
-        "modelManifestArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDecoderManifestsRequestRequestTypeDef = TypedDict(
     "ListDecoderManifestsRequestRequestTypeDef",
     {
         "modelManifestArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
-    "_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
-    {
-        "vehicleName": str,
-    },
-)
-_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
-    "_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef(
-    _RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
-    _OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFleetsForVehicleRequestRequestTypeDef = TypedDict(
     "_RequiredListFleetsForVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalListFleetsForVehicleRequestRequestTypeDef = TypedDict(
@@ -1162,62 +939,23 @@
 class ListFleetsForVehicleRequestRequestTypeDef(
     _RequiredListFleetsForVehicleRequestRequestTypeDef,
     _OptionalListFleetsForVehicleRequestRequestTypeDef,
 ):
     pass
 
 
-ListFleetsForVehicleResponseTypeDef = TypedDict(
-    "ListFleetsForVehicleResponseTypeDef",
-    {
-        "fleets": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
-    "ListFleetsRequestListFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFleetsRequestRequestTypeDef = TypedDict(
     "ListFleetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
-    "_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
-    "_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef(
-    _RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
-    _OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListModelManifestNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListModelManifestNodesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListModelManifestNodesRequestRequestTypeDef = TypedDict(
@@ -1233,23 +971,14 @@
 class ListModelManifestNodesRequestRequestTypeDef(
     _RequiredListModelManifestNodesRequestRequestTypeDef,
     _OptionalListModelManifestNodesRequestRequestTypeDef,
 ):
     pass
 
 
-ListModelManifestsRequestListModelManifestsPaginateTypeDef = TypedDict(
-    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
-    {
-        "signalCatalogArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListModelManifestsRequestRequestTypeDef = TypedDict(
     "ListModelManifestsRequestRequestTypeDef",
     {
         "signalCatalogArn": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1278,36 +1007,14 @@
 
 class ModelManifestSummaryTypeDef(
     _RequiredModelManifestSummaryTypeDef, _OptionalModelManifestSummaryTypeDef
 ):
     pass
 
 
-_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
-    "_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
-    "_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef(
-    _RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
-    _OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSignalCatalogNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListSignalCatalogNodesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListSignalCatalogNodesRequestRequestTypeDef = TypedDict(
@@ -1323,22 +1030,14 @@
 class ListSignalCatalogNodesRequestRequestTypeDef(
     _RequiredListSignalCatalogNodesRequestRequestTypeDef,
     _OptionalListSignalCatalogNodesRequestRequestTypeDef,
 ):
     pass
 
 
-ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef = TypedDict(
-    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSignalCatalogsRequestRequestTypeDef = TypedDict(
     "ListSignalCatalogsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1358,36 +1057,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
-    "_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
-    {
-        "fleetId": str,
-    },
-)
-_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
-    "_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef(
-    _RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
-    _OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVehiclesInFleetRequestRequestTypeDef = TypedDict(
     "_RequiredListVehiclesInFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 _OptionalListVehiclesInFleetRequestRequestTypeDef = TypedDict(
@@ -1403,32 +1080,14 @@
 class ListVehiclesInFleetRequestRequestTypeDef(
     _RequiredListVehiclesInFleetRequestRequestTypeDef,
     _OptionalListVehiclesInFleetRequestRequestTypeDef,
 ):
     pass
 
 
-ListVehiclesInFleetResponseTypeDef = TypedDict(
-    "ListVehiclesInFleetResponseTypeDef",
-    {
-        "vehicles": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListVehiclesRequestListVehiclesPaginateTypeDef = TypedDict(
-    "ListVehiclesRequestListVehiclesPaginateTypeDef",
-    {
-        "modelManifestArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVehiclesRequestRequestTypeDef = TypedDict(
     "ListVehiclesRequestRequestTypeDef",
     {
         "modelManifestArn": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1467,14 +1126,40 @@
 )
 
 
 class ObdInterfaceTypeDef(_RequiredObdInterfaceTypeDef, _OptionalObdInterfaceTypeDef):
     pass
 
 
+_RequiredSensorOutputTypeDef = TypedDict(
+    "_RequiredSensorOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "dataType": NodeDataTypeType,
+    },
+)
+_OptionalSensorOutputTypeDef = TypedDict(
+    "_OptionalSensorOutputTypeDef",
+    {
+        "description": str,
+        "unit": str,
+        "allowedValues": List[str],
+        "min": float,
+        "max": float,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+
+class SensorOutputTypeDef(_RequiredSensorOutputTypeDef, _OptionalSensorOutputTypeDef):
+    pass
+
+
 _RequiredSensorTypeDef = TypedDict(
     "_RequiredSensorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -1519,43 +1204,22 @@
 )
 
 
 class ObdSignalTypeDef(_RequiredObdSignalTypeDef, _OptionalObdSignalTypeDef):
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
 TimestreamResourcesTypeDef = TypedDict(
     "TimestreamResourcesTypeDef",
     {
         "timestreamDatabaseName": str,
         "timestreamTableName": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1579,33 +1243,14 @@
 
 class UpdateCampaignRequestRequestTypeDef(
     _RequiredUpdateCampaignRequestRequestTypeDef, _OptionalUpdateCampaignRequestRequestTypeDef
 ):
     pass
 
 
-UpdateCampaignResponseTypeDef = TypedDict(
-    "UpdateCampaignResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "status": CampaignStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDecoderManifestResponseTypeDef = TypedDict(
-    "UpdateDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 _OptionalUpdateFleetRequestRequestTypeDef = TypedDict(
@@ -1619,23 +1264,14 @@
 
 class UpdateFleetRequestRequestTypeDef(
     _RequiredUpdateFleetRequestRequestTypeDef, _OptionalUpdateFleetRequestRequestTypeDef
 ):
     pass
 
 
-UpdateFleetResponseTypeDef = TypedDict(
-    "UpdateFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateModelManifestRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateModelManifestRequestRequestTypeDef = TypedDict(
@@ -1653,32 +1289,14 @@
 class UpdateModelManifestRequestRequestTypeDef(
     _RequiredUpdateModelManifestRequestRequestTypeDef,
     _OptionalUpdateModelManifestRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateModelManifestResponseTypeDef = TypedDict(
-    "UpdateModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSignalCatalogResponseTypeDef = TypedDict(
-    "UpdateSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVehicleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalUpdateVehicleRequestRequestTypeDef = TypedDict(
@@ -1695,29 +1313,275 @@
 
 class UpdateVehicleRequestRequestTypeDef(
     _RequiredUpdateVehicleRequestRequestTypeDef, _OptionalUpdateVehicleRequestRequestTypeDef
 ):
     pass
 
 
-UpdateVehicleResponseTypeDef = TypedDict(
-    "UpdateVehicleResponseTypeDef",
+BatchCreateVehicleResponseTypeDef = TypedDict(
+    "BatchCreateVehicleResponseTypeDef",
+    {
+        "vehicles": List[CreateVehicleResponseItemTypeDef],
+        "errors": List[CreateVehicleErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDecoderManifestResponseTypeDef = TypedDict(
+    "CreateDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelManifestResponseTypeDef = TypedDict(
+    "CreateModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSignalCatalogResponseTypeDef = TypedDict(
+    "CreateSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVehicleResponseTypeDef = TypedDict(
+    "CreateVehicleResponseTypeDef",
     {
         "vehicleName": str,
         "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "thingArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchCreateVehicleResponseTypeDef = TypedDict(
-    "BatchCreateVehicleResponseTypeDef",
+DeleteCampaignResponseTypeDef = TypedDict(
+    "DeleteCampaignResponseTypeDef",
     {
-        "vehicles": List[CreateVehicleResponseItemTypeDef],
-        "errors": List[CreateVehicleErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDecoderManifestResponseTypeDef = TypedDict(
+    "DeleteDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFleetResponseTypeDef = TypedDict(
+    "DeleteFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteModelManifestResponseTypeDef = TypedDict(
+    "DeleteModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSignalCatalogResponseTypeDef = TypedDict(
+    "DeleteSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVehicleResponseTypeDef = TypedDict(
+    "DeleteVehicleResponseTypeDef",
+    {
+        "vehicleName": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDecoderManifestResponseTypeDef = TypedDict(
+    "GetDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "modelManifestArn": str,
+        "status": ManifestStatusType,
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFleetResponseTypeDef = TypedDict(
+    "GetFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "description": str,
+        "signalCatalogArn": str,
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelManifestResponseTypeDef = TypedDict(
+    "GetModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "signalCatalogArn": str,
+        "status": ManifestStatusType,
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVehicleResponseTypeDef = TypedDict(
+    "GetVehicleResponseTypeDef",
+    {
+        "vehicleName": str,
+        "arn": str,
+        "modelManifestArn": str,
+        "decoderManifestArn": str,
+        "attributes": Dict[str, str],
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportDecoderManifestResponseTypeDef = TypedDict(
+    "ImportDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportSignalCatalogResponseTypeDef = TypedDict(
+    "ImportSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFleetsForVehicleResponseTypeDef = TypedDict(
+    "ListFleetsForVehicleResponseTypeDef",
+    {
+        "fleets": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVehiclesInFleetResponseTypeDef = TypedDict(
+    "ListVehiclesInFleetResponseTypeDef",
+    {
+        "vehicles": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCampaignResponseTypeDef = TypedDict(
+    "UpdateCampaignResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "status": CampaignStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDecoderManifestResponseTypeDef = TypedDict(
+    "UpdateDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFleetResponseTypeDef = TypedDict(
+    "UpdateFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateModelManifestResponseTypeDef = TypedDict(
+    "UpdateModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSignalCatalogResponseTypeDef = TypedDict(
+    "UpdateSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVehicleResponseTypeDef = TypedDict(
+    "UpdateVehicleResponseTypeDef",
+    {
+        "vehicleName": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateVehicleRequestRequestTypeDef = TypedDict(
     "BatchUpdateVehicleRequestRequestTypeDef",
     {
         "vehicles": Sequence[UpdateVehicleRequestItemTypeDef],
@@ -1725,40 +1589,52 @@
 )
 
 BatchUpdateVehicleResponseTypeDef = TypedDict(
     "BatchUpdateVehicleResponseTypeDef",
     {
         "vehicles": List[UpdateVehicleResponseItemTypeDef],
         "errors": List[UpdateVehicleErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListCampaignsResponseTypeDef = TypedDict(
-    "ListCampaignsResponseTypeDef",
+_RequiredCanDbcDefinitionTypeDef = TypedDict(
+    "_RequiredCanDbcDefinitionTypeDef",
     {
-        "campaignSummaries": List[CampaignSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "networkInterface": str,
+        "canDbcFiles": Sequence[BlobTypeDef],
     },
 )
-
-NetworkFileDefinitionTypeDef = TypedDict(
-    "NetworkFileDefinitionTypeDef",
+_OptionalCanDbcDefinitionTypeDef = TypedDict(
+    "_OptionalCanDbcDefinitionTypeDef",
     {
-        "canDbc": CanDbcDefinitionTypeDef,
+        "signalsMap": Mapping[str, str],
     },
     total=False,
 )
 
+
+class CanDbcDefinitionTypeDef(_RequiredCanDbcDefinitionTypeDef, _OptionalCanDbcDefinitionTypeDef):
+    pass
+
+
+ListCampaignsResponseTypeDef = TypedDict(
+    "ListCampaignsResponseTypeDef",
+    {
+        "campaignSummaries": List[CampaignSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetLoggingOptionsResponseTypeDef = TypedDict(
     "GetLoggingOptionsResponseTypeDef",
     {
         "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
@@ -1872,15 +1748,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1898,24 +1774,24 @@
 )
 
 ListDecoderManifestsResponseTypeDef = TypedDict(
     "ListDecoderManifestsResponseTypeDef",
     {
         "summaries": List[DecoderManifestSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFleetsResponseTypeDef = TypedDict(
     "ListFleetsResponseTypeDef",
     {
         "fleetSummaries": List[FleetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportSignalCatalogRequestRequestTypeDef = TypedDict(
     "_RequiredImportSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
@@ -1944,64 +1820,270 @@
     {
         "customerAccountId": str,
         "accountStatus": RegistrationStatusType,
         "timestreamRegistrationResponse": TimestreamRegistrationResponseTypeDef,
         "iamRegistrationResponse": IamRegistrationResponseTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSignalCatalogResponseTypeDef = TypedDict(
     "GetSignalCatalogResponseTypeDef",
     {
         "name": str,
         "arn": str,
         "description": str,
         "nodeCounts": NodeCountsTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
+    "_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    {
+        "vehicleName": str,
+    },
+)
+_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
+    "_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef(
+    _RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    _OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+):
+    pass
+
+
+ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
+    "ListCampaignsRequestListCampaignsPaginateTypeDef",
+    {
+        "status": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
+    "_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
+    "_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef(
+    _RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+    _OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
+    "_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
+    "_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef(
+    _RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+    _OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+):
+    pass
+
+
+ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef = TypedDict(
+    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
+    {
+        "modelManifestArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
+    "_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
+    {
+        "vehicleName": str,
+    },
+)
+_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
+    "_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef(
+    _RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+    _OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+):
+    pass
+
+
+ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
+    "ListFleetsRequestListFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
+    "_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
+    "_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef(
+    _RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+    _OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+):
+    pass
+
+
+ListModelManifestsRequestListModelManifestsPaginateTypeDef = TypedDict(
+    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
+    {
+        "signalCatalogArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
+    "_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
+    "_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef(
+    _RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+    _OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+):
+    pass
+
+
+ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef = TypedDict(
+    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
+    "_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
+    {
+        "fleetId": str,
+    },
+)
+_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
+    "_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef(
+    _RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+    _OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+):
+    pass
+
+
+ListVehiclesRequestListVehiclesPaginateTypeDef = TypedDict(
+    "ListVehiclesRequestListVehiclesPaginateTypeDef",
+    {
+        "modelManifestArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetVehicleStatusResponseTypeDef = TypedDict(
     "GetVehicleStatusResponseTypeDef",
     {
         "campaigns": List[VehicleStatusTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListModelManifestsResponseTypeDef = TypedDict(
     "ListModelManifestsResponseTypeDef",
     {
         "summaries": List[ModelManifestSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalCatalogsResponseTypeDef = TypedDict(
     "ListSignalCatalogsResponseTypeDef",
     {
         "summaries": List[SignalCatalogSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVehiclesResponseTypeDef = TypedDict(
     "ListVehiclesResponseTypeDef",
     {
         "vehicleSummaries": List[VehicleSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNetworkInterfaceTypeDef = TypedDict(
     "_RequiredNetworkInterfaceTypeDef",
     {
         "interfaceId": str,
@@ -2018,14 +2100,25 @@
 )
 
 
 class NetworkInterfaceTypeDef(_RequiredNetworkInterfaceTypeDef, _OptionalNetworkInterfaceTypeDef):
     pass
 
 
+NodeOutputTypeDef = TypedDict(
+    "NodeOutputTypeDef",
+    {
+        "branch": BranchTypeDef,
+        "sensor": SensorOutputTypeDef,
+        "actuator": ActuatorOutputTypeDef,
+        "attribute": AttributeOutputTypeDef,
+    },
+    total=False,
+)
+
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "branch": BranchTypeDef,
         "sensor": SensorTypeDef,
         "actuator": ActuatorTypeDef,
         "attribute": AttributeTypeDef,
@@ -2068,24 +2161,24 @@
     "RegisterAccountResponseTypeDef",
     {
         "registerAccountStatus": RegistrationStatusType,
         "timestreamResources": TimestreamResourcesTypeDef,
         "iamResources": IamResourcesTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImportDecoderManifestRequestRequestTypeDef = TypedDict(
-    "ImportDecoderManifestRequestRequestTypeDef",
+NetworkFileDefinitionTypeDef = TypedDict(
+    "NetworkFileDefinitionTypeDef",
     {
-        "name": str,
-        "networkFileDefinitions": Sequence[NetworkFileDefinitionTypeDef],
+        "canDbc": CanDbcDefinitionTypeDef,
     },
+    total=False,
 )
 
 BatchCreateVehicleRequestRequestTypeDef = TypedDict(
     "BatchCreateVehicleRequestRequestTypeDef",
     {
         "vehicles": Sequence[CreateVehicleRequestItemTypeDef],
     },
@@ -2100,16 +2193,16 @@
         "collectionScheme": CollectionSchemeTypeDef,
     },
 )
 _OptionalCreateCampaignRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCampaignRequestRequestTypeDef",
     {
         "description": str,
-        "startTime": Union[datetime, str],
-        "expiryTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "expiryTime": TimestampTypeDef,
         "postTriggerCollectionDuration": int,
         "diagnosticsMode": DiagnosticsModeType,
         "spoolingMode": SpoolingModeType,
         "compression": CompressionType,
         "priority": int,
         "signalsToCollect": Sequence[SignalInformationTypeDef],
         "dataExtraDimensions": Sequence[str],
@@ -2144,94 +2237,46 @@
         "priority": int,
         "signalsToCollect": List[SignalInformationTypeDef],
         "collectionScheme": CollectionSchemeTypeDef,
         "dataExtraDimensions": List[str],
         "creationTime": datetime,
         "lastModificationTime": datetime,
         "dataDestinationConfigs": List[DataDestinationConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDecoderManifestNetworkInterfacesResponseTypeDef = TypedDict(
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
     {
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSignalCatalogRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSignalCatalogRequestRequestTypeDef",
-    {
-        "description": str,
-        "nodes": Sequence[NodeTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateSignalCatalogRequestRequestTypeDef(
-    _RequiredCreateSignalCatalogRequestRequestTypeDef,
-    _OptionalCreateSignalCatalogRequestRequestTypeDef,
-):
-    pass
-
-
 ListModelManifestNodesResponseTypeDef = TypedDict(
     "ListModelManifestNodesResponseTypeDef",
     {
-        "nodes": List[NodeTypeDef],
+        "nodes": List[NodeOutputTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalCatalogNodesResponseTypeDef = TypedDict(
     "ListSignalCatalogNodesResponseTypeDef",
     {
-        "nodes": List[NodeTypeDef],
+        "nodes": List[NodeOutputTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
-    {
-        "description": str,
-        "nodesToAdd": Sequence[NodeTypeDef],
-        "nodesToUpdate": Sequence[NodeTypeDef],
-        "nodesToRemove": Sequence[str],
-    },
-    total=False,
-)
-
-
-class UpdateSignalCatalogRequestRequestTypeDef(
-    _RequiredUpdateSignalCatalogRequestRequestTypeDef,
-    _OptionalUpdateSignalCatalogRequestRequestTypeDef,
-):
-    pass
-
-
+NodeUnionTypeDef = Union[NodeTypeDef, NodeOutputTypeDef]
 _RequiredCreateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
         "modelManifestArn": str,
     },
 )
@@ -2255,15 +2300,15 @@
 
 
 ListDecoderManifestSignalsResponseTypeDef = TypedDict(
     "ListDecoderManifestSignalsResponseTypeDef",
     {
         "signalDecoders": List[SignalDecoderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
@@ -2286,7 +2331,64 @@
 
 
 class UpdateDecoderManifestRequestRequestTypeDef(
     _RequiredUpdateDecoderManifestRequestRequestTypeDef,
     _OptionalUpdateDecoderManifestRequestRequestTypeDef,
 ):
     pass
+
+
+ImportDecoderManifestRequestRequestTypeDef = TypedDict(
+    "ImportDecoderManifestRequestRequestTypeDef",
+    {
+        "name": str,
+        "networkFileDefinitions": Sequence[NetworkFileDefinitionTypeDef],
+    },
+)
+
+_RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSignalCatalogRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSignalCatalogRequestRequestTypeDef",
+    {
+        "description": str,
+        "nodes": Sequence[NodeUnionTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateSignalCatalogRequestRequestTypeDef(
+    _RequiredCreateSignalCatalogRequestRequestTypeDef,
+    _OptionalCreateSignalCatalogRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
+    {
+        "description": str,
+        "nodesToAdd": Sequence[NodeUnionTypeDef],
+        "nodesToUpdate": Sequence[NodeUnionTypeDef],
+        "nodesToRemove": Sequence[str],
+    },
+    total=False,
+)
+
+
+class UpdateSignalCatalogRequestRequestTypeDef(
+    _RequiredUpdateSignalCatalogRequestRequestTypeDef,
+    _OptionalUpdateSignalCatalogRequestRequestTypeDef,
+):
+    pass
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise/type_defs.pyi` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotfleetwise service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_iotfleetwise.type_defs import ActuatorTypeDef
+    from types_aiobotocore_iotfleetwise.type_defs import ActuatorOutputTypeDef
 
-    data: ActuatorTypeDef = {...}
+    data: ActuatorOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -39,127 +39,118 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ActuatorOutputTypeDef",
     "ActuatorTypeDef",
     "AssociateVehicleFleetRequestRequestTypeDef",
+    "AttributeOutputTypeDef",
     "AttributeTypeDef",
     "CreateVehicleErrorTypeDef",
     "CreateVehicleResponseItemTypeDef",
+    "ResponseMetadataTypeDef",
     "UpdateVehicleRequestItemTypeDef",
     "UpdateVehicleErrorTypeDef",
     "UpdateVehicleResponseItemTypeDef",
+    "BlobTypeDef",
     "BranchTypeDef",
     "CampaignSummaryTypeDef",
-    "CanDbcDefinitionTypeDef",
     "CanInterfaceTypeDef",
     "CanSignalTypeDef",
     "CloudWatchLogDeliveryOptionsTypeDef",
     "ConditionBasedCollectionSchemeTypeDef",
     "TimeBasedCollectionSchemeTypeDef",
     "SignalInformationTypeDef",
     "TagTypeDef",
-    "CreateCampaignResponseTypeDef",
-    "CreateDecoderManifestResponseTypeDef",
-    "CreateFleetResponseTypeDef",
-    "CreateModelManifestResponseTypeDef",
-    "CreateSignalCatalogResponseTypeDef",
-    "CreateVehicleResponseTypeDef",
+    "TimestampTypeDef",
     "S3ConfigTypeDef",
     "TimestreamConfigTypeDef",
     "DecoderManifestSummaryTypeDef",
     "DeleteCampaignRequestRequestTypeDef",
-    "DeleteCampaignResponseTypeDef",
     "DeleteDecoderManifestRequestRequestTypeDef",
-    "DeleteDecoderManifestResponseTypeDef",
     "DeleteFleetRequestRequestTypeDef",
-    "DeleteFleetResponseTypeDef",
     "DeleteModelManifestRequestRequestTypeDef",
-    "DeleteModelManifestResponseTypeDef",
     "DeleteSignalCatalogRequestRequestTypeDef",
-    "DeleteSignalCatalogResponseTypeDef",
     "DeleteVehicleRequestRequestTypeDef",
-    "DeleteVehicleResponseTypeDef",
     "DisassociateVehicleFleetRequestRequestTypeDef",
     "FleetSummaryTypeDef",
     "FormattedVssTypeDef",
     "GetCampaignRequestRequestTypeDef",
     "GetDecoderManifestRequestRequestTypeDef",
-    "GetDecoderManifestResponseTypeDef",
     "GetFleetRequestRequestTypeDef",
-    "GetFleetResponseTypeDef",
     "GetModelManifestRequestRequestTypeDef",
-    "GetModelManifestResponseTypeDef",
     "IamRegistrationResponseTypeDef",
     "TimestreamRegistrationResponseTypeDef",
     "GetSignalCatalogRequestRequestTypeDef",
     "NodeCountsTypeDef",
     "GetVehicleRequestRequestTypeDef",
-    "GetVehicleResponseTypeDef",
-    "GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetVehicleStatusRequestRequestTypeDef",
     "VehicleStatusTypeDef",
     "IamResourcesTypeDef",
-    "ImportDecoderManifestResponseTypeDef",
-    "ImportSignalCatalogResponseTypeDef",
-    "ListCampaignsRequestListCampaignsPaginateTypeDef",
     "ListCampaignsRequestRequestTypeDef",
-    "ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
     "ListDecoderManifestNetworkInterfacesRequestRequestTypeDef",
-    "ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
     "ListDecoderManifestSignalsRequestRequestTypeDef",
-    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
     "ListDecoderManifestsRequestRequestTypeDef",
-    "ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
     "ListFleetsForVehicleRequestRequestTypeDef",
-    "ListFleetsForVehicleResponseTypeDef",
-    "ListFleetsRequestListFleetsPaginateTypeDef",
     "ListFleetsRequestRequestTypeDef",
-    "ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
     "ListModelManifestNodesRequestRequestTypeDef",
-    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
     "ListModelManifestsRequestRequestTypeDef",
     "ModelManifestSummaryTypeDef",
-    "ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
     "ListSignalCatalogNodesRequestRequestTypeDef",
-    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
     "ListSignalCatalogsRequestRequestTypeDef",
     "SignalCatalogSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
     "ListVehiclesInFleetRequestRequestTypeDef",
-    "ListVehiclesInFleetResponseTypeDef",
-    "ListVehiclesRequestListVehiclesPaginateTypeDef",
     "ListVehiclesRequestRequestTypeDef",
     "VehicleSummaryTypeDef",
     "ObdInterfaceTypeDef",
+    "SensorOutputTypeDef",
     "SensorTypeDef",
     "ObdSignalTypeDef",
-    "PaginatorConfigTypeDef",
     "TimestreamResourcesTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateCampaignRequestRequestTypeDef",
+    "UpdateFleetRequestRequestTypeDef",
+    "UpdateModelManifestRequestRequestTypeDef",
+    "UpdateVehicleRequestRequestTypeDef",
+    "BatchCreateVehicleResponseTypeDef",
+    "CreateCampaignResponseTypeDef",
+    "CreateDecoderManifestResponseTypeDef",
+    "CreateFleetResponseTypeDef",
+    "CreateModelManifestResponseTypeDef",
+    "CreateSignalCatalogResponseTypeDef",
+    "CreateVehicleResponseTypeDef",
+    "DeleteCampaignResponseTypeDef",
+    "DeleteDecoderManifestResponseTypeDef",
+    "DeleteFleetResponseTypeDef",
+    "DeleteModelManifestResponseTypeDef",
+    "DeleteSignalCatalogResponseTypeDef",
+    "DeleteVehicleResponseTypeDef",
+    "GetDecoderManifestResponseTypeDef",
+    "GetFleetResponseTypeDef",
+    "GetModelManifestResponseTypeDef",
+    "GetVehicleResponseTypeDef",
+    "ImportDecoderManifestResponseTypeDef",
+    "ImportSignalCatalogResponseTypeDef",
+    "ListFleetsForVehicleResponseTypeDef",
+    "ListVehiclesInFleetResponseTypeDef",
     "UpdateCampaignResponseTypeDef",
     "UpdateDecoderManifestResponseTypeDef",
-    "UpdateFleetRequestRequestTypeDef",
     "UpdateFleetResponseTypeDef",
-    "UpdateModelManifestRequestRequestTypeDef",
     "UpdateModelManifestResponseTypeDef",
     "UpdateSignalCatalogResponseTypeDef",
-    "UpdateVehicleRequestRequestTypeDef",
     "UpdateVehicleResponseTypeDef",
-    "BatchCreateVehicleResponseTypeDef",
     "BatchUpdateVehicleRequestRequestTypeDef",
     "BatchUpdateVehicleResponseTypeDef",
+    "CanDbcDefinitionTypeDef",
     "ListCampaignsResponseTypeDef",
-    "NetworkFileDefinitionTypeDef",
     "GetLoggingOptionsResponseTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "CollectionSchemeTypeDef",
     "CreateFleetRequestRequestTypeDef",
     "CreateModelManifestRequestRequestTypeDef",
     "CreateVehicleRequestItemTypeDef",
     "CreateVehicleRequestRequestTypeDef",
@@ -167,37 +158,78 @@
     "TagResourceRequestRequestTypeDef",
     "DataDestinationConfigTypeDef",
     "ListDecoderManifestsResponseTypeDef",
     "ListFleetsResponseTypeDef",
     "ImportSignalCatalogRequestRequestTypeDef",
     "GetRegisterAccountStatusResponseTypeDef",
     "GetSignalCatalogResponseTypeDef",
+    "GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    "ListCampaignsRequestListCampaignsPaginateTypeDef",
+    "ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
+    "ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
+    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
+    "ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
+    "ListFleetsRequestListFleetsPaginateTypeDef",
+    "ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
+    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
+    "ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
+    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
+    "ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
+    "ListVehiclesRequestListVehiclesPaginateTypeDef",
     "GetVehicleStatusResponseTypeDef",
     "ListModelManifestsResponseTypeDef",
     "ListSignalCatalogsResponseTypeDef",
     "ListVehiclesResponseTypeDef",
     "NetworkInterfaceTypeDef",
+    "NodeOutputTypeDef",
     "NodeTypeDef",
     "SignalDecoderTypeDef",
     "RegisterAccountRequestRequestTypeDef",
     "RegisterAccountResponseTypeDef",
-    "ImportDecoderManifestRequestRequestTypeDef",
+    "NetworkFileDefinitionTypeDef",
     "BatchCreateVehicleRequestRequestTypeDef",
     "CreateCampaignRequestRequestTypeDef",
     "GetCampaignResponseTypeDef",
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
-    "CreateSignalCatalogRequestRequestTypeDef",
     "ListModelManifestNodesResponseTypeDef",
     "ListSignalCatalogNodesResponseTypeDef",
-    "UpdateSignalCatalogRequestRequestTypeDef",
+    "NodeUnionTypeDef",
     "CreateDecoderManifestRequestRequestTypeDef",
     "ListDecoderManifestSignalsResponseTypeDef",
     "UpdateDecoderManifestRequestRequestTypeDef",
+    "ImportDecoderManifestRequestRequestTypeDef",
+    "CreateSignalCatalogRequestRequestTypeDef",
+    "UpdateSignalCatalogRequestRequestTypeDef",
+)
+
+_RequiredActuatorOutputTypeDef = TypedDict(
+    "_RequiredActuatorOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "dataType": NodeDataTypeType,
+    },
+)
+_OptionalActuatorOutputTypeDef = TypedDict(
+    "_OptionalActuatorOutputTypeDef",
+    {
+        "description": str,
+        "unit": str,
+        "allowedValues": List[str],
+        "min": float,
+        "max": float,
+        "assignedValue": str,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
 )
 
+class ActuatorOutputTypeDef(_RequiredActuatorOutputTypeDef, _OptionalActuatorOutputTypeDef):
+    pass
+
 _RequiredActuatorTypeDef = TypedDict(
     "_RequiredActuatorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -223,14 +255,40 @@
     "AssociateVehicleFleetRequestRequestTypeDef",
     {
         "vehicleName": str,
         "fleetId": str,
     },
 )
 
+_RequiredAttributeOutputTypeDef = TypedDict(
+    "_RequiredAttributeOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "dataType": NodeDataTypeType,
+    },
+)
+_OptionalAttributeOutputTypeDef = TypedDict(
+    "_OptionalAttributeOutputTypeDef",
+    {
+        "description": str,
+        "unit": str,
+        "allowedValues": List[str],
+        "min": float,
+        "max": float,
+        "assignedValue": str,
+        "defaultValue": str,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+class AttributeOutputTypeDef(_RequiredAttributeOutputTypeDef, _OptionalAttributeOutputTypeDef):
+    pass
+
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -269,14 +327,25 @@
         "vehicleName": str,
         "arn": str,
         "thingArn": str,
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
 _RequiredUpdateVehicleRequestItemTypeDef = TypedDict(
     "_RequiredUpdateVehicleRequestItemTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalUpdateVehicleRequestItemTypeDef = TypedDict(
@@ -310,14 +379,15 @@
     {
         "vehicleName": str,
         "arn": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredBranchTypeDef = TypedDict(
     "_RequiredBranchTypeDef",
     {
         "fullyQualifiedName": str,
     },
 )
 _OptionalBranchTypeDef = TypedDict(
@@ -352,32 +422,14 @@
     },
     total=False,
 )
 
 class CampaignSummaryTypeDef(_RequiredCampaignSummaryTypeDef, _OptionalCampaignSummaryTypeDef):
     pass
 
-_RequiredCanDbcDefinitionTypeDef = TypedDict(
-    "_RequiredCanDbcDefinitionTypeDef",
-    {
-        "networkInterface": str,
-        "canDbcFiles": Sequence[Union[str, bytes, IO[Any], StreamingBody]],
-    },
-)
-_OptionalCanDbcDefinitionTypeDef = TypedDict(
-    "_OptionalCanDbcDefinitionTypeDef",
-    {
-        "signalsMap": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CanDbcDefinitionTypeDef(_RequiredCanDbcDefinitionTypeDef, _OptionalCanDbcDefinitionTypeDef):
-    pass
-
 _RequiredCanInterfaceTypeDef = TypedDict(
     "_RequiredCanInterfaceTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCanInterfaceTypeDef = TypedDict(
@@ -486,69 +538,15 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateCampaignResponseTypeDef = TypedDict(
-    "CreateCampaignResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDecoderManifestResponseTypeDef = TypedDict(
-    "CreateDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateModelManifestResponseTypeDef = TypedDict(
-    "CreateModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSignalCatalogResponseTypeDef = TypedDict(
-    "CreateSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVehicleResponseTypeDef = TypedDict(
-    "CreateVehicleResponseTypeDef",
-    {
-        "vehicleName": str,
-        "arn": str,
-        "thingArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "bucketArn": str,
     },
 )
 _OptionalS3ConfigTypeDef = TypedDict(
@@ -599,103 +597,49 @@
 DeleteCampaignRequestRequestTypeDef = TypedDict(
     "DeleteCampaignRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteCampaignResponseTypeDef = TypedDict(
-    "DeleteCampaignResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDecoderManifestRequestRequestTypeDef = TypedDict(
     "DeleteDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteDecoderManifestResponseTypeDef = TypedDict(
-    "DeleteDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteFleetRequestRequestTypeDef = TypedDict(
     "DeleteFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 
-DeleteFleetResponseTypeDef = TypedDict(
-    "DeleteFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteModelManifestRequestRequestTypeDef = TypedDict(
     "DeleteModelManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteModelManifestResponseTypeDef = TypedDict(
-    "DeleteModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSignalCatalogRequestRequestTypeDef = TypedDict(
     "DeleteSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DeleteSignalCatalogResponseTypeDef = TypedDict(
-    "DeleteSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteVehicleRequestRequestTypeDef = TypedDict(
     "DeleteVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 
-DeleteVehicleResponseTypeDef = TypedDict(
-    "DeleteVehicleResponseTypeDef",
-    {
-        "vehicleName": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateVehicleFleetRequestRequestTypeDef = TypedDict(
     "DisassociateVehicleFleetRequestRequestTypeDef",
     {
         "vehicleName": str,
         "fleetId": str,
     },
 )
@@ -739,69 +683,28 @@
 GetDecoderManifestRequestRequestTypeDef = TypedDict(
     "GetDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetDecoderManifestResponseTypeDef = TypedDict(
-    "GetDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "modelManifestArn": str,
-        "status": ManifestStatusType,
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFleetRequestRequestTypeDef = TypedDict(
     "GetFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 
-GetFleetResponseTypeDef = TypedDict(
-    "GetFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "description": str,
-        "signalCatalogArn": str,
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetModelManifestRequestRequestTypeDef = TypedDict(
     "GetModelManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-GetModelManifestResponseTypeDef = TypedDict(
-    "GetModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "description": str,
-        "signalCatalogArn": str,
-        "status": ManifestStatusType,
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredIamRegistrationResponseTypeDef = TypedDict(
     "_RequiredIamRegistrationResponseTypeDef",
     {
         "roleArn": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -863,48 +766,24 @@
 GetVehicleRequestRequestTypeDef = TypedDict(
     "GetVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 
-GetVehicleResponseTypeDef = TypedDict(
-    "GetVehicleResponseTypeDef",
-    {
-        "vehicleName": str,
-        "arn": str,
-        "modelManifestArn": str,
-        "decoderManifestArn": str,
-        "attributes": Dict[str, str],
-        "creationTime": datetime,
-        "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
-    "_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
-    {
-        "vehicleName": str,
-    },
-)
-_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
-    "_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
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
 
-class GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef(
-    _RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
-    _OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
-):
-    pass
-
 _RequiredGetVehicleStatusRequestRequestTypeDef = TypedDict(
     "_RequiredGetVehicleStatusRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalGetVehicleStatusRequestRequestTypeDef = TypedDict(
@@ -934,71 +813,24 @@
 IamResourcesTypeDef = TypedDict(
     "IamResourcesTypeDef",
     {
         "roleArn": str,
     },
 )
 
-ImportDecoderManifestResponseTypeDef = TypedDict(
-    "ImportDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ImportSignalCatalogResponseTypeDef = TypedDict(
-    "ImportSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
-    "ListCampaignsRequestListCampaignsPaginateTypeDef",
-    {
-        "status": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCampaignsRequestRequestTypeDef = TypedDict(
     "ListCampaignsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": str,
     },
     total=False,
 )
 
-_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
-    "_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
-    "_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef(
-    _RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
-    _OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDecoderManifestNetworkInterfacesRequestRequestTypeDef = TypedDict(
     "_RequiredListDecoderManifestNetworkInterfacesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListDecoderManifestNetworkInterfacesRequestRequestTypeDef = TypedDict(
@@ -1012,34 +844,14 @@
 
 class ListDecoderManifestNetworkInterfacesRequestRequestTypeDef(
     _RequiredListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
     _OptionalListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
-    "_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
-    "_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef(
-    _RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
-    _OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDecoderManifestSignalsRequestRequestTypeDef = TypedDict(
     "_RequiredListDecoderManifestSignalsRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListDecoderManifestSignalsRequestRequestTypeDef = TypedDict(
@@ -1053,53 +865,24 @@
 
 class ListDecoderManifestSignalsRequestRequestTypeDef(
     _RequiredListDecoderManifestSignalsRequestRequestTypeDef,
     _OptionalListDecoderManifestSignalsRequestRequestTypeDef,
 ):
     pass
 
-ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef = TypedDict(
-    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
-    {
-        "modelManifestArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDecoderManifestsRequestRequestTypeDef = TypedDict(
     "ListDecoderManifestsRequestRequestTypeDef",
     {
         "modelManifestArn": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
-    "_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
-    {
-        "vehicleName": str,
-    },
-)
-_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
-    "_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef(
-    _RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
-    _OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
-):
-    pass
-
 _RequiredListFleetsForVehicleRequestRequestTypeDef = TypedDict(
     "_RequiredListFleetsForVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalListFleetsForVehicleRequestRequestTypeDef = TypedDict(
@@ -1113,60 +896,23 @@
 
 class ListFleetsForVehicleRequestRequestTypeDef(
     _RequiredListFleetsForVehicleRequestRequestTypeDef,
     _OptionalListFleetsForVehicleRequestRequestTypeDef,
 ):
     pass
 
-ListFleetsForVehicleResponseTypeDef = TypedDict(
-    "ListFleetsForVehicleResponseTypeDef",
-    {
-        "fleets": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
-    "ListFleetsRequestListFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFleetsRequestRequestTypeDef = TypedDict(
     "ListFleetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
-    "_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
-    "_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef(
-    _RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
-    _OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
-):
-    pass
-
 _RequiredListModelManifestNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListModelManifestNodesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListModelManifestNodesRequestRequestTypeDef = TypedDict(
@@ -1180,23 +926,14 @@
 
 class ListModelManifestNodesRequestRequestTypeDef(
     _RequiredListModelManifestNodesRequestRequestTypeDef,
     _OptionalListModelManifestNodesRequestRequestTypeDef,
 ):
     pass
 
-ListModelManifestsRequestListModelManifestsPaginateTypeDef = TypedDict(
-    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
-    {
-        "signalCatalogArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListModelManifestsRequestRequestTypeDef = TypedDict(
     "ListModelManifestsRequestRequestTypeDef",
     {
         "signalCatalogArn": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1223,34 +960,14 @@
 )
 
 class ModelManifestSummaryTypeDef(
     _RequiredModelManifestSummaryTypeDef, _OptionalModelManifestSummaryTypeDef
 ):
     pass
 
-_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
-    "_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
-    "_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef(
-    _RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
-    _OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
-):
-    pass
-
 _RequiredListSignalCatalogNodesRequestRequestTypeDef = TypedDict(
     "_RequiredListSignalCatalogNodesRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalListSignalCatalogNodesRequestRequestTypeDef = TypedDict(
@@ -1264,22 +981,14 @@
 
 class ListSignalCatalogNodesRequestRequestTypeDef(
     _RequiredListSignalCatalogNodesRequestRequestTypeDef,
     _OptionalListSignalCatalogNodesRequestRequestTypeDef,
 ):
     pass
 
-ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef = TypedDict(
-    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSignalCatalogsRequestRequestTypeDef = TypedDict(
     "ListSignalCatalogsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1299,34 +1008,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
-    "_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
-    {
-        "fleetId": str,
-    },
-)
-_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
-    "_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef(
-    _RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
-    _OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
-):
-    pass
-
 _RequiredListVehiclesInFleetRequestRequestTypeDef = TypedDict(
     "_RequiredListVehiclesInFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 _OptionalListVehiclesInFleetRequestRequestTypeDef = TypedDict(
@@ -1340,32 +1029,14 @@
 
 class ListVehiclesInFleetRequestRequestTypeDef(
     _RequiredListVehiclesInFleetRequestRequestTypeDef,
     _OptionalListVehiclesInFleetRequestRequestTypeDef,
 ):
     pass
 
-ListVehiclesInFleetResponseTypeDef = TypedDict(
-    "ListVehiclesInFleetResponseTypeDef",
-    {
-        "vehicles": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListVehiclesRequestListVehiclesPaginateTypeDef = TypedDict(
-    "ListVehiclesRequestListVehiclesPaginateTypeDef",
-    {
-        "modelManifestArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListVehiclesRequestRequestTypeDef = TypedDict(
     "ListVehiclesRequestRequestTypeDef",
     {
         "modelManifestArn": str,
         "nextToken": str,
         "maxResults": int,
     },
@@ -1402,14 +1073,38 @@
     },
     total=False,
 )
 
 class ObdInterfaceTypeDef(_RequiredObdInterfaceTypeDef, _OptionalObdInterfaceTypeDef):
     pass
 
+_RequiredSensorOutputTypeDef = TypedDict(
+    "_RequiredSensorOutputTypeDef",
+    {
+        "fullyQualifiedName": str,
+        "dataType": NodeDataTypeType,
+    },
+)
+_OptionalSensorOutputTypeDef = TypedDict(
+    "_OptionalSensorOutputTypeDef",
+    {
+        "description": str,
+        "unit": str,
+        "allowedValues": List[str],
+        "min": float,
+        "max": float,
+        "deprecationMessage": str,
+        "comment": str,
+    },
+    total=False,
+)
+
+class SensorOutputTypeDef(_RequiredSensorOutputTypeDef, _OptionalSensorOutputTypeDef):
+    pass
+
 _RequiredSensorTypeDef = TypedDict(
     "_RequiredSensorTypeDef",
     {
         "fullyQualifiedName": str,
         "dataType": NodeDataTypeType,
     },
 )
@@ -1450,43 +1145,22 @@
     },
     total=False,
 )
 
 class ObdSignalTypeDef(_RequiredObdSignalTypeDef, _OptionalObdSignalTypeDef):
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
 TimestreamResourcesTypeDef = TypedDict(
     "TimestreamResourcesTypeDef",
     {
         "timestreamDatabaseName": str,
         "timestreamTableName": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1508,33 +1182,14 @@
 )
 
 class UpdateCampaignRequestRequestTypeDef(
     _RequiredUpdateCampaignRequestRequestTypeDef, _OptionalUpdateCampaignRequestRequestTypeDef
 ):
     pass
 
-UpdateCampaignResponseTypeDef = TypedDict(
-    "UpdateCampaignResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "status": CampaignStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDecoderManifestResponseTypeDef = TypedDict(
-    "UpdateDecoderManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFleetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetRequestRequestTypeDef",
     {
         "fleetId": str,
     },
 )
 _OptionalUpdateFleetRequestRequestTypeDef = TypedDict(
@@ -1546,23 +1201,14 @@
 )
 
 class UpdateFleetRequestRequestTypeDef(
     _RequiredUpdateFleetRequestRequestTypeDef, _OptionalUpdateFleetRequestRequestTypeDef
 ):
     pass
 
-UpdateFleetResponseTypeDef = TypedDict(
-    "UpdateFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateModelManifestRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelManifestRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateModelManifestRequestRequestTypeDef = TypedDict(
@@ -1578,32 +1224,14 @@
 
 class UpdateModelManifestRequestRequestTypeDef(
     _RequiredUpdateModelManifestRequestRequestTypeDef,
     _OptionalUpdateModelManifestRequestRequestTypeDef,
 ):
     pass
 
-UpdateModelManifestResponseTypeDef = TypedDict(
-    "UpdateModelManifestResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSignalCatalogResponseTypeDef = TypedDict(
-    "UpdateSignalCatalogResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVehicleRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVehicleRequestRequestTypeDef",
     {
         "vehicleName": str,
     },
 )
 _OptionalUpdateVehicleRequestRequestTypeDef = TypedDict(
@@ -1618,29 +1246,275 @@
 )
 
 class UpdateVehicleRequestRequestTypeDef(
     _RequiredUpdateVehicleRequestRequestTypeDef, _OptionalUpdateVehicleRequestRequestTypeDef
 ):
     pass
 
-UpdateVehicleResponseTypeDef = TypedDict(
-    "UpdateVehicleResponseTypeDef",
+BatchCreateVehicleResponseTypeDef = TypedDict(
+    "BatchCreateVehicleResponseTypeDef",
+    {
+        "vehicles": List[CreateVehicleResponseItemTypeDef],
+        "errors": List[CreateVehicleErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCampaignResponseTypeDef = TypedDict(
+    "CreateCampaignResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDecoderManifestResponseTypeDef = TypedDict(
+    "CreateDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelManifestResponseTypeDef = TypedDict(
+    "CreateModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSignalCatalogResponseTypeDef = TypedDict(
+    "CreateSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVehicleResponseTypeDef = TypedDict(
+    "CreateVehicleResponseTypeDef",
     {
         "vehicleName": str,
         "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "thingArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchCreateVehicleResponseTypeDef = TypedDict(
-    "BatchCreateVehicleResponseTypeDef",
+DeleteCampaignResponseTypeDef = TypedDict(
+    "DeleteCampaignResponseTypeDef",
     {
-        "vehicles": List[CreateVehicleResponseItemTypeDef],
-        "errors": List[CreateVehicleErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDecoderManifestResponseTypeDef = TypedDict(
+    "DeleteDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFleetResponseTypeDef = TypedDict(
+    "DeleteFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteModelManifestResponseTypeDef = TypedDict(
+    "DeleteModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSignalCatalogResponseTypeDef = TypedDict(
+    "DeleteSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVehicleResponseTypeDef = TypedDict(
+    "DeleteVehicleResponseTypeDef",
+    {
+        "vehicleName": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDecoderManifestResponseTypeDef = TypedDict(
+    "GetDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "modelManifestArn": str,
+        "status": ManifestStatusType,
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFleetResponseTypeDef = TypedDict(
+    "GetFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "description": str,
+        "signalCatalogArn": str,
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelManifestResponseTypeDef = TypedDict(
+    "GetModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "description": str,
+        "signalCatalogArn": str,
+        "status": ManifestStatusType,
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVehicleResponseTypeDef = TypedDict(
+    "GetVehicleResponseTypeDef",
+    {
+        "vehicleName": str,
+        "arn": str,
+        "modelManifestArn": str,
+        "decoderManifestArn": str,
+        "attributes": Dict[str, str],
+        "creationTime": datetime,
+        "lastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportDecoderManifestResponseTypeDef = TypedDict(
+    "ImportDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportSignalCatalogResponseTypeDef = TypedDict(
+    "ImportSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFleetsForVehicleResponseTypeDef = TypedDict(
+    "ListFleetsForVehicleResponseTypeDef",
+    {
+        "fleets": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListVehiclesInFleetResponseTypeDef = TypedDict(
+    "ListVehiclesInFleetResponseTypeDef",
+    {
+        "vehicles": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCampaignResponseTypeDef = TypedDict(
+    "UpdateCampaignResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "status": CampaignStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDecoderManifestResponseTypeDef = TypedDict(
+    "UpdateDecoderManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFleetResponseTypeDef = TypedDict(
+    "UpdateFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateModelManifestResponseTypeDef = TypedDict(
+    "UpdateModelManifestResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSignalCatalogResponseTypeDef = TypedDict(
+    "UpdateSignalCatalogResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVehicleResponseTypeDef = TypedDict(
+    "UpdateVehicleResponseTypeDef",
+    {
+        "vehicleName": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateVehicleRequestRequestTypeDef = TypedDict(
     "BatchUpdateVehicleRequestRequestTypeDef",
     {
         "vehicles": Sequence[UpdateVehicleRequestItemTypeDef],
@@ -1648,40 +1522,50 @@
 )
 
 BatchUpdateVehicleResponseTypeDef = TypedDict(
     "BatchUpdateVehicleResponseTypeDef",
     {
         "vehicles": List[UpdateVehicleResponseItemTypeDef],
         "errors": List[UpdateVehicleErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListCampaignsResponseTypeDef = TypedDict(
-    "ListCampaignsResponseTypeDef",
+_RequiredCanDbcDefinitionTypeDef = TypedDict(
+    "_RequiredCanDbcDefinitionTypeDef",
     {
-        "campaignSummaries": List[CampaignSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "networkInterface": str,
+        "canDbcFiles": Sequence[BlobTypeDef],
     },
 )
-
-NetworkFileDefinitionTypeDef = TypedDict(
-    "NetworkFileDefinitionTypeDef",
+_OptionalCanDbcDefinitionTypeDef = TypedDict(
+    "_OptionalCanDbcDefinitionTypeDef",
     {
-        "canDbc": CanDbcDefinitionTypeDef,
+        "signalsMap": Mapping[str, str],
     },
     total=False,
 )
 
+class CanDbcDefinitionTypeDef(_RequiredCanDbcDefinitionTypeDef, _OptionalCanDbcDefinitionTypeDef):
+    pass
+
+ListCampaignsResponseTypeDef = TypedDict(
+    "ListCampaignsResponseTypeDef",
+    {
+        "campaignSummaries": List[CampaignSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetLoggingOptionsResponseTypeDef = TypedDict(
     "GetLoggingOptionsResponseTypeDef",
     {
         "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "cloudWatchLogDelivery": CloudWatchLogDeliveryOptionsTypeDef,
@@ -1787,15 +1671,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1813,24 +1697,24 @@
 )
 
 ListDecoderManifestsResponseTypeDef = TypedDict(
     "ListDecoderManifestsResponseTypeDef",
     {
         "summaries": List[DecoderManifestSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFleetsResponseTypeDef = TypedDict(
     "ListFleetsResponseTypeDef",
     {
         "fleetSummaries": List[FleetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredImportSignalCatalogRequestRequestTypeDef = TypedDict(
     "_RequiredImportSignalCatalogRequestRequestTypeDef",
     {
         "name": str,
@@ -1857,64 +1741,256 @@
     {
         "customerAccountId": str,
         "accountStatus": RegistrationStatusType,
         "timestreamRegistrationResponse": TimestreamRegistrationResponseTypeDef,
         "iamRegistrationResponse": IamRegistrationResponseTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSignalCatalogResponseTypeDef = TypedDict(
     "GetSignalCatalogResponseTypeDef",
     {
         "name": str,
         "arn": str,
         "description": str,
         "nodeCounts": NodeCountsTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
+    "_RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    {
+        "vehicleName": str,
+    },
+)
+_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = TypedDict(
+    "_OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef(
+    _RequiredGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    _OptionalGetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+):
+    pass
+
+ListCampaignsRequestListCampaignsPaginateTypeDef = TypedDict(
+    "ListCampaignsRequestListCampaignsPaginateTypeDef",
+    {
+        "status": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
+    "_RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = TypedDict(
+    "_OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef(
+    _RequiredListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+    _OptionalListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+):
+    pass
+
+_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
+    "_RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = TypedDict(
+    "_OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef(
+    _RequiredListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+    _OptionalListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+):
+    pass
+
+ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef = TypedDict(
+    "ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef",
+    {
+        "modelManifestArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
+    "_RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
+    {
+        "vehicleName": str,
+    },
+)
+_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = TypedDict(
+    "_OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef(
+    _RequiredListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+    _OptionalListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+):
+    pass
+
+ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
+    "ListFleetsRequestListFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
+    "_RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = TypedDict(
+    "_OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef(
+    _RequiredListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+    _OptionalListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+):
+    pass
+
+ListModelManifestsRequestListModelManifestsPaginateTypeDef = TypedDict(
+    "ListModelManifestsRequestListModelManifestsPaginateTypeDef",
+    {
+        "signalCatalogArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
+    "_RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = TypedDict(
+    "_OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef(
+    _RequiredListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+    _OptionalListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+):
+    pass
+
+ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef = TypedDict(
+    "ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
+    "_RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
+    {
+        "fleetId": str,
+    },
+)
+_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = TypedDict(
+    "_OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef(
+    _RequiredListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+    _OptionalListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+):
+    pass
+
+ListVehiclesRequestListVehiclesPaginateTypeDef = TypedDict(
+    "ListVehiclesRequestListVehiclesPaginateTypeDef",
+    {
+        "modelManifestArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 GetVehicleStatusResponseTypeDef = TypedDict(
     "GetVehicleStatusResponseTypeDef",
     {
         "campaigns": List[VehicleStatusTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListModelManifestsResponseTypeDef = TypedDict(
     "ListModelManifestsResponseTypeDef",
     {
         "summaries": List[ModelManifestSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalCatalogsResponseTypeDef = TypedDict(
     "ListSignalCatalogsResponseTypeDef",
     {
         "summaries": List[SignalCatalogSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVehiclesResponseTypeDef = TypedDict(
     "ListVehiclesResponseTypeDef",
     {
         "vehicleSummaries": List[VehicleSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNetworkInterfaceTypeDef = TypedDict(
     "_RequiredNetworkInterfaceTypeDef",
     {
         "interfaceId": str,
@@ -1929,14 +2005,25 @@
     },
     total=False,
 )
 
 class NetworkInterfaceTypeDef(_RequiredNetworkInterfaceTypeDef, _OptionalNetworkInterfaceTypeDef):
     pass
 
+NodeOutputTypeDef = TypedDict(
+    "NodeOutputTypeDef",
+    {
+        "branch": BranchTypeDef,
+        "sensor": SensorOutputTypeDef,
+        "actuator": ActuatorOutputTypeDef,
+        "attribute": AttributeOutputTypeDef,
+    },
+    total=False,
+)
+
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "branch": BranchTypeDef,
         "sensor": SensorTypeDef,
         "actuator": ActuatorTypeDef,
         "attribute": AttributeTypeDef,
@@ -1977,24 +2064,24 @@
     "RegisterAccountResponseTypeDef",
     {
         "registerAccountStatus": RegistrationStatusType,
         "timestreamResources": TimestreamResourcesTypeDef,
         "iamResources": IamResourcesTypeDef,
         "creationTime": datetime,
         "lastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImportDecoderManifestRequestRequestTypeDef = TypedDict(
-    "ImportDecoderManifestRequestRequestTypeDef",
+NetworkFileDefinitionTypeDef = TypedDict(
+    "NetworkFileDefinitionTypeDef",
     {
-        "name": str,
-        "networkFileDefinitions": Sequence[NetworkFileDefinitionTypeDef],
+        "canDbc": CanDbcDefinitionTypeDef,
     },
+    total=False,
 )
 
 BatchCreateVehicleRequestRequestTypeDef = TypedDict(
     "BatchCreateVehicleRequestRequestTypeDef",
     {
         "vehicles": Sequence[CreateVehicleRequestItemTypeDef],
     },
@@ -2009,16 +2096,16 @@
         "collectionScheme": CollectionSchemeTypeDef,
     },
 )
 _OptionalCreateCampaignRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCampaignRequestRequestTypeDef",
     {
         "description": str,
-        "startTime": Union[datetime, str],
-        "expiryTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "expiryTime": TimestampTypeDef,
         "postTriggerCollectionDuration": int,
         "diagnosticsMode": DiagnosticsModeType,
         "spoolingMode": SpoolingModeType,
         "compression": CompressionType,
         "priority": int,
         "signalsToCollect": Sequence[SignalInformationTypeDef],
         "dataExtraDimensions": Sequence[str],
@@ -2051,90 +2138,46 @@
         "priority": int,
         "signalsToCollect": List[SignalInformationTypeDef],
         "collectionScheme": CollectionSchemeTypeDef,
         "dataExtraDimensions": List[str],
         "creationTime": datetime,
         "lastModificationTime": datetime,
         "dataDestinationConfigs": List[DataDestinationConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDecoderManifestNetworkInterfacesResponseTypeDef = TypedDict(
     "ListDecoderManifestNetworkInterfacesResponseTypeDef",
     {
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSignalCatalogRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSignalCatalogRequestRequestTypeDef",
-    {
-        "description": str,
-        "nodes": Sequence[NodeTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateSignalCatalogRequestRequestTypeDef(
-    _RequiredCreateSignalCatalogRequestRequestTypeDef,
-    _OptionalCreateSignalCatalogRequestRequestTypeDef,
-):
-    pass
-
 ListModelManifestNodesResponseTypeDef = TypedDict(
     "ListModelManifestNodesResponseTypeDef",
     {
-        "nodes": List[NodeTypeDef],
+        "nodes": List[NodeOutputTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalCatalogNodesResponseTypeDef = TypedDict(
     "ListSignalCatalogNodesResponseTypeDef",
     {
-        "nodes": List[NodeTypeDef],
+        "nodes": List[NodeOutputTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
-    {
-        "description": str,
-        "nodesToAdd": Sequence[NodeTypeDef],
-        "nodesToUpdate": Sequence[NodeTypeDef],
-        "nodesToRemove": Sequence[str],
-    },
-    total=False,
-)
-
-class UpdateSignalCatalogRequestRequestTypeDef(
-    _RequiredUpdateSignalCatalogRequestRequestTypeDef,
-    _OptionalUpdateSignalCatalogRequestRequestTypeDef,
-):
-    pass
-
+NodeUnionTypeDef = Union[NodeTypeDef, NodeOutputTypeDef]
 _RequiredCreateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
         "modelManifestArn": str,
     },
 )
@@ -2156,15 +2199,15 @@
     pass
 
 ListDecoderManifestSignalsResponseTypeDef = TypedDict(
     "ListDecoderManifestSignalsResponseTypeDef",
     {
         "signalDecoders": List[SignalDecoderTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateDecoderManifestRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDecoderManifestRequestRequestTypeDef",
     {
         "name": str,
@@ -2186,7 +2229,60 @@
 )
 
 class UpdateDecoderManifestRequestRequestTypeDef(
     _RequiredUpdateDecoderManifestRequestRequestTypeDef,
     _OptionalUpdateDecoderManifestRequestRequestTypeDef,
 ):
     pass
+
+ImportDecoderManifestRequestRequestTypeDef = TypedDict(
+    "ImportDecoderManifestRequestRequestTypeDef",
+    {
+        "name": str,
+        "networkFileDefinitions": Sequence[NetworkFileDefinitionTypeDef],
+    },
+)
+
+_RequiredCreateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSignalCatalogRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSignalCatalogRequestRequestTypeDef",
+    {
+        "description": str,
+        "nodes": Sequence[NodeUnionTypeDef],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateSignalCatalogRequestRequestTypeDef(
+    _RequiredCreateSignalCatalogRequestRequestTypeDef,
+    _OptionalCreateSignalCatalogRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSignalCatalogRequestRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalUpdateSignalCatalogRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSignalCatalogRequestRequestTypeDef",
+    {
+        "description": str,
+        "nodesToAdd": Sequence[NodeUnionTypeDef],
+        "nodesToUpdate": Sequence[NodeUnionTypeDef],
+        "nodesToRemove": Sequence[str],
+    },
+    total=False,
+)
+
+class UpdateSignalCatalogRequestRequestTypeDef(
+    _RequiredUpdateSignalCatalogRequestRequestTypeDef,
+    _OptionalUpdateSignalCatalogRequestRequestTypeDef,
+):
+    pass
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotfleetwise
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTFleetWise 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTFleetWise 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotfleetwise type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotfleetwise type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotfleetwise"></a>
 
 # types-aiobotocore-iotfleetwise
 
 [![PyPI - types-aiobotocore-iotfleetwise](https://img.shields.io/pypi/v/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotfleetwise.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotfleetwise?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotfleetwise)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotfleetwise)](https://pepy.tech/project/types-aiobotocore-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTFleetWise 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
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
 [types-aiobotocore-iotfleetwise docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotfleetwise/).
 
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
@@ -380,136 +379,127 @@
 )
 
 
 def check_value(value: CampaignStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotfleetwise.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotfleetwise.type_defs import (
+    ActuatorOutputTypeDef,
     ActuatorTypeDef,
     AssociateVehicleFleetRequestRequestTypeDef,
+    AttributeOutputTypeDef,
     AttributeTypeDef,
     CreateVehicleErrorTypeDef,
     CreateVehicleResponseItemTypeDef,
+    ResponseMetadataTypeDef,
     UpdateVehicleRequestItemTypeDef,
     UpdateVehicleErrorTypeDef,
     UpdateVehicleResponseItemTypeDef,
+    BlobTypeDef,
     BranchTypeDef,
     CampaignSummaryTypeDef,
-    CanDbcDefinitionTypeDef,
     CanInterfaceTypeDef,
     CanSignalTypeDef,
     CloudWatchLogDeliveryOptionsTypeDef,
     ConditionBasedCollectionSchemeTypeDef,
     TimeBasedCollectionSchemeTypeDef,
     SignalInformationTypeDef,
     TagTypeDef,
-    CreateCampaignResponseTypeDef,
-    CreateDecoderManifestResponseTypeDef,
-    CreateFleetResponseTypeDef,
-    CreateModelManifestResponseTypeDef,
-    CreateSignalCatalogResponseTypeDef,
-    CreateVehicleResponseTypeDef,
+    TimestampTypeDef,
     S3ConfigTypeDef,
     TimestreamConfigTypeDef,
     DecoderManifestSummaryTypeDef,
     DeleteCampaignRequestRequestTypeDef,
-    DeleteCampaignResponseTypeDef,
     DeleteDecoderManifestRequestRequestTypeDef,
-    DeleteDecoderManifestResponseTypeDef,
     DeleteFleetRequestRequestTypeDef,
-    DeleteFleetResponseTypeDef,
     DeleteModelManifestRequestRequestTypeDef,
-    DeleteModelManifestResponseTypeDef,
     DeleteSignalCatalogRequestRequestTypeDef,
-    DeleteSignalCatalogResponseTypeDef,
     DeleteVehicleRequestRequestTypeDef,
-    DeleteVehicleResponseTypeDef,
     DisassociateVehicleFleetRequestRequestTypeDef,
     FleetSummaryTypeDef,
     FormattedVssTypeDef,
     GetCampaignRequestRequestTypeDef,
     GetDecoderManifestRequestRequestTypeDef,
-    GetDecoderManifestResponseTypeDef,
     GetFleetRequestRequestTypeDef,
-    GetFleetResponseTypeDef,
     GetModelManifestRequestRequestTypeDef,
-    GetModelManifestResponseTypeDef,
     IamRegistrationResponseTypeDef,
     TimestreamRegistrationResponseTypeDef,
     GetSignalCatalogRequestRequestTypeDef,
     NodeCountsTypeDef,
     GetVehicleRequestRequestTypeDef,
-    GetVehicleResponseTypeDef,
-    GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetVehicleStatusRequestRequestTypeDef,
     VehicleStatusTypeDef,
     IamResourcesTypeDef,
-    ImportDecoderManifestResponseTypeDef,
-    ImportSignalCatalogResponseTypeDef,
-    ListCampaignsRequestListCampaignsPaginateTypeDef,
     ListCampaignsRequestRequestTypeDef,
-    ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
     ListDecoderManifestNetworkInterfacesRequestRequestTypeDef,
-    ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
     ListDecoderManifestSignalsRequestRequestTypeDef,
-    ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef,
     ListDecoderManifestsRequestRequestTypeDef,
-    ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
     ListFleetsForVehicleRequestRequestTypeDef,
-    ListFleetsForVehicleResponseTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
-    ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
     ListModelManifestNodesRequestRequestTypeDef,
-    ListModelManifestsRequestListModelManifestsPaginateTypeDef,
     ListModelManifestsRequestRequestTypeDef,
     ModelManifestSummaryTypeDef,
-    ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
     ListSignalCatalogNodesRequestRequestTypeDef,
-    ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
     ListSignalCatalogsRequestRequestTypeDef,
     SignalCatalogSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
     ListVehiclesInFleetRequestRequestTypeDef,
-    ListVehiclesInFleetResponseTypeDef,
-    ListVehiclesRequestListVehiclesPaginateTypeDef,
     ListVehiclesRequestRequestTypeDef,
     VehicleSummaryTypeDef,
     ObdInterfaceTypeDef,
+    SensorOutputTypeDef,
     SensorTypeDef,
     ObdSignalTypeDef,
-    PaginatorConfigTypeDef,
     TimestreamResourcesTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateCampaignRequestRequestTypeDef,
+    UpdateFleetRequestRequestTypeDef,
+    UpdateModelManifestRequestRequestTypeDef,
+    UpdateVehicleRequestRequestTypeDef,
+    BatchCreateVehicleResponseTypeDef,
+    CreateCampaignResponseTypeDef,
+    CreateDecoderManifestResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    CreateModelManifestResponseTypeDef,
+    CreateSignalCatalogResponseTypeDef,
+    CreateVehicleResponseTypeDef,
+    DeleteCampaignResponseTypeDef,
+    DeleteDecoderManifestResponseTypeDef,
+    DeleteFleetResponseTypeDef,
+    DeleteModelManifestResponseTypeDef,
+    DeleteSignalCatalogResponseTypeDef,
+    DeleteVehicleResponseTypeDef,
+    GetDecoderManifestResponseTypeDef,
+    GetFleetResponseTypeDef,
+    GetModelManifestResponseTypeDef,
+    GetVehicleResponseTypeDef,
+    ImportDecoderManifestResponseTypeDef,
+    ImportSignalCatalogResponseTypeDef,
+    ListFleetsForVehicleResponseTypeDef,
+    ListVehiclesInFleetResponseTypeDef,
     UpdateCampaignResponseTypeDef,
     UpdateDecoderManifestResponseTypeDef,
-    UpdateFleetRequestRequestTypeDef,
     UpdateFleetResponseTypeDef,
-    UpdateModelManifestRequestRequestTypeDef,
     UpdateModelManifestResponseTypeDef,
     UpdateSignalCatalogResponseTypeDef,
-    UpdateVehicleRequestRequestTypeDef,
     UpdateVehicleResponseTypeDef,
-    BatchCreateVehicleResponseTypeDef,
     BatchUpdateVehicleRequestRequestTypeDef,
     BatchUpdateVehicleResponseTypeDef,
+    CanDbcDefinitionTypeDef,
     ListCampaignsResponseTypeDef,
-    NetworkFileDefinitionTypeDef,
     GetLoggingOptionsResponseTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     CollectionSchemeTypeDef,
     CreateFleetRequestRequestTypeDef,
     CreateModelManifestRequestRequestTypeDef,
     CreateVehicleRequestItemTypeDef,
     CreateVehicleRequestRequestTypeDef,
@@ -517,39 +507,55 @@
     TagResourceRequestRequestTypeDef,
     DataDestinationConfigTypeDef,
     ListDecoderManifestsResponseTypeDef,
     ListFleetsResponseTypeDef,
     ImportSignalCatalogRequestRequestTypeDef,
     GetRegisterAccountStatusResponseTypeDef,
     GetSignalCatalogResponseTypeDef,
+    GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef,
+    ListCampaignsRequestListCampaignsPaginateTypeDef,
+    ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef,
+    ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef,
+    ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef,
+    ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
+    ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef,
+    ListModelManifestsRequestListModelManifestsPaginateTypeDef,
+    ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef,
+    ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef,
+    ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef,
+    ListVehiclesRequestListVehiclesPaginateTypeDef,
     GetVehicleStatusResponseTypeDef,
     ListModelManifestsResponseTypeDef,
     ListSignalCatalogsResponseTypeDef,
     ListVehiclesResponseTypeDef,
     NetworkInterfaceTypeDef,
+    NodeOutputTypeDef,
     NodeTypeDef,
     SignalDecoderTypeDef,
     RegisterAccountRequestRequestTypeDef,
     RegisterAccountResponseTypeDef,
-    ImportDecoderManifestRequestRequestTypeDef,
+    NetworkFileDefinitionTypeDef,
     BatchCreateVehicleRequestRequestTypeDef,
     CreateCampaignRequestRequestTypeDef,
     GetCampaignResponseTypeDef,
     ListDecoderManifestNetworkInterfacesResponseTypeDef,
-    CreateSignalCatalogRequestRequestTypeDef,
     ListModelManifestNodesResponseTypeDef,
     ListSignalCatalogNodesResponseTypeDef,
-    UpdateSignalCatalogRequestRequestTypeDef,
+    NodeUnionTypeDef,
     CreateDecoderManifestRequestRequestTypeDef,
     ListDecoderManifestSignalsResponseTypeDef,
     UpdateDecoderManifestRequestRequestTypeDef,
+    ImportDecoderManifestRequestRequestTypeDef,
+    CreateSignalCatalogRequestRequestTypeDef,
+    UpdateSignalCatalogRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActuatorTypeDef:
+def get_value() -> ActuatorOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotfleetwise-2.5.2/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt` & `types-aiobotocore-iotfleetwise-2.5.2.post1/types_aiobotocore_iotfleetwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*


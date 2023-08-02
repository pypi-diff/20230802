# Comparing `tmp/types-aiobotocore-location-2.5.2.tar.gz` & `tmp/types-aiobotocore-location-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-location-2.5.2.tar", last modified: Sat Jul  8 01:43:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-location-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:35 2023, max compression
```

## Comparing `types-aiobotocore-location-2.5.2.tar` & `types-aiobotocore-location-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.274464 types-aiobotocore-location-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:14.000000 types-aiobotocore-location-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21454 2023-07-08 01:43:55.270464 types-aiobotocore-location-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19878 2023-07-08 01:34:14.000000 types-aiobotocore-location-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:55.274464 types-aiobotocore-location-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:34:14.000000 types-aiobotocore-location-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.266463 types-aiobotocore-location-2.5.2/types_aiobotocore_location/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-07-08 01:34:14.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-08 01:34:14.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-08 01:34:14.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48010 2023-07-08 01:34:15.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47933 2023-07-08 01:34:14.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-08 01:34:15.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-08 01:34:15.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-08 01:34:15.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-07-08 01:34:15.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:14.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64877 2023-07-08 01:34:17.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64766 2023-07-08 01:34:17.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:14.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.270464 types-aiobotocore-location-2.5.2/types_aiobotocore_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21454 2023-07-08 01:43:55.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-08 01:43:55.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:55.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:43:55.000000 types-aiobotocore-location-2.5.2/types_aiobotocore_location.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.633534 types-aiobotocore-location-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-08-02 14:52:35.629534 types-aiobotocore-location-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:35.633534 types-aiobotocore-location-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.625534 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-08-02 14:42:26.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47919 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-08-02 14:42:26.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-08-02 14:42:26.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-08-02 14:42:26.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-08-02 14:42:26.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    66009 2023-08-02 14:42:27.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65896 2023-08-02 14:42:26.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.629534 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-08-02 14:52:35.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:35.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:35.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:35.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-location-2.5.2/LICENSE` & `types-aiobotocore-location-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2/PKG-INFO` & `types-aiobotocore-location-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-location
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LocationService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LocationService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore location type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore location type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-location"></a>
 
 # types-aiobotocore-location
 
 [![PyPI - types-aiobotocore-location](https://img.shields.io/pypi/v/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-location?color=blue)](https://pypistats.org/packages/types-aiobotocore-location)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-location)](https://pepy.tech/project/types-aiobotocore-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LocationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [types-aiobotocore-location docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/).
 
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
@@ -356,152 +355,157 @@
 )
 
 
 def check_value(value: BatchItemErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_location.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_location.type_defs import (
     ApiKeyFilterTypeDef,
+    ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
+    TimestampTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
+    CircleOutputTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
-    CreateGeofenceCollectionResponseTypeDef,
-    CreateKeyResponseTypeDef,
     MapConfigurationTypeDef,
-    CreateMapResponseTypeDef,
     DataSourceConfigurationTypeDef,
-    CreatePlaceIndexResponseTypeDef,
     CreateRouteCalculatorRequestRequestTypeDef,
-    CreateRouteCalculatorResponseTypeDef,
     CreateTrackerRequestRequestTypeDef,
-    CreateTrackerResponseTypeDef,
     DeleteGeofenceCollectionRequestRequestTypeDef,
     DeleteKeyRequestRequestTypeDef,
     DeleteMapRequestRequestTypeDef,
     DeletePlaceIndexRequestRequestTypeDef,
     DeleteRouteCalculatorRequestRequestTypeDef,
     DeleteTrackerRequestRequestTypeDef,
     DescribeGeofenceCollectionRequestRequestTypeDef,
-    DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DescribeMapRequestRequestTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
-    DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerRequestRequestTypeDef,
-    DescribeTrackerResponseTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
-    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-    GetDevicePositionHistoryRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
-    GetMapGlyphsResponseTypeDef,
     GetMapSpritesRequestRequestTypeDef,
-    GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorRequestRequestTypeDef,
-    GetMapStyleDescriptorResponseTypeDef,
     GetMapTileRequestRequestTypeDef,
-    GetMapTileResponseTypeDef,
     GetPlaceRequestRequestTypeDef,
     LegGeometryTypeDef,
     StepTypeDef,
-    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
     ListDevicePositionsRequestRequestTypeDef,
-    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
     ListGeofenceCollectionsRequestRequestTypeDef,
     ListGeofenceCollectionsResponseEntryTypeDef,
-    ListGeofencesRequestListGeofencesPaginateTypeDef,
     ListGeofencesRequestRequestTypeDef,
-    ListMapsRequestListMapsPaginateTypeDef,
     ListMapsRequestRequestTypeDef,
     ListMapsResponseEntryTypeDef,
-    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
     ListPlaceIndexesRequestRequestTypeDef,
     ListPlaceIndexesResponseEntryTypeDef,
-    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
     ListRouteCalculatorsRequestRequestTypeDef,
     ListRouteCalculatorsResponseEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
     ListTrackerConsumersRequestRequestTypeDef,
-    ListTrackerConsumersResponseTypeDef,
-    ListTrackersRequestListTrackersPaginateTypeDef,
     ListTrackersRequestRequestTypeDef,
     ListTrackersResponseEntryTypeDef,
     MapConfigurationUpdateTypeDef,
-    PaginatorConfigTypeDef,
     PlaceGeometryTypeDef,
     TimeZoneTypeDef,
-    PutGeofenceResponseTypeDef,
-    ResponseMetadataTypeDef,
     RouteMatrixEntryErrorTypeDef,
     SearchForSuggestionsResultTypeDef,
     SearchPlaceIndexForPositionRequestRequestTypeDef,
     SearchPlaceIndexForPositionSummaryTypeDef,
     SearchPlaceIndexForSuggestionsRequestRequestTypeDef,
     SearchPlaceIndexForSuggestionsSummaryTypeDef,
     SearchPlaceIndexForTextRequestRequestTypeDef,
     SearchPlaceIndexForTextSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGeofenceCollectionRequestRequestTypeDef,
-    UpdateGeofenceCollectionResponseTypeDef,
-    UpdateKeyResponseTypeDef,
-    UpdateMapResponseTypeDef,
-    UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
-    UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerRequestRequestTypeDef,
-    UpdateTrackerResponseTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    CreateKeyRequestRequestTypeDef,
-    DescribeKeyResponseTypeDef,
     ListKeysResponseEntryTypeDef,
-    UpdateKeyRequestRequestTypeDef,
+    ApiKeyRestrictionsUnionTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
+    CreateGeofenceCollectionResponseTypeDef,
+    CreateKeyResponseTypeDef,
+    CreateMapResponseTypeDef,
+    CreatePlaceIndexResponseTypeDef,
+    CreateRouteCalculatorResponseTypeDef,
+    CreateTrackerResponseTypeDef,
+    DescribeGeofenceCollectionResponseTypeDef,
+    DescribeKeyResponseTypeDef,
+    DescribeRouteCalculatorResponseTypeDef,
+    DescribeTrackerResponseTypeDef,
+    GetMapGlyphsResponseTypeDef,
+    GetMapSpritesResponseTypeDef,
+    GetMapStyleDescriptorResponseTypeDef,
+    GetMapTileResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTrackerConsumersResponseTypeDef,
+    PutGeofenceResponseTypeDef,
+    UpdateGeofenceCollectionResponseTypeDef,
+    UpdateKeyResponseTypeDef,
+    UpdateMapResponseTypeDef,
+    UpdatePlaceIndexResponseTypeDef,
+    UpdateRouteCalculatorResponseTypeDef,
+    UpdateTrackerResponseTypeDef,
+    CreateKeyRequestRequestTypeDef,
+    GetDevicePositionHistoryRequestRequestTypeDef,
+    UpdateKeyRequestRequestTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
+    GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
     DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
     DescribePlaceIndexResponseTypeDef,
     UpdatePlaceIndexRequestRequestTypeDef,
     DevicePositionTypeDef,
     DevicePositionUpdateTypeDef,
     GetDevicePositionResponseTypeDef,
     ListDevicePositionsResponseEntryTypeDef,
+    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
+    ListGeofencesRequestListGeofencesPaginateTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
+    ListMapsRequestListMapsPaginateTypeDef,
+    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
+    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
+    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+    ListTrackersRequestListTrackersPaginateTypeDef,
     LegTypeDef,
     ListGeofenceCollectionsResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackersResponseTypeDef,
     UpdateMapRequestRequestTypeDef,
@@ -512,36 +516,37 @@
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
     CalculateRouteMatrixRequestRequestTypeDef,
     CalculateRouteRequestRequestTypeDef,
-    BatchPutGeofenceRequestEntryTypeDef,
     GetGeofenceResponseTypeDef,
     ListGeofenceResponseEntryTypeDef,
+    BatchPutGeofenceRequestEntryTypeDef,
+    GeofenceGeometryUnionTypeDef,
     PutGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     BatchEvaluateGeofencesRequestRequestTypeDef,
     BatchUpdateDevicePositionRequestRequestTypeDef,
     ListDevicePositionsResponseTypeDef,
     CalculateRouteResponseTypeDef,
     GetPlaceResponseTypeDef,
     SearchForPositionResultTypeDef,
     SearchForTextResultTypeDef,
     CalculateRouteMatrixResponseTypeDef,
-    BatchPutGeofenceRequestRequestTypeDef,
     ListGeofencesResponseTypeDef,
+    BatchPutGeofenceRequestRequestTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
 )
 
 
-def get_structure() -> ApiKeyFilterTypeDef:
+def get_value() -> ApiKeyFilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-location-2.5.2/README.md` & `types-aiobotocore-location-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-location"></a>
 
 # types-aiobotocore-location
 
 [![PyPI - types-aiobotocore-location](https://img.shields.io/pypi/v/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-location?color=blue)](https://pypistats.org/packages/types-aiobotocore-location)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-location)](https://pepy.tech/project/types-aiobotocore-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LocationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [types-aiobotocore-location docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/).
 
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
@@ -323,152 +323,157 @@
 )
 
 
 def check_value(value: BatchItemErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_location.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_location.type_defs import (
     ApiKeyFilterTypeDef,
+    ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
+    TimestampTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
+    CircleOutputTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
-    CreateGeofenceCollectionResponseTypeDef,
-    CreateKeyResponseTypeDef,
     MapConfigurationTypeDef,
-    CreateMapResponseTypeDef,
     DataSourceConfigurationTypeDef,
-    CreatePlaceIndexResponseTypeDef,
     CreateRouteCalculatorRequestRequestTypeDef,
-    CreateRouteCalculatorResponseTypeDef,
     CreateTrackerRequestRequestTypeDef,
-    CreateTrackerResponseTypeDef,
     DeleteGeofenceCollectionRequestRequestTypeDef,
     DeleteKeyRequestRequestTypeDef,
     DeleteMapRequestRequestTypeDef,
     DeletePlaceIndexRequestRequestTypeDef,
     DeleteRouteCalculatorRequestRequestTypeDef,
     DeleteTrackerRequestRequestTypeDef,
     DescribeGeofenceCollectionRequestRequestTypeDef,
-    DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DescribeMapRequestRequestTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
-    DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerRequestRequestTypeDef,
-    DescribeTrackerResponseTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
-    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-    GetDevicePositionHistoryRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
-    GetMapGlyphsResponseTypeDef,
     GetMapSpritesRequestRequestTypeDef,
-    GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorRequestRequestTypeDef,
-    GetMapStyleDescriptorResponseTypeDef,
     GetMapTileRequestRequestTypeDef,
-    GetMapTileResponseTypeDef,
     GetPlaceRequestRequestTypeDef,
     LegGeometryTypeDef,
     StepTypeDef,
-    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
     ListDevicePositionsRequestRequestTypeDef,
-    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
     ListGeofenceCollectionsRequestRequestTypeDef,
     ListGeofenceCollectionsResponseEntryTypeDef,
-    ListGeofencesRequestListGeofencesPaginateTypeDef,
     ListGeofencesRequestRequestTypeDef,
-    ListMapsRequestListMapsPaginateTypeDef,
     ListMapsRequestRequestTypeDef,
     ListMapsResponseEntryTypeDef,
-    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
     ListPlaceIndexesRequestRequestTypeDef,
     ListPlaceIndexesResponseEntryTypeDef,
-    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
     ListRouteCalculatorsRequestRequestTypeDef,
     ListRouteCalculatorsResponseEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
     ListTrackerConsumersRequestRequestTypeDef,
-    ListTrackerConsumersResponseTypeDef,
-    ListTrackersRequestListTrackersPaginateTypeDef,
     ListTrackersRequestRequestTypeDef,
     ListTrackersResponseEntryTypeDef,
     MapConfigurationUpdateTypeDef,
-    PaginatorConfigTypeDef,
     PlaceGeometryTypeDef,
     TimeZoneTypeDef,
-    PutGeofenceResponseTypeDef,
-    ResponseMetadataTypeDef,
     RouteMatrixEntryErrorTypeDef,
     SearchForSuggestionsResultTypeDef,
     SearchPlaceIndexForPositionRequestRequestTypeDef,
     SearchPlaceIndexForPositionSummaryTypeDef,
     SearchPlaceIndexForSuggestionsRequestRequestTypeDef,
     SearchPlaceIndexForSuggestionsSummaryTypeDef,
     SearchPlaceIndexForTextRequestRequestTypeDef,
     SearchPlaceIndexForTextSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGeofenceCollectionRequestRequestTypeDef,
-    UpdateGeofenceCollectionResponseTypeDef,
-    UpdateKeyResponseTypeDef,
-    UpdateMapResponseTypeDef,
-    UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
-    UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerRequestRequestTypeDef,
-    UpdateTrackerResponseTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    CreateKeyRequestRequestTypeDef,
-    DescribeKeyResponseTypeDef,
     ListKeysResponseEntryTypeDef,
-    UpdateKeyRequestRequestTypeDef,
+    ApiKeyRestrictionsUnionTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
+    CreateGeofenceCollectionResponseTypeDef,
+    CreateKeyResponseTypeDef,
+    CreateMapResponseTypeDef,
+    CreatePlaceIndexResponseTypeDef,
+    CreateRouteCalculatorResponseTypeDef,
+    CreateTrackerResponseTypeDef,
+    DescribeGeofenceCollectionResponseTypeDef,
+    DescribeKeyResponseTypeDef,
+    DescribeRouteCalculatorResponseTypeDef,
+    DescribeTrackerResponseTypeDef,
+    GetMapGlyphsResponseTypeDef,
+    GetMapSpritesResponseTypeDef,
+    GetMapStyleDescriptorResponseTypeDef,
+    GetMapTileResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTrackerConsumersResponseTypeDef,
+    PutGeofenceResponseTypeDef,
+    UpdateGeofenceCollectionResponseTypeDef,
+    UpdateKeyResponseTypeDef,
+    UpdateMapResponseTypeDef,
+    UpdatePlaceIndexResponseTypeDef,
+    UpdateRouteCalculatorResponseTypeDef,
+    UpdateTrackerResponseTypeDef,
+    CreateKeyRequestRequestTypeDef,
+    GetDevicePositionHistoryRequestRequestTypeDef,
+    UpdateKeyRequestRequestTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
+    GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
     DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
     DescribePlaceIndexResponseTypeDef,
     UpdatePlaceIndexRequestRequestTypeDef,
     DevicePositionTypeDef,
     DevicePositionUpdateTypeDef,
     GetDevicePositionResponseTypeDef,
     ListDevicePositionsResponseEntryTypeDef,
+    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
+    ListGeofencesRequestListGeofencesPaginateTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
+    ListMapsRequestListMapsPaginateTypeDef,
+    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
+    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
+    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+    ListTrackersRequestListTrackersPaginateTypeDef,
     LegTypeDef,
     ListGeofenceCollectionsResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackersResponseTypeDef,
     UpdateMapRequestRequestTypeDef,
@@ -479,36 +484,37 @@
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
     CalculateRouteMatrixRequestRequestTypeDef,
     CalculateRouteRequestRequestTypeDef,
-    BatchPutGeofenceRequestEntryTypeDef,
     GetGeofenceResponseTypeDef,
     ListGeofenceResponseEntryTypeDef,
+    BatchPutGeofenceRequestEntryTypeDef,
+    GeofenceGeometryUnionTypeDef,
     PutGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     BatchEvaluateGeofencesRequestRequestTypeDef,
     BatchUpdateDevicePositionRequestRequestTypeDef,
     ListDevicePositionsResponseTypeDef,
     CalculateRouteResponseTypeDef,
     GetPlaceResponseTypeDef,
     SearchForPositionResultTypeDef,
     SearchForTextResultTypeDef,
     CalculateRouteMatrixResponseTypeDef,
-    BatchPutGeofenceRequestRequestTypeDef,
     ListGeofencesResponseTypeDef,
+    BatchPutGeofenceRequestRequestTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
 )
 
 
-def get_structure() -> ApiKeyFilterTypeDef:
+def get_value() -> ApiKeyFilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-location-2.5.2/setup.py` & `types-aiobotocore-location-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-location",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_location"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LocationService 2.5.2 service generated with"
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
-    keywords="aiobotocore location type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore location type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_location": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/"
```

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location/__init__.py` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location/__init__.pyi` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location/__main__.py` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LocationService 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.LocationService 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService\nOther"
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

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location/client.py` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("location") as client:
         client: LocationServiceClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import DistanceUnitType, PositionFilteringType, PricingPlanType, TravelModeType
 from .paginator import (
     GetDevicePositionHistoryPaginator,
@@ -32,15 +31,15 @@
     ListPlaceIndexesPaginator,
     ListRouteCalculatorsPaginator,
     ListTrackerConsumersPaginator,
     ListTrackersPaginator,
 )
 from .type_defs import (
     ApiKeyFilterTypeDef,
-    ApiKeyRestrictionsTypeDef,
+    ApiKeyRestrictionsUnionTypeDef,
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
@@ -58,15 +57,15 @@
     DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyResponseTypeDef,
     DescribeMapResponseTypeDef,
     DescribePlaceIndexResponseTypeDef,
     DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerResponseTypeDef,
     DevicePositionUpdateTypeDef,
-    GeofenceGeometryTypeDef,
+    GeofenceGeometryUnionTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     GetDevicePositionResponseTypeDef,
     GetGeofenceResponseTypeDef,
     GetMapGlyphsResponseTypeDef,
     GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorResponseTypeDef,
     GetMapTileResponseTypeDef,
@@ -83,14 +82,15 @@
     ListTrackersResponseTypeDef,
     MapConfigurationTypeDef,
     MapConfigurationUpdateTypeDef,
     PutGeofenceResponseTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForSuggestionsResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
+    TimestampTypeDef,
     UpdateGeofenceCollectionResponseTypeDef,
     UpdateKeyResponseTypeDef,
     UpdateMapResponseTypeDef,
     UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerResponseTypeDef,
 )
@@ -218,15 +218,15 @@
         self,
         *,
         CalculatorName: str,
         DeparturePosition: Sequence[float],
         DestinationPosition: Sequence[float],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
-        DepartureTime: Union[datetime, str] = ...,
+        DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         IncludeLegGeometry: bool = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,
         WaypointPositions: Sequence[Sequence[float]] = ...
     ) -> CalculateRouteResponseTypeDef:
         """
@@ -243,15 +243,15 @@
         self,
         *,
         CalculatorName: str,
         DeparturePositions: Sequence[Sequence[float]],
         DestinationPositions: Sequence[Sequence[float]],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
-        DepartureTime: Union[datetime, str] = ...,
+        DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...
     ) -> CalculateRouteMatrixResponseTypeDef:
         """
         [Calculates a route
         matrix](https://docs.aws.amazon.com/location/latest/developerguide/calculate-
@@ -295,17 +295,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_geofence_collection)
         """
 
     async def create_key(
         self,
         *,
         KeyName: str,
-        Restrictions: ApiKeyRestrictionsTypeDef,
+        Restrictions: ApiKeyRestrictionsUnionTypeDef,
         Description: str = ...,
-        ExpireTime: Union[datetime, str] = ...,
+        ExpireTime: TimestampTypeDef = ...,
         NoExpiry: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateKeyResponseTypeDef:
         """
         Creates an API key resource in your Amazon Web Services account, which lets you
         grant `geo:GetMap*` actions for Amazon Location Map resources to the API key
         bearer.
@@ -518,18 +518,18 @@
         """
 
     async def get_device_position_history(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
-        EndTimeExclusive: Union[datetime, str] = ...,
+        EndTimeExclusive: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StartTimeInclusive: Union[datetime, str] = ...
+        StartTimeInclusive: TimestampTypeDef = ...
     ) -> GetDevicePositionHistoryResponseTypeDef:
         """
         Retrieves the device position history from a tracker resource within a specified
         range of time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_device_position_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#get_device_position_history)
@@ -697,15 +697,15 @@
         """
 
     async def put_geofence(
         self,
         *,
         CollectionName: str,
         GeofenceId: str,
-        Geometry: GeofenceGeometryTypeDef,
+        Geometry: GeofenceGeometryUnionTypeDef,
         GeofenceProperties: Mapping[str, str] = ...
     ) -> PutGeofenceResponseTypeDef:
         """
         Stores a geofence geometry in a given geofence collection, or updates the
         geometry of an existing geofence if a geofence ID is included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)
@@ -800,18 +800,18 @@
         """
 
     async def update_key(
         self,
         *,
         KeyName: str,
         Description: str = ...,
-        ExpireTime: Union[datetime, str] = ...,
+        ExpireTime: TimestampTypeDef = ...,
         ForceUpdate: bool = ...,
         NoExpiry: bool = ...,
-        Restrictions: ApiKeyRestrictionsTypeDef = ...
+        Restrictions: ApiKeyRestrictionsUnionTypeDef = ...
     ) -> UpdateKeyResponseTypeDef:
         """
         Updates the specified properties of a given API key resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_key)
         """
```

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location/client.pyi` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("location") as client:
         client: LocationServiceClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import DistanceUnitType, PositionFilteringType, PricingPlanType, TravelModeType
 from .paginator import (
     GetDevicePositionHistoryPaginator,
@@ -32,15 +31,15 @@
     ListPlaceIndexesPaginator,
     ListRouteCalculatorsPaginator,
     ListTrackerConsumersPaginator,
     ListTrackersPaginator,
 )
 from .type_defs import (
     ApiKeyFilterTypeDef,
-    ApiKeyRestrictionsTypeDef,
+    ApiKeyRestrictionsUnionTypeDef,
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
@@ -58,15 +57,15 @@
     DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyResponseTypeDef,
     DescribeMapResponseTypeDef,
     DescribePlaceIndexResponseTypeDef,
     DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerResponseTypeDef,
     DevicePositionUpdateTypeDef,
-    GeofenceGeometryTypeDef,
+    GeofenceGeometryUnionTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     GetDevicePositionResponseTypeDef,
     GetGeofenceResponseTypeDef,
     GetMapGlyphsResponseTypeDef,
     GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorResponseTypeDef,
     GetMapTileResponseTypeDef,
@@ -83,14 +82,15 @@
     ListTrackersResponseTypeDef,
     MapConfigurationTypeDef,
     MapConfigurationUpdateTypeDef,
     PutGeofenceResponseTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForSuggestionsResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
+    TimestampTypeDef,
     UpdateGeofenceCollectionResponseTypeDef,
     UpdateKeyResponseTypeDef,
     UpdateMapResponseTypeDef,
     UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerResponseTypeDef,
 )
@@ -206,15 +206,15 @@
         self,
         *,
         CalculatorName: str,
         DeparturePosition: Sequence[float],
         DestinationPosition: Sequence[float],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
-        DepartureTime: Union[datetime, str] = ...,
+        DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         IncludeLegGeometry: bool = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,
         WaypointPositions: Sequence[Sequence[float]] = ...
     ) -> CalculateRouteResponseTypeDef:
         """
@@ -230,15 +230,15 @@
         self,
         *,
         CalculatorName: str,
         DeparturePositions: Sequence[Sequence[float]],
         DestinationPositions: Sequence[Sequence[float]],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
-        DepartureTime: Union[datetime, str] = ...,
+        DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...
     ) -> CalculateRouteMatrixResponseTypeDef:
         """
         [Calculates a route
         matrix](https://docs.aws.amazon.com/location/latest/developerguide/calculate-
@@ -278,17 +278,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_geofence_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_geofence_collection)
         """
     async def create_key(
         self,
         *,
         KeyName: str,
-        Restrictions: ApiKeyRestrictionsTypeDef,
+        Restrictions: ApiKeyRestrictionsUnionTypeDef,
         Description: str = ...,
-        ExpireTime: Union[datetime, str] = ...,
+        ExpireTime: TimestampTypeDef = ...,
         NoExpiry: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateKeyResponseTypeDef:
         """
         Creates an API key resource in your Amazon Web Services account, which lets you
         grant `geo:GetMap*` actions for Amazon Location Map resources to the API key
         bearer.
@@ -481,18 +481,18 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#get_device_position)
         """
     async def get_device_position_history(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
-        EndTimeExclusive: Union[datetime, str] = ...,
+        EndTimeExclusive: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        StartTimeInclusive: Union[datetime, str] = ...
+        StartTimeInclusive: TimestampTypeDef = ...
     ) -> GetDevicePositionHistoryResponseTypeDef:
         """
         Retrieves the device position history from a tracker resource within a specified
         range of time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_device_position_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#get_device_position_history)
@@ -643,15 +643,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#list_trackers)
         """
     async def put_geofence(
         self,
         *,
         CollectionName: str,
         GeofenceId: str,
-        Geometry: GeofenceGeometryTypeDef,
+        Geometry: GeofenceGeometryUnionTypeDef,
         GeofenceProperties: Mapping[str, str] = ...
     ) -> PutGeofenceResponseTypeDef:
         """
         Stores a geofence geometry in a given geofence collection, or updates the
         geometry of an existing geofence if a geofence ID is included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)
@@ -739,18 +739,18 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_geofence_collection)
         """
     async def update_key(
         self,
         *,
         KeyName: str,
         Description: str = ...,
-        ExpireTime: Union[datetime, str] = ...,
+        ExpireTime: TimestampTypeDef = ...,
         ForceUpdate: bool = ...,
         NoExpiry: bool = ...,
-        Restrictions: ApiKeyRestrictionsTypeDef = ...
+        Restrictions: ApiKeyRestrictionsUnionTypeDef = ...
     ) -> UpdateKeyResponseTypeDef:
         """
         Updates the specified properties of a given API key resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_key)
         """
```

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location/literals.py` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location/literals.pyi` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location/paginator.py` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         list_maps_paginator: ListMapsPaginator = client.get_paginator("list_maps")
         list_place_indexes_paginator: ListPlaceIndexesPaginator = client.get_paginator("list_place_indexes")
         list_route_calculators_paginator: ListRouteCalculatorsPaginator = client.get_paginator("list_route_calculators")
         list_tracker_consumers_paginator: ListTrackerConsumersPaginator = client.get_paginator("list_tracker_consumers")
         list_trackers_paginator: ListTrackersPaginator = client.get_paginator("list_trackers")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ApiKeyFilterTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
@@ -53,14 +52,15 @@
     ListKeysResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackerConsumersResponseTypeDef,
     ListTrackersResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "GetDevicePositionHistoryPaginator",
     "ListDevicePositionsPaginator",
     "ListGeofenceCollectionsPaginator",
     "ListGeofencesPaginator",
@@ -68,172 +68,160 @@
     "ListMapsPaginator",
     "ListPlaceIndexesPaginator",
     "ListRouteCalculatorsPaginator",
     "ListTrackerConsumersPaginator",
     "ListTrackersPaginator",
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
 class GetDevicePositionHistoryPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#getdevicepositionhistorypaginator)
     """
 
     def paginate(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
-        EndTimeExclusive: Union[datetime, str] = ...,
-        StartTimeInclusive: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        EndTimeExclusive: TimestampTypeDef = ...,
+        StartTimeInclusive: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetDevicePositionHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#getdevicepositionhistorypaginator)
         """
 
-
 class ListDevicePositionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listdevicepositionspaginator)
     """
 
     def paginate(
-        self, *, TrackerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TrackerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDevicePositionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listdevicepositionspaginator)
         """
 
-
 class ListGeofenceCollectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listgeofencecollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGeofenceCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listgeofencecollectionspaginator)
         """
 
-
 class ListGeofencesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listgeofencespaginator)
     """
 
     def paginate(
-        self, *, CollectionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CollectionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGeofencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listgeofencespaginator)
         """
 
-
 class ListKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, Filter: ApiKeyFilterTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Filter: ApiKeyFilterTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listkeyspaginator)
         """
 
-
 class ListMapsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listmapspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMapsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listmapspaginator)
         """
 
-
 class ListPlaceIndexesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listplaceindexespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPlaceIndexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listplaceindexespaginator)
         """
 
-
 class ListRouteCalculatorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listroutecalculatorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRouteCalculatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listroutecalculatorspaginator)
         """
 
-
 class ListTrackerConsumersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listtrackerconsumerspaginator)
     """
 
     def paginate(
-        self, *, TrackerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TrackerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTrackerConsumersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listtrackerconsumerspaginator)
         """
 
-
 class ListTrackersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listtrackerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTrackersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listtrackerspaginator)
         """
```

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location/paginator.pyi` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/paginator.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         list_maps_paginator: ListMapsPaginator = client.get_paginator("list_maps")
         list_place_indexes_paginator: ListPlaceIndexesPaginator = client.get_paginator("list_place_indexes")
         list_route_calculators_paginator: ListRouteCalculatorsPaginator = client.get_paginator("list_route_calculators")
         list_tracker_consumers_paginator: ListTrackerConsumersPaginator = client.get_paginator("list_tracker_consumers")
         list_trackers_paginator: ListTrackersPaginator = client.get_paginator("list_trackers")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ApiKeyFilterTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
@@ -53,14 +52,15 @@
     ListKeysResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackerConsumersResponseTypeDef,
     ListTrackersResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "GetDevicePositionHistoryPaginator",
     "ListDevicePositionsPaginator",
     "ListGeofenceCollectionsPaginator",
     "ListGeofencesPaginator",
@@ -68,160 +68,172 @@
     "ListMapsPaginator",
     "ListPlaceIndexesPaginator",
     "ListRouteCalculatorsPaginator",
     "ListTrackerConsumersPaginator",
     "ListTrackersPaginator",
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
 class GetDevicePositionHistoryPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#getdevicepositionhistorypaginator)
     """
 
     def paginate(
         self,
         *,
         DeviceId: str,
         TrackerName: str,
-        EndTimeExclusive: Union[datetime, str] = ...,
-        StartTimeInclusive: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        EndTimeExclusive: TimestampTypeDef = ...,
+        StartTimeInclusive: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetDevicePositionHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.GetDevicePositionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#getdevicepositionhistorypaginator)
         """
 
+
 class ListDevicePositionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listdevicepositionspaginator)
     """
 
     def paginate(
-        self, *, TrackerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TrackerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDevicePositionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListDevicePositions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listdevicepositionspaginator)
         """
 
+
 class ListGeofenceCollectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listgeofencecollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGeofenceCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofenceCollections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listgeofencecollectionspaginator)
         """
 
+
 class ListGeofencesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listgeofencespaginator)
     """
 
     def paginate(
-        self, *, CollectionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CollectionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGeofencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListGeofences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listgeofencespaginator)
         """
 
+
 class ListKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listkeyspaginator)
     """
 
     def paginate(
-        self, *, Filter: ApiKeyFilterTypeDef = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Filter: ApiKeyFilterTypeDef = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listkeyspaginator)
         """
 
+
 class ListMapsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listmapspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMapsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListMaps.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listmapspaginator)
         """
 
+
 class ListPlaceIndexesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listplaceindexespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPlaceIndexesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListPlaceIndexes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listplaceindexespaginator)
         """
 
+
 class ListRouteCalculatorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listroutecalculatorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRouteCalculatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListRouteCalculators.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listroutecalculatorspaginator)
         """
 
+
 class ListTrackerConsumersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listtrackerconsumerspaginator)
     """
 
     def paginate(
-        self, *, TrackerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TrackerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTrackerConsumersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackerConsumers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listtrackerconsumerspaginator)
         """
 
+
 class ListTrackersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listtrackerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTrackersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Paginator.ListTrackers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/paginators/#listtrackerspaginator)
         """
```

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location/type_defs.py` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_location.type_defs import ApiKeyFilterTypeDef
 
-    data: ApiKeyFilterTypeDef = {...}
+    data: ApiKeyFilterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -34,142 +34,147 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApiKeyFilterTypeDef",
+    "ApiKeyRestrictionsOutputTypeDef",
     "ApiKeyRestrictionsTypeDef",
     "AssociateTrackerConsumerRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDeleteGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionRequestRequestTypeDef",
     "BatchPutGeofenceSuccessTypeDef",
     "CalculateRouteCarModeOptionsTypeDef",
+    "TimestampTypeDef",
     "CalculateRouteMatrixSummaryTypeDef",
     "CalculateRouteSummaryTypeDef",
     "TruckDimensionsTypeDef",
     "TruckWeightTypeDef",
+    "CircleOutputTypeDef",
     "CircleTypeDef",
     "CreateGeofenceCollectionRequestRequestTypeDef",
-    "CreateGeofenceCollectionResponseTypeDef",
-    "CreateKeyResponseTypeDef",
     "MapConfigurationTypeDef",
-    "CreateMapResponseTypeDef",
     "DataSourceConfigurationTypeDef",
-    "CreatePlaceIndexResponseTypeDef",
     "CreateRouteCalculatorRequestRequestTypeDef",
-    "CreateRouteCalculatorResponseTypeDef",
     "CreateTrackerRequestRequestTypeDef",
-    "CreateTrackerResponseTypeDef",
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     "DeleteKeyRequestRequestTypeDef",
     "DeleteMapRequestRequestTypeDef",
     "DeletePlaceIndexRequestRequestTypeDef",
     "DeleteRouteCalculatorRequestRequestTypeDef",
     "DeleteTrackerRequestRequestTypeDef",
     "DescribeGeofenceCollectionRequestRequestTypeDef",
-    "DescribeGeofenceCollectionResponseTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DescribeMapRequestRequestTypeDef",
     "DescribePlaceIndexRequestRequestTypeDef",
     "DescribeRouteCalculatorRequestRequestTypeDef",
-    "DescribeRouteCalculatorResponseTypeDef",
     "DescribeTrackerRequestRequestTypeDef",
-    "DescribeTrackerResponseTypeDef",
     "PositionalAccuracyTypeDef",
     "DisassociateTrackerConsumerRequestRequestTypeDef",
-    "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    "GetDevicePositionHistoryRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "GetDevicePositionRequestRequestTypeDef",
     "GetGeofenceRequestRequestTypeDef",
     "GetMapGlyphsRequestRequestTypeDef",
-    "GetMapGlyphsResponseTypeDef",
     "GetMapSpritesRequestRequestTypeDef",
-    "GetMapSpritesResponseTypeDef",
     "GetMapStyleDescriptorRequestRequestTypeDef",
-    "GetMapStyleDescriptorResponseTypeDef",
     "GetMapTileRequestRequestTypeDef",
-    "GetMapTileResponseTypeDef",
     "GetPlaceRequestRequestTypeDef",
     "LegGeometryTypeDef",
     "StepTypeDef",
-    "ListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
     "ListDevicePositionsRequestRequestTypeDef",
-    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
     "ListGeofenceCollectionsRequestRequestTypeDef",
     "ListGeofenceCollectionsResponseEntryTypeDef",
-    "ListGeofencesRequestListGeofencesPaginateTypeDef",
     "ListGeofencesRequestRequestTypeDef",
-    "ListMapsRequestListMapsPaginateTypeDef",
     "ListMapsRequestRequestTypeDef",
     "ListMapsResponseEntryTypeDef",
-    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
     "ListPlaceIndexesRequestRequestTypeDef",
     "ListPlaceIndexesResponseEntryTypeDef",
-    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
     "ListRouteCalculatorsRequestRequestTypeDef",
     "ListRouteCalculatorsResponseEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
     "ListTrackerConsumersRequestRequestTypeDef",
-    "ListTrackerConsumersResponseTypeDef",
-    "ListTrackersRequestListTrackersPaginateTypeDef",
     "ListTrackersRequestRequestTypeDef",
     "ListTrackersResponseEntryTypeDef",
     "MapConfigurationUpdateTypeDef",
-    "PaginatorConfigTypeDef",
     "PlaceGeometryTypeDef",
     "TimeZoneTypeDef",
-    "PutGeofenceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RouteMatrixEntryErrorTypeDef",
     "SearchForSuggestionsResultTypeDef",
     "SearchPlaceIndexForPositionRequestRequestTypeDef",
     "SearchPlaceIndexForPositionSummaryTypeDef",
     "SearchPlaceIndexForSuggestionsRequestRequestTypeDef",
     "SearchPlaceIndexForSuggestionsSummaryTypeDef",
     "SearchPlaceIndexForTextRequestRequestTypeDef",
     "SearchPlaceIndexForTextSummaryTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGeofenceCollectionRequestRequestTypeDef",
-    "UpdateGeofenceCollectionResponseTypeDef",
-    "UpdateKeyResponseTypeDef",
-    "UpdateMapResponseTypeDef",
-    "UpdatePlaceIndexResponseTypeDef",
     "UpdateRouteCalculatorRequestRequestTypeDef",
-    "UpdateRouteCalculatorResponseTypeDef",
     "UpdateTrackerRequestRequestTypeDef",
-    "UpdateTrackerResponseTypeDef",
-    "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
-    "CreateKeyRequestRequestTypeDef",
-    "DescribeKeyResponseTypeDef",
     "ListKeysResponseEntryTypeDef",
-    "UpdateKeyRequestRequestTypeDef",
+    "ApiKeyRestrictionsUnionTypeDef",
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     "BatchDeleteGeofenceErrorTypeDef",
     "BatchEvaluateGeofencesErrorTypeDef",
     "BatchGetDevicePositionErrorTypeDef",
     "BatchPutGeofenceErrorTypeDef",
     "BatchUpdateDevicePositionErrorTypeDef",
+    "CreateGeofenceCollectionResponseTypeDef",
+    "CreateKeyResponseTypeDef",
+    "CreateMapResponseTypeDef",
+    "CreatePlaceIndexResponseTypeDef",
+    "CreateRouteCalculatorResponseTypeDef",
+    "CreateTrackerResponseTypeDef",
+    "DescribeGeofenceCollectionResponseTypeDef",
+    "DescribeKeyResponseTypeDef",
+    "DescribeRouteCalculatorResponseTypeDef",
+    "DescribeTrackerResponseTypeDef",
+    "GetMapGlyphsResponseTypeDef",
+    "GetMapSpritesResponseTypeDef",
+    "GetMapStyleDescriptorResponseTypeDef",
+    "GetMapTileResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTrackerConsumersResponseTypeDef",
+    "PutGeofenceResponseTypeDef",
+    "UpdateGeofenceCollectionResponseTypeDef",
+    "UpdateKeyResponseTypeDef",
+    "UpdateMapResponseTypeDef",
+    "UpdatePlaceIndexResponseTypeDef",
+    "UpdateRouteCalculatorResponseTypeDef",
+    "UpdateTrackerResponseTypeDef",
+    "CreateKeyRequestRequestTypeDef",
+    "GetDevicePositionHistoryRequestRequestTypeDef",
+    "UpdateKeyRequestRequestTypeDef",
     "CalculateRouteTruckModeOptionsTypeDef",
+    "GeofenceGeometryOutputTypeDef",
     "GeofenceGeometryTypeDef",
     "CreateMapRequestRequestTypeDef",
     "DescribeMapResponseTypeDef",
     "CreatePlaceIndexRequestRequestTypeDef",
     "DescribePlaceIndexResponseTypeDef",
     "UpdatePlaceIndexRequestRequestTypeDef",
     "DevicePositionTypeDef",
     "DevicePositionUpdateTypeDef",
     "GetDevicePositionResponseTypeDef",
     "ListDevicePositionsResponseEntryTypeDef",
+    "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+    "ListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
+    "ListGeofencesRequestListGeofencesPaginateTypeDef",
+    "ListKeysRequestListKeysPaginateTypeDef",
+    "ListMapsRequestListMapsPaginateTypeDef",
+    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
+    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
+    "ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    "ListTrackersRequestListTrackersPaginateTypeDef",
     "LegTypeDef",
     "ListGeofenceCollectionsResponseTypeDef",
     "ListMapsResponseTypeDef",
     "ListPlaceIndexesResponseTypeDef",
     "ListRouteCalculatorsResponseTypeDef",
     "ListTrackersResponseTypeDef",
     "UpdateMapRequestRequestTypeDef",
@@ -180,42 +185,65 @@
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     "BatchDeleteGeofenceResponseTypeDef",
     "BatchEvaluateGeofencesResponseTypeDef",
     "BatchPutGeofenceResponseTypeDef",
     "BatchUpdateDevicePositionResponseTypeDef",
     "CalculateRouteMatrixRequestRequestTypeDef",
     "CalculateRouteRequestRequestTypeDef",
-    "BatchPutGeofenceRequestEntryTypeDef",
     "GetGeofenceResponseTypeDef",
     "ListGeofenceResponseEntryTypeDef",
+    "BatchPutGeofenceRequestEntryTypeDef",
+    "GeofenceGeometryUnionTypeDef",
     "PutGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionResponseTypeDef",
     "GetDevicePositionHistoryResponseTypeDef",
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     "BatchUpdateDevicePositionRequestRequestTypeDef",
     "ListDevicePositionsResponseTypeDef",
     "CalculateRouteResponseTypeDef",
     "GetPlaceResponseTypeDef",
     "SearchForPositionResultTypeDef",
     "SearchForTextResultTypeDef",
     "CalculateRouteMatrixResponseTypeDef",
-    "BatchPutGeofenceRequestRequestTypeDef",
     "ListGeofencesResponseTypeDef",
+    "BatchPutGeofenceRequestRequestTypeDef",
     "SearchPlaceIndexForPositionResponseTypeDef",
     "SearchPlaceIndexForTextResponseTypeDef",
 )
 
 ApiKeyFilterTypeDef = TypedDict(
     "ApiKeyFilterTypeDef",
     {
         "KeyStatus": StatusType,
     },
     total=False,
 )
 
+_RequiredApiKeyRestrictionsOutputTypeDef = TypedDict(
+    "_RequiredApiKeyRestrictionsOutputTypeDef",
+    {
+        "AllowActions": List[str],
+        "AllowResources": List[str],
+    },
+)
+_OptionalApiKeyRestrictionsOutputTypeDef = TypedDict(
+    "_OptionalApiKeyRestrictionsOutputTypeDef",
+    {
+        "AllowReferers": List[str],
+    },
+    total=False,
+)
+
+
+class ApiKeyRestrictionsOutputTypeDef(
+    _RequiredApiKeyRestrictionsOutputTypeDef, _OptionalApiKeyRestrictionsOutputTypeDef
+):
+    pass
+
+
 _RequiredApiKeyRestrictionsTypeDef = TypedDict(
     "_RequiredApiKeyRestrictionsTypeDef",
     {
         "AllowActions": Sequence[str],
         "AllowResources": Sequence[str],
     },
 )
@@ -255,14 +283,25 @@
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
     {
         "DeviceIds": Sequence[str],
         "TrackerName": str,
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
 BatchDeleteGeofenceRequestRequestTypeDef = TypedDict(
     "BatchDeleteGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceIds": Sequence[str],
     },
 )
@@ -289,14 +328,15 @@
     {
         "AvoidFerries": bool,
         "AvoidTolls": bool,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 CalculateRouteMatrixSummaryTypeDef = TypedDict(
     "CalculateRouteMatrixSummaryTypeDef",
     {
         "DataSource": str,
         "DistanceUnit": DistanceUnitType,
         "ErrorCount": int,
         "RouteCount": int,
@@ -330,14 +370,22 @@
     {
         "Total": float,
         "Unit": VehicleWeightUnitType,
     },
     total=False,
 )
 
+CircleOutputTypeDef = TypedDict(
+    "CircleOutputTypeDef",
+    {
+        "Center": List[float],
+        "Radius": float,
+    },
+)
+
 CircleTypeDef = TypedDict(
     "CircleTypeDef",
     {
         "Center": Sequence[float],
         "Radius": float,
     },
 )
@@ -364,35 +412,14 @@
 class CreateGeofenceCollectionRequestRequestTypeDef(
     _RequiredCreateGeofenceCollectionRequestRequestTypeDef,
     _OptionalCreateGeofenceCollectionRequestRequestTypeDef,
 ):
     pass
 
 
-CreateGeofenceCollectionResponseTypeDef = TypedDict(
-    "CreateGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "CreateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateKeyResponseTypeDef = TypedDict(
-    "CreateKeyResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Key": str,
-        "KeyArn": str,
-        "KeyName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMapConfigurationTypeDef = TypedDict(
     "_RequiredMapConfigurationTypeDef",
     {
         "Style": str,
     },
 )
 _OptionalMapConfigurationTypeDef = TypedDict(
@@ -404,42 +431,22 @@
 )
 
 
 class MapConfigurationTypeDef(_RequiredMapConfigurationTypeDef, _OptionalMapConfigurationTypeDef):
     pass
 
 
-CreateMapResponseTypeDef = TypedDict(
-    "CreateMapResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "MapArn": str,
-        "MapName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
         "IntendedUse": IntendedUseType,
     },
     total=False,
 )
 
-CreatePlaceIndexResponseTypeDef = TypedDict(
-    "CreatePlaceIndexResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "IndexArn": str,
-        "IndexName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateRouteCalculatorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
         "DataSource": str,
     },
 )
@@ -457,24 +464,14 @@
 class CreateRouteCalculatorRequestRequestTypeDef(
     _RequiredCreateRouteCalculatorRequestRequestTypeDef,
     _OptionalCreateRouteCalculatorRequestRequestTypeDef,
 ):
     pass
 
 
-CreateRouteCalculatorResponseTypeDef = TypedDict(
-    "CreateRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "CreateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalCreateTrackerRequestRequestTypeDef = TypedDict(
@@ -493,24 +490,14 @@
 
 class CreateTrackerRequestRequestTypeDef(
     _RequiredCreateTrackerRequestRequestTypeDef, _OptionalCreateTrackerRequestRequestTypeDef
 ):
     pass
 
 
-CreateTrackerResponseTypeDef = TypedDict(
-    "CreateTrackerResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "TrackerArn": str,
-        "TrackerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
@@ -552,30 +539,14 @@
 DescribeGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DescribeGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
-DescribeGeofenceCollectionResponseTypeDef = TypedDict(
-    "DescribeGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "CreateTime": datetime,
-        "Description": str,
-        "KmsKeyId": str,
-        "PricingPlan": PricingPlanType,
-        "PricingPlanDataSource": str,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeKeyRequestRequestTypeDef = TypedDict(
     "DescribeKeyRequestRequestTypeDef",
     {
         "KeyName": str,
     },
 )
 
@@ -596,53 +567,21 @@
 DescribeRouteCalculatorRequestRequestTypeDef = TypedDict(
     "DescribeRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
     },
 )
 
-DescribeRouteCalculatorResponseTypeDef = TypedDict(
-    "DescribeRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "CreateTime": datetime,
-        "DataSource": str,
-        "Description": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeTrackerRequestRequestTypeDef = TypedDict(
     "DescribeTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 
-DescribeTrackerResponseTypeDef = TypedDict(
-    "DescribeTrackerResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Description": str,
-        "KmsKeyId": str,
-        "PositionFiltering": PositionFilteringType,
-        "PricingPlan": PricingPlanType,
-        "PricingPlanDataSource": str,
-        "Tags": Dict[str, str],
-        "TrackerArn": str,
-        "TrackerName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PositionalAccuracyTypeDef = TypedDict(
     "PositionalAccuracyTypeDef",
     {
         "Horizontal": float,
     },
 )
 
@@ -650,65 +589,24 @@
     "DisassociateTrackerConsumerRequestRequestTypeDef",
     {
         "ConsumerArn": str,
         "TrackerName": str,
     },
 )
 
-_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "TrackerName": str,
-    },
-)
-_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    {
-        "EndTimeExclusive": Union[datetime, str],
-        "StartTimeInclusive": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
-    _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-    _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredGetDevicePositionHistoryRequestRequestTypeDef",
-    {
-        "DeviceId": str,
-        "TrackerName": str,
-    },
-)
-_OptionalGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalGetDevicePositionHistoryRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "EndTimeExclusive": Union[datetime, str],
-        "MaxResults": int,
-        "NextToken": str,
-        "StartTimeInclusive": Union[datetime, str],
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetDevicePositionHistoryRequestRequestTypeDef(
-    _RequiredGetDevicePositionHistoryRequestRequestTypeDef,
-    _OptionalGetDevicePositionHistoryRequestRequestTypeDef,
-):
-    pass
-
-
 GetDevicePositionRequestRequestTypeDef = TypedDict(
     "GetDevicePositionRequestRequestTypeDef",
     {
         "DeviceId": str,
         "TrackerName": str,
     },
 )
@@ -740,24 +638,14 @@
 
 class GetMapGlyphsRequestRequestTypeDef(
     _RequiredGetMapGlyphsRequestRequestTypeDef, _OptionalGetMapGlyphsRequestRequestTypeDef
 ):
     pass
 
 
-GetMapGlyphsResponseTypeDef = TypedDict(
-    "GetMapGlyphsResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMapSpritesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapSpritesRequestRequestTypeDef",
     {
         "FileName": str,
         "MapName": str,
     },
 )
@@ -772,24 +660,14 @@
 
 class GetMapSpritesRequestRequestTypeDef(
     _RequiredGetMapSpritesRequestRequestTypeDef, _OptionalGetMapSpritesRequestRequestTypeDef
 ):
     pass
 
 
-GetMapSpritesResponseTypeDef = TypedDict(
-    "GetMapSpritesResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMapStyleDescriptorRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapStyleDescriptorRequestRequestTypeDef",
     {
         "MapName": str,
     },
 )
 _OptionalGetMapStyleDescriptorRequestRequestTypeDef = TypedDict(
@@ -804,24 +682,14 @@
 class GetMapStyleDescriptorRequestRequestTypeDef(
     _RequiredGetMapStyleDescriptorRequestRequestTypeDef,
     _OptionalGetMapStyleDescriptorRequestRequestTypeDef,
 ):
     pass
 
 
-GetMapStyleDescriptorResponseTypeDef = TypedDict(
-    "GetMapStyleDescriptorResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMapTileRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapTileRequestRequestTypeDef",
     {
         "MapName": str,
         "X": str,
         "Y": str,
         "Z": str,
@@ -838,24 +706,14 @@
 
 class GetMapTileRequestRequestTypeDef(
     _RequiredGetMapTileRequestRequestTypeDef, _OptionalGetMapTileRequestRequestTypeDef
 ):
     pass
 
 
-GetMapTileResponseTypeDef = TypedDict(
-    "GetMapTileResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPlaceRequestRequestTypeDef = TypedDict(
     "_RequiredGetPlaceRequestRequestTypeDef",
     {
         "IndexName": str,
         "PlaceId": str,
     },
 )
@@ -900,36 +758,14 @@
 )
 
 
 class StepTypeDef(_RequiredStepTypeDef, _OptionalStepTypeDef):
     pass
 
 
-_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
-    "_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    {
-        "TrackerName": str,
-    },
-)
-_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
-    "_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(
-    _RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-    _OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDevicePositionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevicePositionsRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalListDevicePositionsRequestRequestTypeDef = TypedDict(
@@ -945,22 +781,14 @@
 class ListDevicePositionsRequestRequestTypeDef(
     _RequiredListDevicePositionsRequestRequestTypeDef,
     _OptionalListDevicePositionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = TypedDict(
-    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGeofenceCollectionsRequestRequestTypeDef = TypedDict(
     "ListGeofenceCollectionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -988,36 +816,14 @@
 class ListGeofenceCollectionsResponseEntryTypeDef(
     _RequiredListGeofenceCollectionsResponseEntryTypeDef,
     _OptionalListGeofenceCollectionsResponseEntryTypeDef,
 ):
     pass
 
 
-_RequiredListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
-    "_RequiredListGeofencesRequestListGeofencesPaginateTypeDef",
-    {
-        "CollectionName": str,
-    },
-)
-_OptionalListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
-    "_OptionalListGeofencesRequestListGeofencesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGeofencesRequestListGeofencesPaginateTypeDef(
-    _RequiredListGeofencesRequestListGeofencesPaginateTypeDef,
-    _OptionalListGeofencesRequestListGeofencesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGeofencesRequestRequestTypeDef = TypedDict(
     "_RequiredListGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 _OptionalListGeofencesRequestRequestTypeDef = TypedDict(
@@ -1032,22 +838,14 @@
 
 class ListGeofencesRequestRequestTypeDef(
     _RequiredListGeofencesRequestRequestTypeDef, _OptionalListGeofencesRequestRequestTypeDef
 ):
     pass
 
 
-ListMapsRequestListMapsPaginateTypeDef = TypedDict(
-    "ListMapsRequestListMapsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMapsRequestRequestTypeDef = TypedDict(
     "ListMapsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1074,22 +872,14 @@
 
 class ListMapsResponseEntryTypeDef(
     _RequiredListMapsResponseEntryTypeDef, _OptionalListMapsResponseEntryTypeDef
 ):
     pass
 
 
-ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = TypedDict(
-    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPlaceIndexesRequestRequestTypeDef = TypedDict(
     "ListPlaceIndexesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1116,22 +906,14 @@
 
 class ListPlaceIndexesResponseEntryTypeDef(
     _RequiredListPlaceIndexesResponseEntryTypeDef, _OptionalListPlaceIndexesResponseEntryTypeDef
 ):
     pass
 
 
-ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = TypedDict(
-    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRouteCalculatorsRequestRequestTypeDef = TypedDict(
     "ListRouteCalculatorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1166,44 +948,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
-    "_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    {
-        "TrackerName": str,
-    },
-)
-_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
-    "_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(
-    _RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-    _OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTrackerConsumersRequestRequestTypeDef = TypedDict(
     "_RequiredListTrackerConsumersRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalListTrackerConsumersRequestRequestTypeDef = TypedDict(
@@ -1219,31 +971,14 @@
 class ListTrackerConsumersRequestRequestTypeDef(
     _RequiredListTrackerConsumersRequestRequestTypeDef,
     _OptionalListTrackerConsumersRequestRequestTypeDef,
 ):
     pass
 
 
-ListTrackerConsumersResponseTypeDef = TypedDict(
-    "ListTrackerConsumersResponseTypeDef",
-    {
-        "ConsumerArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTrackersRequestListTrackersPaginateTypeDef = TypedDict(
-    "ListTrackersRequestListTrackersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTrackersRequestRequestTypeDef = TypedDict(
     "ListTrackersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1278,24 +1013,14 @@
     "MapConfigurationUpdateTypeDef",
     {
         "PoliticalView": str,
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
 PlaceGeometryTypeDef = TypedDict(
     "PlaceGeometryTypeDef",
     {
         "Point": List[float],
     },
     total=False,
 )
@@ -1315,35 +1040,14 @@
 )
 
 
 class TimeZoneTypeDef(_RequiredTimeZoneTypeDef, _OptionalTimeZoneTypeDef):
     pass
 
 
-PutGeofenceResponseTypeDef = TypedDict(
-    "PutGeofenceResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "GeofenceId": str,
-        "UpdateTime": datetime,
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
 _RequiredRouteMatrixEntryErrorTypeDef = TypedDict(
     "_RequiredRouteMatrixEntryErrorTypeDef",
     {
         "Code": RouteMatrixErrorCodeType,
     },
 )
 _OptionalRouteMatrixEntryErrorTypeDef = TypedDict(
@@ -1580,54 +1284,14 @@
 class UpdateGeofenceCollectionRequestRequestTypeDef(
     _RequiredUpdateGeofenceCollectionRequestRequestTypeDef,
     _OptionalUpdateGeofenceCollectionRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateGeofenceCollectionResponseTypeDef = TypedDict(
-    "UpdateGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateKeyResponseTypeDef = TypedDict(
-    "UpdateKeyResponseTypeDef",
-    {
-        "KeyArn": str,
-        "KeyName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateMapResponseTypeDef = TypedDict(
-    "UpdateMapResponseTypeDef",
-    {
-        "MapArn": str,
-        "MapName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdatePlaceIndexResponseTypeDef = TypedDict(
-    "UpdatePlaceIndexResponseTypeDef",
-    {
-        "IndexArn": str,
-        "IndexName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateRouteCalculatorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
     },
 )
 _OptionalUpdateRouteCalculatorRequestRequestTypeDef = TypedDict(
@@ -1643,24 +1307,14 @@
 class UpdateRouteCalculatorRequestRequestTypeDef(
     _RequiredUpdateRouteCalculatorRequestRequestTypeDef,
     _OptionalUpdateRouteCalculatorRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateRouteCalculatorResponseTypeDef = TypedDict(
-    "UpdateRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalUpdateTrackerRequestRequestTypeDef = TypedDict(
@@ -1677,195 +1331,448 @@
 
 class UpdateTrackerRequestRequestTypeDef(
     _RequiredUpdateTrackerRequestRequestTypeDef, _OptionalUpdateTrackerRequestRequestTypeDef
 ):
     pass
 
 
-UpdateTrackerResponseTypeDef = TypedDict(
-    "UpdateTrackerResponseTypeDef",
-    {
-        "TrackerArn": str,
-        "TrackerName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListKeysRequestListKeysPaginateTypeDef = TypedDict(
-    "ListKeysRequestListKeysPaginateTypeDef",
-    {
-        "Filter": ApiKeyFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKeysRequestRequestTypeDef = TypedDict(
     "ListKeysRequestRequestTypeDef",
     {
         "Filter": ApiKeyFilterTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredCreateKeyRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyRequestRequestTypeDef",
+_RequiredListKeysResponseEntryTypeDef = TypedDict(
+    "_RequiredListKeysResponseEntryTypeDef",
     {
+        "CreateTime": datetime,
+        "ExpireTime": datetime,
         "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
+        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
+        "UpdateTime": datetime,
     },
 )
-_OptionalCreateKeyRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyRequestRequestTypeDef",
+_OptionalListKeysResponseEntryTypeDef = TypedDict(
+    "_OptionalListKeysResponseEntryTypeDef",
     {
         "Description": str,
-        "ExpireTime": Union[datetime, str],
-        "NoExpiry": bool,
-        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class CreateKeyRequestRequestTypeDef(
-    _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
+class ListKeysResponseEntryTypeDef(
+    _RequiredListKeysResponseEntryTypeDef, _OptionalListKeysResponseEntryTypeDef
 ):
     pass
 
 
+ApiKeyRestrictionsUnionTypeDef = Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef]
+BatchDeleteDevicePositionHistoryErrorTypeDef = TypedDict(
+    "BatchDeleteDevicePositionHistoryErrorTypeDef",
+    {
+        "DeviceId": str,
+        "Error": BatchItemErrorTypeDef,
+    },
+)
+
+BatchDeleteGeofenceErrorTypeDef = TypedDict(
+    "BatchDeleteGeofenceErrorTypeDef",
+    {
+        "Error": BatchItemErrorTypeDef,
+        "GeofenceId": str,
+    },
+)
+
+BatchEvaluateGeofencesErrorTypeDef = TypedDict(
+    "BatchEvaluateGeofencesErrorTypeDef",
+    {
+        "DeviceId": str,
+        "Error": BatchItemErrorTypeDef,
+        "SampleTime": datetime,
+    },
+)
+
+BatchGetDevicePositionErrorTypeDef = TypedDict(
+    "BatchGetDevicePositionErrorTypeDef",
+    {
+        "DeviceId": str,
+        "Error": BatchItemErrorTypeDef,
+    },
+)
+
+BatchPutGeofenceErrorTypeDef = TypedDict(
+    "BatchPutGeofenceErrorTypeDef",
+    {
+        "Error": BatchItemErrorTypeDef,
+        "GeofenceId": str,
+    },
+)
+
+BatchUpdateDevicePositionErrorTypeDef = TypedDict(
+    "BatchUpdateDevicePositionErrorTypeDef",
+    {
+        "DeviceId": str,
+        "Error": BatchItemErrorTypeDef,
+        "SampleTime": datetime,
+    },
+)
+
+CreateGeofenceCollectionResponseTypeDef = TypedDict(
+    "CreateGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "CreateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKeyResponseTypeDef = TypedDict(
+    "CreateKeyResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Key": str,
+        "KeyArn": str,
+        "KeyName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMapResponseTypeDef = TypedDict(
+    "CreateMapResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "MapArn": str,
+        "MapName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePlaceIndexResponseTypeDef = TypedDict(
+    "CreatePlaceIndexResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "IndexArn": str,
+        "IndexName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRouteCalculatorResponseTypeDef = TypedDict(
+    "CreateRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "CreateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrackerResponseTypeDef = TypedDict(
+    "CreateTrackerResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "TrackerArn": str,
+        "TrackerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGeofenceCollectionResponseTypeDef = TypedDict(
+    "DescribeGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "CreateTime": datetime,
+        "Description": str,
+        "KmsKeyId": str,
+        "PricingPlan": PricingPlanType,
+        "PricingPlanDataSource": str,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeKeyResponseTypeDef = TypedDict(
     "DescribeKeyResponseTypeDef",
     {
         "CreateTime": datetime,
         "Description": str,
         "ExpireTime": datetime,
         "Key": str,
         "KeyArn": str,
         "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
+        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListKeysResponseEntryTypeDef = TypedDict(
-    "_RequiredListKeysResponseEntryTypeDef",
+DescribeRouteCalculatorResponseTypeDef = TypedDict(
+    "DescribeRouteCalculatorResponseTypeDef",
     {
+        "CalculatorArn": str,
+        "CalculatorName": str,
         "CreateTime": datetime,
-        "ExpireTime": datetime,
-        "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
+        "DataSource": str,
+        "Description": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
         "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListKeysResponseEntryTypeDef = TypedDict(
-    "_OptionalListKeysResponseEntryTypeDef",
+
+DescribeTrackerResponseTypeDef = TypedDict(
+    "DescribeTrackerResponseTypeDef",
     {
+        "CreateTime": datetime,
         "Description": str,
+        "KmsKeyId": str,
+        "PositionFiltering": PositionFilteringType,
+        "PricingPlan": PricingPlanType,
+        "PricingPlanDataSource": str,
+        "Tags": Dict[str, str],
+        "TrackerArn": str,
+        "TrackerName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetMapGlyphsResponseTypeDef = TypedDict(
+    "GetMapGlyphsResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ListKeysResponseEntryTypeDef(
-    _RequiredListKeysResponseEntryTypeDef, _OptionalListKeysResponseEntryTypeDef
-):
-    pass
+GetMapSpritesResponseTypeDef = TypedDict(
+    "GetMapSpritesResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetMapStyleDescriptorResponseTypeDef = TypedDict(
+    "GetMapStyleDescriptorResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredUpdateKeyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateKeyRequestRequestTypeDef",
+GetMapTileResponseTypeDef = TypedDict(
+    "GetMapTileResponseTypeDef",
     {
-        "KeyName": str,
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateKeyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateKeyRequestRequestTypeDef",
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "Description": str,
-        "ExpireTime": Union[datetime, str],
-        "ForceUpdate": bool,
-        "NoExpiry": bool,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListTrackerConsumersResponseTypeDef = TypedDict(
+    "ListTrackerConsumersResponseTypeDef",
+    {
+        "ConsumerArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateKeyRequestRequestTypeDef(
-    _RequiredUpdateKeyRequestRequestTypeDef, _OptionalUpdateKeyRequestRequestTypeDef
-):
-    pass
+PutGeofenceResponseTypeDef = TypedDict(
+    "PutGeofenceResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "GeofenceId": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateGeofenceCollectionResponseTypeDef = TypedDict(
+    "UpdateGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-BatchDeleteDevicePositionHistoryErrorTypeDef = TypedDict(
-    "BatchDeleteDevicePositionHistoryErrorTypeDef",
+UpdateKeyResponseTypeDef = TypedDict(
+    "UpdateKeyResponseTypeDef",
     {
-        "DeviceId": str,
-        "Error": BatchItemErrorTypeDef,
+        "KeyArn": str,
+        "KeyName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDeleteGeofenceErrorTypeDef = TypedDict(
-    "BatchDeleteGeofenceErrorTypeDef",
+UpdateMapResponseTypeDef = TypedDict(
+    "UpdateMapResponseTypeDef",
     {
-        "Error": BatchItemErrorTypeDef,
-        "GeofenceId": str,
+        "MapArn": str,
+        "MapName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchEvaluateGeofencesErrorTypeDef = TypedDict(
-    "BatchEvaluateGeofencesErrorTypeDef",
+UpdatePlaceIndexResponseTypeDef = TypedDict(
+    "UpdatePlaceIndexResponseTypeDef",
     {
-        "DeviceId": str,
-        "Error": BatchItemErrorTypeDef,
-        "SampleTime": datetime,
+        "IndexArn": str,
+        "IndexName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetDevicePositionErrorTypeDef = TypedDict(
-    "BatchGetDevicePositionErrorTypeDef",
+UpdateRouteCalculatorResponseTypeDef = TypedDict(
+    "UpdateRouteCalculatorResponseTypeDef",
     {
-        "DeviceId": str,
-        "Error": BatchItemErrorTypeDef,
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutGeofenceErrorTypeDef = TypedDict(
-    "BatchPutGeofenceErrorTypeDef",
+UpdateTrackerResponseTypeDef = TypedDict(
+    "UpdateTrackerResponseTypeDef",
     {
-        "Error": BatchItemErrorTypeDef,
-        "GeofenceId": str,
+        "TrackerArn": str,
+        "TrackerName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchUpdateDevicePositionErrorTypeDef = TypedDict(
-    "BatchUpdateDevicePositionErrorTypeDef",
+_RequiredCreateKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyRequestRequestTypeDef",
+    {
+        "KeyName": str,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
+    },
+)
+_OptionalCreateKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ExpireTime": TimestampTypeDef,
+        "NoExpiry": bool,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateKeyRequestRequestTypeDef(
+    _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetDevicePositionHistoryRequestRequestTypeDef",
     {
         "DeviceId": str,
-        "Error": BatchItemErrorTypeDef,
-        "SampleTime": datetime,
+        "TrackerName": str,
+    },
+)
+_OptionalGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetDevicePositionHistoryRequestRequestTypeDef",
+    {
+        "EndTimeExclusive": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "StartTimeInclusive": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class GetDevicePositionHistoryRequestRequestTypeDef(
+    _RequiredGetDevicePositionHistoryRequestRequestTypeDef,
+    _OptionalGetDevicePositionHistoryRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateKeyRequestRequestTypeDef",
+    {
+        "KeyName": str,
     },
 )
+_OptionalUpdateKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateKeyRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ExpireTime": TimestampTypeDef,
+        "ForceUpdate": bool,
+        "NoExpiry": bool,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateKeyRequestRequestTypeDef(
+    _RequiredUpdateKeyRequestRequestTypeDef, _OptionalUpdateKeyRequestRequestTypeDef
+):
+    pass
+
 
 CalculateRouteTruckModeOptionsTypeDef = TypedDict(
     "CalculateRouteTruckModeOptionsTypeDef",
     {
         "AvoidFerries": bool,
         "AvoidTolls": bool,
         "Dimensions": TruckDimensionsTypeDef,
         "Weight": TruckWeightTypeDef,
     },
     total=False,
 )
 
+GeofenceGeometryOutputTypeDef = TypedDict(
+    "GeofenceGeometryOutputTypeDef",
+    {
+        "Circle": CircleOutputTypeDef,
+        "Polygon": List[List[List[float]]],
+    },
+    total=False,
+)
+
 GeofenceGeometryTypeDef = TypedDict(
     "GeofenceGeometryTypeDef",
     {
         "Circle": CircleTypeDef,
         "Polygon": Sequence[Sequence[Sequence[float]]],
     },
     total=False,
@@ -1903,15 +1810,15 @@
         "DataSource": str,
         "Description": str,
         "MapArn": str,
         "MapName": str,
         "PricingPlan": PricingPlanType,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlaceIndexRequestRequestTypeDef",
     {
         "DataSource": str,
@@ -1944,15 +1851,15 @@
         "DataSourceConfiguration": DataSourceConfigurationTypeDef,
         "Description": str,
         "IndexArn": str,
         "IndexName": str,
         "PricingPlan": PricingPlanType,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePlaceIndexRequestRequestTypeDef",
     {
         "IndexName": str,
@@ -1999,15 +1906,15 @@
 
 
 _RequiredDevicePositionUpdateTypeDef = TypedDict(
     "_RequiredDevicePositionUpdateTypeDef",
     {
         "DeviceId": str,
         "Position": Sequence[float],
-        "SampleTime": Union[datetime, str],
+        "SampleTime": TimestampTypeDef,
     },
 )
 _OptionalDevicePositionUpdateTypeDef = TypedDict(
     "_OptionalDevicePositionUpdateTypeDef",
     {
         "Accuracy": PositionalAccuracyTypeDef,
         "PositionProperties": Mapping[str, str],
@@ -2027,15 +1934,15 @@
     {
         "Accuracy": PositionalAccuracyTypeDef,
         "DeviceId": str,
         "Position": List[float],
         "PositionProperties": Dict[str, str],
         "ReceivedTime": datetime,
         "SampleTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListDevicePositionsResponseEntryTypeDef = TypedDict(
     "_RequiredListDevicePositionsResponseEntryTypeDef",
     {
         "DeviceId": str,
@@ -2056,14 +1963,154 @@
 class ListDevicePositionsResponseEntryTypeDef(
     _RequiredListDevicePositionsResponseEntryTypeDef,
     _OptionalListDevicePositionsResponseEntryTypeDef,
 ):
     pass
 
 
+_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+    {
+        "DeviceId": str,
+        "TrackerName": str,
+    },
+)
+_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+    {
+        "EndTimeExclusive": TimestampTypeDef,
+        "StartTimeInclusive": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
+    _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    {
+        "TrackerName": str,
+    },
+)
+_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(
+    _RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+    _OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+):
+    pass
+
+
+ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = TypedDict(
+    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
+    "_RequiredListGeofencesRequestListGeofencesPaginateTypeDef",
+    {
+        "CollectionName": str,
+    },
+)
+_OptionalListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
+    "_OptionalListGeofencesRequestListGeofencesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGeofencesRequestListGeofencesPaginateTypeDef(
+    _RequiredListGeofencesRequestListGeofencesPaginateTypeDef,
+    _OptionalListGeofencesRequestListGeofencesPaginateTypeDef,
+):
+    pass
+
+
+ListKeysRequestListKeysPaginateTypeDef = TypedDict(
+    "ListKeysRequestListKeysPaginateTypeDef",
+    {
+        "Filter": ApiKeyFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMapsRequestListMapsPaginateTypeDef = TypedDict(
+    "ListMapsRequestListMapsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = TypedDict(
+    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = TypedDict(
+    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
+    "_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    {
+        "TrackerName": str,
+    },
+)
+_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
+    "_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(
+    _RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+    _OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+):
+    pass
+
+
+ListTrackersRequestListTrackersPaginateTypeDef = TypedDict(
+    "ListTrackersRequestListTrackersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredLegTypeDef = TypedDict(
     "_RequiredLegTypeDef",
     {
         "Distance": float,
         "DurationSeconds": float,
         "EndPosition": List[float],
         "StartPosition": List[float],
@@ -2084,51 +2131,51 @@
 
 
 ListGeofenceCollectionsResponseTypeDef = TypedDict(
     "ListGeofenceCollectionsResponseTypeDef",
     {
         "Entries": List[ListGeofenceCollectionsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMapsResponseTypeDef = TypedDict(
     "ListMapsResponseTypeDef",
     {
         "Entries": List[ListMapsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlaceIndexesResponseTypeDef = TypedDict(
     "ListPlaceIndexesResponseTypeDef",
     {
         "Entries": List[ListPlaceIndexesResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRouteCalculatorsResponseTypeDef = TypedDict(
     "ListRouteCalculatorsResponseTypeDef",
     {
         "Entries": List[ListRouteCalculatorsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrackersResponseTypeDef = TypedDict(
     "ListTrackersResponseTypeDef",
     {
         "Entries": List[ListTrackersResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateMapRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMapRequestRequestTypeDef",
     {
         "MapName": str,
@@ -2195,65 +2242,65 @@
 )
 
 SearchPlaceIndexForSuggestionsResponseTypeDef = TypedDict(
     "SearchPlaceIndexForSuggestionsResponseTypeDef",
     {
         "Results": List[SearchForSuggestionsResultTypeDef],
         "Summary": SearchPlaceIndexForSuggestionsSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKeysResponseTypeDef = TypedDict(
     "ListKeysResponseTypeDef",
     {
         "Entries": List[ListKeysResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteDevicePositionHistoryResponseTypeDef = TypedDict(
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     {
         "Errors": List[BatchDeleteDevicePositionHistoryErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteGeofenceResponseTypeDef = TypedDict(
     "BatchDeleteGeofenceResponseTypeDef",
     {
         "Errors": List[BatchDeleteGeofenceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEvaluateGeofencesResponseTypeDef = TypedDict(
     "BatchEvaluateGeofencesResponseTypeDef",
     {
         "Errors": List[BatchEvaluateGeofencesErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutGeofenceResponseTypeDef = TypedDict(
     "BatchPutGeofenceResponseTypeDef",
     {
         "Errors": List[BatchPutGeofenceErrorTypeDef],
         "Successes": List[BatchPutGeofenceSuccessTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateDevicePositionResponseTypeDef = TypedDict(
     "BatchUpdateDevicePositionResponseTypeDef",
     {
         "Errors": List[BatchUpdateDevicePositionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_RequiredCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CalculatorName": str,
@@ -2262,15 +2309,15 @@
     },
 )
 _OptionalCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_OptionalCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
-        "DepartureTime": Union[datetime, str],
+        "DepartureTime": TimestampTypeDef,
         "DistanceUnit": DistanceUnitType,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
     },
     total=False,
 )
 
@@ -2291,15 +2338,15 @@
     },
 )
 _OptionalCalculateRouteRequestRequestTypeDef = TypedDict(
     "_OptionalCalculateRouteRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
-        "DepartureTime": Union[datetime, str],
+        "DepartureTime": TimestampTypeDef,
         "DistanceUnit": DistanceUnitType,
         "IncludeLegGeometry": bool,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
         "WaypointPositions": Sequence[Sequence[float]],
     },
     total=False,
@@ -2308,55 +2355,33 @@
 
 class CalculateRouteRequestRequestTypeDef(
     _RequiredCalculateRouteRequestRequestTypeDef, _OptionalCalculateRouteRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
-    {
-        "GeofenceId": str,
-        "Geometry": GeofenceGeometryTypeDef,
-    },
-)
-_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
-    {
-        "GeofenceProperties": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class BatchPutGeofenceRequestEntryTypeDef(
-    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
-):
-    pass
-
-
 GetGeofenceResponseTypeDef = TypedDict(
     "GetGeofenceResponseTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
         "GeofenceProperties": Dict[str, str],
-        "Geometry": GeofenceGeometryTypeDef,
+        "Geometry": GeofenceGeometryOutputTypeDef,
         "Status": str,
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListGeofenceResponseEntryTypeDef = TypedDict(
     "_RequiredListGeofenceResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
-        "Geometry": GeofenceGeometryTypeDef,
+        "Geometry": GeofenceGeometryOutputTypeDef,
         "Status": str,
         "UpdateTime": datetime,
     },
 )
 _OptionalListGeofenceResponseEntryTypeDef = TypedDict(
     "_OptionalListGeofenceResponseEntryTypeDef",
     {
@@ -2368,14 +2393,37 @@
 
 class ListGeofenceResponseEntryTypeDef(
     _RequiredListGeofenceResponseEntryTypeDef, _OptionalListGeofenceResponseEntryTypeDef
 ):
     pass
 
 
+_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceId": str,
+        "Geometry": GeofenceGeometryTypeDef,
+    },
+)
+_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class BatchPutGeofenceRequestEntryTypeDef(
+    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
+):
+    pass
+
+
+GeofenceGeometryUnionTypeDef = Union[GeofenceGeometryTypeDef, GeofenceGeometryOutputTypeDef]
 _RequiredPutGeofenceRequestRequestTypeDef = TypedDict(
     "_RequiredPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
     },
@@ -2396,24 +2444,24 @@
 
 
 BatchGetDevicePositionResponseTypeDef = TypedDict(
     "BatchGetDevicePositionResponseTypeDef",
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "Errors": List[BatchGetDevicePositionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDevicePositionHistoryResponseTypeDef = TypedDict(
     "GetDevicePositionHistoryResponseTypeDef",
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEvaluateGeofencesRequestRequestTypeDef = TypedDict(
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
@@ -2430,32 +2478,32 @@
 )
 
 ListDevicePositionsResponseTypeDef = TypedDict(
     "ListDevicePositionsResponseTypeDef",
     {
         "Entries": List[ListDevicePositionsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CalculateRouteResponseTypeDef = TypedDict(
     "CalculateRouteResponseTypeDef",
     {
         "Legs": List[LegTypeDef],
         "Summary": CalculateRouteSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPlaceResponseTypeDef = TypedDict(
     "GetPlaceResponseTypeDef",
     {
         "Place": PlaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchForPositionResultTypeDef = TypedDict(
     "_RequiredSearchForPositionResultTypeDef",
     {
         "Distance": float,
@@ -2503,45 +2551,45 @@
 CalculateRouteMatrixResponseTypeDef = TypedDict(
     "CalculateRouteMatrixResponseTypeDef",
     {
         "RouteMatrix": List[List[RouteMatrixEntryTypeDef]],
         "SnappedDeparturePositions": List[List[float]],
         "SnappedDestinationPositions": List[List[float]],
         "Summary": CalculateRouteMatrixSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchPutGeofenceRequestRequestTypeDef = TypedDict(
-    "BatchPutGeofenceRequestRequestTypeDef",
-    {
-        "CollectionName": str,
-        "Entries": Sequence[BatchPutGeofenceRequestEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGeofencesResponseTypeDef = TypedDict(
     "ListGeofencesResponseTypeDef",
     {
         "Entries": List[ListGeofenceResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchPutGeofenceRequestRequestTypeDef = TypedDict(
+    "BatchPutGeofenceRequestRequestTypeDef",
+    {
+        "CollectionName": str,
+        "Entries": Sequence[BatchPutGeofenceRequestEntryTypeDef],
     },
 )
 
 SearchPlaceIndexForPositionResponseTypeDef = TypedDict(
     "SearchPlaceIndexForPositionResponseTypeDef",
     {
         "Results": List[SearchForPositionResultTypeDef],
         "Summary": SearchPlaceIndexForPositionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchPlaceIndexForTextResponseTypeDef = TypedDict(
     "SearchPlaceIndexForTextResponseTypeDef",
     {
         "Results": List[SearchForTextResultTypeDef],
         "Summary": SearchPlaceIndexForTextSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location/type_defs.pyi` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_location.type_defs import ApiKeyFilterTypeDef
 
-    data: ApiKeyFilterTypeDef = {...}
+    data: ApiKeyFilterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -33,142 +33,147 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApiKeyFilterTypeDef",
+    "ApiKeyRestrictionsOutputTypeDef",
     "ApiKeyRestrictionsTypeDef",
     "AssociateTrackerConsumerRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDeleteGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionRequestRequestTypeDef",
     "BatchPutGeofenceSuccessTypeDef",
     "CalculateRouteCarModeOptionsTypeDef",
+    "TimestampTypeDef",
     "CalculateRouteMatrixSummaryTypeDef",
     "CalculateRouteSummaryTypeDef",
     "TruckDimensionsTypeDef",
     "TruckWeightTypeDef",
+    "CircleOutputTypeDef",
     "CircleTypeDef",
     "CreateGeofenceCollectionRequestRequestTypeDef",
-    "CreateGeofenceCollectionResponseTypeDef",
-    "CreateKeyResponseTypeDef",
     "MapConfigurationTypeDef",
-    "CreateMapResponseTypeDef",
     "DataSourceConfigurationTypeDef",
-    "CreatePlaceIndexResponseTypeDef",
     "CreateRouteCalculatorRequestRequestTypeDef",
-    "CreateRouteCalculatorResponseTypeDef",
     "CreateTrackerRequestRequestTypeDef",
-    "CreateTrackerResponseTypeDef",
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     "DeleteKeyRequestRequestTypeDef",
     "DeleteMapRequestRequestTypeDef",
     "DeletePlaceIndexRequestRequestTypeDef",
     "DeleteRouteCalculatorRequestRequestTypeDef",
     "DeleteTrackerRequestRequestTypeDef",
     "DescribeGeofenceCollectionRequestRequestTypeDef",
-    "DescribeGeofenceCollectionResponseTypeDef",
     "DescribeKeyRequestRequestTypeDef",
     "DescribeMapRequestRequestTypeDef",
     "DescribePlaceIndexRequestRequestTypeDef",
     "DescribeRouteCalculatorRequestRequestTypeDef",
-    "DescribeRouteCalculatorResponseTypeDef",
     "DescribeTrackerRequestRequestTypeDef",
-    "DescribeTrackerResponseTypeDef",
     "PositionalAccuracyTypeDef",
     "DisassociateTrackerConsumerRequestRequestTypeDef",
-    "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    "GetDevicePositionHistoryRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "GetDevicePositionRequestRequestTypeDef",
     "GetGeofenceRequestRequestTypeDef",
     "GetMapGlyphsRequestRequestTypeDef",
-    "GetMapGlyphsResponseTypeDef",
     "GetMapSpritesRequestRequestTypeDef",
-    "GetMapSpritesResponseTypeDef",
     "GetMapStyleDescriptorRequestRequestTypeDef",
-    "GetMapStyleDescriptorResponseTypeDef",
     "GetMapTileRequestRequestTypeDef",
-    "GetMapTileResponseTypeDef",
     "GetPlaceRequestRequestTypeDef",
     "LegGeometryTypeDef",
     "StepTypeDef",
-    "ListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
     "ListDevicePositionsRequestRequestTypeDef",
-    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
     "ListGeofenceCollectionsRequestRequestTypeDef",
     "ListGeofenceCollectionsResponseEntryTypeDef",
-    "ListGeofencesRequestListGeofencesPaginateTypeDef",
     "ListGeofencesRequestRequestTypeDef",
-    "ListMapsRequestListMapsPaginateTypeDef",
     "ListMapsRequestRequestTypeDef",
     "ListMapsResponseEntryTypeDef",
-    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
     "ListPlaceIndexesRequestRequestTypeDef",
     "ListPlaceIndexesResponseEntryTypeDef",
-    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
     "ListRouteCalculatorsRequestRequestTypeDef",
     "ListRouteCalculatorsResponseEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
     "ListTrackerConsumersRequestRequestTypeDef",
-    "ListTrackerConsumersResponseTypeDef",
-    "ListTrackersRequestListTrackersPaginateTypeDef",
     "ListTrackersRequestRequestTypeDef",
     "ListTrackersResponseEntryTypeDef",
     "MapConfigurationUpdateTypeDef",
-    "PaginatorConfigTypeDef",
     "PlaceGeometryTypeDef",
     "TimeZoneTypeDef",
-    "PutGeofenceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RouteMatrixEntryErrorTypeDef",
     "SearchForSuggestionsResultTypeDef",
     "SearchPlaceIndexForPositionRequestRequestTypeDef",
     "SearchPlaceIndexForPositionSummaryTypeDef",
     "SearchPlaceIndexForSuggestionsRequestRequestTypeDef",
     "SearchPlaceIndexForSuggestionsSummaryTypeDef",
     "SearchPlaceIndexForTextRequestRequestTypeDef",
     "SearchPlaceIndexForTextSummaryTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGeofenceCollectionRequestRequestTypeDef",
-    "UpdateGeofenceCollectionResponseTypeDef",
-    "UpdateKeyResponseTypeDef",
-    "UpdateMapResponseTypeDef",
-    "UpdatePlaceIndexResponseTypeDef",
     "UpdateRouteCalculatorRequestRequestTypeDef",
-    "UpdateRouteCalculatorResponseTypeDef",
     "UpdateTrackerRequestRequestTypeDef",
-    "UpdateTrackerResponseTypeDef",
-    "ListKeysRequestListKeysPaginateTypeDef",
     "ListKeysRequestRequestTypeDef",
-    "CreateKeyRequestRequestTypeDef",
-    "DescribeKeyResponseTypeDef",
     "ListKeysResponseEntryTypeDef",
-    "UpdateKeyRequestRequestTypeDef",
+    "ApiKeyRestrictionsUnionTypeDef",
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     "BatchDeleteGeofenceErrorTypeDef",
     "BatchEvaluateGeofencesErrorTypeDef",
     "BatchGetDevicePositionErrorTypeDef",
     "BatchPutGeofenceErrorTypeDef",
     "BatchUpdateDevicePositionErrorTypeDef",
+    "CreateGeofenceCollectionResponseTypeDef",
+    "CreateKeyResponseTypeDef",
+    "CreateMapResponseTypeDef",
+    "CreatePlaceIndexResponseTypeDef",
+    "CreateRouteCalculatorResponseTypeDef",
+    "CreateTrackerResponseTypeDef",
+    "DescribeGeofenceCollectionResponseTypeDef",
+    "DescribeKeyResponseTypeDef",
+    "DescribeRouteCalculatorResponseTypeDef",
+    "DescribeTrackerResponseTypeDef",
+    "GetMapGlyphsResponseTypeDef",
+    "GetMapSpritesResponseTypeDef",
+    "GetMapStyleDescriptorResponseTypeDef",
+    "GetMapTileResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTrackerConsumersResponseTypeDef",
+    "PutGeofenceResponseTypeDef",
+    "UpdateGeofenceCollectionResponseTypeDef",
+    "UpdateKeyResponseTypeDef",
+    "UpdateMapResponseTypeDef",
+    "UpdatePlaceIndexResponseTypeDef",
+    "UpdateRouteCalculatorResponseTypeDef",
+    "UpdateTrackerResponseTypeDef",
+    "CreateKeyRequestRequestTypeDef",
+    "GetDevicePositionHistoryRequestRequestTypeDef",
+    "UpdateKeyRequestRequestTypeDef",
     "CalculateRouteTruckModeOptionsTypeDef",
+    "GeofenceGeometryOutputTypeDef",
     "GeofenceGeometryTypeDef",
     "CreateMapRequestRequestTypeDef",
     "DescribeMapResponseTypeDef",
     "CreatePlaceIndexRequestRequestTypeDef",
     "DescribePlaceIndexResponseTypeDef",
     "UpdatePlaceIndexRequestRequestTypeDef",
     "DevicePositionTypeDef",
     "DevicePositionUpdateTypeDef",
     "GetDevicePositionResponseTypeDef",
     "ListDevicePositionsResponseEntryTypeDef",
+    "GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+    "ListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
+    "ListGeofencesRequestListGeofencesPaginateTypeDef",
+    "ListKeysRequestListKeysPaginateTypeDef",
+    "ListMapsRequestListMapsPaginateTypeDef",
+    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
+    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
+    "ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    "ListTrackersRequestListTrackersPaginateTypeDef",
     "LegTypeDef",
     "ListGeofenceCollectionsResponseTypeDef",
     "ListMapsResponseTypeDef",
     "ListPlaceIndexesResponseTypeDef",
     "ListRouteCalculatorsResponseTypeDef",
     "ListTrackersResponseTypeDef",
     "UpdateMapRequestRequestTypeDef",
@@ -179,42 +184,63 @@
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     "BatchDeleteGeofenceResponseTypeDef",
     "BatchEvaluateGeofencesResponseTypeDef",
     "BatchPutGeofenceResponseTypeDef",
     "BatchUpdateDevicePositionResponseTypeDef",
     "CalculateRouteMatrixRequestRequestTypeDef",
     "CalculateRouteRequestRequestTypeDef",
-    "BatchPutGeofenceRequestEntryTypeDef",
     "GetGeofenceResponseTypeDef",
     "ListGeofenceResponseEntryTypeDef",
+    "BatchPutGeofenceRequestEntryTypeDef",
+    "GeofenceGeometryUnionTypeDef",
     "PutGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionResponseTypeDef",
     "GetDevicePositionHistoryResponseTypeDef",
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     "BatchUpdateDevicePositionRequestRequestTypeDef",
     "ListDevicePositionsResponseTypeDef",
     "CalculateRouteResponseTypeDef",
     "GetPlaceResponseTypeDef",
     "SearchForPositionResultTypeDef",
     "SearchForTextResultTypeDef",
     "CalculateRouteMatrixResponseTypeDef",
-    "BatchPutGeofenceRequestRequestTypeDef",
     "ListGeofencesResponseTypeDef",
+    "BatchPutGeofenceRequestRequestTypeDef",
     "SearchPlaceIndexForPositionResponseTypeDef",
     "SearchPlaceIndexForTextResponseTypeDef",
 )
 
 ApiKeyFilterTypeDef = TypedDict(
     "ApiKeyFilterTypeDef",
     {
         "KeyStatus": StatusType,
     },
     total=False,
 )
 
+_RequiredApiKeyRestrictionsOutputTypeDef = TypedDict(
+    "_RequiredApiKeyRestrictionsOutputTypeDef",
+    {
+        "AllowActions": List[str],
+        "AllowResources": List[str],
+    },
+)
+_OptionalApiKeyRestrictionsOutputTypeDef = TypedDict(
+    "_OptionalApiKeyRestrictionsOutputTypeDef",
+    {
+        "AllowReferers": List[str],
+    },
+    total=False,
+)
+
+class ApiKeyRestrictionsOutputTypeDef(
+    _RequiredApiKeyRestrictionsOutputTypeDef, _OptionalApiKeyRestrictionsOutputTypeDef
+):
+    pass
+
 _RequiredApiKeyRestrictionsTypeDef = TypedDict(
     "_RequiredApiKeyRestrictionsTypeDef",
     {
         "AllowActions": Sequence[str],
         "AllowResources": Sequence[str],
     },
 )
@@ -252,14 +278,25 @@
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
     {
         "DeviceIds": Sequence[str],
         "TrackerName": str,
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
 BatchDeleteGeofenceRequestRequestTypeDef = TypedDict(
     "BatchDeleteGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceIds": Sequence[str],
     },
 )
@@ -286,14 +323,15 @@
     {
         "AvoidFerries": bool,
         "AvoidTolls": bool,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 CalculateRouteMatrixSummaryTypeDef = TypedDict(
     "CalculateRouteMatrixSummaryTypeDef",
     {
         "DataSource": str,
         "DistanceUnit": DistanceUnitType,
         "ErrorCount": int,
         "RouteCount": int,
@@ -327,14 +365,22 @@
     {
         "Total": float,
         "Unit": VehicleWeightUnitType,
     },
     total=False,
 )
 
+CircleOutputTypeDef = TypedDict(
+    "CircleOutputTypeDef",
+    {
+        "Center": List[float],
+        "Radius": float,
+    },
+)
+
 CircleTypeDef = TypedDict(
     "CircleTypeDef",
     {
         "Center": Sequence[float],
         "Radius": float,
     },
 )
@@ -359,35 +405,14 @@
 
 class CreateGeofenceCollectionRequestRequestTypeDef(
     _RequiredCreateGeofenceCollectionRequestRequestTypeDef,
     _OptionalCreateGeofenceCollectionRequestRequestTypeDef,
 ):
     pass
 
-CreateGeofenceCollectionResponseTypeDef = TypedDict(
-    "CreateGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "CreateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateKeyResponseTypeDef = TypedDict(
-    "CreateKeyResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Key": str,
-        "KeyArn": str,
-        "KeyName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMapConfigurationTypeDef = TypedDict(
     "_RequiredMapConfigurationTypeDef",
     {
         "Style": str,
     },
 )
 _OptionalMapConfigurationTypeDef = TypedDict(
@@ -397,42 +422,22 @@
     },
     total=False,
 )
 
 class MapConfigurationTypeDef(_RequiredMapConfigurationTypeDef, _OptionalMapConfigurationTypeDef):
     pass
 
-CreateMapResponseTypeDef = TypedDict(
-    "CreateMapResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "MapArn": str,
-        "MapName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DataSourceConfigurationTypeDef = TypedDict(
     "DataSourceConfigurationTypeDef",
     {
         "IntendedUse": IntendedUseType,
     },
     total=False,
 )
 
-CreatePlaceIndexResponseTypeDef = TypedDict(
-    "CreatePlaceIndexResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "IndexArn": str,
-        "IndexName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateRouteCalculatorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
         "DataSource": str,
     },
 )
@@ -448,24 +453,14 @@
 
 class CreateRouteCalculatorRequestRequestTypeDef(
     _RequiredCreateRouteCalculatorRequestRequestTypeDef,
     _OptionalCreateRouteCalculatorRequestRequestTypeDef,
 ):
     pass
 
-CreateRouteCalculatorResponseTypeDef = TypedDict(
-    "CreateRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "CreateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalCreateTrackerRequestRequestTypeDef = TypedDict(
@@ -482,24 +477,14 @@
 )
 
 class CreateTrackerRequestRequestTypeDef(
     _RequiredCreateTrackerRequestRequestTypeDef, _OptionalCreateTrackerRequestRequestTypeDef
 ):
     pass
 
-CreateTrackerResponseTypeDef = TypedDict(
-    "CreateTrackerResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "TrackerArn": str,
-        "TrackerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DeleteGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
@@ -541,30 +526,14 @@
 DescribeGeofenceCollectionRequestRequestTypeDef = TypedDict(
     "DescribeGeofenceCollectionRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 
-DescribeGeofenceCollectionResponseTypeDef = TypedDict(
-    "DescribeGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "CreateTime": datetime,
-        "Description": str,
-        "KmsKeyId": str,
-        "PricingPlan": PricingPlanType,
-        "PricingPlanDataSource": str,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeKeyRequestRequestTypeDef = TypedDict(
     "DescribeKeyRequestRequestTypeDef",
     {
         "KeyName": str,
     },
 )
 
@@ -585,53 +554,21 @@
 DescribeRouteCalculatorRequestRequestTypeDef = TypedDict(
     "DescribeRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
     },
 )
 
-DescribeRouteCalculatorResponseTypeDef = TypedDict(
-    "DescribeRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "CreateTime": datetime,
-        "DataSource": str,
-        "Description": str,
-        "PricingPlan": PricingPlanType,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeTrackerRequestRequestTypeDef = TypedDict(
     "DescribeTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 
-DescribeTrackerResponseTypeDef = TypedDict(
-    "DescribeTrackerResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Description": str,
-        "KmsKeyId": str,
-        "PositionFiltering": PositionFilteringType,
-        "PricingPlan": PricingPlanType,
-        "PricingPlanDataSource": str,
-        "Tags": Dict[str, str],
-        "TrackerArn": str,
-        "TrackerName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PositionalAccuracyTypeDef = TypedDict(
     "PositionalAccuracyTypeDef",
     {
         "Horizontal": float,
     },
 )
 
@@ -639,61 +576,24 @@
     "DisassociateTrackerConsumerRequestRequestTypeDef",
     {
         "ConsumerArn": str,
         "TrackerName": str,
     },
 )
 
-_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "TrackerName": str,
-    },
-)
-_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
-    {
-        "EndTimeExclusive": Union[datetime, str],
-        "StartTimeInclusive": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
-    _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-    _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-):
-    pass
-
-_RequiredGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredGetDevicePositionHistoryRequestRequestTypeDef",
-    {
-        "DeviceId": str,
-        "TrackerName": str,
-    },
-)
-_OptionalGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalGetDevicePositionHistoryRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "EndTimeExclusive": Union[datetime, str],
-        "MaxResults": int,
-        "NextToken": str,
-        "StartTimeInclusive": Union[datetime, str],
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetDevicePositionHistoryRequestRequestTypeDef(
-    _RequiredGetDevicePositionHistoryRequestRequestTypeDef,
-    _OptionalGetDevicePositionHistoryRequestRequestTypeDef,
-):
-    pass
-
 GetDevicePositionRequestRequestTypeDef = TypedDict(
     "GetDevicePositionRequestRequestTypeDef",
     {
         "DeviceId": str,
         "TrackerName": str,
     },
 )
@@ -723,24 +623,14 @@
 )
 
 class GetMapGlyphsRequestRequestTypeDef(
     _RequiredGetMapGlyphsRequestRequestTypeDef, _OptionalGetMapGlyphsRequestRequestTypeDef
 ):
     pass
 
-GetMapGlyphsResponseTypeDef = TypedDict(
-    "GetMapGlyphsResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMapSpritesRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapSpritesRequestRequestTypeDef",
     {
         "FileName": str,
         "MapName": str,
     },
 )
@@ -753,24 +643,14 @@
 )
 
 class GetMapSpritesRequestRequestTypeDef(
     _RequiredGetMapSpritesRequestRequestTypeDef, _OptionalGetMapSpritesRequestRequestTypeDef
 ):
     pass
 
-GetMapSpritesResponseTypeDef = TypedDict(
-    "GetMapSpritesResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMapStyleDescriptorRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapStyleDescriptorRequestRequestTypeDef",
     {
         "MapName": str,
     },
 )
 _OptionalGetMapStyleDescriptorRequestRequestTypeDef = TypedDict(
@@ -783,24 +663,14 @@
 
 class GetMapStyleDescriptorRequestRequestTypeDef(
     _RequiredGetMapStyleDescriptorRequestRequestTypeDef,
     _OptionalGetMapStyleDescriptorRequestRequestTypeDef,
 ):
     pass
 
-GetMapStyleDescriptorResponseTypeDef = TypedDict(
-    "GetMapStyleDescriptorResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetMapTileRequestRequestTypeDef = TypedDict(
     "_RequiredGetMapTileRequestRequestTypeDef",
     {
         "MapName": str,
         "X": str,
         "Y": str,
         "Z": str,
@@ -815,24 +685,14 @@
 )
 
 class GetMapTileRequestRequestTypeDef(
     _RequiredGetMapTileRequestRequestTypeDef, _OptionalGetMapTileRequestRequestTypeDef
 ):
     pass
 
-GetMapTileResponseTypeDef = TypedDict(
-    "GetMapTileResponseTypeDef",
-    {
-        "Blob": StreamingBody,
-        "CacheControl": str,
-        "ContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPlaceRequestRequestTypeDef = TypedDict(
     "_RequiredGetPlaceRequestRequestTypeDef",
     {
         "IndexName": str,
         "PlaceId": str,
     },
 )
@@ -873,34 +733,14 @@
     },
     total=False,
 )
 
 class StepTypeDef(_RequiredStepTypeDef, _OptionalStepTypeDef):
     pass
 
-_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
-    "_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    {
-        "TrackerName": str,
-    },
-)
-_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
-    "_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(
-    _RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-    _OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDevicePositionsRequestRequestTypeDef = TypedDict(
     "_RequiredListDevicePositionsRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalListDevicePositionsRequestRequestTypeDef = TypedDict(
@@ -914,22 +754,14 @@
 
 class ListDevicePositionsRequestRequestTypeDef(
     _RequiredListDevicePositionsRequestRequestTypeDef,
     _OptionalListDevicePositionsRequestRequestTypeDef,
 ):
     pass
 
-ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = TypedDict(
-    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGeofenceCollectionsRequestRequestTypeDef = TypedDict(
     "ListGeofenceCollectionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -955,34 +787,14 @@
 
 class ListGeofenceCollectionsResponseEntryTypeDef(
     _RequiredListGeofenceCollectionsResponseEntryTypeDef,
     _OptionalListGeofenceCollectionsResponseEntryTypeDef,
 ):
     pass
 
-_RequiredListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
-    "_RequiredListGeofencesRequestListGeofencesPaginateTypeDef",
-    {
-        "CollectionName": str,
-    },
-)
-_OptionalListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
-    "_OptionalListGeofencesRequestListGeofencesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGeofencesRequestListGeofencesPaginateTypeDef(
-    _RequiredListGeofencesRequestListGeofencesPaginateTypeDef,
-    _OptionalListGeofencesRequestListGeofencesPaginateTypeDef,
-):
-    pass
-
 _RequiredListGeofencesRequestRequestTypeDef = TypedDict(
     "_RequiredListGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
     },
 )
 _OptionalListGeofencesRequestRequestTypeDef = TypedDict(
@@ -995,22 +807,14 @@
 )
 
 class ListGeofencesRequestRequestTypeDef(
     _RequiredListGeofencesRequestRequestTypeDef, _OptionalListGeofencesRequestRequestTypeDef
 ):
     pass
 
-ListMapsRequestListMapsPaginateTypeDef = TypedDict(
-    "ListMapsRequestListMapsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMapsRequestRequestTypeDef = TypedDict(
     "ListMapsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1035,22 +839,14 @@
 )
 
 class ListMapsResponseEntryTypeDef(
     _RequiredListMapsResponseEntryTypeDef, _OptionalListMapsResponseEntryTypeDef
 ):
     pass
 
-ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = TypedDict(
-    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPlaceIndexesRequestRequestTypeDef = TypedDict(
     "ListPlaceIndexesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1075,22 +871,14 @@
 )
 
 class ListPlaceIndexesResponseEntryTypeDef(
     _RequiredListPlaceIndexesResponseEntryTypeDef, _OptionalListPlaceIndexesResponseEntryTypeDef
 ):
     pass
 
-ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = TypedDict(
-    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRouteCalculatorsRequestRequestTypeDef = TypedDict(
     "ListRouteCalculatorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1123,42 +911,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
-    "_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    {
-        "TrackerName": str,
-    },
-)
-_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
-    "_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(
-    _RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-    _OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
-):
-    pass
-
 _RequiredListTrackerConsumersRequestRequestTypeDef = TypedDict(
     "_RequiredListTrackerConsumersRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalListTrackerConsumersRequestRequestTypeDef = TypedDict(
@@ -1172,31 +932,14 @@
 
 class ListTrackerConsumersRequestRequestTypeDef(
     _RequiredListTrackerConsumersRequestRequestTypeDef,
     _OptionalListTrackerConsumersRequestRequestTypeDef,
 ):
     pass
 
-ListTrackerConsumersResponseTypeDef = TypedDict(
-    "ListTrackerConsumersResponseTypeDef",
-    {
-        "ConsumerArns": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTrackersRequestListTrackersPaginateTypeDef = TypedDict(
-    "ListTrackersRequestListTrackersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTrackersRequestRequestTypeDef = TypedDict(
     "ListTrackersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1229,24 +972,14 @@
     "MapConfigurationUpdateTypeDef",
     {
         "PoliticalView": str,
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
 PlaceGeometryTypeDef = TypedDict(
     "PlaceGeometryTypeDef",
     {
         "Point": List[float],
     },
     total=False,
 )
@@ -1264,35 +997,14 @@
     },
     total=False,
 )
 
 class TimeZoneTypeDef(_RequiredTimeZoneTypeDef, _OptionalTimeZoneTypeDef):
     pass
 
-PutGeofenceResponseTypeDef = TypedDict(
-    "PutGeofenceResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "GeofenceId": str,
-        "UpdateTime": datetime,
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
 _RequiredRouteMatrixEntryErrorTypeDef = TypedDict(
     "_RequiredRouteMatrixEntryErrorTypeDef",
     {
         "Code": RouteMatrixErrorCodeType,
     },
 )
 _OptionalRouteMatrixEntryErrorTypeDef = TypedDict(
@@ -1511,54 +1223,14 @@
 
 class UpdateGeofenceCollectionRequestRequestTypeDef(
     _RequiredUpdateGeofenceCollectionRequestRequestTypeDef,
     _OptionalUpdateGeofenceCollectionRequestRequestTypeDef,
 ):
     pass
 
-UpdateGeofenceCollectionResponseTypeDef = TypedDict(
-    "UpdateGeofenceCollectionResponseTypeDef",
-    {
-        "CollectionArn": str,
-        "CollectionName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateKeyResponseTypeDef = TypedDict(
-    "UpdateKeyResponseTypeDef",
-    {
-        "KeyArn": str,
-        "KeyName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateMapResponseTypeDef = TypedDict(
-    "UpdateMapResponseTypeDef",
-    {
-        "MapArn": str,
-        "MapName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdatePlaceIndexResponseTypeDef = TypedDict(
-    "UpdatePlaceIndexResponseTypeDef",
-    {
-        "IndexArn": str,
-        "IndexName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateRouteCalculatorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteCalculatorRequestRequestTypeDef",
     {
         "CalculatorName": str,
     },
 )
 _OptionalUpdateRouteCalculatorRequestRequestTypeDef = TypedDict(
@@ -1572,24 +1244,14 @@
 
 class UpdateRouteCalculatorRequestRequestTypeDef(
     _RequiredUpdateRouteCalculatorRequestRequestTypeDef,
     _OptionalUpdateRouteCalculatorRequestRequestTypeDef,
 ):
     pass
 
-UpdateRouteCalculatorResponseTypeDef = TypedDict(
-    "UpdateRouteCalculatorResponseTypeDef",
-    {
-        "CalculatorArn": str,
-        "CalculatorName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateTrackerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTrackerRequestRequestTypeDef",
     {
         "TrackerName": str,
     },
 )
 _OptionalUpdateTrackerRequestRequestTypeDef = TypedDict(
@@ -1604,89 +1266,31 @@
 )
 
 class UpdateTrackerRequestRequestTypeDef(
     _RequiredUpdateTrackerRequestRequestTypeDef, _OptionalUpdateTrackerRequestRequestTypeDef
 ):
     pass
 
-UpdateTrackerResponseTypeDef = TypedDict(
-    "UpdateTrackerResponseTypeDef",
-    {
-        "TrackerArn": str,
-        "TrackerName": str,
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListKeysRequestListKeysPaginateTypeDef = TypedDict(
-    "ListKeysRequestListKeysPaginateTypeDef",
-    {
-        "Filter": ApiKeyFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListKeysRequestRequestTypeDef = TypedDict(
     "ListKeysRequestRequestTypeDef",
     {
         "Filter": ApiKeyFilterTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredCreateKeyRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyRequestRequestTypeDef",
-    {
-        "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
-    },
-)
-_OptionalCreateKeyRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ExpireTime": Union[datetime, str],
-        "NoExpiry": bool,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateKeyRequestRequestTypeDef(
-    _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
-):
-    pass
-
-DescribeKeyResponseTypeDef = TypedDict(
-    "DescribeKeyResponseTypeDef",
-    {
-        "CreateTime": datetime,
-        "Description": str,
-        "ExpireTime": datetime,
-        "Key": str,
-        "KeyArn": str,
-        "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
-        "Tags": Dict[str, str],
-        "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListKeysResponseEntryTypeDef = TypedDict(
     "_RequiredListKeysResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "ExpireTime": datetime,
         "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
+        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
         "UpdateTime": datetime,
     },
 )
 _OptionalListKeysResponseEntryTypeDef = TypedDict(
     "_OptionalListKeysResponseEntryTypeDef",
     {
         "Description": str,
@@ -1695,37 +1299,15 @@
 )
 
 class ListKeysResponseEntryTypeDef(
     _RequiredListKeysResponseEntryTypeDef, _OptionalListKeysResponseEntryTypeDef
 ):
     pass
 
-_RequiredUpdateKeyRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateKeyRequestRequestTypeDef",
-    {
-        "KeyName": str,
-    },
-)
-_OptionalUpdateKeyRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateKeyRequestRequestTypeDef",
-    {
-        "Description": str,
-        "ExpireTime": Union[datetime, str],
-        "ForceUpdate": bool,
-        "NoExpiry": bool,
-        "Restrictions": ApiKeyRestrictionsTypeDef,
-    },
-    total=False,
-)
-
-class UpdateKeyRequestRequestTypeDef(
-    _RequiredUpdateKeyRequestRequestTypeDef, _OptionalUpdateKeyRequestRequestTypeDef
-):
-    pass
-
+ApiKeyRestrictionsUnionTypeDef = Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef]
 BatchDeleteDevicePositionHistoryErrorTypeDef = TypedDict(
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     {
         "DeviceId": str,
         "Error": BatchItemErrorTypeDef,
     },
 )
@@ -1768,25 +1350,356 @@
     {
         "DeviceId": str,
         "Error": BatchItemErrorTypeDef,
         "SampleTime": datetime,
     },
 )
 
+CreateGeofenceCollectionResponseTypeDef = TypedDict(
+    "CreateGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "CreateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKeyResponseTypeDef = TypedDict(
+    "CreateKeyResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Key": str,
+        "KeyArn": str,
+        "KeyName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMapResponseTypeDef = TypedDict(
+    "CreateMapResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "MapArn": str,
+        "MapName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePlaceIndexResponseTypeDef = TypedDict(
+    "CreatePlaceIndexResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "IndexArn": str,
+        "IndexName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRouteCalculatorResponseTypeDef = TypedDict(
+    "CreateRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "CreateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTrackerResponseTypeDef = TypedDict(
+    "CreateTrackerResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "TrackerArn": str,
+        "TrackerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeGeofenceCollectionResponseTypeDef = TypedDict(
+    "DescribeGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "CreateTime": datetime,
+        "Description": str,
+        "KmsKeyId": str,
+        "PricingPlan": PricingPlanType,
+        "PricingPlanDataSource": str,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeKeyResponseTypeDef = TypedDict(
+    "DescribeKeyResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Description": str,
+        "ExpireTime": datetime,
+        "Key": str,
+        "KeyArn": str,
+        "KeyName": str,
+        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRouteCalculatorResponseTypeDef = TypedDict(
+    "DescribeRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "CreateTime": datetime,
+        "DataSource": str,
+        "Description": str,
+        "PricingPlan": PricingPlanType,
+        "Tags": Dict[str, str],
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTrackerResponseTypeDef = TypedDict(
+    "DescribeTrackerResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "Description": str,
+        "KmsKeyId": str,
+        "PositionFiltering": PositionFilteringType,
+        "PricingPlan": PricingPlanType,
+        "PricingPlanDataSource": str,
+        "Tags": Dict[str, str],
+        "TrackerArn": str,
+        "TrackerName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMapGlyphsResponseTypeDef = TypedDict(
+    "GetMapGlyphsResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMapSpritesResponseTypeDef = TypedDict(
+    "GetMapSpritesResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMapStyleDescriptorResponseTypeDef = TypedDict(
+    "GetMapStyleDescriptorResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMapTileResponseTypeDef = TypedDict(
+    "GetMapTileResponseTypeDef",
+    {
+        "Blob": StreamingBody,
+        "CacheControl": str,
+        "ContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTrackerConsumersResponseTypeDef = TypedDict(
+    "ListTrackerConsumersResponseTypeDef",
+    {
+        "ConsumerArns": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutGeofenceResponseTypeDef = TypedDict(
+    "PutGeofenceResponseTypeDef",
+    {
+        "CreateTime": datetime,
+        "GeofenceId": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateGeofenceCollectionResponseTypeDef = TypedDict(
+    "UpdateGeofenceCollectionResponseTypeDef",
+    {
+        "CollectionArn": str,
+        "CollectionName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateKeyResponseTypeDef = TypedDict(
+    "UpdateKeyResponseTypeDef",
+    {
+        "KeyArn": str,
+        "KeyName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMapResponseTypeDef = TypedDict(
+    "UpdateMapResponseTypeDef",
+    {
+        "MapArn": str,
+        "MapName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePlaceIndexResponseTypeDef = TypedDict(
+    "UpdatePlaceIndexResponseTypeDef",
+    {
+        "IndexArn": str,
+        "IndexName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRouteCalculatorResponseTypeDef = TypedDict(
+    "UpdateRouteCalculatorResponseTypeDef",
+    {
+        "CalculatorArn": str,
+        "CalculatorName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTrackerResponseTypeDef = TypedDict(
+    "UpdateTrackerResponseTypeDef",
+    {
+        "TrackerArn": str,
+        "TrackerName": str,
+        "UpdateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyRequestRequestTypeDef",
+    {
+        "KeyName": str,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
+    },
+)
+_OptionalCreateKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ExpireTime": TimestampTypeDef,
+        "NoExpiry": bool,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateKeyRequestRequestTypeDef(
+    _RequiredCreateKeyRequestRequestTypeDef, _OptionalCreateKeyRequestRequestTypeDef
+):
+    pass
+
+_RequiredGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetDevicePositionHistoryRequestRequestTypeDef",
+    {
+        "DeviceId": str,
+        "TrackerName": str,
+    },
+)
+_OptionalGetDevicePositionHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetDevicePositionHistoryRequestRequestTypeDef",
+    {
+        "EndTimeExclusive": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "StartTimeInclusive": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class GetDevicePositionHistoryRequestRequestTypeDef(
+    _RequiredGetDevicePositionHistoryRequestRequestTypeDef,
+    _OptionalGetDevicePositionHistoryRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateKeyRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateKeyRequestRequestTypeDef",
+    {
+        "KeyName": str,
+    },
+)
+_OptionalUpdateKeyRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateKeyRequestRequestTypeDef",
+    {
+        "Description": str,
+        "ExpireTime": TimestampTypeDef,
+        "ForceUpdate": bool,
+        "NoExpiry": bool,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
+    },
+    total=False,
+)
+
+class UpdateKeyRequestRequestTypeDef(
+    _RequiredUpdateKeyRequestRequestTypeDef, _OptionalUpdateKeyRequestRequestTypeDef
+):
+    pass
+
 CalculateRouteTruckModeOptionsTypeDef = TypedDict(
     "CalculateRouteTruckModeOptionsTypeDef",
     {
         "AvoidFerries": bool,
         "AvoidTolls": bool,
         "Dimensions": TruckDimensionsTypeDef,
         "Weight": TruckWeightTypeDef,
     },
     total=False,
 )
 
+GeofenceGeometryOutputTypeDef = TypedDict(
+    "GeofenceGeometryOutputTypeDef",
+    {
+        "Circle": CircleOutputTypeDef,
+        "Polygon": List[List[List[float]]],
+    },
+    total=False,
+)
+
 GeofenceGeometryTypeDef = TypedDict(
     "GeofenceGeometryTypeDef",
     {
         "Circle": CircleTypeDef,
         "Polygon": Sequence[Sequence[Sequence[float]]],
     },
     total=False,
@@ -1822,15 +1735,15 @@
         "DataSource": str,
         "Description": str,
         "MapArn": str,
         "MapName": str,
         "PricingPlan": PricingPlanType,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlaceIndexRequestRequestTypeDef",
     {
         "DataSource": str,
@@ -1861,15 +1774,15 @@
         "DataSourceConfiguration": DataSourceConfigurationTypeDef,
         "Description": str,
         "IndexArn": str,
         "IndexName": str,
         "PricingPlan": PricingPlanType,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdatePlaceIndexRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePlaceIndexRequestRequestTypeDef",
     {
         "IndexName": str,
@@ -1912,15 +1825,15 @@
     pass
 
 _RequiredDevicePositionUpdateTypeDef = TypedDict(
     "_RequiredDevicePositionUpdateTypeDef",
     {
         "DeviceId": str,
         "Position": Sequence[float],
-        "SampleTime": Union[datetime, str],
+        "SampleTime": TimestampTypeDef,
     },
 )
 _OptionalDevicePositionUpdateTypeDef = TypedDict(
     "_OptionalDevicePositionUpdateTypeDef",
     {
         "Accuracy": PositionalAccuracyTypeDef,
         "PositionProperties": Mapping[str, str],
@@ -1938,15 +1851,15 @@
     {
         "Accuracy": PositionalAccuracyTypeDef,
         "DeviceId": str,
         "Position": List[float],
         "PositionProperties": Dict[str, str],
         "ReceivedTime": datetime,
         "SampleTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListDevicePositionsResponseEntryTypeDef = TypedDict(
     "_RequiredListDevicePositionsResponseEntryTypeDef",
     {
         "DeviceId": str,
@@ -1965,14 +1878,146 @@
 
 class ListDevicePositionsResponseEntryTypeDef(
     _RequiredListDevicePositionsResponseEntryTypeDef,
     _OptionalListDevicePositionsResponseEntryTypeDef,
 ):
     pass
 
+_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+    {
+        "DeviceId": str,
+        "TrackerName": str,
+    },
+)
+_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef",
+    {
+        "EndTimeExclusive": TimestampTypeDef,
+        "StartTimeInclusive": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef(
+    _RequiredGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    _OptionalGetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+):
+    pass
+
+_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
+    "_RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    {
+        "TrackerName": str,
+    },
+)
+_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef = TypedDict(
+    "_OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDevicePositionsRequestListDevicePositionsPaginateTypeDef(
+    _RequiredListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+    _OptionalListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+):
+    pass
+
+ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef = TypedDict(
+    "ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
+    "_RequiredListGeofencesRequestListGeofencesPaginateTypeDef",
+    {
+        "CollectionName": str,
+    },
+)
+_OptionalListGeofencesRequestListGeofencesPaginateTypeDef = TypedDict(
+    "_OptionalListGeofencesRequestListGeofencesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGeofencesRequestListGeofencesPaginateTypeDef(
+    _RequiredListGeofencesRequestListGeofencesPaginateTypeDef,
+    _OptionalListGeofencesRequestListGeofencesPaginateTypeDef,
+):
+    pass
+
+ListKeysRequestListKeysPaginateTypeDef = TypedDict(
+    "ListKeysRequestListKeysPaginateTypeDef",
+    {
+        "Filter": ApiKeyFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMapsRequestListMapsPaginateTypeDef = TypedDict(
+    "ListMapsRequestListMapsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef = TypedDict(
+    "ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef = TypedDict(
+    "ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
+    "_RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    {
+        "TrackerName": str,
+    },
+)
+_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef = TypedDict(
+    "_OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef(
+    _RequiredListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+    _OptionalListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+):
+    pass
+
+ListTrackersRequestListTrackersPaginateTypeDef = TypedDict(
+    "ListTrackersRequestListTrackersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredLegTypeDef = TypedDict(
     "_RequiredLegTypeDef",
     {
         "Distance": float,
         "DurationSeconds": float,
         "EndPosition": List[float],
         "StartPosition": List[float],
@@ -1991,51 +2036,51 @@
     pass
 
 ListGeofenceCollectionsResponseTypeDef = TypedDict(
     "ListGeofenceCollectionsResponseTypeDef",
     {
         "Entries": List[ListGeofenceCollectionsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMapsResponseTypeDef = TypedDict(
     "ListMapsResponseTypeDef",
     {
         "Entries": List[ListMapsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlaceIndexesResponseTypeDef = TypedDict(
     "ListPlaceIndexesResponseTypeDef",
     {
         "Entries": List[ListPlaceIndexesResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRouteCalculatorsResponseTypeDef = TypedDict(
     "ListRouteCalculatorsResponseTypeDef",
     {
         "Entries": List[ListRouteCalculatorsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrackersResponseTypeDef = TypedDict(
     "ListTrackersResponseTypeDef",
     {
         "Entries": List[ListTrackersResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateMapRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMapRequestRequestTypeDef",
     {
         "MapName": str,
@@ -2098,65 +2143,65 @@
 )
 
 SearchPlaceIndexForSuggestionsResponseTypeDef = TypedDict(
     "SearchPlaceIndexForSuggestionsResponseTypeDef",
     {
         "Results": List[SearchForSuggestionsResultTypeDef],
         "Summary": SearchPlaceIndexForSuggestionsSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKeysResponseTypeDef = TypedDict(
     "ListKeysResponseTypeDef",
     {
         "Entries": List[ListKeysResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteDevicePositionHistoryResponseTypeDef = TypedDict(
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     {
         "Errors": List[BatchDeleteDevicePositionHistoryErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteGeofenceResponseTypeDef = TypedDict(
     "BatchDeleteGeofenceResponseTypeDef",
     {
         "Errors": List[BatchDeleteGeofenceErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEvaluateGeofencesResponseTypeDef = TypedDict(
     "BatchEvaluateGeofencesResponseTypeDef",
     {
         "Errors": List[BatchEvaluateGeofencesErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutGeofenceResponseTypeDef = TypedDict(
     "BatchPutGeofenceResponseTypeDef",
     {
         "Errors": List[BatchPutGeofenceErrorTypeDef],
         "Successes": List[BatchPutGeofenceSuccessTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateDevicePositionResponseTypeDef = TypedDict(
     "BatchUpdateDevicePositionResponseTypeDef",
     {
         "Errors": List[BatchUpdateDevicePositionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_RequiredCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CalculatorName": str,
@@ -2165,15 +2210,15 @@
     },
 )
 _OptionalCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_OptionalCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
-        "DepartureTime": Union[datetime, str],
+        "DepartureTime": TimestampTypeDef,
         "DistanceUnit": DistanceUnitType,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
     },
     total=False,
 )
 
@@ -2192,68 +2237,48 @@
     },
 )
 _OptionalCalculateRouteRequestRequestTypeDef = TypedDict(
     "_OptionalCalculateRouteRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
-        "DepartureTime": Union[datetime, str],
+        "DepartureTime": TimestampTypeDef,
         "DistanceUnit": DistanceUnitType,
         "IncludeLegGeometry": bool,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
         "WaypointPositions": Sequence[Sequence[float]],
     },
     total=False,
 )
 
 class CalculateRouteRequestRequestTypeDef(
     _RequiredCalculateRouteRequestRequestTypeDef, _OptionalCalculateRouteRequestRequestTypeDef
 ):
     pass
 
-_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
-    {
-        "GeofenceId": str,
-        "Geometry": GeofenceGeometryTypeDef,
-    },
-)
-_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
-    {
-        "GeofenceProperties": Mapping[str, str],
-    },
-    total=False,
-)
-
-class BatchPutGeofenceRequestEntryTypeDef(
-    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
-):
-    pass
-
 GetGeofenceResponseTypeDef = TypedDict(
     "GetGeofenceResponseTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
         "GeofenceProperties": Dict[str, str],
-        "Geometry": GeofenceGeometryTypeDef,
+        "Geometry": GeofenceGeometryOutputTypeDef,
         "Status": str,
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListGeofenceResponseEntryTypeDef = TypedDict(
     "_RequiredListGeofenceResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
-        "Geometry": GeofenceGeometryTypeDef,
+        "Geometry": GeofenceGeometryOutputTypeDef,
         "Status": str,
         "UpdateTime": datetime,
     },
 )
 _OptionalListGeofenceResponseEntryTypeDef = TypedDict(
     "_OptionalListGeofenceResponseEntryTypeDef",
     {
@@ -2263,14 +2288,35 @@
 )
 
 class ListGeofenceResponseEntryTypeDef(
     _RequiredListGeofenceResponseEntryTypeDef, _OptionalListGeofenceResponseEntryTypeDef
 ):
     pass
 
+_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceId": str,
+        "Geometry": GeofenceGeometryTypeDef,
+    },
+)
+_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+class BatchPutGeofenceRequestEntryTypeDef(
+    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
+):
+    pass
+
+GeofenceGeometryUnionTypeDef = Union[GeofenceGeometryTypeDef, GeofenceGeometryOutputTypeDef]
 _RequiredPutGeofenceRequestRequestTypeDef = TypedDict(
     "_RequiredPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
     },
@@ -2289,24 +2335,24 @@
     pass
 
 BatchGetDevicePositionResponseTypeDef = TypedDict(
     "BatchGetDevicePositionResponseTypeDef",
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "Errors": List[BatchGetDevicePositionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDevicePositionHistoryResponseTypeDef = TypedDict(
     "GetDevicePositionHistoryResponseTypeDef",
     {
         "DevicePositions": List[DevicePositionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchEvaluateGeofencesRequestRequestTypeDef = TypedDict(
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     {
         "CollectionName": str,
@@ -2323,32 +2369,32 @@
 )
 
 ListDevicePositionsResponseTypeDef = TypedDict(
     "ListDevicePositionsResponseTypeDef",
     {
         "Entries": List[ListDevicePositionsResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CalculateRouteResponseTypeDef = TypedDict(
     "CalculateRouteResponseTypeDef",
     {
         "Legs": List[LegTypeDef],
         "Summary": CalculateRouteSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPlaceResponseTypeDef = TypedDict(
     "GetPlaceResponseTypeDef",
     {
         "Place": PlaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchForPositionResultTypeDef = TypedDict(
     "_RequiredSearchForPositionResultTypeDef",
     {
         "Distance": float,
@@ -2392,45 +2438,45 @@
 CalculateRouteMatrixResponseTypeDef = TypedDict(
     "CalculateRouteMatrixResponseTypeDef",
     {
         "RouteMatrix": List[List[RouteMatrixEntryTypeDef]],
         "SnappedDeparturePositions": List[List[float]],
         "SnappedDestinationPositions": List[List[float]],
         "Summary": CalculateRouteMatrixSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchPutGeofenceRequestRequestTypeDef = TypedDict(
-    "BatchPutGeofenceRequestRequestTypeDef",
-    {
-        "CollectionName": str,
-        "Entries": Sequence[BatchPutGeofenceRequestEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGeofencesResponseTypeDef = TypedDict(
     "ListGeofencesResponseTypeDef",
     {
         "Entries": List[ListGeofenceResponseEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchPutGeofenceRequestRequestTypeDef = TypedDict(
+    "BatchPutGeofenceRequestRequestTypeDef",
+    {
+        "CollectionName": str,
+        "Entries": Sequence[BatchPutGeofenceRequestEntryTypeDef],
     },
 )
 
 SearchPlaceIndexForPositionResponseTypeDef = TypedDict(
     "SearchPlaceIndexForPositionResponseTypeDef",
     {
         "Results": List[SearchForPositionResultTypeDef],
         "Summary": SearchPlaceIndexForPositionSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchPlaceIndexForTextResponseTypeDef = TypedDict(
     "SearchPlaceIndexForTextResponseTypeDef",
     {
         "Results": List[SearchForTextResultTypeDef],
         "Summary": SearchPlaceIndexForTextSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location.egg-info/PKG-INFO` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-location
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LocationService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LocationService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore location type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore location type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-location"></a>
 
 # types-aiobotocore-location
 
 [![PyPI - types-aiobotocore-location](https://img.shields.io/pypi/v/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-location.svg?color=blue)](https://pypi.org/project/types-aiobotocore-location)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-location?color=blue)](https://pypistats.org/packages/types-aiobotocore-location)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-location)](https://pepy.tech/project/types-aiobotocore-location)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LocationService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
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
 [types-aiobotocore-location docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/).
 
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
@@ -356,152 +355,157 @@
 )
 
 
 def check_value(value: BatchItemErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_location.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_location.type_defs import (
     ApiKeyFilterTypeDef,
+    ApiKeyRestrictionsOutputTypeDef,
     ApiKeyRestrictionsTypeDef,
     AssociateTrackerConsumerRequestRequestTypeDef,
     BatchItemErrorTypeDef,
     BatchDeleteDevicePositionHistoryRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionRequestRequestTypeDef,
     BatchPutGeofenceSuccessTypeDef,
     CalculateRouteCarModeOptionsTypeDef,
+    TimestampTypeDef,
     CalculateRouteMatrixSummaryTypeDef,
     CalculateRouteSummaryTypeDef,
     TruckDimensionsTypeDef,
     TruckWeightTypeDef,
+    CircleOutputTypeDef,
     CircleTypeDef,
     CreateGeofenceCollectionRequestRequestTypeDef,
-    CreateGeofenceCollectionResponseTypeDef,
-    CreateKeyResponseTypeDef,
     MapConfigurationTypeDef,
-    CreateMapResponseTypeDef,
     DataSourceConfigurationTypeDef,
-    CreatePlaceIndexResponseTypeDef,
     CreateRouteCalculatorRequestRequestTypeDef,
-    CreateRouteCalculatorResponseTypeDef,
     CreateTrackerRequestRequestTypeDef,
-    CreateTrackerResponseTypeDef,
     DeleteGeofenceCollectionRequestRequestTypeDef,
     DeleteKeyRequestRequestTypeDef,
     DeleteMapRequestRequestTypeDef,
     DeletePlaceIndexRequestRequestTypeDef,
     DeleteRouteCalculatorRequestRequestTypeDef,
     DeleteTrackerRequestRequestTypeDef,
     DescribeGeofenceCollectionRequestRequestTypeDef,
-    DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyRequestRequestTypeDef,
     DescribeMapRequestRequestTypeDef,
     DescribePlaceIndexRequestRequestTypeDef,
     DescribeRouteCalculatorRequestRequestTypeDef,
-    DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerRequestRequestTypeDef,
-    DescribeTrackerResponseTypeDef,
     PositionalAccuracyTypeDef,
     DisassociateTrackerConsumerRequestRequestTypeDef,
-    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
-    GetDevicePositionHistoryRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     GetDevicePositionRequestRequestTypeDef,
     GetGeofenceRequestRequestTypeDef,
     GetMapGlyphsRequestRequestTypeDef,
-    GetMapGlyphsResponseTypeDef,
     GetMapSpritesRequestRequestTypeDef,
-    GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorRequestRequestTypeDef,
-    GetMapStyleDescriptorResponseTypeDef,
     GetMapTileRequestRequestTypeDef,
-    GetMapTileResponseTypeDef,
     GetPlaceRequestRequestTypeDef,
     LegGeometryTypeDef,
     StepTypeDef,
-    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
     ListDevicePositionsRequestRequestTypeDef,
-    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
     ListGeofenceCollectionsRequestRequestTypeDef,
     ListGeofenceCollectionsResponseEntryTypeDef,
-    ListGeofencesRequestListGeofencesPaginateTypeDef,
     ListGeofencesRequestRequestTypeDef,
-    ListMapsRequestListMapsPaginateTypeDef,
     ListMapsRequestRequestTypeDef,
     ListMapsResponseEntryTypeDef,
-    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
     ListPlaceIndexesRequestRequestTypeDef,
     ListPlaceIndexesResponseEntryTypeDef,
-    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
     ListRouteCalculatorsRequestRequestTypeDef,
     ListRouteCalculatorsResponseEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
     ListTrackerConsumersRequestRequestTypeDef,
-    ListTrackerConsumersResponseTypeDef,
-    ListTrackersRequestListTrackersPaginateTypeDef,
     ListTrackersRequestRequestTypeDef,
     ListTrackersResponseEntryTypeDef,
     MapConfigurationUpdateTypeDef,
-    PaginatorConfigTypeDef,
     PlaceGeometryTypeDef,
     TimeZoneTypeDef,
-    PutGeofenceResponseTypeDef,
-    ResponseMetadataTypeDef,
     RouteMatrixEntryErrorTypeDef,
     SearchForSuggestionsResultTypeDef,
     SearchPlaceIndexForPositionRequestRequestTypeDef,
     SearchPlaceIndexForPositionSummaryTypeDef,
     SearchPlaceIndexForSuggestionsRequestRequestTypeDef,
     SearchPlaceIndexForSuggestionsSummaryTypeDef,
     SearchPlaceIndexForTextRequestRequestTypeDef,
     SearchPlaceIndexForTextSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGeofenceCollectionRequestRequestTypeDef,
-    UpdateGeofenceCollectionResponseTypeDef,
-    UpdateKeyResponseTypeDef,
-    UpdateMapResponseTypeDef,
-    UpdatePlaceIndexResponseTypeDef,
     UpdateRouteCalculatorRequestRequestTypeDef,
-    UpdateRouteCalculatorResponseTypeDef,
     UpdateTrackerRequestRequestTypeDef,
-    UpdateTrackerResponseTypeDef,
-    ListKeysRequestListKeysPaginateTypeDef,
     ListKeysRequestRequestTypeDef,
-    CreateKeyRequestRequestTypeDef,
-    DescribeKeyResponseTypeDef,
     ListKeysResponseEntryTypeDef,
-    UpdateKeyRequestRequestTypeDef,
+    ApiKeyRestrictionsUnionTypeDef,
     BatchDeleteDevicePositionHistoryErrorTypeDef,
     BatchDeleteGeofenceErrorTypeDef,
     BatchEvaluateGeofencesErrorTypeDef,
     BatchGetDevicePositionErrorTypeDef,
     BatchPutGeofenceErrorTypeDef,
     BatchUpdateDevicePositionErrorTypeDef,
+    CreateGeofenceCollectionResponseTypeDef,
+    CreateKeyResponseTypeDef,
+    CreateMapResponseTypeDef,
+    CreatePlaceIndexResponseTypeDef,
+    CreateRouteCalculatorResponseTypeDef,
+    CreateTrackerResponseTypeDef,
+    DescribeGeofenceCollectionResponseTypeDef,
+    DescribeKeyResponseTypeDef,
+    DescribeRouteCalculatorResponseTypeDef,
+    DescribeTrackerResponseTypeDef,
+    GetMapGlyphsResponseTypeDef,
+    GetMapSpritesResponseTypeDef,
+    GetMapStyleDescriptorResponseTypeDef,
+    GetMapTileResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTrackerConsumersResponseTypeDef,
+    PutGeofenceResponseTypeDef,
+    UpdateGeofenceCollectionResponseTypeDef,
+    UpdateKeyResponseTypeDef,
+    UpdateMapResponseTypeDef,
+    UpdatePlaceIndexResponseTypeDef,
+    UpdateRouteCalculatorResponseTypeDef,
+    UpdateTrackerResponseTypeDef,
+    CreateKeyRequestRequestTypeDef,
+    GetDevicePositionHistoryRequestRequestTypeDef,
+    UpdateKeyRequestRequestTypeDef,
     CalculateRouteTruckModeOptionsTypeDef,
+    GeofenceGeometryOutputTypeDef,
     GeofenceGeometryTypeDef,
     CreateMapRequestRequestTypeDef,
     DescribeMapResponseTypeDef,
     CreatePlaceIndexRequestRequestTypeDef,
     DescribePlaceIndexResponseTypeDef,
     UpdatePlaceIndexRequestRequestTypeDef,
     DevicePositionTypeDef,
     DevicePositionUpdateTypeDef,
     GetDevicePositionResponseTypeDef,
     ListDevicePositionsResponseEntryTypeDef,
+    GetDevicePositionHistoryRequestGetDevicePositionHistoryPaginateTypeDef,
+    ListDevicePositionsRequestListDevicePositionsPaginateTypeDef,
+    ListGeofenceCollectionsRequestListGeofenceCollectionsPaginateTypeDef,
+    ListGeofencesRequestListGeofencesPaginateTypeDef,
+    ListKeysRequestListKeysPaginateTypeDef,
+    ListMapsRequestListMapsPaginateTypeDef,
+    ListPlaceIndexesRequestListPlaceIndexesPaginateTypeDef,
+    ListRouteCalculatorsRequestListRouteCalculatorsPaginateTypeDef,
+    ListTrackerConsumersRequestListTrackerConsumersPaginateTypeDef,
+    ListTrackersRequestListTrackersPaginateTypeDef,
     LegTypeDef,
     ListGeofenceCollectionsResponseTypeDef,
     ListMapsResponseTypeDef,
     ListPlaceIndexesResponseTypeDef,
     ListRouteCalculatorsResponseTypeDef,
     ListTrackersResponseTypeDef,
     UpdateMapRequestRequestTypeDef,
@@ -512,36 +516,37 @@
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
     CalculateRouteMatrixRequestRequestTypeDef,
     CalculateRouteRequestRequestTypeDef,
-    BatchPutGeofenceRequestEntryTypeDef,
     GetGeofenceResponseTypeDef,
     ListGeofenceResponseEntryTypeDef,
+    BatchPutGeofenceRequestEntryTypeDef,
+    GeofenceGeometryUnionTypeDef,
     PutGeofenceRequestRequestTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     BatchEvaluateGeofencesRequestRequestTypeDef,
     BatchUpdateDevicePositionRequestRequestTypeDef,
     ListDevicePositionsResponseTypeDef,
     CalculateRouteResponseTypeDef,
     GetPlaceResponseTypeDef,
     SearchForPositionResultTypeDef,
     SearchForTextResultTypeDef,
     CalculateRouteMatrixResponseTypeDef,
-    BatchPutGeofenceRequestRequestTypeDef,
     ListGeofencesResponseTypeDef,
+    BatchPutGeofenceRequestRequestTypeDef,
     SearchPlaceIndexForPositionResponseTypeDef,
     SearchPlaceIndexForTextResponseTypeDef,
 )
 
 
-def get_structure() -> ApiKeyFilterTypeDef:
+def get_value() -> ApiKeyFilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-location-2.5.2/types_aiobotocore_location.egg-info/SOURCES.txt` & `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*


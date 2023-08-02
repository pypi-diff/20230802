# Comparing `tmp/types-aiobotocore-iot-roborunner-2.5.2.tar.gz` & `tmp/types-aiobotocore-iot-roborunner-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot-roborunner-2.5.2.tar", last modified: Sat Jul  8 01:43:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot-roborunner-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
```

## Comparing `types-aiobotocore-iot-roborunner-2.5.2.tar` & `types-aiobotocore-iot-roborunner-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.338296 types-aiobotocore-iot-roborunner-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:34.000000 types-aiobotocore-iot-roborunner-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-07-08 01:43:46.338296 types-aiobotocore-iot-roborunner-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-07-08 01:32:34.000000 types-aiobotocore-iot-roborunner-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:46.338296 types-aiobotocore-iot-roborunner-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-08 01:32:34.000000 types-aiobotocore-iot-roborunner-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.334296 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-08 01:32:34.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-08 01:32:34.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-08 01:32:34.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-07-08 01:32:34.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20814 2023-07-08 01:32:34.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-07-08 01:32:35.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-08 01:32:35.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-08 01:32:34.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-08 01:32:34.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:34.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20276 2023-07-08 01:32:36.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20237 2023-07-08 01:32:36.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:34.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.338296 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-07-08 01:43:46.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:43:46.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:46.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:43:46.000000 types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.349563 types-aiobotocore-iot-roborunner-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-08-02 14:52:26.349563 types-aiobotocore-iot-roborunner-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.349563 types-aiobotocore-iot-roborunner-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.345564 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20814 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20234 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-08-02 14:40:37.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:36.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.349563 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-08-02 14:52:26.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:26.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:26.000000 types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/LICENSE` & `types-aiobotocore-iot-roborunner-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/PKG-INFO` & `types-aiobotocore-iot-roborunner-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot-roborunner
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTRoboRunner 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTRoboRunner 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot-roborunner type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iot-roborunner type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot-roborunner"></a>
 
 # types-aiobotocore-iot-roborunner
 
 [![PyPI - types-aiobotocore-iot-roborunner](https://img.shields.io/pypi/v/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot-roborunner?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot-roborunner)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot-roborunner)](https://pepy.tech/project/types-aiobotocore-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTRoboRunner 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [types-aiobotocore-iot-roborunner docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/).
 
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
@@ -321,77 +320,77 @@
 )
 
 
 def check_value(value: DestinationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot_roborunner.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot_roborunner.type_defs import (
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    CreateDestinationResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateSiteRequestRequestTypeDef,
-    CreateSiteResponseTypeDef,
     CreateWorkerFleetRequestRequestTypeDef,
-    CreateWorkerFleetResponseTypeDef,
     OrientationTypeDef,
     VendorPropertiesTypeDef,
-    CreateWorkerResponseTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteSiteRequestRequestTypeDef,
     DeleteWorkerFleetRequestRequestTypeDef,
     DeleteWorkerRequestRequestTypeDef,
     DestinationTypeDef,
     GetDestinationRequestRequestTypeDef,
-    GetDestinationResponseTypeDef,
     GetSiteRequestRequestTypeDef,
-    GetSiteResponseTypeDef,
     GetWorkerFleetRequestRequestTypeDef,
-    GetWorkerFleetResponseTypeDef,
     GetWorkerRequestRequestTypeDef,
-    ListDestinationsRequestListDestinationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDestinationsRequestRequestTypeDef,
-    ListSitesRequestListSitesPaginateTypeDef,
     ListSitesRequestRequestTypeDef,
     SiteTypeDef,
-    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
     ListWorkerFleetsRequestRequestTypeDef,
     WorkerFleetTypeDef,
-    ListWorkersRequestListWorkersPaginateTypeDef,
     ListWorkersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateDestinationRequestRequestTypeDef,
-    UpdateDestinationResponseTypeDef,
     UpdateSiteRequestRequestTypeDef,
-    UpdateSiteResponseTypeDef,
     UpdateWorkerFleetRequestRequestTypeDef,
-    UpdateWorkerFleetResponseTypeDef,
     PositionCoordinatesTypeDef,
+    CreateDestinationResponseTypeDef,
+    CreateSiteResponseTypeDef,
+    CreateWorkerFleetResponseTypeDef,
+    CreateWorkerResponseTypeDef,
+    GetDestinationResponseTypeDef,
+    GetSiteResponseTypeDef,
+    GetWorkerFleetResponseTypeDef,
+    UpdateDestinationResponseTypeDef,
+    UpdateSiteResponseTypeDef,
+    UpdateWorkerFleetResponseTypeDef,
     ListDestinationsResponseTypeDef,
+    ListDestinationsRequestListDestinationsPaginateTypeDef,
+    ListSitesRequestListSitesPaginateTypeDef,
+    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+    ListWorkersRequestListWorkersPaginateTypeDef,
     ListSitesResponseTypeDef,
     ListWorkerFleetsResponseTypeDef,
     CreateWorkerRequestRequestTypeDef,
     GetWorkerResponseTypeDef,
     UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
     ListWorkersResponseTypeDef,
 )
 
 
-def get_structure() -> CartesianCoordinatesTypeDef:
+def get_value() -> CartesianCoordinatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/README.md` & `types-aiobotocore-iot-roborunner-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iot-roborunner"></a>
 
 # types-aiobotocore-iot-roborunner
 
 [![PyPI - types-aiobotocore-iot-roborunner](https://img.shields.io/pypi/v/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot-roborunner?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot-roborunner)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot-roborunner)](https://pepy.tech/project/types-aiobotocore-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTRoboRunner 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [types-aiobotocore-iot-roborunner docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/).
 
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
@@ -288,77 +288,77 @@
 )
 
 
 def check_value(value: DestinationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot_roborunner.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot_roborunner.type_defs import (
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    CreateDestinationResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateSiteRequestRequestTypeDef,
-    CreateSiteResponseTypeDef,
     CreateWorkerFleetRequestRequestTypeDef,
-    CreateWorkerFleetResponseTypeDef,
     OrientationTypeDef,
     VendorPropertiesTypeDef,
-    CreateWorkerResponseTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteSiteRequestRequestTypeDef,
     DeleteWorkerFleetRequestRequestTypeDef,
     DeleteWorkerRequestRequestTypeDef,
     DestinationTypeDef,
     GetDestinationRequestRequestTypeDef,
-    GetDestinationResponseTypeDef,
     GetSiteRequestRequestTypeDef,
-    GetSiteResponseTypeDef,
     GetWorkerFleetRequestRequestTypeDef,
-    GetWorkerFleetResponseTypeDef,
     GetWorkerRequestRequestTypeDef,
-    ListDestinationsRequestListDestinationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDestinationsRequestRequestTypeDef,
-    ListSitesRequestListSitesPaginateTypeDef,
     ListSitesRequestRequestTypeDef,
     SiteTypeDef,
-    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
     ListWorkerFleetsRequestRequestTypeDef,
     WorkerFleetTypeDef,
-    ListWorkersRequestListWorkersPaginateTypeDef,
     ListWorkersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateDestinationRequestRequestTypeDef,
-    UpdateDestinationResponseTypeDef,
     UpdateSiteRequestRequestTypeDef,
-    UpdateSiteResponseTypeDef,
     UpdateWorkerFleetRequestRequestTypeDef,
-    UpdateWorkerFleetResponseTypeDef,
     PositionCoordinatesTypeDef,
+    CreateDestinationResponseTypeDef,
+    CreateSiteResponseTypeDef,
+    CreateWorkerFleetResponseTypeDef,
+    CreateWorkerResponseTypeDef,
+    GetDestinationResponseTypeDef,
+    GetSiteResponseTypeDef,
+    GetWorkerFleetResponseTypeDef,
+    UpdateDestinationResponseTypeDef,
+    UpdateSiteResponseTypeDef,
+    UpdateWorkerFleetResponseTypeDef,
     ListDestinationsResponseTypeDef,
+    ListDestinationsRequestListDestinationsPaginateTypeDef,
+    ListSitesRequestListSitesPaginateTypeDef,
+    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+    ListWorkersRequestListWorkersPaginateTypeDef,
     ListSitesResponseTypeDef,
     ListWorkerFleetsResponseTypeDef,
     CreateWorkerRequestRequestTypeDef,
     GetWorkerResponseTypeDef,
     UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
     ListWorkersResponseTypeDef,
 )
 
 
-def get_structure() -> CartesianCoordinatesTypeDef:
+def get_value() -> CartesianCoordinatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/setup.py` & `types-aiobotocore-iot-roborunner-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot-roborunner",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iot_roborunner"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTRoboRunner 2.5.2 service generated with"
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
-    keywords="aiobotocore iot-roborunner type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore iot-roborunner type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iot_roborunner": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/"
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/__init__.py` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/__init__.pyi` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/__main__.py` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTRoboRunner 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IoTRoboRunner 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner\nOther"
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

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/client.py` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/client.pyi` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/literals.py` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/literals.pyi` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/paginator.py` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -43,80 +43,74 @@
 __all__ = (
     "ListDestinationsPaginator",
     "ListSitesPaginator",
     "ListWorkerFleetsPaginator",
     "ListWorkersPaginator",
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
 class ListDestinationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listdestinationspaginator)
     """
 
     def paginate(
         self,
         *,
         site: str,
         state: DestinationStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listdestinationspaginator)
         """
 
-
 class ListSitesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listsitespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listsitespaginator)
         """
 
-
 class ListWorkerFleetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listworkerfleetspaginator)
     """
 
     def paginate(
-        self, *, site: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, site: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkerFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listworkerfleetspaginator)
         """
 
-
 class ListWorkersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listworkerspaginator)
     """
 
     def paginate(
-        self, *, site: str, fleet: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, site: str, fleet: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listworkerspaginator)
         """
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/paginator.pyi` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/paginator.py`

 * *Files 17% similar despite different names*

```diff
@@ -43,74 +43,80 @@
 __all__ = (
     "ListDestinationsPaginator",
     "ListSitesPaginator",
     "ListWorkerFleetsPaginator",
     "ListWorkersPaginator",
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
 class ListDestinationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listdestinationspaginator)
     """
 
     def paginate(
         self,
         *,
         site: str,
         state: DestinationStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listdestinationspaginator)
         """
 
+
 class ListSitesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listsitespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listsitespaginator)
         """
 
+
 class ListWorkerFleetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listworkerfleetspaginator)
     """
 
     def paginate(
-        self, *, site: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, site: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkerFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listworkerfleetspaginator)
         """
 
+
 class ListWorkersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listworkerspaginator)
     """
 
     def paginate(
-        self, *, site: str, fleet: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, site: str, fleet: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorkersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/paginators/#listworkerspaginator)
         """
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/type_defs.py` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iot_roborunner.type_defs import CartesianCoordinatesTypeDef
 
-    data: CartesianCoordinatesTypeDef = {...}
+    data: CartesianCoordinatesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import DestinationStateType
@@ -22,54 +22,54 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CartesianCoordinatesTypeDef",
     "CreateDestinationRequestRequestTypeDef",
-    "CreateDestinationResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSiteRequestRequestTypeDef",
-    "CreateSiteResponseTypeDef",
     "CreateWorkerFleetRequestRequestTypeDef",
-    "CreateWorkerFleetResponseTypeDef",
     "OrientationTypeDef",
     "VendorPropertiesTypeDef",
-    "CreateWorkerResponseTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteSiteRequestRequestTypeDef",
     "DeleteWorkerFleetRequestRequestTypeDef",
     "DeleteWorkerRequestRequestTypeDef",
     "DestinationTypeDef",
     "GetDestinationRequestRequestTypeDef",
-    "GetDestinationResponseTypeDef",
     "GetSiteRequestRequestTypeDef",
-    "GetSiteResponseTypeDef",
     "GetWorkerFleetRequestRequestTypeDef",
-    "GetWorkerFleetResponseTypeDef",
     "GetWorkerRequestRequestTypeDef",
-    "ListDestinationsRequestListDestinationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDestinationsRequestRequestTypeDef",
-    "ListSitesRequestListSitesPaginateTypeDef",
     "ListSitesRequestRequestTypeDef",
     "SiteTypeDef",
-    "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
     "ListWorkerFleetsRequestRequestTypeDef",
     "WorkerFleetTypeDef",
-    "ListWorkersRequestListWorkersPaginateTypeDef",
     "ListWorkersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
-    "UpdateDestinationResponseTypeDef",
     "UpdateSiteRequestRequestTypeDef",
-    "UpdateSiteResponseTypeDef",
     "UpdateWorkerFleetRequestRequestTypeDef",
-    "UpdateWorkerFleetResponseTypeDef",
     "PositionCoordinatesTypeDef",
+    "CreateDestinationResponseTypeDef",
+    "CreateSiteResponseTypeDef",
+    "CreateWorkerFleetResponseTypeDef",
+    "CreateWorkerResponseTypeDef",
+    "GetDestinationResponseTypeDef",
+    "GetSiteResponseTypeDef",
+    "GetWorkerFleetResponseTypeDef",
+    "UpdateDestinationResponseTypeDef",
+    "UpdateSiteResponseTypeDef",
+    "UpdateWorkerFleetResponseTypeDef",
     "ListDestinationsResponseTypeDef",
+    "ListDestinationsRequestListDestinationsPaginateTypeDef",
+    "ListSitesRequestListSitesPaginateTypeDef",
+    "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    "ListWorkersRequestListWorkersPaginateTypeDef",
     "ListSitesResponseTypeDef",
     "ListWorkerFleetsResponseTypeDef",
     "CreateWorkerRequestRequestTypeDef",
     "GetWorkerResponseTypeDef",
     "UpdateWorkerRequestRequestTypeDef",
     "UpdateWorkerResponseTypeDef",
     "WorkerTypeDef",
@@ -118,23 +118,22 @@
 
 class CreateDestinationRequestRequestTypeDef(
     _RequiredCreateDestinationRequestRequestTypeDef, _OptionalCreateDestinationRequestRequestTypeDef
 ):
     pass
 
 
-CreateDestinationResponseTypeDef = TypedDict(
-    "CreateDestinationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSiteRequestRequestTypeDef",
     {
         "name": str,
@@ -153,25 +152,14 @@
 
 class CreateSiteRequestRequestTypeDef(
     _RequiredCreateSiteRequestRequestTypeDef, _OptionalCreateSiteRequestRequestTypeDef
 ):
     pass
 
 
-CreateSiteResponseTypeDef = TypedDict(
-    "CreateSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateWorkerFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerFleetRequestRequestTypeDef",
     {
         "name": str,
         "site": str,
     },
 )
@@ -187,25 +175,14 @@
 
 class CreateWorkerFleetRequestRequestTypeDef(
     _RequiredCreateWorkerFleetRequestRequestTypeDef, _OptionalCreateWorkerFleetRequestRequestTypeDef
 ):
     pass
 
 
-CreateWorkerFleetResponseTypeDef = TypedDict(
-    "CreateWorkerFleetResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OrientationTypeDef = TypedDict(
     "OrientationTypeDef",
     {
         "degrees": float,
     },
     total=False,
 )
@@ -227,26 +204,14 @@
 )
 
 
 class VendorPropertiesTypeDef(_RequiredVendorPropertiesTypeDef, _OptionalVendorPropertiesTypeDef):
     pass
 
 
-CreateWorkerResponseTypeDef = TypedDict(
-    "CreateWorkerResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "site": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDestinationRequestRequestTypeDef = TypedDict(
     "DeleteDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -299,101 +264,45 @@
 GetDestinationRequestRequestTypeDef = TypedDict(
     "GetDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetDestinationResponseTypeDef = TypedDict(
-    "GetDestinationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "site": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSiteRequestRequestTypeDef = TypedDict(
     "GetSiteRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetSiteResponseTypeDef = TypedDict(
-    "GetSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "countryCode": str,
-        "description": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkerFleetRequestRequestTypeDef = TypedDict(
     "GetWorkerFleetRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetWorkerFleetResponseTypeDef = TypedDict(
-    "GetWorkerFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "site": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkerRequestRequestTypeDef = TypedDict(
     "GetWorkerRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListDestinationsRequestListDestinationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "state": DestinationStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListDestinationsRequestListDestinationsPaginateTypeDef(
-    _RequiredListDestinationsRequestListDestinationsPaginateTypeDef,
-    _OptionalListDestinationsRequestListDestinationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListDestinationsRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListDestinationsRequestRequestTypeDef = TypedDict(
@@ -409,22 +318,14 @@
 
 class ListDestinationsRequestRequestTypeDef(
     _RequiredListDestinationsRequestRequestTypeDef, _OptionalListDestinationsRequestRequestTypeDef
 ):
     pass
 
 
-ListSitesRequestListSitesPaginateTypeDef = TypedDict(
-    "ListSitesRequestListSitesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSitesRequestRequestTypeDef = TypedDict(
     "ListSitesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -436,36 +337,14 @@
         "arn": str,
         "name": str,
         "countryCode": str,
         "createdAt": datetime,
     },
 )
 
-_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(
-    _RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-    _OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListWorkerFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkerFleetsRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListWorkerFleetsRequestRequestTypeDef = TypedDict(
@@ -504,37 +383,14 @@
 )
 
 
 class WorkerFleetTypeDef(_RequiredWorkerFleetTypeDef, _OptionalWorkerFleetTypeDef):
     pass
 
 
-_RequiredListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
-    "_RequiredListWorkersRequestListWorkersPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
-    "_OptionalListWorkersRequestListWorkersPaginateTypeDef",
-    {
-        "fleet": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListWorkersRequestListWorkersPaginateTypeDef(
-    _RequiredListWorkersRequestListWorkersPaginateTypeDef,
-    _OptionalListWorkersRequestListWorkersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListWorkersRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkersRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListWorkersRequestRequestTypeDef = TypedDict(
@@ -550,35 +406,14 @@
 
 class ListWorkersRequestRequestTypeDef(
     _RequiredListWorkersRequestRequestTypeDef, _OptionalListWorkersRequestRequestTypeDef
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
 _RequiredUpdateDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateDestinationRequestRequestTypeDef = TypedDict(
@@ -594,27 +429,14 @@
 
 class UpdateDestinationRequestRequestTypeDef(
     _RequiredUpdateDestinationRequestRequestTypeDef, _OptionalUpdateDestinationRequestRequestTypeDef
 ):
     pass
 
 
-UpdateDestinationResponseTypeDef = TypedDict(
-    "UpdateDestinationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateSiteRequestRequestTypeDef = TypedDict(
@@ -630,27 +452,14 @@
 
 class UpdateSiteRequestRequestTypeDef(
     _RequiredUpdateSiteRequestRequestTypeDef, _OptionalUpdateSiteRequestRequestTypeDef
 ):
     pass
 
 
-UpdateSiteResponseTypeDef = TypedDict(
-    "UpdateSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "countryCode": str,
-        "description": str,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkerFleetRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
@@ -665,58 +474,249 @@
 
 class UpdateWorkerFleetRequestRequestTypeDef(
     _RequiredUpdateWorkerFleetRequestRequestTypeDef, _OptionalUpdateWorkerFleetRequestRequestTypeDef
 ):
     pass
 
 
-UpdateWorkerFleetResponseTypeDef = TypedDict(
-    "UpdateWorkerFleetResponseTypeDef",
+PositionCoordinatesTypeDef = TypedDict(
+    "PositionCoordinatesTypeDef",
+    {
+        "cartesianCoordinates": CartesianCoordinatesTypeDef,
+    },
+    total=False,
+)
+
+CreateDestinationResponseTypeDef = TypedDict(
+    "CreateDestinationResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSiteResponseTypeDef = TypedDict(
+    "CreateSiteResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkerFleetResponseTypeDef = TypedDict(
+    "CreateWorkerFleetResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkerResponseTypeDef = TypedDict(
+    "CreateWorkerResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "site": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDestinationResponseTypeDef = TypedDict(
+    "GetDestinationResponseTypeDef",
     {
         "arn": str,
         "id": str,
         "name": str,
+        "site": str,
+        "createdAt": datetime,
         "updatedAt": datetime,
+        "state": DestinationStateType,
         "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PositionCoordinatesTypeDef = TypedDict(
-    "PositionCoordinatesTypeDef",
+GetSiteResponseTypeDef = TypedDict(
+    "GetSiteResponseTypeDef",
     {
-        "cartesianCoordinates": CartesianCoordinatesTypeDef,
+        "arn": str,
+        "id": str,
+        "name": str,
+        "countryCode": str,
+        "description": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkerFleetResponseTypeDef = TypedDict(
+    "GetWorkerFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "site": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDestinationResponseTypeDef = TypedDict(
+    "UpdateDestinationResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSiteResponseTypeDef = TypedDict(
+    "UpdateSiteResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "countryCode": str,
+        "description": str,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorkerFleetResponseTypeDef = TypedDict(
+    "UpdateWorkerFleetResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "updatedAt": datetime,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListDestinationsResponseTypeDef = TypedDict(
     "ListDestinationsResponseTypeDef",
     {
         "nextToken": str,
         "destinations": List[DestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListDestinationsRequestListDestinationsPaginateTypeDef",
+    {
+        "state": DestinationStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDestinationsRequestListDestinationsPaginateTypeDef(
+    _RequiredListDestinationsRequestListDestinationsPaginateTypeDef,
+    _OptionalListDestinationsRequestListDestinationsPaginateTypeDef,
+):
+    pass
+
+
+ListSitesRequestListSitesPaginateTypeDef = TypedDict(
+    "ListSitesRequestListSitesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(
+    _RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+    _OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
+    "_RequiredListWorkersRequestListWorkersPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
+    "_OptionalListWorkersRequestListWorkersPaginateTypeDef",
+    {
+        "fleet": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListWorkersRequestListWorkersPaginateTypeDef(
+    _RequiredListWorkersRequestListWorkersPaginateTypeDef,
+    _OptionalListWorkersRequestListWorkersPaginateTypeDef,
+):
+    pass
+
+
 ListSitesResponseTypeDef = TypedDict(
     "ListSitesResponseTypeDef",
     {
         "nextToken": str,
         "sites": List[SiteTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkerFleetsResponseTypeDef = TypedDict(
     "ListWorkerFleetsResponseTypeDef",
     {
         "nextToken": str,
         "workerFleets": List[WorkerFleetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWorkerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerRequestRequestTypeDef",
     {
         "name": str,
@@ -754,15 +754,15 @@
         "updatedAt": datetime,
         "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
         "orientation": OrientationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateWorkerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkerRequestRequestTypeDef",
     {
         "id": str,
@@ -797,15 +797,15 @@
         "updatedAt": datetime,
         "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
         "orientation": OrientationTypeDef,
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredWorkerTypeDef = TypedDict(
     "_RequiredWorkerTypeDef",
     {
         "arn": str,
@@ -835,10 +835,10 @@
 
 
 ListWorkersResponseTypeDef = TypedDict(
     "ListWorkersResponseTypeDef",
     {
         "nextToken": str,
         "workers": List[WorkerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner/type_defs.pyi` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iot_roborunner.type_defs import CartesianCoordinatesTypeDef
 
-    data: CartesianCoordinatesTypeDef = {...}
+    data: CartesianCoordinatesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import DestinationStateType
@@ -21,54 +21,54 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CartesianCoordinatesTypeDef",
     "CreateDestinationRequestRequestTypeDef",
-    "CreateDestinationResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSiteRequestRequestTypeDef",
-    "CreateSiteResponseTypeDef",
     "CreateWorkerFleetRequestRequestTypeDef",
-    "CreateWorkerFleetResponseTypeDef",
     "OrientationTypeDef",
     "VendorPropertiesTypeDef",
-    "CreateWorkerResponseTypeDef",
     "DeleteDestinationRequestRequestTypeDef",
     "DeleteSiteRequestRequestTypeDef",
     "DeleteWorkerFleetRequestRequestTypeDef",
     "DeleteWorkerRequestRequestTypeDef",
     "DestinationTypeDef",
     "GetDestinationRequestRequestTypeDef",
-    "GetDestinationResponseTypeDef",
     "GetSiteRequestRequestTypeDef",
-    "GetSiteResponseTypeDef",
     "GetWorkerFleetRequestRequestTypeDef",
-    "GetWorkerFleetResponseTypeDef",
     "GetWorkerRequestRequestTypeDef",
-    "ListDestinationsRequestListDestinationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDestinationsRequestRequestTypeDef",
-    "ListSitesRequestListSitesPaginateTypeDef",
     "ListSitesRequestRequestTypeDef",
     "SiteTypeDef",
-    "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
     "ListWorkerFleetsRequestRequestTypeDef",
     "WorkerFleetTypeDef",
-    "ListWorkersRequestListWorkersPaginateTypeDef",
     "ListWorkersRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateDestinationRequestRequestTypeDef",
-    "UpdateDestinationResponseTypeDef",
     "UpdateSiteRequestRequestTypeDef",
-    "UpdateSiteResponseTypeDef",
     "UpdateWorkerFleetRequestRequestTypeDef",
-    "UpdateWorkerFleetResponseTypeDef",
     "PositionCoordinatesTypeDef",
+    "CreateDestinationResponseTypeDef",
+    "CreateSiteResponseTypeDef",
+    "CreateWorkerFleetResponseTypeDef",
+    "CreateWorkerResponseTypeDef",
+    "GetDestinationResponseTypeDef",
+    "GetSiteResponseTypeDef",
+    "GetWorkerFleetResponseTypeDef",
+    "UpdateDestinationResponseTypeDef",
+    "UpdateSiteResponseTypeDef",
+    "UpdateWorkerFleetResponseTypeDef",
     "ListDestinationsResponseTypeDef",
+    "ListDestinationsRequestListDestinationsPaginateTypeDef",
+    "ListSitesRequestListSitesPaginateTypeDef",
+    "ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    "ListWorkersRequestListWorkersPaginateTypeDef",
     "ListSitesResponseTypeDef",
     "ListWorkerFleetsResponseTypeDef",
     "CreateWorkerRequestRequestTypeDef",
     "GetWorkerResponseTypeDef",
     "UpdateWorkerRequestRequestTypeDef",
     "UpdateWorkerResponseTypeDef",
     "WorkerTypeDef",
@@ -113,23 +113,22 @@
 )
 
 class CreateDestinationRequestRequestTypeDef(
     _RequiredCreateDestinationRequestRequestTypeDef, _OptionalCreateDestinationRequestRequestTypeDef
 ):
     pass
 
-CreateDestinationResponseTypeDef = TypedDict(
-    "CreateDestinationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSiteRequestRequestTypeDef",
     {
         "name": str,
@@ -146,25 +145,14 @@
 )
 
 class CreateSiteRequestRequestTypeDef(
     _RequiredCreateSiteRequestRequestTypeDef, _OptionalCreateSiteRequestRequestTypeDef
 ):
     pass
 
-CreateSiteResponseTypeDef = TypedDict(
-    "CreateSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateWorkerFleetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerFleetRequestRequestTypeDef",
     {
         "name": str,
         "site": str,
     },
 )
@@ -178,25 +166,14 @@
 )
 
 class CreateWorkerFleetRequestRequestTypeDef(
     _RequiredCreateWorkerFleetRequestRequestTypeDef, _OptionalCreateWorkerFleetRequestRequestTypeDef
 ):
     pass
 
-CreateWorkerFleetResponseTypeDef = TypedDict(
-    "CreateWorkerFleetResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OrientationTypeDef = TypedDict(
     "OrientationTypeDef",
     {
         "degrees": float,
     },
     total=False,
 )
@@ -216,26 +193,14 @@
     },
     total=False,
 )
 
 class VendorPropertiesTypeDef(_RequiredVendorPropertiesTypeDef, _OptionalVendorPropertiesTypeDef):
     pass
 
-CreateWorkerResponseTypeDef = TypedDict(
-    "CreateWorkerResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "site": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDestinationRequestRequestTypeDef = TypedDict(
     "DeleteDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -286,99 +251,45 @@
 GetDestinationRequestRequestTypeDef = TypedDict(
     "GetDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetDestinationResponseTypeDef = TypedDict(
-    "GetDestinationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "site": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSiteRequestRequestTypeDef = TypedDict(
     "GetSiteRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetSiteResponseTypeDef = TypedDict(
-    "GetSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "countryCode": str,
-        "description": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkerFleetRequestRequestTypeDef = TypedDict(
     "GetWorkerFleetRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetWorkerFleetResponseTypeDef = TypedDict(
-    "GetWorkerFleetResponseTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "name": str,
-        "site": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkerRequestRequestTypeDef = TypedDict(
     "GetWorkerRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-_RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListDestinationsRequestListDestinationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "state": DestinationStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListDestinationsRequestListDestinationsPaginateTypeDef(
-    _RequiredListDestinationsRequestListDestinationsPaginateTypeDef,
-    _OptionalListDestinationsRequestListDestinationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListDestinationsRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListDestinationsRequestRequestTypeDef = TypedDict(
@@ -392,22 +303,14 @@
 )
 
 class ListDestinationsRequestRequestTypeDef(
     _RequiredListDestinationsRequestRequestTypeDef, _OptionalListDestinationsRequestRequestTypeDef
 ):
     pass
 
-ListSitesRequestListSitesPaginateTypeDef = TypedDict(
-    "ListSitesRequestListSitesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSitesRequestRequestTypeDef = TypedDict(
     "ListSitesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -419,34 +322,14 @@
         "arn": str,
         "name": str,
         "countryCode": str,
         "createdAt": datetime,
     },
 )
 
-_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(
-    _RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-    _OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListWorkerFleetsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkerFleetsRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListWorkerFleetsRequestRequestTypeDef = TypedDict(
@@ -481,35 +364,14 @@
     },
     total=False,
 )
 
 class WorkerFleetTypeDef(_RequiredWorkerFleetTypeDef, _OptionalWorkerFleetTypeDef):
     pass
 
-_RequiredListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
-    "_RequiredListWorkersRequestListWorkersPaginateTypeDef",
-    {
-        "site": str,
-    },
-)
-_OptionalListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
-    "_OptionalListWorkersRequestListWorkersPaginateTypeDef",
-    {
-        "fleet": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListWorkersRequestListWorkersPaginateTypeDef(
-    _RequiredListWorkersRequestListWorkersPaginateTypeDef,
-    _OptionalListWorkersRequestListWorkersPaginateTypeDef,
-):
-    pass
-
 _RequiredListWorkersRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkersRequestRequestTypeDef",
     {
         "site": str,
     },
 )
 _OptionalListWorkersRequestRequestTypeDef = TypedDict(
@@ -523,35 +385,14 @@
 )
 
 class ListWorkersRequestRequestTypeDef(
     _RequiredListWorkersRequestRequestTypeDef, _OptionalListWorkersRequestRequestTypeDef
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
 _RequiredUpdateDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDestinationRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateDestinationRequestRequestTypeDef = TypedDict(
@@ -565,27 +406,14 @@
 )
 
 class UpdateDestinationRequestRequestTypeDef(
     _RequiredUpdateDestinationRequestRequestTypeDef, _OptionalUpdateDestinationRequestRequestTypeDef
 ):
     pass
 
-UpdateDestinationResponseTypeDef = TypedDict(
-    "UpdateDestinationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "updatedAt": datetime,
-        "state": DestinationStateType,
-        "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateSiteRequestRequestTypeDef = TypedDict(
@@ -599,27 +427,14 @@
 )
 
 class UpdateSiteRequestRequestTypeDef(
     _RequiredUpdateSiteRequestRequestTypeDef, _OptionalUpdateSiteRequestRequestTypeDef
 ):
     pass
 
-UpdateSiteResponseTypeDef = TypedDict(
-    "UpdateSiteResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "countryCode": str,
-        "description": str,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkerFleetRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalUpdateWorkerFleetRequestRequestTypeDef = TypedDict(
@@ -632,58 +447,243 @@
 )
 
 class UpdateWorkerFleetRequestRequestTypeDef(
     _RequiredUpdateWorkerFleetRequestRequestTypeDef, _OptionalUpdateWorkerFleetRequestRequestTypeDef
 ):
     pass
 
-UpdateWorkerFleetResponseTypeDef = TypedDict(
-    "UpdateWorkerFleetResponseTypeDef",
+PositionCoordinatesTypeDef = TypedDict(
+    "PositionCoordinatesTypeDef",
+    {
+        "cartesianCoordinates": CartesianCoordinatesTypeDef,
+    },
+    total=False,
+)
+
+CreateDestinationResponseTypeDef = TypedDict(
+    "CreateDestinationResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSiteResponseTypeDef = TypedDict(
+    "CreateSiteResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkerFleetResponseTypeDef = TypedDict(
+    "CreateWorkerFleetResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkerResponseTypeDef = TypedDict(
+    "CreateWorkerResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "site": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDestinationResponseTypeDef = TypedDict(
+    "GetDestinationResponseTypeDef",
     {
         "arn": str,
         "id": str,
         "name": str,
+        "site": str,
+        "createdAt": datetime,
         "updatedAt": datetime,
+        "state": DestinationStateType,
         "additionalFixedProperties": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PositionCoordinatesTypeDef = TypedDict(
-    "PositionCoordinatesTypeDef",
+GetSiteResponseTypeDef = TypedDict(
+    "GetSiteResponseTypeDef",
     {
-        "cartesianCoordinates": CartesianCoordinatesTypeDef,
+        "arn": str,
+        "id": str,
+        "name": str,
+        "countryCode": str,
+        "description": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkerFleetResponseTypeDef = TypedDict(
+    "GetWorkerFleetResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "site": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDestinationResponseTypeDef = TypedDict(
+    "UpdateDestinationResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "updatedAt": datetime,
+        "state": DestinationStateType,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSiteResponseTypeDef = TypedDict(
+    "UpdateSiteResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "countryCode": str,
+        "description": str,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateWorkerFleetResponseTypeDef = TypedDict(
+    "UpdateWorkerFleetResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "name": str,
+        "updatedAt": datetime,
+        "additionalFixedProperties": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListDestinationsResponseTypeDef = TypedDict(
     "ListDestinationsResponseTypeDef",
     {
         "nextToken": str,
         "destinations": List[DestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListDestinationsRequestListDestinationsPaginateTypeDef",
+    {
+        "site": str,
     },
 )
+_OptionalListDestinationsRequestListDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListDestinationsRequestListDestinationsPaginateTypeDef",
+    {
+        "state": DestinationStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDestinationsRequestListDestinationsPaginateTypeDef(
+    _RequiredListDestinationsRequestListDestinationsPaginateTypeDef,
+    _OptionalListDestinationsRequestListDestinationsPaginateTypeDef,
+):
+    pass
+
+ListSitesRequestListSitesPaginateTypeDef = TypedDict(
+    "ListSitesRequestListSitesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef(
+    _RequiredListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+    _OptionalListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
+    "_RequiredListWorkersRequestListWorkersPaginateTypeDef",
+    {
+        "site": str,
+    },
+)
+_OptionalListWorkersRequestListWorkersPaginateTypeDef = TypedDict(
+    "_OptionalListWorkersRequestListWorkersPaginateTypeDef",
+    {
+        "fleet": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListWorkersRequestListWorkersPaginateTypeDef(
+    _RequiredListWorkersRequestListWorkersPaginateTypeDef,
+    _OptionalListWorkersRequestListWorkersPaginateTypeDef,
+):
+    pass
 
 ListSitesResponseTypeDef = TypedDict(
     "ListSitesResponseTypeDef",
     {
         "nextToken": str,
         "sites": List[SiteTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkerFleetsResponseTypeDef = TypedDict(
     "ListWorkerFleetsResponseTypeDef",
     {
         "nextToken": str,
         "workerFleets": List[WorkerFleetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWorkerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkerRequestRequestTypeDef",
     {
         "name": str,
@@ -719,15 +719,15 @@
         "updatedAt": datetime,
         "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
         "orientation": OrientationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateWorkerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkerRequestRequestTypeDef",
     {
         "id": str,
@@ -760,15 +760,15 @@
         "updatedAt": datetime,
         "name": str,
         "additionalTransientProperties": str,
         "additionalFixedProperties": str,
         "orientation": OrientationTypeDef,
         "vendorProperties": VendorPropertiesTypeDef,
         "position": PositionCoordinatesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredWorkerTypeDef = TypedDict(
     "_RequiredWorkerTypeDef",
     {
         "arn": str,
@@ -796,10 +796,10 @@
     pass
 
 ListWorkersResponseTypeDef = TypedDict(
     "ListWorkersResponseTypeDef",
     {
         "nextToken": str,
         "workers": List[WorkerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot-roborunner
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTRoboRunner 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTRoboRunner 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot-roborunner type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iot-roborunner type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot-roborunner"></a>
 
 # types-aiobotocore-iot-roborunner
 
 [![PyPI - types-aiobotocore-iot-roborunner](https://img.shields.io/pypi/v/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot-roborunner.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot-roborunner)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot-roborunner?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot-roborunner)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot-roborunner)](https://pepy.tech/project/types-aiobotocore-iot-roborunner)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTRoboRunner 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
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
 [types-aiobotocore-iot-roborunner docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot_roborunner/).
 
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
@@ -321,77 +320,77 @@
 )
 
 
 def check_value(value: DestinationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot_roborunner.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot_roborunner.type_defs import (
     CartesianCoordinatesTypeDef,
     CreateDestinationRequestRequestTypeDef,
-    CreateDestinationResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateSiteRequestRequestTypeDef,
-    CreateSiteResponseTypeDef,
     CreateWorkerFleetRequestRequestTypeDef,
-    CreateWorkerFleetResponseTypeDef,
     OrientationTypeDef,
     VendorPropertiesTypeDef,
-    CreateWorkerResponseTypeDef,
     DeleteDestinationRequestRequestTypeDef,
     DeleteSiteRequestRequestTypeDef,
     DeleteWorkerFleetRequestRequestTypeDef,
     DeleteWorkerRequestRequestTypeDef,
     DestinationTypeDef,
     GetDestinationRequestRequestTypeDef,
-    GetDestinationResponseTypeDef,
     GetSiteRequestRequestTypeDef,
-    GetSiteResponseTypeDef,
     GetWorkerFleetRequestRequestTypeDef,
-    GetWorkerFleetResponseTypeDef,
     GetWorkerRequestRequestTypeDef,
-    ListDestinationsRequestListDestinationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDestinationsRequestRequestTypeDef,
-    ListSitesRequestListSitesPaginateTypeDef,
     ListSitesRequestRequestTypeDef,
     SiteTypeDef,
-    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
     ListWorkerFleetsRequestRequestTypeDef,
     WorkerFleetTypeDef,
-    ListWorkersRequestListWorkersPaginateTypeDef,
     ListWorkersRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateDestinationRequestRequestTypeDef,
-    UpdateDestinationResponseTypeDef,
     UpdateSiteRequestRequestTypeDef,
-    UpdateSiteResponseTypeDef,
     UpdateWorkerFleetRequestRequestTypeDef,
-    UpdateWorkerFleetResponseTypeDef,
     PositionCoordinatesTypeDef,
+    CreateDestinationResponseTypeDef,
+    CreateSiteResponseTypeDef,
+    CreateWorkerFleetResponseTypeDef,
+    CreateWorkerResponseTypeDef,
+    GetDestinationResponseTypeDef,
+    GetSiteResponseTypeDef,
+    GetWorkerFleetResponseTypeDef,
+    UpdateDestinationResponseTypeDef,
+    UpdateSiteResponseTypeDef,
+    UpdateWorkerFleetResponseTypeDef,
     ListDestinationsResponseTypeDef,
+    ListDestinationsRequestListDestinationsPaginateTypeDef,
+    ListSitesRequestListSitesPaginateTypeDef,
+    ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef,
+    ListWorkersRequestListWorkersPaginateTypeDef,
     ListSitesResponseTypeDef,
     ListWorkerFleetsResponseTypeDef,
     CreateWorkerRequestRequestTypeDef,
     GetWorkerResponseTypeDef,
     UpdateWorkerRequestRequestTypeDef,
     UpdateWorkerResponseTypeDef,
     WorkerTypeDef,
     ListWorkersResponseTypeDef,
 )
 
 
-def get_structure() -> CartesianCoordinatesTypeDef:
+def get_value() -> CartesianCoordinatesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot-roborunner-2.5.2/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt` & `types-aiobotocore-iot-roborunner-2.5.2.post1/types_aiobotocore_iot_roborunner.egg-info/SOURCES.txt`

 * *Files identical despite different names*


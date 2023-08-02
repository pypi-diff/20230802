# Comparing `tmp/types-aiobotocore-iot1click-devices-2.5.2.tar.gz` & `tmp/types-aiobotocore-iot1click-devices-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot1click-devices-2.5.2.tar", last modified: Sat Jul  8 01:43:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot1click-devices-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
```

## Comparing `types-aiobotocore-iot1click-devices-2.5.2.tar` & `types-aiobotocore-iot1click-devices-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.590263 types-aiobotocore-iot1click-devices-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-07-08 01:43:44.586263 types-aiobotocore-iot1click-devices-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13220 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:44.590263 types-aiobotocore-iot1click-devices-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.586263 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9748 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:37.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.586263 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-07-08 01:43:44.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-08 01:43:44.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:44.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:44.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:44.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:44.000000 types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.357569 types-aiobotocore-iot1click-devices-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-08-02 14:52:24.357569 types-aiobotocore-iot1click-devices-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.357569 types-aiobotocore-iot1click-devices-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.353569 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9779 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:37.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.357569 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/LICENSE` & `types-aiobotocore-iot1click-devices-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/PKG-INFO` & `types-aiobotocore-iot1click-devices-2.5.2.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-devices
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoT1ClickDevicesService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoT1ClickDevicesService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot1click-devices type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iot1click-devices type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot1click-devices"></a>
 
 # types-aiobotocore-iot1click-devices
 
 [![PyPI - types-aiobotocore-iot1click-devices](https://img.shields.io/pypi/v/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot1click-devices?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot1click-devices)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-devices)](https://pepy.tech/project/types-aiobotocore-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoT1ClickDevicesService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [types-aiobotocore-iot1click-devices docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/).
 
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
@@ -311,59 +310,60 @@
 )
 
 
 def check_value(value: ListDeviceEventsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot1click_devices.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
-    ClaimDevicesByClaimCodeResponseTypeDef,
+    ResponseMetadataTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
     DeviceMethodTypeDef,
-    EmptyResponseMetadataTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
-    FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
-    InitiateDeviceClaimResponseTypeDef,
-    InvokeDeviceMethodResponseTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    ListDeviceEventsRequestRequestTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
+    PaginatorConfigTypeDef,
+    TimestampTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UnclaimDeviceRequestRequestTypeDef,
-    UnclaimDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceStateRequestRequestTypeDef,
+    ClaimDevicesByClaimCodeResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FinalizeDeviceClaimResponseTypeDef,
+    InitiateDeviceClaimResponseTypeDef,
+    InvokeDeviceMethodResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UnclaimDeviceResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     DeviceEventTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InvokeDeviceMethodRequestRequestTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
+    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    ListDeviceEventsRequestRequestTypeDef,
     ListDeviceEventsResponseTypeDef,
 )
 
 
-def get_structure() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
+def get_value() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/README.md` & `types-aiobotocore-iot1click-devices-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iot1click-devices"></a>
 
 # types-aiobotocore-iot1click-devices
 
 [![PyPI - types-aiobotocore-iot1click-devices](https://img.shields.io/pypi/v/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot1click-devices?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot1click-devices)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-devices)](https://pepy.tech/project/types-aiobotocore-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoT1ClickDevicesService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [types-aiobotocore-iot1click-devices docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/).
 
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
@@ -278,59 +278,60 @@
 )
 
 
 def check_value(value: ListDeviceEventsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot1click_devices.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
-    ClaimDevicesByClaimCodeResponseTypeDef,
+    ResponseMetadataTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
     DeviceMethodTypeDef,
-    EmptyResponseMetadataTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
-    FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
-    InitiateDeviceClaimResponseTypeDef,
-    InvokeDeviceMethodResponseTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    ListDeviceEventsRequestRequestTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
+    PaginatorConfigTypeDef,
+    TimestampTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UnclaimDeviceRequestRequestTypeDef,
-    UnclaimDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceStateRequestRequestTypeDef,
+    ClaimDevicesByClaimCodeResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FinalizeDeviceClaimResponseTypeDef,
+    InitiateDeviceClaimResponseTypeDef,
+    InvokeDeviceMethodResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UnclaimDeviceResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     DeviceEventTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InvokeDeviceMethodRequestRequestTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
+    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    ListDeviceEventsRequestRequestTypeDef,
     ListDeviceEventsResponseTypeDef,
 )
 
 
-def get_structure() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
+def get_value() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/setup.py` & `types-aiobotocore-iot1click-devices-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot1click-devices",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iot1click_devices"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoT1ClickDevicesService 2.5.2 service generated with"
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
-    keywords=(
-        "aiobotocore iot1click-devices type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore iot1click-devices type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iot1click_devices": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/"
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/__init__.py` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/__init__.pyi` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/__main__.py` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.IoT1ClickDevicesService 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService\nOther"
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

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/client.py` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("iot1click-devices") as client:
         client: IoT1ClickDevicesServiceClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import ListDeviceEventsPaginator, ListDevicesPaginator
 from .type_defs import (
     ClaimDevicesByClaimCodeResponseTypeDef,
@@ -30,14 +29,15 @@
     FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InitiateDeviceClaimResponseTypeDef,
     InvokeDeviceMethodResponseTypeDef,
     ListDeviceEventsResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TimestampTypeDef,
     UnclaimDeviceResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -173,16 +173,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/client/#invoke_device_method)
         """
 
     async def list_device_events(
         self,
         *,
         DeviceId: str,
-        FromTimeStamp: Union[datetime, str],
-        ToTimeStamp: Union[datetime, str],
+        FromTimeStamp: TimestampTypeDef,
+        ToTimeStamp: TimestampTypeDef,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListDeviceEventsResponseTypeDef:
         """
         Using a device ID, returns a DeviceEventsResponse object containing an array of
         events for the device.
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/client.pyi` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("iot1click-devices") as client:
         client: IoT1ClickDevicesServiceClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import ListDeviceEventsPaginator, ListDevicesPaginator
 from .type_defs import (
     ClaimDevicesByClaimCodeResponseTypeDef,
@@ -30,14 +29,15 @@
     FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InitiateDeviceClaimResponseTypeDef,
     InvokeDeviceMethodResponseTypeDef,
     ListDeviceEventsResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TimestampTypeDef,
     UnclaimDeviceResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -159,16 +159,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Client.invoke_device_method)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/client/#invoke_device_method)
         """
     async def list_device_events(
         self,
         *,
         DeviceId: str,
-        FromTimeStamp: Union[datetime, str],
-        ToTimeStamp: Union[datetime, str],
+        FromTimeStamp: TimestampTypeDef,
+        ToTimeStamp: TimestampTypeDef,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListDeviceEventsResponseTypeDef:
         """
         Using a device ID, returns a DeviceEventsResponse object containing an array of
         events for the device.
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/literals.py` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/literals.pyi` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/paginator.py` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,24 +18,24 @@
     with session.create_client("iot1click-devices") as client:
         client: IoT1ClickDevicesServiceClient
 
         list_device_events_paginator: ListDeviceEventsPaginator = client.get_paginator("list_device_events")
         list_devices_paginator: ListDevicesPaginator = client.get_paginator("list_devices")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ListDeviceEventsResponseTypeDef,
     ListDevicesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("ListDeviceEventsPaginator", "ListDevicesPaginator")
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -53,30 +53,30 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/paginators/#listdeviceeventspaginator)
     """
 
     def paginate(
         self,
         *,
         DeviceId: str,
-        FromTimeStamp: Union[datetime, str],
-        ToTimeStamp: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        FromTimeStamp: TimestampTypeDef,
+        ToTimeStamp: TimestampTypeDef,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeviceEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/paginators/#listdeviceeventspaginator)
         """
 
 
 class ListDevicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/paginators/#listdevicespaginator)
     """
 
     def paginate(
-        self, *, DeviceType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DeviceType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/paginators/#listdevicespaginator)
         """
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/paginator.pyi` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/paginator.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -18,24 +18,24 @@
     with session.create_client("iot1click-devices") as client:
         client: IoT1ClickDevicesServiceClient
 
         list_device_events_paginator: ListDeviceEventsPaginator = client.get_paginator("list_device_events")
         list_devices_paginator: ListDevicesPaginator = client.get_paginator("list_devices")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ListDeviceEventsResponseTypeDef,
     ListDevicesResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("ListDeviceEventsPaginator", "ListDevicesPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -50,29 +50,29 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/paginators/#listdeviceeventspaginator)
     """
 
     def paginate(
         self,
         *,
         DeviceId: str,
-        FromTimeStamp: Union[datetime, str],
-        ToTimeStamp: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        FromTimeStamp: TimestampTypeDef,
+        ToTimeStamp: TimestampTypeDef,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeviceEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/paginators/#listdeviceeventspaginator)
         """
 
 class ListDevicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/paginators/#listdevicespaginator)
     """
 
     def paginate(
-        self, *, DeviceType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DeviceType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/paginators/#listdevicespaginator)
         """
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/type_defs.py` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -4,75 +4,77 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iot1click_devices.type_defs import ClaimDevicesByClaimCodeRequestRequestTypeDef
 
-    data: ClaimDevicesByClaimCodeRequestRequestTypeDef = {...}
+    data: ClaimDevicesByClaimCodeRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
-    "ClaimDevicesByClaimCodeResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "DeviceDescriptionTypeDef",
     "DeviceTypeDef",
     "DeviceMethodTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FinalizeDeviceClaimRequestRequestTypeDef",
-    "FinalizeDeviceClaimResponseTypeDef",
     "GetDeviceMethodsRequestRequestTypeDef",
     "InitiateDeviceClaimRequestRequestTypeDef",
-    "InitiateDeviceClaimResponseTypeDef",
-    "InvokeDeviceMethodResponseTypeDef",
-    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    "ListDeviceEventsRequestRequestTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
+    "TimestampTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnclaimDeviceRequestRequestTypeDef",
-    "UnclaimDeviceResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceStateRequestRequestTypeDef",
+    "ClaimDevicesByClaimCodeResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "FinalizeDeviceClaimResponseTypeDef",
+    "InitiateDeviceClaimResponseTypeDef",
+    "InvokeDeviceMethodResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UnclaimDeviceResponseTypeDef",
     "DescribeDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "DeviceEventTypeDef",
     "GetDeviceMethodsResponseTypeDef",
     "InvokeDeviceMethodRequestRequestTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    "ListDeviceEventsRequestRequestTypeDef",
     "ListDeviceEventsResponseTypeDef",
 )
 
 ClaimDevicesByClaimCodeRequestRequestTypeDef = TypedDict(
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
     {
         "ClaimCode": str,
     },
 )
 
-ClaimDevicesByClaimCodeResponseTypeDef = TypedDict(
-    "ClaimDevicesByClaimCodeResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ClaimCode": str,
-        "Total": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
@@ -108,138 +110,59 @@
     {
         "DeviceType": str,
         "MethodName": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFinalizeDeviceClaimRequestRequestTypeDef = TypedDict(
     "_RequiredFinalizeDeviceClaimRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 _OptionalFinalizeDeviceClaimRequestRequestTypeDef = TypedDict(
     "_OptionalFinalizeDeviceClaimRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class FinalizeDeviceClaimRequestRequestTypeDef(
     _RequiredFinalizeDeviceClaimRequestRequestTypeDef,
     _OptionalFinalizeDeviceClaimRequestRequestTypeDef,
 ):
     pass
 
-
-FinalizeDeviceClaimResponseTypeDef = TypedDict(
-    "FinalizeDeviceClaimResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDeviceMethodsRequestRequestTypeDef = TypedDict(
     "GetDeviceMethodsRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
 InitiateDeviceClaimRequestRequestTypeDef = TypedDict(
     "InitiateDeviceClaimRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-InitiateDeviceClaimResponseTypeDef = TypedDict(
-    "InitiateDeviceClaimResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-InvokeDeviceMethodResponseTypeDef = TypedDict(
-    "InvokeDeviceMethodResponseTypeDef",
-    {
-        "DeviceMethodResponse": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "FromTimeStamp": Union[datetime, str],
-        "ToTimeStamp": Union[datetime, str],
-    },
-)
-_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
-    _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDeviceEventsRequestRequestTypeDef",
-    {
-        "DeviceId": str,
-        "FromTimeStamp": Union[datetime, str],
-        "ToTimeStamp": Union[datetime, str],
-    },
-)
-_OptionalListDeviceEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDeviceEventsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class ListDeviceEventsRequestRequestTypeDef(
-    _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
-):
-    pass
-
-
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "DeviceType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "DeviceType": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -249,43 +172,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -293,22 +187,14 @@
 UnclaimDeviceRequestRequestTypeDef = TypedDict(
     "UnclaimDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-UnclaimDeviceResponseTypeDef = TypedDict(
-    "UnclaimDeviceResponseTypeDef",
-    {
-        "State": str,
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
@@ -323,35 +209,89 @@
     "_OptionalUpdateDeviceStateRequestRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-
 class UpdateDeviceStateRequestRequestTypeDef(
     _RequiredUpdateDeviceStateRequestRequestTypeDef, _OptionalUpdateDeviceStateRequestRequestTypeDef
 ):
     pass
 
+ClaimDevicesByClaimCodeResponseTypeDef = TypedDict(
+    "ClaimDevicesByClaimCodeResponseTypeDef",
+    {
+        "ClaimCode": str,
+        "Total": int,
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
+FinalizeDeviceClaimResponseTypeDef = TypedDict(
+    "FinalizeDeviceClaimResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateDeviceClaimResponseTypeDef = TypedDict(
+    "InitiateDeviceClaimResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InvokeDeviceMethodResponseTypeDef = TypedDict(
+    "InvokeDeviceMethodResponseTypeDef",
+    {
+        "DeviceMethodResponse": str,
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
+UnclaimDeviceResponseTypeDef = TypedDict(
+    "UnclaimDeviceResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 DescribeDeviceResponseTypeDef = TypedDict(
     "DescribeDeviceResponseTypeDef",
     {
         "DeviceDescription": DeviceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceEventTypeDef = TypedDict(
     "DeviceEventTypeDef",
     {
         "Device": DeviceTypeDef,
@@ -360,15 +300,15 @@
     total=False,
 )
 
 GetDeviceMethodsResponseTypeDef = TypedDict(
     "GetDeviceMethodsResponseTypeDef",
     {
         "DeviceMethods": List[DeviceMethodTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInvokeDeviceMethodRequestRequestTypeDef = TypedDict(
     "_RequiredInvokeDeviceMethodRequestRequestTypeDef",
     {
         "DeviceId": str,
@@ -379,23 +319,74 @@
     {
         "DeviceMethod": DeviceMethodTypeDef,
         "DeviceMethodParameters": str,
     },
     total=False,
 )
 
-
 class InvokeDeviceMethodRequestRequestTypeDef(
     _RequiredInvokeDeviceMethodRequestRequestTypeDef,
     _OptionalInvokeDeviceMethodRequestRequestTypeDef,
 ):
     pass
 
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "DeviceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    {
+        "DeviceId": str,
+        "FromTimeStamp": TimestampTypeDef,
+        "ToTimeStamp": TimestampTypeDef,
+    },
+)
+_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
+    _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+):
+    pass
+
+_RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDeviceEventsRequestRequestTypeDef",
+    {
+        "DeviceId": str,
+        "FromTimeStamp": TimestampTypeDef,
+        "ToTimeStamp": TimestampTypeDef,
+    },
+)
+_OptionalListDeviceEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDeviceEventsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListDeviceEventsRequestRequestTypeDef(
+    _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
+):
+    pass
 
 ListDeviceEventsResponseTypeDef = TypedDict(
     "ListDeviceEventsResponseTypeDef",
     {
         "Events": List[DeviceEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices/type_defs.pyi` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,74 +4,78 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iot1click_devices.type_defs import ClaimDevicesByClaimCodeRequestRequestTypeDef
 
-    data: ClaimDevicesByClaimCodeRequestRequestTypeDef = {...}
+    data: ClaimDevicesByClaimCodeRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
-    "ClaimDevicesByClaimCodeResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "DeviceDescriptionTypeDef",
     "DeviceTypeDef",
     "DeviceMethodTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FinalizeDeviceClaimRequestRequestTypeDef",
-    "FinalizeDeviceClaimResponseTypeDef",
     "GetDeviceMethodsRequestRequestTypeDef",
     "InitiateDeviceClaimRequestRequestTypeDef",
-    "InitiateDeviceClaimResponseTypeDef",
-    "InvokeDeviceMethodResponseTypeDef",
-    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    "ListDeviceEventsRequestRequestTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
+    "TimestampTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnclaimDeviceRequestRequestTypeDef",
-    "UnclaimDeviceResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceStateRequestRequestTypeDef",
+    "ClaimDevicesByClaimCodeResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "FinalizeDeviceClaimResponseTypeDef",
+    "InitiateDeviceClaimResponseTypeDef",
+    "InvokeDeviceMethodResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UnclaimDeviceResponseTypeDef",
     "DescribeDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "DeviceEventTypeDef",
     "GetDeviceMethodsResponseTypeDef",
     "InvokeDeviceMethodRequestRequestTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    "ListDeviceEventsRequestRequestTypeDef",
     "ListDeviceEventsResponseTypeDef",
 )
 
 ClaimDevicesByClaimCodeRequestRequestTypeDef = TypedDict(
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
     {
         "ClaimCode": str,
     },
 )
 
-ClaimDevicesByClaimCodeResponseTypeDef = TypedDict(
-    "ClaimDevicesByClaimCodeResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ClaimCode": str,
-        "Total": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
@@ -107,48 +111,35 @@
     {
         "DeviceType": str,
         "MethodName": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFinalizeDeviceClaimRequestRequestTypeDef = TypedDict(
     "_RequiredFinalizeDeviceClaimRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 _OptionalFinalizeDeviceClaimRequestRequestTypeDef = TypedDict(
     "_OptionalFinalizeDeviceClaimRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class FinalizeDeviceClaimRequestRequestTypeDef(
     _RequiredFinalizeDeviceClaimRequestRequestTypeDef,
     _OptionalFinalizeDeviceClaimRequestRequestTypeDef,
 ):
     pass
 
-FinalizeDeviceClaimResponseTypeDef = TypedDict(
-    "FinalizeDeviceClaimResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetDeviceMethodsRequestRequestTypeDef = TypedDict(
     "GetDeviceMethodsRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
@@ -156,83 +147,25 @@
 InitiateDeviceClaimRequestRequestTypeDef = TypedDict(
     "InitiateDeviceClaimRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-InitiateDeviceClaimResponseTypeDef = TypedDict(
-    "InitiateDeviceClaimResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-InvokeDeviceMethodResponseTypeDef = TypedDict(
-    "InvokeDeviceMethodResponseTypeDef",
-    {
-        "DeviceMethodResponse": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "FromTimeStamp": Union[datetime, str],
-        "ToTimeStamp": Union[datetime, str],
-    },
-)
-_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
-    _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-):
-    pass
-
-_RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDeviceEventsRequestRequestTypeDef",
-    {
-        "DeviceId": str,
-        "FromTimeStamp": Union[datetime, str],
-        "ToTimeStamp": Union[datetime, str],
-    },
-)
-_OptionalListDeviceEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDeviceEventsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class ListDeviceEventsRequestRequestTypeDef(
-    _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
-):
-    pass
-
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "DeviceType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "DeviceType": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -242,43 +175,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -286,22 +190,14 @@
 UnclaimDeviceRequestRequestTypeDef = TypedDict(
     "UnclaimDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-UnclaimDeviceResponseTypeDef = TypedDict(
-    "UnclaimDeviceResponseTypeDef",
-    {
-        "State": str,
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
@@ -316,33 +212,91 @@
     "_OptionalUpdateDeviceStateRequestRequestTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
+
 class UpdateDeviceStateRequestRequestTypeDef(
     _RequiredUpdateDeviceStateRequestRequestTypeDef, _OptionalUpdateDeviceStateRequestRequestTypeDef
 ):
     pass
 
+
+ClaimDevicesByClaimCodeResponseTypeDef = TypedDict(
+    "ClaimDevicesByClaimCodeResponseTypeDef",
+    {
+        "ClaimCode": str,
+        "Total": int,
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
+FinalizeDeviceClaimResponseTypeDef = TypedDict(
+    "FinalizeDeviceClaimResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateDeviceClaimResponseTypeDef = TypedDict(
+    "InitiateDeviceClaimResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InvokeDeviceMethodResponseTypeDef = TypedDict(
+    "InvokeDeviceMethodResponseTypeDef",
+    {
+        "DeviceMethodResponse": str,
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
+UnclaimDeviceResponseTypeDef = TypedDict(
+    "UnclaimDeviceResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeDeviceResponseTypeDef = TypedDict(
     "DescribeDeviceResponseTypeDef",
     {
         "DeviceDescription": DeviceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceEventTypeDef = TypedDict(
     "DeviceEventTypeDef",
     {
         "Device": DeviceTypeDef,
@@ -351,15 +305,15 @@
     total=False,
 )
 
 GetDeviceMethodsResponseTypeDef = TypedDict(
     "GetDeviceMethodsResponseTypeDef",
     {
         "DeviceMethods": List[DeviceMethodTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInvokeDeviceMethodRequestRequestTypeDef = TypedDict(
     "_RequiredInvokeDeviceMethodRequestRequestTypeDef",
     {
         "DeviceId": str,
@@ -370,21 +324,80 @@
     {
         "DeviceMethod": DeviceMethodTypeDef,
         "DeviceMethodParameters": str,
     },
     total=False,
 )
 
+
 class InvokeDeviceMethodRequestRequestTypeDef(
     _RequiredInvokeDeviceMethodRequestRequestTypeDef,
     _OptionalInvokeDeviceMethodRequestRequestTypeDef,
 ):
     pass
 
+
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "DeviceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    {
+        "DeviceId": str,
+        "FromTimeStamp": TimestampTypeDef,
+        "ToTimeStamp": TimestampTypeDef,
+    },
+)
+_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
+    _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDeviceEventsRequestRequestTypeDef",
+    {
+        "DeviceId": str,
+        "FromTimeStamp": TimestampTypeDef,
+        "ToTimeStamp": TimestampTypeDef,
+    },
+)
+_OptionalListDeviceEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDeviceEventsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListDeviceEventsRequestRequestTypeDef(
+    _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
+):
+    pass
+
+
 ListDeviceEventsResponseTypeDef = TypedDict(
     "ListDeviceEventsResponseTypeDef",
     {
         "Events": List[DeviceEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices.egg-info/PKG-INFO` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-devices
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoT1ClickDevicesService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoT1ClickDevicesService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iot1click-devices type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iot1click-devices type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iot1click-devices"></a>
 
 # types-aiobotocore-iot1click-devices
 
 [![PyPI - types-aiobotocore-iot1click-devices](https://img.shields.io/pypi/v/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iot1click-devices.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iot1click-devices?color=blue)](https://pypistats.org/packages/types-aiobotocore-iot1click-devices)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iot1click-devices)](https://pepy.tech/project/types-aiobotocore-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoT1ClickDevicesService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [types-aiobotocore-iot1click-devices docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_devices/).
 
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
@@ -311,59 +310,60 @@
 )
 
 
 def check_value(value: ListDeviceEventsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iot1click_devices.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
-    ClaimDevicesByClaimCodeResponseTypeDef,
+    ResponseMetadataTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
     DeviceMethodTypeDef,
-    EmptyResponseMetadataTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
-    FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
-    InitiateDeviceClaimResponseTypeDef,
-    InvokeDeviceMethodResponseTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    ListDeviceEventsRequestRequestTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
+    PaginatorConfigTypeDef,
+    TimestampTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UnclaimDeviceRequestRequestTypeDef,
-    UnclaimDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceStateRequestRequestTypeDef,
+    ClaimDevicesByClaimCodeResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FinalizeDeviceClaimResponseTypeDef,
+    InitiateDeviceClaimResponseTypeDef,
+    InvokeDeviceMethodResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UnclaimDeviceResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     DeviceEventTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InvokeDeviceMethodRequestRequestTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
+    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    ListDeviceEventsRequestRequestTypeDef,
     ListDeviceEventsResponseTypeDef,
 )
 
 
-def get_structure() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
+def get_value() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iot1click-devices-2.5.2/types_aiobotocore_iot1click_devices.egg-info/SOURCES.txt` & `types-aiobotocore-iot1click-devices-2.5.2.post1/types_aiobotocore_iot1click_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*


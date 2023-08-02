# Comparing `tmp/types-aiobotocore-internetmonitor-2.5.2.tar.gz` & `tmp/types-aiobotocore-internetmonitor-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-internetmonitor-2.5.2.tar", last modified: Sat Jul  8 01:43:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-internetmonitor-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
```

## Comparing `types-aiobotocore-internetmonitor-2.5.2.tar` & `types-aiobotocore-internetmonitor-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.534262 types-aiobotocore-internetmonitor-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:19.000000 types-aiobotocore-internetmonitor-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-07-08 01:43:44.530262 types-aiobotocore-internetmonitor-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-08 01:32:19.000000 types-aiobotocore-internetmonitor-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:44.534262 types-aiobotocore-internetmonitor-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-08 01:32:19.000000 types-aiobotocore-internetmonitor-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.522261 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-08 01:32:19.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-08 01:32:19.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-08 01:32:19.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-07-08 01:32:20.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-07-08 01:32:19.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-07-08 01:32:20.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-08 01:32:20.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-08 01:32:20.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-07-08 01:32:20.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:19.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12156 2023-07-08 01:32:20.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-07-08 01:32:20.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:19.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.530262 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-07-08 01:43:44.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-08 01:43:44.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:44.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:44.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:44.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-08 01:43:44.000000 types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.341569 types-aiobotocore-internetmonitor-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-08-02 14:52:24.341569 types-aiobotocore-internetmonitor-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13196 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.341569 types-aiobotocore-internetmonitor-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.337569 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-08-02 14:40:20.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:19.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.341569 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14756 2023-08-02 14:52:24.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:52:24.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:24.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:24.000000 types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2/LICENSE` & `types-aiobotocore-internetmonitor-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2/PKG-INFO` & `types-aiobotocore-internetmonitor-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-internetmonitor
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore internetmonitor type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore internetmonitor type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-internetmonitor"></a>
 
 # types-aiobotocore-internetmonitor
 
 [![PyPI - types-aiobotocore-internetmonitor](https://img.shields.io/pypi/v/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-internetmonitor?color=blue)](https://pypistats.org/packages/types-aiobotocore-internetmonitor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-internetmonitor)](https://pepy.tech/project/types-aiobotocore-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudWatchInternetMonitor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
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
 [types-aiobotocore-internetmonitor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/).
 
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
@@ -318,59 +317,60 @@
 )
 
 
 def check_value(value: HealthEventImpactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_internetmonitor.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
-    CreateMonitorOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
     S3ConfigTypeDef,
-    ListHealthEventsInputListHealthEventsPaginateTypeDef,
-    ListHealthEventsInputRequestTypeDef,
-    ListMonitorsInputListMonitorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
+    TimestampTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     NetworkTypeDef,
-    PaginatorConfigTypeDef,
     RoundTripTimeTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    CreateMonitorOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
+    ListMonitorsInputListMonitorsPaginateTypeDef,
+    ListHealthEventsInputListHealthEventsPaginateTypeDef,
+    ListHealthEventsInputRequestTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
     CreateMonitorInputRequestTypeDef,
     GetMonitorOutputTypeDef,
     UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
 
 
-def get_structure() -> AvailabilityMeasurementTypeDef:
+def get_value() -> AvailabilityMeasurementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2/README.md` & `types-aiobotocore-internetmonitor-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-internetmonitor"></a>
 
 # types-aiobotocore-internetmonitor
 
 [![PyPI - types-aiobotocore-internetmonitor](https://img.shields.io/pypi/v/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-internetmonitor?color=blue)](https://pypistats.org/packages/types-aiobotocore-internetmonitor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-internetmonitor)](https://pepy.tech/project/types-aiobotocore-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudWatchInternetMonitor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
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
 [types-aiobotocore-internetmonitor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/).
 
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
@@ -285,59 +285,60 @@
 )
 
 
 def check_value(value: HealthEventImpactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_internetmonitor.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
-    CreateMonitorOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
     S3ConfigTypeDef,
-    ListHealthEventsInputListHealthEventsPaginateTypeDef,
-    ListHealthEventsInputRequestTypeDef,
-    ListMonitorsInputListMonitorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
+    TimestampTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     NetworkTypeDef,
-    PaginatorConfigTypeDef,
     RoundTripTimeTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    CreateMonitorOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
+    ListMonitorsInputListMonitorsPaginateTypeDef,
+    ListHealthEventsInputListHealthEventsPaginateTypeDef,
+    ListHealthEventsInputRequestTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
     CreateMonitorInputRequestTypeDef,
     GetMonitorOutputTypeDef,
     UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
 
 
-def get_structure() -> AvailabilityMeasurementTypeDef:
+def get_value() -> AvailabilityMeasurementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2/setup.py` & `types-aiobotocore-internetmonitor-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-internetmonitor",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_internetmonitor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with"
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
-    keywords="aiobotocore internetmonitor type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore internetmonitor type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_internetmonitor": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/"
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/__init__.py` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/__init__.pyi` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/__main__.py` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor\nOther"
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

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/client.py` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 
     session = get_session()
     async with session.create_client("internetmonitor") as client:
         client: CloudWatchInternetMonitorClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import HealthEventStatusType, MonitorConfigStateType
 from .paginator import ListHealthEventsPaginator, ListMonitorsPaginator
 from .type_defs import (
     CreateMonitorOutputTypeDef,
     GetHealthEventOutputTypeDef,
     GetMonitorOutputTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
     ListHealthEventsOutputTypeDef,
     ListMonitorsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    TimestampTypeDef,
     UpdateMonitorOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -159,16 +159,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/client/#get_monitor)
         """
 
     async def list_health_events(
         self,
         *,
         MonitorName: str,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         EventStatus: HealthEventStatusType = ...
     ) -> ListHealthEventsOutputTypeDef:
         """
         Lists all health events for a monitor in Amazon CloudWatch Internet Monitor.
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/client.pyi` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 
     session = get_session()
     async with session.create_client("internetmonitor") as client:
         client: CloudWatchInternetMonitorClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import HealthEventStatusType, MonitorConfigStateType
 from .paginator import ListHealthEventsPaginator, ListMonitorsPaginator
 from .type_defs import (
     CreateMonitorOutputTypeDef,
     GetHealthEventOutputTypeDef,
     GetMonitorOutputTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
     ListHealthEventsOutputTypeDef,
     ListMonitorsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    TimestampTypeDef,
     UpdateMonitorOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -147,16 +147,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.get_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/client/#get_monitor)
         """
     async def list_health_events(
         self,
         *,
         MonitorName: str,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         EventStatus: HealthEventStatusType = ...
     ) -> ListHealthEventsOutputTypeDef:
         """
         Lists all health events for a monitor in Amazon CloudWatch Internet Monitor.
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/literals.py` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/literals.pyi` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/paginator.py` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,25 +18,25 @@
     with session.create_client("internetmonitor") as client:
         client: CloudWatchInternetMonitorClient
 
         list_health_events_paginator: ListHealthEventsPaginator = client.get_paginator("list_health_events")
         list_monitors_paginator: ListMonitorsPaginator = client.get_paginator("list_monitors")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import HealthEventStatusType
 from .type_defs import (
     ListHealthEventsOutputTypeDef,
     ListMonitorsOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("ListHealthEventsPaginator", "ListMonitorsPaginator")
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -54,31 +54,31 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/paginators/#listhealtheventspaginator)
     """
 
     def paginate(
         self,
         *,
         MonitorName: str,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventStatus: HealthEventStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHealthEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListHealthEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/paginators/#listhealtheventspaginator)
         """
 
 
 class ListMonitorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListMonitors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/paginators/#listmonitorspaginator)
     """
 
     def paginate(
-        self, *, MonitorStatus: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, MonitorStatus: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMonitorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListMonitors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/paginators/#listmonitorspaginator)
         """
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/paginator.pyi` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/paginator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -18,25 +18,25 @@
     with session.create_client("internetmonitor") as client:
         client: CloudWatchInternetMonitorClient
 
         list_health_events_paginator: ListHealthEventsPaginator = client.get_paginator("list_health_events")
         list_monitors_paginator: ListMonitorsPaginator = client.get_paginator("list_monitors")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import HealthEventStatusType
 from .type_defs import (
     ListHealthEventsOutputTypeDef,
     ListMonitorsOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("ListHealthEventsPaginator", "ListMonitorsPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -51,30 +51,30 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/paginators/#listhealtheventspaginator)
     """
 
     def paginate(
         self,
         *,
         MonitorName: str,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventStatus: HealthEventStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHealthEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListHealthEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/paginators/#listhealtheventspaginator)
         """
 
 class ListMonitorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListMonitors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/paginators/#listmonitorspaginator)
     """
 
     def paginate(
-        self, *, MonitorStatus: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, MonitorStatus: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMonitorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Paginator.ListMonitors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/paginators/#listmonitorspaginator)
         """
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/type_defs.py` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_internetmonitor.type_defs import AvailabilityMeasurementTypeDef
 
-    data: AvailabilityMeasurementTypeDef = {...}
+    data: AvailabilityMeasurementTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -25,37 +25,37 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AvailabilityMeasurementTypeDef",
-    "CreateMonitorOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
     "S3ConfigTypeDef",
-    "ListHealthEventsInputListHealthEventsPaginateTypeDef",
-    "ListHealthEventsInputRequestTypeDef",
-    "ListMonitorsInputListMonitorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
+    "TimestampTypeDef",
     "ListMonitorsInputRequestTypeDef",
     "MonitorTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "NetworkTypeDef",
-    "PaginatorConfigTypeDef",
     "RoundTripTimeTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "CreateMonitorOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "UpdateMonitorOutputTypeDef",
     "InternetMeasurementsLogDeliveryTypeDef",
+    "ListMonitorsInputListMonitorsPaginateTypeDef",
+    "ListHealthEventsInputListHealthEventsPaginateTypeDef",
+    "ListHealthEventsInputRequestTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
     "CreateMonitorInputRequestTypeDef",
     "GetMonitorOutputTypeDef",
     "UpdateMonitorInputRequestTypeDef",
     "InternetHealthTypeDef",
@@ -71,20 +71,22 @@
         "ExperienceScore": float,
         "PercentOfTotalTrafficImpacted": float,
         "PercentOfClientLocationImpacted": float,
     },
     total=False,
 )
 
-CreateMonitorOutputTypeDef = TypedDict(
-    "CreateMonitorOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "Status": MonitorConfigStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteMonitorInputRequestTypeDef = TypedDict(
     "DeleteMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
@@ -112,73 +114,25 @@
         "BucketName": str,
         "BucketPrefix": str,
         "LogDeliveryStatus": LogDeliveryStatusType,
     },
     total=False,
 )
 
-_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
-    "_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef",
-    {
-        "MonitorName": str,
-    },
-)
-_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
-    "_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "EventStatus": HealthEventStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListHealthEventsInputListHealthEventsPaginateTypeDef(
-    _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef,
-    _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListHealthEventsInputRequestTypeDef = TypedDict(
-    "_RequiredListHealthEventsInputRequestTypeDef",
-    {
-        "MonitorName": str,
-    },
-)
-_OptionalListHealthEventsInputRequestTypeDef = TypedDict(
-    "_OptionalListHealthEventsInputRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-        "EventStatus": HealthEventStatusType,
-    },
-    total=False,
-)
-
-
-class ListHealthEventsInputRequestTypeDef(
-    _RequiredListHealthEventsInputRequestTypeDef, _OptionalListHealthEventsInputRequestTypeDef
-):
-    pass
-
-
-ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
-    "ListMonitorsInputListMonitorsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "MonitorStatus": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 ListMonitorsInputRequestTypeDef = TypedDict(
     "ListMonitorsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "MonitorStatus": str,
     },
@@ -197,73 +151,42 @@
     "_OptionalMonitorTypeDef",
     {
         "ProcessingStatus": MonitorProcessingStatusCodeType,
     },
     total=False,
 )
 
-
 class MonitorTypeDef(_RequiredMonitorTypeDef, _OptionalMonitorTypeDef):
     pass
 
-
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NetworkTypeDef = TypedDict(
     "NetworkTypeDef",
     {
         "ASName": str,
         "ASNumber": int,
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
 RoundTripTimeTypeDef = TypedDict(
     "RoundTripTimeTypeDef",
     {
         "P50": float,
         "P90": float,
         "P95": float,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -272,37 +195,109 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+CreateMonitorOutputTypeDef = TypedDict(
+    "CreateMonitorOutputTypeDef",
+    {
+        "Arn": str,
+        "Status": MonitorConfigStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateMonitorOutputTypeDef = TypedDict(
     "UpdateMonitorOutputTypeDef",
     {
         "MonitorArn": str,
         "Status": MonitorConfigStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InternetMeasurementsLogDeliveryTypeDef = TypedDict(
     "InternetMeasurementsLogDeliveryTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
     total=False,
 )
 
+ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
+    "ListMonitorsInputListMonitorsPaginateTypeDef",
+    {
+        "MonitorStatus": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
+    "_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef",
+    {
+        "MonitorName": str,
+    },
+)
+_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
+    "_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "EventStatus": HealthEventStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListHealthEventsInputListHealthEventsPaginateTypeDef(
+    _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef,
+    _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef,
+):
+    pass
+
+_RequiredListHealthEventsInputRequestTypeDef = TypedDict(
+    "_RequiredListHealthEventsInputRequestTypeDef",
+    {
+        "MonitorName": str,
+    },
+)
+_OptionalListHealthEventsInputRequestTypeDef = TypedDict(
+    "_OptionalListHealthEventsInputRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+        "EventStatus": HealthEventStatusType,
+    },
+    total=False,
+)
+
+class ListHealthEventsInputRequestTypeDef(
+    _RequiredListHealthEventsInputRequestTypeDef, _OptionalListHealthEventsInputRequestTypeDef
+):
+    pass
+
 ListMonitorsOutputTypeDef = TypedDict(
     "ListMonitorsOutputTypeDef",
     {
         "Monitors": List[MonitorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkImpairmentTypeDef = TypedDict(
     "NetworkImpairmentTypeDef",
     {
         "Networks": List[NetworkTypeDef],
@@ -337,21 +332,19 @@
         "MaxCityNetworksToMonitor": int,
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
     },
     total=False,
 )
 
-
 class CreateMonitorInputRequestTypeDef(
     _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
 ):
     pass
 
-
 GetMonitorOutputTypeDef = TypedDict(
     "GetMonitorOutputTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "Resources": List[str],
         "Status": MonitorConfigStateType,
@@ -359,15 +352,15 @@
         "ModifiedAt": datetime,
         "ProcessingStatus": MonitorProcessingStatusCodeType,
         "ProcessingStatusInfo": str,
         "Tags": Dict[str, str],
         "MaxCityNetworksToMonitor": int,
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateMonitorInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
@@ -383,21 +376,19 @@
         "MaxCityNetworksToMonitor": int,
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
     },
     total=False,
 )
 
-
 class UpdateMonitorInputRequestTypeDef(
     _RequiredUpdateMonitorInputRequestTypeDef, _OptionalUpdateMonitorInputRequestTypeDef
 ):
     pass
 
-
 InternetHealthTypeDef = TypedDict(
     "InternetHealthTypeDef",
     {
         "Availability": AvailabilityMeasurementTypeDef,
         "Performance": PerformanceMeasurementTypeDef,
     },
     total=False,
@@ -425,33 +416,31 @@
         "ServiceLocation": str,
         "CausedBy": NetworkImpairmentTypeDef,
         "InternetHealth": InternetHealthTypeDef,
     },
     total=False,
 )
 
-
 class ImpactedLocationTypeDef(_RequiredImpactedLocationTypeDef, _OptionalImpactedLocationTypeDef):
     pass
 
-
 GetHealthEventOutputTypeDef = TypedDict(
     "GetHealthEventOutputTypeDef",
     {
         "EventArn": str,
         "EventId": str,
         "StartedAt": datetime,
         "EndedAt": datetime,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "ImpactedLocations": List[ImpactedLocationTypeDef],
         "Status": HealthEventStatusType,
         "PercentOfTotalTrafficImpacted": float,
         "ImpactType": HealthEventImpactTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHealthEventTypeDef = TypedDict(
     "_RequiredHealthEventTypeDef",
     {
         "EventArn": str,
@@ -469,20 +458,18 @@
         "EndedAt": datetime,
         "CreatedAt": datetime,
         "PercentOfTotalTrafficImpacted": float,
     },
     total=False,
 )
 
-
 class HealthEventTypeDef(_RequiredHealthEventTypeDef, _OptionalHealthEventTypeDef):
     pass
 
-
 ListHealthEventsOutputTypeDef = TypedDict(
     "ListHealthEventsOutputTypeDef",
     {
         "HealthEvents": List[HealthEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor/type_defs.pyi` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_internetmonitor.type_defs import AvailabilityMeasurementTypeDef
 
-    data: AvailabilityMeasurementTypeDef = {...}
+    data: AvailabilityMeasurementTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -25,36 +25,38 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AvailabilityMeasurementTypeDef",
-    "CreateMonitorOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteMonitorInputRequestTypeDef",
     "GetHealthEventInputRequestTypeDef",
     "GetMonitorInputRequestTypeDef",
     "S3ConfigTypeDef",
-    "ListHealthEventsInputListHealthEventsPaginateTypeDef",
-    "ListHealthEventsInputRequestTypeDef",
-    "ListMonitorsInputListMonitorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
+    "TimestampTypeDef",
     "ListMonitorsInputRequestTypeDef",
     "MonitorTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "NetworkTypeDef",
-    "PaginatorConfigTypeDef",
     "RoundTripTimeTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
+    "CreateMonitorOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "UpdateMonitorOutputTypeDef",
     "InternetMeasurementsLogDeliveryTypeDef",
+    "ListMonitorsInputListMonitorsPaginateTypeDef",
+    "ListHealthEventsInputListHealthEventsPaginateTypeDef",
+    "ListHealthEventsInputRequestTypeDef",
     "ListMonitorsOutputTypeDef",
     "NetworkImpairmentTypeDef",
     "PerformanceMeasurementTypeDef",
     "CreateMonitorInputRequestTypeDef",
     "GetMonitorOutputTypeDef",
     "UpdateMonitorInputRequestTypeDef",
     "InternetHealthTypeDef",
@@ -70,20 +72,22 @@
         "ExperienceScore": float,
         "PercentOfTotalTrafficImpacted": float,
         "PercentOfClientLocationImpacted": float,
     },
     total=False,
 )
 
-CreateMonitorOutputTypeDef = TypedDict(
-    "CreateMonitorOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "Status": MonitorConfigStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteMonitorInputRequestTypeDef = TypedDict(
     "DeleteMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
@@ -111,69 +115,25 @@
         "BucketName": str,
         "BucketPrefix": str,
         "LogDeliveryStatus": LogDeliveryStatusType,
     },
     total=False,
 )
 
-_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
-    "_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef",
-    {
-        "MonitorName": str,
-    },
-)
-_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
-    "_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "EventStatus": HealthEventStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListHealthEventsInputListHealthEventsPaginateTypeDef(
-    _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef,
-    _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef,
-):
-    pass
-
-_RequiredListHealthEventsInputRequestTypeDef = TypedDict(
-    "_RequiredListHealthEventsInputRequestTypeDef",
-    {
-        "MonitorName": str,
-    },
-)
-_OptionalListHealthEventsInputRequestTypeDef = TypedDict(
-    "_OptionalListHealthEventsInputRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-        "EventStatus": HealthEventStatusType,
-    },
-    total=False,
-)
-
-class ListHealthEventsInputRequestTypeDef(
-    _RequiredListHealthEventsInputRequestTypeDef, _OptionalListHealthEventsInputRequestTypeDef
-):
-    pass
-
-ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
-    "ListMonitorsInputListMonitorsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "MonitorStatus": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 ListMonitorsInputRequestTypeDef = TypedDict(
     "ListMonitorsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "MonitorStatus": str,
     },
@@ -192,71 +152,44 @@
     "_OptionalMonitorTypeDef",
     {
         "ProcessingStatus": MonitorProcessingStatusCodeType,
     },
     total=False,
 )
 
+
 class MonitorTypeDef(_RequiredMonitorTypeDef, _OptionalMonitorTypeDef):
     pass
 
+
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NetworkTypeDef = TypedDict(
     "NetworkTypeDef",
     {
         "ASName": str,
         "ASNumber": int,
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
 RoundTripTimeTypeDef = TypedDict(
     "RoundTripTimeTypeDef",
     {
         "P50": float,
         "P90": float,
         "P95": float,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -265,37 +198,113 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+CreateMonitorOutputTypeDef = TypedDict(
+    "CreateMonitorOutputTypeDef",
+    {
+        "Arn": str,
+        "Status": MonitorConfigStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateMonitorOutputTypeDef = TypedDict(
     "UpdateMonitorOutputTypeDef",
     {
         "MonitorArn": str,
         "Status": MonitorConfigStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InternetMeasurementsLogDeliveryTypeDef = TypedDict(
     "InternetMeasurementsLogDeliveryTypeDef",
     {
         "S3Config": S3ConfigTypeDef,
     },
     total=False,
 )
 
+ListMonitorsInputListMonitorsPaginateTypeDef = TypedDict(
+    "ListMonitorsInputListMonitorsPaginateTypeDef",
+    {
+        "MonitorStatus": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
+    "_RequiredListHealthEventsInputListHealthEventsPaginateTypeDef",
+    {
+        "MonitorName": str,
+    },
+)
+_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef = TypedDict(
+    "_OptionalListHealthEventsInputListHealthEventsPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "EventStatus": HealthEventStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListHealthEventsInputListHealthEventsPaginateTypeDef(
+    _RequiredListHealthEventsInputListHealthEventsPaginateTypeDef,
+    _OptionalListHealthEventsInputListHealthEventsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListHealthEventsInputRequestTypeDef = TypedDict(
+    "_RequiredListHealthEventsInputRequestTypeDef",
+    {
+        "MonitorName": str,
+    },
+)
+_OptionalListHealthEventsInputRequestTypeDef = TypedDict(
+    "_OptionalListHealthEventsInputRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+        "EventStatus": HealthEventStatusType,
+    },
+    total=False,
+)
+
+
+class ListHealthEventsInputRequestTypeDef(
+    _RequiredListHealthEventsInputRequestTypeDef, _OptionalListHealthEventsInputRequestTypeDef
+):
+    pass
+
+
 ListMonitorsOutputTypeDef = TypedDict(
     "ListMonitorsOutputTypeDef",
     {
         "Monitors": List[MonitorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkImpairmentTypeDef = TypedDict(
     "NetworkImpairmentTypeDef",
     {
         "Networks": List[NetworkTypeDef],
@@ -330,19 +339,21 @@
         "MaxCityNetworksToMonitor": int,
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
     },
     total=False,
 )
 
+
 class CreateMonitorInputRequestTypeDef(
     _RequiredCreateMonitorInputRequestTypeDef, _OptionalCreateMonitorInputRequestTypeDef
 ):
     pass
 
+
 GetMonitorOutputTypeDef = TypedDict(
     "GetMonitorOutputTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "Resources": List[str],
         "Status": MonitorConfigStateType,
@@ -350,15 +361,15 @@
         "ModifiedAt": datetime,
         "ProcessingStatus": MonitorProcessingStatusCodeType,
         "ProcessingStatusInfo": str,
         "Tags": Dict[str, str],
         "MaxCityNetworksToMonitor": int,
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateMonitorInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMonitorInputRequestTypeDef",
     {
         "MonitorName": str,
@@ -374,19 +385,21 @@
         "MaxCityNetworksToMonitor": int,
         "InternetMeasurementsLogDelivery": InternetMeasurementsLogDeliveryTypeDef,
         "TrafficPercentageToMonitor": int,
     },
     total=False,
 )
 
+
 class UpdateMonitorInputRequestTypeDef(
     _RequiredUpdateMonitorInputRequestTypeDef, _OptionalUpdateMonitorInputRequestTypeDef
 ):
     pass
 
+
 InternetHealthTypeDef = TypedDict(
     "InternetHealthTypeDef",
     {
         "Availability": AvailabilityMeasurementTypeDef,
         "Performance": PerformanceMeasurementTypeDef,
     },
     total=False,
@@ -414,31 +427,33 @@
         "ServiceLocation": str,
         "CausedBy": NetworkImpairmentTypeDef,
         "InternetHealth": InternetHealthTypeDef,
     },
     total=False,
 )
 
+
 class ImpactedLocationTypeDef(_RequiredImpactedLocationTypeDef, _OptionalImpactedLocationTypeDef):
     pass
 
+
 GetHealthEventOutputTypeDef = TypedDict(
     "GetHealthEventOutputTypeDef",
     {
         "EventArn": str,
         "EventId": str,
         "StartedAt": datetime,
         "EndedAt": datetime,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "ImpactedLocations": List[ImpactedLocationTypeDef],
         "Status": HealthEventStatusType,
         "PercentOfTotalTrafficImpacted": float,
         "ImpactType": HealthEventImpactTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHealthEventTypeDef = TypedDict(
     "_RequiredHealthEventTypeDef",
     {
         "EventArn": str,
@@ -456,18 +471,20 @@
         "EndedAt": datetime,
         "CreatedAt": datetime,
         "PercentOfTotalTrafficImpacted": float,
     },
     total=False,
 )
 
+
 class HealthEventTypeDef(_RequiredHealthEventTypeDef, _OptionalHealthEventTypeDef):
     pass
 
+
 ListHealthEventsOutputTypeDef = TypedDict(
     "ListHealthEventsOutputTypeDef",
     {
         "HealthEvents": List[HealthEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor.egg-info/PKG-INFO` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-internetmonitor
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudWatchInternetMonitor 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore internetmonitor type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore internetmonitor type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-internetmonitor"></a>
 
 # types-aiobotocore-internetmonitor
 
 [![PyPI - types-aiobotocore-internetmonitor](https://img.shields.io/pypi/v/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-internetmonitor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-internetmonitor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-internetmonitor?color=blue)](https://pypistats.org/packages/types-aiobotocore-internetmonitor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-internetmonitor)](https://pepy.tech/project/types-aiobotocore-internetmonitor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudWatchInternetMonitor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
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
 [types-aiobotocore-internetmonitor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_internetmonitor/).
 
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
@@ -318,59 +317,60 @@
 )
 
 
 def check_value(value: HealthEventImpactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_internetmonitor.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_internetmonitor.type_defs import (
     AvailabilityMeasurementTypeDef,
-    CreateMonitorOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeleteMonitorInputRequestTypeDef,
     GetHealthEventInputRequestTypeDef,
     GetMonitorInputRequestTypeDef,
     S3ConfigTypeDef,
-    ListHealthEventsInputListHealthEventsPaginateTypeDef,
-    ListHealthEventsInputRequestTypeDef,
-    ListMonitorsInputListMonitorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
+    TimestampTypeDef,
     ListMonitorsInputRequestTypeDef,
     MonitorTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     NetworkTypeDef,
-    PaginatorConfigTypeDef,
     RoundTripTimeTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
+    CreateMonitorOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     UpdateMonitorOutputTypeDef,
     InternetMeasurementsLogDeliveryTypeDef,
+    ListMonitorsInputListMonitorsPaginateTypeDef,
+    ListHealthEventsInputListHealthEventsPaginateTypeDef,
+    ListHealthEventsInputRequestTypeDef,
     ListMonitorsOutputTypeDef,
     NetworkImpairmentTypeDef,
     PerformanceMeasurementTypeDef,
     CreateMonitorInputRequestTypeDef,
     GetMonitorOutputTypeDef,
     UpdateMonitorInputRequestTypeDef,
     InternetHealthTypeDef,
     ImpactedLocationTypeDef,
     GetHealthEventOutputTypeDef,
     HealthEventTypeDef,
     ListHealthEventsOutputTypeDef,
 )
 
 
-def get_structure() -> AvailabilityMeasurementTypeDef:
+def get_value() -> AvailabilityMeasurementTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-internetmonitor-2.5.2/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt` & `types-aiobotocore-internetmonitor-2.5.2.post1/types_aiobotocore_internetmonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*


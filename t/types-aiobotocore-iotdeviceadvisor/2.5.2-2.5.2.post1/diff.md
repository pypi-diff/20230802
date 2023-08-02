# Comparing `tmp/types-aiobotocore-iotdeviceadvisor-2.5.2.tar.gz` & `tmp/types-aiobotocore-iotdeviceadvisor-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotdeviceadvisor-2.5.2.tar", last modified: Sat Jul  8 01:43:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotdeviceadvisor-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
```

## Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2.tar` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.642301 types-aiobotocore-iotdeviceadvisor-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:40.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-07-08 01:43:46.634301 types-aiobotocore-iotdeviceadvisor-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12310 2023-07-08 01:32:40.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:46.642301 types-aiobotocore-iotdeviceadvisor-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-08 01:32:40.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.634301 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-08 01:32:40.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-08 01:32:40.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-08 01:32:40.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-07-08 01:32:40.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-07-08 01:32:40.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-07-08 01:32:40.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-08 01:32:40.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:40.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-07-08 01:32:42.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12323 2023-07-08 01:32:41.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:40.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.634301 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-07-08 01:43:46.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-08 01:43:46.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:46.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 01:43:46.000000 types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.549563 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-08-02 14:52:26.549563 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.549563 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.549563 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12966 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13985 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:43.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.549563 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-08-02 14:52:26.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 14:52:26.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:26.000000 types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/LICENSE` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/PKG-INFO` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotdeviceadvisor
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotdeviceadvisor type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotdeviceadvisor type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotdeviceadvisor"></a>
 
 # types-aiobotocore-iotdeviceadvisor
 
 [![PyPI - types-aiobotocore-iotdeviceadvisor](https://img.shields.io/pypi/v/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotdeviceadvisor?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotdeviceadvisor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotdeviceadvisor)](https://pepy.tech/project/types-aiobotocore-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTDeviceAdvisor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [types-aiobotocore-iotdeviceadvisor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/).
 
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
@@ -286,61 +285,65 @@
 )
 
 
 def check_value(value: AuthenticationMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotdeviceadvisor.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotdeviceadvisor.type_defs import (
-    CreateSuiteDefinitionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteSuiteDefinitionRequestRequestTypeDef,
     DeviceUnderTestTypeDef,
     GetEndpointRequestRequestTypeDef,
-    GetEndpointResponseTypeDef,
     GetSuiteDefinitionRequestRequestTypeDef,
     GetSuiteRunReportRequestRequestTypeDef,
-    GetSuiteRunReportResponseTypeDef,
     GetSuiteRunRequestRequestTypeDef,
     ListSuiteDefinitionsRequestRequestTypeDef,
     ListSuiteRunsRequestRequestTypeDef,
     SuiteRunInformationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
-    StartSuiteRunResponseTypeDef,
     StopSuiteRunRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestCaseScenarioTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateSuiteDefinitionResponseTypeDef,
+    GetEndpointResponseTypeDef,
+    GetSuiteRunReportResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartSuiteRunResponseTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
+    SuiteDefinitionConfigurationOutputTypeDef,
     SuiteDefinitionConfigurationTypeDef,
     SuiteDefinitionInformationTypeDef,
+    SuiteRunConfigurationOutputTypeDef,
     SuiteRunConfigurationTypeDef,
     ListSuiteRunsResponseTypeDef,
     TestCaseRunTypeDef,
-    CreateSuiteDefinitionRequestRequestTypeDef,
     GetSuiteDefinitionResponseTypeDef,
+    CreateSuiteDefinitionRequestRequestTypeDef,
+    SuiteDefinitionConfigurationUnionTypeDef,
     UpdateSuiteDefinitionRequestRequestTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     StartSuiteRunRequestRequestTypeDef,
+    SuiteRunConfigurationUnionTypeDef,
     GroupResultTypeDef,
     TestResultTypeDef,
     GetSuiteRunResponseTypeDef,
 )
 
 
-def get_structure() -> CreateSuiteDefinitionResponseTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/README.md` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iotdeviceadvisor"></a>
 
 # types-aiobotocore-iotdeviceadvisor
 
 [![PyPI - types-aiobotocore-iotdeviceadvisor](https://img.shields.io/pypi/v/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotdeviceadvisor?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotdeviceadvisor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotdeviceadvisor)](https://pepy.tech/project/types-aiobotocore-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTDeviceAdvisor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [types-aiobotocore-iotdeviceadvisor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/).
 
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
@@ -253,61 +253,65 @@
 )
 
 
 def check_value(value: AuthenticationMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotdeviceadvisor.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotdeviceadvisor.type_defs import (
-    CreateSuiteDefinitionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteSuiteDefinitionRequestRequestTypeDef,
     DeviceUnderTestTypeDef,
     GetEndpointRequestRequestTypeDef,
-    GetEndpointResponseTypeDef,
     GetSuiteDefinitionRequestRequestTypeDef,
     GetSuiteRunReportRequestRequestTypeDef,
-    GetSuiteRunReportResponseTypeDef,
     GetSuiteRunRequestRequestTypeDef,
     ListSuiteDefinitionsRequestRequestTypeDef,
     ListSuiteRunsRequestRequestTypeDef,
     SuiteRunInformationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
-    StartSuiteRunResponseTypeDef,
     StopSuiteRunRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestCaseScenarioTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateSuiteDefinitionResponseTypeDef,
+    GetEndpointResponseTypeDef,
+    GetSuiteRunReportResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartSuiteRunResponseTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
+    SuiteDefinitionConfigurationOutputTypeDef,
     SuiteDefinitionConfigurationTypeDef,
     SuiteDefinitionInformationTypeDef,
+    SuiteRunConfigurationOutputTypeDef,
     SuiteRunConfigurationTypeDef,
     ListSuiteRunsResponseTypeDef,
     TestCaseRunTypeDef,
-    CreateSuiteDefinitionRequestRequestTypeDef,
     GetSuiteDefinitionResponseTypeDef,
+    CreateSuiteDefinitionRequestRequestTypeDef,
+    SuiteDefinitionConfigurationUnionTypeDef,
     UpdateSuiteDefinitionRequestRequestTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     StartSuiteRunRequestRequestTypeDef,
+    SuiteRunConfigurationUnionTypeDef,
     GroupResultTypeDef,
     TestResultTypeDef,
     GetSuiteRunResponseTypeDef,
 )
 
 
-def get_structure() -> CreateSuiteDefinitionResponseTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/setup.py` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotdeviceadvisor",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iotdeviceadvisor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with"
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
-    keywords="aiobotocore iotdeviceadvisor type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore iotdeviceadvisor type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotdeviceadvisor": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/"
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/__init__.py` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/__init__.pyi` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/__main__.py` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor\nOther"
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

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/client.py` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     GetSuiteDefinitionResponseTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunResponseTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     ListSuiteRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartSuiteRunResponseTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
-    SuiteRunConfigurationTypeDef,
+    SuiteDefinitionConfigurationUnionTypeDef,
+    SuiteRunConfigurationUnionTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
 )
 
 __all__ = ("IoTDeviceAdvisorClient",)
 
 
 class BotocoreClientError(BaseException):
@@ -86,15 +86,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#close)
         """
 
     async def create_suite_definition(
         self,
         *,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef,
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationUnionTypeDef,
         tags: Mapping[str, str] = ...
     ) -> CreateSuiteDefinitionResponseTypeDef:
         """
         Creates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.create_suite_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#create_suite_definition)
@@ -203,15 +203,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#list_tags_for_resource)
         """
 
     async def start_suite_run(
         self,
         *,
         suiteDefinitionId: str,
-        suiteRunConfiguration: SuiteRunConfigurationTypeDef,
+        suiteRunConfiguration: SuiteRunConfigurationUnionTypeDef,
         suiteDefinitionVersion: str = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSuiteRunResponseTypeDef:
         """
         Starts a Device Advisor test suite run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.start_suite_run)
@@ -242,15 +242,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#untag_resource)
         """
 
     async def update_suite_definition(
         self,
         *,
         suiteDefinitionId: str,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationUnionTypeDef
     ) -> UpdateSuiteDefinitionResponseTypeDef:
         """
         Updates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.update_suite_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#update_suite_definition)
         """
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/client.pyi` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     GetSuiteDefinitionResponseTypeDef,
     GetSuiteRunReportResponseTypeDef,
     GetSuiteRunResponseTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     ListSuiteRunsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartSuiteRunResponseTypeDef,
-    SuiteDefinitionConfigurationTypeDef,
-    SuiteRunConfigurationTypeDef,
+    SuiteDefinitionConfigurationUnionTypeDef,
+    SuiteRunConfigurationUnionTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
 )
 
 __all__ = ("IoTDeviceAdvisorClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -80,15 +80,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#close)
         """
     async def create_suite_definition(
         self,
         *,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef,
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationUnionTypeDef,
         tags: Mapping[str, str] = ...
     ) -> CreateSuiteDefinitionResponseTypeDef:
         """
         Creates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.create_suite_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#create_suite_definition)
@@ -187,15 +187,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#list_tags_for_resource)
         """
     async def start_suite_run(
         self,
         *,
         suiteDefinitionId: str,
-        suiteRunConfiguration: SuiteRunConfigurationTypeDef,
+        suiteRunConfiguration: SuiteRunConfigurationUnionTypeDef,
         suiteDefinitionVersion: str = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSuiteRunResponseTypeDef:
         """
         Starts a Device Advisor test suite run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.start_suite_run)
@@ -222,15 +222,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#untag_resource)
         """
     async def update_suite_definition(
         self,
         *,
         suiteDefinitionId: str,
-        suiteDefinitionConfiguration: SuiteDefinitionConfigurationTypeDef
+        suiteDefinitionConfiguration: SuiteDefinitionConfigurationUnionTypeDef
     ) -> UpdateSuiteDefinitionResponseTypeDef:
         """
         Updates a Device Advisor test suite.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor.Client.update_suite_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/client/#update_suite_definition)
         """
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/literals.py` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/literals.pyi` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/type_defs.py` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for iotdeviceadvisor service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_iotdeviceadvisor.type_defs import CreateSuiteDefinitionResponseTypeDef
+    from types_aiobotocore_iotdeviceadvisor.type_defs import ResponseMetadataTypeDef
 
-    data: CreateSuiteDefinitionResponseTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AuthenticationMethodType,
     ProtocolType,
     StatusType,
     SuiteRunStatusType,
     TestCaseScenarioStatusType,
@@ -25,60 +25,63 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "CreateSuiteDefinitionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteSuiteDefinitionRequestRequestTypeDef",
     "DeviceUnderTestTypeDef",
     "GetEndpointRequestRequestTypeDef",
-    "GetEndpointResponseTypeDef",
     "GetSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteRunReportRequestRequestTypeDef",
-    "GetSuiteRunReportResponseTypeDef",
     "GetSuiteRunRequestRequestTypeDef",
     "ListSuiteDefinitionsRequestRequestTypeDef",
     "ListSuiteRunsRequestRequestTypeDef",
     "SuiteRunInformationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartSuiteRunResponseTypeDef",
     "StopSuiteRunRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestCaseScenarioTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CreateSuiteDefinitionResponseTypeDef",
+    "GetEndpointResponseTypeDef",
+    "GetSuiteRunReportResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartSuiteRunResponseTypeDef",
     "UpdateSuiteDefinitionResponseTypeDef",
+    "SuiteDefinitionConfigurationOutputTypeDef",
     "SuiteDefinitionConfigurationTypeDef",
     "SuiteDefinitionInformationTypeDef",
+    "SuiteRunConfigurationOutputTypeDef",
     "SuiteRunConfigurationTypeDef",
     "ListSuiteRunsResponseTypeDef",
     "TestCaseRunTypeDef",
-    "CreateSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteDefinitionResponseTypeDef",
+    "CreateSuiteDefinitionRequestRequestTypeDef",
+    "SuiteDefinitionConfigurationUnionTypeDef",
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     "ListSuiteDefinitionsResponseTypeDef",
     "StartSuiteRunRequestRequestTypeDef",
+    "SuiteRunConfigurationUnionTypeDef",
     "GroupResultTypeDef",
     "TestResultTypeDef",
     "GetSuiteRunResponseTypeDef",
 )
 
-CreateSuiteDefinitionResponseTypeDef = TypedDict(
-    "CreateSuiteDefinitionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "suiteDefinitionId": str,
-        "suiteDefinitionArn": str,
-        "suiteDefinitionName": str,
-        "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
@@ -102,60 +105,42 @@
         "certificateArn": str,
         "deviceRoleArn": str,
         "authenticationMethod": AuthenticationMethodType,
     },
     total=False,
 )
 
-GetEndpointResponseTypeDef = TypedDict(
-    "GetEndpointResponseTypeDef",
-    {
-        "endpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
     },
 )
 _OptionalGetSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalGetSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionVersion": str,
     },
     total=False,
 )
 
-
 class GetSuiteDefinitionRequestRequestTypeDef(
     _RequiredGetSuiteDefinitionRequestRequestTypeDef,
     _OptionalGetSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
 GetSuiteRunReportRequestRequestTypeDef = TypedDict(
     "GetSuiteRunReportRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
 
-GetSuiteRunReportResponseTypeDef = TypedDict(
-    "GetSuiteRunReportResponseTypeDef",
-    {
-        "qualificationReportDownloadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSuiteRunRequestRequestTypeDef = TypedDict(
     "GetSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
@@ -200,44 +185,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
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
-StartSuiteRunResponseTypeDef = TypedDict(
-    "StartSuiteRunResponseTypeDef",
-    {
-        "suiteRunId": str,
-        "suiteRunArn": str,
-        "createdAt": datetime,
-        "endpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopSuiteRunRequestRequestTypeDef = TypedDict(
     "StopSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
@@ -266,27 +221,98 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+CreateSuiteDefinitionResponseTypeDef = TypedDict(
+    "CreateSuiteDefinitionResponseTypeDef",
+    {
+        "suiteDefinitionId": str,
+        "suiteDefinitionArn": str,
+        "suiteDefinitionName": str,
+        "createdAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEndpointResponseTypeDef = TypedDict(
+    "GetEndpointResponseTypeDef",
+    {
+        "endpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSuiteRunReportResponseTypeDef = TypedDict(
+    "GetSuiteRunReportResponseTypeDef",
+    {
+        "qualificationReportDownloadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSuiteRunResponseTypeDef = TypedDict(
+    "StartSuiteRunResponseTypeDef",
+    {
+        "suiteRunId": str,
+        "suiteRunArn": str,
+        "createdAt": datetime,
+        "endpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSuiteDefinitionResponseTypeDef = TypedDict(
     "UpdateSuiteDefinitionResponseTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionArn": str,
         "suiteDefinitionName": str,
         "suiteDefinitionVersion": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSuiteDefinitionConfigurationOutputTypeDef",
+    {
+        "suiteDefinitionName": str,
+        "rootGroup": str,
+        "devicePermissionRoleArn": str,
+    },
+)
+_OptionalSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSuiteDefinitionConfigurationOutputTypeDef",
+    {
+        "devices": List[DeviceUnderTestTypeDef],
+        "intendedForQualification": bool,
+        "isLongDurationTest": bool,
+        "protocol": ProtocolType,
+    },
+    total=False,
+)
+
+class SuiteDefinitionConfigurationOutputTypeDef(
+    _RequiredSuiteDefinitionConfigurationOutputTypeDef,
+    _OptionalSuiteDefinitionConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredSuiteDefinitionConfigurationTypeDef = TypedDict(
     "_RequiredSuiteDefinitionConfigurationTypeDef",
     {
         "suiteDefinitionName": str,
         "rootGroup": str,
         "devicePermissionRoleArn": str,
     },
@@ -298,63 +324,79 @@
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
     },
     total=False,
 )
 
-
 class SuiteDefinitionConfigurationTypeDef(
     _RequiredSuiteDefinitionConfigurationTypeDef, _OptionalSuiteDefinitionConfigurationTypeDef
 ):
     pass
 
-
 SuiteDefinitionInformationTypeDef = TypedDict(
     "SuiteDefinitionInformationTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionName": str,
         "defaultDevices": List[DeviceUnderTestTypeDef],
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
         "createdAt": datetime,
     },
     total=False,
 )
 
+_RequiredSuiteRunConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSuiteRunConfigurationOutputTypeDef",
+    {
+        "primaryDevice": DeviceUnderTestTypeDef,
+    },
+)
+_OptionalSuiteRunConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSuiteRunConfigurationOutputTypeDef",
+    {
+        "selectedTestList": List[str],
+        "parallelRun": bool,
+    },
+    total=False,
+)
+
+class SuiteRunConfigurationOutputTypeDef(
+    _RequiredSuiteRunConfigurationOutputTypeDef, _OptionalSuiteRunConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredSuiteRunConfigurationTypeDef = TypedDict(
     "_RequiredSuiteRunConfigurationTypeDef",
     {
         "primaryDevice": DeviceUnderTestTypeDef,
     },
 )
 _OptionalSuiteRunConfigurationTypeDef = TypedDict(
     "_OptionalSuiteRunConfigurationTypeDef",
     {
-        "selectedTestList": List[str],
+        "selectedTestList": Sequence[str],
         "parallelRun": bool,
     },
     total=False,
 )
 
-
 class SuiteRunConfigurationTypeDef(
     _RequiredSuiteRunConfigurationTypeDef, _OptionalSuiteRunConfigurationTypeDef
 ):
     pass
 
-
 ListSuiteRunsResponseTypeDef = TypedDict(
     "ListSuiteRunsResponseTypeDef",
     {
         "suiteRunsList": List[SuiteRunInformationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestCaseRunTypeDef = TypedDict(
     "TestCaseRunTypeDef",
     {
         "testCaseRunId": str,
@@ -367,65 +409,66 @@
         "warnings": str,
         "failure": str,
         "testScenarios": List[TestCaseScenarioTypeDef],
     },
     total=False,
 )
 
+GetSuiteDefinitionResponseTypeDef = TypedDict(
+    "GetSuiteDefinitionResponseTypeDef",
+    {
+        "suiteDefinitionId": str,
+        "suiteDefinitionArn": str,
+        "suiteDefinitionVersion": str,
+        "latestVersion": str,
+        "suiteDefinitionConfiguration": SuiteDefinitionConfigurationOutputTypeDef,
+        "createdAt": datetime,
+        "lastModifiedAt": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
 _OptionalCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateSuiteDefinitionRequestRequestTypeDef(
     _RequiredCreateSuiteDefinitionRequestRequestTypeDef,
     _OptionalCreateSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
-
-GetSuiteDefinitionResponseTypeDef = TypedDict(
-    "GetSuiteDefinitionResponseTypeDef",
-    {
-        "suiteDefinitionId": str,
-        "suiteDefinitionArn": str,
-        "suiteDefinitionVersion": str,
-        "latestVersion": str,
-        "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
-        "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+SuiteDefinitionConfigurationUnionTypeDef = Union[
+    SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
+]
 UpdateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
 
 ListSuiteDefinitionsResponseTypeDef = TypedDict(
     "ListSuiteDefinitionsResponseTypeDef",
     {
         "suiteDefinitionInformationList": List[SuiteDefinitionInformationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartSuiteRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
@@ -437,21 +480,22 @@
     {
         "suiteDefinitionVersion": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class StartSuiteRunRequestRequestTypeDef(
     _RequiredStartSuiteRunRequestRequestTypeDef, _OptionalStartSuiteRunRequestRequestTypeDef
 ):
     pass
 
-
+SuiteRunConfigurationUnionTypeDef = Union[
+    SuiteRunConfigurationTypeDef, SuiteRunConfigurationOutputTypeDef
+]
 GroupResultTypeDef = TypedDict(
     "GroupResultTypeDef",
     {
         "groupId": str,
         "groupName": str,
         "tests": List[TestCaseRunTypeDef],
     },
@@ -469,17 +513,17 @@
 GetSuiteRunResponseTypeDef = TypedDict(
     "GetSuiteRunResponseTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionVersion": str,
         "suiteRunId": str,
         "suiteRunArn": str,
-        "suiteRunConfiguration": SuiteRunConfigurationTypeDef,
+        "suiteRunConfiguration": SuiteRunConfigurationOutputTypeDef,
         "testResult": TestResultTypeDef,
         "startTime": datetime,
         "endTime": datetime,
         "status": SuiteRunStatusType,
         "errorReason": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor/type_defs.pyi` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for iotdeviceadvisor service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_iotdeviceadvisor.type_defs import CreateSuiteDefinitionResponseTypeDef
+    from types_aiobotocore_iotdeviceadvisor.type_defs import ResponseMetadataTypeDef
 
-    data: CreateSuiteDefinitionResponseTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AuthenticationMethodType,
     ProtocolType,
     StatusType,
     SuiteRunStatusType,
     TestCaseScenarioStatusType,
@@ -25,59 +25,64 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "CreateSuiteDefinitionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteSuiteDefinitionRequestRequestTypeDef",
     "DeviceUnderTestTypeDef",
     "GetEndpointRequestRequestTypeDef",
-    "GetEndpointResponseTypeDef",
     "GetSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteRunReportRequestRequestTypeDef",
-    "GetSuiteRunReportResponseTypeDef",
     "GetSuiteRunRequestRequestTypeDef",
     "ListSuiteDefinitionsRequestRequestTypeDef",
     "ListSuiteRunsRequestRequestTypeDef",
     "SuiteRunInformationTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartSuiteRunResponseTypeDef",
     "StopSuiteRunRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestCaseScenarioTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CreateSuiteDefinitionResponseTypeDef",
+    "GetEndpointResponseTypeDef",
+    "GetSuiteRunReportResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartSuiteRunResponseTypeDef",
     "UpdateSuiteDefinitionResponseTypeDef",
+    "SuiteDefinitionConfigurationOutputTypeDef",
     "SuiteDefinitionConfigurationTypeDef",
     "SuiteDefinitionInformationTypeDef",
+    "SuiteRunConfigurationOutputTypeDef",
     "SuiteRunConfigurationTypeDef",
     "ListSuiteRunsResponseTypeDef",
     "TestCaseRunTypeDef",
-    "CreateSuiteDefinitionRequestRequestTypeDef",
     "GetSuiteDefinitionResponseTypeDef",
+    "CreateSuiteDefinitionRequestRequestTypeDef",
+    "SuiteDefinitionConfigurationUnionTypeDef",
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     "ListSuiteDefinitionsResponseTypeDef",
     "StartSuiteRunRequestRequestTypeDef",
+    "SuiteRunConfigurationUnionTypeDef",
     "GroupResultTypeDef",
     "TestResultTypeDef",
     "GetSuiteRunResponseTypeDef",
 )
 
-CreateSuiteDefinitionResponseTypeDef = TypedDict(
-    "CreateSuiteDefinitionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "suiteDefinitionId": str,
-        "suiteDefinitionArn": str,
-        "suiteDefinitionName": str,
-        "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
@@ -101,58 +106,44 @@
         "certificateArn": str,
         "deviceRoleArn": str,
         "authenticationMethod": AuthenticationMethodType,
     },
     total=False,
 )
 
-GetEndpointResponseTypeDef = TypedDict(
-    "GetEndpointResponseTypeDef",
-    {
-        "endpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
     },
 )
 _OptionalGetSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalGetSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionVersion": str,
     },
     total=False,
 )
 
+
 class GetSuiteDefinitionRequestRequestTypeDef(
     _RequiredGetSuiteDefinitionRequestRequestTypeDef,
     _OptionalGetSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
 GetSuiteRunReportRequestRequestTypeDef = TypedDict(
     "GetSuiteRunReportRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
 
-GetSuiteRunReportResponseTypeDef = TypedDict(
-    "GetSuiteRunReportResponseTypeDef",
-    {
-        "qualificationReportDownloadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSuiteRunRequestRequestTypeDef = TypedDict(
     "GetSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
@@ -197,44 +188,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
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
-StartSuiteRunResponseTypeDef = TypedDict(
-    "StartSuiteRunResponseTypeDef",
-    {
-        "suiteRunId": str,
-        "suiteRunArn": str,
-        "createdAt": datetime,
-        "endpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopSuiteRunRequestRequestTypeDef = TypedDict(
     "StopSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteRunId": str,
     },
 )
@@ -263,27 +224,100 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+CreateSuiteDefinitionResponseTypeDef = TypedDict(
+    "CreateSuiteDefinitionResponseTypeDef",
+    {
+        "suiteDefinitionId": str,
+        "suiteDefinitionArn": str,
+        "suiteDefinitionName": str,
+        "createdAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEndpointResponseTypeDef = TypedDict(
+    "GetEndpointResponseTypeDef",
+    {
+        "endpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSuiteRunReportResponseTypeDef = TypedDict(
+    "GetSuiteRunReportResponseTypeDef",
+    {
+        "qualificationReportDownloadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSuiteRunResponseTypeDef = TypedDict(
+    "StartSuiteRunResponseTypeDef",
+    {
+        "suiteRunId": str,
+        "suiteRunArn": str,
+        "createdAt": datetime,
+        "endpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSuiteDefinitionResponseTypeDef = TypedDict(
     "UpdateSuiteDefinitionResponseTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionArn": str,
         "suiteDefinitionName": str,
         "suiteDefinitionVersion": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSuiteDefinitionConfigurationOutputTypeDef",
+    {
+        "suiteDefinitionName": str,
+        "rootGroup": str,
+        "devicePermissionRoleArn": str,
+    },
+)
+_OptionalSuiteDefinitionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSuiteDefinitionConfigurationOutputTypeDef",
+    {
+        "devices": List[DeviceUnderTestTypeDef],
+        "intendedForQualification": bool,
+        "isLongDurationTest": bool,
+        "protocol": ProtocolType,
     },
+    total=False,
 )
 
+
+class SuiteDefinitionConfigurationOutputTypeDef(
+    _RequiredSuiteDefinitionConfigurationOutputTypeDef,
+    _OptionalSuiteDefinitionConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredSuiteDefinitionConfigurationTypeDef = TypedDict(
     "_RequiredSuiteDefinitionConfigurationTypeDef",
     {
         "suiteDefinitionName": str,
         "rootGroup": str,
         "devicePermissionRoleArn": str,
     },
@@ -295,59 +329,85 @@
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
     },
     total=False,
 )
 
+
 class SuiteDefinitionConfigurationTypeDef(
     _RequiredSuiteDefinitionConfigurationTypeDef, _OptionalSuiteDefinitionConfigurationTypeDef
 ):
     pass
 
+
 SuiteDefinitionInformationTypeDef = TypedDict(
     "SuiteDefinitionInformationTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionName": str,
         "defaultDevices": List[DeviceUnderTestTypeDef],
         "intendedForQualification": bool,
         "isLongDurationTest": bool,
         "protocol": ProtocolType,
         "createdAt": datetime,
     },
     total=False,
 )
 
+_RequiredSuiteRunConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSuiteRunConfigurationOutputTypeDef",
+    {
+        "primaryDevice": DeviceUnderTestTypeDef,
+    },
+)
+_OptionalSuiteRunConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSuiteRunConfigurationOutputTypeDef",
+    {
+        "selectedTestList": List[str],
+        "parallelRun": bool,
+    },
+    total=False,
+)
+
+
+class SuiteRunConfigurationOutputTypeDef(
+    _RequiredSuiteRunConfigurationOutputTypeDef, _OptionalSuiteRunConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredSuiteRunConfigurationTypeDef = TypedDict(
     "_RequiredSuiteRunConfigurationTypeDef",
     {
         "primaryDevice": DeviceUnderTestTypeDef,
     },
 )
 _OptionalSuiteRunConfigurationTypeDef = TypedDict(
     "_OptionalSuiteRunConfigurationTypeDef",
     {
-        "selectedTestList": List[str],
+        "selectedTestList": Sequence[str],
         "parallelRun": bool,
     },
     total=False,
 )
 
+
 class SuiteRunConfigurationTypeDef(
     _RequiredSuiteRunConfigurationTypeDef, _OptionalSuiteRunConfigurationTypeDef
 ):
     pass
 
+
 ListSuiteRunsResponseTypeDef = TypedDict(
     "ListSuiteRunsResponseTypeDef",
     {
         "suiteRunsList": List[SuiteRunInformationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestCaseRunTypeDef = TypedDict(
     "TestCaseRunTypeDef",
     {
         "testCaseRunId": str,
@@ -360,63 +420,68 @@
         "warnings": str,
         "failure": str,
         "testScenarios": List[TestCaseScenarioTypeDef],
     },
     total=False,
 )
 
+GetSuiteDefinitionResponseTypeDef = TypedDict(
+    "GetSuiteDefinitionResponseTypeDef",
+    {
+        "suiteDefinitionId": str,
+        "suiteDefinitionArn": str,
+        "suiteDefinitionVersion": str,
+        "latestVersion": str,
+        "suiteDefinitionConfiguration": SuiteDefinitionConfigurationOutputTypeDef,
+        "createdAt": datetime,
+        "lastModifiedAt": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
 _OptionalCreateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSuiteDefinitionRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateSuiteDefinitionRequestRequestTypeDef(
     _RequiredCreateSuiteDefinitionRequestRequestTypeDef,
     _OptionalCreateSuiteDefinitionRequestRequestTypeDef,
 ):
     pass
 
-GetSuiteDefinitionResponseTypeDef = TypedDict(
-    "GetSuiteDefinitionResponseTypeDef",
-    {
-        "suiteDefinitionId": str,
-        "suiteDefinitionArn": str,
-        "suiteDefinitionVersion": str,
-        "latestVersion": str,
-        "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
-        "createdAt": datetime,
-        "lastModifiedAt": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
+SuiteDefinitionConfigurationUnionTypeDef = Union[
+    SuiteDefinitionConfigurationTypeDef, SuiteDefinitionConfigurationOutputTypeDef
+]
 UpdateSuiteDefinitionRequestRequestTypeDef = TypedDict(
     "UpdateSuiteDefinitionRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionConfiguration": SuiteDefinitionConfigurationTypeDef,
     },
 )
 
 ListSuiteDefinitionsResponseTypeDef = TypedDict(
     "ListSuiteDefinitionsResponseTypeDef",
     {
         "suiteDefinitionInformationList": List[SuiteDefinitionInformationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartSuiteRunRequestRequestTypeDef = TypedDict(
     "_RequiredStartSuiteRunRequestRequestTypeDef",
     {
         "suiteDefinitionId": str,
@@ -428,19 +493,24 @@
     {
         "suiteDefinitionVersion": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class StartSuiteRunRequestRequestTypeDef(
     _RequiredStartSuiteRunRequestRequestTypeDef, _OptionalStartSuiteRunRequestRequestTypeDef
 ):
     pass
 
+
+SuiteRunConfigurationUnionTypeDef = Union[
+    SuiteRunConfigurationTypeDef, SuiteRunConfigurationOutputTypeDef
+]
 GroupResultTypeDef = TypedDict(
     "GroupResultTypeDef",
     {
         "groupId": str,
         "groupName": str,
         "tests": List[TestCaseRunTypeDef],
     },
@@ -458,17 +528,17 @@
 GetSuiteRunResponseTypeDef = TypedDict(
     "GetSuiteRunResponseTypeDef",
     {
         "suiteDefinitionId": str,
         "suiteDefinitionVersion": str,
         "suiteRunId": str,
         "suiteRunArn": str,
-        "suiteRunConfiguration": SuiteRunConfigurationTypeDef,
+        "suiteRunConfiguration": SuiteRunConfigurationOutputTypeDef,
         "testResult": TestResultTypeDef,
         "startTime": datetime,
         "endTime": datetime,
         "status": SuiteRunStatusType,
         "errorReason": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotdeviceadvisor
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTDeviceAdvisor 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotdeviceadvisor type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotdeviceadvisor type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotdeviceadvisor"></a>
 
 # types-aiobotocore-iotdeviceadvisor
 
 [![PyPI - types-aiobotocore-iotdeviceadvisor](https://img.shields.io/pypi/v/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotdeviceadvisor.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotdeviceadvisor)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotdeviceadvisor?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotdeviceadvisor)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotdeviceadvisor)](https://pepy.tech/project/types-aiobotocore-iotdeviceadvisor)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTDeviceAdvisor 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#IoTDeviceAdvisor)
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
 [types-aiobotocore-iotdeviceadvisor docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotdeviceadvisor/).
 
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
@@ -286,61 +285,65 @@
 )
 
 
 def check_value(value: AuthenticationMethodType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotdeviceadvisor.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotdeviceadvisor.type_defs import (
-    CreateSuiteDefinitionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteSuiteDefinitionRequestRequestTypeDef,
     DeviceUnderTestTypeDef,
     GetEndpointRequestRequestTypeDef,
-    GetEndpointResponseTypeDef,
     GetSuiteDefinitionRequestRequestTypeDef,
     GetSuiteRunReportRequestRequestTypeDef,
-    GetSuiteRunReportResponseTypeDef,
     GetSuiteRunRequestRequestTypeDef,
     ListSuiteDefinitionsRequestRequestTypeDef,
     ListSuiteRunsRequestRequestTypeDef,
     SuiteRunInformationTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
-    StartSuiteRunResponseTypeDef,
     StopSuiteRunRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TestCaseScenarioTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateSuiteDefinitionResponseTypeDef,
+    GetEndpointResponseTypeDef,
+    GetSuiteRunReportResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartSuiteRunResponseTypeDef,
     UpdateSuiteDefinitionResponseTypeDef,
+    SuiteDefinitionConfigurationOutputTypeDef,
     SuiteDefinitionConfigurationTypeDef,
     SuiteDefinitionInformationTypeDef,
+    SuiteRunConfigurationOutputTypeDef,
     SuiteRunConfigurationTypeDef,
     ListSuiteRunsResponseTypeDef,
     TestCaseRunTypeDef,
-    CreateSuiteDefinitionRequestRequestTypeDef,
     GetSuiteDefinitionResponseTypeDef,
+    CreateSuiteDefinitionRequestRequestTypeDef,
+    SuiteDefinitionConfigurationUnionTypeDef,
     UpdateSuiteDefinitionRequestRequestTypeDef,
     ListSuiteDefinitionsResponseTypeDef,
     StartSuiteRunRequestRequestTypeDef,
+    SuiteRunConfigurationUnionTypeDef,
     GroupResultTypeDef,
     TestResultTypeDef,
     GetSuiteRunResponseTypeDef,
 )
 
 
-def get_structure() -> CreateSuiteDefinitionResponseTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotdeviceadvisor-2.5.2/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt` & `types-aiobotocore-iotdeviceadvisor-2.5.2.post1/types_aiobotocore_iotdeviceadvisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*


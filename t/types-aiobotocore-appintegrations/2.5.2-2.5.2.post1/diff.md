# Comparing `tmp/types-aiobotocore-appintegrations-2.5.2.tar.gz` & `tmp/types-aiobotocore-appintegrations-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appintegrations-2.5.2.tar", last modified: Sat Jul  8 01:43:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-appintegrations-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
```

## Comparing `types-aiobotocore-appintegrations-2.5.2.tar` & `types-aiobotocore-appintegrations-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.445654 types-aiobotocore-appintegrations-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:45.000000 types-aiobotocore-appintegrations-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-07-08 01:43:12.437654 types-aiobotocore-appintegrations-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-07-08 01:25:45.000000 types-aiobotocore-appintegrations-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:12.445654 types-aiobotocore-appintegrations-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-08 01:25:45.000000 types-aiobotocore-appintegrations-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.437654 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-08 01:25:45.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-08 01:25:45.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-08 01:25:45.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-07-08 01:25:45.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-07-08 01:25:45.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-07-08 01:25:45.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-07-08 01:25:45.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:45.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-07-08 01:25:46.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-07-08 01:25:46.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:45.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.437654 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-07-08 01:43:12.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:12.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:12.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-08 01:43:12.000000 types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.565660 types-aiobotocore-appintegrations-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-08-02 14:51:50.565660 types-aiobotocore-appintegrations-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.565660 types-aiobotocore-appintegrations-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.565660 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14082 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.565660 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-08-02 14:51:50.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:51:50.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:51:50.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appintegrations-2.5.2/LICENSE` & `types-aiobotocore-appintegrations-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2/PKG-INFO` & `types-aiobotocore-appintegrations-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appintegrations
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore appintegrations type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore appintegrations type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appintegrations"></a>
 
 # types-aiobotocore-appintegrations
 
 [![PyPI - types-aiobotocore-appintegrations](https://img.shields.io/pypi/v/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appintegrations?color=blue)](https://pypistats.org/packages/types-aiobotocore-appintegrations)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appintegrations)](https://pepy.tech/project/types-aiobotocore-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppIntegrationsService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [types-aiobotocore-appintegrations docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/).
 
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
@@ -280,59 +279,61 @@
 )
 
 
 def check_value(value: AppIntegrationsServiceServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appintegrations.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
+    FileConfigurationOutputTypeDef,
+    ResponseMetadataTypeDef,
     EventFilterTypeDef,
-    CreateEventIntegrationResponseTypeDef,
     DataIntegrationAssociationSummaryTypeDef,
     DataIntegrationSummaryTypeDef,
     DeleteDataIntegrationRequestRequestTypeDef,
     DeleteEventIntegrationRequestRequestTypeDef,
     EventIntegrationAssociationTypeDef,
     GetDataIntegrationRequestRequestTypeDef,
     GetEventIntegrationRequestRequestTypeDef,
     ListDataIntegrationAssociationsRequestRequestTypeDef,
     ListDataIntegrationsRequestRequestTypeDef,
     ListEventIntegrationAssociationsRequestRequestTypeDef,
     ListEventIntegrationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
+    FileConfigurationUnionTypeDef,
     CreateDataIntegrationResponseTypeDef,
+    CreateEventIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
     EventIntegrationTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
 )
 
 
-def get_structure() -> FileConfigurationTypeDef:
+def get_value() -> FileConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appintegrations-2.5.2/README.md` & `types-aiobotocore-appintegrations-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-appintegrations"></a>
 
 # types-aiobotocore-appintegrations
 
 [![PyPI - types-aiobotocore-appintegrations](https://img.shields.io/pypi/v/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appintegrations?color=blue)](https://pypistats.org/packages/types-aiobotocore-appintegrations)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appintegrations)](https://pepy.tech/project/types-aiobotocore-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppIntegrationsService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [types-aiobotocore-appintegrations docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/).
 
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
@@ -247,59 +247,61 @@
 )
 
 
 def check_value(value: AppIntegrationsServiceServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appintegrations.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
+    FileConfigurationOutputTypeDef,
+    ResponseMetadataTypeDef,
     EventFilterTypeDef,
-    CreateEventIntegrationResponseTypeDef,
     DataIntegrationAssociationSummaryTypeDef,
     DataIntegrationSummaryTypeDef,
     DeleteDataIntegrationRequestRequestTypeDef,
     DeleteEventIntegrationRequestRequestTypeDef,
     EventIntegrationAssociationTypeDef,
     GetDataIntegrationRequestRequestTypeDef,
     GetEventIntegrationRequestRequestTypeDef,
     ListDataIntegrationAssociationsRequestRequestTypeDef,
     ListDataIntegrationsRequestRequestTypeDef,
     ListEventIntegrationAssociationsRequestRequestTypeDef,
     ListEventIntegrationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
+    FileConfigurationUnionTypeDef,
     CreateDataIntegrationResponseTypeDef,
+    CreateEventIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
     EventIntegrationTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
 )
 
 
-def get_structure() -> FileConfigurationTypeDef:
+def get_value() -> FileConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appintegrations-2.5.2/setup.py` & `types-aiobotocore-appintegrations-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appintegrations",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_appintegrations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with"
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
-    keywords="aiobotocore appintegrations type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore appintegrations type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appintegrations": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/"
```

### Comparing `types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/__init__.py` & `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/__init__.pyi` & `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/__main__.py` & `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.AppIntegrationsService 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService\nOther"
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

### Comparing `types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/client.py` & `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
     CreateDataIntegrationResponseTypeDef,
     CreateEventIntegrationResponseTypeDef,
     EventFilterTypeDef,
-    FileConfigurationTypeDef,
+    FileConfigurationUnionTypeDef,
     GetDataIntegrationResponseTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -95,15 +95,15 @@
         Name: str,
         KmsKey: str,
         SourceURI: str,
         ScheduleConfig: ScheduleConfigurationTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...,
-        FileConfiguration: FileConfigurationTypeDef = ...,
+        FileConfiguration: FileConfigurationUnionTypeDef = ...,
         ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...
     ) -> CreateDataIntegrationResponseTypeDef:
         """
         Creates and persists a DataIntegration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.create_data_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/client/#create_data_integration)
```

### Comparing `types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/client.pyi` & `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
     CreateDataIntegrationResponseTypeDef,
     CreateEventIntegrationResponseTypeDef,
     EventFilterTypeDef,
-    FileConfigurationTypeDef,
+    FileConfigurationUnionTypeDef,
     GetDataIntegrationResponseTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -89,15 +89,15 @@
         Name: str,
         KmsKey: str,
         SourceURI: str,
         ScheduleConfig: ScheduleConfigurationTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...,
-        FileConfiguration: FileConfigurationTypeDef = ...,
+        FileConfiguration: FileConfigurationUnionTypeDef = ...,
         ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...
     ) -> CreateDataIntegrationResponseTypeDef:
         """
         Creates and persists a DataIntegration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.create_data_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/client/#create_data_integration)
```

### Comparing `types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/literals.py` & `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/literals.pyi` & `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/type_defs.py` & `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,52 +4,53 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_appintegrations.type_defs import FileConfigurationTypeDef
 
-    data: FileConfigurationTypeDef = {...}
+    data: FileConfigurationTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "FileConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
+    "FileConfigurationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "EventFilterTypeDef",
-    "CreateEventIntegrationResponseTypeDef",
     "DataIntegrationAssociationSummaryTypeDef",
     "DataIntegrationSummaryTypeDef",
     "DeleteDataIntegrationRequestRequestTypeDef",
     "DeleteEventIntegrationRequestRequestTypeDef",
     "EventIntegrationAssociationTypeDef",
     "GetDataIntegrationRequestRequestTypeDef",
     "GetEventIntegrationRequestRequestTypeDef",
     "ListDataIntegrationAssociationsRequestRequestTypeDef",
     "ListDataIntegrationsRequestRequestTypeDef",
     "ListEventIntegrationAssociationsRequestRequestTypeDef",
     "ListEventIntegrationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataIntegrationRequestRequestTypeDef",
     "UpdateEventIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationRequestRequestTypeDef",
+    "FileConfigurationUnionTypeDef",
     "CreateDataIntegrationResponseTypeDef",
+    "CreateEventIntegrationResponseTypeDef",
     "GetDataIntegrationResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateEventIntegrationRequestRequestTypeDef",
     "EventIntegrationTypeDef",
     "GetEventIntegrationResponseTypeDef",
     "ListDataIntegrationAssociationsResponseTypeDef",
     "ListDataIntegrationsResponseTypeDef",
     "ListEventIntegrationAssociationsResponseTypeDef",
     "ListEventIntegrationsResponseTypeDef",
@@ -65,21 +66,19 @@
     "_OptionalFileConfigurationTypeDef",
     {
         "Filters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class FileConfigurationTypeDef(
     _RequiredFileConfigurationTypeDef, _OptionalFileConfigurationTypeDef
 ):
     pass
 
-
 _RequiredScheduleConfigurationTypeDef = TypedDict(
     "_RequiredScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 _OptionalScheduleConfigurationTypeDef = TypedDict(
@@ -87,33 +86,53 @@
     {
         "FirstExecutionFrom": str,
         "Object": str,
     },
     total=False,
 )
 
-
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
+_RequiredFileConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFileConfigurationOutputTypeDef",
+    {
+        "Folders": List[str],
+    },
+)
+_OptionalFileConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFileConfigurationOutputTypeDef",
+    {
+        "Filters": Dict[str, List[str]],
+    },
+    total=False,
+)
 
-EventFilterTypeDef = TypedDict(
-    "EventFilterTypeDef",
+class FileConfigurationOutputTypeDef(
+    _RequiredFileConfigurationOutputTypeDef, _OptionalFileConfigurationOutputTypeDef
+):
+    pass
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Source": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-CreateEventIntegrationResponseTypeDef = TypedDict(
-    "CreateEventIntegrationResponseTypeDef",
+EventFilterTypeDef = TypedDict(
+    "EventFilterTypeDef",
     {
-        "EventIntegrationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Source": str,
     },
 )
 
 DataIntegrationAssociationSummaryTypeDef = TypedDict(
     "DataIntegrationAssociationSummaryTypeDef",
     {
         "DataIntegrationAssociationArn": str,
@@ -185,22 +204,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDataIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListDataIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListDataIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListDataIntegrationsRequestRequestTypeDef = TypedDict(
     "ListDataIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -217,22 +234,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListEventIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListEventIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListEventIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListEventIntegrationsRequestRequestTypeDef = TypedDict(
     "ListEventIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -241,33 +256,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -291,44 +287,40 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateDataIntegrationRequestRequestTypeDef(
     _RequiredUpdateDataIntegrationRequestRequestTypeDef,
     _OptionalUpdateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateEventIntegrationRequestRequestTypeDef(
     _RequiredUpdateEventIntegrationRequestRequestTypeDef,
     _OptionalUpdateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDataIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataIntegrationRequestRequestTypeDef",
     {
         "Name": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfig": ScheduleConfigurationTypeDef,
@@ -342,54 +334,69 @@
         "ClientToken": str,
         "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Mapping[str, Mapping[str, Sequence[str]]],
     },
     total=False,
 )
 
-
 class CreateDataIntegrationRequestRequestTypeDef(
     _RequiredCreateDataIntegrationRequestRequestTypeDef,
     _OptionalCreateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
+FileConfigurationUnionTypeDef = Union[FileConfigurationTypeDef, FileConfigurationOutputTypeDef]
 CreateDataIntegrationResponseTypeDef = TypedDict(
     "CreateDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
         "ClientToken": str,
-        "FileConfiguration": FileConfigurationTypeDef,
+        "FileConfiguration": FileConfigurationOutputTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEventIntegrationResponseTypeDef = TypedDict(
+    "CreateEventIntegrationResponseTypeDef",
+    {
+        "EventIntegrationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataIntegrationResponseTypeDef = TypedDict(
     "GetDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
-        "FileConfiguration": FileConfigurationTypeDef,
+        "FileConfiguration": FileConfigurationOutputTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
@@ -403,22 +410,20 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateEventIntegrationRequestRequestTypeDef(
     _RequiredCreateEventIntegrationRequestRequestTypeDef,
     _OptionalCreateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
 EventIntegrationTypeDef = TypedDict(
     "EventIntegrationTypeDef",
     {
         "EventIntegrationArn": str,
         "Name": str,
         "Description": str,
         "EventFilter": EventFilterTypeDef,
@@ -433,46 +438,46 @@
     {
         "Name": str,
         "Description": str,
         "EventIntegrationArn": str,
         "EventBridgeBus": str,
         "EventFilter": EventFilterTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListDataIntegrationAssociationsResponseTypeDef",
     {
         "DataIntegrationAssociations": List[DataIntegrationAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataIntegrationsResponseTypeDef = TypedDict(
     "ListDataIntegrationsResponseTypeDef",
     {
         "DataIntegrations": List[DataIntegrationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListEventIntegrationAssociationsResponseTypeDef",
     {
         "EventIntegrationAssociations": List[EventIntegrationAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventIntegrationsResponseTypeDef = TypedDict(
     "ListEventIntegrationsResponseTypeDef",
     {
         "EventIntegrations": List[EventIntegrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations/type_defs.pyi` & `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,51 +4,54 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_appintegrations.type_defs import FileConfigurationTypeDef
 
-    data: FileConfigurationTypeDef = {...}
+    data: FileConfigurationTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "FileConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
+    "FileConfigurationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "EventFilterTypeDef",
-    "CreateEventIntegrationResponseTypeDef",
     "DataIntegrationAssociationSummaryTypeDef",
     "DataIntegrationSummaryTypeDef",
     "DeleteDataIntegrationRequestRequestTypeDef",
     "DeleteEventIntegrationRequestRequestTypeDef",
     "EventIntegrationAssociationTypeDef",
     "GetDataIntegrationRequestRequestTypeDef",
     "GetEventIntegrationRequestRequestTypeDef",
     "ListDataIntegrationAssociationsRequestRequestTypeDef",
     "ListDataIntegrationsRequestRequestTypeDef",
     "ListEventIntegrationAssociationsRequestRequestTypeDef",
     "ListEventIntegrationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataIntegrationRequestRequestTypeDef",
     "UpdateEventIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationRequestRequestTypeDef",
+    "FileConfigurationUnionTypeDef",
     "CreateDataIntegrationResponseTypeDef",
+    "CreateEventIntegrationResponseTypeDef",
     "GetDataIntegrationResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateEventIntegrationRequestRequestTypeDef",
     "EventIntegrationTypeDef",
     "GetEventIntegrationResponseTypeDef",
     "ListDataIntegrationAssociationsResponseTypeDef",
     "ListDataIntegrationsResponseTypeDef",
     "ListEventIntegrationAssociationsResponseTypeDef",
     "ListEventIntegrationsResponseTypeDef",
@@ -64,19 +67,21 @@
     "_OptionalFileConfigurationTypeDef",
     {
         "Filters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class FileConfigurationTypeDef(
     _RequiredFileConfigurationTypeDef, _OptionalFileConfigurationTypeDef
 ):
     pass
 
+
 _RequiredScheduleConfigurationTypeDef = TypedDict(
     "_RequiredScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 _OptionalScheduleConfigurationTypeDef = TypedDict(
@@ -84,31 +89,57 @@
     {
         "FirstExecutionFrom": str,
         "Object": str,
     },
     total=False,
 )
 
+
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
-EventFilterTypeDef = TypedDict(
-    "EventFilterTypeDef",
+
+_RequiredFileConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFileConfigurationOutputTypeDef",
     {
-        "Source": str,
+        "Folders": List[str],
     },
 )
+_OptionalFileConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFileConfigurationOutputTypeDef",
+    {
+        "Filters": Dict[str, List[str]],
+    },
+    total=False,
+)
 
-CreateEventIntegrationResponseTypeDef = TypedDict(
-    "CreateEventIntegrationResponseTypeDef",
+
+class FileConfigurationOutputTypeDef(
+    _RequiredFileConfigurationOutputTypeDef, _OptionalFileConfigurationOutputTypeDef
+):
+    pass
+
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "EventIntegrationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+EventFilterTypeDef = TypedDict(
+    "EventFilterTypeDef",
+    {
+        "Source": str,
     },
 )
 
 DataIntegrationAssociationSummaryTypeDef = TypedDict(
     "DataIntegrationAssociationSummaryTypeDef",
     {
         "DataIntegrationAssociationArn": str,
@@ -180,20 +211,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDataIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListDataIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListDataIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListDataIntegrationsRequestRequestTypeDef = TypedDict(
     "ListDataIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -210,20 +243,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListEventIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListEventIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListEventIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListEventIntegrationsRequestRequestTypeDef = TypedDict(
     "ListEventIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -232,33 +267,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -282,40 +298,44 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateDataIntegrationRequestRequestTypeDef(
     _RequiredUpdateDataIntegrationRequestRequestTypeDef,
     _OptionalUpdateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateEventIntegrationRequestRequestTypeDef(
     _RequiredUpdateEventIntegrationRequestRequestTypeDef,
     _OptionalUpdateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDataIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataIntegrationRequestRequestTypeDef",
     {
         "Name": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfig": ScheduleConfigurationTypeDef,
@@ -329,52 +349,71 @@
         "ClientToken": str,
         "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Mapping[str, Mapping[str, Sequence[str]]],
     },
     total=False,
 )
 
+
 class CreateDataIntegrationRequestRequestTypeDef(
     _RequiredCreateDataIntegrationRequestRequestTypeDef,
     _OptionalCreateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
+FileConfigurationUnionTypeDef = Union[FileConfigurationTypeDef, FileConfigurationOutputTypeDef]
 CreateDataIntegrationResponseTypeDef = TypedDict(
     "CreateDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
         "ClientToken": str,
-        "FileConfiguration": FileConfigurationTypeDef,
+        "FileConfiguration": FileConfigurationOutputTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEventIntegrationResponseTypeDef = TypedDict(
+    "CreateEventIntegrationResponseTypeDef",
+    {
+        "EventIntegrationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataIntegrationResponseTypeDef = TypedDict(
     "GetDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
-        "FileConfiguration": FileConfigurationTypeDef,
+        "FileConfiguration": FileConfigurationOutputTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
@@ -388,20 +427,22 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateEventIntegrationRequestRequestTypeDef(
     _RequiredCreateEventIntegrationRequestRequestTypeDef,
     _OptionalCreateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
 EventIntegrationTypeDef = TypedDict(
     "EventIntegrationTypeDef",
     {
         "EventIntegrationArn": str,
         "Name": str,
         "Description": str,
         "EventFilter": EventFilterTypeDef,
@@ -416,46 +457,46 @@
     {
         "Name": str,
         "Description": str,
         "EventIntegrationArn": str,
         "EventBridgeBus": str,
         "EventFilter": EventFilterTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListDataIntegrationAssociationsResponseTypeDef",
     {
         "DataIntegrationAssociations": List[DataIntegrationAssociationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataIntegrationsResponseTypeDef = TypedDict(
     "ListDataIntegrationsResponseTypeDef",
     {
         "DataIntegrations": List[DataIntegrationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventIntegrationAssociationsResponseTypeDef = TypedDict(
     "ListEventIntegrationAssociationsResponseTypeDef",
     {
         "EventIntegrationAssociations": List[EventIntegrationAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventIntegrationsResponseTypeDef = TypedDict(
     "ListEventIntegrationsResponseTypeDef",
     {
         "EventIntegrations": List[EventIntegrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations.egg-info/PKG-INFO` & `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appintegrations
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore appintegrations type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore appintegrations type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appintegrations"></a>
 
 # types-aiobotocore-appintegrations
 
 [![PyPI - types-aiobotocore-appintegrations](https://img.shields.io/pypi/v/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appintegrations.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appintegrations)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appintegrations?color=blue)](https://pypistats.org/packages/types-aiobotocore-appintegrations)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appintegrations)](https://pepy.tech/project/types-aiobotocore-appintegrations)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppIntegrationsService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
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
 [types-aiobotocore-appintegrations docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/).
 
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
@@ -280,59 +279,61 @@
 )
 
 
 def check_value(value: AppIntegrationsServiceServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appintegrations.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appintegrations.type_defs import (
     FileConfigurationTypeDef,
     ScheduleConfigurationTypeDef,
+    FileConfigurationOutputTypeDef,
+    ResponseMetadataTypeDef,
     EventFilterTypeDef,
-    CreateEventIntegrationResponseTypeDef,
     DataIntegrationAssociationSummaryTypeDef,
     DataIntegrationSummaryTypeDef,
     DeleteDataIntegrationRequestRequestTypeDef,
     DeleteEventIntegrationRequestRequestTypeDef,
     EventIntegrationAssociationTypeDef,
     GetDataIntegrationRequestRequestTypeDef,
     GetEventIntegrationRequestRequestTypeDef,
     ListDataIntegrationAssociationsRequestRequestTypeDef,
     ListDataIntegrationsRequestRequestTypeDef,
     ListEventIntegrationAssociationsRequestRequestTypeDef,
     ListEventIntegrationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDataIntegrationRequestRequestTypeDef,
     UpdateEventIntegrationRequestRequestTypeDef,
     CreateDataIntegrationRequestRequestTypeDef,
+    FileConfigurationUnionTypeDef,
     CreateDataIntegrationResponseTypeDef,
+    CreateEventIntegrationResponseTypeDef,
     GetDataIntegrationResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateEventIntegrationRequestRequestTypeDef,
     EventIntegrationTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
 )
 
 
-def get_structure() -> FileConfigurationTypeDef:
+def get_value() -> FileConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appintegrations-2.5.2/types_aiobotocore_appintegrations.egg-info/SOURCES.txt` & `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*


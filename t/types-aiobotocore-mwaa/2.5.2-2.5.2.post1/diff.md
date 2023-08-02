# Comparing `tmp/types-aiobotocore-mwaa-2.5.2.tar.gz` & `tmp/types-aiobotocore-mwaa-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mwaa-2.5.2.tar", last modified: Sat Jul  8 01:44:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-mwaa-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:43 2023, max compression
```

## Comparing `types-aiobotocore-mwaa-2.5.2.tar` & `types-aiobotocore-mwaa-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.310595 types-aiobotocore-mwaa-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:35:35.000000 types-aiobotocore-mwaa-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-07-08 01:44:02.310595 types-aiobotocore-mwaa-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-07-08 01:35:35.000000 types-aiobotocore-mwaa-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:02.310595 types-aiobotocore-mwaa-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-08 01:35:35.000000 types-aiobotocore-mwaa-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.306595 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-08 01:35:35.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-08 01:35:35.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:35:35.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-08 01:35:35.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-07-08 01:35:35.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-08 01:35:36.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-08 01:35:36.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-08 01:35:35.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-08 01:35:35.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:35:35.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-07-08 01:35:36.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11651 2023-07-08 01:35:36.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:35:35.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.310595 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-07-08 01:44:02.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-08 01:44:02.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:02.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 01:44:02.000000 types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.009513 types-aiobotocore-mwaa-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-08-02 14:52:43.009513 types-aiobotocore-mwaa-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12482 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:43.009513 types-aiobotocore-mwaa-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.001513 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-08-02 14:43:52.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:51.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.009513 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-08-02 14:52:42.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-02 14:52:42.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:42.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 14:52:42.000000 types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mwaa-2.5.2/LICENSE` & `types-aiobotocore-mwaa-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.5.2/PKG-INFO` & `types-aiobotocore-mwaa-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mwaa
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.MWAA 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.MWAA 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore mwaa type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore mwaa type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-mwaa"></a>
 
 # types-aiobotocore-mwaa
 
 [![PyPI - types-aiobotocore-mwaa](https://img.shields.io/pypi/v/types-aiobotocore-mwaa.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mwaa)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mwaa.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mwaa)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-mwaa?color=blue)](https://pypistats.org/packages/types-aiobotocore-mwaa)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mwaa)](https://pepy.tech/project/types-aiobotocore-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MWAA 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
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
 [types-aiobotocore-mwaa docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/).
 
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
@@ -310,60 +309,63 @@
 )
 
 
 def check_value(value: EnvironmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_mwaa.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_mwaa.type_defs import (
     CreateCliTokenRequestRequestTypeDef,
-    CreateCliTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     NetworkConfigurationTypeDef,
-    CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenRequestRequestTypeDef,
-    CreateWebLoginTokenResponseTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DimensionTypeDef,
+    NetworkConfigurationOutputTypeDef,
     GetEnvironmentInputRequestTypeDef,
     UpdateErrorTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEnvironmentsInputRequestTypeDef,
-    ListEnvironmentsOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ModuleLoggingConfigurationInputTypeDef,
     ModuleLoggingConfigurationTypeDef,
     StatisticSetTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
+    CreateCliTokenResponseTypeDef,
+    CreateEnvironmentOutputTypeDef,
+    CreateWebLoginTokenResponseTypeDef,
+    ListEnvironmentsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
+    NetworkConfigurationUnionTypeDef,
     LastUpdateTypeDef,
+    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     LoggingConfigurationInputTypeDef,
     LoggingConfigurationTypeDef,
     MetricDatumTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     EnvironmentTypeDef,
     PublishMetricsInputRequestTypeDef,
     GetEnvironmentOutputTypeDef,
 )
 
 
-def get_structure() -> CreateCliTokenRequestRequestTypeDef:
+def get_value() -> CreateCliTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-mwaa-2.5.2/README.md` & `types-aiobotocore-mwaa-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-mwaa"></a>
 
 # types-aiobotocore-mwaa
 
 [![PyPI - types-aiobotocore-mwaa](https://img.shields.io/pypi/v/types-aiobotocore-mwaa.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mwaa)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mwaa.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mwaa)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-mwaa?color=blue)](https://pypistats.org/packages/types-aiobotocore-mwaa)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mwaa)](https://pepy.tech/project/types-aiobotocore-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MWAA 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
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
 [types-aiobotocore-mwaa docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/).
 
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
@@ -277,60 +277,63 @@
 )
 
 
 def check_value(value: EnvironmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_mwaa.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_mwaa.type_defs import (
     CreateCliTokenRequestRequestTypeDef,
-    CreateCliTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     NetworkConfigurationTypeDef,
-    CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenRequestRequestTypeDef,
-    CreateWebLoginTokenResponseTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DimensionTypeDef,
+    NetworkConfigurationOutputTypeDef,
     GetEnvironmentInputRequestTypeDef,
     UpdateErrorTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEnvironmentsInputRequestTypeDef,
-    ListEnvironmentsOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ModuleLoggingConfigurationInputTypeDef,
     ModuleLoggingConfigurationTypeDef,
     StatisticSetTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
+    CreateCliTokenResponseTypeDef,
+    CreateEnvironmentOutputTypeDef,
+    CreateWebLoginTokenResponseTypeDef,
+    ListEnvironmentsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
+    NetworkConfigurationUnionTypeDef,
     LastUpdateTypeDef,
+    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     LoggingConfigurationInputTypeDef,
     LoggingConfigurationTypeDef,
     MetricDatumTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     EnvironmentTypeDef,
     PublishMetricsInputRequestTypeDef,
     GetEnvironmentOutputTypeDef,
 )
 
 
-def get_structure() -> CreateCliTokenRequestRequestTypeDef:
+def get_value() -> CreateCliTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-mwaa-2.5.2/setup.py` & `types-aiobotocore-mwaa-2.5.2.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mwaa",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_mwaa"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MWAA 2.5.2 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        " 7.17.1"
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
-    keywords="aiobotocore mwaa type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore mwaa type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mwaa": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/__init__.py` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/__init__.pyi` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/__main__.py` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MWAA 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.MWAA 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA\nOther"
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

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/client.py` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenResponseTypeDef,
     GetEnvironmentOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     LoggingConfigurationInputTypeDef,
     MetricDatumTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationUnionTypeDef,
     UpdateEnvironmentOutputTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -104,15 +104,15 @@
 
     async def create_environment(
         self,
         *,
         DagS3Path: str,
         ExecutionRoleArn: str,
         Name: str,
-        NetworkConfiguration: NetworkConfigurationTypeDef,
+        NetworkConfiguration: NetworkConfigurationUnionTypeDef,
         SourceBucketArn: str,
         AirflowConfigurationOptions: Mapping[str, str] = ...,
         AirflowVersion: str = ...,
         EnvironmentClass: str = ...,
         KmsKey: str = ...,
         LoggingConfiguration: LoggingConfigurationInputTypeDef = ...,
         MaxWorkers: int = ...,
```

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/client.pyi` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenResponseTypeDef,
     GetEnvironmentOutputTypeDef,
     ListEnvironmentsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     LoggingConfigurationInputTypeDef,
     MetricDatumTypeDef,
-    NetworkConfigurationTypeDef,
+    NetworkConfigurationUnionTypeDef,
     UpdateEnvironmentOutputTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -96,15 +96,15 @@
         """
     async def create_environment(
         self,
         *,
         DagS3Path: str,
         ExecutionRoleArn: str,
         Name: str,
-        NetworkConfiguration: NetworkConfigurationTypeDef,
+        NetworkConfiguration: NetworkConfigurationUnionTypeDef,
         SourceBucketArn: str,
         AirflowConfigurationOptions: Mapping[str, str] = ...,
         AirflowVersion: str = ...,
         EnvironmentClass: str = ...,
         KmsKey: str = ...,
         LoggingConfiguration: LoggingConfigurationInputTypeDef = ...,
         MaxWorkers: int = ...,
```

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/literals.py` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/literals.pyi` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/paginator.py` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,13 @@
 class ListEnvironmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/paginators/#listenvironmentspaginator)
         """
```

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/paginator.pyi` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,13 +40,13 @@
 class ListEnvironmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/paginators/#listenvironmentspaginator)
         """
```

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/type_defs.py` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_mwaa.type_defs import CreateCliTokenRequestRequestTypeDef
 
-    data: CreateCliTokenRequestRequestTypeDef = {...}
+    data: CreateCliTokenRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -27,38 +27,41 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CreateCliTokenRequestRequestTypeDef",
-    "CreateCliTokenResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "NetworkConfigurationTypeDef",
-    "CreateEnvironmentOutputTypeDef",
     "CreateWebLoginTokenRequestRequestTypeDef",
-    "CreateWebLoginTokenResponseTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DimensionTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "UpdateErrorTypeDef",
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
-    "ListEnvironmentsOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ModuleLoggingConfigurationInputTypeDef",
     "ModuleLoggingConfigurationTypeDef",
     "StatisticSetTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateNetworkConfigurationInputTypeDef",
+    "CreateCliTokenResponseTypeDef",
+    "CreateEnvironmentOutputTypeDef",
+    "CreateWebLoginTokenResponseTypeDef",
+    "ListEnvironmentsOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "UpdateEnvironmentOutputTypeDef",
+    "NetworkConfigurationUnionTypeDef",
     "LastUpdateTypeDef",
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "LoggingConfigurationInputTypeDef",
     "LoggingConfigurationTypeDef",
     "MetricDatumTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
     "EnvironmentTypeDef",
     "PublishMetricsInputRequestTypeDef",
@@ -68,56 +71,41 @@
 CreateCliTokenRequestRequestTypeDef = TypedDict(
     "CreateCliTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-CreateCliTokenResponseTypeDef = TypedDict(
-    "CreateCliTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CliToken": str,
-        "WebServerHostname": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
-CreateEnvironmentOutputTypeDef = TypedDict(
-    "CreateEnvironmentOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateWebLoginTokenRequestRequestTypeDef = TypedDict(
     "CreateWebLoginTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-CreateWebLoginTokenResponseTypeDef = TypedDict(
-    "CreateWebLoginTokenResponseTypeDef",
-    {
-        "WebServerHostname": str,
-        "WebToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEnvironmentInputRequestTypeDef = TypedDict(
     "DeleteEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -125,14 +113,23 @@
     "DimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+    },
+    total=False,
+)
+
 GetEnvironmentInputRequestTypeDef = TypedDict(
     "GetEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -141,55 +138,40 @@
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
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
 
 ListEnvironmentsInputRequestTypeDef = TypedDict(
     "ListEnvironmentsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListEnvironmentsOutputTypeDef = TypedDict(
-    "ListEnvironmentsOutputTypeDef",
-    {
-        "Environments": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 ModuleLoggingConfigurationInputTypeDef = TypedDict(
     "ModuleLoggingConfigurationInputTypeDef",
     {
         "Enabled": bool,
         "LogLevel": LoggingLevelType,
     },
 )
@@ -211,35 +193,15 @@
         "Minimum": float,
         "SampleCount": int,
         "Sum": float,
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
+TimestampTypeDef = Union[datetime, str]
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -255,33 +217,87 @@
 UpdateNetworkConfigurationInputTypeDef = TypedDict(
     "UpdateNetworkConfigurationInputTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
 )
 
+CreateCliTokenResponseTypeDef = TypedDict(
+    "CreateCliTokenResponseTypeDef",
+    {
+        "CliToken": str,
+        "WebServerHostname": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEnvironmentOutputTypeDef = TypedDict(
+    "CreateEnvironmentOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWebLoginTokenResponseTypeDef = TypedDict(
+    "CreateWebLoginTokenResponseTypeDef",
+    {
+        "WebServerHostname": str,
+        "WebToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEnvironmentsOutputTypeDef = TypedDict(
+    "ListEnvironmentsOutputTypeDef",
+    {
+        "Environments": List[str],
+        "NextToken": str,
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
 UpdateEnvironmentOutputTypeDef = TypedDict(
     "UpdateEnvironmentOutputTypeDef",
     {
         "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NetworkConfigurationUnionTypeDef = Union[
+    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+]
 LastUpdateTypeDef = TypedDict(
     "LastUpdateTypeDef",
     {
         "CreatedAt": datetime,
         "Error": UpdateErrorTypeDef,
         "Source": str,
         "Status": UpdateStatusType,
     },
     total=False,
 )
 
+ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 LoggingConfigurationInputTypeDef = TypedDict(
     "LoggingConfigurationInputTypeDef",
     {
         "DagProcessingLogs": ModuleLoggingConfigurationInputTypeDef,
         "SchedulerLogs": ModuleLoggingConfigurationInputTypeDef,
         "TaskLogs": ModuleLoggingConfigurationInputTypeDef,
         "WebserverLogs": ModuleLoggingConfigurationInputTypeDef,
@@ -302,15 +318,15 @@
     total=False,
 )
 
 _RequiredMetricDatumTypeDef = TypedDict(
     "_RequiredMetricDatumTypeDef",
     {
         "MetricName": str,
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
     },
 )
 _OptionalMetricDatumTypeDef = TypedDict(
     "_OptionalMetricDatumTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
         "StatisticValues": StatisticSetTypeDef,
@@ -417,15 +433,15 @@
         "ExecutionRoleArn": str,
         "KmsKey": str,
         "LastUpdate": LastUpdateTypeDef,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "MaxWorkers": int,
         "MinWorkers": int,
         "Name": str,
-        "NetworkConfiguration": NetworkConfigurationTypeDef,
+        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
         "PluginsS3ObjectVersion": str,
         "PluginsS3Path": str,
         "RequirementsS3ObjectVersion": str,
         "RequirementsS3Path": str,
         "Schedulers": int,
         "ServiceRoleArn": str,
         "SourceBucketArn": str,
@@ -448,10 +464,10 @@
     },
 )
 
 GetEnvironmentOutputTypeDef = TypedDict(
     "GetEnvironmentOutputTypeDef",
     {
         "Environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa/type_defs.pyi` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_mwaa.type_defs import CreateCliTokenRequestRequestTypeDef
 
-    data: CreateCliTokenRequestRequestTypeDef = {...}
+    data: CreateCliTokenRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -26,38 +26,41 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CreateCliTokenRequestRequestTypeDef",
-    "CreateCliTokenResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "NetworkConfigurationTypeDef",
-    "CreateEnvironmentOutputTypeDef",
     "CreateWebLoginTokenRequestRequestTypeDef",
-    "CreateWebLoginTokenResponseTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DimensionTypeDef",
+    "NetworkConfigurationOutputTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "UpdateErrorTypeDef",
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
-    "ListEnvironmentsOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ModuleLoggingConfigurationInputTypeDef",
     "ModuleLoggingConfigurationTypeDef",
     "StatisticSetTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateNetworkConfigurationInputTypeDef",
+    "CreateCliTokenResponseTypeDef",
+    "CreateEnvironmentOutputTypeDef",
+    "CreateWebLoginTokenResponseTypeDef",
+    "ListEnvironmentsOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "UpdateEnvironmentOutputTypeDef",
+    "NetworkConfigurationUnionTypeDef",
     "LastUpdateTypeDef",
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "LoggingConfigurationInputTypeDef",
     "LoggingConfigurationTypeDef",
     "MetricDatumTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
     "EnvironmentTypeDef",
     "PublishMetricsInputRequestTypeDef",
@@ -67,56 +70,41 @@
 CreateCliTokenRequestRequestTypeDef = TypedDict(
     "CreateCliTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-CreateCliTokenResponseTypeDef = TypedDict(
-    "CreateCliTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CliToken": str,
-        "WebServerHostname": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
-CreateEnvironmentOutputTypeDef = TypedDict(
-    "CreateEnvironmentOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateWebLoginTokenRequestRequestTypeDef = TypedDict(
     "CreateWebLoginTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-CreateWebLoginTokenResponseTypeDef = TypedDict(
-    "CreateWebLoginTokenResponseTypeDef",
-    {
-        "WebServerHostname": str,
-        "WebToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEnvironmentInputRequestTypeDef = TypedDict(
     "DeleteEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -124,14 +112,23 @@
     "DimensionTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
 
+NetworkConfigurationOutputTypeDef = TypedDict(
+    "NetworkConfigurationOutputTypeDef",
+    {
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+    },
+    total=False,
+)
+
 GetEnvironmentInputRequestTypeDef = TypedDict(
     "GetEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -140,55 +137,40 @@
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
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
 
 ListEnvironmentsInputRequestTypeDef = TypedDict(
     "ListEnvironmentsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListEnvironmentsOutputTypeDef = TypedDict(
-    "ListEnvironmentsOutputTypeDef",
-    {
-        "Environments": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 ModuleLoggingConfigurationInputTypeDef = TypedDict(
     "ModuleLoggingConfigurationInputTypeDef",
     {
         "Enabled": bool,
         "LogLevel": LoggingLevelType,
     },
 )
@@ -210,35 +192,15 @@
         "Minimum": float,
         "SampleCount": int,
         "Sum": float,
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
+TimestampTypeDef = Union[datetime, str]
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -254,33 +216,87 @@
 UpdateNetworkConfigurationInputTypeDef = TypedDict(
     "UpdateNetworkConfigurationInputTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
 )
 
+CreateCliTokenResponseTypeDef = TypedDict(
+    "CreateCliTokenResponseTypeDef",
+    {
+        "CliToken": str,
+        "WebServerHostname": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEnvironmentOutputTypeDef = TypedDict(
+    "CreateEnvironmentOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWebLoginTokenResponseTypeDef = TypedDict(
+    "CreateWebLoginTokenResponseTypeDef",
+    {
+        "WebServerHostname": str,
+        "WebToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEnvironmentsOutputTypeDef = TypedDict(
+    "ListEnvironmentsOutputTypeDef",
+    {
+        "Environments": List[str],
+        "NextToken": str,
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
 UpdateEnvironmentOutputTypeDef = TypedDict(
     "UpdateEnvironmentOutputTypeDef",
     {
         "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+NetworkConfigurationUnionTypeDef = Union[
+    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
+]
 LastUpdateTypeDef = TypedDict(
     "LastUpdateTypeDef",
     {
         "CreatedAt": datetime,
         "Error": UpdateErrorTypeDef,
         "Source": str,
         "Status": UpdateStatusType,
     },
     total=False,
 )
 
+ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 LoggingConfigurationInputTypeDef = TypedDict(
     "LoggingConfigurationInputTypeDef",
     {
         "DagProcessingLogs": ModuleLoggingConfigurationInputTypeDef,
         "SchedulerLogs": ModuleLoggingConfigurationInputTypeDef,
         "TaskLogs": ModuleLoggingConfigurationInputTypeDef,
         "WebserverLogs": ModuleLoggingConfigurationInputTypeDef,
@@ -301,15 +317,15 @@
     total=False,
 )
 
 _RequiredMetricDatumTypeDef = TypedDict(
     "_RequiredMetricDatumTypeDef",
     {
         "MetricName": str,
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
     },
 )
 _OptionalMetricDatumTypeDef = TypedDict(
     "_OptionalMetricDatumTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
         "StatisticValues": StatisticSetTypeDef,
@@ -410,15 +426,15 @@
         "ExecutionRoleArn": str,
         "KmsKey": str,
         "LastUpdate": LastUpdateTypeDef,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
         "MaxWorkers": int,
         "MinWorkers": int,
         "Name": str,
-        "NetworkConfiguration": NetworkConfigurationTypeDef,
+        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
         "PluginsS3ObjectVersion": str,
         "PluginsS3Path": str,
         "RequirementsS3ObjectVersion": str,
         "RequirementsS3Path": str,
         "Schedulers": int,
         "ServiceRoleArn": str,
         "SourceBucketArn": str,
@@ -441,10 +457,10 @@
     },
 )
 
 GetEnvironmentOutputTypeDef = TypedDict(
     "GetEnvironmentOutputTypeDef",
     {
         "Environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa.egg-info/PKG-INFO` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mwaa
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.MWAA 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.MWAA 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore mwaa type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore mwaa type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-mwaa"></a>
 
 # types-aiobotocore-mwaa
 
 [![PyPI - types-aiobotocore-mwaa](https://img.shields.io/pypi/v/types-aiobotocore-mwaa.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mwaa)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mwaa.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mwaa)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-mwaa?color=blue)](https://pypistats.org/packages/types-aiobotocore-mwaa)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mwaa)](https://pepy.tech/project/types-aiobotocore-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MWAA 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
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
 [types-aiobotocore-mwaa docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mwaa/).
 
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
@@ -310,60 +309,63 @@
 )
 
 
 def check_value(value: EnvironmentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_mwaa.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_mwaa.type_defs import (
     CreateCliTokenRequestRequestTypeDef,
-    CreateCliTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     NetworkConfigurationTypeDef,
-    CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenRequestRequestTypeDef,
-    CreateWebLoginTokenResponseTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DimensionTypeDef,
+    NetworkConfigurationOutputTypeDef,
     GetEnvironmentInputRequestTypeDef,
     UpdateErrorTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEnvironmentsInputRequestTypeDef,
-    ListEnvironmentsOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ModuleLoggingConfigurationInputTypeDef,
     ModuleLoggingConfigurationTypeDef,
     StatisticSetTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    TimestampTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
+    CreateCliTokenResponseTypeDef,
+    CreateEnvironmentOutputTypeDef,
+    CreateWebLoginTokenResponseTypeDef,
+    ListEnvironmentsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
+    NetworkConfigurationUnionTypeDef,
     LastUpdateTypeDef,
+    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     LoggingConfigurationInputTypeDef,
     LoggingConfigurationTypeDef,
     MetricDatumTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     EnvironmentTypeDef,
     PublishMetricsInputRequestTypeDef,
     GetEnvironmentOutputTypeDef,
 )
 
 
-def get_structure() -> CreateCliTokenRequestRequestTypeDef:
+def get_value() -> CreateCliTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-mwaa-2.5.2/types_aiobotocore_mwaa.egg-info/SOURCES.txt` & `types-aiobotocore-mwaa-2.5.2.post1/types_aiobotocore_mwaa.egg-info/SOURCES.txt`

 * *Files identical despite different names*


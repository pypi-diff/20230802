# Comparing `tmp/types-aiobotocore-simspaceweaver-2.5.2.tar.gz` & `tmp/types-aiobotocore-simspaceweaver-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-simspaceweaver-2.5.2.tar", last modified: Sat Jul  8 01:44:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-simspaceweaver-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:02 2023, max compression
```

## Comparing `types-aiobotocore-simspaceweaver-2.5.2.tar` & `types-aiobotocore-simspaceweaver-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.550910 types-aiobotocore-simspaceweaver-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-07-08 01:44:20.550910 types-aiobotocore-simspaceweaver-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:20.550910 types-aiobotocore-simspaceweaver-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.546910 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13255 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:10.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.550910 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-07-08 01:44:20.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-08 01:44:20.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:20.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:20.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:20.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:44:20.000000 types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.021454 types-aiobotocore-simspaceweaver-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-08-02 14:53:02.021454 types-aiobotocore-simspaceweaver-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:02.021454 types-aiobotocore-simspaceweaver-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.021454 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:47.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.021454 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13823 2023-08-02 14:53:01.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 14:53:01.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:01.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:53:01.000000 types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/LICENSE` & `types-aiobotocore-simspaceweaver-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/PKG-INFO` & `types-aiobotocore-simspaceweaver-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-simspaceweaver
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore simspaceweaver type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore simspaceweaver type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-simspaceweaver"></a>
 
 # types-aiobotocore-simspaceweaver
 
 [![PyPI - types-aiobotocore-simspaceweaver](https://img.shields.io/pypi/v/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-simspaceweaver?color=blue)](https://pypistats.org/packages/types-aiobotocore-simspaceweaver)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-simspaceweaver)](https://pepy.tech/project/types-aiobotocore-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SimSpaceWeaver 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [types-aiobotocore-simspaceweaver docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/).
 
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
@@ -287,64 +286,66 @@
 )
 
 
 def check_value(value: ClockStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_simspaceweaver.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_simspaceweaver.type_defs import (
     CloudWatchLogsLogGroupTypeDef,
     S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
-    LaunchOverridesTypeDef,
+    LaunchOverridesOutputTypeDef,
+    ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
     S3LocationTypeDef,
     DomainTypeDef,
+    LaunchOverridesTypeDef,
     ListAppsInputRequestTypeDef,
     SimulationAppMetadataTypeDef,
     ListSimulationsInputRequestTypeDef,
     SimulationMetadataTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     SimulationClockTypeDef,
-    ResponseMetadataTypeDef,
     SimulationAppPortMappingTypeDef,
-    StartAppOutputTypeDef,
     StartClockInputRequestTypeDef,
-    StartSimulationOutputTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
     CreateSnapshotInputRequestTypeDef,
-    StartAppInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    StartAppOutputTypeDef,
+    StartSimulationOutputTypeDef,
     StartSimulationInputRequestTypeDef,
+    LaunchOverridesUnionTypeDef,
+    StartAppInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     LiveSimulationStateTypeDef,
     SimulationAppEndpointInfoTypeDef,
     LoggingConfigurationTypeDef,
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLogsLogGroupTypeDef:
+def get_value() -> CloudWatchLogsLogGroupTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/README.md` & `types-aiobotocore-simspaceweaver-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-simspaceweaver"></a>
 
 # types-aiobotocore-simspaceweaver
 
 [![PyPI - types-aiobotocore-simspaceweaver](https://img.shields.io/pypi/v/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-simspaceweaver?color=blue)](https://pypistats.org/packages/types-aiobotocore-simspaceweaver)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-simspaceweaver)](https://pepy.tech/project/types-aiobotocore-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SimSpaceWeaver 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [types-aiobotocore-simspaceweaver docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/).
 
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
@@ -254,64 +254,66 @@
 )
 
 
 def check_value(value: ClockStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_simspaceweaver.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_simspaceweaver.type_defs import (
     CloudWatchLogsLogGroupTypeDef,
     S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
-    LaunchOverridesTypeDef,
+    LaunchOverridesOutputTypeDef,
+    ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
     S3LocationTypeDef,
     DomainTypeDef,
+    LaunchOverridesTypeDef,
     ListAppsInputRequestTypeDef,
     SimulationAppMetadataTypeDef,
     ListSimulationsInputRequestTypeDef,
     SimulationMetadataTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     SimulationClockTypeDef,
-    ResponseMetadataTypeDef,
     SimulationAppPortMappingTypeDef,
-    StartAppOutputTypeDef,
     StartClockInputRequestTypeDef,
-    StartSimulationOutputTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
     CreateSnapshotInputRequestTypeDef,
-    StartAppInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    StartAppOutputTypeDef,
+    StartSimulationOutputTypeDef,
     StartSimulationInputRequestTypeDef,
+    LaunchOverridesUnionTypeDef,
+    StartAppInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     LiveSimulationStateTypeDef,
     SimulationAppEndpointInfoTypeDef,
     LoggingConfigurationTypeDef,
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLogsLogGroupTypeDef:
+def get_value() -> CloudWatchLogsLogGroupTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/setup.py` & `types-aiobotocore-simspaceweaver-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-simspaceweaver",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_simspaceweaver"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with"
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
-    keywords="aiobotocore simspaceweaver type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore simspaceweaver type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_simspaceweaver": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/"
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/__main__.py` & `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SimSpaceWeaver 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SimSpaceWeaver 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver\nOther"
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

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/client.py` & `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
-    LaunchOverridesTypeDef,
+    LaunchOverridesUnionTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     S3DestinationTypeDef,
     S3LocationTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
@@ -178,15 +178,15 @@
         self,
         *,
         Domain: str,
         Name: str,
         Simulation: str,
         ClientToken: str = ...,
         Description: str = ...,
-        LaunchOverrides: LaunchOverridesTypeDef = ...
+        LaunchOverrides: LaunchOverridesUnionTypeDef = ...
     ) -> StartAppOutputTypeDef:
         """
         Starts a custom app with the configuration specified in the simulation schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.start_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/client/#start_app)
         """
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/client.pyi` & `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
-    LaunchOverridesTypeDef,
+    LaunchOverridesUnionTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     S3DestinationTypeDef,
     S3LocationTypeDef,
     StartAppOutputTypeDef,
     StartSimulationOutputTypeDef,
@@ -163,15 +163,15 @@
         self,
         *,
         Domain: str,
         Name: str,
         Simulation: str,
         ClientToken: str = ...,
         Description: str = ...,
-        LaunchOverrides: LaunchOverridesTypeDef = ...
+        LaunchOverrides: LaunchOverridesUnionTypeDef = ...
     ) -> StartAppOutputTypeDef:
         """
         Starts a custom app with the configuration specified in the simulation schema.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver.Client.start_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/client/#start_app)
         """
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/literals.py` & `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/literals.pyi` & `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/type_defs.py` & `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_simspaceweaver.type_defs import CloudWatchLogsLogGroupTypeDef
 
-    data: CloudWatchLogsLogGroupTypeDef = {...}
+    data: CloudWatchLogsLogGroupTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ClockStatusType,
     ClockTargetStatusType,
     LifecycleManagementStrategyType,
     SimulationAppStatusType,
     SimulationAppTargetStatusType,
@@ -33,39 +33,41 @@
 
 __all__ = (
     "CloudWatchLogsLogGroupTypeDef",
     "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
-    "LaunchOverridesTypeDef",
+    "LaunchOverridesOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeSimulationInputRequestTypeDef",
     "S3LocationTypeDef",
     "DomainTypeDef",
+    "LaunchOverridesTypeDef",
     "ListAppsInputRequestTypeDef",
     "SimulationAppMetadataTypeDef",
     "ListSimulationsInputRequestTypeDef",
     "SimulationMetadataTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "SimulationClockTypeDef",
-    "ResponseMetadataTypeDef",
     "SimulationAppPortMappingTypeDef",
-    "StartAppOutputTypeDef",
     "StartClockInputRequestTypeDef",
-    "StartSimulationOutputTypeDef",
     "StopAppInputRequestTypeDef",
     "StopClockInputRequestTypeDef",
     "StopSimulationInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "LogDestinationTypeDef",
     "CreateSnapshotInputRequestTypeDef",
-    "StartAppInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "StartAppOutputTypeDef",
+    "StartSimulationOutputTypeDef",
     "StartSimulationInputRequestTypeDef",
+    "LaunchOverridesUnionTypeDef",
+    "StartAppInputRequestTypeDef",
     "ListAppsOutputTypeDef",
     "ListSimulationsOutputTypeDef",
     "LiveSimulationStateTypeDef",
     "SimulationAppEndpointInfoTypeDef",
     "LoggingConfigurationTypeDef",
     "DescribeAppOutputTypeDef",
     "DescribeSimulationOutputTypeDef",
@@ -109,22 +111,33 @@
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
 )
 
-LaunchOverridesTypeDef = TypedDict(
-    "LaunchOverridesTypeDef",
+LaunchOverridesOutputTypeDef = TypedDict(
+    "LaunchOverridesOutputTypeDef",
     {
         "LaunchCommands": List[str],
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
 DescribeSimulationInputRequestTypeDef = TypedDict(
     "DescribeSimulationInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
@@ -142,14 +155,22 @@
     {
         "Lifecycle": LifecycleManagementStrategyType,
         "Name": str,
     },
     total=False,
 )
 
+LaunchOverridesTypeDef = TypedDict(
+    "LaunchOverridesTypeDef",
+    {
+        "LaunchCommands": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredListAppsInputRequestTypeDef = TypedDict(
     "_RequiredListAppsInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 _OptionalListAppsInputRequestTypeDef = TypedDict(
@@ -205,78 +226,39 @@
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
 SimulationClockTypeDef = TypedDict(
     "SimulationClockTypeDef",
     {
         "Status": ClockStatusType,
         "TargetStatus": ClockTargetStatusType,
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
 SimulationAppPortMappingTypeDef = TypedDict(
     "SimulationAppPortMappingTypeDef",
     {
         "Actual": int,
         "Declared": int,
     },
     total=False,
 )
 
-StartAppOutputTypeDef = TypedDict(
-    "StartAppOutputTypeDef",
-    {
-        "Domain": str,
-        "Name": str,
-        "Simulation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartClockInputRequestTypeDef = TypedDict(
     "StartClockInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
-StartSimulationOutputTypeDef = TypedDict(
-    "StartSimulationOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "ExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopAppInputRequestTypeDef = TypedDict(
     "StopAppInputRequestTypeDef",
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
@@ -324,39 +306,42 @@
     "CreateSnapshotInputRequestTypeDef",
     {
         "Destination": S3DestinationTypeDef,
         "Simulation": str,
     },
 )
 
-_RequiredStartAppInputRequestTypeDef = TypedDict(
-    "_RequiredStartAppInputRequestTypeDef",
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAppOutputTypeDef = TypedDict(
+    "StartAppOutputTypeDef",
     {
         "Domain": str,
         "Name": str,
         "Simulation": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartAppInputRequestTypeDef = TypedDict(
-    "_OptionalStartAppInputRequestTypeDef",
+
+StartSimulationOutputTypeDef = TypedDict(
+    "StartSimulationOutputTypeDef",
     {
-        "ClientToken": str,
-        "Description": str,
-        "LaunchOverrides": LaunchOverridesTypeDef,
+        "Arn": str,
+        "CreationTime": datetime,
+        "ExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class StartAppInputRequestTypeDef(
-    _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
-):
-    pass
-
-
 _RequiredStartSimulationInputRequestTypeDef = TypedDict(
     "_RequiredStartSimulationInputRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
     },
 )
@@ -376,29 +361,55 @@
 
 class StartSimulationInputRequestTypeDef(
     _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
 ):
     pass
 
 
+LaunchOverridesUnionTypeDef = Union[LaunchOverridesTypeDef, LaunchOverridesOutputTypeDef]
+_RequiredStartAppInputRequestTypeDef = TypedDict(
+    "_RequiredStartAppInputRequestTypeDef",
+    {
+        "Domain": str,
+        "Name": str,
+        "Simulation": str,
+    },
+)
+_OptionalStartAppInputRequestTypeDef = TypedDict(
+    "_OptionalStartAppInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+        "LaunchOverrides": LaunchOverridesTypeDef,
+    },
+    total=False,
+)
+
+
+class StartAppInputRequestTypeDef(
+    _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
+):
+    pass
+
+
 ListAppsOutputTypeDef = TypedDict(
     "ListAppsOutputTypeDef",
     {
         "Apps": List[SimulationAppMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSimulationsOutputTypeDef = TypedDict(
     "ListSimulationsOutputTypeDef",
     {
         "NextToken": str,
         "Simulations": List[SimulationMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LiveSimulationStateTypeDef = TypedDict(
     "LiveSimulationStateTypeDef",
     {
         "Clocks": List[SimulationClockTypeDef],
@@ -426,20 +437,20 @@
 
 DescribeAppOutputTypeDef = TypedDict(
     "DescribeAppOutputTypeDef",
     {
         "Description": str,
         "Domain": str,
         "EndpointInfo": SimulationAppEndpointInfoTypeDef,
-        "LaunchOverrides": LaunchOverridesTypeDef,
+        "LaunchOverrides": LaunchOverridesOutputTypeDef,
         "Name": str,
         "Simulation": str,
         "Status": SimulationAppStatusType,
         "TargetStatus": SimulationAppTargetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationOutputTypeDef = TypedDict(
     "DescribeSimulationOutputTypeDef",
     {
         "Arn": str,
@@ -453,10 +464,10 @@
         "RoleArn": str,
         "SchemaError": str,
         "SchemaS3Location": S3LocationTypeDef,
         "SnapshotS3Location": S3LocationTypeDef,
         "StartError": str,
         "Status": SimulationStatusType,
         "TargetStatus": SimulationTargetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver/type_defs.pyi` & `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_simspaceweaver.type_defs import CloudWatchLogsLogGroupTypeDef
 
-    data: CloudWatchLogsLogGroupTypeDef = {...}
+    data: CloudWatchLogsLogGroupTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ClockStatusType,
     ClockTargetStatusType,
     LifecycleManagementStrategyType,
     SimulationAppStatusType,
     SimulationAppTargetStatusType,
@@ -32,39 +32,41 @@
 
 __all__ = (
     "CloudWatchLogsLogGroupTypeDef",
     "S3DestinationTypeDef",
     "DeleteAppInputRequestTypeDef",
     "DeleteSimulationInputRequestTypeDef",
     "DescribeAppInputRequestTypeDef",
-    "LaunchOverridesTypeDef",
+    "LaunchOverridesOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeSimulationInputRequestTypeDef",
     "S3LocationTypeDef",
     "DomainTypeDef",
+    "LaunchOverridesTypeDef",
     "ListAppsInputRequestTypeDef",
     "SimulationAppMetadataTypeDef",
     "ListSimulationsInputRequestTypeDef",
     "SimulationMetadataTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "SimulationClockTypeDef",
-    "ResponseMetadataTypeDef",
     "SimulationAppPortMappingTypeDef",
-    "StartAppOutputTypeDef",
     "StartClockInputRequestTypeDef",
-    "StartSimulationOutputTypeDef",
     "StopAppInputRequestTypeDef",
     "StopClockInputRequestTypeDef",
     "StopSimulationInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "LogDestinationTypeDef",
     "CreateSnapshotInputRequestTypeDef",
-    "StartAppInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "StartAppOutputTypeDef",
+    "StartSimulationOutputTypeDef",
     "StartSimulationInputRequestTypeDef",
+    "LaunchOverridesUnionTypeDef",
+    "StartAppInputRequestTypeDef",
     "ListAppsOutputTypeDef",
     "ListSimulationsOutputTypeDef",
     "LiveSimulationStateTypeDef",
     "SimulationAppEndpointInfoTypeDef",
     "LoggingConfigurationTypeDef",
     "DescribeAppOutputTypeDef",
     "DescribeSimulationOutputTypeDef",
@@ -108,22 +110,33 @@
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
 )
 
-LaunchOverridesTypeDef = TypedDict(
-    "LaunchOverridesTypeDef",
+LaunchOverridesOutputTypeDef = TypedDict(
+    "LaunchOverridesOutputTypeDef",
     {
         "LaunchCommands": List[str],
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
 DescribeSimulationInputRequestTypeDef = TypedDict(
     "DescribeSimulationInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
@@ -141,14 +154,22 @@
     {
         "Lifecycle": LifecycleManagementStrategyType,
         "Name": str,
     },
     total=False,
 )
 
+LaunchOverridesTypeDef = TypedDict(
+    "LaunchOverridesTypeDef",
+    {
+        "LaunchCommands": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredListAppsInputRequestTypeDef = TypedDict(
     "_RequiredListAppsInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 _OptionalListAppsInputRequestTypeDef = TypedDict(
@@ -202,78 +223,39 @@
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
 SimulationClockTypeDef = TypedDict(
     "SimulationClockTypeDef",
     {
         "Status": ClockStatusType,
         "TargetStatus": ClockTargetStatusType,
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
 SimulationAppPortMappingTypeDef = TypedDict(
     "SimulationAppPortMappingTypeDef",
     {
         "Actual": int,
         "Declared": int,
     },
     total=False,
 )
 
-StartAppOutputTypeDef = TypedDict(
-    "StartAppOutputTypeDef",
-    {
-        "Domain": str,
-        "Name": str,
-        "Simulation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartClockInputRequestTypeDef = TypedDict(
     "StartClockInputRequestTypeDef",
     {
         "Simulation": str,
     },
 )
 
-StartSimulationOutputTypeDef = TypedDict(
-    "StartSimulationOutputTypeDef",
-    {
-        "Arn": str,
-        "CreationTime": datetime,
-        "ExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopAppInputRequestTypeDef = TypedDict(
     "StopAppInputRequestTypeDef",
     {
         "App": str,
         "Domain": str,
         "Simulation": str,
     },
@@ -321,37 +303,42 @@
     "CreateSnapshotInputRequestTypeDef",
     {
         "Destination": S3DestinationTypeDef,
         "Simulation": str,
     },
 )
 
-_RequiredStartAppInputRequestTypeDef = TypedDict(
-    "_RequiredStartAppInputRequestTypeDef",
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAppOutputTypeDef = TypedDict(
+    "StartAppOutputTypeDef",
     {
         "Domain": str,
         "Name": str,
         "Simulation": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartAppInputRequestTypeDef = TypedDict(
-    "_OptionalStartAppInputRequestTypeDef",
+
+StartSimulationOutputTypeDef = TypedDict(
+    "StartSimulationOutputTypeDef",
     {
-        "ClientToken": str,
-        "Description": str,
-        "LaunchOverrides": LaunchOverridesTypeDef,
+        "Arn": str,
+        "CreationTime": datetime,
+        "ExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class StartAppInputRequestTypeDef(
-    _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
-):
-    pass
-
 _RequiredStartSimulationInputRequestTypeDef = TypedDict(
     "_RequiredStartSimulationInputRequestTypeDef",
     {
         "Name": str,
         "RoleArn": str,
     },
 )
@@ -369,29 +356,53 @@
 )
 
 class StartSimulationInputRequestTypeDef(
     _RequiredStartSimulationInputRequestTypeDef, _OptionalStartSimulationInputRequestTypeDef
 ):
     pass
 
+LaunchOverridesUnionTypeDef = Union[LaunchOverridesTypeDef, LaunchOverridesOutputTypeDef]
+_RequiredStartAppInputRequestTypeDef = TypedDict(
+    "_RequiredStartAppInputRequestTypeDef",
+    {
+        "Domain": str,
+        "Name": str,
+        "Simulation": str,
+    },
+)
+_OptionalStartAppInputRequestTypeDef = TypedDict(
+    "_OptionalStartAppInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+        "LaunchOverrides": LaunchOverridesTypeDef,
+    },
+    total=False,
+)
+
+class StartAppInputRequestTypeDef(
+    _RequiredStartAppInputRequestTypeDef, _OptionalStartAppInputRequestTypeDef
+):
+    pass
+
 ListAppsOutputTypeDef = TypedDict(
     "ListAppsOutputTypeDef",
     {
         "Apps": List[SimulationAppMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSimulationsOutputTypeDef = TypedDict(
     "ListSimulationsOutputTypeDef",
     {
         "NextToken": str,
         "Simulations": List[SimulationMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LiveSimulationStateTypeDef = TypedDict(
     "LiveSimulationStateTypeDef",
     {
         "Clocks": List[SimulationClockTypeDef],
@@ -419,20 +430,20 @@
 
 DescribeAppOutputTypeDef = TypedDict(
     "DescribeAppOutputTypeDef",
     {
         "Description": str,
         "Domain": str,
         "EndpointInfo": SimulationAppEndpointInfoTypeDef,
-        "LaunchOverrides": LaunchOverridesTypeDef,
+        "LaunchOverrides": LaunchOverridesOutputTypeDef,
         "Name": str,
         "Simulation": str,
         "Status": SimulationAppStatusType,
         "TargetStatus": SimulationAppTargetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationOutputTypeDef = TypedDict(
     "DescribeSimulationOutputTypeDef",
     {
         "Arn": str,
@@ -446,10 +457,10 @@
         "RoleArn": str,
         "SchemaError": str,
         "SchemaS3Location": S3LocationTypeDef,
         "SnapshotS3Location": S3LocationTypeDef,
         "StartError": str,
         "Status": SimulationStatusType,
         "TargetStatus": SimulationTargetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO` & `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-simspaceweaver
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SimSpaceWeaver 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore simspaceweaver type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore simspaceweaver type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-simspaceweaver"></a>
 
 # types-aiobotocore-simspaceweaver
 
 [![PyPI - types-aiobotocore-simspaceweaver](https://img.shields.io/pypi/v/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-simspaceweaver.svg?color=blue)](https://pypi.org/project/types-aiobotocore-simspaceweaver)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-simspaceweaver?color=blue)](https://pypistats.org/packages/types-aiobotocore-simspaceweaver)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-simspaceweaver)](https://pepy.tech/project/types-aiobotocore-simspaceweaver)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SimSpaceWeaver 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#SimSpaceWeaver)
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
 [types-aiobotocore-simspaceweaver docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_simspaceweaver/).
 
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
@@ -287,64 +286,66 @@
 )
 
 
 def check_value(value: ClockStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_simspaceweaver.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_simspaceweaver.type_defs import (
     CloudWatchLogsLogGroupTypeDef,
     S3DestinationTypeDef,
     DeleteAppInputRequestTypeDef,
     DeleteSimulationInputRequestTypeDef,
     DescribeAppInputRequestTypeDef,
-    LaunchOverridesTypeDef,
+    LaunchOverridesOutputTypeDef,
+    ResponseMetadataTypeDef,
     DescribeSimulationInputRequestTypeDef,
     S3LocationTypeDef,
     DomainTypeDef,
+    LaunchOverridesTypeDef,
     ListAppsInputRequestTypeDef,
     SimulationAppMetadataTypeDef,
     ListSimulationsInputRequestTypeDef,
     SimulationMetadataTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     SimulationClockTypeDef,
-    ResponseMetadataTypeDef,
     SimulationAppPortMappingTypeDef,
-    StartAppOutputTypeDef,
     StartClockInputRequestTypeDef,
-    StartSimulationOutputTypeDef,
     StopAppInputRequestTypeDef,
     StopClockInputRequestTypeDef,
     StopSimulationInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     LogDestinationTypeDef,
     CreateSnapshotInputRequestTypeDef,
-    StartAppInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    StartAppOutputTypeDef,
+    StartSimulationOutputTypeDef,
     StartSimulationInputRequestTypeDef,
+    LaunchOverridesUnionTypeDef,
+    StartAppInputRequestTypeDef,
     ListAppsOutputTypeDef,
     ListSimulationsOutputTypeDef,
     LiveSimulationStateTypeDef,
     SimulationAppEndpointInfoTypeDef,
     LoggingConfigurationTypeDef,
     DescribeAppOutputTypeDef,
     DescribeSimulationOutputTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLogsLogGroupTypeDef:
+def get_value() -> CloudWatchLogsLogGroupTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-simspaceweaver-2.5.2/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt` & `types-aiobotocore-simspaceweaver-2.5.2.post1/types_aiobotocore_simspaceweaver.egg-info/SOURCES.txt`

 * *Files identical despite different names*


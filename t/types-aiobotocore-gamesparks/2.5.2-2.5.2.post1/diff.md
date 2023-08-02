# Comparing `tmp/types-aiobotocore-gamesparks-2.5.2.tar.gz` & `tmp/types-aiobotocore-gamesparks-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-gamesparks-2.5.2.tar", last modified: Sat Jul  8 01:43:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-gamesparks-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:19 2023, max compression
```

## Comparing `types-aiobotocore-gamesparks-2.5.2.tar` & `types-aiobotocore-gamesparks-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:40.054177 types-aiobotocore-gamesparks-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-07-08 01:43:40.038177 types-aiobotocore-gamesparks-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:40.054177 types-aiobotocore-gamesparks-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:40.038177 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26620 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29885 2023-07-08 01:31:21.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29842 2023-07-08 01:31:21.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:31:20.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:40.038177 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-07-08 01:43:39.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:39.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:39.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:39.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:39.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:39.000000 types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.565581 types-aiobotocore-gamesparks-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17505 2023-08-02 14:52:19.561581 types-aiobotocore-gamesparks-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:19.565581 types-aiobotocore-gamesparks-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.561581 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26620 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-08-02 14:39:14.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29844 2023-08-02 14:39:14.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29801 2023-08-02 14:39:14.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:13.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.561581 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17505 2023-08-02 14:52:19.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:19.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:19.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:19.000000 types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-gamesparks-2.5.2/LICENSE` & `types-aiobotocore-gamesparks-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2/PKG-INFO` & `types-aiobotocore-gamesparks-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-gamesparks
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.GameSparks 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.GameSparks 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore gamesparks type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore gamesparks type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-gamesparks"></a>
 
 # types-aiobotocore-gamesparks
 
 [![PyPI - types-aiobotocore-gamesparks](https://img.shields.io/pypi/v/types-aiobotocore-gamesparks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamesparks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-gamesparks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamesparks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-gamesparks?color=blue)](https://pypistats.org/packages/types-aiobotocore-gamesparks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-gamesparks)](https://pepy.tech/project/types-aiobotocore-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.GameSparks 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
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
 [types-aiobotocore-gamesparks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/).
 
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
@@ -338,36 +337,36 @@
 )
 
 
 def check_value(value: DeploymentActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_gamesparks.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_gamesparks.type_defs import (
+    BlobTypeDef,
     ConnectionTypeDef,
     CreateGameRequestRequestTypeDef,
     GameDetailsTypeDef,
+    ResponseMetadataTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateStageRequestRequestTypeDef,
     StageDetailsTypeDef,
     DeleteGameRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeploymentResultTypeDef,
     DisconnectPlayerRequestRequestTypeDef,
-    DisconnectPlayerResultTypeDef,
     ExportSnapshotRequestRequestTypeDef,
-    ExportSnapshotResultTypeDef,
     ExtensionDetailsTypeDef,
     ExtensionVersionDetailsTypeDef,
     SectionTypeDef,
     GameSummaryTypeDef,
     GeneratedCodeJobDetailsTypeDef,
     GeneratorTypeDef,
     GetExtensionRequestRequestTypeDef,
@@ -375,46 +374,40 @@
     GetGameConfigurationRequestRequestTypeDef,
     GetGameRequestRequestTypeDef,
     GetGeneratedCodeJobRequestRequestTypeDef,
     GetPlayerConnectionStatusRequestRequestTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetStageDeploymentRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    ImportGameConfigurationSourceTypeDef,
-    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListExtensionVersionsRequestRequestTypeDef,
-    ListExtensionsRequestListExtensionsPaginateTypeDef,
     ListExtensionsRequestRequestTypeDef,
-    ListGamesRequestListGamesPaginateTypeDef,
     ListGamesRequestRequestTypeDef,
-    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
     ListGeneratedCodeJobsRequestRequestTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     SnapshotSummaryTypeDef,
-    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
     ListStageDeploymentsRequestRequestTypeDef,
-    ListStagesRequestListStagesPaginateTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SectionModificationTypeDef,
-    StartGeneratedCodeJobResultTypeDef,
     StartStageDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGameRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
-    GetPlayerConnectionStatusResultTypeDef,
+    ImportGameConfigurationSourceTypeDef,
     CreateGameResultTypeDef,
+    DisconnectPlayerResultTypeDef,
+    ExportSnapshotResultTypeDef,
     GetGameResultTypeDef,
+    GetPlayerConnectionStatusResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    StartGeneratedCodeJobResultTypeDef,
     UpdateGameResultTypeDef,
     CreateStageResultTypeDef,
     GetStageResultTypeDef,
     UpdateStageResultTypeDef,
     StageDeploymentDetailsTypeDef,
     StageDeploymentSummaryTypeDef,
     GetExtensionResultTypeDef,
@@ -423,31 +416,38 @@
     ListExtensionVersionsResultTypeDef,
     GameConfigurationDetailsTypeDef,
     SnapshotDetailsTypeDef,
     ListGamesResultTypeDef,
     GetGeneratedCodeJobResultTypeDef,
     ListGeneratedCodeJobsResultTypeDef,
     StartGeneratedCodeJobRequestRequestTypeDef,
-    ImportGameConfigurationRequestRequestTypeDef,
+    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    ListExtensionsRequestListExtensionsPaginateTypeDef,
+    ListGamesRequestListGamesPaginateTypeDef,
+    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+    ListStagesRequestListStagesPaginateTypeDef,
     ListSnapshotsResultTypeDef,
     ListStagesResultTypeDef,
     UpdateGameConfigurationRequestRequestTypeDef,
+    ImportGameConfigurationRequestRequestTypeDef,
     GetStageDeploymentResultTypeDef,
     StartStageDeploymentResultTypeDef,
     ListStageDeploymentsResultTypeDef,
     GetGameConfigurationResultTypeDef,
     ImportGameConfigurationResultTypeDef,
     UpdateGameConfigurationResultTypeDef,
     CreateSnapshotResultTypeDef,
     GetSnapshotResultTypeDef,
     UpdateSnapshotResultTypeDef,
 )
 
 
-def get_structure() -> ConnectionTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-gamesparks-2.5.2/README.md` & `types-aiobotocore-gamesparks-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-gamesparks"></a>
 
 # types-aiobotocore-gamesparks
 
 [![PyPI - types-aiobotocore-gamesparks](https://img.shields.io/pypi/v/types-aiobotocore-gamesparks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamesparks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-gamesparks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamesparks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-gamesparks?color=blue)](https://pypistats.org/packages/types-aiobotocore-gamesparks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-gamesparks)](https://pepy.tech/project/types-aiobotocore-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.GameSparks 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
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
 [types-aiobotocore-gamesparks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/).
 
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
@@ -305,36 +305,36 @@
 )
 
 
 def check_value(value: DeploymentActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_gamesparks.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_gamesparks.type_defs import (
+    BlobTypeDef,
     ConnectionTypeDef,
     CreateGameRequestRequestTypeDef,
     GameDetailsTypeDef,
+    ResponseMetadataTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateStageRequestRequestTypeDef,
     StageDetailsTypeDef,
     DeleteGameRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeploymentResultTypeDef,
     DisconnectPlayerRequestRequestTypeDef,
-    DisconnectPlayerResultTypeDef,
     ExportSnapshotRequestRequestTypeDef,
-    ExportSnapshotResultTypeDef,
     ExtensionDetailsTypeDef,
     ExtensionVersionDetailsTypeDef,
     SectionTypeDef,
     GameSummaryTypeDef,
     GeneratedCodeJobDetailsTypeDef,
     GeneratorTypeDef,
     GetExtensionRequestRequestTypeDef,
@@ -342,46 +342,40 @@
     GetGameConfigurationRequestRequestTypeDef,
     GetGameRequestRequestTypeDef,
     GetGeneratedCodeJobRequestRequestTypeDef,
     GetPlayerConnectionStatusRequestRequestTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetStageDeploymentRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    ImportGameConfigurationSourceTypeDef,
-    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListExtensionVersionsRequestRequestTypeDef,
-    ListExtensionsRequestListExtensionsPaginateTypeDef,
     ListExtensionsRequestRequestTypeDef,
-    ListGamesRequestListGamesPaginateTypeDef,
     ListGamesRequestRequestTypeDef,
-    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
     ListGeneratedCodeJobsRequestRequestTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     SnapshotSummaryTypeDef,
-    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
     ListStageDeploymentsRequestRequestTypeDef,
-    ListStagesRequestListStagesPaginateTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SectionModificationTypeDef,
-    StartGeneratedCodeJobResultTypeDef,
     StartStageDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGameRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
-    GetPlayerConnectionStatusResultTypeDef,
+    ImportGameConfigurationSourceTypeDef,
     CreateGameResultTypeDef,
+    DisconnectPlayerResultTypeDef,
+    ExportSnapshotResultTypeDef,
     GetGameResultTypeDef,
+    GetPlayerConnectionStatusResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    StartGeneratedCodeJobResultTypeDef,
     UpdateGameResultTypeDef,
     CreateStageResultTypeDef,
     GetStageResultTypeDef,
     UpdateStageResultTypeDef,
     StageDeploymentDetailsTypeDef,
     StageDeploymentSummaryTypeDef,
     GetExtensionResultTypeDef,
@@ -390,31 +384,38 @@
     ListExtensionVersionsResultTypeDef,
     GameConfigurationDetailsTypeDef,
     SnapshotDetailsTypeDef,
     ListGamesResultTypeDef,
     GetGeneratedCodeJobResultTypeDef,
     ListGeneratedCodeJobsResultTypeDef,
     StartGeneratedCodeJobRequestRequestTypeDef,
-    ImportGameConfigurationRequestRequestTypeDef,
+    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    ListExtensionsRequestListExtensionsPaginateTypeDef,
+    ListGamesRequestListGamesPaginateTypeDef,
+    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+    ListStagesRequestListStagesPaginateTypeDef,
     ListSnapshotsResultTypeDef,
     ListStagesResultTypeDef,
     UpdateGameConfigurationRequestRequestTypeDef,
+    ImportGameConfigurationRequestRequestTypeDef,
     GetStageDeploymentResultTypeDef,
     StartStageDeploymentResultTypeDef,
     ListStageDeploymentsResultTypeDef,
     GetGameConfigurationResultTypeDef,
     ImportGameConfigurationResultTypeDef,
     UpdateGameConfigurationResultTypeDef,
     CreateSnapshotResultTypeDef,
     GetSnapshotResultTypeDef,
     UpdateSnapshotResultTypeDef,
 )
 
 
-def get_structure() -> ConnectionTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-gamesparks-2.5.2/setup.py` & `types-aiobotocore-gamesparks-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-gamesparks",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_gamesparks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.GameSparks 2.5.2 service generated with"
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
-    keywords="aiobotocore gamesparks type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore gamesparks type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_gamesparks": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/"
```

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/__init__.py` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/__init__.pyi` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/__main__.py` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GameSparks 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.GameSparks 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks\nOther"
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

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/client.py` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/client.pyi` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/literals.py` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/literals.pyi` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/paginator.py` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,103 +72,103 @@
 class ListExtensionVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listextensionversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, Namespace: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Name: str, Namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExtensionVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listextensionversionspaginator)
         """
 
 
 class ListExtensionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listextensionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExtensionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listextensionspaginator)
         """
 
 
 class ListGamesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listgamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGamesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listgamespaginator)
         """
 
 
 class ListGeneratedCodeJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listgeneratedcodejobspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, SnapshotId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, SnapshotId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGeneratedCodeJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listgeneratedcodejobspaginator)
         """
 
 
 class ListSnapshotsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listsnapshotspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listsnapshotspaginator)
         """
 
 
 class ListStageDeploymentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#liststagedeploymentspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, StageName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, StageName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStageDeploymentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#liststagedeploymentspaginator)
         """
 
 
 class ListStagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#liststagespaginator)
     """
 
     def paginate(
-        self, *, GameName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#liststagespaginator)
         """
```

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/paginator.pyi` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -69,97 +69,97 @@
 class ListExtensionVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listextensionversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, Namespace: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Name: str, Namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExtensionVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listextensionversionspaginator)
         """
 
 class ListExtensionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listextensionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExtensionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listextensionspaginator)
         """
 
 class ListGamesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listgamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGamesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listgamespaginator)
         """
 
 class ListGeneratedCodeJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listgeneratedcodejobspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, SnapshotId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, SnapshotId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGeneratedCodeJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listgeneratedcodejobspaginator)
         """
 
 class ListSnapshotsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listsnapshotspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#listsnapshotspaginator)
         """
 
 class ListStageDeploymentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#liststagedeploymentspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, StageName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, StageName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStageDeploymentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#liststagedeploymentspaginator)
         """
 
 class ListStagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#liststagespaginator)
     """
 
     def paginate(
-        self, *, GameName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/paginators/#liststagespaginator)
         """
```

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/type_defs.py` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for gamesparks service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_gamesparks.type_defs import ConnectionTypeDef
+    from types_aiobotocore_gamesparks.type_defs import BlobTypeDef
 
-    data: ConnectionTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -28,29 +28,28 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "BlobTypeDef",
     "ConnectionTypeDef",
     "CreateGameRequestRequestTypeDef",
     "GameDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateStageRequestRequestTypeDef",
     "StageDetailsTypeDef",
     "DeleteGameRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeploymentResultTypeDef",
     "DisconnectPlayerRequestRequestTypeDef",
-    "DisconnectPlayerResultTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
-    "ExportSnapshotResultTypeDef",
     "ExtensionDetailsTypeDef",
     "ExtensionVersionDetailsTypeDef",
     "SectionTypeDef",
     "GameSummaryTypeDef",
     "GeneratedCodeJobDetailsTypeDef",
     "GeneratorTypeDef",
     "GetExtensionRequestRequestTypeDef",
@@ -58,46 +57,40 @@
     "GetGameConfigurationRequestRequestTypeDef",
     "GetGameRequestRequestTypeDef",
     "GetGeneratedCodeJobRequestRequestTypeDef",
     "GetPlayerConnectionStatusRequestRequestTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetStageDeploymentRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
-    "ImportGameConfigurationSourceTypeDef",
-    "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListExtensionVersionsRequestRequestTypeDef",
-    "ListExtensionsRequestListExtensionsPaginateTypeDef",
     "ListExtensionsRequestRequestTypeDef",
-    "ListGamesRequestListGamesPaginateTypeDef",
     "ListGamesRequestRequestTypeDef",
-    "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
     "ListGeneratedCodeJobsRequestRequestTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
     "SnapshotSummaryTypeDef",
-    "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
     "ListStageDeploymentsRequestRequestTypeDef",
-    "ListStagesRequestListStagesPaginateTypeDef",
     "ListStagesRequestRequestTypeDef",
     "StageSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SectionModificationTypeDef",
-    "StartGeneratedCodeJobResultTypeDef",
     "StartStageDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGameRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
-    "GetPlayerConnectionStatusResultTypeDef",
+    "ImportGameConfigurationSourceTypeDef",
     "CreateGameResultTypeDef",
+    "DisconnectPlayerResultTypeDef",
+    "ExportSnapshotResultTypeDef",
     "GetGameResultTypeDef",
+    "GetPlayerConnectionStatusResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "StartGeneratedCodeJobResultTypeDef",
     "UpdateGameResultTypeDef",
     "CreateStageResultTypeDef",
     "GetStageResultTypeDef",
     "UpdateStageResultTypeDef",
     "StageDeploymentDetailsTypeDef",
     "StageDeploymentSummaryTypeDef",
     "GetExtensionResultTypeDef",
@@ -106,29 +99,37 @@
     "ListExtensionVersionsResultTypeDef",
     "GameConfigurationDetailsTypeDef",
     "SnapshotDetailsTypeDef",
     "ListGamesResultTypeDef",
     "GetGeneratedCodeJobResultTypeDef",
     "ListGeneratedCodeJobsResultTypeDef",
     "StartGeneratedCodeJobRequestRequestTypeDef",
-    "ImportGameConfigurationRequestRequestTypeDef",
+    "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    "ListExtensionsRequestListExtensionsPaginateTypeDef",
+    "ListGamesRequestListGamesPaginateTypeDef",
+    "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    "ListStagesRequestListStagesPaginateTypeDef",
     "ListSnapshotsResultTypeDef",
     "ListStagesResultTypeDef",
     "UpdateGameConfigurationRequestRequestTypeDef",
+    "ImportGameConfigurationRequestRequestTypeDef",
     "GetStageDeploymentResultTypeDef",
     "StartStageDeploymentResultTypeDef",
     "ListStageDeploymentsResultTypeDef",
     "GetGameConfigurationResultTypeDef",
     "ImportGameConfigurationResultTypeDef",
     "UpdateGameConfigurationResultTypeDef",
     "CreateSnapshotResultTypeDef",
     "GetSnapshotResultTypeDef",
     "UpdateSnapshotResultTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "Created": datetime,
         "Id": str,
     },
     total=False,
@@ -146,21 +147,19 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateGameRequestRequestTypeDef(
     _RequiredCreateGameRequestRequestTypeDef, _OptionalCreateGameRequestRequestTypeDef
 ):
     pass
 
-
 GameDetailsTypeDef = TypedDict(
     "GameDetailsTypeDef",
     {
         "Arn": str,
         "Created": datetime,
         "Description": str,
         "EnableTerminationProtection": bool,
@@ -168,35 +167,44 @@
         "Name": str,
         "State": GameStateType,
         "Tags": Dict[str, str],
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
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 _OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSnapshotRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "GameName": str,
         "Role": str,
         "StageName": str,
     },
@@ -207,21 +215,19 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStageRequestRequestTypeDef(
     _RequiredCreateStageRequestRequestTypeDef, _OptionalCreateStageRequestRequestTypeDef
 ):
     pass
 
-
 StageDetailsTypeDef = TypedDict(
     "StageDetailsTypeDef",
     {
         "Arn": str,
         "Created": datetime,
         "Description": str,
         "GameKey": str,
@@ -264,39 +270,22 @@
     {
         "GameName": str,
         "PlayerId": str,
         "StageName": str,
     },
 )
 
-DisconnectPlayerResultTypeDef = TypedDict(
-    "DisconnectPlayerResultTypeDef",
-    {
-        "DisconnectFailures": List[str],
-        "DisconnectSuccesses": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExportSnapshotRequestRequestTypeDef = TypedDict(
     "ExportSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
 
-ExportSnapshotResultTypeDef = TypedDict(
-    "ExportSnapshotResultTypeDef",
-    {
-        "S3Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExtensionDetailsTypeDef = TypedDict(
     "ExtensionDetailsTypeDef",
     {
         "Description": str,
         "Name": str,
         "Namespace": str,
     },
@@ -384,22 +373,20 @@
     "_OptionalGetGameConfigurationRequestRequestTypeDef",
     {
         "Sections": Sequence[str],
     },
     total=False,
 )
 
-
 class GetGameConfigurationRequestRequestTypeDef(
     _RequiredGetGameConfigurationRequestRequestTypeDef,
     _OptionalGetGameConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetGameRequestRequestTypeDef = TypedDict(
     "GetGameRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 
@@ -432,21 +419,19 @@
     "_OptionalGetSnapshotRequestRequestTypeDef",
     {
         "Sections": Sequence[str],
     },
     total=False,
 )
 
-
 class GetSnapshotRequestRequestTypeDef(
     _RequiredGetSnapshotRequestRequestTypeDef, _OptionalGetSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetStageDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredGetStageDeploymentRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -454,60 +439,38 @@
     "_OptionalGetStageDeploymentRequestRequestTypeDef",
     {
         "DeploymentId": str,
     },
     total=False,
 )
 
-
 class GetStageDeploymentRequestRequestTypeDef(
     _RequiredGetStageDeploymentRequestRequestTypeDef,
     _OptionalGetStageDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 GetStageRequestRequestTypeDef = TypedDict(
     "GetStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
 
-ImportGameConfigurationSourceTypeDef = TypedDict(
-    "ImportGameConfigurationSourceTypeDef",
-    {
-        "File": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
-_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
-    {
-        "Name": str,
-        "Namespace": str,
-    },
-)
-_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
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
-class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(
-    _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-    _OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListExtensionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExtensionVersionsRequestRequestTypeDef",
     {
         "Name": str,
         "Namespace": str,
     },
 )
@@ -516,79 +479,38 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListExtensionVersionsRequestRequestTypeDef(
     _RequiredListExtensionVersionsRequestRequestTypeDef,
     _OptionalListExtensionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListExtensionsRequestListExtensionsPaginateTypeDef = TypedDict(
-    "ListExtensionsRequestListExtensionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExtensionsRequestRequestTypeDef = TypedDict(
     "ListExtensionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListGamesRequestListGamesPaginateTypeDef = TypedDict(
-    "ListGamesRequestListGamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGamesRequestRequestTypeDef = TypedDict(
     "ListGamesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
-    "_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    {
-        "GameName": str,
-        "SnapshotId": str,
-    },
-)
-_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
-    "_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(
-    _RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-    _OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGeneratedCodeJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListGeneratedCodeJobsRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
@@ -597,44 +519,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListGeneratedCodeJobsRequestRequestTypeDef(
     _RequiredListGeneratedCodeJobsRequestRequestTypeDef,
     _OptionalListGeneratedCodeJobsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "GameName": str,
-    },
-)
-_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSnapshotsRequestListSnapshotsPaginateTypeDef(
-    _RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    _OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredListSnapshotsRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 _OptionalListSnapshotsRequestRequestTypeDef = TypedDict(
@@ -642,55 +540,30 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListSnapshotsRequestRequestTypeDef(
     _RequiredListSnapshotsRequestRequestTypeDef, _OptionalListSnapshotsRequestRequestTypeDef
 ):
     pass
 
-
 SnapshotSummaryTypeDef = TypedDict(
     "SnapshotSummaryTypeDef",
     {
         "Created": datetime,
         "Description": str,
         "Id": str,
         "LastUpdated": datetime,
     },
     total=False,
 )
 
-_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    {
-        "GameName": str,
-        "StageName": str,
-    },
-)
-_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(
-    _RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-    _OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStageDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListStageDeploymentsRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -699,44 +572,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListStageDeploymentsRequestRequestTypeDef(
     _RequiredListStageDeploymentsRequestRequestTypeDef,
     _OptionalListStageDeploymentsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListStagesRequestListStagesPaginateTypeDef = TypedDict(
-    "_RequiredListStagesRequestListStagesPaginateTypeDef",
-    {
-        "GameName": str,
-    },
-)
-_OptionalListStagesRequestListStagesPaginateTypeDef = TypedDict(
-    "_OptionalListStagesRequestListStagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStagesRequestListStagesPaginateTypeDef(
-    _RequiredListStagesRequestListStagesPaginateTypeDef,
-    _OptionalListStagesRequestListStagesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStagesRequestRequestTypeDef = TypedDict(
     "_RequiredListStagesRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 _OptionalListStagesRequestRequestTypeDef = TypedDict(
@@ -744,21 +593,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListStagesRequestRequestTypeDef(
     _RequiredListStagesRequestRequestTypeDef, _OptionalListStagesRequestRequestTypeDef
 ):
     pass
 
-
 StageSummaryTypeDef = TypedDict(
     "StageSummaryTypeDef",
     {
         "Description": str,
         "GameKey": str,
         "Name": str,
         "State": StageStateType,
@@ -770,43 +617,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": Dict[str, str],
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
 _RequiredSectionModificationTypeDef = TypedDict(
     "_RequiredSectionModificationTypeDef",
     {
         "Operation": OperationType,
         "Path": str,
         "Section": str,
     },
@@ -815,29 +633,19 @@
     "_OptionalSectionModificationTypeDef",
     {
         "Value": Mapping[str, Any],
     },
     total=False,
 )
 
-
 class SectionModificationTypeDef(
     _RequiredSectionModificationTypeDef, _OptionalSectionModificationTypeDef
 ):
     pass
 
-
-StartGeneratedCodeJobResultTypeDef = TypedDict(
-    "StartGeneratedCodeJobResultTypeDef",
-    {
-        "GeneratedCodeJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartStageDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartStageDeploymentRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
         "StageName": str,
     },
@@ -846,22 +654,20 @@
     "_OptionalStartStageDeploymentRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartStageDeploymentRequestRequestTypeDef(
     _RequiredStartStageDeploymentRequestRequestTypeDef,
     _OptionalStartStageDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -884,21 +690,19 @@
     "_OptionalUpdateGameRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateGameRequestRequestTypeDef(
     _RequiredUpdateGameRequestRequestTypeDef, _OptionalUpdateGameRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
@@ -906,21 +710,19 @@
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateStageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -929,74 +731,112 @@
     {
         "Description": str,
         "Role": str,
     },
     total=False,
 )
 
-
 class UpdateStageRequestRequestTypeDef(
     _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
 ):
     pass
 
-
-GetPlayerConnectionStatusResultTypeDef = TypedDict(
-    "GetPlayerConnectionStatusResultTypeDef",
+ImportGameConfigurationSourceTypeDef = TypedDict(
+    "ImportGameConfigurationSourceTypeDef",
     {
-        "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "File": BlobTypeDef,
     },
 )
 
 CreateGameResultTypeDef = TypedDict(
     "CreateGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisconnectPlayerResultTypeDef = TypedDict(
+    "DisconnectPlayerResultTypeDef",
+    {
+        "DisconnectFailures": List[str],
+        "DisconnectSuccesses": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportSnapshotResultTypeDef = TypedDict(
+    "ExportSnapshotResultTypeDef",
+    {
+        "S3Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGameResultTypeDef = TypedDict(
     "GetGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPlayerConnectionStatusResultTypeDef = TypedDict(
+    "GetPlayerConnectionStatusResultTypeDef",
+    {
+        "Connections": List[ConnectionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartGeneratedCodeJobResultTypeDef = TypedDict(
+    "StartGeneratedCodeJobResultTypeDef",
+    {
+        "GeneratedCodeJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGameResultTypeDef = TypedDict(
     "UpdateGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStageResultTypeDef = TypedDict(
     "CreateStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageResultTypeDef = TypedDict(
     "GetStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStageResultTypeDef = TypedDict(
     "UpdateStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StageDeploymentDetailsTypeDef = TypedDict(
     "StageDeploymentDetailsTypeDef",
     {
         "Created": datetime,
@@ -1023,41 +863,41 @@
     total=False,
 )
 
 GetExtensionResultTypeDef = TypedDict(
     "GetExtensionResultTypeDef",
     {
         "Extension": ExtensionDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExtensionsResultTypeDef = TypedDict(
     "ListExtensionsResultTypeDef",
     {
         "Extensions": List[ExtensionDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExtensionVersionResultTypeDef = TypedDict(
     "GetExtensionVersionResultTypeDef",
     {
         "ExtensionVersion": ExtensionVersionDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExtensionVersionsResultTypeDef = TypedDict(
     "ListExtensionVersionsResultTypeDef",
     {
         "ExtensionVersions": List[ExtensionVersionDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GameConfigurationDetailsTypeDef = TypedDict(
     "GameConfigurationDetailsTypeDef",
     {
         "Created": datetime,
@@ -1080,143 +920,262 @@
 )
 
 ListGamesResultTypeDef = TypedDict(
     "ListGamesResultTypeDef",
     {
         "Games": List[GameSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGeneratedCodeJobResultTypeDef = TypedDict(
     "GetGeneratedCodeJobResultTypeDef",
     {
         "GeneratedCodeJob": GeneratedCodeJobDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGeneratedCodeJobsResultTypeDef = TypedDict(
     "ListGeneratedCodeJobsResultTypeDef",
     {
         "GeneratedCodeJobs": List[GeneratedCodeJobDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartGeneratedCodeJobRequestRequestTypeDef = TypedDict(
     "StartGeneratedCodeJobRequestRequestTypeDef",
     {
         "GameName": str,
         "Generator": GeneratorTypeDef,
         "SnapshotId": str,
     },
 )
 
-ImportGameConfigurationRequestRequestTypeDef = TypedDict(
-    "ImportGameConfigurationRequestRequestTypeDef",
+_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    {
+        "Name": str,
+        "Namespace": str,
+    },
+)
+_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(
+    _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    _OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+):
+    pass
+
+ListExtensionsRequestListExtensionsPaginateTypeDef = TypedDict(
+    "ListExtensionsRequestListExtensionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGamesRequestListGamesPaginateTypeDef = TypedDict(
+    "ListGamesRequestListGamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
+    "_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    {
+        "GameName": str,
+        "SnapshotId": str,
+    },
+)
+_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
+    "_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(
+    _RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+    _OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef",
     {
         "GameName": str,
-        "ImportSource": ImportGameConfigurationSourceTypeDef,
     },
 )
+_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSnapshotsRequestListSnapshotsPaginateTypeDef(
+    _RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    _OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef,
+):
+    pass
+
+_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    {
+        "GameName": str,
+        "StageName": str,
+    },
+)
+_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(
+    _RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+    _OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+):
+    pass
+
+_RequiredListStagesRequestListStagesPaginateTypeDef = TypedDict(
+    "_RequiredListStagesRequestListStagesPaginateTypeDef",
+    {
+        "GameName": str,
+    },
+)
+_OptionalListStagesRequestListStagesPaginateTypeDef = TypedDict(
+    "_OptionalListStagesRequestListStagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStagesRequestListStagesPaginateTypeDef(
+    _RequiredListStagesRequestListStagesPaginateTypeDef,
+    _OptionalListStagesRequestListStagesPaginateTypeDef,
+):
+    pass
 
 ListSnapshotsResultTypeDef = TypedDict(
     "ListSnapshotsResultTypeDef",
     {
         "NextToken": str,
         "Snapshots": List[SnapshotSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStagesResultTypeDef = TypedDict(
     "ListStagesResultTypeDef",
     {
         "NextToken": str,
         "Stages": List[StageSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGameConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateGameConfigurationRequestRequestTypeDef",
     {
         "GameName": str,
         "Modifications": Sequence[SectionModificationTypeDef],
     },
 )
 
+ImportGameConfigurationRequestRequestTypeDef = TypedDict(
+    "ImportGameConfigurationRequestRequestTypeDef",
+    {
+        "GameName": str,
+        "ImportSource": ImportGameConfigurationSourceTypeDef,
+    },
+)
+
 GetStageDeploymentResultTypeDef = TypedDict(
     "GetStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartStageDeploymentResultTypeDef = TypedDict(
     "StartStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStageDeploymentsResultTypeDef = TypedDict(
     "ListStageDeploymentsResultTypeDef",
     {
         "NextToken": str,
         "StageDeployments": List[StageDeploymentSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGameConfigurationResultTypeDef = TypedDict(
     "GetGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportGameConfigurationResultTypeDef = TypedDict(
     "ImportGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGameConfigurationResultTypeDef = TypedDict(
     "UpdateGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSnapshotResultTypeDef = TypedDict(
     "CreateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotResultTypeDef = TypedDict(
     "GetSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSnapshotResultTypeDef = TypedDict(
     "UpdateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks/type_defs.pyi` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for gamesparks service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_gamesparks.type_defs import ConnectionTypeDef
+    from types_aiobotocore_gamesparks.type_defs import BlobTypeDef
 
-    data: ConnectionTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -28,28 +28,29 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "BlobTypeDef",
     "ConnectionTypeDef",
     "CreateGameRequestRequestTypeDef",
     "GameDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateStageRequestRequestTypeDef",
     "StageDetailsTypeDef",
     "DeleteGameRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeploymentResultTypeDef",
     "DisconnectPlayerRequestRequestTypeDef",
-    "DisconnectPlayerResultTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
-    "ExportSnapshotResultTypeDef",
     "ExtensionDetailsTypeDef",
     "ExtensionVersionDetailsTypeDef",
     "SectionTypeDef",
     "GameSummaryTypeDef",
     "GeneratedCodeJobDetailsTypeDef",
     "GeneratorTypeDef",
     "GetExtensionRequestRequestTypeDef",
@@ -57,46 +58,40 @@
     "GetGameConfigurationRequestRequestTypeDef",
     "GetGameRequestRequestTypeDef",
     "GetGeneratedCodeJobRequestRequestTypeDef",
     "GetPlayerConnectionStatusRequestRequestTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetStageDeploymentRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
-    "ImportGameConfigurationSourceTypeDef",
-    "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListExtensionVersionsRequestRequestTypeDef",
-    "ListExtensionsRequestListExtensionsPaginateTypeDef",
     "ListExtensionsRequestRequestTypeDef",
-    "ListGamesRequestListGamesPaginateTypeDef",
     "ListGamesRequestRequestTypeDef",
-    "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
     "ListGeneratedCodeJobsRequestRequestTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
     "SnapshotSummaryTypeDef",
-    "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
     "ListStageDeploymentsRequestRequestTypeDef",
-    "ListStagesRequestListStagesPaginateTypeDef",
     "ListStagesRequestRequestTypeDef",
     "StageSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SectionModificationTypeDef",
-    "StartGeneratedCodeJobResultTypeDef",
     "StartStageDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGameRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
-    "GetPlayerConnectionStatusResultTypeDef",
+    "ImportGameConfigurationSourceTypeDef",
     "CreateGameResultTypeDef",
+    "DisconnectPlayerResultTypeDef",
+    "ExportSnapshotResultTypeDef",
     "GetGameResultTypeDef",
+    "GetPlayerConnectionStatusResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "StartGeneratedCodeJobResultTypeDef",
     "UpdateGameResultTypeDef",
     "CreateStageResultTypeDef",
     "GetStageResultTypeDef",
     "UpdateStageResultTypeDef",
     "StageDeploymentDetailsTypeDef",
     "StageDeploymentSummaryTypeDef",
     "GetExtensionResultTypeDef",
@@ -105,29 +100,37 @@
     "ListExtensionVersionsResultTypeDef",
     "GameConfigurationDetailsTypeDef",
     "SnapshotDetailsTypeDef",
     "ListGamesResultTypeDef",
     "GetGeneratedCodeJobResultTypeDef",
     "ListGeneratedCodeJobsResultTypeDef",
     "StartGeneratedCodeJobRequestRequestTypeDef",
-    "ImportGameConfigurationRequestRequestTypeDef",
+    "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    "ListExtensionsRequestListExtensionsPaginateTypeDef",
+    "ListGamesRequestListGamesPaginateTypeDef",
+    "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    "ListStagesRequestListStagesPaginateTypeDef",
     "ListSnapshotsResultTypeDef",
     "ListStagesResultTypeDef",
     "UpdateGameConfigurationRequestRequestTypeDef",
+    "ImportGameConfigurationRequestRequestTypeDef",
     "GetStageDeploymentResultTypeDef",
     "StartStageDeploymentResultTypeDef",
     "ListStageDeploymentsResultTypeDef",
     "GetGameConfigurationResultTypeDef",
     "ImportGameConfigurationResultTypeDef",
     "UpdateGameConfigurationResultTypeDef",
     "CreateSnapshotResultTypeDef",
     "GetSnapshotResultTypeDef",
     "UpdateSnapshotResultTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "Created": datetime,
         "Id": str,
     },
     total=False,
@@ -145,19 +148,21 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateGameRequestRequestTypeDef(
     _RequiredCreateGameRequestRequestTypeDef, _OptionalCreateGameRequestRequestTypeDef
 ):
     pass
 
+
 GameDetailsTypeDef = TypedDict(
     "GameDetailsTypeDef",
     {
         "Arn": str,
         "Created": datetime,
         "Description": str,
         "EnableTerminationProtection": bool,
@@ -165,33 +170,46 @@
         "Name": str,
         "State": GameStateType,
         "Tags": Dict[str, str],
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
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 _OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSnapshotRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "GameName": str,
         "Role": str,
         "StageName": str,
     },
@@ -202,19 +220,21 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStageRequestRequestTypeDef(
     _RequiredCreateStageRequestRequestTypeDef, _OptionalCreateStageRequestRequestTypeDef
 ):
     pass
 
+
 StageDetailsTypeDef = TypedDict(
     "StageDetailsTypeDef",
     {
         "Arn": str,
         "Created": datetime,
         "Description": str,
         "GameKey": str,
@@ -257,39 +277,22 @@
     {
         "GameName": str,
         "PlayerId": str,
         "StageName": str,
     },
 )
 
-DisconnectPlayerResultTypeDef = TypedDict(
-    "DisconnectPlayerResultTypeDef",
-    {
-        "DisconnectFailures": List[str],
-        "DisconnectSuccesses": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExportSnapshotRequestRequestTypeDef = TypedDict(
     "ExportSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
 
-ExportSnapshotResultTypeDef = TypedDict(
-    "ExportSnapshotResultTypeDef",
-    {
-        "S3Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExtensionDetailsTypeDef = TypedDict(
     "ExtensionDetailsTypeDef",
     {
         "Description": str,
         "Name": str,
         "Namespace": str,
     },
@@ -377,20 +380,22 @@
     "_OptionalGetGameConfigurationRequestRequestTypeDef",
     {
         "Sections": Sequence[str],
     },
     total=False,
 )
 
+
 class GetGameConfigurationRequestRequestTypeDef(
     _RequiredGetGameConfigurationRequestRequestTypeDef,
     _OptionalGetGameConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetGameRequestRequestTypeDef = TypedDict(
     "GetGameRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 
@@ -423,19 +428,21 @@
     "_OptionalGetSnapshotRequestRequestTypeDef",
     {
         "Sections": Sequence[str],
     },
     total=False,
 )
 
+
 class GetSnapshotRequestRequestTypeDef(
     _RequiredGetSnapshotRequestRequestTypeDef, _OptionalGetSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetStageDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredGetStageDeploymentRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -443,56 +450,40 @@
     "_OptionalGetStageDeploymentRequestRequestTypeDef",
     {
         "DeploymentId": str,
     },
     total=False,
 )
 
+
 class GetStageDeploymentRequestRequestTypeDef(
     _RequiredGetStageDeploymentRequestRequestTypeDef,
     _OptionalGetStageDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 GetStageRequestRequestTypeDef = TypedDict(
     "GetStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
 
-ImportGameConfigurationSourceTypeDef = TypedDict(
-    "ImportGameConfigurationSourceTypeDef",
-    {
-        "File": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
-_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
-    {
-        "Name": str,
-        "Namespace": str,
-    },
-)
-_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
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
 
-class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(
-    _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-    _OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListExtensionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExtensionVersionsRequestRequestTypeDef",
     {
         "Name": str,
         "Namespace": str,
     },
 )
@@ -501,75 +492,40 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListExtensionVersionsRequestRequestTypeDef(
     _RequiredListExtensionVersionsRequestRequestTypeDef,
     _OptionalListExtensionVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListExtensionsRequestListExtensionsPaginateTypeDef = TypedDict(
-    "ListExtensionsRequestListExtensionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListExtensionsRequestRequestTypeDef = TypedDict(
     "ListExtensionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListGamesRequestListGamesPaginateTypeDef = TypedDict(
-    "ListGamesRequestListGamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGamesRequestRequestTypeDef = TypedDict(
     "ListGamesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
-    "_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    {
-        "GameName": str,
-        "SnapshotId": str,
-    },
-)
-_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
-    "_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(
-    _RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-    _OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-):
-    pass
-
 _RequiredListGeneratedCodeJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListGeneratedCodeJobsRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
@@ -578,39 +534,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListGeneratedCodeJobsRequestRequestTypeDef(
     _RequiredListGeneratedCodeJobsRequestRequestTypeDef,
     _OptionalListGeneratedCodeJobsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "GameName": str,
-    },
-)
-_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSnapshotsRequestListSnapshotsPaginateTypeDef(
-    _RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    _OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef,
-):
-    pass
 
 _RequiredListSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredListSnapshotsRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
@@ -619,51 +557,32 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListSnapshotsRequestRequestTypeDef(
     _RequiredListSnapshotsRequestRequestTypeDef, _OptionalListSnapshotsRequestRequestTypeDef
 ):
     pass
 
+
 SnapshotSummaryTypeDef = TypedDict(
     "SnapshotSummaryTypeDef",
     {
         "Created": datetime,
         "Description": str,
         "Id": str,
         "LastUpdated": datetime,
     },
     total=False,
 )
 
-_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    {
-        "GameName": str,
-        "StageName": str,
-    },
-)
-_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(
-    _RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-    _OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListStageDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListStageDeploymentsRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -672,39 +591,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListStageDeploymentsRequestRequestTypeDef(
     _RequiredListStageDeploymentsRequestRequestTypeDef,
     _OptionalListStageDeploymentsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListStagesRequestListStagesPaginateTypeDef = TypedDict(
-    "_RequiredListStagesRequestListStagesPaginateTypeDef",
-    {
-        "GameName": str,
-    },
-)
-_OptionalListStagesRequestListStagesPaginateTypeDef = TypedDict(
-    "_OptionalListStagesRequestListStagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStagesRequestListStagesPaginateTypeDef(
-    _RequiredListStagesRequestListStagesPaginateTypeDef,
-    _OptionalListStagesRequestListStagesPaginateTypeDef,
-):
-    pass
 
 _RequiredListStagesRequestRequestTypeDef = TypedDict(
     "_RequiredListStagesRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
@@ -713,19 +614,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListStagesRequestRequestTypeDef(
     _RequiredListStagesRequestRequestTypeDef, _OptionalListStagesRequestRequestTypeDef
 ):
     pass
 
+
 StageSummaryTypeDef = TypedDict(
     "StageSummaryTypeDef",
     {
         "Description": str,
         "GameKey": str,
         "Name": str,
         "State": StageStateType,
@@ -737,43 +640,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": Dict[str, str],
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
 _RequiredSectionModificationTypeDef = TypedDict(
     "_RequiredSectionModificationTypeDef",
     {
         "Operation": OperationType,
         "Path": str,
         "Section": str,
     },
@@ -782,26 +656,20 @@
     "_OptionalSectionModificationTypeDef",
     {
         "Value": Mapping[str, Any],
     },
     total=False,
 )
 
+
 class SectionModificationTypeDef(
     _RequiredSectionModificationTypeDef, _OptionalSectionModificationTypeDef
 ):
     pass
 
-StartGeneratedCodeJobResultTypeDef = TypedDict(
-    "StartGeneratedCodeJobResultTypeDef",
-    {
-        "GeneratedCodeJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStartStageDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartStageDeploymentRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
         "StageName": str,
@@ -811,20 +679,22 @@
     "_OptionalStartStageDeploymentRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartStageDeploymentRequestRequestTypeDef(
     _RequiredStartStageDeploymentRequestRequestTypeDef,
     _OptionalStartStageDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -847,19 +717,21 @@
     "_OptionalUpdateGameRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateGameRequestRequestTypeDef(
     _RequiredUpdateGameRequestRequestTypeDef, _OptionalUpdateGameRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
@@ -867,19 +739,21 @@
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateStageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -888,72 +762,114 @@
     {
         "Description": str,
         "Role": str,
     },
     total=False,
 )
 
+
 class UpdateStageRequestRequestTypeDef(
     _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
 ):
     pass
 
-GetPlayerConnectionStatusResultTypeDef = TypedDict(
-    "GetPlayerConnectionStatusResultTypeDef",
+
+ImportGameConfigurationSourceTypeDef = TypedDict(
+    "ImportGameConfigurationSourceTypeDef",
     {
-        "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "File": BlobTypeDef,
     },
 )
 
 CreateGameResultTypeDef = TypedDict(
     "CreateGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisconnectPlayerResultTypeDef = TypedDict(
+    "DisconnectPlayerResultTypeDef",
+    {
+        "DisconnectFailures": List[str],
+        "DisconnectSuccesses": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportSnapshotResultTypeDef = TypedDict(
+    "ExportSnapshotResultTypeDef",
+    {
+        "S3Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGameResultTypeDef = TypedDict(
     "GetGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPlayerConnectionStatusResultTypeDef = TypedDict(
+    "GetPlayerConnectionStatusResultTypeDef",
+    {
+        "Connections": List[ConnectionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartGeneratedCodeJobResultTypeDef = TypedDict(
+    "StartGeneratedCodeJobResultTypeDef",
+    {
+        "GeneratedCodeJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGameResultTypeDef = TypedDict(
     "UpdateGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStageResultTypeDef = TypedDict(
     "CreateStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageResultTypeDef = TypedDict(
     "GetStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStageResultTypeDef = TypedDict(
     "UpdateStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StageDeploymentDetailsTypeDef = TypedDict(
     "StageDeploymentDetailsTypeDef",
     {
         "Created": datetime,
@@ -980,41 +896,41 @@
     total=False,
 )
 
 GetExtensionResultTypeDef = TypedDict(
     "GetExtensionResultTypeDef",
     {
         "Extension": ExtensionDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExtensionsResultTypeDef = TypedDict(
     "ListExtensionsResultTypeDef",
     {
         "Extensions": List[ExtensionDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExtensionVersionResultTypeDef = TypedDict(
     "GetExtensionVersionResultTypeDef",
     {
         "ExtensionVersion": ExtensionVersionDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExtensionVersionsResultTypeDef = TypedDict(
     "ListExtensionVersionsResultTypeDef",
     {
         "ExtensionVersions": List[ExtensionVersionDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GameConfigurationDetailsTypeDef = TypedDict(
     "GameConfigurationDetailsTypeDef",
     {
         "Created": datetime,
@@ -1037,143 +953,272 @@
 )
 
 ListGamesResultTypeDef = TypedDict(
     "ListGamesResultTypeDef",
     {
         "Games": List[GameSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGeneratedCodeJobResultTypeDef = TypedDict(
     "GetGeneratedCodeJobResultTypeDef",
     {
         "GeneratedCodeJob": GeneratedCodeJobDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGeneratedCodeJobsResultTypeDef = TypedDict(
     "ListGeneratedCodeJobsResultTypeDef",
     {
         "GeneratedCodeJobs": List[GeneratedCodeJobDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartGeneratedCodeJobRequestRequestTypeDef = TypedDict(
     "StartGeneratedCodeJobRequestRequestTypeDef",
     {
         "GameName": str,
         "Generator": GeneratorTypeDef,
         "SnapshotId": str,
     },
 )
 
-ImportGameConfigurationRequestRequestTypeDef = TypedDict(
-    "ImportGameConfigurationRequestRequestTypeDef",
+_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    {
+        "Name": str,
+        "Namespace": str,
+    },
+)
+_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(
+    _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    _OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListExtensionsRequestListExtensionsPaginateTypeDef = TypedDict(
+    "ListExtensionsRequestListExtensionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGamesRequestListGamesPaginateTypeDef = TypedDict(
+    "ListGamesRequestListGamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
+    "_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
     {
         "GameName": str,
-        "ImportSource": ImportGameConfigurationSourceTypeDef,
+        "SnapshotId": str,
     },
 )
+_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
+    "_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(
+    _RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+    _OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "GameName": str,
+    },
+)
+_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSnapshotsRequestListSnapshotsPaginateTypeDef(
+    _RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    _OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    {
+        "GameName": str,
+        "StageName": str,
+    },
+)
+_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(
+    _RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+    _OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStagesRequestListStagesPaginateTypeDef = TypedDict(
+    "_RequiredListStagesRequestListStagesPaginateTypeDef",
+    {
+        "GameName": str,
+    },
+)
+_OptionalListStagesRequestListStagesPaginateTypeDef = TypedDict(
+    "_OptionalListStagesRequestListStagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStagesRequestListStagesPaginateTypeDef(
+    _RequiredListStagesRequestListStagesPaginateTypeDef,
+    _OptionalListStagesRequestListStagesPaginateTypeDef,
+):
+    pass
+
 
 ListSnapshotsResultTypeDef = TypedDict(
     "ListSnapshotsResultTypeDef",
     {
         "NextToken": str,
         "Snapshots": List[SnapshotSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStagesResultTypeDef = TypedDict(
     "ListStagesResultTypeDef",
     {
         "NextToken": str,
         "Stages": List[StageSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGameConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateGameConfigurationRequestRequestTypeDef",
     {
         "GameName": str,
         "Modifications": Sequence[SectionModificationTypeDef],
     },
 )
 
+ImportGameConfigurationRequestRequestTypeDef = TypedDict(
+    "ImportGameConfigurationRequestRequestTypeDef",
+    {
+        "GameName": str,
+        "ImportSource": ImportGameConfigurationSourceTypeDef,
+    },
+)
+
 GetStageDeploymentResultTypeDef = TypedDict(
     "GetStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartStageDeploymentResultTypeDef = TypedDict(
     "StartStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStageDeploymentsResultTypeDef = TypedDict(
     "ListStageDeploymentsResultTypeDef",
     {
         "NextToken": str,
         "StageDeployments": List[StageDeploymentSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGameConfigurationResultTypeDef = TypedDict(
     "GetGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportGameConfigurationResultTypeDef = TypedDict(
     "ImportGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGameConfigurationResultTypeDef = TypedDict(
     "UpdateGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSnapshotResultTypeDef = TypedDict(
     "CreateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotResultTypeDef = TypedDict(
     "GetSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSnapshotResultTypeDef = TypedDict(
     "UpdateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks.egg-info/PKG-INFO` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-gamesparks
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.GameSparks 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.GameSparks 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore gamesparks type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore gamesparks type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-gamesparks"></a>
 
 # types-aiobotocore-gamesparks
 
 [![PyPI - types-aiobotocore-gamesparks](https://img.shields.io/pypi/v/types-aiobotocore-gamesparks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamesparks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-gamesparks.svg?color=blue)](https://pypi.org/project/types-aiobotocore-gamesparks)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-gamesparks?color=blue)](https://pypistats.org/packages/types-aiobotocore-gamesparks)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-gamesparks)](https://pepy.tech/project/types-aiobotocore-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.GameSparks 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
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
 [types-aiobotocore-gamesparks docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_gamesparks/).
 
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
@@ -338,36 +337,36 @@
 )
 
 
 def check_value(value: DeploymentActionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_gamesparks.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_gamesparks.type_defs import (
+    BlobTypeDef,
     ConnectionTypeDef,
     CreateGameRequestRequestTypeDef,
     GameDetailsTypeDef,
+    ResponseMetadataTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateStageRequestRequestTypeDef,
     StageDetailsTypeDef,
     DeleteGameRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeploymentResultTypeDef,
     DisconnectPlayerRequestRequestTypeDef,
-    DisconnectPlayerResultTypeDef,
     ExportSnapshotRequestRequestTypeDef,
-    ExportSnapshotResultTypeDef,
     ExtensionDetailsTypeDef,
     ExtensionVersionDetailsTypeDef,
     SectionTypeDef,
     GameSummaryTypeDef,
     GeneratedCodeJobDetailsTypeDef,
     GeneratorTypeDef,
     GetExtensionRequestRequestTypeDef,
@@ -375,46 +374,40 @@
     GetGameConfigurationRequestRequestTypeDef,
     GetGameRequestRequestTypeDef,
     GetGeneratedCodeJobRequestRequestTypeDef,
     GetPlayerConnectionStatusRequestRequestTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetStageDeploymentRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    ImportGameConfigurationSourceTypeDef,
-    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListExtensionVersionsRequestRequestTypeDef,
-    ListExtensionsRequestListExtensionsPaginateTypeDef,
     ListExtensionsRequestRequestTypeDef,
-    ListGamesRequestListGamesPaginateTypeDef,
     ListGamesRequestRequestTypeDef,
-    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
     ListGeneratedCodeJobsRequestRequestTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     SnapshotSummaryTypeDef,
-    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
     ListStageDeploymentsRequestRequestTypeDef,
-    ListStagesRequestListStagesPaginateTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SectionModificationTypeDef,
-    StartGeneratedCodeJobResultTypeDef,
     StartStageDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGameRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
-    GetPlayerConnectionStatusResultTypeDef,
+    ImportGameConfigurationSourceTypeDef,
     CreateGameResultTypeDef,
+    DisconnectPlayerResultTypeDef,
+    ExportSnapshotResultTypeDef,
     GetGameResultTypeDef,
+    GetPlayerConnectionStatusResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    StartGeneratedCodeJobResultTypeDef,
     UpdateGameResultTypeDef,
     CreateStageResultTypeDef,
     GetStageResultTypeDef,
     UpdateStageResultTypeDef,
     StageDeploymentDetailsTypeDef,
     StageDeploymentSummaryTypeDef,
     GetExtensionResultTypeDef,
@@ -423,31 +416,38 @@
     ListExtensionVersionsResultTypeDef,
     GameConfigurationDetailsTypeDef,
     SnapshotDetailsTypeDef,
     ListGamesResultTypeDef,
     GetGeneratedCodeJobResultTypeDef,
     ListGeneratedCodeJobsResultTypeDef,
     StartGeneratedCodeJobRequestRequestTypeDef,
-    ImportGameConfigurationRequestRequestTypeDef,
+    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    ListExtensionsRequestListExtensionsPaginateTypeDef,
+    ListGamesRequestListGamesPaginateTypeDef,
+    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+    ListStagesRequestListStagesPaginateTypeDef,
     ListSnapshotsResultTypeDef,
     ListStagesResultTypeDef,
     UpdateGameConfigurationRequestRequestTypeDef,
+    ImportGameConfigurationRequestRequestTypeDef,
     GetStageDeploymentResultTypeDef,
     StartStageDeploymentResultTypeDef,
     ListStageDeploymentsResultTypeDef,
     GetGameConfigurationResultTypeDef,
     ImportGameConfigurationResultTypeDef,
     UpdateGameConfigurationResultTypeDef,
     CreateSnapshotResultTypeDef,
     GetSnapshotResultTypeDef,
     UpdateSnapshotResultTypeDef,
 )
 
 
-def get_structure() -> ConnectionTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-gamesparks-2.5.2/types_aiobotocore_gamesparks.egg-info/SOURCES.txt` & `types-aiobotocore-gamesparks-2.5.2.post1/types_aiobotocore_gamesparks.egg-info/SOURCES.txt`

 * *Files identical despite different names*


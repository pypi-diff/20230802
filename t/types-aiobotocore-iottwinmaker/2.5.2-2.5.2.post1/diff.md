# Comparing `tmp/types-aiobotocore-iottwinmaker-2.5.2.tar.gz` & `tmp/types-aiobotocore-iottwinmaker-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iottwinmaker-2.5.2.tar", last modified: Sat Jul  8 01:43:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-iottwinmaker-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:28 2023, max compression
```

## Comparing `types-aiobotocore-iottwinmaker-2.5.2.tar` & `types-aiobotocore-iottwinmaker-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:48.574338 types-aiobotocore-iottwinmaker-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:58.000000 types-aiobotocore-iottwinmaker-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-07-08 01:43:48.574338 types-aiobotocore-iottwinmaker-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-07-08 01:32:58.000000 types-aiobotocore-iottwinmaker-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:48.574338 types-aiobotocore-iottwinmaker-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:32:58.000000 types-aiobotocore-iottwinmaker-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:48.574338 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-08 01:32:58.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-08 01:32:58.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:32:58.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26613 2023-07-08 01:32:58.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26571 2023-07-08 01:32:58.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-08 01:32:59.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-07-08 01:32:59.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:58.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43559 2023-07-08 01:33:00.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43486 2023-07-08 01:32:59.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:58.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:48.574338 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-07-08 01:43:48.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-08 01:43:48.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:48.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:48.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:48.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:48.000000 types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.809556 types-aiobotocore-iottwinmaker-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-08-02 14:52:28.809556 types-aiobotocore-iottwinmaker-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:28.809556 types-aiobotocore-iottwinmaker-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.805556 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26600 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46383 2023-08-02 14:41:03.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46302 2023-08-02 14:41:03.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:02.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.809556 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-08-02 14:52:28.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:52:28.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:28.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:28.000000 types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/LICENSE` & `types-aiobotocore-iottwinmaker-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/PKG-INFO` & `types-aiobotocore-iottwinmaker-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iottwinmaker
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTTwinMaker 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTTwinMaker 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iottwinmaker type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iottwinmaker type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iottwinmaker"></a>
 
 # types-aiobotocore-iottwinmaker
 
 [![PyPI - types-aiobotocore-iottwinmaker](https://img.shields.io/pypi/v/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iottwinmaker?color=blue)](https://pypistats.org/packages/types-aiobotocore-iottwinmaker)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iottwinmaker)](https://pepy.tech/project/types-aiobotocore-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTTwinMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [types-aiobotocore-iottwinmaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/).
 
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
@@ -300,140 +299,147 @@
 )
 
 
 def check_value(value: ColumnTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iottwinmaker.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iottwinmaker.type_defs import (
+    ResponseMetadataTypeDef,
     BundleInformationTypeDef,
     ColumnDescriptionTypeDef,
     ComponentPropertyGroupRequestTypeDef,
     ComponentPropertyGroupResponseTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyGroupRequestTypeDef,
-    CreateComponentTypeResponseTypeDef,
-    CreateEntityResponseTypeDef,
     CreateSceneRequestRequestTypeDef,
-    CreateSceneResponseTypeDef,
     CreateSyncJobRequestRequestTypeDef,
-    CreateSyncJobResponseTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
-    CreateWorkspaceResponseTypeDef,
     LambdaFunctionTypeDef,
     RelationshipTypeDef,
     RelationshipValueTypeDef,
     DeleteComponentTypeRequestRequestTypeDef,
-    DeleteComponentTypeResponseTypeDef,
     DeleteEntityRequestRequestTypeDef,
-    DeleteEntityResponseTypeDef,
     DeleteSceneRequestRequestTypeDef,
     DeleteSyncJobRequestRequestTypeDef,
-    DeleteSyncJobResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
+    EntityPropertyReferenceOutputTypeDef,
     EntityPropertyReferenceTypeDef,
     ErrorDetailsTypeDef,
     ExecuteQueryRequestRequestTypeDef,
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
     PropertyDefinitionResponseTypeDef,
     PropertyGroupResponseTypeDef,
     GetEntityRequestRequestTypeDef,
     InterpolationParametersTypeDef,
     PropertyFilterTypeDef,
+    TimestampTypeDef,
     GetSceneRequestRequestTypeDef,
     SceneErrorTypeDef,
     GetSyncJobRequestRequestTypeDef,
     GetWorkspaceRequestRequestTypeDef,
-    GetWorkspaceResponseTypeDef,
     ListComponentTypesFilterTypeDef,
     ListEntitiesFilterTypeDef,
     ListScenesRequestRequestTypeDef,
     SceneSummaryTypeDef,
     ListSyncJobsRequestRequestTypeDef,
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
-    PropertyValueTypeDef,
-    ResponseMetadataTypeDef,
+    PropertyValueOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateComponentTypeResponseTypeDef,
-    UpdateEntityResponseTypeDef,
     UpdatePricingPlanRequestRequestTypeDef,
     UpdateSceneRequestRequestTypeDef,
-    UpdateSceneResponseTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
+    CreateComponentTypeResponseTypeDef,
+    CreateEntityResponseTypeDef,
+    CreateSceneResponseTypeDef,
+    CreateSyncJobResponseTypeDef,
+    CreateWorkspaceResponseTypeDef,
+    DeleteComponentTypeResponseTypeDef,
+    DeleteEntityResponseTypeDef,
+    DeleteSyncJobResponseTypeDef,
+    GetWorkspaceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateComponentTypeResponseTypeDef,
+    UpdateEntityResponseTypeDef,
+    UpdateSceneResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
     PricingPlanTypeDef,
     PropertyRequestTypeDef,
     DataConnectorTypeDef,
+    DataTypeOutputTypeDef,
     DataTypeTypeDef,
+    DataValueOutputTypeDef,
     DataValueTypeDef,
     PropertyLatestValueTypeDef,
     StatusTypeDef,
     SyncJobStatusTypeDef,
     SyncResourceStatusTypeDef,
     ExecuteQueryResponseTypeDef,
     PropertyResponseTypeDef,
     GetPropertyValueHistoryRequestRequestTypeDef,
+    PropertyValueTypeDef,
     GetSceneResponseTypeDef,
     ListComponentTypesRequestRequestTypeDef,
     ListEntitiesRequestRequestTypeDef,
     ListScenesResponseTypeDef,
     ListSyncResourcesRequestRequestTypeDef,
     ListWorkspacesResponseTypeDef,
     TabularConditionsTypeDef,
-    PropertyValueEntryTypeDef,
+    PropertyValueEntryOutputTypeDef,
     PropertyValueHistoryTypeDef,
     GetPricingPlanResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     ComponentRequestTypeDef,
     ComponentUpdateRequestTypeDef,
     FunctionRequestTypeDef,
     FunctionResponseTypeDef,
     GetPropertyValueResponseTypeDef,
     ComponentTypeSummaryTypeDef,
     EntitySummaryTypeDef,
     GetSyncJobResponseTypeDef,
     SyncJobSummaryTypeDef,
     SyncResourceSummaryTypeDef,
     ComponentResponseTypeDef,
+    PropertyValueEntryTypeDef,
     GetPropertyValueRequestRequestTypeDef,
     BatchPutPropertyErrorTypeDef,
-    BatchPutPropertyValuesRequestRequestTypeDef,
     GetPropertyValueHistoryResponseTypeDef,
     CreateEntityRequestRequestTypeDef,
     UpdateEntityRequestRequestTypeDef,
     CreateComponentTypeRequestRequestTypeDef,
     UpdateComponentTypeRequestRequestTypeDef,
     GetComponentTypeResponseTypeDef,
     ListComponentTypesResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListSyncJobsResponseTypeDef,
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
+    PropertyValueEntryUnionTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
+    BatchPutPropertyValuesRequestRequestTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
 )
 
 
-def get_structure() -> BundleInformationTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/README.md` & `types-aiobotocore-iottwinmaker-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iottwinmaker"></a>
 
 # types-aiobotocore-iottwinmaker
 
 [![PyPI - types-aiobotocore-iottwinmaker](https://img.shields.io/pypi/v/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iottwinmaker?color=blue)](https://pypistats.org/packages/types-aiobotocore-iottwinmaker)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iottwinmaker)](https://pepy.tech/project/types-aiobotocore-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTTwinMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [types-aiobotocore-iottwinmaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/).
 
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
@@ -267,140 +267,147 @@
 )
 
 
 def check_value(value: ColumnTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iottwinmaker.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iottwinmaker.type_defs import (
+    ResponseMetadataTypeDef,
     BundleInformationTypeDef,
     ColumnDescriptionTypeDef,
     ComponentPropertyGroupRequestTypeDef,
     ComponentPropertyGroupResponseTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyGroupRequestTypeDef,
-    CreateComponentTypeResponseTypeDef,
-    CreateEntityResponseTypeDef,
     CreateSceneRequestRequestTypeDef,
-    CreateSceneResponseTypeDef,
     CreateSyncJobRequestRequestTypeDef,
-    CreateSyncJobResponseTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
-    CreateWorkspaceResponseTypeDef,
     LambdaFunctionTypeDef,
     RelationshipTypeDef,
     RelationshipValueTypeDef,
     DeleteComponentTypeRequestRequestTypeDef,
-    DeleteComponentTypeResponseTypeDef,
     DeleteEntityRequestRequestTypeDef,
-    DeleteEntityResponseTypeDef,
     DeleteSceneRequestRequestTypeDef,
     DeleteSyncJobRequestRequestTypeDef,
-    DeleteSyncJobResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
+    EntityPropertyReferenceOutputTypeDef,
     EntityPropertyReferenceTypeDef,
     ErrorDetailsTypeDef,
     ExecuteQueryRequestRequestTypeDef,
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
     PropertyDefinitionResponseTypeDef,
     PropertyGroupResponseTypeDef,
     GetEntityRequestRequestTypeDef,
     InterpolationParametersTypeDef,
     PropertyFilterTypeDef,
+    TimestampTypeDef,
     GetSceneRequestRequestTypeDef,
     SceneErrorTypeDef,
     GetSyncJobRequestRequestTypeDef,
     GetWorkspaceRequestRequestTypeDef,
-    GetWorkspaceResponseTypeDef,
     ListComponentTypesFilterTypeDef,
     ListEntitiesFilterTypeDef,
     ListScenesRequestRequestTypeDef,
     SceneSummaryTypeDef,
     ListSyncJobsRequestRequestTypeDef,
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
-    PropertyValueTypeDef,
-    ResponseMetadataTypeDef,
+    PropertyValueOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateComponentTypeResponseTypeDef,
-    UpdateEntityResponseTypeDef,
     UpdatePricingPlanRequestRequestTypeDef,
     UpdateSceneRequestRequestTypeDef,
-    UpdateSceneResponseTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
+    CreateComponentTypeResponseTypeDef,
+    CreateEntityResponseTypeDef,
+    CreateSceneResponseTypeDef,
+    CreateSyncJobResponseTypeDef,
+    CreateWorkspaceResponseTypeDef,
+    DeleteComponentTypeResponseTypeDef,
+    DeleteEntityResponseTypeDef,
+    DeleteSyncJobResponseTypeDef,
+    GetWorkspaceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateComponentTypeResponseTypeDef,
+    UpdateEntityResponseTypeDef,
+    UpdateSceneResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
     PricingPlanTypeDef,
     PropertyRequestTypeDef,
     DataConnectorTypeDef,
+    DataTypeOutputTypeDef,
     DataTypeTypeDef,
+    DataValueOutputTypeDef,
     DataValueTypeDef,
     PropertyLatestValueTypeDef,
     StatusTypeDef,
     SyncJobStatusTypeDef,
     SyncResourceStatusTypeDef,
     ExecuteQueryResponseTypeDef,
     PropertyResponseTypeDef,
     GetPropertyValueHistoryRequestRequestTypeDef,
+    PropertyValueTypeDef,
     GetSceneResponseTypeDef,
     ListComponentTypesRequestRequestTypeDef,
     ListEntitiesRequestRequestTypeDef,
     ListScenesResponseTypeDef,
     ListSyncResourcesRequestRequestTypeDef,
     ListWorkspacesResponseTypeDef,
     TabularConditionsTypeDef,
-    PropertyValueEntryTypeDef,
+    PropertyValueEntryOutputTypeDef,
     PropertyValueHistoryTypeDef,
     GetPricingPlanResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     ComponentRequestTypeDef,
     ComponentUpdateRequestTypeDef,
     FunctionRequestTypeDef,
     FunctionResponseTypeDef,
     GetPropertyValueResponseTypeDef,
     ComponentTypeSummaryTypeDef,
     EntitySummaryTypeDef,
     GetSyncJobResponseTypeDef,
     SyncJobSummaryTypeDef,
     SyncResourceSummaryTypeDef,
     ComponentResponseTypeDef,
+    PropertyValueEntryTypeDef,
     GetPropertyValueRequestRequestTypeDef,
     BatchPutPropertyErrorTypeDef,
-    BatchPutPropertyValuesRequestRequestTypeDef,
     GetPropertyValueHistoryResponseTypeDef,
     CreateEntityRequestRequestTypeDef,
     UpdateEntityRequestRequestTypeDef,
     CreateComponentTypeRequestRequestTypeDef,
     UpdateComponentTypeRequestRequestTypeDef,
     GetComponentTypeResponseTypeDef,
     ListComponentTypesResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListSyncJobsResponseTypeDef,
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
+    PropertyValueEntryUnionTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
+    BatchPutPropertyValuesRequestRequestTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
 )
 
 
-def get_structure() -> BundleInformationTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/setup.py` & `types-aiobotocore-iottwinmaker-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iottwinmaker",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iottwinmaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTTwinMaker 2.5.2 service generated with"
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
-    keywords="aiobotocore iottwinmaker type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore iottwinmaker type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iottwinmaker": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/"
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/__main__.py` & `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTTwinMaker 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IoTTwinMaker 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker\nOther"
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

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/client.py` & `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from types_aiobotocore_iottwinmaker.client import IoTTwinMakerClient
 
     session = get_session()
     async with session.create_client("iottwinmaker") as client:
         client: IoTTwinMakerClient
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import OrderByTimeType, PricingModeType
 from .type_defs import (
     BatchPutPropertyValuesResponseTypeDef,
@@ -53,50 +52,48 @@
     ListSyncResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyFilterTypeDef,
     PropertyGroupRequestTypeDef,
-    PropertyValueEntryTypeDef,
+    PropertyValueEntryUnionTypeDef,
     SyncResourceFilterTypeDef,
     TabularConditionsTypeDef,
+    TimestampTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     UpdateSceneResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
 )
 
 __all__ = ("IoTTwinMakerClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ConnectorFailureException: Type[BotocoreClientError]
     ConnectorTimeoutException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     QueryTimeoutException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class IoTTwinMakerClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/)
     """
 
     meta: ClientMeta
@@ -105,41 +102,37 @@
     def exceptions(self) -> Exceptions:
         """
         IoTTwinMakerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#exceptions)
         """
-
     async def batch_put_property_values(
-        self, *, workspaceId: str, entries: Sequence[PropertyValueEntryTypeDef]
+        self, *, workspaceId: str, entries: Sequence[PropertyValueEntryUnionTypeDef]
     ) -> BatchPutPropertyValuesResponseTypeDef:
         """
         Sets values for multiple time series properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.batch_put_property_values)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#batch_put_property_values)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#close)
         """
-
     async def create_component_type(
         self,
         *,
         workspaceId: str,
         componentTypeId: str,
         isSingleton: bool = ...,
         description: str = ...,
@@ -152,15 +145,14 @@
     ) -> CreateComponentTypeResponseTypeDef:
         """
         Creates a component type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_component_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_component_type)
         """
-
     async def create_entity(
         self,
         *,
         workspaceId: str,
         entityName: str,
         entityId: str = ...,
         description: str = ...,
@@ -170,15 +162,14 @@
     ) -> CreateEntityResponseTypeDef:
         """
         Creates an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_entity)
         """
-
     async def create_scene(
         self,
         *,
         workspaceId: str,
         sceneId: str,
         contentLocation: str,
         description: str = ...,
@@ -188,25 +179,23 @@
     ) -> CreateSceneResponseTypeDef:
         """
         Creates a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_scene)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_scene)
         """
-
     async def create_sync_job(
         self, *, workspaceId: str, syncSource: str, syncRole: str, tags: Mapping[str, str] = ...
     ) -> CreateSyncJobResponseTypeDef:
         """
         This action creates a SyncJob.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_sync_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_sync_job)
         """
-
     async def create_workspace(
         self,
         *,
         workspaceId: str,
         s3Location: str,
         role: str,
         description: str = ...,
@@ -214,112 +203,101 @@
     ) -> CreateWorkspaceResponseTypeDef:
         """
         Creates a workplace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_workspace)
         """
-
     async def delete_component_type(
         self, *, workspaceId: str, componentTypeId: str
     ) -> DeleteComponentTypeResponseTypeDef:
         """
         Deletes a component type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.delete_component_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#delete_component_type)
         """
-
     async def delete_entity(
         self, *, workspaceId: str, entityId: str, isRecursive: bool = ...
     ) -> DeleteEntityResponseTypeDef:
         """
         Deletes an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.delete_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#delete_entity)
         """
-
     async def delete_scene(self, *, workspaceId: str, sceneId: str) -> Dict[str, Any]:
         """
         Deletes a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.delete_scene)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#delete_scene)
         """
-
     async def delete_sync_job(
         self, *, workspaceId: str, syncSource: str
     ) -> DeleteSyncJobResponseTypeDef:
         """
         Delete the SyncJob.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.delete_sync_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#delete_sync_job)
         """
-
     async def delete_workspace(self, *, workspaceId: str) -> Dict[str, Any]:
         """
         Deletes a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.delete_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#delete_workspace)
         """
-
     async def execute_query(
         self, *, workspaceId: str, queryStatement: str, maxResults: int = ..., nextToken: str = ...
     ) -> ExecuteQueryResponseTypeDef:
         """
         Run queries to access information from your knowledge graph of entities within
         individual workspaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.execute_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#execute_query)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#generate_presigned_url)
         """
-
     async def get_component_type(
         self, *, workspaceId: str, componentTypeId: str
     ) -> GetComponentTypeResponseTypeDef:
         """
         Retrieves information about a component type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_component_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_component_type)
         """
-
     async def get_entity(self, *, workspaceId: str, entityId: str) -> GetEntityResponseTypeDef:
         """
         Retrieves information about an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_entity)
         """
-
     async def get_pricing_plan(self) -> GetPricingPlanResponseTypeDef:
         """
         Gets the pricing plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_pricing_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_pricing_plan)
         """
-
     async def get_property_value(
         self,
         *,
         selectedProperties: Sequence[str],
         workspaceId: str,
         componentName: str = ...,
         componentTypeId: str = ...,
@@ -331,117 +309,108 @@
     ) -> GetPropertyValueResponseTypeDef:
         """
         Gets the property values for a component, component type, entity, or workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_property_value)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_property_value)
         """
-
     async def get_property_value_history(
         self,
         *,
         workspaceId: str,
         selectedProperties: Sequence[str],
         entityId: str = ...,
         componentName: str = ...,
         componentTypeId: str = ...,
         propertyFilters: Sequence[PropertyFilterTypeDef] = ...,
-        startDateTime: Union[datetime, str] = ...,
-        endDateTime: Union[datetime, str] = ...,
+        startDateTime: TimestampTypeDef = ...,
+        endDateTime: TimestampTypeDef = ...,
         interpolation: InterpolationParametersTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         orderByTime: OrderByTimeType = ...,
         startTime: str = ...,
         endTime: str = ...
     ) -> GetPropertyValueHistoryResponseTypeDef:
         """
         Retrieves information about the history of a time series property value for a
         component, component type, entity, or workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_property_value_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_property_value_history)
         """
-
     async def get_scene(self, *, workspaceId: str, sceneId: str) -> GetSceneResponseTypeDef:
         """
         Retrieves information about a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_scene)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_scene)
         """
-
     async def get_sync_job(
         self, *, syncSource: str, workspaceId: str = ...
     ) -> GetSyncJobResponseTypeDef:
         """
         Gets the SyncJob.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_sync_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_sync_job)
         """
-
     async def get_workspace(self, *, workspaceId: str) -> GetWorkspaceResponseTypeDef:
         """
         Retrieves information about a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_workspace)
         """
-
     async def list_component_types(
         self,
         *,
         workspaceId: str,
         filters: Sequence[ListComponentTypesFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListComponentTypesResponseTypeDef:
         """
         Lists all component types in a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_component_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_component_types)
         """
-
     async def list_entities(
         self,
         *,
         workspaceId: str,
         filters: Sequence[ListEntitiesFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListEntitiesResponseTypeDef:
         """
         Lists all entities in a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_entities)
         """
-
     async def list_scenes(
         self, *, workspaceId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListScenesResponseTypeDef:
         """
         Lists all scenes in a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_scenes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_scenes)
         """
-
     async def list_sync_jobs(
         self, *, workspaceId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListSyncJobsResponseTypeDef:
         """
         List all SyncJobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_sync_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_sync_jobs)
         """
-
     async def list_sync_resources(
         self,
         *,
         workspaceId: str,
         syncSource: str,
         filters: Sequence[SyncResourceFilterTypeDef] = ...,
         maxResults: int = ...,
@@ -449,51 +418,46 @@
     ) -> ListSyncResourcesResponseTypeDef:
         """
         Lists the sync resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_sync_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_sync_resources)
         """
-
     async def list_tags_for_resource(
         self, *, resourceARN: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all tags associated with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_tags_for_resource)
         """
-
     async def list_workspaces(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListWorkspacesResponseTypeDef:
         """
         Retrieves information about workspaces in the current account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_workspaces)
         """
-
     async def tag_resource(self, *, resourceARN: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#tag_resource)
         """
-
     async def untag_resource(self, *, resourceARN: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#untag_resource)
         """
-
     async def update_component_type(
         self,
         *,
         workspaceId: str,
         componentTypeId: str,
         isSingleton: bool = ...,
         description: str = ...,
@@ -505,15 +469,14 @@
     ) -> UpdateComponentTypeResponseTypeDef:
         """
         Updates information in a component type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_component_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_component_type)
         """
-
     async def update_entity(
         self,
         *,
         workspaceId: str,
         entityId: str,
         entityName: str = ...,
         description: str = ...,
@@ -522,25 +485,23 @@
     ) -> UpdateEntityResponseTypeDef:
         """
         Updates an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_entity)
         """
-
     async def update_pricing_plan(
         self, *, pricingMode: PricingModeType, bundleNames: Sequence[str] = ...
     ) -> UpdatePricingPlanResponseTypeDef:
         """
         Update the pricing plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_pricing_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_pricing_plan)
         """
-
     async def update_scene(
         self,
         *,
         workspaceId: str,
         sceneId: str,
         contentLocation: str = ...,
         description: str = ...,
@@ -549,29 +510,26 @@
     ) -> UpdateSceneResponseTypeDef:
         """
         Updates a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_scene)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_scene)
         """
-
     async def update_workspace(
         self, *, workspaceId: str, description: str = ..., role: str = ...
     ) -> UpdateWorkspaceResponseTypeDef:
         """
         Updates a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_workspace)
         """
-
     async def __aenter__(self) -> "IoTTwinMakerClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/)
         """
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/client.pyi` & `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from types_aiobotocore_iottwinmaker.client import IoTTwinMakerClient
 
     session = get_session()
     async with session.create_client("iottwinmaker") as client:
         client: IoTTwinMakerClient
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import OrderByTimeType, PricingModeType
 from .type_defs import (
     BatchPutPropertyValuesResponseTypeDef,
@@ -53,47 +52,51 @@
     ListSyncResourcesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkspacesResponseTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyFilterTypeDef,
     PropertyGroupRequestTypeDef,
-    PropertyValueEntryTypeDef,
+    PropertyValueEntryUnionTypeDef,
     SyncResourceFilterTypeDef,
     TabularConditionsTypeDef,
+    TimestampTypeDef,
     UpdateComponentTypeResponseTypeDef,
     UpdateEntityResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     UpdateSceneResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
 )
 
 __all__ = ("IoTTwinMakerClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ConnectorFailureException: Type[BotocoreClientError]
     ConnectorTimeoutException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     QueryTimeoutException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class IoTTwinMakerClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/)
     """
 
     meta: ClientMeta
@@ -102,37 +105,41 @@
     def exceptions(self) -> Exceptions:
         """
         IoTTwinMakerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#exceptions)
         """
+
     async def batch_put_property_values(
-        self, *, workspaceId: str, entries: Sequence[PropertyValueEntryTypeDef]
+        self, *, workspaceId: str, entries: Sequence[PropertyValueEntryUnionTypeDef]
     ) -> BatchPutPropertyValuesResponseTypeDef:
         """
         Sets values for multiple time series properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.batch_put_property_values)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#batch_put_property_values)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#close)
         """
+
     async def create_component_type(
         self,
         *,
         workspaceId: str,
         componentTypeId: str,
         isSingleton: bool = ...,
         description: str = ...,
@@ -145,14 +152,15 @@
     ) -> CreateComponentTypeResponseTypeDef:
         """
         Creates a component type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_component_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_component_type)
         """
+
     async def create_entity(
         self,
         *,
         workspaceId: str,
         entityName: str,
         entityId: str = ...,
         description: str = ...,
@@ -162,14 +170,15 @@
     ) -> CreateEntityResponseTypeDef:
         """
         Creates an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_entity)
         """
+
     async def create_scene(
         self,
         *,
         workspaceId: str,
         sceneId: str,
         contentLocation: str,
         description: str = ...,
@@ -179,23 +188,25 @@
     ) -> CreateSceneResponseTypeDef:
         """
         Creates a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_scene)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_scene)
         """
+
     async def create_sync_job(
         self, *, workspaceId: str, syncSource: str, syncRole: str, tags: Mapping[str, str] = ...
     ) -> CreateSyncJobResponseTypeDef:
         """
         This action creates a SyncJob.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_sync_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_sync_job)
         """
+
     async def create_workspace(
         self,
         *,
         workspaceId: str,
         s3Location: str,
         role: str,
         description: str = ...,
@@ -203,101 +214,112 @@
     ) -> CreateWorkspaceResponseTypeDef:
         """
         Creates a workplace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.create_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#create_workspace)
         """
+
     async def delete_component_type(
         self, *, workspaceId: str, componentTypeId: str
     ) -> DeleteComponentTypeResponseTypeDef:
         """
         Deletes a component type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.delete_component_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#delete_component_type)
         """
+
     async def delete_entity(
         self, *, workspaceId: str, entityId: str, isRecursive: bool = ...
     ) -> DeleteEntityResponseTypeDef:
         """
         Deletes an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.delete_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#delete_entity)
         """
+
     async def delete_scene(self, *, workspaceId: str, sceneId: str) -> Dict[str, Any]:
         """
         Deletes a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.delete_scene)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#delete_scene)
         """
+
     async def delete_sync_job(
         self, *, workspaceId: str, syncSource: str
     ) -> DeleteSyncJobResponseTypeDef:
         """
         Delete the SyncJob.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.delete_sync_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#delete_sync_job)
         """
+
     async def delete_workspace(self, *, workspaceId: str) -> Dict[str, Any]:
         """
         Deletes a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.delete_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#delete_workspace)
         """
+
     async def execute_query(
         self, *, workspaceId: str, queryStatement: str, maxResults: int = ..., nextToken: str = ...
     ) -> ExecuteQueryResponseTypeDef:
         """
         Run queries to access information from your knowledge graph of entities within
         individual workspaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.execute_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#execute_query)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#generate_presigned_url)
         """
+
     async def get_component_type(
         self, *, workspaceId: str, componentTypeId: str
     ) -> GetComponentTypeResponseTypeDef:
         """
         Retrieves information about a component type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_component_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_component_type)
         """
+
     async def get_entity(self, *, workspaceId: str, entityId: str) -> GetEntityResponseTypeDef:
         """
         Retrieves information about an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_entity)
         """
+
     async def get_pricing_plan(self) -> GetPricingPlanResponseTypeDef:
         """
         Gets the pricing plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_pricing_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_pricing_plan)
         """
+
     async def get_property_value(
         self,
         *,
         selectedProperties: Sequence[str],
         workspaceId: str,
         componentName: str = ...,
         componentTypeId: str = ...,
@@ -309,108 +331,117 @@
     ) -> GetPropertyValueResponseTypeDef:
         """
         Gets the property values for a component, component type, entity, or workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_property_value)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_property_value)
         """
+
     async def get_property_value_history(
         self,
         *,
         workspaceId: str,
         selectedProperties: Sequence[str],
         entityId: str = ...,
         componentName: str = ...,
         componentTypeId: str = ...,
         propertyFilters: Sequence[PropertyFilterTypeDef] = ...,
-        startDateTime: Union[datetime, str] = ...,
-        endDateTime: Union[datetime, str] = ...,
+        startDateTime: TimestampTypeDef = ...,
+        endDateTime: TimestampTypeDef = ...,
         interpolation: InterpolationParametersTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         orderByTime: OrderByTimeType = ...,
         startTime: str = ...,
         endTime: str = ...
     ) -> GetPropertyValueHistoryResponseTypeDef:
         """
         Retrieves information about the history of a time series property value for a
         component, component type, entity, or workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_property_value_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_property_value_history)
         """
+
     async def get_scene(self, *, workspaceId: str, sceneId: str) -> GetSceneResponseTypeDef:
         """
         Retrieves information about a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_scene)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_scene)
         """
+
     async def get_sync_job(
         self, *, syncSource: str, workspaceId: str = ...
     ) -> GetSyncJobResponseTypeDef:
         """
         Gets the SyncJob.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_sync_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_sync_job)
         """
+
     async def get_workspace(self, *, workspaceId: str) -> GetWorkspaceResponseTypeDef:
         """
         Retrieves information about a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.get_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#get_workspace)
         """
+
     async def list_component_types(
         self,
         *,
         workspaceId: str,
         filters: Sequence[ListComponentTypesFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> ListComponentTypesResponseTypeDef:
         """
         Lists all component types in a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_component_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_component_types)
         """
+
     async def list_entities(
         self,
         *,
         workspaceId: str,
         filters: Sequence[ListEntitiesFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListEntitiesResponseTypeDef:
         """
         Lists all entities in a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_entities)
         """
+
     async def list_scenes(
         self, *, workspaceId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListScenesResponseTypeDef:
         """
         Lists all scenes in a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_scenes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_scenes)
         """
+
     async def list_sync_jobs(
         self, *, workspaceId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListSyncJobsResponseTypeDef:
         """
         List all SyncJobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_sync_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_sync_jobs)
         """
+
     async def list_sync_resources(
         self,
         *,
         workspaceId: str,
         syncSource: str,
         filters: Sequence[SyncResourceFilterTypeDef] = ...,
         maxResults: int = ...,
@@ -418,46 +449,51 @@
     ) -> ListSyncResourcesResponseTypeDef:
         """
         Lists the sync resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_sync_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_sync_resources)
         """
+
     async def list_tags_for_resource(
         self, *, resourceARN: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all tags associated with a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_tags_for_resource)
         """
+
     async def list_workspaces(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListWorkspacesResponseTypeDef:
         """
         Retrieves information about workspaces in the current account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.list_workspaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#list_workspaces)
         """
+
     async def tag_resource(self, *, resourceARN: str, tags: Mapping[str, str]) -> Dict[str, Any]:
         """
         Adds tags to a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#tag_resource)
         """
+
     async def untag_resource(self, *, resourceARN: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#untag_resource)
         """
+
     async def update_component_type(
         self,
         *,
         workspaceId: str,
         componentTypeId: str,
         isSingleton: bool = ...,
         description: str = ...,
@@ -469,14 +505,15 @@
     ) -> UpdateComponentTypeResponseTypeDef:
         """
         Updates information in a component type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_component_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_component_type)
         """
+
     async def update_entity(
         self,
         *,
         workspaceId: str,
         entityId: str,
         entityName: str = ...,
         description: str = ...,
@@ -485,23 +522,25 @@
     ) -> UpdateEntityResponseTypeDef:
         """
         Updates an entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_entity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_entity)
         """
+
     async def update_pricing_plan(
         self, *, pricingMode: PricingModeType, bundleNames: Sequence[str] = ...
     ) -> UpdatePricingPlanResponseTypeDef:
         """
         Update the pricing plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_pricing_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_pricing_plan)
         """
+
     async def update_scene(
         self,
         *,
         workspaceId: str,
         sceneId: str,
         contentLocation: str = ...,
         description: str = ...,
@@ -510,26 +549,29 @@
     ) -> UpdateSceneResponseTypeDef:
         """
         Updates a scene.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_scene)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_scene)
         """
+
     async def update_workspace(
         self, *, workspaceId: str, description: str = ..., role: str = ...
     ) -> UpdateWorkspaceResponseTypeDef:
         """
         Updates a workspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client.update_workspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/#update_workspace)
         """
+
     async def __aenter__(self) -> "IoTTwinMakerClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/client/)
         """
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/literals.py` & `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/literals.pyi` & `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/type_defs.py` & `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iottwinmaker service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_iottwinmaker.type_defs import BundleInformationTypeDef
+    from types_aiobotocore_iottwinmaker.type_defs import ResponseMetadataTypeDef
 
-    data: BundleInformationTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -42,129 +42,147 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ResponseMetadataTypeDef",
     "BundleInformationTypeDef",
     "ColumnDescriptionTypeDef",
     "ComponentPropertyGroupRequestTypeDef",
     "ComponentPropertyGroupResponseTypeDef",
     "PropertyDefinitionRequestTypeDef",
     "PropertyGroupRequestTypeDef",
-    "CreateComponentTypeResponseTypeDef",
-    "CreateEntityResponseTypeDef",
     "CreateSceneRequestRequestTypeDef",
-    "CreateSceneResponseTypeDef",
     "CreateSyncJobRequestRequestTypeDef",
-    "CreateSyncJobResponseTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
-    "CreateWorkspaceResponseTypeDef",
     "LambdaFunctionTypeDef",
     "RelationshipTypeDef",
     "RelationshipValueTypeDef",
     "DeleteComponentTypeRequestRequestTypeDef",
-    "DeleteComponentTypeResponseTypeDef",
     "DeleteEntityRequestRequestTypeDef",
-    "DeleteEntityResponseTypeDef",
     "DeleteSceneRequestRequestTypeDef",
     "DeleteSyncJobRequestRequestTypeDef",
-    "DeleteSyncJobResponseTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
+    "EntityPropertyReferenceOutputTypeDef",
     "EntityPropertyReferenceTypeDef",
     "ErrorDetailsTypeDef",
     "ExecuteQueryRequestRequestTypeDef",
     "RowTypeDef",
     "GetComponentTypeRequestRequestTypeDef",
     "PropertyDefinitionResponseTypeDef",
     "PropertyGroupResponseTypeDef",
     "GetEntityRequestRequestTypeDef",
     "InterpolationParametersTypeDef",
     "PropertyFilterTypeDef",
+    "TimestampTypeDef",
     "GetSceneRequestRequestTypeDef",
     "SceneErrorTypeDef",
     "GetSyncJobRequestRequestTypeDef",
     "GetWorkspaceRequestRequestTypeDef",
-    "GetWorkspaceResponseTypeDef",
     "ListComponentTypesFilterTypeDef",
     "ListEntitiesFilterTypeDef",
     "ListScenesRequestRequestTypeDef",
     "SceneSummaryTypeDef",
     "ListSyncJobsRequestRequestTypeDef",
     "SyncResourceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "WorkspaceSummaryTypeDef",
     "OrderByTypeDef",
     "ParentEntityUpdateRequestTypeDef",
-    "PropertyValueTypeDef",
-    "ResponseMetadataTypeDef",
+    "PropertyValueOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateComponentTypeResponseTypeDef",
-    "UpdateEntityResponseTypeDef",
     "UpdatePricingPlanRequestRequestTypeDef",
     "UpdateSceneRequestRequestTypeDef",
-    "UpdateSceneResponseTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
+    "CreateComponentTypeResponseTypeDef",
+    "CreateEntityResponseTypeDef",
+    "CreateSceneResponseTypeDef",
+    "CreateSyncJobResponseTypeDef",
+    "CreateWorkspaceResponseTypeDef",
+    "DeleteComponentTypeResponseTypeDef",
+    "DeleteEntityResponseTypeDef",
+    "DeleteSyncJobResponseTypeDef",
+    "GetWorkspaceResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateComponentTypeResponseTypeDef",
+    "UpdateEntityResponseTypeDef",
+    "UpdateSceneResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "PricingPlanTypeDef",
     "PropertyRequestTypeDef",
     "DataConnectorTypeDef",
+    "DataTypeOutputTypeDef",
     "DataTypeTypeDef",
+    "DataValueOutputTypeDef",
     "DataValueTypeDef",
     "PropertyLatestValueTypeDef",
     "StatusTypeDef",
     "SyncJobStatusTypeDef",
     "SyncResourceStatusTypeDef",
     "ExecuteQueryResponseTypeDef",
     "PropertyResponseTypeDef",
     "GetPropertyValueHistoryRequestRequestTypeDef",
+    "PropertyValueTypeDef",
     "GetSceneResponseTypeDef",
     "ListComponentTypesRequestRequestTypeDef",
     "ListEntitiesRequestRequestTypeDef",
     "ListScenesResponseTypeDef",
     "ListSyncResourcesRequestRequestTypeDef",
     "ListWorkspacesResponseTypeDef",
     "TabularConditionsTypeDef",
-    "PropertyValueEntryTypeDef",
+    "PropertyValueEntryOutputTypeDef",
     "PropertyValueHistoryTypeDef",
     "GetPricingPlanResponseTypeDef",
     "UpdatePricingPlanResponseTypeDef",
     "ComponentRequestTypeDef",
     "ComponentUpdateRequestTypeDef",
     "FunctionRequestTypeDef",
     "FunctionResponseTypeDef",
     "GetPropertyValueResponseTypeDef",
     "ComponentTypeSummaryTypeDef",
     "EntitySummaryTypeDef",
     "GetSyncJobResponseTypeDef",
     "SyncJobSummaryTypeDef",
     "SyncResourceSummaryTypeDef",
     "ComponentResponseTypeDef",
+    "PropertyValueEntryTypeDef",
     "GetPropertyValueRequestRequestTypeDef",
     "BatchPutPropertyErrorTypeDef",
-    "BatchPutPropertyValuesRequestRequestTypeDef",
     "GetPropertyValueHistoryResponseTypeDef",
     "CreateEntityRequestRequestTypeDef",
     "UpdateEntityRequestRequestTypeDef",
     "CreateComponentTypeRequestRequestTypeDef",
     "UpdateComponentTypeRequestRequestTypeDef",
     "GetComponentTypeResponseTypeDef",
     "ListComponentTypesResponseTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListSyncJobsResponseTypeDef",
     "ListSyncResourcesResponseTypeDef",
     "GetEntityResponseTypeDef",
+    "PropertyValueEntryUnionTypeDef",
     "BatchPutPropertyErrorEntryTypeDef",
+    "BatchPutPropertyValuesRequestRequestTypeDef",
     "BatchPutPropertyValuesResponseTypeDef",
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
 _RequiredBundleInformationTypeDef = TypedDict(
     "_RequiredBundleInformationTypeDef",
     {
         "bundleNames": List[str],
     },
 )
 _OptionalBundleInformationTypeDef = TypedDict(
@@ -230,35 +248,14 @@
     {
         "groupType": Literal["TABULAR"],
         "propertyNames": Sequence[str],
     },
     total=False,
 )
 
-CreateComponentTypeResponseTypeDef = TypedDict(
-    "CreateComponentTypeResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEntityResponseTypeDef = TypedDict(
-    "CreateEntityResponseTypeDef",
-    {
-        "entityId": str,
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSceneRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
         "contentLocation": str,
     },
@@ -277,23 +274,14 @@
 
 class CreateSceneRequestRequestTypeDef(
     _RequiredCreateSceneRequestRequestTypeDef, _OptionalCreateSceneRequestRequestTypeDef
 ):
     pass
 
 
-CreateSceneResponseTypeDef = TypedDict(
-    "CreateSceneResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSyncJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSyncJobRequestRequestTypeDef",
     {
         "workspaceId": str,
         "syncSource": str,
         "syncRole": str,
     },
@@ -309,24 +297,14 @@
 
 class CreateSyncJobRequestRequestTypeDef(
     _RequiredCreateSyncJobRequestRequestTypeDef, _OptionalCreateSyncJobRequestRequestTypeDef
 ):
     pass
 
 
-CreateSyncJobResponseTypeDef = TypedDict(
-    "CreateSyncJobResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": SyncJobStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
         "s3Location": str,
         "role": str,
     },
@@ -343,23 +321,14 @@
 
 class CreateWorkspaceRequestRequestTypeDef(
     _RequiredCreateWorkspaceRequestRequestTypeDef, _OptionalCreateWorkspaceRequestRequestTypeDef
 ):
     pass
 
 
-CreateWorkspaceResponseTypeDef = TypedDict(
-    "CreateWorkspaceResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LambdaFunctionTypeDef = TypedDict(
     "LambdaFunctionTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -385,22 +354,14 @@
     "DeleteComponentTypeRequestRequestTypeDef",
     {
         "workspaceId": str,
         "componentTypeId": str,
     },
 )
 
-DeleteComponentTypeResponseTypeDef = TypedDict(
-    "DeleteComponentTypeResponseTypeDef",
-    {
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteEntityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
         "entityId": str,
     },
 )
@@ -415,22 +376,14 @@
 
 class DeleteEntityRequestRequestTypeDef(
     _RequiredDeleteEntityRequestRequestTypeDef, _OptionalDeleteEntityRequestRequestTypeDef
 ):
     pass
 
 
-DeleteEntityResponseTypeDef = TypedDict(
-    "DeleteEntityResponseTypeDef",
-    {
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSceneRequestRequestTypeDef = TypedDict(
     "DeleteSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
     },
 )
@@ -439,29 +392,44 @@
     "DeleteSyncJobRequestRequestTypeDef",
     {
         "workspaceId": str,
         "syncSource": str,
     },
 )
 
-DeleteSyncJobResponseTypeDef = TypedDict(
-    "DeleteSyncJobResponseTypeDef",
+DeleteWorkspaceRequestRequestTypeDef = TypedDict(
+    "DeleteWorkspaceRequestRequestTypeDef",
     {
-        "state": SyncJobStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "workspaceId": str,
     },
 )
 
-DeleteWorkspaceRequestRequestTypeDef = TypedDict(
-    "DeleteWorkspaceRequestRequestTypeDef",
+_RequiredEntityPropertyReferenceOutputTypeDef = TypedDict(
+    "_RequiredEntityPropertyReferenceOutputTypeDef",
     {
-        "workspaceId": str,
+        "propertyName": str,
+    },
+)
+_OptionalEntityPropertyReferenceOutputTypeDef = TypedDict(
+    "_OptionalEntityPropertyReferenceOutputTypeDef",
+    {
+        "componentName": str,
+        "externalIdProperty": Dict[str, str],
+        "entityId": str,
     },
+    total=False,
 )
 
+
+class EntityPropertyReferenceOutputTypeDef(
+    _RequiredEntityPropertyReferenceOutputTypeDef, _OptionalEntityPropertyReferenceOutputTypeDef
+):
+    pass
+
+
 _RequiredEntityPropertyReferenceTypeDef = TypedDict(
     "_RequiredEntityPropertyReferenceTypeDef",
     {
         "propertyName": str,
     },
 )
 _OptionalEntityPropertyReferenceTypeDef = TypedDict(
@@ -528,28 +496,28 @@
         "componentTypeId": str,
     },
 )
 
 _RequiredPropertyDefinitionResponseTypeDef = TypedDict(
     "_RequiredPropertyDefinitionResponseTypeDef",
     {
-        "dataType": "DataTypeTypeDef",
+        "dataType": "DataTypeOutputTypeDef",
         "isTimeSeries": bool,
         "isRequiredInEntity": bool,
         "isExternalId": bool,
         "isStoredExternally": bool,
         "isImported": bool,
         "isFinal": bool,
         "isInherited": bool,
     },
 )
 _OptionalPropertyDefinitionResponseTypeDef = TypedDict(
     "_OptionalPropertyDefinitionResponseTypeDef",
     {
-        "defaultValue": "DataValueTypeDef",
+        "defaultValue": "DataValueOutputTypeDef",
         "configuration": Dict[str, str],
         "displayName": str,
     },
     total=False,
 )
 
 
@@ -591,14 +559,15 @@
         "propertyName": str,
         "operator": str,
         "value": "DataValueTypeDef",
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 GetSceneRequestRequestTypeDef = TypedDict(
     "GetSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
     },
 )
@@ -636,28 +605,14 @@
 GetWorkspaceRequestRequestTypeDef = TypedDict(
     "GetWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
-GetWorkspaceResponseTypeDef = TypedDict(
-    "GetWorkspaceResponseTypeDef",
-    {
-        "workspaceId": str,
-        "arn": str,
-        "description": str,
-        "s3Location": str,
-        "role": str,
-        "creationDateTime": datetime,
-        "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListComponentTypesFilterTypeDef = TypedDict(
     "ListComponentTypesFilterTypeDef",
     {
         "extendsFrom": str,
         "namespace": str,
         "isAbstract": bool,
     },
@@ -771,23 +726,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -851,45 +797,36 @@
 
 class ParentEntityUpdateRequestTypeDef(
     _RequiredParentEntityUpdateRequestTypeDef, _OptionalParentEntityUpdateRequestTypeDef
 ):
     pass
 
 
-_RequiredPropertyValueTypeDef = TypedDict(
-    "_RequiredPropertyValueTypeDef",
+_RequiredPropertyValueOutputTypeDef = TypedDict(
+    "_RequiredPropertyValueOutputTypeDef",
     {
-        "value": "DataValueTypeDef",
+        "value": "DataValueOutputTypeDef",
     },
 )
-_OptionalPropertyValueTypeDef = TypedDict(
-    "_OptionalPropertyValueTypeDef",
+_OptionalPropertyValueOutputTypeDef = TypedDict(
+    "_OptionalPropertyValueOutputTypeDef",
     {
-        "timestamp": Union[datetime, str],
+        "timestamp": datetime,
         "time": str,
     },
     total=False,
 )
 
 
-class PropertyValueTypeDef(_RequiredPropertyValueTypeDef, _OptionalPropertyValueTypeDef):
+class PropertyValueOutputTypeDef(
+    _RequiredPropertyValueOutputTypeDef, _OptionalPropertyValueOutputTypeDef
+):
     pass
 
 
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
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -898,34 +835,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateComponentTypeResponseTypeDef = TypedDict(
-    "UpdateComponentTypeResponseTypeDef",
-    {
-        "workspaceId": str,
-        "arn": str,
-        "componentTypeId": str,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateEntityResponseTypeDef = TypedDict(
-    "UpdateEntityResponseTypeDef",
-    {
-        "updateDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePricingPlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePricingPlanRequestRequestTypeDef",
     {
         "pricingMode": PricingModeType,
     },
 )
 _OptionalUpdatePricingPlanRequestRequestTypeDef = TypedDict(
@@ -964,22 +881,14 @@
 
 class UpdateSceneRequestRequestTypeDef(
     _RequiredUpdateSceneRequestRequestTypeDef, _OptionalUpdateSceneRequestRequestTypeDef
 ):
     pass
 
 
-UpdateSceneResponseTypeDef = TypedDict(
-    "UpdateSceneResponseTypeDef",
-    {
-        "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalUpdateWorkspaceRequestRequestTypeDef = TypedDict(
@@ -994,19 +903,143 @@
 
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
 
+CreateComponentTypeResponseTypeDef = TypedDict(
+    "CreateComponentTypeResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEntityResponseTypeDef = TypedDict(
+    "CreateEntityResponseTypeDef",
+    {
+        "entityId": str,
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSceneResponseTypeDef = TypedDict(
+    "CreateSceneResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSyncJobResponseTypeDef = TypedDict(
+    "CreateSyncJobResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": SyncJobStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkspaceResponseTypeDef = TypedDict(
+    "CreateWorkspaceResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteComponentTypeResponseTypeDef = TypedDict(
+    "DeleteComponentTypeResponseTypeDef",
+    {
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteEntityResponseTypeDef = TypedDict(
+    "DeleteEntityResponseTypeDef",
+    {
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSyncJobResponseTypeDef = TypedDict(
+    "DeleteSyncJobResponseTypeDef",
+    {
+        "state": SyncJobStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkspaceResponseTypeDef = TypedDict(
+    "GetWorkspaceResponseTypeDef",
+    {
+        "workspaceId": str,
+        "arn": str,
+        "description": str,
+        "s3Location": str,
+        "role": str,
+        "creationDateTime": datetime,
+        "updateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateComponentTypeResponseTypeDef = TypedDict(
+    "UpdateComponentTypeResponseTypeDef",
+    {
+        "workspaceId": str,
+        "arn": str,
+        "componentTypeId": str,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEntityResponseTypeDef = TypedDict(
+    "UpdateEntityResponseTypeDef",
+    {
+        "updateDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSceneResponseTypeDef = TypedDict(
+    "UpdateSceneResponseTypeDef",
+    {
+        "updateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateWorkspaceResponseTypeDef = TypedDict(
     "UpdateWorkspaceResponseTypeDef",
     {
         "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPricingPlanTypeDef = TypedDict(
     "_RequiredPricingPlanTypeDef",
     {
         "effectiveDateTime": datetime,
@@ -1044,14 +1077,36 @@
     {
         "lambda": LambdaFunctionTypeDef,
         "isNative": bool,
     },
     total=False,
 )
 
+_RequiredDataTypeOutputTypeDef = TypedDict(
+    "_RequiredDataTypeOutputTypeDef",
+    {
+        "type": TypeType,
+    },
+)
+_OptionalDataTypeOutputTypeDef = TypedDict(
+    "_OptionalDataTypeOutputTypeDef",
+    {
+        "nestedType": Dict[str, Any],
+        "allowedValues": List["DataValueOutputTypeDef"],
+        "unitOfMeasure": str,
+        "relationship": RelationshipTypeDef,
+    },
+    total=False,
+)
+
+
+class DataTypeOutputTypeDef(_RequiredDataTypeOutputTypeDef, _OptionalDataTypeOutputTypeDef):
+    pass
+
+
 _RequiredDataTypeTypeDef = TypedDict(
     "_RequiredDataTypeTypeDef",
     {
         "type": TypeType,
     },
 )
 _OptionalDataTypeTypeDef = TypedDict(
@@ -1066,14 +1121,30 @@
 )
 
 
 class DataTypeTypeDef(_RequiredDataTypeTypeDef, _OptionalDataTypeTypeDef):
     pass
 
 
+DataValueOutputTypeDef = TypedDict(
+    "DataValueOutputTypeDef",
+    {
+        "booleanValue": bool,
+        "doubleValue": float,
+        "integerValue": int,
+        "longValue": int,
+        "stringValue": str,
+        "listValue": List[Dict[str, Any]],
+        "mapValue": Dict[str, Dict[str, Any]],
+        "relationshipValue": RelationshipValueTypeDef,
+        "expression": str,
+    },
+    total=False,
+)
+
 DataValueTypeDef = TypedDict(
     "DataValueTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
         "integerValue": int,
         "longValue": int,
@@ -1085,21 +1156,21 @@
     },
     total=False,
 )
 
 _RequiredPropertyLatestValueTypeDef = TypedDict(
     "_RequiredPropertyLatestValueTypeDef",
     {
-        "propertyReference": EntityPropertyReferenceTypeDef,
+        "propertyReference": EntityPropertyReferenceOutputTypeDef,
     },
 )
 _OptionalPropertyLatestValueTypeDef = TypedDict(
     "_OptionalPropertyLatestValueTypeDef",
     {
-        "propertyValue": "DataValueTypeDef",
+        "propertyValue": "DataValueOutputTypeDef",
     },
     total=False,
 )
 
 
 class PropertyLatestValueTypeDef(
     _RequiredPropertyLatestValueTypeDef, _OptionalPropertyLatestValueTypeDef
@@ -1136,23 +1207,23 @@
 
 ExecuteQueryResponseTypeDef = TypedDict(
     "ExecuteQueryResponseTypeDef",
     {
         "columnDescriptions": List[ColumnDescriptionTypeDef],
         "rows": List[RowTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PropertyResponseTypeDef = TypedDict(
     "PropertyResponseTypeDef",
     {
         "definition": PropertyDefinitionResponseTypeDef,
-        "value": "DataValueTypeDef",
+        "value": "DataValueOutputTypeDef",
     },
     total=False,
 )
 
 _RequiredGetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetPropertyValueHistoryRequestRequestTypeDef",
     {
@@ -1163,16 +1234,16 @@
 _OptionalGetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "_OptionalGetPropertyValueHistoryRequestRequestTypeDef",
     {
         "entityId": str,
         "componentName": str,
         "componentTypeId": str,
         "propertyFilters": Sequence[PropertyFilterTypeDef],
-        "startDateTime": Union[datetime, str],
-        "endDateTime": Union[datetime, str],
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
         "interpolation": InterpolationParametersTypeDef,
         "nextToken": str,
         "maxResults": int,
         "orderByTime": OrderByTimeType,
         "startTime": str,
         "endTime": str,
     },
@@ -1183,29 +1254,49 @@
 class GetPropertyValueHistoryRequestRequestTypeDef(
     _RequiredGetPropertyValueHistoryRequestRequestTypeDef,
     _OptionalGetPropertyValueHistoryRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredPropertyValueTypeDef = TypedDict(
+    "_RequiredPropertyValueTypeDef",
+    {
+        "value": "DataValueTypeDef",
+    },
+)
+_OptionalPropertyValueTypeDef = TypedDict(
+    "_OptionalPropertyValueTypeDef",
+    {
+        "timestamp": TimestampTypeDef,
+        "time": str,
+    },
+    total=False,
+)
+
+
+class PropertyValueTypeDef(_RequiredPropertyValueTypeDef, _OptionalPropertyValueTypeDef):
+    pass
+
+
 GetSceneResponseTypeDef = TypedDict(
     "GetSceneResponseTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
         "contentLocation": str,
         "arn": str,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "description": str,
         "capabilities": List[str],
         "sceneMetadata": Dict[str, str],
         "generatedSceneMetadata": Dict[str, str],
         "error": SceneErrorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListComponentTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentTypesRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1253,15 +1344,15 @@
 
 
 ListScenesResponseTypeDef = TypedDict(
     "ListScenesResponseTypeDef",
     {
         "sceneSummaries": List[SceneSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSyncResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListSyncResourcesRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1286,58 +1377,58 @@
 
 
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
         "workspaceSummaries": List[WorkspaceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TabularConditionsTypeDef = TypedDict(
     "TabularConditionsTypeDef",
     {
         "orderBy": Sequence[OrderByTypeDef],
         "propertyFilters": Sequence[PropertyFilterTypeDef],
     },
     total=False,
 )
 
-_RequiredPropertyValueEntryTypeDef = TypedDict(
-    "_RequiredPropertyValueEntryTypeDef",
+_RequiredPropertyValueEntryOutputTypeDef = TypedDict(
+    "_RequiredPropertyValueEntryOutputTypeDef",
     {
-        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+        "entityPropertyReference": EntityPropertyReferenceOutputTypeDef,
     },
 )
-_OptionalPropertyValueEntryTypeDef = TypedDict(
-    "_OptionalPropertyValueEntryTypeDef",
+_OptionalPropertyValueEntryOutputTypeDef = TypedDict(
+    "_OptionalPropertyValueEntryOutputTypeDef",
     {
-        "propertyValues": Sequence[PropertyValueTypeDef],
+        "propertyValues": List[PropertyValueOutputTypeDef],
     },
     total=False,
 )
 
 
-class PropertyValueEntryTypeDef(
-    _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
+class PropertyValueEntryOutputTypeDef(
+    _RequiredPropertyValueEntryOutputTypeDef, _OptionalPropertyValueEntryOutputTypeDef
 ):
     pass
 
 
 _RequiredPropertyValueHistoryTypeDef = TypedDict(
     "_RequiredPropertyValueHistoryTypeDef",
     {
-        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+        "entityPropertyReference": EntityPropertyReferenceOutputTypeDef,
     },
 )
 _OptionalPropertyValueHistoryTypeDef = TypedDict(
     "_OptionalPropertyValueHistoryTypeDef",
     {
-        "values": List[PropertyValueTypeDef],
+        "values": List[PropertyValueOutputTypeDef],
     },
     total=False,
 )
 
 
 class PropertyValueHistoryTypeDef(
     _RequiredPropertyValueHistoryTypeDef, _OptionalPropertyValueHistoryTypeDef
@@ -1346,24 +1437,24 @@
 
 
 GetPricingPlanResponseTypeDef = TypedDict(
     "GetPricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePricingPlanResponseTypeDef = TypedDict(
     "UpdatePricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComponentRequestTypeDef = TypedDict(
     "ComponentRequestTypeDef",
     {
         "description": str,
@@ -1408,16 +1499,16 @@
 )
 
 GetPropertyValueResponseTypeDef = TypedDict(
     "GetPropertyValueResponseTypeDef",
     {
         "propertyValues": Dict[str, PropertyLatestValueTypeDef],
         "nextToken": str,
-        "tabularPropertyValues": List[List[Dict[str, "DataValueTypeDef"]]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tabularPropertyValues": List[List[Dict[str, "DataValueOutputTypeDef"]]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredComponentTypeSummaryTypeDef = TypedDict(
     "_RequiredComponentTypeSummaryTypeDef",
     {
         "arn": str,
@@ -1475,15 +1566,15 @@
         "arn": str,
         "workspaceId": str,
         "syncSource": str,
         "syncRole": str,
         "status": SyncJobStatusTypeDef,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SyncJobSummaryTypeDef = TypedDict(
     "SyncJobSummaryTypeDef",
     {
         "arn": str,
@@ -1519,14 +1610,35 @@
         "properties": Dict[str, PropertyResponseTypeDef],
         "propertyGroups": Dict[str, ComponentPropertyGroupResponseTypeDef],
         "syncSource": str,
     },
     total=False,
 )
 
+_RequiredPropertyValueEntryTypeDef = TypedDict(
+    "_RequiredPropertyValueEntryTypeDef",
+    {
+        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+    },
+)
+_OptionalPropertyValueEntryTypeDef = TypedDict(
+    "_OptionalPropertyValueEntryTypeDef",
+    {
+        "propertyValues": Sequence[PropertyValueTypeDef],
+    },
+    total=False,
+)
+
+
+class PropertyValueEntryTypeDef(
+    _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
+):
+    pass
+
+
 _RequiredGetPropertyValueRequestRequestTypeDef = TypedDict(
     "_RequiredGetPropertyValueRequestRequestTypeDef",
     {
         "selectedProperties": Sequence[str],
         "workspaceId": str,
     },
 )
@@ -1552,32 +1664,24 @@
 
 
 BatchPutPropertyErrorTypeDef = TypedDict(
     "BatchPutPropertyErrorTypeDef",
     {
         "errorCode": str,
         "errorMessage": str,
-        "entry": PropertyValueEntryTypeDef,
-    },
-)
-
-BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
-    "BatchPutPropertyValuesRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "entries": Sequence[PropertyValueEntryTypeDef],
+        "entry": PropertyValueEntryOutputTypeDef,
     },
 )
 
 GetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetPropertyValueHistoryResponseTypeDef",
     {
         "propertyValues": List[PropertyValueHistoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEntityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1702,53 +1806,53 @@
         "arn": str,
         "isAbstract": bool,
         "isSchemaInitialized": bool,
         "status": StatusTypeDef,
         "propertyGroups": Dict[str, PropertyGroupResponseTypeDef],
         "syncSource": str,
         "componentTypeName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListComponentTypesResponseTypeDef = TypedDict(
     "ListComponentTypesResponseTypeDef",
     {
         "workspaceId": str,
         "componentTypeSummaries": List[ComponentTypeSummaryTypeDef],
         "nextToken": str,
         "maxResults": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitiesResponseTypeDef = TypedDict(
     "ListEntitiesResponseTypeDef",
     {
         "entitySummaries": List[EntitySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSyncJobsResponseTypeDef = TypedDict(
     "ListSyncJobsResponseTypeDef",
     {
         "syncJobSummaries": List[SyncJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSyncResourcesResponseTypeDef = TypedDict(
     "ListSyncResourcesResponseTypeDef",
     {
         "syncResources": List[SyncResourceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEntityResponseTypeDef = TypedDict(
     "GetEntityResponseTypeDef",
     {
         "entityId": str,
@@ -1759,25 +1863,34 @@
         "description": str,
         "components": Dict[str, ComponentResponseTypeDef],
         "parentEntityId": str,
         "hasChildEntities": bool,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "syncSource": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PropertyValueEntryUnionTypeDef = Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]
 BatchPutPropertyErrorEntryTypeDef = TypedDict(
     "BatchPutPropertyErrorEntryTypeDef",
     {
         "errors": List[BatchPutPropertyErrorTypeDef],
     },
 )
 
+BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
+    "BatchPutPropertyValuesRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "entries": Sequence[PropertyValueEntryUnionTypeDef],
+    },
+)
+
 BatchPutPropertyValuesResponseTypeDef = TypedDict(
     "BatchPutPropertyValuesResponseTypeDef",
     {
         "errorEntries": List[BatchPutPropertyErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker/type_defs.pyi` & `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iottwinmaker service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_iottwinmaker.type_defs import BundleInformationTypeDef
+    from types_aiobotocore_iottwinmaker.type_defs import ResponseMetadataTypeDef
 
-    data: BundleInformationTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -41,129 +41,147 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ResponseMetadataTypeDef",
     "BundleInformationTypeDef",
     "ColumnDescriptionTypeDef",
     "ComponentPropertyGroupRequestTypeDef",
     "ComponentPropertyGroupResponseTypeDef",
     "PropertyDefinitionRequestTypeDef",
     "PropertyGroupRequestTypeDef",
-    "CreateComponentTypeResponseTypeDef",
-    "CreateEntityResponseTypeDef",
     "CreateSceneRequestRequestTypeDef",
-    "CreateSceneResponseTypeDef",
     "CreateSyncJobRequestRequestTypeDef",
-    "CreateSyncJobResponseTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
-    "CreateWorkspaceResponseTypeDef",
     "LambdaFunctionTypeDef",
     "RelationshipTypeDef",
     "RelationshipValueTypeDef",
     "DeleteComponentTypeRequestRequestTypeDef",
-    "DeleteComponentTypeResponseTypeDef",
     "DeleteEntityRequestRequestTypeDef",
-    "DeleteEntityResponseTypeDef",
     "DeleteSceneRequestRequestTypeDef",
     "DeleteSyncJobRequestRequestTypeDef",
-    "DeleteSyncJobResponseTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
+    "EntityPropertyReferenceOutputTypeDef",
     "EntityPropertyReferenceTypeDef",
     "ErrorDetailsTypeDef",
     "ExecuteQueryRequestRequestTypeDef",
     "RowTypeDef",
     "GetComponentTypeRequestRequestTypeDef",
     "PropertyDefinitionResponseTypeDef",
     "PropertyGroupResponseTypeDef",
     "GetEntityRequestRequestTypeDef",
     "InterpolationParametersTypeDef",
     "PropertyFilterTypeDef",
+    "TimestampTypeDef",
     "GetSceneRequestRequestTypeDef",
     "SceneErrorTypeDef",
     "GetSyncJobRequestRequestTypeDef",
     "GetWorkspaceRequestRequestTypeDef",
-    "GetWorkspaceResponseTypeDef",
     "ListComponentTypesFilterTypeDef",
     "ListEntitiesFilterTypeDef",
     "ListScenesRequestRequestTypeDef",
     "SceneSummaryTypeDef",
     "ListSyncJobsRequestRequestTypeDef",
     "SyncResourceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "WorkspaceSummaryTypeDef",
     "OrderByTypeDef",
     "ParentEntityUpdateRequestTypeDef",
-    "PropertyValueTypeDef",
-    "ResponseMetadataTypeDef",
+    "PropertyValueOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateComponentTypeResponseTypeDef",
-    "UpdateEntityResponseTypeDef",
     "UpdatePricingPlanRequestRequestTypeDef",
     "UpdateSceneRequestRequestTypeDef",
-    "UpdateSceneResponseTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
+    "CreateComponentTypeResponseTypeDef",
+    "CreateEntityResponseTypeDef",
+    "CreateSceneResponseTypeDef",
+    "CreateSyncJobResponseTypeDef",
+    "CreateWorkspaceResponseTypeDef",
+    "DeleteComponentTypeResponseTypeDef",
+    "DeleteEntityResponseTypeDef",
+    "DeleteSyncJobResponseTypeDef",
+    "GetWorkspaceResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateComponentTypeResponseTypeDef",
+    "UpdateEntityResponseTypeDef",
+    "UpdateSceneResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "PricingPlanTypeDef",
     "PropertyRequestTypeDef",
     "DataConnectorTypeDef",
+    "DataTypeOutputTypeDef",
     "DataTypeTypeDef",
+    "DataValueOutputTypeDef",
     "DataValueTypeDef",
     "PropertyLatestValueTypeDef",
     "StatusTypeDef",
     "SyncJobStatusTypeDef",
     "SyncResourceStatusTypeDef",
     "ExecuteQueryResponseTypeDef",
     "PropertyResponseTypeDef",
     "GetPropertyValueHistoryRequestRequestTypeDef",
+    "PropertyValueTypeDef",
     "GetSceneResponseTypeDef",
     "ListComponentTypesRequestRequestTypeDef",
     "ListEntitiesRequestRequestTypeDef",
     "ListScenesResponseTypeDef",
     "ListSyncResourcesRequestRequestTypeDef",
     "ListWorkspacesResponseTypeDef",
     "TabularConditionsTypeDef",
-    "PropertyValueEntryTypeDef",
+    "PropertyValueEntryOutputTypeDef",
     "PropertyValueHistoryTypeDef",
     "GetPricingPlanResponseTypeDef",
     "UpdatePricingPlanResponseTypeDef",
     "ComponentRequestTypeDef",
     "ComponentUpdateRequestTypeDef",
     "FunctionRequestTypeDef",
     "FunctionResponseTypeDef",
     "GetPropertyValueResponseTypeDef",
     "ComponentTypeSummaryTypeDef",
     "EntitySummaryTypeDef",
     "GetSyncJobResponseTypeDef",
     "SyncJobSummaryTypeDef",
     "SyncResourceSummaryTypeDef",
     "ComponentResponseTypeDef",
+    "PropertyValueEntryTypeDef",
     "GetPropertyValueRequestRequestTypeDef",
     "BatchPutPropertyErrorTypeDef",
-    "BatchPutPropertyValuesRequestRequestTypeDef",
     "GetPropertyValueHistoryResponseTypeDef",
     "CreateEntityRequestRequestTypeDef",
     "UpdateEntityRequestRequestTypeDef",
     "CreateComponentTypeRequestRequestTypeDef",
     "UpdateComponentTypeRequestRequestTypeDef",
     "GetComponentTypeResponseTypeDef",
     "ListComponentTypesResponseTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListSyncJobsResponseTypeDef",
     "ListSyncResourcesResponseTypeDef",
     "GetEntityResponseTypeDef",
+    "PropertyValueEntryUnionTypeDef",
     "BatchPutPropertyErrorEntryTypeDef",
+    "BatchPutPropertyValuesRequestRequestTypeDef",
     "BatchPutPropertyValuesResponseTypeDef",
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
 _RequiredBundleInformationTypeDef = TypedDict(
     "_RequiredBundleInformationTypeDef",
     {
         "bundleNames": List[str],
     },
 )
 _OptionalBundleInformationTypeDef = TypedDict(
@@ -227,35 +245,14 @@
     {
         "groupType": Literal["TABULAR"],
         "propertyNames": Sequence[str],
     },
     total=False,
 )
 
-CreateComponentTypeResponseTypeDef = TypedDict(
-    "CreateComponentTypeResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEntityResponseTypeDef = TypedDict(
-    "CreateEntityResponseTypeDef",
-    {
-        "entityId": str,
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSceneRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
         "contentLocation": str,
     },
@@ -272,23 +269,14 @@
 )
 
 class CreateSceneRequestRequestTypeDef(
     _RequiredCreateSceneRequestRequestTypeDef, _OptionalCreateSceneRequestRequestTypeDef
 ):
     pass
 
-CreateSceneResponseTypeDef = TypedDict(
-    "CreateSceneResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSyncJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSyncJobRequestRequestTypeDef",
     {
         "workspaceId": str,
         "syncSource": str,
         "syncRole": str,
     },
@@ -302,24 +290,14 @@
 )
 
 class CreateSyncJobRequestRequestTypeDef(
     _RequiredCreateSyncJobRequestRequestTypeDef, _OptionalCreateSyncJobRequestRequestTypeDef
 ):
     pass
 
-CreateSyncJobResponseTypeDef = TypedDict(
-    "CreateSyncJobResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": SyncJobStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
         "s3Location": str,
         "role": str,
     },
@@ -334,23 +312,14 @@
 )
 
 class CreateWorkspaceRequestRequestTypeDef(
     _RequiredCreateWorkspaceRequestRequestTypeDef, _OptionalCreateWorkspaceRequestRequestTypeDef
 ):
     pass
 
-CreateWorkspaceResponseTypeDef = TypedDict(
-    "CreateWorkspaceResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LambdaFunctionTypeDef = TypedDict(
     "LambdaFunctionTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -376,22 +345,14 @@
     "DeleteComponentTypeRequestRequestTypeDef",
     {
         "workspaceId": str,
         "componentTypeId": str,
     },
 )
 
-DeleteComponentTypeResponseTypeDef = TypedDict(
-    "DeleteComponentTypeResponseTypeDef",
-    {
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteEntityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
         "entityId": str,
     },
 )
@@ -404,22 +365,14 @@
 )
 
 class DeleteEntityRequestRequestTypeDef(
     _RequiredDeleteEntityRequestRequestTypeDef, _OptionalDeleteEntityRequestRequestTypeDef
 ):
     pass
 
-DeleteEntityResponseTypeDef = TypedDict(
-    "DeleteEntityResponseTypeDef",
-    {
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSceneRequestRequestTypeDef = TypedDict(
     "DeleteSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
     },
 )
@@ -428,29 +381,42 @@
     "DeleteSyncJobRequestRequestTypeDef",
     {
         "workspaceId": str,
         "syncSource": str,
     },
 )
 
-DeleteSyncJobResponseTypeDef = TypedDict(
-    "DeleteSyncJobResponseTypeDef",
+DeleteWorkspaceRequestRequestTypeDef = TypedDict(
+    "DeleteWorkspaceRequestRequestTypeDef",
     {
-        "state": SyncJobStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "workspaceId": str,
     },
 )
 
-DeleteWorkspaceRequestRequestTypeDef = TypedDict(
-    "DeleteWorkspaceRequestRequestTypeDef",
+_RequiredEntityPropertyReferenceOutputTypeDef = TypedDict(
+    "_RequiredEntityPropertyReferenceOutputTypeDef",
     {
-        "workspaceId": str,
+        "propertyName": str,
+    },
+)
+_OptionalEntityPropertyReferenceOutputTypeDef = TypedDict(
+    "_OptionalEntityPropertyReferenceOutputTypeDef",
+    {
+        "componentName": str,
+        "externalIdProperty": Dict[str, str],
+        "entityId": str,
     },
+    total=False,
 )
 
+class EntityPropertyReferenceOutputTypeDef(
+    _RequiredEntityPropertyReferenceOutputTypeDef, _OptionalEntityPropertyReferenceOutputTypeDef
+):
+    pass
+
 _RequiredEntityPropertyReferenceTypeDef = TypedDict(
     "_RequiredEntityPropertyReferenceTypeDef",
     {
         "propertyName": str,
     },
 )
 _OptionalEntityPropertyReferenceTypeDef = TypedDict(
@@ -513,28 +479,28 @@
         "componentTypeId": str,
     },
 )
 
 _RequiredPropertyDefinitionResponseTypeDef = TypedDict(
     "_RequiredPropertyDefinitionResponseTypeDef",
     {
-        "dataType": "DataTypeTypeDef",
+        "dataType": "DataTypeOutputTypeDef",
         "isTimeSeries": bool,
         "isRequiredInEntity": bool,
         "isExternalId": bool,
         "isStoredExternally": bool,
         "isImported": bool,
         "isFinal": bool,
         "isInherited": bool,
     },
 )
 _OptionalPropertyDefinitionResponseTypeDef = TypedDict(
     "_OptionalPropertyDefinitionResponseTypeDef",
     {
-        "defaultValue": "DataValueTypeDef",
+        "defaultValue": "DataValueOutputTypeDef",
         "configuration": Dict[str, str],
         "displayName": str,
     },
     total=False,
 )
 
 class PropertyDefinitionResponseTypeDef(
@@ -574,14 +540,15 @@
         "propertyName": str,
         "operator": str,
         "value": "DataValueTypeDef",
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 GetSceneRequestRequestTypeDef = TypedDict(
     "GetSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
     },
 )
@@ -617,28 +584,14 @@
 GetWorkspaceRequestRequestTypeDef = TypedDict(
     "GetWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
-GetWorkspaceResponseTypeDef = TypedDict(
-    "GetWorkspaceResponseTypeDef",
-    {
-        "workspaceId": str,
-        "arn": str,
-        "description": str,
-        "s3Location": str,
-        "role": str,
-        "creationDateTime": datetime,
-        "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListComponentTypesFilterTypeDef = TypedDict(
     "ListComponentTypesFilterTypeDef",
     {
         "extendsFrom": str,
         "namespace": str,
         "isAbstract": bool,
     },
@@ -744,23 +697,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -818,43 +762,34 @@
 )
 
 class ParentEntityUpdateRequestTypeDef(
     _RequiredParentEntityUpdateRequestTypeDef, _OptionalParentEntityUpdateRequestTypeDef
 ):
     pass
 
-_RequiredPropertyValueTypeDef = TypedDict(
-    "_RequiredPropertyValueTypeDef",
+_RequiredPropertyValueOutputTypeDef = TypedDict(
+    "_RequiredPropertyValueOutputTypeDef",
     {
-        "value": "DataValueTypeDef",
+        "value": "DataValueOutputTypeDef",
     },
 )
-_OptionalPropertyValueTypeDef = TypedDict(
-    "_OptionalPropertyValueTypeDef",
+_OptionalPropertyValueOutputTypeDef = TypedDict(
+    "_OptionalPropertyValueOutputTypeDef",
     {
-        "timestamp": Union[datetime, str],
+        "timestamp": datetime,
         "time": str,
     },
     total=False,
 )
 
-class PropertyValueTypeDef(_RequiredPropertyValueTypeDef, _OptionalPropertyValueTypeDef):
+class PropertyValueOutputTypeDef(
+    _RequiredPropertyValueOutputTypeDef, _OptionalPropertyValueOutputTypeDef
+):
     pass
 
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
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -863,34 +798,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateComponentTypeResponseTypeDef = TypedDict(
-    "UpdateComponentTypeResponseTypeDef",
-    {
-        "workspaceId": str,
-        "arn": str,
-        "componentTypeId": str,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateEntityResponseTypeDef = TypedDict(
-    "UpdateEntityResponseTypeDef",
-    {
-        "updateDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePricingPlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePricingPlanRequestRequestTypeDef",
     {
         "pricingMode": PricingModeType,
     },
 )
 _OptionalUpdatePricingPlanRequestRequestTypeDef = TypedDict(
@@ -925,22 +840,14 @@
 )
 
 class UpdateSceneRequestRequestTypeDef(
     _RequiredUpdateSceneRequestRequestTypeDef, _OptionalUpdateSceneRequestRequestTypeDef
 ):
     pass
 
-UpdateSceneResponseTypeDef = TypedDict(
-    "UpdateSceneResponseTypeDef",
-    {
-        "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalUpdateWorkspaceRequestRequestTypeDef = TypedDict(
@@ -953,19 +860,143 @@
 )
 
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
+CreateComponentTypeResponseTypeDef = TypedDict(
+    "CreateComponentTypeResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEntityResponseTypeDef = TypedDict(
+    "CreateEntityResponseTypeDef",
+    {
+        "entityId": str,
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSceneResponseTypeDef = TypedDict(
+    "CreateSceneResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSyncJobResponseTypeDef = TypedDict(
+    "CreateSyncJobResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": SyncJobStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkspaceResponseTypeDef = TypedDict(
+    "CreateWorkspaceResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteComponentTypeResponseTypeDef = TypedDict(
+    "DeleteComponentTypeResponseTypeDef",
+    {
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteEntityResponseTypeDef = TypedDict(
+    "DeleteEntityResponseTypeDef",
+    {
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSyncJobResponseTypeDef = TypedDict(
+    "DeleteSyncJobResponseTypeDef",
+    {
+        "state": SyncJobStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkspaceResponseTypeDef = TypedDict(
+    "GetWorkspaceResponseTypeDef",
+    {
+        "workspaceId": str,
+        "arn": str,
+        "description": str,
+        "s3Location": str,
+        "role": str,
+        "creationDateTime": datetime,
+        "updateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateComponentTypeResponseTypeDef = TypedDict(
+    "UpdateComponentTypeResponseTypeDef",
+    {
+        "workspaceId": str,
+        "arn": str,
+        "componentTypeId": str,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEntityResponseTypeDef = TypedDict(
+    "UpdateEntityResponseTypeDef",
+    {
+        "updateDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSceneResponseTypeDef = TypedDict(
+    "UpdateSceneResponseTypeDef",
+    {
+        "updateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateWorkspaceResponseTypeDef = TypedDict(
     "UpdateWorkspaceResponseTypeDef",
     {
         "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPricingPlanTypeDef = TypedDict(
     "_RequiredPricingPlanTypeDef",
     {
         "effectiveDateTime": datetime,
@@ -1001,14 +1032,34 @@
     {
         "lambda": LambdaFunctionTypeDef,
         "isNative": bool,
     },
     total=False,
 )
 
+_RequiredDataTypeOutputTypeDef = TypedDict(
+    "_RequiredDataTypeOutputTypeDef",
+    {
+        "type": TypeType,
+    },
+)
+_OptionalDataTypeOutputTypeDef = TypedDict(
+    "_OptionalDataTypeOutputTypeDef",
+    {
+        "nestedType": Dict[str, Any],
+        "allowedValues": List["DataValueOutputTypeDef"],
+        "unitOfMeasure": str,
+        "relationship": RelationshipTypeDef,
+    },
+    total=False,
+)
+
+class DataTypeOutputTypeDef(_RequiredDataTypeOutputTypeDef, _OptionalDataTypeOutputTypeDef):
+    pass
+
 _RequiredDataTypeTypeDef = TypedDict(
     "_RequiredDataTypeTypeDef",
     {
         "type": TypeType,
     },
 )
 _OptionalDataTypeTypeDef = TypedDict(
@@ -1021,14 +1072,30 @@
     },
     total=False,
 )
 
 class DataTypeTypeDef(_RequiredDataTypeTypeDef, _OptionalDataTypeTypeDef):
     pass
 
+DataValueOutputTypeDef = TypedDict(
+    "DataValueOutputTypeDef",
+    {
+        "booleanValue": bool,
+        "doubleValue": float,
+        "integerValue": int,
+        "longValue": int,
+        "stringValue": str,
+        "listValue": List[Dict[str, Any]],
+        "mapValue": Dict[str, Dict[str, Any]],
+        "relationshipValue": RelationshipValueTypeDef,
+        "expression": str,
+    },
+    total=False,
+)
+
 DataValueTypeDef = TypedDict(
     "DataValueTypeDef",
     {
         "booleanValue": bool,
         "doubleValue": float,
         "integerValue": int,
         "longValue": int,
@@ -1040,21 +1107,21 @@
     },
     total=False,
 )
 
 _RequiredPropertyLatestValueTypeDef = TypedDict(
     "_RequiredPropertyLatestValueTypeDef",
     {
-        "propertyReference": EntityPropertyReferenceTypeDef,
+        "propertyReference": EntityPropertyReferenceOutputTypeDef,
     },
 )
 _OptionalPropertyLatestValueTypeDef = TypedDict(
     "_OptionalPropertyLatestValueTypeDef",
     {
-        "propertyValue": "DataValueTypeDef",
+        "propertyValue": "DataValueOutputTypeDef",
     },
     total=False,
 )
 
 class PropertyLatestValueTypeDef(
     _RequiredPropertyLatestValueTypeDef, _OptionalPropertyLatestValueTypeDef
 ):
@@ -1089,23 +1156,23 @@
 
 ExecuteQueryResponseTypeDef = TypedDict(
     "ExecuteQueryResponseTypeDef",
     {
         "columnDescriptions": List[ColumnDescriptionTypeDef],
         "rows": List[RowTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PropertyResponseTypeDef = TypedDict(
     "PropertyResponseTypeDef",
     {
         "definition": PropertyDefinitionResponseTypeDef,
-        "value": "DataValueTypeDef",
+        "value": "DataValueOutputTypeDef",
     },
     total=False,
 )
 
 _RequiredGetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetPropertyValueHistoryRequestRequestTypeDef",
     {
@@ -1116,16 +1183,16 @@
 _OptionalGetPropertyValueHistoryRequestRequestTypeDef = TypedDict(
     "_OptionalGetPropertyValueHistoryRequestRequestTypeDef",
     {
         "entityId": str,
         "componentName": str,
         "componentTypeId": str,
         "propertyFilters": Sequence[PropertyFilterTypeDef],
-        "startDateTime": Union[datetime, str],
-        "endDateTime": Union[datetime, str],
+        "startDateTime": TimestampTypeDef,
+        "endDateTime": TimestampTypeDef,
         "interpolation": InterpolationParametersTypeDef,
         "nextToken": str,
         "maxResults": int,
         "orderByTime": OrderByTimeType,
         "startTime": str,
         "endTime": str,
     },
@@ -1134,29 +1201,47 @@
 
 class GetPropertyValueHistoryRequestRequestTypeDef(
     _RequiredGetPropertyValueHistoryRequestRequestTypeDef,
     _OptionalGetPropertyValueHistoryRequestRequestTypeDef,
 ):
     pass
 
+_RequiredPropertyValueTypeDef = TypedDict(
+    "_RequiredPropertyValueTypeDef",
+    {
+        "value": "DataValueTypeDef",
+    },
+)
+_OptionalPropertyValueTypeDef = TypedDict(
+    "_OptionalPropertyValueTypeDef",
+    {
+        "timestamp": TimestampTypeDef,
+        "time": str,
+    },
+    total=False,
+)
+
+class PropertyValueTypeDef(_RequiredPropertyValueTypeDef, _OptionalPropertyValueTypeDef):
+    pass
+
 GetSceneResponseTypeDef = TypedDict(
     "GetSceneResponseTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
         "contentLocation": str,
         "arn": str,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "description": str,
         "capabilities": List[str],
         "sceneMetadata": Dict[str, str],
         "generatedSceneMetadata": Dict[str, str],
         "error": SceneErrorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListComponentTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentTypesRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1200,15 +1285,15 @@
     pass
 
 ListScenesResponseTypeDef = TypedDict(
     "ListScenesResponseTypeDef",
     {
         "sceneSummaries": List[SceneSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSyncResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListSyncResourcesRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1231,80 +1316,80 @@
     pass
 
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
         "workspaceSummaries": List[WorkspaceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TabularConditionsTypeDef = TypedDict(
     "TabularConditionsTypeDef",
     {
         "orderBy": Sequence[OrderByTypeDef],
         "propertyFilters": Sequence[PropertyFilterTypeDef],
     },
     total=False,
 )
 
-_RequiredPropertyValueEntryTypeDef = TypedDict(
-    "_RequiredPropertyValueEntryTypeDef",
+_RequiredPropertyValueEntryOutputTypeDef = TypedDict(
+    "_RequiredPropertyValueEntryOutputTypeDef",
     {
-        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+        "entityPropertyReference": EntityPropertyReferenceOutputTypeDef,
     },
 )
-_OptionalPropertyValueEntryTypeDef = TypedDict(
-    "_OptionalPropertyValueEntryTypeDef",
+_OptionalPropertyValueEntryOutputTypeDef = TypedDict(
+    "_OptionalPropertyValueEntryOutputTypeDef",
     {
-        "propertyValues": Sequence[PropertyValueTypeDef],
+        "propertyValues": List[PropertyValueOutputTypeDef],
     },
     total=False,
 )
 
-class PropertyValueEntryTypeDef(
-    _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
+class PropertyValueEntryOutputTypeDef(
+    _RequiredPropertyValueEntryOutputTypeDef, _OptionalPropertyValueEntryOutputTypeDef
 ):
     pass
 
 _RequiredPropertyValueHistoryTypeDef = TypedDict(
     "_RequiredPropertyValueHistoryTypeDef",
     {
-        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+        "entityPropertyReference": EntityPropertyReferenceOutputTypeDef,
     },
 )
 _OptionalPropertyValueHistoryTypeDef = TypedDict(
     "_OptionalPropertyValueHistoryTypeDef",
     {
-        "values": List[PropertyValueTypeDef],
+        "values": List[PropertyValueOutputTypeDef],
     },
     total=False,
 )
 
 class PropertyValueHistoryTypeDef(
     _RequiredPropertyValueHistoryTypeDef, _OptionalPropertyValueHistoryTypeDef
 ):
     pass
 
 GetPricingPlanResponseTypeDef = TypedDict(
     "GetPricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePricingPlanResponseTypeDef = TypedDict(
     "UpdatePricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComponentRequestTypeDef = TypedDict(
     "ComponentRequestTypeDef",
     {
         "description": str,
@@ -1349,16 +1434,16 @@
 )
 
 GetPropertyValueResponseTypeDef = TypedDict(
     "GetPropertyValueResponseTypeDef",
     {
         "propertyValues": Dict[str, PropertyLatestValueTypeDef],
         "nextToken": str,
-        "tabularPropertyValues": List[List[Dict[str, "DataValueTypeDef"]]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tabularPropertyValues": List[List[Dict[str, "DataValueOutputTypeDef"]]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredComponentTypeSummaryTypeDef = TypedDict(
     "_RequiredComponentTypeSummaryTypeDef",
     {
         "arn": str,
@@ -1412,15 +1497,15 @@
         "arn": str,
         "workspaceId": str,
         "syncSource": str,
         "syncRole": str,
         "status": SyncJobStatusTypeDef,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SyncJobSummaryTypeDef = TypedDict(
     "SyncJobSummaryTypeDef",
     {
         "arn": str,
@@ -1456,14 +1541,33 @@
         "properties": Dict[str, PropertyResponseTypeDef],
         "propertyGroups": Dict[str, ComponentPropertyGroupResponseTypeDef],
         "syncSource": str,
     },
     total=False,
 )
 
+_RequiredPropertyValueEntryTypeDef = TypedDict(
+    "_RequiredPropertyValueEntryTypeDef",
+    {
+        "entityPropertyReference": EntityPropertyReferenceTypeDef,
+    },
+)
+_OptionalPropertyValueEntryTypeDef = TypedDict(
+    "_OptionalPropertyValueEntryTypeDef",
+    {
+        "propertyValues": Sequence[PropertyValueTypeDef],
+    },
+    total=False,
+)
+
+class PropertyValueEntryTypeDef(
+    _RequiredPropertyValueEntryTypeDef, _OptionalPropertyValueEntryTypeDef
+):
+    pass
+
 _RequiredGetPropertyValueRequestRequestTypeDef = TypedDict(
     "_RequiredGetPropertyValueRequestRequestTypeDef",
     {
         "selectedProperties": Sequence[str],
         "workspaceId": str,
     },
 )
@@ -1487,32 +1591,24 @@
     pass
 
 BatchPutPropertyErrorTypeDef = TypedDict(
     "BatchPutPropertyErrorTypeDef",
     {
         "errorCode": str,
         "errorMessage": str,
-        "entry": PropertyValueEntryTypeDef,
-    },
-)
-
-BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
-    "BatchPutPropertyValuesRequestRequestTypeDef",
-    {
-        "workspaceId": str,
-        "entries": Sequence[PropertyValueEntryTypeDef],
+        "entry": PropertyValueEntryOutputTypeDef,
     },
 )
 
 GetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetPropertyValueHistoryResponseTypeDef",
     {
         "propertyValues": List[PropertyValueHistoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEntityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1629,53 +1725,53 @@
         "arn": str,
         "isAbstract": bool,
         "isSchemaInitialized": bool,
         "status": StatusTypeDef,
         "propertyGroups": Dict[str, PropertyGroupResponseTypeDef],
         "syncSource": str,
         "componentTypeName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListComponentTypesResponseTypeDef = TypedDict(
     "ListComponentTypesResponseTypeDef",
     {
         "workspaceId": str,
         "componentTypeSummaries": List[ComponentTypeSummaryTypeDef],
         "nextToken": str,
         "maxResults": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitiesResponseTypeDef = TypedDict(
     "ListEntitiesResponseTypeDef",
     {
         "entitySummaries": List[EntitySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSyncJobsResponseTypeDef = TypedDict(
     "ListSyncJobsResponseTypeDef",
     {
         "syncJobSummaries": List[SyncJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSyncResourcesResponseTypeDef = TypedDict(
     "ListSyncResourcesResponseTypeDef",
     {
         "syncResources": List[SyncResourceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEntityResponseTypeDef = TypedDict(
     "GetEntityResponseTypeDef",
     {
         "entityId": str,
@@ -1686,25 +1782,34 @@
         "description": str,
         "components": Dict[str, ComponentResponseTypeDef],
         "parentEntityId": str,
         "hasChildEntities": bool,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "syncSource": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PropertyValueEntryUnionTypeDef = Union[PropertyValueEntryTypeDef, PropertyValueEntryOutputTypeDef]
 BatchPutPropertyErrorEntryTypeDef = TypedDict(
     "BatchPutPropertyErrorEntryTypeDef",
     {
         "errors": List[BatchPutPropertyErrorTypeDef],
     },
 )
 
+BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
+    "BatchPutPropertyValuesRequestRequestTypeDef",
+    {
+        "workspaceId": str,
+        "entries": Sequence[PropertyValueEntryUnionTypeDef],
+    },
+)
+
 BatchPutPropertyValuesResponseTypeDef = TypedDict(
     "BatchPutPropertyValuesResponseTypeDef",
     {
         "errorEntries": List[BatchPutPropertyErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO` & `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iottwinmaker
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTTwinMaker 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTTwinMaker 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iottwinmaker type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iottwinmaker type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iottwinmaker"></a>
 
 # types-aiobotocore-iottwinmaker
 
 [![PyPI - types-aiobotocore-iottwinmaker](https://img.shields.io/pypi/v/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iottwinmaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iottwinmaker?color=blue)](https://pypistats.org/packages/types-aiobotocore-iottwinmaker)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iottwinmaker)](https://pepy.tech/project/types-aiobotocore-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTTwinMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [types-aiobotocore-iottwinmaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iottwinmaker/).
 
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
@@ -300,140 +299,147 @@
 )
 
 
 def check_value(value: ColumnTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iottwinmaker.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iottwinmaker.type_defs import (
+    ResponseMetadataTypeDef,
     BundleInformationTypeDef,
     ColumnDescriptionTypeDef,
     ComponentPropertyGroupRequestTypeDef,
     ComponentPropertyGroupResponseTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyGroupRequestTypeDef,
-    CreateComponentTypeResponseTypeDef,
-    CreateEntityResponseTypeDef,
     CreateSceneRequestRequestTypeDef,
-    CreateSceneResponseTypeDef,
     CreateSyncJobRequestRequestTypeDef,
-    CreateSyncJobResponseTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
-    CreateWorkspaceResponseTypeDef,
     LambdaFunctionTypeDef,
     RelationshipTypeDef,
     RelationshipValueTypeDef,
     DeleteComponentTypeRequestRequestTypeDef,
-    DeleteComponentTypeResponseTypeDef,
     DeleteEntityRequestRequestTypeDef,
-    DeleteEntityResponseTypeDef,
     DeleteSceneRequestRequestTypeDef,
     DeleteSyncJobRequestRequestTypeDef,
-    DeleteSyncJobResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
+    EntityPropertyReferenceOutputTypeDef,
     EntityPropertyReferenceTypeDef,
     ErrorDetailsTypeDef,
     ExecuteQueryRequestRequestTypeDef,
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
     PropertyDefinitionResponseTypeDef,
     PropertyGroupResponseTypeDef,
     GetEntityRequestRequestTypeDef,
     InterpolationParametersTypeDef,
     PropertyFilterTypeDef,
+    TimestampTypeDef,
     GetSceneRequestRequestTypeDef,
     SceneErrorTypeDef,
     GetSyncJobRequestRequestTypeDef,
     GetWorkspaceRequestRequestTypeDef,
-    GetWorkspaceResponseTypeDef,
     ListComponentTypesFilterTypeDef,
     ListEntitiesFilterTypeDef,
     ListScenesRequestRequestTypeDef,
     SceneSummaryTypeDef,
     ListSyncJobsRequestRequestTypeDef,
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
-    PropertyValueTypeDef,
-    ResponseMetadataTypeDef,
+    PropertyValueOutputTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateComponentTypeResponseTypeDef,
-    UpdateEntityResponseTypeDef,
     UpdatePricingPlanRequestRequestTypeDef,
     UpdateSceneRequestRequestTypeDef,
-    UpdateSceneResponseTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
+    CreateComponentTypeResponseTypeDef,
+    CreateEntityResponseTypeDef,
+    CreateSceneResponseTypeDef,
+    CreateSyncJobResponseTypeDef,
+    CreateWorkspaceResponseTypeDef,
+    DeleteComponentTypeResponseTypeDef,
+    DeleteEntityResponseTypeDef,
+    DeleteSyncJobResponseTypeDef,
+    GetWorkspaceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateComponentTypeResponseTypeDef,
+    UpdateEntityResponseTypeDef,
+    UpdateSceneResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
     PricingPlanTypeDef,
     PropertyRequestTypeDef,
     DataConnectorTypeDef,
+    DataTypeOutputTypeDef,
     DataTypeTypeDef,
+    DataValueOutputTypeDef,
     DataValueTypeDef,
     PropertyLatestValueTypeDef,
     StatusTypeDef,
     SyncJobStatusTypeDef,
     SyncResourceStatusTypeDef,
     ExecuteQueryResponseTypeDef,
     PropertyResponseTypeDef,
     GetPropertyValueHistoryRequestRequestTypeDef,
+    PropertyValueTypeDef,
     GetSceneResponseTypeDef,
     ListComponentTypesRequestRequestTypeDef,
     ListEntitiesRequestRequestTypeDef,
     ListScenesResponseTypeDef,
     ListSyncResourcesRequestRequestTypeDef,
     ListWorkspacesResponseTypeDef,
     TabularConditionsTypeDef,
-    PropertyValueEntryTypeDef,
+    PropertyValueEntryOutputTypeDef,
     PropertyValueHistoryTypeDef,
     GetPricingPlanResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     ComponentRequestTypeDef,
     ComponentUpdateRequestTypeDef,
     FunctionRequestTypeDef,
     FunctionResponseTypeDef,
     GetPropertyValueResponseTypeDef,
     ComponentTypeSummaryTypeDef,
     EntitySummaryTypeDef,
     GetSyncJobResponseTypeDef,
     SyncJobSummaryTypeDef,
     SyncResourceSummaryTypeDef,
     ComponentResponseTypeDef,
+    PropertyValueEntryTypeDef,
     GetPropertyValueRequestRequestTypeDef,
     BatchPutPropertyErrorTypeDef,
-    BatchPutPropertyValuesRequestRequestTypeDef,
     GetPropertyValueHistoryResponseTypeDef,
     CreateEntityRequestRequestTypeDef,
     UpdateEntityRequestRequestTypeDef,
     CreateComponentTypeRequestRequestTypeDef,
     UpdateComponentTypeRequestRequestTypeDef,
     GetComponentTypeResponseTypeDef,
     ListComponentTypesResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListSyncJobsResponseTypeDef,
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
+    PropertyValueEntryUnionTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
+    BatchPutPropertyValuesRequestRequestTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
 )
 
 
-def get_structure() -> BundleInformationTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iottwinmaker-2.5.2/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt` & `types-aiobotocore-iottwinmaker-2.5.2.post1/types_aiobotocore_iottwinmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*


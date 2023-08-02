# Comparing `tmp/types-aiobotocore-iotthingsgraph-2.5.2.tar.gz` & `tmp/types-aiobotocore-iotthingsgraph-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotthingsgraph-2.5.2.tar", last modified: Sat Jul  8 01:43:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotthingsgraph-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:28 2023, max compression
```

## Comparing `types-aiobotocore-iotthingsgraph-2.5.2.tar` & `types-aiobotocore-iotthingsgraph-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:48.558337 types-aiobotocore-iotthingsgraph-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:55.000000 types-aiobotocore-iotthingsgraph-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-07-08 01:43:48.554337 types-aiobotocore-iotthingsgraph-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17743 2023-07-08 01:32:55.000000 types-aiobotocore-iotthingsgraph-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:48.558337 types-aiobotocore-iotthingsgraph-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 01:32:55.000000 types-aiobotocore-iotthingsgraph-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:48.546337 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-08 01:32:55.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-08 01:32:55.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:32:55.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31325 2023-07-08 01:32:56.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31271 2023-07-08 01:32:55.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-07-08 01:32:56.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-07-08 01:32:56.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-07-08 01:32:56.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13654 2023-07-08 01:32:56.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:55.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33777 2023-07-08 01:32:58.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33730 2023-07-08 01:32:57.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:55.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:48.554337 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-07-08 01:43:48.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:43:48.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:48.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:48.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:48.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:43:48.000000 types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.613556 types-aiobotocore-iotthingsgraph-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19294 2023-08-02 14:52:28.605557 types-aiobotocore-iotthingsgraph-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:28.613556 types-aiobotocore-iotthingsgraph-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.605557 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-08-02 14:40:59.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31248 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-08-02 14:40:59.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-08-02 14:40:59.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-08-02 14:40:59.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-08-02 14:40:59.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33751 2023-08-02 14:41:01.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33704 2023-08-02 14:41:01.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.605557 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19294 2023-08-02 14:52:28.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:28.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:28.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:28.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/LICENSE` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/PKG-INFO` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotthingsgraph
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTThingsGraph 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTThingsGraph 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotthingsgraph type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotthingsgraph type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotthingsgraph"></a>
 
 # types-aiobotocore-iotthingsgraph
 
 [![PyPI - types-aiobotocore-iotthingsgraph](https://img.shields.io/pypi/v/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotthingsgraph?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotthingsgraph)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotthingsgraph)](https://pepy.tech/project/types-aiobotocore-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTThingsGraph 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [types-aiobotocore-iotthingsgraph docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/).
 
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
@@ -363,116 +362,117 @@
 )
 
 
 def check_value(value: DefinitionLanguageType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotthingsgraph.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotthingsgraph.type_defs import (
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
+    ResponseMetadataTypeDef,
     MetricsConfigurationTypeDef,
     TagTypeDef,
     SystemInstanceSummaryTypeDef,
     SystemTemplateSummaryTypeDef,
     DeleteFlowTemplateRequestRequestTypeDef,
-    DeleteNamespaceResponseTypeDef,
     DeleteSystemInstanceRequestRequestTypeDef,
     DeleteSystemTemplateRequestRequestTypeDef,
     DependencyRevisionTypeDef,
     DeploySystemInstanceRequestRequestTypeDef,
     DeprecateFlowTemplateRequestRequestTypeDef,
     DeprecateSystemTemplateRequestRequestTypeDef,
     DescribeNamespaceRequestRequestTypeDef,
-    DescribeNamespaceResponseTypeDef,
     DissociateEntityFromThingRequestRequestTypeDef,
     EntityFilterTypeDef,
     FlowExecutionMessageTypeDef,
     FlowExecutionSummaryTypeDef,
     FlowTemplateFilterTypeDef,
     GetEntitiesRequestRequestTypeDef,
     GetFlowTemplateRequestRequestTypeDef,
-    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetFlowTemplateRevisionsRequestRequestTypeDef,
-    GetNamespaceDeletionStatusResponseTypeDef,
     GetSystemInstanceRequestRequestTypeDef,
     GetSystemTemplateRequestRequestTypeDef,
-    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
-    GetUploadStatusResponseTypeDef,
-    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    SearchFlowExecutionsRequestRequestTypeDef,
-    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+    TimestampTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
-    SearchThingsRequestSearchThingsPaginateTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadEntityDefinitionsResponseTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
     CreateSystemTemplateRequestRequestTypeDef,
     EntityDescriptionTypeDef,
     UpdateFlowTemplateRequestRequestTypeDef,
     UpdateSystemTemplateRequestRequestTypeDef,
     UploadEntityDefinitionsRequestRequestTypeDef,
-    CreateFlowTemplateResponseTypeDef,
     FlowTemplateDescriptionTypeDef,
+    CreateFlowTemplateResponseTypeDef,
+    DeleteNamespaceResponseTypeDef,
+    DescribeNamespaceResponseTypeDef,
     GetFlowTemplateRevisionsResponseTypeDef,
+    GetNamespaceDeletionStatusResponseTypeDef,
+    GetUploadStatusResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
+    UploadEntityDefinitionsResponseTypeDef,
     CreateSystemInstanceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSystemInstanceResponseTypeDef,
     DeploySystemInstanceResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     CreateSystemTemplateResponseTypeDef,
     GetSystemTemplateRevisionsResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SystemTemplateDescriptionTypeDef,
     UpdateSystemTemplateResponseTypeDef,
     SystemInstanceDescriptionTypeDef,
     SearchEntitiesRequestRequestTypeDef,
-    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     ListFlowExecutionMessagesResponseTypeDef,
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
+    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
+    SearchThingsRequestSearchThingsPaginateTypeDef,
+    SearchFlowExecutionsRequestRequestTypeDef,
+    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
     GetFlowTemplateResponseTypeDef,
     GetSystemTemplateResponseTypeDef,
     GetSystemInstanceResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateEntityToThingRequestRequestTypeDef:
+def get_value() -> AssociateEntityToThingRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/README.md` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iotthingsgraph"></a>
 
 # types-aiobotocore-iotthingsgraph
 
 [![PyPI - types-aiobotocore-iotthingsgraph](https://img.shields.io/pypi/v/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotthingsgraph?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotthingsgraph)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotthingsgraph)](https://pepy.tech/project/types-aiobotocore-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTThingsGraph 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [types-aiobotocore-iotthingsgraph docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/).
 
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
@@ -330,116 +330,117 @@
 )
 
 
 def check_value(value: DefinitionLanguageType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotthingsgraph.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotthingsgraph.type_defs import (
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
+    ResponseMetadataTypeDef,
     MetricsConfigurationTypeDef,
     TagTypeDef,
     SystemInstanceSummaryTypeDef,
     SystemTemplateSummaryTypeDef,
     DeleteFlowTemplateRequestRequestTypeDef,
-    DeleteNamespaceResponseTypeDef,
     DeleteSystemInstanceRequestRequestTypeDef,
     DeleteSystemTemplateRequestRequestTypeDef,
     DependencyRevisionTypeDef,
     DeploySystemInstanceRequestRequestTypeDef,
     DeprecateFlowTemplateRequestRequestTypeDef,
     DeprecateSystemTemplateRequestRequestTypeDef,
     DescribeNamespaceRequestRequestTypeDef,
-    DescribeNamespaceResponseTypeDef,
     DissociateEntityFromThingRequestRequestTypeDef,
     EntityFilterTypeDef,
     FlowExecutionMessageTypeDef,
     FlowExecutionSummaryTypeDef,
     FlowTemplateFilterTypeDef,
     GetEntitiesRequestRequestTypeDef,
     GetFlowTemplateRequestRequestTypeDef,
-    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetFlowTemplateRevisionsRequestRequestTypeDef,
-    GetNamespaceDeletionStatusResponseTypeDef,
     GetSystemInstanceRequestRequestTypeDef,
     GetSystemTemplateRequestRequestTypeDef,
-    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
-    GetUploadStatusResponseTypeDef,
-    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    SearchFlowExecutionsRequestRequestTypeDef,
-    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+    TimestampTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
-    SearchThingsRequestSearchThingsPaginateTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadEntityDefinitionsResponseTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
     CreateSystemTemplateRequestRequestTypeDef,
     EntityDescriptionTypeDef,
     UpdateFlowTemplateRequestRequestTypeDef,
     UpdateSystemTemplateRequestRequestTypeDef,
     UploadEntityDefinitionsRequestRequestTypeDef,
-    CreateFlowTemplateResponseTypeDef,
     FlowTemplateDescriptionTypeDef,
+    CreateFlowTemplateResponseTypeDef,
+    DeleteNamespaceResponseTypeDef,
+    DescribeNamespaceResponseTypeDef,
     GetFlowTemplateRevisionsResponseTypeDef,
+    GetNamespaceDeletionStatusResponseTypeDef,
+    GetUploadStatusResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
+    UploadEntityDefinitionsResponseTypeDef,
     CreateSystemInstanceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSystemInstanceResponseTypeDef,
     DeploySystemInstanceResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     CreateSystemTemplateResponseTypeDef,
     GetSystemTemplateRevisionsResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SystemTemplateDescriptionTypeDef,
     UpdateSystemTemplateResponseTypeDef,
     SystemInstanceDescriptionTypeDef,
     SearchEntitiesRequestRequestTypeDef,
-    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     ListFlowExecutionMessagesResponseTypeDef,
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
+    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
+    SearchThingsRequestSearchThingsPaginateTypeDef,
+    SearchFlowExecutionsRequestRequestTypeDef,
+    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
     GetFlowTemplateResponseTypeDef,
     GetSystemTemplateResponseTypeDef,
     GetSystemInstanceResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateEntityToThingRequestRequestTypeDef:
+def get_value() -> AssociateEntityToThingRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/setup.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotthingsgraph",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iotthingsgraph"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTThingsGraph 2.5.2 service generated with"
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
-    keywords="aiobotocore iotthingsgraph type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore iotthingsgraph type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotthingsgraph": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/"
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/__init__.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/__init__.pyi` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/__main__.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTThingsGraph 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IoTThingsGraph 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph\nOther"
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

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/client.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("iotthingsgraph") as client:
         client: IoTThingsGraphClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import DeploymentTargetType, EntityTypeType
 from .paginator import (
     GetFlowTemplateRevisionsPaginator,
@@ -60,14 +59,15 @@
     SearchFlowTemplatesResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SearchThingsResponseTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
     UpdateSystemTemplateResponseTypeDef,
     UploadEntityDefinitionsResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -384,16 +384,16 @@
         """
 
     async def search_flow_executions(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> SearchFlowExecutionsResponseTypeDef:
         """
         Searches for AWS IoT Things Graph workflow execution instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_flow_executions)
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/client.pyi` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("iotthingsgraph") as client:
         client: IoTThingsGraphClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import DeploymentTargetType, EntityTypeType
 from .paginator import (
     GetFlowTemplateRevisionsPaginator,
@@ -60,14 +59,15 @@
     SearchFlowTemplatesResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SearchThingsResponseTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
     UpdateSystemTemplateResponseTypeDef,
     UploadEntityDefinitionsResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -352,16 +352,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/client/#search_entities)
         """
     async def search_flow_executions(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> SearchFlowExecutionsResponseTypeDef:
         """
         Searches for AWS IoT Things Graph workflow execution instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Client.search_flow_executions)
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/literals.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/literals.pyi` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/paginator.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         search_flow_executions_paginator: SearchFlowExecutionsPaginator = client.get_paginator("search_flow_executions")
         search_flow_templates_paginator: SearchFlowTemplatesPaginator = client.get_paginator("search_flow_templates")
         search_system_instances_paginator: SearchSystemInstancesPaginator = client.get_paginator("search_system_instances")
         search_system_templates_paginator: SearchSystemTemplatesPaginator = client.get_paginator("search_system_templates")
         search_things_paginator: SearchThingsPaginator = client.get_paginator("search_things")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import EntityTypeType
 from .type_defs import (
     EntityFilterTypeDef,
@@ -57,14 +56,15 @@
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SearchThingsResponseTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "GetFlowTemplateRevisionsPaginator",
     "GetSystemTemplateRevisionsPaginator",
     "ListFlowExecutionMessagesPaginator",
     "ListTagsForResourcePaginator",
@@ -90,60 +90,60 @@
 class GetFlowTemplateRevisionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#getflowtemplaterevisionspaginator)
     """
 
     def paginate(
-        self, *, id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, id: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetFlowTemplateRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#getflowtemplaterevisionspaginator)
         """
 
 
 class GetSystemTemplateRevisionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#getsystemtemplaterevisionspaginator)
     """
 
     def paginate(
-        self, *, id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, id: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetSystemTemplateRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#getsystemtemplaterevisionspaginator)
         """
 
 
 class ListFlowExecutionMessagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#listflowexecutionmessagespaginator)
     """
 
     def paginate(
-        self, *, flowExecutionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, flowExecutionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFlowExecutionMessagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#listflowexecutionmessagespaginator)
         """
 
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#listtagsforresourcepaginator)
         """
 
 
@@ -155,15 +155,15 @@
 
     def paginate(
         self,
         *,
         entityTypes: Sequence[EntityTypeType],
         filters: Sequence[EntityFilterTypeDef] = ...,
         namespaceVersion: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchEntities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchentitiespaginator)
         """
 
 
@@ -174,17 +174,17 @@
     """
 
     def paginate(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchFlowExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchflowexecutionspaginator)
         """
 
 
@@ -194,15 +194,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchflowtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FlowTemplateFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchFlowTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchflowtemplatespaginator)
         """
 
 
@@ -212,15 +212,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsysteminstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemInstanceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchSystemInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsysteminstancespaginator)
         """
 
 
@@ -230,15 +230,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemTemplateFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchSystemTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
         """
 
 
@@ -249,13 +249,13 @@
     """
 
     def paginate(
         self,
         *,
         entityId: str,
         namespaceVersion: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchThings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchthingspaginator)
         """
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/paginator.pyi` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         search_flow_executions_paginator: SearchFlowExecutionsPaginator = client.get_paginator("search_flow_executions")
         search_flow_templates_paginator: SearchFlowTemplatesPaginator = client.get_paginator("search_flow_templates")
         search_system_instances_paginator: SearchSystemInstancesPaginator = client.get_paginator("search_system_instances")
         search_system_templates_paginator: SearchSystemTemplatesPaginator = client.get_paginator("search_system_templates")
         search_things_paginator: SearchThingsPaginator = client.get_paginator("search_things")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import EntityTypeType
 from .type_defs import (
     EntityFilterTypeDef,
@@ -57,14 +56,15 @@
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SearchThingsResponseTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "GetFlowTemplateRevisionsPaginator",
     "GetSystemTemplateRevisionsPaginator",
     "ListFlowExecutionMessagesPaginator",
     "ListTagsForResourcePaginator",
@@ -87,57 +87,57 @@
 class GetFlowTemplateRevisionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#getflowtemplaterevisionspaginator)
     """
 
     def paginate(
-        self, *, id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, id: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetFlowTemplateRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#getflowtemplaterevisionspaginator)
         """
 
 class GetSystemTemplateRevisionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#getsystemtemplaterevisionspaginator)
     """
 
     def paginate(
-        self, *, id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, id: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetSystemTemplateRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#getsystemtemplaterevisionspaginator)
         """
 
 class ListFlowExecutionMessagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#listflowexecutionmessagespaginator)
     """
 
     def paginate(
-        self, *, flowExecutionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, flowExecutionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFlowExecutionMessagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#listflowexecutionmessagespaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#listtagsforresourcepaginator)
         """
 
 class SearchEntitiesPaginator(AioPaginator):
@@ -148,15 +148,15 @@
 
     def paginate(
         self,
         *,
         entityTypes: Sequence[EntityTypeType],
         filters: Sequence[EntityFilterTypeDef] = ...,
         namespaceVersion: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchEntities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchentitiespaginator)
         """
 
 class SearchFlowExecutionsPaginator(AioPaginator):
@@ -166,17 +166,17 @@
     """
 
     def paginate(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchFlowExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchflowexecutionspaginator)
         """
 
 class SearchFlowTemplatesPaginator(AioPaginator):
@@ -185,15 +185,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchflowtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FlowTemplateFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchFlowTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchflowtemplatespaginator)
         """
 
 class SearchSystemInstancesPaginator(AioPaginator):
@@ -202,15 +202,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsysteminstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemInstanceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchSystemInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsysteminstancespaginator)
         """
 
 class SearchSystemTemplatesPaginator(AioPaginator):
@@ -219,15 +219,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemTemplateFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchSystemTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
         """
 
 class SearchThingsPaginator(AioPaginator):
@@ -237,13 +237,13 @@
     """
 
     def paginate(
         self,
         *,
         entityId: str,
         namespaceVersion: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchThings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/paginators/#searchthingspaginator)
         """
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/type_defs.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iotthingsgraph.type_defs import AssociateEntityToThingRequestRequestTypeDef
 
-    data: AssociateEntityToThingRequestRequestTypeDef = {...}
+    data: AssociateEntityToThingRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -32,95 +32,95 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateEntityToThingRequestRequestTypeDef",
     "DefinitionDocumentTypeDef",
     "FlowTemplateSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricsConfigurationTypeDef",
     "TagTypeDef",
     "SystemInstanceSummaryTypeDef",
     "SystemTemplateSummaryTypeDef",
     "DeleteFlowTemplateRequestRequestTypeDef",
-    "DeleteNamespaceResponseTypeDef",
     "DeleteSystemInstanceRequestRequestTypeDef",
     "DeleteSystemTemplateRequestRequestTypeDef",
     "DependencyRevisionTypeDef",
     "DeploySystemInstanceRequestRequestTypeDef",
     "DeprecateFlowTemplateRequestRequestTypeDef",
     "DeprecateSystemTemplateRequestRequestTypeDef",
     "DescribeNamespaceRequestRequestTypeDef",
-    "DescribeNamespaceResponseTypeDef",
     "DissociateEntityFromThingRequestRequestTypeDef",
     "EntityFilterTypeDef",
     "FlowExecutionMessageTypeDef",
     "FlowExecutionSummaryTypeDef",
     "FlowTemplateFilterTypeDef",
     "GetEntitiesRequestRequestTypeDef",
     "GetFlowTemplateRequestRequestTypeDef",
-    "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetFlowTemplateRevisionsRequestRequestTypeDef",
-    "GetNamespaceDeletionStatusResponseTypeDef",
     "GetSystemInstanceRequestRequestTypeDef",
     "GetSystemTemplateRequestRequestTypeDef",
-    "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
     "GetSystemTemplateRevisionsRequestRequestTypeDef",
     "GetUploadStatusRequestRequestTypeDef",
-    "GetUploadStatusResponseTypeDef",
-    "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
     "ListFlowExecutionMessagesRequestRequestTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "SearchFlowExecutionsRequestRequestTypeDef",
-    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+    "TimestampTypeDef",
     "SystemInstanceFilterTypeDef",
     "SystemTemplateFilterTypeDef",
     "SearchThingsRequestRequestTypeDef",
-    "SearchThingsRequestSearchThingsPaginateTypeDef",
     "ThingTypeDef",
     "UndeploySystemInstanceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UploadEntityDefinitionsResponseTypeDef",
     "CreateFlowTemplateRequestRequestTypeDef",
     "CreateSystemTemplateRequestRequestTypeDef",
     "EntityDescriptionTypeDef",
     "UpdateFlowTemplateRequestRequestTypeDef",
     "UpdateSystemTemplateRequestRequestTypeDef",
     "UploadEntityDefinitionsRequestRequestTypeDef",
-    "CreateFlowTemplateResponseTypeDef",
     "FlowTemplateDescriptionTypeDef",
+    "CreateFlowTemplateResponseTypeDef",
+    "DeleteNamespaceResponseTypeDef",
+    "DescribeNamespaceResponseTypeDef",
     "GetFlowTemplateRevisionsResponseTypeDef",
+    "GetNamespaceDeletionStatusResponseTypeDef",
+    "GetUploadStatusResponseTypeDef",
     "SearchFlowTemplatesResponseTypeDef",
     "UpdateFlowTemplateResponseTypeDef",
+    "UploadEntityDefinitionsResponseTypeDef",
     "CreateSystemInstanceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSystemInstanceResponseTypeDef",
     "DeploySystemInstanceResponseTypeDef",
     "SearchSystemInstancesResponseTypeDef",
     "UndeploySystemInstanceResponseTypeDef",
     "CreateSystemTemplateResponseTypeDef",
     "GetSystemTemplateRevisionsResponseTypeDef",
     "SearchSystemTemplatesResponseTypeDef",
     "SystemTemplateDescriptionTypeDef",
     "UpdateSystemTemplateResponseTypeDef",
     "SystemInstanceDescriptionTypeDef",
     "SearchEntitiesRequestRequestTypeDef",
-    "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     "ListFlowExecutionMessagesResponseTypeDef",
     "SearchFlowExecutionsResponseTypeDef",
     "SearchFlowTemplatesRequestRequestTypeDef",
+    "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
+    "SearchThingsRequestSearchThingsPaginateTypeDef",
+    "SearchFlowExecutionsRequestRequestTypeDef",
+    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SearchSystemInstancesRequestRequestTypeDef",
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     "SearchSystemTemplatesRequestRequestTypeDef",
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     "SearchThingsResponseTypeDef",
     "GetEntitiesResponseTypeDef",
     "SearchEntitiesResponseTypeDef",
@@ -140,22 +140,20 @@
     "_OptionalAssociateEntityToThingRequestRequestTypeDef",
     {
         "namespaceVersion": int,
     },
     total=False,
 )
 
-
 class AssociateEntityToThingRequestRequestTypeDef(
     _RequiredAssociateEntityToThingRequestRequestTypeDef,
     _OptionalAssociateEntityToThingRequestRequestTypeDef,
 ):
     pass
 
-
 DefinitionDocumentTypeDef = TypedDict(
     "DefinitionDocumentTypeDef",
     {
         "language": Literal["GRAPHQL"],
         "text": str,
     },
 )
@@ -167,14 +165,25 @@
         "arn": str,
         "revisionNumber": int,
         "createdAt": datetime,
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
 MetricsConfigurationTypeDef = TypedDict(
     "MetricsConfigurationTypeDef",
     {
         "cloudMetricEnabled": bool,
         "metricRuleRoleArn": str,
     },
     total=False,
@@ -218,23 +227,14 @@
 DeleteFlowTemplateRequestRequestTypeDef = TypedDict(
     "DeleteFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DeleteNamespaceResponseTypeDef = TypedDict(
-    "DeleteNamespaceResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSystemInstanceRequestRequestTypeDef = TypedDict(
     "DeleteSystemInstanceRequestRequestTypeDef",
     {
         "id": str,
     },
     total=False,
 )
@@ -281,26 +281,14 @@
     "DescribeNamespaceRequestRequestTypeDef",
     {
         "namespaceName": str,
     },
     total=False,
 )
 
-DescribeNamespaceResponseTypeDef = TypedDict(
-    "DescribeNamespaceResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "trackingNamespaceName": str,
-        "trackingNamespaceVersion": int,
-        "namespaceVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DissociateEntityFromThingRequestRequestTypeDef = TypedDict(
     "DissociateEntityFromThingRequestRequestTypeDef",
     {
         "thingName": str,
         "entityType": EntityTypeType,
     },
 )
@@ -356,64 +344,48 @@
     "_OptionalGetEntitiesRequestRequestTypeDef",
     {
         "namespaceVersion": int,
     },
     total=False,
 )
 
-
 class GetEntitiesRequestRequestTypeDef(
     _RequiredGetEntitiesRequestRequestTypeDef, _OptionalGetEntitiesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalGetFlowTemplateRequestRequestTypeDef",
     {
         "revisionNumber": int,
     },
     total=False,
 )
 
-
 class GetFlowTemplateRequestRequestTypeDef(
     _RequiredGetFlowTemplateRequestRequestTypeDef, _OptionalGetFlowTemplateRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
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
-class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
-    _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-    _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -421,34 +393,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetFlowTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
-
-GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
-    "GetNamespaceDeletionStatusResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "status": NamespaceDeletionStatusType,
-        "errorCode": Literal["VALIDATION_FAILED"],
-        "errorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSystemInstanceRequestRequestTypeDef = TypedDict(
     "GetSystemInstanceRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -462,43 +420,19 @@
     "_OptionalGetSystemTemplateRequestRequestTypeDef",
     {
         "revisionNumber": int,
     },
     total=False,
 )
 
-
 class GetSystemTemplateRequestRequestTypeDef(
     _RequiredGetSystemTemplateRequestRequestTypeDef, _OptionalGetSystemTemplateRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
-    _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-    _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSystemTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -506,65 +440,27 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetSystemTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetSystemTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
-
 GetUploadStatusRequestRequestTypeDef = TypedDict(
     "GetUploadStatusRequestRequestTypeDef",
     {
         "uploadId": str,
     },
 )
 
-GetUploadStatusResponseTypeDef = TypedDict(
-    "GetUploadStatusResponseTypeDef",
-    {
-        "uploadId": str,
-        "uploadStatus": UploadStatusType,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "namespaceVersion": int,
-        "failureReason": List[str],
-        "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
-    "_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    {
-        "flowExecutionId": str,
-    },
-)
-_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
-    "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
-    _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-    _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
     "_RequiredListFlowExecutionMessagesRequestRequestTypeDef",
     {
         "flowExecutionId": str,
     },
 )
 _OptionalListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
@@ -572,44 +468,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListFlowExecutionMessagesRequestRequestTypeDef(
     _RequiredListFlowExecutionMessagesRequestRequestTypeDef,
     _OptionalListFlowExecutionMessagesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -617,94 +489,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
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
-_RequiredSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchFlowExecutionsRequestRequestTypeDef",
-    {
-        "systemInstanceId": str,
-    },
-)
-_OptionalSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchFlowExecutionsRequestRequestTypeDef",
-    {
-        "flowExecutionId": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class SearchFlowExecutionsRequestRequestTypeDef(
-    _RequiredSearchFlowExecutionsRequestRequestTypeDef,
-    _OptionalSearchFlowExecutionsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
-    {
-        "systemInstanceId": str,
-    },
-)
-_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
-    {
-        "flowExecutionId": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
-    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 SystemInstanceFilterTypeDef = TypedDict(
     "SystemInstanceFilterTypeDef",
     {
         "name": SystemInstanceFilterNameType,
         "value": Sequence[str],
     },
     total=False,
@@ -730,44 +529,19 @@
         "nextToken": str,
         "maxResults": int,
         "namespaceVersion": int,
     },
     total=False,
 )
 
-
 class SearchThingsRequestRequestTypeDef(
     _RequiredSearchThingsRequestRequestTypeDef, _OptionalSearchThingsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
-    {
-        "entityId": str,
-    },
-)
-_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
-    {
-        "namespaceVersion": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SearchThingsRequestSearchThingsPaginateTypeDef(
-    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
-    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
-):
-    pass
-
-
 ThingTypeDef = TypedDict(
     "ThingTypeDef",
     {
         "thingArn": str,
         "thingName": str,
     },
     total=False,
@@ -785,66 +559,54 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UploadEntityDefinitionsResponseTypeDef = TypedDict(
-    "UploadEntityDefinitionsResponseTypeDef",
-    {
-        "uploadId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowTemplateRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
     },
 )
 _OptionalCreateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
-
 class CreateFlowTemplateRequestRequestTypeDef(
     _RequiredCreateFlowTemplateRequestRequestTypeDef,
     _OptionalCreateFlowTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSystemTemplateRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
     },
 )
 _OptionalCreateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSystemTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
-
 class CreateSystemTemplateRequestRequestTypeDef(
     _RequiredCreateSystemTemplateRequestRequestTypeDef,
     _OptionalCreateSystemTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 EntityDescriptionTypeDef = TypedDict(
     "EntityDescriptionTypeDef",
     {
         "id": str,
         "arn": str,
         "type": EntityTypeType,
         "createdAt": datetime,
@@ -864,22 +626,20 @@
     "_OptionalUpdateFlowTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
-
 class UpdateFlowTemplateRequestRequestTypeDef(
     _RequiredUpdateFlowTemplateRequestRequestTypeDef,
     _OptionalUpdateFlowTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSystemTemplateRequestRequestTypeDef",
     {
         "id": str,
         "definition": DefinitionDocumentTypeDef,
     },
 )
@@ -887,73 +647,126 @@
     "_OptionalUpdateSystemTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
-
 class UpdateSystemTemplateRequestRequestTypeDef(
     _RequiredUpdateSystemTemplateRequestRequestTypeDef,
     _OptionalUpdateSystemTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 UploadEntityDefinitionsRequestRequestTypeDef = TypedDict(
     "UploadEntityDefinitionsRequestRequestTypeDef",
     {
         "document": DefinitionDocumentTypeDef,
         "syncWithPublicNamespace": bool,
         "deprecateExistingEntities": bool,
     },
     total=False,
 )
 
+FlowTemplateDescriptionTypeDef = TypedDict(
+    "FlowTemplateDescriptionTypeDef",
+    {
+        "summary": FlowTemplateSummaryTypeDef,
+        "definition": DefinitionDocumentTypeDef,
+        "validatedNamespaceVersion": int,
+    },
+    total=False,
+)
+
 CreateFlowTemplateResponseTypeDef = TypedDict(
     "CreateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FlowTemplateDescriptionTypeDef = TypedDict(
-    "FlowTemplateDescriptionTypeDef",
+DeleteNamespaceResponseTypeDef = TypedDict(
+    "DeleteNamespaceResponseTypeDef",
     {
-        "summary": FlowTemplateSummaryTypeDef,
-        "definition": DefinitionDocumentTypeDef,
-        "validatedNamespaceVersion": int,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeNamespaceResponseTypeDef = TypedDict(
+    "DescribeNamespaceResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "trackingNamespaceName": str,
+        "trackingNamespaceVersion": int,
+        "namespaceVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetFlowTemplateRevisionsResponseTypeDef = TypedDict(
     "GetFlowTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
+    "GetNamespaceDeletionStatusResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "status": NamespaceDeletionStatusType,
+        "errorCode": Literal["VALIDATION_FAILED"],
+        "errorMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUploadStatusResponseTypeDef = TypedDict(
+    "GetUploadStatusResponseTypeDef",
+    {
+        "uploadId": str,
+        "uploadStatus": UploadStatusType,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "namespaceVersion": int,
+        "failureReason": List[str],
+        "createdDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFlowTemplatesResponseTypeDef = TypedDict(
     "SearchFlowTemplatesResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowTemplateResponseTypeDef = TypedDict(
     "UpdateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadEntityDefinitionsResponseTypeDef = TypedDict(
+    "UploadEntityDefinitionsResponseTypeDef",
+    {
+        "uploadId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSystemInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSystemInstanceRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
@@ -968,28 +781,26 @@
         "s3BucketName": str,
         "metricsConfiguration": MetricsConfigurationTypeDef,
         "flowActionsRoleArn": str,
     },
     total=False,
 )
 
-
 class CreateSystemInstanceRequestRequestTypeDef(
     _RequiredCreateSystemInstanceRequestRequestTypeDef,
     _OptionalCreateSystemInstanceRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -997,67 +808,67 @@
     },
 )
 
 CreateSystemInstanceResponseTypeDef = TypedDict(
     "CreateSystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploySystemInstanceResponseTypeDef = TypedDict(
     "DeploySystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
         "greengrassDeploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchSystemInstancesResponseTypeDef = TypedDict(
     "SearchSystemInstancesResponseTypeDef",
     {
         "summaries": List[SystemInstanceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UndeploySystemInstanceResponseTypeDef = TypedDict(
     "UndeploySystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSystemTemplateResponseTypeDef = TypedDict(
     "CreateSystemTemplateResponseTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSystemTemplateRevisionsResponseTypeDef = TypedDict(
     "GetSystemTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchSystemTemplatesResponseTypeDef = TypedDict(
     "SearchSystemTemplatesResponseTypeDef",
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SystemTemplateDescriptionTypeDef = TypedDict(
     "SystemTemplateDescriptionTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
@@ -1067,15 +878,15 @@
     total=False,
 )
 
 UpdateSystemTemplateResponseTypeDef = TypedDict(
     "UpdateSystemTemplateResponseTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SystemInstanceDescriptionTypeDef = TypedDict(
     "SystemInstanceDescriptionTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
@@ -1102,97 +913,241 @@
         "nextToken": str,
         "maxResults": int,
         "namespaceVersion": int,
     },
     total=False,
 )
 
-
 class SearchEntitiesRequestRequestTypeDef(
     _RequiredSearchEntitiesRequestRequestTypeDef, _OptionalSearchEntitiesRequestRequestTypeDef
 ):
     pass
 
+ListFlowExecutionMessagesResponseTypeDef = TypedDict(
+    "ListFlowExecutionMessagesResponseTypeDef",
+    {
+        "messages": List[FlowExecutionMessageTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchFlowExecutionsResponseTypeDef = TypedDict(
+    "SearchFlowExecutionsResponseTypeDef",
+    {
+        "summaries": List[FlowExecutionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchFlowTemplatesRequestRequestTypeDef = TypedDict(
+    "SearchFlowTemplatesRequestRequestTypeDef",
+    {
+        "filters": Sequence[FlowTemplateFilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
+    _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
+    _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+    _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
+    "_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    {
+        "flowExecutionId": str,
+    },
+)
+_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
+    "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
+    _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+    _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+):
+    pass
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
 
 _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "entityTypes": Sequence[EntityTypeType],
     },
 )
 _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "filters": Sequence[EntityFilterTypeDef],
         "namespaceVersion": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchEntitiesRequestSearchEntitiesPaginateTypeDef(
     _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
 ):
     pass
 
-
-ListFlowExecutionMessagesResponseTypeDef = TypedDict(
-    "ListFlowExecutionMessagesResponseTypeDef",
+SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
+    "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
     {
-        "messages": List[FlowExecutionMessageTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "filters": Sequence[FlowTemplateFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-SearchFlowExecutionsResponseTypeDef = TypedDict(
-    "SearchFlowExecutionsResponseTypeDef",
+_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
     {
-        "summaries": List[FlowExecutionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "entityId": str,
     },
 )
+_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
+    {
+        "namespaceVersion": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-SearchFlowTemplatesRequestRequestTypeDef = TypedDict(
-    "SearchFlowTemplatesRequestRequestTypeDef",
+class SearchThingsRequestSearchThingsPaginateTypeDef(
+    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
+    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
+):
+    pass
+
+_RequiredSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchFlowExecutionsRequestRequestTypeDef",
     {
-        "filters": Sequence[FlowTemplateFilterTypeDef],
+        "systemInstanceId": str,
+    },
+)
+_OptionalSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchFlowExecutionsRequestRequestTypeDef",
+    {
+        "flowExecutionId": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
-    "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
+class SearchFlowExecutionsRequestRequestTypeDef(
+    _RequiredSearchFlowExecutionsRequestRequestTypeDef,
+    _OptionalSearchFlowExecutionsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     {
-        "filters": Sequence[FlowTemplateFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "systemInstanceId": str,
+    },
+)
+_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+    {
+        "flowExecutionId": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
+    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+):
+    pass
+
 SearchSystemInstancesRequestRequestTypeDef = TypedDict(
     "SearchSystemInstancesRequestRequestTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
 SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef = TypedDict(
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 SearchSystemTemplatesRequestRequestTypeDef = TypedDict(
     "SearchSystemTemplatesRequestRequestTypeDef",
     {
@@ -1203,61 +1158,61 @@
     total=False,
 )
 
 SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef = TypedDict(
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     {
         "filters": Sequence[SystemTemplateFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 SearchThingsResponseTypeDef = TypedDict(
     "SearchThingsResponseTypeDef",
     {
         "things": List[ThingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEntitiesResponseTypeDef = TypedDict(
     "GetEntitiesResponseTypeDef",
     {
         "descriptions": List[EntityDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchEntitiesResponseTypeDef = TypedDict(
     "SearchEntitiesResponseTypeDef",
     {
         "descriptions": List[EntityDescriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFlowTemplateResponseTypeDef = TypedDict(
     "GetFlowTemplateResponseTypeDef",
     {
         "description": FlowTemplateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSystemTemplateResponseTypeDef = TypedDict(
     "GetSystemTemplateResponseTypeDef",
     {
         "description": SystemTemplateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSystemInstanceResponseTypeDef = TypedDict(
     "GetSystemInstanceResponseTypeDef",
     {
         "description": SystemInstanceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph/type_defs.pyi` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iotthingsgraph.type_defs import AssociateEntityToThingRequestRequestTypeDef
 
-    data: AssociateEntityToThingRequestRequestTypeDef = {...}
+    data: AssociateEntityToThingRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -32,94 +32,96 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateEntityToThingRequestRequestTypeDef",
     "DefinitionDocumentTypeDef",
     "FlowTemplateSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricsConfigurationTypeDef",
     "TagTypeDef",
     "SystemInstanceSummaryTypeDef",
     "SystemTemplateSummaryTypeDef",
     "DeleteFlowTemplateRequestRequestTypeDef",
-    "DeleteNamespaceResponseTypeDef",
     "DeleteSystemInstanceRequestRequestTypeDef",
     "DeleteSystemTemplateRequestRequestTypeDef",
     "DependencyRevisionTypeDef",
     "DeploySystemInstanceRequestRequestTypeDef",
     "DeprecateFlowTemplateRequestRequestTypeDef",
     "DeprecateSystemTemplateRequestRequestTypeDef",
     "DescribeNamespaceRequestRequestTypeDef",
-    "DescribeNamespaceResponseTypeDef",
     "DissociateEntityFromThingRequestRequestTypeDef",
     "EntityFilterTypeDef",
     "FlowExecutionMessageTypeDef",
     "FlowExecutionSummaryTypeDef",
     "FlowTemplateFilterTypeDef",
     "GetEntitiesRequestRequestTypeDef",
     "GetFlowTemplateRequestRequestTypeDef",
-    "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetFlowTemplateRevisionsRequestRequestTypeDef",
-    "GetNamespaceDeletionStatusResponseTypeDef",
     "GetSystemInstanceRequestRequestTypeDef",
     "GetSystemTemplateRequestRequestTypeDef",
-    "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
     "GetSystemTemplateRevisionsRequestRequestTypeDef",
     "GetUploadStatusRequestRequestTypeDef",
-    "GetUploadStatusResponseTypeDef",
-    "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
     "ListFlowExecutionMessagesRequestRequestTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "SearchFlowExecutionsRequestRequestTypeDef",
-    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+    "TimestampTypeDef",
     "SystemInstanceFilterTypeDef",
     "SystemTemplateFilterTypeDef",
     "SearchThingsRequestRequestTypeDef",
-    "SearchThingsRequestSearchThingsPaginateTypeDef",
     "ThingTypeDef",
     "UndeploySystemInstanceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UploadEntityDefinitionsResponseTypeDef",
     "CreateFlowTemplateRequestRequestTypeDef",
     "CreateSystemTemplateRequestRequestTypeDef",
     "EntityDescriptionTypeDef",
     "UpdateFlowTemplateRequestRequestTypeDef",
     "UpdateSystemTemplateRequestRequestTypeDef",
     "UploadEntityDefinitionsRequestRequestTypeDef",
-    "CreateFlowTemplateResponseTypeDef",
     "FlowTemplateDescriptionTypeDef",
+    "CreateFlowTemplateResponseTypeDef",
+    "DeleteNamespaceResponseTypeDef",
+    "DescribeNamespaceResponseTypeDef",
     "GetFlowTemplateRevisionsResponseTypeDef",
+    "GetNamespaceDeletionStatusResponseTypeDef",
+    "GetUploadStatusResponseTypeDef",
     "SearchFlowTemplatesResponseTypeDef",
     "UpdateFlowTemplateResponseTypeDef",
+    "UploadEntityDefinitionsResponseTypeDef",
     "CreateSystemInstanceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSystemInstanceResponseTypeDef",
     "DeploySystemInstanceResponseTypeDef",
     "SearchSystemInstancesResponseTypeDef",
     "UndeploySystemInstanceResponseTypeDef",
     "CreateSystemTemplateResponseTypeDef",
     "GetSystemTemplateRevisionsResponseTypeDef",
     "SearchSystemTemplatesResponseTypeDef",
     "SystemTemplateDescriptionTypeDef",
     "UpdateSystemTemplateResponseTypeDef",
     "SystemInstanceDescriptionTypeDef",
     "SearchEntitiesRequestRequestTypeDef",
-    "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     "ListFlowExecutionMessagesResponseTypeDef",
     "SearchFlowExecutionsResponseTypeDef",
     "SearchFlowTemplatesRequestRequestTypeDef",
+    "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
+    "SearchThingsRequestSearchThingsPaginateTypeDef",
+    "SearchFlowExecutionsRequestRequestTypeDef",
+    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SearchSystemInstancesRequestRequestTypeDef",
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     "SearchSystemTemplatesRequestRequestTypeDef",
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     "SearchThingsResponseTypeDef",
     "GetEntitiesResponseTypeDef",
     "SearchEntitiesResponseTypeDef",
@@ -139,20 +141,22 @@
     "_OptionalAssociateEntityToThingRequestRequestTypeDef",
     {
         "namespaceVersion": int,
     },
     total=False,
 )
 
+
 class AssociateEntityToThingRequestRequestTypeDef(
     _RequiredAssociateEntityToThingRequestRequestTypeDef,
     _OptionalAssociateEntityToThingRequestRequestTypeDef,
 ):
     pass
 
+
 DefinitionDocumentTypeDef = TypedDict(
     "DefinitionDocumentTypeDef",
     {
         "language": Literal["GRAPHQL"],
         "text": str,
     },
 )
@@ -164,14 +168,25 @@
         "arn": str,
         "revisionNumber": int,
         "createdAt": datetime,
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
 MetricsConfigurationTypeDef = TypedDict(
     "MetricsConfigurationTypeDef",
     {
         "cloudMetricEnabled": bool,
         "metricRuleRoleArn": str,
     },
     total=False,
@@ -215,23 +230,14 @@
 DeleteFlowTemplateRequestRequestTypeDef = TypedDict(
     "DeleteFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DeleteNamespaceResponseTypeDef = TypedDict(
-    "DeleteNamespaceResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSystemInstanceRequestRequestTypeDef = TypedDict(
     "DeleteSystemInstanceRequestRequestTypeDef",
     {
         "id": str,
     },
     total=False,
 )
@@ -278,26 +284,14 @@
     "DescribeNamespaceRequestRequestTypeDef",
     {
         "namespaceName": str,
     },
     total=False,
 )
 
-DescribeNamespaceResponseTypeDef = TypedDict(
-    "DescribeNamespaceResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "trackingNamespaceName": str,
-        "trackingNamespaceVersion": int,
-        "namespaceVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DissociateEntityFromThingRequestRequestTypeDef = TypedDict(
     "DissociateEntityFromThingRequestRequestTypeDef",
     {
         "thingName": str,
         "entityType": EntityTypeType,
     },
 )
@@ -353,58 +347,52 @@
     "_OptionalGetEntitiesRequestRequestTypeDef",
     {
         "namespaceVersion": int,
     },
     total=False,
 )
 
+
 class GetEntitiesRequestRequestTypeDef(
     _RequiredGetEntitiesRequestRequestTypeDef, _OptionalGetEntitiesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalGetFlowTemplateRequestRequestTypeDef",
     {
         "revisionNumber": int,
     },
     total=False,
 )
 
+
 class GetFlowTemplateRequestRequestTypeDef(
     _RequiredGetFlowTemplateRequestRequestTypeDef, _OptionalGetFlowTemplateRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+
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
 
-class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
-    _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-    _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -412,31 +400,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetFlowTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
-GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
-    "GetNamespaceDeletionStatusResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "status": NamespaceDeletionStatusType,
-        "errorCode": Literal["VALIDATION_FAILED"],
-        "errorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetSystemInstanceRequestRequestTypeDef = TypedDict(
     "GetSystemInstanceRequestRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -451,38 +429,20 @@
     "_OptionalGetSystemTemplateRequestRequestTypeDef",
     {
         "revisionNumber": int,
     },
     total=False,
 )
 
+
 class GetSystemTemplateRequestRequestTypeDef(
     _RequiredGetSystemTemplateRequestRequestTypeDef, _OptionalGetSystemTemplateRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
-    _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-    _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-):
-    pass
 
 _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSystemTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -491,61 +451,29 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetSystemTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetSystemTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
+
 GetUploadStatusRequestRequestTypeDef = TypedDict(
     "GetUploadStatusRequestRequestTypeDef",
     {
         "uploadId": str,
     },
 )
 
-GetUploadStatusResponseTypeDef = TypedDict(
-    "GetUploadStatusResponseTypeDef",
-    {
-        "uploadId": str,
-        "uploadStatus": UploadStatusType,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "namespaceVersion": int,
-        "failureReason": List[str],
-        "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
-    "_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    {
-        "flowExecutionId": str,
-    },
-)
-_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
-    "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
-    _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-    _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
     "_RequiredListFlowExecutionMessagesRequestRequestTypeDef",
     {
         "flowExecutionId": str,
     },
 )
 _OptionalListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
@@ -553,39 +481,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListFlowExecutionMessagesRequestRequestTypeDef(
     _RequiredListFlowExecutionMessagesRequestRequestTypeDef,
     _OptionalListFlowExecutionMessagesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
 
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
@@ -594,88 +504,23 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
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
-_RequiredSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
-    "_RequiredSearchFlowExecutionsRequestRequestTypeDef",
-    {
-        "systemInstanceId": str,
-    },
-)
-_OptionalSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
-    "_OptionalSearchFlowExecutionsRequestRequestTypeDef",
-    {
-        "flowExecutionId": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class SearchFlowExecutionsRequestRequestTypeDef(
-    _RequiredSearchFlowExecutionsRequestRequestTypeDef,
-    _OptionalSearchFlowExecutionsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
-    {
-        "systemInstanceId": str,
-    },
-)
-_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
-    {
-        "flowExecutionId": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
-    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-):
-    pass
 
+TimestampTypeDef = Union[datetime, str]
 SystemInstanceFilterTypeDef = TypedDict(
     "SystemInstanceFilterTypeDef",
     {
         "name": SystemInstanceFilterNameType,
         "value": Sequence[str],
     },
     total=False,
@@ -701,39 +546,20 @@
         "nextToken": str,
         "maxResults": int,
         "namespaceVersion": int,
     },
     total=False,
 )
 
+
 class SearchThingsRequestRequestTypeDef(
     _RequiredSearchThingsRequestRequestTypeDef, _OptionalSearchThingsRequestRequestTypeDef
 ):
     pass
 
-_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
-    {
-        "entityId": str,
-    },
-)
-_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
-    {
-        "namespaceVersion": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SearchThingsRequestSearchThingsPaginateTypeDef(
-    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
-    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
-):
-    pass
 
 ThingTypeDef = TypedDict(
     "ThingTypeDef",
     {
         "thingArn": str,
         "thingName": str,
     },
@@ -752,62 +578,58 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UploadEntityDefinitionsResponseTypeDef = TypedDict(
-    "UploadEntityDefinitionsResponseTypeDef",
-    {
-        "uploadId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowTemplateRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
     },
 )
 _OptionalCreateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
+
 class CreateFlowTemplateRequestRequestTypeDef(
     _RequiredCreateFlowTemplateRequestRequestTypeDef,
     _OptionalCreateFlowTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSystemTemplateRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
     },
 )
 _OptionalCreateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSystemTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
+
 class CreateSystemTemplateRequestRequestTypeDef(
     _RequiredCreateSystemTemplateRequestRequestTypeDef,
     _OptionalCreateSystemTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 EntityDescriptionTypeDef = TypedDict(
     "EntityDescriptionTypeDef",
     {
         "id": str,
         "arn": str,
         "type": EntityTypeType,
         "createdAt": datetime,
@@ -827,20 +649,22 @@
     "_OptionalUpdateFlowTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
+
 class UpdateFlowTemplateRequestRequestTypeDef(
     _RequiredUpdateFlowTemplateRequestRequestTypeDef,
     _OptionalUpdateFlowTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSystemTemplateRequestRequestTypeDef",
     {
         "id": str,
         "definition": DefinitionDocumentTypeDef,
     },
 )
@@ -848,71 +672,128 @@
     "_OptionalUpdateSystemTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
+
 class UpdateSystemTemplateRequestRequestTypeDef(
     _RequiredUpdateSystemTemplateRequestRequestTypeDef,
     _OptionalUpdateSystemTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 UploadEntityDefinitionsRequestRequestTypeDef = TypedDict(
     "UploadEntityDefinitionsRequestRequestTypeDef",
     {
         "document": DefinitionDocumentTypeDef,
         "syncWithPublicNamespace": bool,
         "deprecateExistingEntities": bool,
     },
     total=False,
 )
 
+FlowTemplateDescriptionTypeDef = TypedDict(
+    "FlowTemplateDescriptionTypeDef",
+    {
+        "summary": FlowTemplateSummaryTypeDef,
+        "definition": DefinitionDocumentTypeDef,
+        "validatedNamespaceVersion": int,
+    },
+    total=False,
+)
+
 CreateFlowTemplateResponseTypeDef = TypedDict(
     "CreateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FlowTemplateDescriptionTypeDef = TypedDict(
-    "FlowTemplateDescriptionTypeDef",
+DeleteNamespaceResponseTypeDef = TypedDict(
+    "DeleteNamespaceResponseTypeDef",
     {
-        "summary": FlowTemplateSummaryTypeDef,
-        "definition": DefinitionDocumentTypeDef,
-        "validatedNamespaceVersion": int,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeNamespaceResponseTypeDef = TypedDict(
+    "DescribeNamespaceResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "trackingNamespaceName": str,
+        "trackingNamespaceVersion": int,
+        "namespaceVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetFlowTemplateRevisionsResponseTypeDef = TypedDict(
     "GetFlowTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
+    "GetNamespaceDeletionStatusResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "status": NamespaceDeletionStatusType,
+        "errorCode": Literal["VALIDATION_FAILED"],
+        "errorMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUploadStatusResponseTypeDef = TypedDict(
+    "GetUploadStatusResponseTypeDef",
+    {
+        "uploadId": str,
+        "uploadStatus": UploadStatusType,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "namespaceVersion": int,
+        "failureReason": List[str],
+        "createdDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFlowTemplatesResponseTypeDef = TypedDict(
     "SearchFlowTemplatesResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowTemplateResponseTypeDef = TypedDict(
     "UpdateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadEntityDefinitionsResponseTypeDef = TypedDict(
+    "UploadEntityDefinitionsResponseTypeDef",
+    {
+        "uploadId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSystemInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSystemInstanceRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
@@ -927,26 +808,28 @@
         "s3BucketName": str,
         "metricsConfiguration": MetricsConfigurationTypeDef,
         "flowActionsRoleArn": str,
     },
     total=False,
 )
 
+
 class CreateSystemInstanceRequestRequestTypeDef(
     _RequiredCreateSystemInstanceRequestRequestTypeDef,
     _OptionalCreateSystemInstanceRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -954,67 +837,67 @@
     },
 )
 
 CreateSystemInstanceResponseTypeDef = TypedDict(
     "CreateSystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploySystemInstanceResponseTypeDef = TypedDict(
     "DeploySystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
         "greengrassDeploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchSystemInstancesResponseTypeDef = TypedDict(
     "SearchSystemInstancesResponseTypeDef",
     {
         "summaries": List[SystemInstanceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UndeploySystemInstanceResponseTypeDef = TypedDict(
     "UndeploySystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSystemTemplateResponseTypeDef = TypedDict(
     "CreateSystemTemplateResponseTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSystemTemplateRevisionsResponseTypeDef = TypedDict(
     "GetSystemTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchSystemTemplatesResponseTypeDef = TypedDict(
     "SearchSystemTemplatesResponseTypeDef",
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SystemTemplateDescriptionTypeDef = TypedDict(
     "SystemTemplateDescriptionTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
@@ -1024,15 +907,15 @@
     total=False,
 )
 
 UpdateSystemTemplateResponseTypeDef = TypedDict(
     "UpdateSystemTemplateResponseTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SystemInstanceDescriptionTypeDef = TypedDict(
     "SystemInstanceDescriptionTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
@@ -1059,93 +942,259 @@
         "nextToken": str,
         "maxResults": int,
         "namespaceVersion": int,
     },
     total=False,
 )
 
+
 class SearchEntitiesRequestRequestTypeDef(
     _RequiredSearchEntitiesRequestRequestTypeDef, _OptionalSearchEntitiesRequestRequestTypeDef
 ):
     pass
 
+
+ListFlowExecutionMessagesResponseTypeDef = TypedDict(
+    "ListFlowExecutionMessagesResponseTypeDef",
+    {
+        "messages": List[FlowExecutionMessageTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchFlowExecutionsResponseTypeDef = TypedDict(
+    "SearchFlowExecutionsResponseTypeDef",
+    {
+        "summaries": List[FlowExecutionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchFlowTemplatesRequestRequestTypeDef = TypedDict(
+    "SearchFlowTemplatesRequestRequestTypeDef",
+    {
+        "filters": Sequence[FlowTemplateFilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
+    _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
+    _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+    _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
+    "_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    {
+        "flowExecutionId": str,
+    },
+)
+_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
+    "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
+    _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+    _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "entityTypes": Sequence[EntityTypeType],
     },
 )
 _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "filters": Sequence[EntityFilterTypeDef],
         "namespaceVersion": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchEntitiesRequestSearchEntitiesPaginateTypeDef(
     _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
 ):
     pass
 
-ListFlowExecutionMessagesResponseTypeDef = TypedDict(
-    "ListFlowExecutionMessagesResponseTypeDef",
+
+SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
+    "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
     {
-        "messages": List[FlowExecutionMessageTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "filters": Sequence[FlowTemplateFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-SearchFlowExecutionsResponseTypeDef = TypedDict(
-    "SearchFlowExecutionsResponseTypeDef",
+_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
     {
-        "summaries": List[FlowExecutionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "entityId": str,
+    },
+)
+_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
+    {
+        "namespaceVersion": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-SearchFlowTemplatesRequestRequestTypeDef = TypedDict(
-    "SearchFlowTemplatesRequestRequestTypeDef",
+
+class SearchThingsRequestSearchThingsPaginateTypeDef(
+    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
+    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
+    "_RequiredSearchFlowExecutionsRequestRequestTypeDef",
     {
-        "filters": Sequence[FlowTemplateFilterTypeDef],
+        "systemInstanceId": str,
+    },
+)
+_OptionalSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
+    "_OptionalSearchFlowExecutionsRequestRequestTypeDef",
+    {
+        "flowExecutionId": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
-    "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
+
+class SearchFlowExecutionsRequestRequestTypeDef(
+    _RequiredSearchFlowExecutionsRequestRequestTypeDef,
+    _OptionalSearchFlowExecutionsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     {
-        "filters": Sequence[FlowTemplateFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "systemInstanceId": str,
+    },
+)
+_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
+    {
+        "flowExecutionId": str,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
+class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
+    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+):
+    pass
+
+
 SearchSystemInstancesRequestRequestTypeDef = TypedDict(
     "SearchSystemInstancesRequestRequestTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
 SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef = TypedDict(
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 SearchSystemTemplatesRequestRequestTypeDef = TypedDict(
     "SearchSystemTemplatesRequestRequestTypeDef",
     {
@@ -1156,61 +1205,61 @@
     total=False,
 )
 
 SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef = TypedDict(
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     {
         "filters": Sequence[SystemTemplateFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 SearchThingsResponseTypeDef = TypedDict(
     "SearchThingsResponseTypeDef",
     {
         "things": List[ThingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEntitiesResponseTypeDef = TypedDict(
     "GetEntitiesResponseTypeDef",
     {
         "descriptions": List[EntityDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchEntitiesResponseTypeDef = TypedDict(
     "SearchEntitiesResponseTypeDef",
     {
         "descriptions": List[EntityDescriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFlowTemplateResponseTypeDef = TypedDict(
     "GetFlowTemplateResponseTypeDef",
     {
         "description": FlowTemplateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSystemTemplateResponseTypeDef = TypedDict(
     "GetSystemTemplateResponseTypeDef",
     {
         "description": SystemTemplateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSystemInstanceResponseTypeDef = TypedDict(
     "GetSystemInstanceResponseTypeDef",
     {
         "description": SystemInstanceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotthingsgraph
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTThingsGraph 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTThingsGraph 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotthingsgraph type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotthingsgraph type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotthingsgraph"></a>
 
 # types-aiobotocore-iotthingsgraph
 
 [![PyPI - types-aiobotocore-iotthingsgraph](https://img.shields.io/pypi/v/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotthingsgraph.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotthingsgraph?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotthingsgraph)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotthingsgraph)](https://pepy.tech/project/types-aiobotocore-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTThingsGraph 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [types-aiobotocore-iotthingsgraph docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph/).
 
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
@@ -363,116 +362,117 @@
 )
 
 
 def check_value(value: DefinitionLanguageType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotthingsgraph.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotthingsgraph.type_defs import (
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
+    ResponseMetadataTypeDef,
     MetricsConfigurationTypeDef,
     TagTypeDef,
     SystemInstanceSummaryTypeDef,
     SystemTemplateSummaryTypeDef,
     DeleteFlowTemplateRequestRequestTypeDef,
-    DeleteNamespaceResponseTypeDef,
     DeleteSystemInstanceRequestRequestTypeDef,
     DeleteSystemTemplateRequestRequestTypeDef,
     DependencyRevisionTypeDef,
     DeploySystemInstanceRequestRequestTypeDef,
     DeprecateFlowTemplateRequestRequestTypeDef,
     DeprecateSystemTemplateRequestRequestTypeDef,
     DescribeNamespaceRequestRequestTypeDef,
-    DescribeNamespaceResponseTypeDef,
     DissociateEntityFromThingRequestRequestTypeDef,
     EntityFilterTypeDef,
     FlowExecutionMessageTypeDef,
     FlowExecutionSummaryTypeDef,
     FlowTemplateFilterTypeDef,
     GetEntitiesRequestRequestTypeDef,
     GetFlowTemplateRequestRequestTypeDef,
-    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetFlowTemplateRevisionsRequestRequestTypeDef,
-    GetNamespaceDeletionStatusResponseTypeDef,
     GetSystemInstanceRequestRequestTypeDef,
     GetSystemTemplateRequestRequestTypeDef,
-    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
-    GetUploadStatusResponseTypeDef,
-    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    SearchFlowExecutionsRequestRequestTypeDef,
-    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+    TimestampTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
-    SearchThingsRequestSearchThingsPaginateTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadEntityDefinitionsResponseTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
     CreateSystemTemplateRequestRequestTypeDef,
     EntityDescriptionTypeDef,
     UpdateFlowTemplateRequestRequestTypeDef,
     UpdateSystemTemplateRequestRequestTypeDef,
     UploadEntityDefinitionsRequestRequestTypeDef,
-    CreateFlowTemplateResponseTypeDef,
     FlowTemplateDescriptionTypeDef,
+    CreateFlowTemplateResponseTypeDef,
+    DeleteNamespaceResponseTypeDef,
+    DescribeNamespaceResponseTypeDef,
     GetFlowTemplateRevisionsResponseTypeDef,
+    GetNamespaceDeletionStatusResponseTypeDef,
+    GetUploadStatusResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
+    UploadEntityDefinitionsResponseTypeDef,
     CreateSystemInstanceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSystemInstanceResponseTypeDef,
     DeploySystemInstanceResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     CreateSystemTemplateResponseTypeDef,
     GetSystemTemplateRevisionsResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
     SystemTemplateDescriptionTypeDef,
     UpdateSystemTemplateResponseTypeDef,
     SystemInstanceDescriptionTypeDef,
     SearchEntitiesRequestRequestTypeDef,
-    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     ListFlowExecutionMessagesResponseTypeDef,
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
+    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
+    SearchThingsRequestSearchThingsPaginateTypeDef,
+    SearchFlowExecutionsRequestRequestTypeDef,
+    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
     GetFlowTemplateResponseTypeDef,
     GetSystemTemplateResponseTypeDef,
     GetSystemInstanceResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateEntityToThingRequestRequestTypeDef:
+def get_value() -> AssociateEntityToThingRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt` & `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*


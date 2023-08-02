# Comparing `tmp/types-aiobotocore-discovery-2.5.2.tar.gz` & `tmp/types-aiobotocore-discovery-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-discovery-2.5.2.tar", last modified: Sat Jul  8 01:43:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-discovery-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:10 2023, max compression
```

## Comparing `types-aiobotocore-discovery-2.5.2.tar` & `types-aiobotocore-discovery-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.922004 types-aiobotocore-discovery-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-08 01:43:30.914004 types-aiobotocore-discovery-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15861 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:30.922004 types-aiobotocore-discovery-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.914004 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24648 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24608 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25199 2023-07-08 01:28:48.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-08 01:28:48.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:47.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.914004 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-08 01:43:30.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-08 01:43:30.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:30.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:30.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:30.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:30.000000 types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:10.037606 types-aiobotocore-discovery-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-08-02 14:52:10.037606 types-aiobotocore-discovery-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15866 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:10.037606 types-aiobotocore-discovery-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:10.037606 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24585 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-08-02 14:36:27.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-08-02 14:36:27.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-08-02 14:36:27.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-08-02 14:36:27.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25203 2023-08-02 14:36:28.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25182 2023-08-02 14:36:28.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:26.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:10.037606 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-08-02 14:52:09.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:09.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:09.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:09.000000 types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-discovery-2.5.2/LICENSE` & `types-aiobotocore-discovery-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2/PKG-INFO` & `types-aiobotocore-discovery-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-discovery
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore discovery type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore discovery type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-discovery"></a>
 
 # types-aiobotocore-discovery
 
 [![PyPI - types-aiobotocore-discovery](https://img.shields.io/pypi/v/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-discovery?color=blue)](https://pypistats.org/packages/types-aiobotocore-discovery)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-discovery)](https://pepy.tech/project/types-aiobotocore-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApplicationDiscoveryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [types-aiobotocore-discovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/).
 
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
@@ -344,79 +343,80 @@
 )
 
 
 def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_discovery.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_discovery.type_defs import (
     AgentConfigurationStatusTypeDef,
     AgentNetworkInfoTypeDef,
     AssociateConfigurationItemsToApplicationRequestRequestTypeDef,
     BatchDeleteImportDataErrorTypeDef,
     BatchDeleteImportDataRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ConfigurationTagTypeDef,
     ContinuousExportDescriptionTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
     TagTypeDef,
     CustomerAgentInfoTypeDef,
     CustomerAgentlessCollectorInfoTypeDef,
     CustomerConnectorInfoTypeDef,
     CustomerMeCollectorInfoTypeDef,
     DeleteApplicationsRequestRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeConfigurationsRequestRequestTypeDef,
-    DescribeConfigurationsResponseTypeDef,
-    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
     DescribeContinuousExportsRequestRequestTypeDef,
-    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
     DescribeExportConfigurationsRequestRequestTypeDef,
     ExportInfoTypeDef,
     ExportFilterTypeDef,
     ImportTaskFilterTypeDef,
     ImportTaskTypeDef,
     TagFilterTypeDef,
     DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef,
     ReservedInstanceOptionsTypeDef,
     UsageMetricBasisTypeDef,
-    ExportConfigurationsResponseTypeDef,
     OrderByElementTypeDef,
-    ListConfigurationsResponseTypeDef,
     ListServerNeighborsRequestRequestTypeDef,
     NeighborConnectionDetailTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartContinuousExportResponseTypeDef,
     StartDataCollectionByAgentIdsRequestRequestTypeDef,
-    StartExportTaskResponseTypeDef,
+    TimestampTypeDef,
     StartImportTaskRequestRequestTypeDef,
     StopContinuousExportRequestRequestTypeDef,
-    StopContinuousExportResponseTypeDef,
     StopDataCollectionByAgentIdsRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    StartDataCollectionByAgentIdsResponseTypeDef,
-    StopDataCollectionByAgentIdsResponseTypeDef,
     AgentInfoTypeDef,
     BatchDeleteImportDataResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    DescribeConfigurationsResponseTypeDef,
+    ExportConfigurationsResponseTypeDef,
+    ListConfigurationsResponseTypeDef,
+    StartContinuousExportResponseTypeDef,
+    StartDataCollectionByAgentIdsResponseTypeDef,
+    StartExportTaskResponseTypeDef,
+    StopContinuousExportResponseTypeDef,
+    StopDataCollectionByAgentIdsResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DescribeContinuousExportsResponseTypeDef,
     CreateTagsRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     GetDiscoverySummaryResponseTypeDef,
-    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
     DescribeAgentsRequestRequestTypeDef,
+    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
+    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
+    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
     DescribeExportConfigurationsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
     DescribeExportTasksRequestRequestTypeDef,
     DescribeImportTasksRequestRequestTypeDef,
     DescribeImportTasksResponseTypeDef,
     StartImportTaskResponseTypeDef,
@@ -428,15 +428,15 @@
     ListServerNeighborsResponseTypeDef,
     DescribeAgentsResponseTypeDef,
     ExportPreferencesTypeDef,
     StartExportTaskRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AgentConfigurationStatusTypeDef:
+def get_value() -> AgentConfigurationStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-discovery-2.5.2/README.md` & `types-aiobotocore-discovery-2.5.2.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-discovery"></a>
 
 # types-aiobotocore-discovery
 
 [![PyPI - types-aiobotocore-discovery](https://img.shields.io/pypi/v/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-discovery?color=blue)](https://pypistats.org/packages/types-aiobotocore-discovery)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-discovery)](https://pepy.tech/project/types-aiobotocore-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApplicationDiscoveryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [types-aiobotocore-discovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/).
 
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
@@ -311,79 +311,80 @@
 )
 
 
 def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_discovery.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_discovery.type_defs import (
     AgentConfigurationStatusTypeDef,
     AgentNetworkInfoTypeDef,
     AssociateConfigurationItemsToApplicationRequestRequestTypeDef,
     BatchDeleteImportDataErrorTypeDef,
     BatchDeleteImportDataRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ConfigurationTagTypeDef,
     ContinuousExportDescriptionTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
     TagTypeDef,
     CustomerAgentInfoTypeDef,
     CustomerAgentlessCollectorInfoTypeDef,
     CustomerConnectorInfoTypeDef,
     CustomerMeCollectorInfoTypeDef,
     DeleteApplicationsRequestRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeConfigurationsRequestRequestTypeDef,
-    DescribeConfigurationsResponseTypeDef,
-    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
     DescribeContinuousExportsRequestRequestTypeDef,
-    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
     DescribeExportConfigurationsRequestRequestTypeDef,
     ExportInfoTypeDef,
     ExportFilterTypeDef,
     ImportTaskFilterTypeDef,
     ImportTaskTypeDef,
     TagFilterTypeDef,
     DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef,
     ReservedInstanceOptionsTypeDef,
     UsageMetricBasisTypeDef,
-    ExportConfigurationsResponseTypeDef,
     OrderByElementTypeDef,
-    ListConfigurationsResponseTypeDef,
     ListServerNeighborsRequestRequestTypeDef,
     NeighborConnectionDetailTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartContinuousExportResponseTypeDef,
     StartDataCollectionByAgentIdsRequestRequestTypeDef,
-    StartExportTaskResponseTypeDef,
+    TimestampTypeDef,
     StartImportTaskRequestRequestTypeDef,
     StopContinuousExportRequestRequestTypeDef,
-    StopContinuousExportResponseTypeDef,
     StopDataCollectionByAgentIdsRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    StartDataCollectionByAgentIdsResponseTypeDef,
-    StopDataCollectionByAgentIdsResponseTypeDef,
     AgentInfoTypeDef,
     BatchDeleteImportDataResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    DescribeConfigurationsResponseTypeDef,
+    ExportConfigurationsResponseTypeDef,
+    ListConfigurationsResponseTypeDef,
+    StartContinuousExportResponseTypeDef,
+    StartDataCollectionByAgentIdsResponseTypeDef,
+    StartExportTaskResponseTypeDef,
+    StopContinuousExportResponseTypeDef,
+    StopDataCollectionByAgentIdsResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DescribeContinuousExportsResponseTypeDef,
     CreateTagsRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     GetDiscoverySummaryResponseTypeDef,
-    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
     DescribeAgentsRequestRequestTypeDef,
+    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
+    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
+    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
     DescribeExportConfigurationsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
     DescribeExportTasksRequestRequestTypeDef,
     DescribeImportTasksRequestRequestTypeDef,
     DescribeImportTasksResponseTypeDef,
     StartImportTaskResponseTypeDef,
@@ -395,15 +396,15 @@
     ListServerNeighborsResponseTypeDef,
     DescribeAgentsResponseTypeDef,
     ExportPreferencesTypeDef,
     StartExportTaskRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AgentConfigurationStatusTypeDef:
+def get_value() -> AgentConfigurationStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-discovery-2.5.2/setup.py` & `types-aiobotocore-discovery-2.5.2.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-discovery",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_discovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with"
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
-    keywords="aiobotocore discovery type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore discovery type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_discovery": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/"
```

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/__init__.py` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/__init__.pyi` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/__main__.py` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService\nOther"
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

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/client.py` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("discovery") as client:
         client: ApplicationDiscoveryServiceClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ConfigurationItemTypeType
 from .paginator import (
     DescribeAgentsPaginator,
@@ -53,14 +52,15 @@
     StartDataCollectionByAgentIdsResponseTypeDef,
     StartExportTaskResponseTypeDef,
     StartImportTaskResponseTypeDef,
     StopContinuousExportResponseTypeDef,
     StopDataCollectionByAgentIdsResponseTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -363,16 +363,16 @@
         """
 
     async def start_export_task(
         self,
         *,
         exportDataFormat: Sequence[Literal["CSV"]] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         preferences: ExportPreferencesTypeDef = ...
     ) -> StartExportTaskResponseTypeDef:
         """
         Begins the export of a discovered data report to an Amazon S3 bucket managed by
         Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.start_export_task)
```

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/client.pyi` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("discovery") as client:
         client: ApplicationDiscoveryServiceClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ConfigurationItemTypeType
 from .paginator import (
     DescribeAgentsPaginator,
@@ -53,14 +52,15 @@
     StartDataCollectionByAgentIdsResponseTypeDef,
     StartExportTaskResponseTypeDef,
     StartImportTaskResponseTypeDef,
     StopContinuousExportResponseTypeDef,
     StopDataCollectionByAgentIdsResponseTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -335,16 +335,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/client/#start_data_collection_by_agent_ids)
         """
     async def start_export_task(
         self,
         *,
         exportDataFormat: Sequence[Literal["CSV"]] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
-        startTime: Union[datetime, str] = ...,
-        endTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
+        endTime: TimestampTypeDef = ...,
         preferences: ExportPreferencesTypeDef = ...
     ) -> StartExportTaskResponseTypeDef:
         """
         Begins the export of a discovered data report to an Amazon S3 bucket managed by
         Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.start_export_task)
```

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/literals.py` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/literals.pyi` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/paginator.py` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,45 +77,45 @@
     """
 
     def paginate(
         self,
         *,
         agentIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeAgents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeagentspaginator)
         """
 
 
 class DescribeContinuousExportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeContinuousExports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describecontinuousexportspaginator)
     """
 
     def paginate(
-        self, *, exportIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, exportIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeContinuousExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeContinuousExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describecontinuousexportspaginator)
         """
 
 
 class DescribeExportConfigurationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportConfigurations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeexportconfigurationspaginator)
     """
 
     def paginate(
-        self, *, exportIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, exportIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeExportConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeexportconfigurationspaginator)
         """
 
 
@@ -126,15 +126,15 @@
     """
 
     def paginate(
         self,
         *,
         exportIds: Sequence[str] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeexporttaskspaginator)
         """
 
 
@@ -144,15 +144,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describetagspaginator)
         """
 
 
@@ -164,13 +164,13 @@
 
     def paginate(
         self,
         *,
         configurationType: ConfigurationItemTypeType,
         filters: Sequence[FilterTypeDef] = ...,
         orderBy: Sequence[OrderByElementTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.ListConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#listconfigurationspaginator)
         """
```

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/paginator.pyi` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -74,43 +74,43 @@
     """
 
     def paginate(
         self,
         *,
         agentIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeAgents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeagentspaginator)
         """
 
 class DescribeContinuousExportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeContinuousExports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describecontinuousexportspaginator)
     """
 
     def paginate(
-        self, *, exportIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, exportIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeContinuousExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeContinuousExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describecontinuousexportspaginator)
         """
 
 class DescribeExportConfigurationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportConfigurations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeexportconfigurationspaginator)
     """
 
     def paginate(
-        self, *, exportIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, exportIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeExportConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeexportconfigurationspaginator)
         """
 
 class DescribeExportTasksPaginator(AioPaginator):
@@ -120,15 +120,15 @@
     """
 
     def paginate(
         self,
         *,
         exportIds: Sequence[str] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeexporttaskspaginator)
         """
 
 class DescribeTagsPaginator(AioPaginator):
@@ -137,15 +137,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describetagspaginator)
         """
 
 class ListConfigurationsPaginator(AioPaginator):
@@ -156,13 +156,13 @@
 
     def paginate(
         self,
         *,
         configurationType: ConfigurationItemTypeType,
         filters: Sequence[FilterTypeDef] = ...,
         orderBy: Sequence[OrderByElementTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.ListConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#listconfigurationspaginator)
         """
```

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/type_defs.py` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_discovery.type_defs import AgentConfigurationStatusTypeDef
 
-    data: AgentConfigurationStatusTypeDef = {...}
+    data: AgentConfigurationStatusTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -42,65 +42,66 @@
 
 __all__ = (
     "AgentConfigurationStatusTypeDef",
     "AgentNetworkInfoTypeDef",
     "AssociateConfigurationItemsToApplicationRequestRequestTypeDef",
     "BatchDeleteImportDataErrorTypeDef",
     "BatchDeleteImportDataRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ConfigurationTagTypeDef",
     "ContinuousExportDescriptionTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "CreateApplicationResponseTypeDef",
     "TagTypeDef",
     "CustomerAgentInfoTypeDef",
     "CustomerAgentlessCollectorInfoTypeDef",
     "CustomerConnectorInfoTypeDef",
     "CustomerMeCollectorInfoTypeDef",
     "DeleteApplicationsRequestRequestTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeConfigurationsRequestRequestTypeDef",
-    "DescribeConfigurationsResponseTypeDef",
-    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
     "DescribeContinuousExportsRequestRequestTypeDef",
-    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
     "DescribeExportConfigurationsRequestRequestTypeDef",
     "ExportInfoTypeDef",
     "ExportFilterTypeDef",
     "ImportTaskFilterTypeDef",
     "ImportTaskTypeDef",
     "TagFilterTypeDef",
     "DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef",
     "ReservedInstanceOptionsTypeDef",
     "UsageMetricBasisTypeDef",
-    "ExportConfigurationsResponseTypeDef",
     "OrderByElementTypeDef",
-    "ListConfigurationsResponseTypeDef",
     "ListServerNeighborsRequestRequestTypeDef",
     "NeighborConnectionDetailTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartContinuousExportResponseTypeDef",
     "StartDataCollectionByAgentIdsRequestRequestTypeDef",
-    "StartExportTaskResponseTypeDef",
+    "TimestampTypeDef",
     "StartImportTaskRequestRequestTypeDef",
     "StopContinuousExportRequestRequestTypeDef",
-    "StopContinuousExportResponseTypeDef",
     "StopDataCollectionByAgentIdsRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "StartDataCollectionByAgentIdsResponseTypeDef",
-    "StopDataCollectionByAgentIdsResponseTypeDef",
     "AgentInfoTypeDef",
     "BatchDeleteImportDataResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "DescribeConfigurationsResponseTypeDef",
+    "ExportConfigurationsResponseTypeDef",
+    "ListConfigurationsResponseTypeDef",
+    "StartContinuousExportResponseTypeDef",
+    "StartDataCollectionByAgentIdsResponseTypeDef",
+    "StartExportTaskResponseTypeDef",
+    "StopContinuousExportResponseTypeDef",
+    "StopDataCollectionByAgentIdsResponseTypeDef",
     "DescribeTagsResponseTypeDef",
     "DescribeContinuousExportsResponseTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "GetDiscoverySummaryResponseTypeDef",
-    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
     "DescribeAgentsRequestRequestTypeDef",
+    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
+    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
+    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
     "DescribeExportConfigurationsResponseTypeDef",
     "DescribeExportTasksResponseTypeDef",
     "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
     "DescribeExportTasksRequestRequestTypeDef",
     "DescribeImportTasksRequestRequestTypeDef",
     "DescribeImportTasksResponseTypeDef",
     "StartImportTaskResponseTypeDef",
@@ -155,14 +156,25 @@
 BatchDeleteImportDataRequestRequestTypeDef = TypedDict(
     "BatchDeleteImportDataRequestRequestTypeDef",
     {
         "importTaskIds": Sequence[str],
     },
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
 ConfigurationTagTypeDef = TypedDict(
     "ConfigurationTagTypeDef",
     {
         "configurationType": ConfigurationItemTypeType,
         "configurationId": str,
         "key": str,
         "value": str,
@@ -203,22 +215,14 @@
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "configurationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -287,57 +291,41 @@
     {
         "name": str,
         "values": Sequence[str],
         "condition": str,
     },
 )
 
-DescribeConfigurationsRequestRequestTypeDef = TypedDict(
-    "DescribeConfigurationsRequestRequestTypeDef",
-    {
-        "configurationIds": Sequence[str],
-    },
-)
-
-DescribeConfigurationsResponseTypeDef = TypedDict(
-    "DescribeConfigurationsResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "configurations": List[Dict[str, str]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef = TypedDict(
-    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
+DescribeConfigurationsRequestRequestTypeDef = TypedDict(
+    "DescribeConfigurationsRequestRequestTypeDef",
     {
-        "exportIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "configurationIds": Sequence[str],
     },
-    total=False,
 )
 
 DescribeContinuousExportsRequestRequestTypeDef = TypedDict(
     "DescribeContinuousExportsRequestRequestTypeDef",
     {
         "exportIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
-    {
-        "exportIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeExportConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeExportConfigurationsRequestRequestTypeDef",
     {
         "exportIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -437,22 +425,14 @@
     {
         "name": str,
         "percentageAdjust": float,
     },
     total=False,
 )
 
-ExportConfigurationsResponseTypeDef = TypedDict(
-    "ExportConfigurationsResponseTypeDef",
-    {
-        "exportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredOrderByElementTypeDef = TypedDict(
     "_RequiredOrderByElementTypeDef",
     {
         "fieldName": str,
     },
 )
 _OptionalOrderByElementTypeDef = TypedDict(
@@ -464,23 +444,14 @@
 )
 
 
 class OrderByElementTypeDef(_RequiredOrderByElementTypeDef, _OptionalOrderByElementTypeDef):
     pass
 
 
-ListConfigurationsResponseTypeDef = TypedDict(
-    "ListConfigurationsResponseTypeDef",
-    {
-        "configurations": List[Dict[str, str]],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListServerNeighborsRequestRequestTypeDef = TypedDict(
     "_RequiredListServerNeighborsRequestRequestTypeDef",
     {
         "configurationId": str,
     },
 )
 _OptionalListServerNeighborsRequestRequestTypeDef = TypedDict(
@@ -522,62 +493,22 @@
 
 class NeighborConnectionDetailTypeDef(
     _RequiredNeighborConnectionDetailTypeDef, _OptionalNeighborConnectionDetailTypeDef
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
-StartContinuousExportResponseTypeDef = TypedDict(
-    "StartContinuousExportResponseTypeDef",
-    {
-        "exportId": str,
-        "s3Bucket": str,
-        "startTime": datetime,
-        "dataSource": Literal["AGENT"],
-        "schemaStorageConfig": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartDataCollectionByAgentIdsRequestRequestTypeDef = TypedDict(
     "StartDataCollectionByAgentIdsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
     },
 )
 
-StartExportTaskResponseTypeDef = TypedDict(
-    "StartExportTaskResponseTypeDef",
-    {
-        "exportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredStartImportTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportTaskRequestRequestTypeDef",
     {
         "name": str,
         "importUrl": str,
     },
 )
@@ -599,23 +530,14 @@
 StopContinuousExportRequestRequestTypeDef = TypedDict(
     "StopContinuousExportRequestRequestTypeDef",
     {
         "exportId": str,
     },
 )
 
-StopContinuousExportResponseTypeDef = TypedDict(
-    "StopContinuousExportResponseTypeDef",
-    {
-        "startTime": datetime,
-        "stopTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopDataCollectionByAgentIdsRequestRequestTypeDef = TypedDict(
     "StopDataCollectionByAgentIdsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
     },
 )
 
@@ -637,30 +559,14 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-StartDataCollectionByAgentIdsResponseTypeDef = TypedDict(
-    "StartDataCollectionByAgentIdsResponseTypeDef",
-    {
-        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StopDataCollectionByAgentIdsResponseTypeDef = TypedDict(
-    "StopDataCollectionByAgentIdsResponseTypeDef",
-    {
-        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AgentInfoTypeDef = TypedDict(
     "AgentInfoTypeDef",
     {
         "agentId": str,
         "hostName": str,
         "agentNetworkInfoList": List[AgentNetworkInfoTypeDef],
         "connectorId": str,
@@ -674,33 +580,111 @@
     total=False,
 )
 
 BatchDeleteImportDataResponseTypeDef = TypedDict(
     "BatchDeleteImportDataResponseTypeDef",
     {
         "errors": List[BatchDeleteImportDataErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "configurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeConfigurationsResponseTypeDef = TypedDict(
+    "DescribeConfigurationsResponseTypeDef",
+    {
+        "configurations": List[Dict[str, str]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportConfigurationsResponseTypeDef = TypedDict(
+    "ExportConfigurationsResponseTypeDef",
+    {
+        "exportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationsResponseTypeDef = TypedDict(
+    "ListConfigurationsResponseTypeDef",
+    {
+        "configurations": List[Dict[str, str]],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartContinuousExportResponseTypeDef = TypedDict(
+    "StartContinuousExportResponseTypeDef",
+    {
+        "exportId": str,
+        "s3Bucket": str,
+        "startTime": datetime,
+        "dataSource": Literal["AGENT"],
+        "schemaStorageConfig": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDataCollectionByAgentIdsResponseTypeDef = TypedDict(
+    "StartDataCollectionByAgentIdsResponseTypeDef",
+    {
+        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartExportTaskResponseTypeDef = TypedDict(
+    "StartExportTaskResponseTypeDef",
+    {
+        "exportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopContinuousExportResponseTypeDef = TypedDict(
+    "StopContinuousExportResponseTypeDef",
+    {
+        "startTime": datetime,
+        "stopTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDataCollectionByAgentIdsResponseTypeDef = TypedDict(
+    "StopDataCollectionByAgentIdsResponseTypeDef",
+    {
+        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagsResponseTypeDef = TypedDict(
     "DescribeTagsResponseTypeDef",
     {
         "tags": List[ConfigurationTagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousExportsResponseTypeDef = TypedDict(
     "DescribeContinuousExportsResponseTypeDef",
     {
         "descriptions": List[ContinuousExportDescriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTagsRequestRequestTypeDef = TypedDict(
     "CreateTagsRequestRequestTypeDef",
     {
         "configurationIds": Sequence[str],
@@ -736,63 +720,81 @@
         "applications": int,
         "serversMappedToApplications": int,
         "serversMappedtoTags": int,
         "agentSummary": CustomerAgentInfoTypeDef,
         "connectorSummary": CustomerConnectorInfoTypeDef,
         "meCollectorSummary": CustomerMeCollectorInfoTypeDef,
         "agentlessCollectorSummary": CustomerAgentlessCollectorInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAgentsRequestDescribeAgentsPaginateTypeDef = TypedDict(
-    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
+DescribeAgentsRequestRequestTypeDef = TypedDict(
+    "DescribeAgentsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "maxResults": int,
+        "nextToken": str,
     },
     total=False,
 )
 
-DescribeAgentsRequestRequestTypeDef = TypedDict(
-    "DescribeAgentsRequestRequestTypeDef",
+DescribeAgentsRequestDescribeAgentsPaginateTypeDef = TypedDict(
+    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
     {
         "agentIds": Sequence[str],
         "filters": Sequence[FilterTypeDef],
-        "maxResults": int,
-        "nextToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef = TypedDict(
+    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
+    {
+        "exportIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
+    {
+        "exportIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeExportConfigurationsResponseTypeDef = TypedDict(
     "DescribeExportConfigurationsResponseTypeDef",
     {
         "exportsInfo": List[ExportInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportTasksResponseTypeDef = TypedDict(
     "DescribeExportTasksResponseTypeDef",
     {
         "exportsInfo": List[ExportInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = TypedDict(
     "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
     {
         "exportIds": Sequence[str],
         "filters": Sequence[ExportFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeExportTasksRequestRequestTypeDef = TypedDict(
     "DescribeExportTasksRequestRequestTypeDef",
     {
@@ -815,31 +817,31 @@
 )
 
 DescribeImportTasksResponseTypeDef = TypedDict(
     "DescribeImportTasksResponseTypeDef",
     {
         "nextToken": str,
         "tasks": List[ImportTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartImportTaskResponseTypeDef = TypedDict(
     "StartImportTaskResponseTypeDef",
     {
         "task": ImportTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
     "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     {
         "filters": Sequence[TagFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
@@ -871,15 +873,15 @@
     },
 )
 _OptionalListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
     "_OptionalListConfigurationsRequestListConfigurationsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
         "orderBy": Sequence[OrderByElementTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListConfigurationsRequestListConfigurationsPaginateTypeDef(
     _RequiredListConfigurationsRequestListConfigurationsPaginateTypeDef,
@@ -915,24 +917,24 @@
 
 ListServerNeighborsResponseTypeDef = TypedDict(
     "ListServerNeighborsResponseTypeDef",
     {
         "neighbors": List[NeighborConnectionDetailTypeDef],
         "nextToken": str,
         "knownDependencyCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAgentsResponseTypeDef = TypedDict(
     "DescribeAgentsResponseTypeDef",
     {
         "agentsInfo": List[AgentInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportPreferencesTypeDef = TypedDict(
     "ExportPreferencesTypeDef",
     {
         "ec2RecommendationsPreferences": Ec2RecommendationsExportPreferencesTypeDef,
@@ -941,13 +943,13 @@
 )
 
 StartExportTaskRequestRequestTypeDef = TypedDict(
     "StartExportTaskRequestRequestTypeDef",
     {
         "exportDataFormat": Sequence[Literal["CSV"]],
         "filters": Sequence[ExportFilterTypeDef],
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "preferences": ExportPreferencesTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery/type_defs.pyi` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_discovery.type_defs import AgentConfigurationStatusTypeDef
 
-    data: AgentConfigurationStatusTypeDef = {...}
+    data: AgentConfigurationStatusTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -41,65 +41,66 @@
 
 __all__ = (
     "AgentConfigurationStatusTypeDef",
     "AgentNetworkInfoTypeDef",
     "AssociateConfigurationItemsToApplicationRequestRequestTypeDef",
     "BatchDeleteImportDataErrorTypeDef",
     "BatchDeleteImportDataRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ConfigurationTagTypeDef",
     "ContinuousExportDescriptionTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "CreateApplicationResponseTypeDef",
     "TagTypeDef",
     "CustomerAgentInfoTypeDef",
     "CustomerAgentlessCollectorInfoTypeDef",
     "CustomerConnectorInfoTypeDef",
     "CustomerMeCollectorInfoTypeDef",
     "DeleteApplicationsRequestRequestTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeConfigurationsRequestRequestTypeDef",
-    "DescribeConfigurationsResponseTypeDef",
-    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
     "DescribeContinuousExportsRequestRequestTypeDef",
-    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
     "DescribeExportConfigurationsRequestRequestTypeDef",
     "ExportInfoTypeDef",
     "ExportFilterTypeDef",
     "ImportTaskFilterTypeDef",
     "ImportTaskTypeDef",
     "TagFilterTypeDef",
     "DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef",
     "ReservedInstanceOptionsTypeDef",
     "UsageMetricBasisTypeDef",
-    "ExportConfigurationsResponseTypeDef",
     "OrderByElementTypeDef",
-    "ListConfigurationsResponseTypeDef",
     "ListServerNeighborsRequestRequestTypeDef",
     "NeighborConnectionDetailTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartContinuousExportResponseTypeDef",
     "StartDataCollectionByAgentIdsRequestRequestTypeDef",
-    "StartExportTaskResponseTypeDef",
+    "TimestampTypeDef",
     "StartImportTaskRequestRequestTypeDef",
     "StopContinuousExportRequestRequestTypeDef",
-    "StopContinuousExportResponseTypeDef",
     "StopDataCollectionByAgentIdsRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "StartDataCollectionByAgentIdsResponseTypeDef",
-    "StopDataCollectionByAgentIdsResponseTypeDef",
     "AgentInfoTypeDef",
     "BatchDeleteImportDataResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "DescribeConfigurationsResponseTypeDef",
+    "ExportConfigurationsResponseTypeDef",
+    "ListConfigurationsResponseTypeDef",
+    "StartContinuousExportResponseTypeDef",
+    "StartDataCollectionByAgentIdsResponseTypeDef",
+    "StartExportTaskResponseTypeDef",
+    "StopContinuousExportResponseTypeDef",
+    "StopDataCollectionByAgentIdsResponseTypeDef",
     "DescribeTagsResponseTypeDef",
     "DescribeContinuousExportsResponseTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "GetDiscoverySummaryResponseTypeDef",
-    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
     "DescribeAgentsRequestRequestTypeDef",
+    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
+    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
+    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
     "DescribeExportConfigurationsResponseTypeDef",
     "DescribeExportTasksResponseTypeDef",
     "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
     "DescribeExportTasksRequestRequestTypeDef",
     "DescribeImportTasksRequestRequestTypeDef",
     "DescribeImportTasksResponseTypeDef",
     "StartImportTaskResponseTypeDef",
@@ -154,14 +155,25 @@
 BatchDeleteImportDataRequestRequestTypeDef = TypedDict(
     "BatchDeleteImportDataRequestRequestTypeDef",
     {
         "importTaskIds": Sequence[str],
     },
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
 ConfigurationTagTypeDef = TypedDict(
     "ConfigurationTagTypeDef",
     {
         "configurationType": ConfigurationItemTypeType,
         "configurationId": str,
         "key": str,
         "value": str,
@@ -200,22 +212,14 @@
 )
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "configurationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -284,57 +288,41 @@
     {
         "name": str,
         "values": Sequence[str],
         "condition": str,
     },
 )
 
-DescribeConfigurationsRequestRequestTypeDef = TypedDict(
-    "DescribeConfigurationsRequestRequestTypeDef",
-    {
-        "configurationIds": Sequence[str],
-    },
-)
-
-DescribeConfigurationsResponseTypeDef = TypedDict(
-    "DescribeConfigurationsResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "configurations": List[Dict[str, str]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef = TypedDict(
-    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
+DescribeConfigurationsRequestRequestTypeDef = TypedDict(
+    "DescribeConfigurationsRequestRequestTypeDef",
     {
-        "exportIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "configurationIds": Sequence[str],
     },
-    total=False,
 )
 
 DescribeContinuousExportsRequestRequestTypeDef = TypedDict(
     "DescribeContinuousExportsRequestRequestTypeDef",
     {
         "exportIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
-    {
-        "exportIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeExportConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeExportConfigurationsRequestRequestTypeDef",
     {
         "exportIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -432,22 +420,14 @@
     {
         "name": str,
         "percentageAdjust": float,
     },
     total=False,
 )
 
-ExportConfigurationsResponseTypeDef = TypedDict(
-    "ExportConfigurationsResponseTypeDef",
-    {
-        "exportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredOrderByElementTypeDef = TypedDict(
     "_RequiredOrderByElementTypeDef",
     {
         "fieldName": str,
     },
 )
 _OptionalOrderByElementTypeDef = TypedDict(
@@ -457,23 +437,14 @@
     },
     total=False,
 )
 
 class OrderByElementTypeDef(_RequiredOrderByElementTypeDef, _OptionalOrderByElementTypeDef):
     pass
 
-ListConfigurationsResponseTypeDef = TypedDict(
-    "ListConfigurationsResponseTypeDef",
-    {
-        "configurations": List[Dict[str, str]],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListServerNeighborsRequestRequestTypeDef = TypedDict(
     "_RequiredListServerNeighborsRequestRequestTypeDef",
     {
         "configurationId": str,
     },
 )
 _OptionalListServerNeighborsRequestRequestTypeDef = TypedDict(
@@ -511,62 +482,22 @@
 )
 
 class NeighborConnectionDetailTypeDef(
     _RequiredNeighborConnectionDetailTypeDef, _OptionalNeighborConnectionDetailTypeDef
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
-StartContinuousExportResponseTypeDef = TypedDict(
-    "StartContinuousExportResponseTypeDef",
-    {
-        "exportId": str,
-        "s3Bucket": str,
-        "startTime": datetime,
-        "dataSource": Literal["AGENT"],
-        "schemaStorageConfig": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartDataCollectionByAgentIdsRequestRequestTypeDef = TypedDict(
     "StartDataCollectionByAgentIdsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
     },
 )
 
-StartExportTaskResponseTypeDef = TypedDict(
-    "StartExportTaskResponseTypeDef",
-    {
-        "exportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredStartImportTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportTaskRequestRequestTypeDef",
     {
         "name": str,
         "importUrl": str,
     },
 )
@@ -586,23 +517,14 @@
 StopContinuousExportRequestRequestTypeDef = TypedDict(
     "StopContinuousExportRequestRequestTypeDef",
     {
         "exportId": str,
     },
 )
 
-StopContinuousExportResponseTypeDef = TypedDict(
-    "StopContinuousExportResponseTypeDef",
-    {
-        "startTime": datetime,
-        "stopTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopDataCollectionByAgentIdsRequestRequestTypeDef = TypedDict(
     "StopDataCollectionByAgentIdsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
     },
 )
 
@@ -622,30 +544,14 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-StartDataCollectionByAgentIdsResponseTypeDef = TypedDict(
-    "StartDataCollectionByAgentIdsResponseTypeDef",
-    {
-        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StopDataCollectionByAgentIdsResponseTypeDef = TypedDict(
-    "StopDataCollectionByAgentIdsResponseTypeDef",
-    {
-        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AgentInfoTypeDef = TypedDict(
     "AgentInfoTypeDef",
     {
         "agentId": str,
         "hostName": str,
         "agentNetworkInfoList": List[AgentNetworkInfoTypeDef],
         "connectorId": str,
@@ -659,33 +565,111 @@
     total=False,
 )
 
 BatchDeleteImportDataResponseTypeDef = TypedDict(
     "BatchDeleteImportDataResponseTypeDef",
     {
         "errors": List[BatchDeleteImportDataErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "configurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeConfigurationsResponseTypeDef = TypedDict(
+    "DescribeConfigurationsResponseTypeDef",
+    {
+        "configurations": List[Dict[str, str]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportConfigurationsResponseTypeDef = TypedDict(
+    "ExportConfigurationsResponseTypeDef",
+    {
+        "exportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationsResponseTypeDef = TypedDict(
+    "ListConfigurationsResponseTypeDef",
+    {
+        "configurations": List[Dict[str, str]],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartContinuousExportResponseTypeDef = TypedDict(
+    "StartContinuousExportResponseTypeDef",
+    {
+        "exportId": str,
+        "s3Bucket": str,
+        "startTime": datetime,
+        "dataSource": Literal["AGENT"],
+        "schemaStorageConfig": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDataCollectionByAgentIdsResponseTypeDef = TypedDict(
+    "StartDataCollectionByAgentIdsResponseTypeDef",
+    {
+        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartExportTaskResponseTypeDef = TypedDict(
+    "StartExportTaskResponseTypeDef",
+    {
+        "exportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopContinuousExportResponseTypeDef = TypedDict(
+    "StopContinuousExportResponseTypeDef",
+    {
+        "startTime": datetime,
+        "stopTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDataCollectionByAgentIdsResponseTypeDef = TypedDict(
+    "StopDataCollectionByAgentIdsResponseTypeDef",
+    {
+        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagsResponseTypeDef = TypedDict(
     "DescribeTagsResponseTypeDef",
     {
         "tags": List[ConfigurationTagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousExportsResponseTypeDef = TypedDict(
     "DescribeContinuousExportsResponseTypeDef",
     {
         "descriptions": List[ContinuousExportDescriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTagsRequestRequestTypeDef = TypedDict(
     "CreateTagsRequestRequestTypeDef",
     {
         "configurationIds": Sequence[str],
@@ -719,63 +703,81 @@
         "applications": int,
         "serversMappedToApplications": int,
         "serversMappedtoTags": int,
         "agentSummary": CustomerAgentInfoTypeDef,
         "connectorSummary": CustomerConnectorInfoTypeDef,
         "meCollectorSummary": CustomerMeCollectorInfoTypeDef,
         "agentlessCollectorSummary": CustomerAgentlessCollectorInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAgentsRequestDescribeAgentsPaginateTypeDef = TypedDict(
-    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
+DescribeAgentsRequestRequestTypeDef = TypedDict(
+    "DescribeAgentsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "maxResults": int,
+        "nextToken": str,
     },
     total=False,
 )
 
-DescribeAgentsRequestRequestTypeDef = TypedDict(
-    "DescribeAgentsRequestRequestTypeDef",
+DescribeAgentsRequestDescribeAgentsPaginateTypeDef = TypedDict(
+    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
     {
         "agentIds": Sequence[str],
         "filters": Sequence[FilterTypeDef],
-        "maxResults": int,
-        "nextToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef = TypedDict(
+    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
+    {
+        "exportIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
+    {
+        "exportIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeExportConfigurationsResponseTypeDef = TypedDict(
     "DescribeExportConfigurationsResponseTypeDef",
     {
         "exportsInfo": List[ExportInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportTasksResponseTypeDef = TypedDict(
     "DescribeExportTasksResponseTypeDef",
     {
         "exportsInfo": List[ExportInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = TypedDict(
     "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
     {
         "exportIds": Sequence[str],
         "filters": Sequence[ExportFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeExportTasksRequestRequestTypeDef = TypedDict(
     "DescribeExportTasksRequestRequestTypeDef",
     {
@@ -798,31 +800,31 @@
 )
 
 DescribeImportTasksResponseTypeDef = TypedDict(
     "DescribeImportTasksResponseTypeDef",
     {
         "nextToken": str,
         "tasks": List[ImportTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartImportTaskResponseTypeDef = TypedDict(
     "StartImportTaskResponseTypeDef",
     {
         "task": ImportTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
     "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     {
         "filters": Sequence[TagFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
@@ -854,15 +856,15 @@
     },
 )
 _OptionalListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
     "_OptionalListConfigurationsRequestListConfigurationsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
         "orderBy": Sequence[OrderByElementTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListConfigurationsRequestListConfigurationsPaginateTypeDef(
     _RequiredListConfigurationsRequestListConfigurationsPaginateTypeDef,
     _OptionalListConfigurationsRequestListConfigurationsPaginateTypeDef,
@@ -894,24 +896,24 @@
 
 ListServerNeighborsResponseTypeDef = TypedDict(
     "ListServerNeighborsResponseTypeDef",
     {
         "neighbors": List[NeighborConnectionDetailTypeDef],
         "nextToken": str,
         "knownDependencyCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAgentsResponseTypeDef = TypedDict(
     "DescribeAgentsResponseTypeDef",
     {
         "agentsInfo": List[AgentInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportPreferencesTypeDef = TypedDict(
     "ExportPreferencesTypeDef",
     {
         "ec2RecommendationsPreferences": Ec2RecommendationsExportPreferencesTypeDef,
@@ -920,13 +922,13 @@
 )
 
 StartExportTaskRequestRequestTypeDef = TypedDict(
     "StartExportTaskRequestRequestTypeDef",
     {
         "exportDataFormat": Sequence[Literal["CSV"]],
         "filters": Sequence[ExportFilterTypeDef],
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
         "preferences": ExportPreferencesTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery.egg-info/PKG-INFO` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-discovery
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore discovery type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore discovery type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-discovery"></a>
 
 # types-aiobotocore-discovery
 
 [![PyPI - types-aiobotocore-discovery](https://img.shields.io/pypi/v/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-discovery?color=blue)](https://pypistats.org/packages/types-aiobotocore-discovery)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-discovery)](https://pepy.tech/project/types-aiobotocore-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApplicationDiscoveryService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [types-aiobotocore-discovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/).
 
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
@@ -344,79 +343,80 @@
 )
 
 
 def check_value(value: AgentStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_discovery.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_discovery.type_defs import (
     AgentConfigurationStatusTypeDef,
     AgentNetworkInfoTypeDef,
     AssociateConfigurationItemsToApplicationRequestRequestTypeDef,
     BatchDeleteImportDataErrorTypeDef,
     BatchDeleteImportDataRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ConfigurationTagTypeDef,
     ContinuousExportDescriptionTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
     TagTypeDef,
     CustomerAgentInfoTypeDef,
     CustomerAgentlessCollectorInfoTypeDef,
     CustomerConnectorInfoTypeDef,
     CustomerMeCollectorInfoTypeDef,
     DeleteApplicationsRequestRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeConfigurationsRequestRequestTypeDef,
-    DescribeConfigurationsResponseTypeDef,
-    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
     DescribeContinuousExportsRequestRequestTypeDef,
-    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
     DescribeExportConfigurationsRequestRequestTypeDef,
     ExportInfoTypeDef,
     ExportFilterTypeDef,
     ImportTaskFilterTypeDef,
     ImportTaskTypeDef,
     TagFilterTypeDef,
     DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef,
     ReservedInstanceOptionsTypeDef,
     UsageMetricBasisTypeDef,
-    ExportConfigurationsResponseTypeDef,
     OrderByElementTypeDef,
-    ListConfigurationsResponseTypeDef,
     ListServerNeighborsRequestRequestTypeDef,
     NeighborConnectionDetailTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartContinuousExportResponseTypeDef,
     StartDataCollectionByAgentIdsRequestRequestTypeDef,
-    StartExportTaskResponseTypeDef,
+    TimestampTypeDef,
     StartImportTaskRequestRequestTypeDef,
     StopContinuousExportRequestRequestTypeDef,
-    StopContinuousExportResponseTypeDef,
     StopDataCollectionByAgentIdsRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    StartDataCollectionByAgentIdsResponseTypeDef,
-    StopDataCollectionByAgentIdsResponseTypeDef,
     AgentInfoTypeDef,
     BatchDeleteImportDataResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    DescribeConfigurationsResponseTypeDef,
+    ExportConfigurationsResponseTypeDef,
+    ListConfigurationsResponseTypeDef,
+    StartContinuousExportResponseTypeDef,
+    StartDataCollectionByAgentIdsResponseTypeDef,
+    StartExportTaskResponseTypeDef,
+    StopContinuousExportResponseTypeDef,
+    StopDataCollectionByAgentIdsResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DescribeContinuousExportsResponseTypeDef,
     CreateTagsRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     GetDiscoverySummaryResponseTypeDef,
-    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
     DescribeAgentsRequestRequestTypeDef,
+    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
+    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
+    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
     DescribeExportConfigurationsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
     DescribeExportTasksRequestRequestTypeDef,
     DescribeImportTasksRequestRequestTypeDef,
     DescribeImportTasksResponseTypeDef,
     StartImportTaskResponseTypeDef,
@@ -428,15 +428,15 @@
     ListServerNeighborsResponseTypeDef,
     DescribeAgentsResponseTypeDef,
     ExportPreferencesTypeDef,
     StartExportTaskRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AgentConfigurationStatusTypeDef:
+def get_value() -> AgentConfigurationStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-discovery-2.5.2/types_aiobotocore_discovery.egg-info/SOURCES.txt` & `types-aiobotocore-discovery-2.5.2.post1/types_aiobotocore_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*


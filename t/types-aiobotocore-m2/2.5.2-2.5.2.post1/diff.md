# Comparing `tmp/types-aiobotocore-m2-2.5.2.tar.gz` & `tmp/types-aiobotocore-m2-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-m2-2.5.2.tar", last modified: Sat Jul  8 01:43:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-m2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:35 2023, max compression
```

## Comparing `types-aiobotocore-m2-2.5.2.tar` & `types-aiobotocore-m2-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.822474 types-aiobotocore-m2-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18881 2023-07-08 01:43:55.822474 types-aiobotocore-m2-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17316 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:55.822474 types-aiobotocore-m2-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-08 01:34:25.000000 types-aiobotocore-m2-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.810474 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29334 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29284 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42341 2023-07-08 01:34:28.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42273 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:26.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.822474 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18881 2023-07-08 01:43:55.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-08 01:43:55.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:55.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 01:43:55.000000 types-aiobotocore-m2-2.5.2/types_aiobotocore_m2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.973533 types-aiobotocore-m2-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-08-02 14:52:35.969533 types-aiobotocore-m2-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:35.973533 types-aiobotocore-m2-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.961533 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29311 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29261 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42321 2023-08-02 14:42:39.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42253 2023-08-02 14:42:39.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.969533 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-08-02 14:52:35.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 14:52:35.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:35.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 14:52:35.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-m2-2.5.2/LICENSE` & `types-aiobotocore-m2-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2/PKG-INFO` & `types-aiobotocore-m2-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-m2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.MainframeModernization 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.MainframeModernization 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore m2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore m2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-m2"></a>
 
 # types-aiobotocore-m2
 
 [![PyPI - types-aiobotocore-m2](https://img.shields.io/pypi/v/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-m2?color=blue)](https://pypistats.org/packages/types-aiobotocore-m2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-m2)](https://pepy.tech/project/types-aiobotocore-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MainframeModernization 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [types-aiobotocore-m2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/).
 
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
@@ -353,38 +352,35 @@
 )
 
 
 def check_value(value: ApplicationDeploymentLifecycleType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_m2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_m2.type_defs import (
     AlternateKeyTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateDataSetImportTaskResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
     HighAvailabilityConfigTypeDef,
-    CreateEnvironmentResponseTypeDef,
     ExternalLocationTypeDef,
     DataSetImportSummaryTypeDef,
     DataSetSummaryTypeDef,
     RecordLengthTypeDef,
     GdgDetailAttributesTypeDef,
     PoDetailAttributesTypeDef,
     PsDetailAttributesTypeDef,
@@ -399,67 +395,71 @@
     EfsStorageConfigurationTypeDef,
     EngineVersionsSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     FsxStorageConfigurationTypeDef,
     GetApplicationRequestRequestTypeDef,
     LogGroupSummaryTypeDef,
     GetApplicationVersionRequestRequestTypeDef,
-    GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionRequestRequestTypeDef,
     GetDataSetDetailsRequestRequestTypeDef,
     GetDataSetImportTaskRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetDeploymentResponseTypeDef,
     GetEnvironmentRequestRequestTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     ListBatchJobDefinitionsRequestRequestTypeDef,
-    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    ListBatchJobExecutionsRequestRequestTypeDef,
-    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+    TimestampTypeDef,
     ListDataSetImportHistoryRequestRequestTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
-    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
     ListEngineVersionsRequestRequestTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MaintenanceScheduleTypeDef,
-    PaginatorConfigTypeDef,
     PrimaryKeyTypeDef,
-    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
-    StartBatchJobResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateApplicationResponseTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
-    UpdateEnvironmentResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListApplicationVersionsResponseTypeDef,
     BatchJobDefinitionTypeDef,
     BatchJobIdentifierTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    CreateApplicationResponseTypeDef,
+    CreateDataSetImportTaskResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateEnvironmentResponseTypeDef,
+    GetApplicationVersionResponseTypeDef,
+    GetDeploymentResponseTypeDef,
+    ListApplicationVersionsResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartBatchJobResponseTypeDef,
+    UpdateApplicationResponseTypeDef,
+    UpdateEnvironmentResponseTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     StorageConfigurationTypeDef,
     GetApplicationResponseTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
+    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+    ListBatchJobExecutionsRequestRequestTypeDef,
     PendingMaintenanceTypeDef,
     VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     BatchJobExecutionSummaryTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
@@ -473,15 +473,15 @@
     GetDataSetDetailsResponseTypeDef,
     DataSetImportItemTypeDef,
     DataSetImportConfigTypeDef,
     CreateDataSetImportTaskRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AlternateKeyTypeDef:
+def get_value() -> AlternateKeyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-m2-2.5.2/README.md` & `types-aiobotocore-m2-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-m2"></a>
 
 # types-aiobotocore-m2
 
 [![PyPI - types-aiobotocore-m2](https://img.shields.io/pypi/v/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-m2?color=blue)](https://pypistats.org/packages/types-aiobotocore-m2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-m2)](https://pepy.tech/project/types-aiobotocore-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MainframeModernization 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [types-aiobotocore-m2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/).
 
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
@@ -320,38 +320,35 @@
 )
 
 
 def check_value(value: ApplicationDeploymentLifecycleType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_m2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_m2.type_defs import (
     AlternateKeyTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateDataSetImportTaskResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
     HighAvailabilityConfigTypeDef,
-    CreateEnvironmentResponseTypeDef,
     ExternalLocationTypeDef,
     DataSetImportSummaryTypeDef,
     DataSetSummaryTypeDef,
     RecordLengthTypeDef,
     GdgDetailAttributesTypeDef,
     PoDetailAttributesTypeDef,
     PsDetailAttributesTypeDef,
@@ -366,67 +363,71 @@
     EfsStorageConfigurationTypeDef,
     EngineVersionsSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     FsxStorageConfigurationTypeDef,
     GetApplicationRequestRequestTypeDef,
     LogGroupSummaryTypeDef,
     GetApplicationVersionRequestRequestTypeDef,
-    GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionRequestRequestTypeDef,
     GetDataSetDetailsRequestRequestTypeDef,
     GetDataSetImportTaskRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetDeploymentResponseTypeDef,
     GetEnvironmentRequestRequestTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     ListBatchJobDefinitionsRequestRequestTypeDef,
-    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    ListBatchJobExecutionsRequestRequestTypeDef,
-    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+    TimestampTypeDef,
     ListDataSetImportHistoryRequestRequestTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
-    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
     ListEngineVersionsRequestRequestTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MaintenanceScheduleTypeDef,
-    PaginatorConfigTypeDef,
     PrimaryKeyTypeDef,
-    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
-    StartBatchJobResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateApplicationResponseTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
-    UpdateEnvironmentResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListApplicationVersionsResponseTypeDef,
     BatchJobDefinitionTypeDef,
     BatchJobIdentifierTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    CreateApplicationResponseTypeDef,
+    CreateDataSetImportTaskResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateEnvironmentResponseTypeDef,
+    GetApplicationVersionResponseTypeDef,
+    GetDeploymentResponseTypeDef,
+    ListApplicationVersionsResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartBatchJobResponseTypeDef,
+    UpdateApplicationResponseTypeDef,
+    UpdateEnvironmentResponseTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     StorageConfigurationTypeDef,
     GetApplicationResponseTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
+    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+    ListBatchJobExecutionsRequestRequestTypeDef,
     PendingMaintenanceTypeDef,
     VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     BatchJobExecutionSummaryTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
@@ -440,15 +441,15 @@
     GetDataSetDetailsResponseTypeDef,
     DataSetImportItemTypeDef,
     DataSetImportConfigTypeDef,
     CreateDataSetImportTaskRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AlternateKeyTypeDef:
+def get_value() -> AlternateKeyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-m2-2.5.2/setup.py` & `types-aiobotocore-m2-2.5.2.post1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-m2",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_m2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MainframeModernization 2.5.2 service generated with"
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
-    keywords="aiobotocore m2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore m2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_m2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/__init__.py` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/__init__.pyi` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/__main__.py` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.MainframeModernization 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization\nOther"
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

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/client.py` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("m2") as client:
         client: MainframeModernizationClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import BatchJobExecutionStatusType, EngineTypeType
 from .paginator import (
     ListApplicationsPaginator,
@@ -57,14 +56,15 @@
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartBatchJobResponseTypeDef,
     StorageConfigurationTypeDef,
+    TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -358,16 +358,16 @@
         self,
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        startedAfter: Union[datetime, str] = ...,
-        startedBefore: Union[datetime, str] = ...,
+        startedAfter: TimestampTypeDef = ...,
+        startedBefore: TimestampTypeDef = ...,
         status: BatchJobExecutionStatusType = ...
     ) -> ListBatchJobExecutionsResponseTypeDef:
         """
         Lists historical, current, and scheduled batch job executions for a specific
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_executions)
```

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/client.pyi` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("m2") as client:
         client: MainframeModernizationClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import BatchJobExecutionStatusType, EngineTypeType
 from .paginator import (
     ListApplicationsPaginator,
@@ -57,14 +56,15 @@
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     StartBatchJobResponseTypeDef,
     StorageConfigurationTypeDef,
+    TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -332,16 +332,16 @@
         self,
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        startedAfter: Union[datetime, str] = ...,
-        startedBefore: Union[datetime, str] = ...,
+        startedAfter: TimestampTypeDef = ...,
+        startedBefore: TimestampTypeDef = ...,
         status: BatchJobExecutionStatusType = ...
     ) -> ListBatchJobExecutionsResponseTypeDef:
         """
         Lists historical, current, and scheduled batch job executions for a specific
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_batch_job_executions)
```

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/literals.py` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/literals.pyi` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/paginator.py` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,15 @@
         list_data_set_import_history_paginator: ListDataSetImportHistoryPaginator = client.get_paginator("list_data_set_import_history")
         list_data_sets_paginator: ListDataSetsPaginator = client.get_paginator("list_data_sets")
         list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
         list_engine_versions_paginator: ListEngineVersionsPaginator = client.get_paginator("list_engine_versions")
         list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import BatchJobExecutionStatusType, EngineTypeType
 from .type_defs import (
     ListApplicationsResponseTypeDef,
@@ -50,14 +49,15 @@
     ListBatchJobExecutionsResponseTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListApplicationVersionsPaginator",
     "ListApplicationsPaginator",
     "ListBatchJobDefinitionsPaginator",
     "ListBatchJobExecutionsPaginator",
@@ -82,15 +82,15 @@
 class ListApplicationVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listapplicationversionspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listapplicationversionspaginator)
         """
 
 
@@ -101,15 +101,15 @@
     """
 
     def paginate(
         self,
         *,
         environmentId: str = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listapplicationspaginator)
         """
 
 
@@ -120,15 +120,15 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBatchJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listbatchjobdefinitionspaginator)
         """
 
 
@@ -140,33 +140,33 @@
 
     def paginate(
         self,
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
-        startedAfter: Union[datetime, str] = ...,
-        startedBefore: Union[datetime, str] = ...,
+        startedAfter: TimestampTypeDef = ...,
+        startedBefore: TimestampTypeDef = ...,
         status: BatchJobExecutionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBatchJobExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listbatchjobexecutionspaginator)
         """
 
 
 class ListDataSetImportHistoryPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listdatasetimporthistorypaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataSetImportHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listdatasetimporthistorypaginator)
         """
 
 
@@ -177,45 +177,45 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listdatasetspaginator)
         """
 
 
 class ListDeploymentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listdeploymentspaginator)
         """
 
 
 class ListEngineVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listengineversionspaginator)
     """
 
     def paginate(
-        self, *, engineType: EngineTypeType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, engineType: EngineTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEngineVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listengineversionspaginator)
         """
 
 
@@ -226,13 +226,13 @@
     """
 
     def paginate(
         self,
         *,
         engineType: EngineTypeType = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listenvironmentspaginator)
         """
```

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/paginator.pyi` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,15 @@
         list_data_set_import_history_paginator: ListDataSetImportHistoryPaginator = client.get_paginator("list_data_set_import_history")
         list_data_sets_paginator: ListDataSetsPaginator = client.get_paginator("list_data_sets")
         list_deployments_paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")
         list_engine_versions_paginator: ListEngineVersionsPaginator = client.get_paginator("list_engine_versions")
         list_environments_paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import BatchJobExecutionStatusType, EngineTypeType
 from .type_defs import (
     ListApplicationsResponseTypeDef,
@@ -50,14 +49,15 @@
     ListBatchJobExecutionsResponseTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "ListApplicationVersionsPaginator",
     "ListApplicationsPaginator",
     "ListBatchJobDefinitionsPaginator",
     "ListBatchJobExecutionsPaginator",
@@ -79,15 +79,15 @@
 class ListApplicationVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listapplicationversionspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplicationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listapplicationversionspaginator)
         """
 
 class ListApplicationsPaginator(AioPaginator):
@@ -97,15 +97,15 @@
     """
 
     def paginate(
         self,
         *,
         environmentId: str = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listapplicationspaginator)
         """
 
 class ListBatchJobDefinitionsPaginator(AioPaginator):
@@ -115,15 +115,15 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBatchJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listbatchjobdefinitionspaginator)
         """
 
 class ListBatchJobExecutionsPaginator(AioPaginator):
@@ -134,32 +134,32 @@
 
     def paginate(
         self,
         *,
         applicationId: str,
         executionIds: Sequence[str] = ...,
         jobName: str = ...,
-        startedAfter: Union[datetime, str] = ...,
-        startedBefore: Union[datetime, str] = ...,
+        startedAfter: TimestampTypeDef = ...,
+        startedBefore: TimestampTypeDef = ...,
         status: BatchJobExecutionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListBatchJobExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListBatchJobExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listbatchjobexecutionspaginator)
         """
 
 class ListDataSetImportHistoryPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listdatasetimporthistorypaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataSetImportHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSetImportHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listdatasetimporthistorypaginator)
         """
 
 class ListDataSetsPaginator(AioPaginator):
@@ -169,43 +169,43 @@
     """
 
     def paginate(
         self,
         *,
         applicationId: str,
         prefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDataSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listdatasetspaginator)
         """
 
 class ListDeploymentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
-        self, *, applicationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, applicationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listdeploymentspaginator)
         """
 
 class ListEngineVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listengineversionspaginator)
     """
 
     def paginate(
-        self, *, engineType: EngineTypeType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, engineType: EngineTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEngineVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listengineversionspaginator)
         """
 
 class ListEnvironmentsPaginator(AioPaginator):
@@ -215,13 +215,13 @@
     """
 
     def paginate(
         self,
         *,
         engineType: EngineTypeType = ...,
         names: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Paginator.ListEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/paginators/#listenvironmentspaginator)
         """
```

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/type_defs.py` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_m2.type_defs import AlternateKeyTypeDef
 
-    data: AlternateKeyTypeDef = {...}
+    data: AlternateKeyTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -39,20 +39,17 @@
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
     "FileBatchJobIdentifierTypeDef",
     "ScriptBatchJobIdentifierTypeDef",
     "CancelBatchJobExecutionRequestRequestTypeDef",
     "DefinitionTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "CreateDataSetImportTaskResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "CreateDeploymentResponseTypeDef",
     "HighAvailabilityConfigTypeDef",
-    "CreateEnvironmentResponseTypeDef",
     "ExternalLocationTypeDef",
     "DataSetImportSummaryTypeDef",
     "DataSetSummaryTypeDef",
     "RecordLengthTypeDef",
     "GdgDetailAttributesTypeDef",
     "PoDetailAttributesTypeDef",
     "PsDetailAttributesTypeDef",
@@ -67,67 +64,71 @@
     "EfsStorageConfigurationTypeDef",
     "EngineVersionsSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "FsxStorageConfigurationTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "LogGroupSummaryTypeDef",
     "GetApplicationVersionRequestRequestTypeDef",
-    "GetApplicationVersionResponseTypeDef",
     "GetBatchJobExecutionRequestRequestTypeDef",
     "GetDataSetDetailsRequestRequestTypeDef",
     "GetDataSetImportTaskRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
-    "GetDeploymentResponseTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
-    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
     "ListBatchJobDefinitionsRequestRequestTypeDef",
-    "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    "ListBatchJobExecutionsRequestRequestTypeDef",
-    "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    "TimestampTypeDef",
     "ListDataSetImportHistoryRequestRequestTypeDef",
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDataSetsRequestRequestTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
-    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
     "ListEngineVersionsRequestRequestTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MaintenanceScheduleTypeDef",
-    "PaginatorConfigTypeDef",
     "PrimaryKeyTypeDef",
-    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
-    "StartBatchJobResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateApplicationResponseTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
-    "UpdateEnvironmentResponseTypeDef",
-    "ListApplicationsResponseTypeDef",
-    "ListApplicationVersionsResponseTypeDef",
     "BatchJobDefinitionTypeDef",
     "BatchJobIdentifierTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "CreateDataSetImportTaskResponseTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "CreateEnvironmentResponseTypeDef",
+    "GetApplicationVersionResponseTypeDef",
+    "GetDeploymentResponseTypeDef",
+    "ListApplicationVersionsResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartBatchJobResponseTypeDef",
+    "UpdateApplicationResponseTypeDef",
+    "UpdateEnvironmentResponseTypeDef",
     "DataSetImportTaskTypeDef",
     "GetDataSetImportTaskResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
     "ListEngineVersionsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "StorageConfigurationTypeDef",
     "GetApplicationResponseTypeDef",
+    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    "ListBatchJobExecutionsRequestRequestTypeDef",
     "PendingMaintenanceTypeDef",
     "VsamAttributesTypeDef",
     "VsamDetailAttributesTypeDef",
     "ListBatchJobDefinitionsResponseTypeDef",
     "BatchJobExecutionSummaryTypeDef",
     "GetBatchJobExecutionResponseTypeDef",
     "StartBatchJobRequestRequestTypeDef",
@@ -289,29 +290,22 @@
     {
         "content": str,
         "s3Location": str,
     },
     total=False,
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "applicationArn": str,
-        "applicationId": str,
-        "applicationVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDataSetImportTaskResponseTypeDef = TypedDict(
-    "CreateDataSetImportTaskResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -330,37 +324,21 @@
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "deploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 HighAvailabilityConfigTypeDef = TypedDict(
     "HighAvailabilityConfigTypeDef",
     {
         "desiredCapacity": int,
     },
 )
 
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExternalLocationTypeDef = TypedDict(
     "ExternalLocationTypeDef",
     {
         "s3Location": str,
     },
     total=False,
 )
@@ -607,28 +585,14 @@
     "GetApplicationVersionRequestRequestTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
     },
 )
 
-GetApplicationVersionResponseTypeDef = TypedDict(
-    "GetApplicationVersionResponseTypeDef",
-    {
-        "applicationVersion": int,
-        "creationTime": datetime,
-        "definitionContent": str,
-        "description": str,
-        "name": str,
-        "status": ApplicationVersionLifecycleType,
-        "statusReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBatchJobExecutionRequestRequestTypeDef = TypedDict(
     "GetBatchJobExecutionRequestRequestTypeDef",
     {
         "applicationId": str,
         "executionId": str,
     },
 )
@@ -653,57 +617,31 @@
     "GetDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
         "deploymentId": str,
     },
 )
 
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "applicationId": str,
-        "applicationVersion": int,
-        "creationTime": datetime,
-        "deploymentId": str,
-        "environmentId": str,
-        "status": DeploymentLifecycleType,
-        "statusReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
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
-class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
-    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -719,58 +657,25 @@
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "environmentId": str,
-        "names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "environmentId": str,
         "maxResults": int,
         "names": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
-    "_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
-    "_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    {
-        "prefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
-    _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-    _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBatchJobDefinitionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
@@ -787,91 +692,15 @@
 class ListBatchJobDefinitionsRequestRequestTypeDef(
     _RequiredListBatchJobDefinitionsRequestRequestTypeDef,
     _OptionalListBatchJobDefinitionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    {
-        "executionIds": Sequence[str],
-        "jobName": str,
-        "startedAfter": Union[datetime, str],
-        "startedBefore": Union[datetime, str],
-        "status": BatchJobExecutionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
-    _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
-    "_RequiredListBatchJobExecutionsRequestRequestTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
-    "_OptionalListBatchJobExecutionsRequestRequestTypeDef",
-    {
-        "executionIds": Sequence[str],
-        "jobName": str,
-        "maxResults": int,
-        "nextToken": str,
-        "startedAfter": Union[datetime, str],
-        "startedBefore": Union[datetime, str],
-        "status": BatchJobExecutionStatusType,
-    },
-    total=False,
-)
-
-
-class ListBatchJobExecutionsRequestRequestTypeDef(
-    _RequiredListBatchJobExecutionsRequestRequestTypeDef,
-    _OptionalListBatchJobExecutionsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
-    _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-    _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetImportHistoryRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
@@ -887,37 +716,14 @@
 class ListDataSetImportHistoryRequestRequestTypeDef(
     _RequiredListDataSetImportHistoryRequestRequestTypeDef,
     _OptionalListDataSetImportHistoryRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "prefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDataSetsRequestListDataSetsPaginateTypeDef(
-    _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
-    _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDataSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetsRequestRequestTypeDef = TypedDict(
@@ -933,36 +739,14 @@
 
 class ListDataSetsRequestRequestTypeDef(
     _RequiredListDataSetsRequestRequestTypeDef, _OptionalListDataSetsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
-    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDeploymentsRequestRequestTypeDef = TypedDict(
@@ -977,43 +761,24 @@
 
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
 
-ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
-    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
-    {
-        "engineType": EngineTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEngineVersionsRequestRequestTypeDef = TypedDict(
     "ListEngineVersionsRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "engineType": EngineTypeType,
-        "names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
         "maxResults": int,
         "names": Sequence[str],
         "nextToken": str,
@@ -1024,41 +789,23 @@
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
 MaintenanceScheduleTypeDef = TypedDict(
     "MaintenanceScheduleTypeDef",
     {
         "endTime": datetime,
         "startTime": datetime,
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
 _RequiredPrimaryKeyTypeDef = TypedDict(
     "_RequiredPrimaryKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -1071,40 +818,21 @@
 )
 
 
 class PrimaryKeyTypeDef(_RequiredPrimaryKeyTypeDef, _OptionalPrimaryKeyTypeDef):
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
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
-StartBatchJobResponseTypeDef = TypedDict(
-    "StartBatchJobResponseTypeDef",
-    {
-        "executionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredStopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalStopApplicationRequestRequestTypeDef = TypedDict(
@@ -1134,22 +862,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateApplicationResponseTypeDef = TypedDict(
-    "UpdateApplicationResponseTypeDef",
-    {
-        "applicationVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -1167,40 +887,14 @@
 
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
 
-UpdateEnvironmentResponseTypeDef = TypedDict(
-    "UpdateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListApplicationsResponseTypeDef = TypedDict(
-    "ListApplicationsResponseTypeDef",
-    {
-        "applications": List[ApplicationSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListApplicationVersionsResponseTypeDef = TypedDict(
-    "ListApplicationVersionsResponseTypeDef",
-    {
-        "applicationVersions": List[ApplicationVersionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchJobDefinitionTypeDef = TypedDict(
     "BatchJobDefinitionTypeDef",
     {
         "fileBatchJobDefinition": FileBatchJobDefinitionTypeDef,
         "scriptBatchJobDefinition": ScriptBatchJobDefinitionTypeDef,
     },
     total=False,
@@ -1261,14 +955,126 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationArn": str,
+        "applicationId": str,
+        "applicationVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataSetImportTaskResponseTypeDef = TypedDict(
+    "CreateDataSetImportTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "deploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApplicationVersionResponseTypeDef = TypedDict(
+    "GetApplicationVersionResponseTypeDef",
+    {
+        "applicationVersion": int,
+        "creationTime": datetime,
+        "definitionContent": str,
+        "description": str,
+        "name": str,
+        "status": ApplicationVersionLifecycleType,
+        "statusReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "applicationId": str,
+        "applicationVersion": int,
+        "creationTime": datetime,
+        "deploymentId": str,
+        "environmentId": str,
+        "status": DeploymentLifecycleType,
+        "statusReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationVersionsResponseTypeDef = TypedDict(
+    "ListApplicationVersionsResponseTypeDef",
+    {
+        "applicationVersions": List[ApplicationVersionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsResponseTypeDef = TypedDict(
+    "ListApplicationsResponseTypeDef",
+    {
+        "applications": List[ApplicationSummaryTypeDef],
+        "nextToken": str,
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
+StartBatchJobResponseTypeDef = TypedDict(
+    "StartBatchJobResponseTypeDef",
+    {
+        "executionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationResponseTypeDef = TypedDict(
+    "UpdateApplicationResponseTypeDef",
+    {
+        "applicationVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEnvironmentResponseTypeDef = TypedDict(
+    "UpdateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DataSetImportTaskTypeDef = TypedDict(
     "DataSetImportTaskTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
     },
@@ -1276,51 +1082,51 @@
 
 GetDataSetImportTaskResponseTypeDef = TypedDict(
     "GetDataSetImportTaskResponseTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "dataSets": List[DataSetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "deployments": List[DeploymentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEngineVersionsResponseTypeDef = TypedDict(
     "ListEngineVersionsResponseTypeDef",
     {
         "engineVersions": List[EngineVersionsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "environments": List[EnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StorageConfigurationTypeDef = TypedDict(
     "StorageConfigurationTypeDef",
     {
         "efs": EfsStorageConfigurationTypeDef,
@@ -1348,18 +1154,214 @@
         "logGroups": List[LogGroupSummaryTypeDef],
         "name": str,
         "roleArn": str,
         "status": ApplicationLifecycleType,
         "statusReason": str,
         "tags": Dict[str, str],
         "targetGroupArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
+    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "environmentId": str,
+        "names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
+    "_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
+    "_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    {
+        "prefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
+    _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+    _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
+    _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+    _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "prefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDataSetsRequestListDataSetsPaginateTypeDef(
+    _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
+    _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
+    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
+):
+    pass
+
+
+ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
+    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
+    {
+        "engineType": EngineTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "engineType": EngineTypeType,
+        "names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    {
+        "executionIds": Sequence[str],
+        "jobName": str,
+        "startedAfter": TimestampTypeDef,
+        "startedBefore": TimestampTypeDef,
+        "status": BatchJobExecutionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
+    _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+    _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListBatchJobExecutionsRequestRequestTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListBatchJobExecutionsRequestRequestTypeDef",
+    {
+        "executionIds": Sequence[str],
+        "jobName": str,
+        "maxResults": int,
+        "nextToken": str,
+        "startedAfter": TimestampTypeDef,
+        "startedBefore": TimestampTypeDef,
+        "status": BatchJobExecutionStatusType,
+    },
+    total=False,
+)
+
+
+class ListBatchJobExecutionsRequestRequestTypeDef(
+    _RequiredListBatchJobExecutionsRequestRequestTypeDef,
+    _OptionalListBatchJobExecutionsRequestRequestTypeDef,
+):
+    pass
+
+
 PendingMaintenanceTypeDef = TypedDict(
     "PendingMaintenanceTypeDef",
     {
         "engineVersion": str,
         "schedule": MaintenanceScheduleTypeDef,
     },
     total=False,
@@ -1401,15 +1403,15 @@
 )
 
 ListBatchJobDefinitionsResponseTypeDef = TypedDict(
     "ListBatchJobDefinitionsResponseTypeDef",
     {
         "batchJobDefinitions": List[BatchJobDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
     "_RequiredBatchJobExecutionSummaryTypeDef",
     {
         "applicationId": str,
@@ -1449,15 +1451,15 @@
         "jobName": str,
         "jobType": BatchJobTypeType,
         "jobUser": str,
         "returnCode": str,
         "startTime": datetime,
         "status": BatchJobExecutionStatusType,
         "statusReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartBatchJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartBatchJobRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -1480,15 +1482,15 @@
 
 
 ListDataSetImportHistoryResponseTypeDef = TypedDict(
     "ListDataSetImportHistoryResponseTypeDef",
     {
         "dataSetImportTasks": List[DataSetImportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
@@ -1542,15 +1544,15 @@
         "securityGroupIds": List[str],
         "status": EnvironmentLifecycleType,
         "statusReason": str,
         "storageConfigurations": List[StorageConfigurationTypeDef],
         "subnetIds": List[str],
         "tags": Dict[str, str],
         "vpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetOrgAttributesTypeDef = TypedDict(
     "DatasetOrgAttributesTypeDef",
     {
         "gdg": GdgAttributesTypeDef,
@@ -1573,15 +1575,15 @@
 )
 
 ListBatchJobExecutionsResponseTypeDef = TypedDict(
     "ListBatchJobExecutionsResponseTypeDef",
     {
         "batchJobExecutions": List[BatchJobExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDataSetTypeDef = TypedDict(
     "_RequiredDataSetTypeDef",
     {
         "datasetName": str,
@@ -1610,15 +1612,15 @@
         "creationTime": datetime,
         "dataSetName": str,
         "dataSetOrg": DatasetDetailOrgAttributesTypeDef,
         "lastReferencedTime": datetime,
         "lastUpdatedTime": datetime,
         "location": str,
         "recordLength": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataSetImportItemTypeDef = TypedDict(
     "DataSetImportItemTypeDef",
     {
         "dataSet": DataSetTypeDef,
```

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2/type_defs.pyi` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_m2.type_defs import AlternateKeyTypeDef
 
-    data: AlternateKeyTypeDef = {...}
+    data: AlternateKeyTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -38,20 +38,17 @@
     "ApplicationVersionSummaryTypeDef",
     "FileBatchJobDefinitionTypeDef",
     "ScriptBatchJobDefinitionTypeDef",
     "FileBatchJobIdentifierTypeDef",
     "ScriptBatchJobIdentifierTypeDef",
     "CancelBatchJobExecutionRequestRequestTypeDef",
     "DefinitionTypeDef",
-    "CreateApplicationResponseTypeDef",
-    "CreateDataSetImportTaskResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "CreateDeploymentResponseTypeDef",
     "HighAvailabilityConfigTypeDef",
-    "CreateEnvironmentResponseTypeDef",
     "ExternalLocationTypeDef",
     "DataSetImportSummaryTypeDef",
     "DataSetSummaryTypeDef",
     "RecordLengthTypeDef",
     "GdgDetailAttributesTypeDef",
     "PoDetailAttributesTypeDef",
     "PsDetailAttributesTypeDef",
@@ -66,67 +63,71 @@
     "EfsStorageConfigurationTypeDef",
     "EngineVersionsSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "FsxStorageConfigurationTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "LogGroupSummaryTypeDef",
     "GetApplicationVersionRequestRequestTypeDef",
-    "GetApplicationVersionResponseTypeDef",
     "GetBatchJobExecutionRequestRequestTypeDef",
     "GetDataSetDetailsRequestRequestTypeDef",
     "GetDataSetImportTaskRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
-    "GetDeploymentResponseTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
-    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
     "ListBatchJobDefinitionsRequestRequestTypeDef",
-    "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    "ListBatchJobExecutionsRequestRequestTypeDef",
-    "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    "TimestampTypeDef",
     "ListDataSetImportHistoryRequestRequestTypeDef",
-    "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListDataSetsRequestRequestTypeDef",
-    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListDeploymentsRequestRequestTypeDef",
-    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
     "ListEngineVersionsRequestRequestTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MaintenanceScheduleTypeDef",
-    "PaginatorConfigTypeDef",
     "PrimaryKeyTypeDef",
-    "ResponseMetadataTypeDef",
     "StartApplicationRequestRequestTypeDef",
-    "StartBatchJobResponseTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateApplicationResponseTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
-    "UpdateEnvironmentResponseTypeDef",
-    "ListApplicationsResponseTypeDef",
-    "ListApplicationVersionsResponseTypeDef",
     "BatchJobDefinitionTypeDef",
     "BatchJobIdentifierTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "CreateDataSetImportTaskResponseTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "CreateEnvironmentResponseTypeDef",
+    "GetApplicationVersionResponseTypeDef",
+    "GetDeploymentResponseTypeDef",
+    "ListApplicationVersionsResponseTypeDef",
+    "ListApplicationsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartBatchJobResponseTypeDef",
+    "UpdateApplicationResponseTypeDef",
+    "UpdateEnvironmentResponseTypeDef",
     "DataSetImportTaskTypeDef",
     "GetDataSetImportTaskResponseTypeDef",
     "ListDataSetsResponseTypeDef",
     "ListDeploymentsResponseTypeDef",
     "ListEngineVersionsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "StorageConfigurationTypeDef",
     "GetApplicationResponseTypeDef",
+    "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    "ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    "ListDataSetsRequestListDataSetsPaginateTypeDef",
+    "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    "ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    "ListBatchJobExecutionsRequestRequestTypeDef",
     "PendingMaintenanceTypeDef",
     "VsamAttributesTypeDef",
     "VsamDetailAttributesTypeDef",
     "ListBatchJobDefinitionsResponseTypeDef",
     "BatchJobExecutionSummaryTypeDef",
     "GetBatchJobExecutionResponseTypeDef",
     "StartBatchJobRequestRequestTypeDef",
@@ -278,29 +279,22 @@
     {
         "content": str,
         "s3Location": str,
     },
     total=False,
 )
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "applicationArn": str,
-        "applicationId": str,
-        "applicationVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDataSetImportTaskResponseTypeDef = TypedDict(
-    "CreateDataSetImportTaskResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -317,37 +311,21 @@
 )
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
-    {
-        "deploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 HighAvailabilityConfigTypeDef = TypedDict(
     "HighAvailabilityConfigTypeDef",
     {
         "desiredCapacity": int,
     },
 )
 
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExternalLocationTypeDef = TypedDict(
     "ExternalLocationTypeDef",
     {
         "s3Location": str,
     },
     total=False,
 )
@@ -584,28 +562,14 @@
     "GetApplicationVersionRequestRequestTypeDef",
     {
         "applicationId": str,
         "applicationVersion": int,
     },
 )
 
-GetApplicationVersionResponseTypeDef = TypedDict(
-    "GetApplicationVersionResponseTypeDef",
-    {
-        "applicationVersion": int,
-        "creationTime": datetime,
-        "definitionContent": str,
-        "description": str,
-        "name": str,
-        "status": ApplicationVersionLifecycleType,
-        "statusReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBatchJobExecutionRequestRequestTypeDef = TypedDict(
     "GetBatchJobExecutionRequestRequestTypeDef",
     {
         "applicationId": str,
         "executionId": str,
     },
 )
@@ -630,55 +594,31 @@
     "GetDeploymentRequestRequestTypeDef",
     {
         "applicationId": str,
         "deploymentId": str,
     },
 )
 
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "applicationId": str,
-        "applicationVersion": int,
-        "creationTime": datetime,
-        "deploymentId": str,
-        "environmentId": str,
-        "status": DeploymentLifecycleType,
-        "statusReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEnvironmentRequestRequestTypeDef = TypedDict(
     "GetEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
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
 
-class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
-    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListApplicationVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationVersionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListApplicationVersionsRequestRequestTypeDef = TypedDict(
@@ -692,56 +632,25 @@
 
 class ListApplicationVersionsRequestRequestTypeDef(
     _RequiredListApplicationVersionsRequestRequestTypeDef,
     _OptionalListApplicationVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "environmentId": str,
-        "names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
         "environmentId": str,
         "maxResults": int,
         "names": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
-    "_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
-    "_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
-    {
-        "prefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
-    _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-    _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
     "_RequiredListBatchJobDefinitionsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListBatchJobDefinitionsRequestRequestTypeDef = TypedDict(
@@ -756,85 +665,15 @@
 
 class ListBatchJobDefinitionsRequestRequestTypeDef(
     _RequiredListBatchJobDefinitionsRequestRequestTypeDef,
     _OptionalListBatchJobDefinitionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
-    {
-        "executionIds": Sequence[str],
-        "jobName": str,
-        "startedAfter": Union[datetime, str],
-        "startedBefore": Union[datetime, str],
-        "status": BatchJobExecutionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
-    _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-):
-    pass
-
-_RequiredListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
-    "_RequiredListBatchJobExecutionsRequestRequestTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
-    "_OptionalListBatchJobExecutionsRequestRequestTypeDef",
-    {
-        "executionIds": Sequence[str],
-        "jobName": str,
-        "maxResults": int,
-        "nextToken": str,
-        "startedAfter": Union[datetime, str],
-        "startedBefore": Union[datetime, str],
-        "status": BatchJobExecutionStatusType,
-    },
-    total=False,
-)
-
-class ListBatchJobExecutionsRequestRequestTypeDef(
-    _RequiredListBatchJobExecutionsRequestRequestTypeDef,
-    _OptionalListBatchJobExecutionsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
-    _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-    _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetImportHistoryRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetImportHistoryRequestRequestTypeDef = TypedDict(
@@ -848,35 +687,14 @@
 
 class ListDataSetImportHistoryRequestRequestTypeDef(
     _RequiredListDataSetImportHistoryRequestRequestTypeDef,
     _OptionalListDataSetImportHistoryRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
-    "_OptionalListDataSetsRequestListDataSetsPaginateTypeDef",
-    {
-        "prefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDataSetsRequestListDataSetsPaginateTypeDef(
-    _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
-    _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDataSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSetsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDataSetsRequestRequestTypeDef = TypedDict(
@@ -890,34 +708,14 @@
 )
 
 class ListDataSetsRequestRequestTypeDef(
     _RequiredListDataSetsRequestRequestTypeDef, _OptionalListDataSetsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "applicationId": str,
-    },
-)
-_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
-    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
-    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeploymentsRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalListDeploymentsRequestRequestTypeDef = TypedDict(
@@ -930,43 +728,24 @@
 )
 
 class ListDeploymentsRequestRequestTypeDef(
     _RequiredListDeploymentsRequestRequestTypeDef, _OptionalListDeploymentsRequestRequestTypeDef
 ):
     pass
 
-ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
-    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
-    {
-        "engineType": EngineTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEngineVersionsRequestRequestTypeDef = TypedDict(
     "ListEngineVersionsRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "engineType": EngineTypeType,
-        "names": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
         "maxResults": int,
         "names": Sequence[str],
         "nextToken": str,
@@ -977,41 +756,23 @@
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
 MaintenanceScheduleTypeDef = TypedDict(
     "MaintenanceScheduleTypeDef",
     {
         "endTime": datetime,
         "startTime": datetime,
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
 _RequiredPrimaryKeyTypeDef = TypedDict(
     "_RequiredPrimaryKeyTypeDef",
     {
         "length": int,
         "offset": int,
     },
 )
@@ -1022,40 +783,21 @@
     },
     total=False,
 )
 
 class PrimaryKeyTypeDef(_RequiredPrimaryKeyTypeDef, _OptionalPrimaryKeyTypeDef):
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
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
-StartBatchJobResponseTypeDef = TypedDict(
-    "StartBatchJobResponseTypeDef",
-    {
-        "executionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredStopApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 _OptionalStopApplicationRequestRequestTypeDef = TypedDict(
@@ -1083,22 +825,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateApplicationResponseTypeDef = TypedDict(
-    "UpdateApplicationResponseTypeDef",
-    {
-        "applicationVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateEnvironmentRequestRequestTypeDef = TypedDict(
@@ -1114,40 +848,14 @@
 )
 
 class UpdateEnvironmentRequestRequestTypeDef(
     _RequiredUpdateEnvironmentRequestRequestTypeDef, _OptionalUpdateEnvironmentRequestRequestTypeDef
 ):
     pass
 
-UpdateEnvironmentResponseTypeDef = TypedDict(
-    "UpdateEnvironmentResponseTypeDef",
-    {
-        "environmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListApplicationsResponseTypeDef = TypedDict(
-    "ListApplicationsResponseTypeDef",
-    {
-        "applications": List[ApplicationSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListApplicationVersionsResponseTypeDef = TypedDict(
-    "ListApplicationVersionsResponseTypeDef",
-    {
-        "applicationVersions": List[ApplicationVersionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchJobDefinitionTypeDef = TypedDict(
     "BatchJobDefinitionTypeDef",
     {
         "fileBatchJobDefinition": FileBatchJobDefinitionTypeDef,
         "scriptBatchJobDefinition": ScriptBatchJobDefinitionTypeDef,
     },
     total=False,
@@ -1204,14 +912,126 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationArn": str,
+        "applicationId": str,
+        "applicationVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataSetImportTaskResponseTypeDef = TypedDict(
+    "CreateDataSetImportTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "deploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApplicationVersionResponseTypeDef = TypedDict(
+    "GetApplicationVersionResponseTypeDef",
+    {
+        "applicationVersion": int,
+        "creationTime": datetime,
+        "definitionContent": str,
+        "description": str,
+        "name": str,
+        "status": ApplicationVersionLifecycleType,
+        "statusReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "applicationId": str,
+        "applicationVersion": int,
+        "creationTime": datetime,
+        "deploymentId": str,
+        "environmentId": str,
+        "status": DeploymentLifecycleType,
+        "statusReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationVersionsResponseTypeDef = TypedDict(
+    "ListApplicationVersionsResponseTypeDef",
+    {
+        "applicationVersions": List[ApplicationVersionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsResponseTypeDef = TypedDict(
+    "ListApplicationsResponseTypeDef",
+    {
+        "applications": List[ApplicationSummaryTypeDef],
+        "nextToken": str,
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
+StartBatchJobResponseTypeDef = TypedDict(
+    "StartBatchJobResponseTypeDef",
+    {
+        "executionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApplicationResponseTypeDef = TypedDict(
+    "UpdateApplicationResponseTypeDef",
+    {
+        "applicationVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEnvironmentResponseTypeDef = TypedDict(
+    "UpdateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DataSetImportTaskTypeDef = TypedDict(
     "DataSetImportTaskTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
     },
@@ -1219,51 +1039,51 @@
 
 GetDataSetImportTaskResponseTypeDef = TypedDict(
     "GetDataSetImportTaskResponseTypeDef",
     {
         "status": DataSetTaskLifecycleType,
         "summary": DataSetImportSummaryTypeDef,
         "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataSetsResponseTypeDef = TypedDict(
     "ListDataSetsResponseTypeDef",
     {
         "dataSets": List[DataSetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDeploymentsResponseTypeDef = TypedDict(
     "ListDeploymentsResponseTypeDef",
     {
         "deployments": List[DeploymentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEngineVersionsResponseTypeDef = TypedDict(
     "ListEngineVersionsResponseTypeDef",
     {
         "engineVersions": List[EngineVersionsSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "environments": List[EnvironmentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StorageConfigurationTypeDef = TypedDict(
     "StorageConfigurationTypeDef",
     {
         "efs": EfsStorageConfigurationTypeDef,
@@ -1291,17 +1111,199 @@
         "logGroups": List[LogGroupSummaryTypeDef],
         "name": str,
         "roleArn": str,
         "status": ApplicationLifecycleType,
         "statusReason": str,
         "tags": Dict[str, str],
         "targetGroupArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "applicationId": str,
     },
 )
+_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef(
+    _RequiredListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    _OptionalListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+):
+    pass
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "environmentId": str,
+        "names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
+    "_RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef = TypedDict(
+    "_OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef",
+    {
+        "prefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef(
+    _RequiredListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+    _OptionalListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef(
+    _RequiredListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+    _OptionalListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+):
+    pass
+
+_RequiredListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "_RequiredListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDataSetsRequestListDataSetsPaginateTypeDef = TypedDict(
+    "_OptionalListDataSetsRequestListDataSetsPaginateTypeDef",
+    {
+        "prefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDataSetsRequestListDataSetsPaginateTypeDef(
+    _RequiredListDataSetsRequestListDataSetsPaginateTypeDef,
+    _OptionalListDataSetsRequestListDataSetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDeploymentsRequestListDeploymentsPaginateTypeDef(
+    _RequiredListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    _OptionalListDeploymentsRequestListDeploymentsPaginateTypeDef,
+):
+    pass
+
+ListEngineVersionsRequestListEngineVersionsPaginateTypeDef = TypedDict(
+    "ListEngineVersionsRequestListEngineVersionsPaginateTypeDef",
+    {
+        "engineType": EngineTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "engineType": EngineTypeType,
+        "names": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef",
+    {
+        "executionIds": Sequence[str],
+        "jobName": str,
+        "startedAfter": TimestampTypeDef,
+        "startedBefore": TimestampTypeDef,
+        "status": BatchJobExecutionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef(
+    _RequiredListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+    _OptionalListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListBatchJobExecutionsRequestRequestTypeDef",
+    {
+        "applicationId": str,
+    },
+)
+_OptionalListBatchJobExecutionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListBatchJobExecutionsRequestRequestTypeDef",
+    {
+        "executionIds": Sequence[str],
+        "jobName": str,
+        "maxResults": int,
+        "nextToken": str,
+        "startedAfter": TimestampTypeDef,
+        "startedBefore": TimestampTypeDef,
+        "status": BatchJobExecutionStatusType,
+    },
+    total=False,
+)
+
+class ListBatchJobExecutionsRequestRequestTypeDef(
+    _RequiredListBatchJobExecutionsRequestRequestTypeDef,
+    _OptionalListBatchJobExecutionsRequestRequestTypeDef,
+):
+    pass
 
 PendingMaintenanceTypeDef = TypedDict(
     "PendingMaintenanceTypeDef",
     {
         "engineVersion": str,
         "schedule": MaintenanceScheduleTypeDef,
     },
@@ -1342,15 +1344,15 @@
 )
 
 ListBatchJobDefinitionsResponseTypeDef = TypedDict(
     "ListBatchJobDefinitionsResponseTypeDef",
     {
         "batchJobDefinitions": List[BatchJobDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchJobExecutionSummaryTypeDef = TypedDict(
     "_RequiredBatchJobExecutionSummaryTypeDef",
     {
         "applicationId": str,
@@ -1388,15 +1390,15 @@
         "jobName": str,
         "jobType": BatchJobTypeType,
         "jobUser": str,
         "returnCode": str,
         "startTime": datetime,
         "status": BatchJobExecutionStatusType,
         "statusReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartBatchJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartBatchJobRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -1417,15 +1419,15 @@
     pass
 
 ListDataSetImportHistoryResponseTypeDef = TypedDict(
     "ListDataSetImportHistoryResponseTypeDef",
     {
         "dataSetImportTasks": List[DataSetImportTaskTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "engineType": EngineTypeType,
@@ -1477,15 +1479,15 @@
         "securityGroupIds": List[str],
         "status": EnvironmentLifecycleType,
         "statusReason": str,
         "storageConfigurations": List[StorageConfigurationTypeDef],
         "subnetIds": List[str],
         "tags": Dict[str, str],
         "vpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetOrgAttributesTypeDef = TypedDict(
     "DatasetOrgAttributesTypeDef",
     {
         "gdg": GdgAttributesTypeDef,
@@ -1508,15 +1510,15 @@
 )
 
 ListBatchJobExecutionsResponseTypeDef = TypedDict(
     "ListBatchJobExecutionsResponseTypeDef",
     {
         "batchJobExecutions": List[BatchJobExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDataSetTypeDef = TypedDict(
     "_RequiredDataSetTypeDef",
     {
         "datasetName": str,
@@ -1543,15 +1545,15 @@
         "creationTime": datetime,
         "dataSetName": str,
         "dataSetOrg": DatasetDetailOrgAttributesTypeDef,
         "lastReferencedTime": datetime,
         "lastUpdatedTime": datetime,
         "location": str,
         "recordLength": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataSetImportItemTypeDef = TypedDict(
     "DataSetImportItemTypeDef",
     {
         "dataSet": DataSetTypeDef,
```

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2.egg-info/PKG-INFO` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-m2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.MainframeModernization 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.MainframeModernization 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore m2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore m2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-m2"></a>
 
 # types-aiobotocore-m2
 
 [![PyPI - types-aiobotocore-m2](https://img.shields.io/pypi/v/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-m2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-m2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-m2?color=blue)](https://pypistats.org/packages/types-aiobotocore-m2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-m2)](https://pepy.tech/project/types-aiobotocore-m2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MainframeModernization 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization)
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
 [types-aiobotocore-m2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/).
 
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
@@ -353,38 +352,35 @@
 )
 
 
 def check_value(value: ApplicationDeploymentLifecycleType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_m2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_m2.type_defs import (
     AlternateKeyTypeDef,
     ApplicationSummaryTypeDef,
     ApplicationVersionSummaryTypeDef,
     FileBatchJobDefinitionTypeDef,
     ScriptBatchJobDefinitionTypeDef,
     FileBatchJobIdentifierTypeDef,
     ScriptBatchJobIdentifierTypeDef,
     CancelBatchJobExecutionRequestRequestTypeDef,
     DefinitionTypeDef,
-    CreateApplicationResponseTypeDef,
-    CreateDataSetImportTaskResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
     HighAvailabilityConfigTypeDef,
-    CreateEnvironmentResponseTypeDef,
     ExternalLocationTypeDef,
     DataSetImportSummaryTypeDef,
     DataSetSummaryTypeDef,
     RecordLengthTypeDef,
     GdgDetailAttributesTypeDef,
     PoDetailAttributesTypeDef,
     PsDetailAttributesTypeDef,
@@ -399,67 +395,71 @@
     EfsStorageConfigurationTypeDef,
     EngineVersionsSummaryTypeDef,
     EnvironmentSummaryTypeDef,
     FsxStorageConfigurationTypeDef,
     GetApplicationRequestRequestTypeDef,
     LogGroupSummaryTypeDef,
     GetApplicationVersionRequestRequestTypeDef,
-    GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionRequestRequestTypeDef,
     GetDataSetDetailsRequestRequestTypeDef,
     GetDataSetImportTaskRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetDeploymentResponseTypeDef,
     GetEnvironmentRequestRequestTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationVersionsRequestRequestTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
     ListBatchJobDefinitionsRequestRequestTypeDef,
-    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
-    ListBatchJobExecutionsRequestRequestTypeDef,
-    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+    TimestampTypeDef,
     ListDataSetImportHistoryRequestRequestTypeDef,
-    ListDataSetsRequestListDataSetsPaginateTypeDef,
     ListDataSetsRequestRequestTypeDef,
-    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
     ListDeploymentsRequestRequestTypeDef,
-    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
     ListEngineVersionsRequestRequestTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MaintenanceScheduleTypeDef,
-    PaginatorConfigTypeDef,
     PrimaryKeyTypeDef,
-    ResponseMetadataTypeDef,
     StartApplicationRequestRequestTypeDef,
-    StartBatchJobResponseTypeDef,
     StopApplicationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateApplicationResponseTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
-    UpdateEnvironmentResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    ListApplicationVersionsResponseTypeDef,
     BatchJobDefinitionTypeDef,
     BatchJobIdentifierTypeDef,
     CreateApplicationRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    CreateApplicationResponseTypeDef,
+    CreateDataSetImportTaskResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateEnvironmentResponseTypeDef,
+    GetApplicationVersionResponseTypeDef,
+    GetDeploymentResponseTypeDef,
+    ListApplicationVersionsResponseTypeDef,
+    ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartBatchJobResponseTypeDef,
+    UpdateApplicationResponseTypeDef,
+    UpdateEnvironmentResponseTypeDef,
     DataSetImportTaskTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDeploymentsResponseTypeDef,
     ListEngineVersionsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     StorageConfigurationTypeDef,
     GetApplicationResponseTypeDef,
+    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListBatchJobDefinitionsRequestListBatchJobDefinitionsPaginateTypeDef,
+    ListDataSetImportHistoryRequestListDataSetImportHistoryPaginateTypeDef,
+    ListDataSetsRequestListDataSetsPaginateTypeDef,
+    ListDeploymentsRequestListDeploymentsPaginateTypeDef,
+    ListEngineVersionsRequestListEngineVersionsPaginateTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
+    ListBatchJobExecutionsRequestListBatchJobExecutionsPaginateTypeDef,
+    ListBatchJobExecutionsRequestRequestTypeDef,
     PendingMaintenanceTypeDef,
     VsamAttributesTypeDef,
     VsamDetailAttributesTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     BatchJobExecutionSummaryTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     StartBatchJobRequestRequestTypeDef,
@@ -473,15 +473,15 @@
     GetDataSetDetailsResponseTypeDef,
     DataSetImportItemTypeDef,
     DataSetImportConfigTypeDef,
     CreateDataSetImportTaskRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AlternateKeyTypeDef:
+def get_value() -> AlternateKeyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-m2-2.5.2/types_aiobotocore_m2.egg-info/SOURCES.txt` & `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


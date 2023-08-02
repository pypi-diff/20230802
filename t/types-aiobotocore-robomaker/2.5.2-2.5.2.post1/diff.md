# Comparing `tmp/types-aiobotocore-robomaker-2.5.2.tar.gz` & `tmp/types-aiobotocore-robomaker-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-robomaker-2.5.2.tar", last modified: Sat Jul  8 01:44:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-robomaker-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:53 2023, max compression
```

## Comparing `types-aiobotocore-robomaker-2.5.2.tar` & `types-aiobotocore-robomaker-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:12.342779 types-aiobotocore-robomaker-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:21.000000 types-aiobotocore-robomaker-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22174 2023-07-08 01:44:12.342779 types-aiobotocore-robomaker-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-07-08 01:39:21.000000 types-aiobotocore-robomaker-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:12.342779 types-aiobotocore-robomaker-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:39:19.000000 types-aiobotocore-robomaker-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:12.338780 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-08 01:39:21.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-08 01:39:21.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:39:21.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44856 2023-07-08 01:39:22.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    44779 2023-07-08 01:39:22.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-07-08 01:39:22.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-07-08 01:39:22.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14027 2023-07-08 01:39:22.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-08 01:39:22.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:21.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63629 2023-07-08 01:39:23.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63574 2023-07-08 01:39:23.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:21.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:12.342779 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22174 2023-07-08 01:44:12.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-08 01:44:12.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:12.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:12.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:12.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:44:12.000000 types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:53.529479 types-aiobotocore-robomaker-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-08-02 14:52:53.521479 types-aiobotocore-robomaker-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:53.529479 types-aiobotocore-robomaker-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:53.521479 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44916 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44839 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-08-02 14:47:58.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    69711 2023-08-02 14:47:59.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69645 2023-08-02 14:47:58.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:53.521479 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-08-02 14:52:53.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:53.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:53.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:53.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:53.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:53.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-robomaker-2.5.2/LICENSE` & `types-aiobotocore-robomaker-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2/PKG-INFO` & `types-aiobotocore-robomaker-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-robomaker
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.RoboMaker 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.RoboMaker 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore robomaker type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore robomaker type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-robomaker"></a>
 
 # types-aiobotocore-robomaker
 
 [![PyPI - types-aiobotocore-robomaker](https://img.shields.io/pypi/v/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-robomaker?color=blue)](https://pypistats.org/packages/types-aiobotocore-robomaker)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-robomaker)](https://pepy.tech/project/types-aiobotocore-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.RoboMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [types-aiobotocore-robomaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/).
 
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
@@ -375,106 +374,108 @@
 )
 
 
 def check_value(value: ArchitectureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_robomaker.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
-    BatchDeleteWorldsResponseTypeDef,
+    ResponseMetadataTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
     BatchPolicyTypeDef,
     CancelDeploymentJobRequestRequestTypeDef,
     CancelSimulationJobBatchRequestRequestTypeDef,
     CancelSimulationJobRequestRequestTypeDef,
     CancelWorldExportJobRequestRequestTypeDef,
     CancelWorldGenerationJobRequestRequestTypeDef,
     ComputeResponseTypeDef,
     ComputeTypeDef,
     CreateFleetRequestRequestTypeDef,
-    CreateFleetResponseTypeDef,
     EnvironmentTypeDef,
     RobotSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
-    CreateRobotResponseTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
-    DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
     TemplateLocationTypeDef,
-    CreateWorldTemplateResponseTypeDef,
+    DataSourceConfigOutputTypeDef,
+    DataSourceConfigTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
+    DeploymentLaunchConfigOutputTypeDef,
     DeploymentLaunchConfigTypeDef,
     S3ObjectTypeDef,
     DeregisterRobotRequestRequestTypeDef,
-    DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobRequestRequestTypeDef,
     DescribeFleetRequestRequestTypeDef,
     RobotTypeDef,
     DescribeRobotApplicationRequestRequestTypeDef,
     DescribeRobotRequestRequestTypeDef,
-    DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationRequestRequestTypeDef,
     DescribeSimulationJobBatchRequestRequestTypeDef,
     SimulationJobSummaryTypeDef,
     DescribeSimulationJobRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeWorldExportJobRequestRequestTypeDef,
     DescribeWorldGenerationJobRequestRequestTypeDef,
     DescribeWorldRequestRequestTypeDef,
-    DescribeWorldResponseTypeDef,
     DescribeWorldTemplateRequestRequestTypeDef,
-    DescribeWorldTemplateResponseTypeDef,
     WorldFailureTypeDef,
     FilterTypeDef,
     FleetTypeDef,
     GetWorldTemplateBodyRequestRequestTypeDef,
-    GetWorldTemplateBodyResponseTypeDef,
+    PaginatorConfigTypeDef,
     SimulationJobBatchSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
     ListWorldTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     WorldSummaryTypeDef,
-    PaginatorConfigTypeDef,
     PortMappingTypeDef,
     ProgressDetailTypeDef,
     RegisterRobotRequestRequestTypeDef,
-    RegisterRobotResponseTypeDef,
-    ResponseMetadataTypeDef,
     RestartSimulationJobRequestRequestTypeDef,
     ToolTypeDef,
     UploadConfigurationTypeDef,
     WorldConfigTypeDef,
+    VPCConfigOutputTypeDef,
     SyncDeploymentJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    BatchDeleteWorldsResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    CreateRobotResponseTypeDef,
+    CreateWorldTemplateResponseTypeDef,
+    DeregisterRobotResponseTypeDef,
+    DescribeRobotResponseTypeDef,
+    DescribeWorldResponseTypeDef,
+    DescribeWorldTemplateResponseTypeDef,
+    GetWorldTemplateBodyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterRobotResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
     RobotApplicationSummaryTypeDef,
     CreateRobotApplicationRequestRequestTypeDef,
     UpdateRobotApplicationRequestRequestTypeDef,
     CreateRobotApplicationResponseTypeDef,
     CreateRobotApplicationVersionResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
@@ -491,76 +492,89 @@
     DescribeWorldExportJobResponseTypeDef,
     WorldExportJobSummaryTypeDef,
     CreateWorldGenerationJobRequestRequestTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     WorldGenerationJobSummaryTypeDef,
     CreateWorldTemplateRequestRequestTypeDef,
     UpdateWorldTemplateRequestRequestTypeDef,
+    DataSourceConfigUnionTypeDef,
     DataSourceTypeDef,
+    DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
     FailureSummaryTypeDef,
-    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
     ListDeploymentJobsRequestRequestTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
-    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
     ListRobotApplicationsRequestRequestTypeDef,
-    ListRobotsRequestListRobotsPaginateTypeDef,
     ListRobotsRequestRequestTypeDef,
-    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
     ListSimulationApplicationsRequestRequestTypeDef,
-    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
     ListSimulationJobBatchesRequestRequestTypeDef,
-    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
     ListSimulationJobsRequestRequestTypeDef,
-    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
     ListWorldExportJobsRequestRequestTypeDef,
-    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
     ListWorldGenerationJobsRequestRequestTypeDef,
-    ListWorldsRequestListWorldsPaginateTypeDef,
     ListWorldsRequestRequestTypeDef,
     ListFleetsResponseTypeDef,
+    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
+    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
+    ListRobotsRequestListRobotsPaginateTypeDef,
+    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
+    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
+    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
+    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
+    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
+    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
+    ListWorldsRequestListWorldsPaginateTypeDef,
     ListSimulationJobBatchesResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     ListWorldsResponseTypeDef,
+    PortForwardingConfigOutputTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
+    VPCConfigUnionTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
     ListWorldExportJobsResponseTypeDef,
     ListWorldGenerationJobsResponseTypeDef,
-    CreateDeploymentJobRequestRequestTypeDef,
+    DeploymentApplicationConfigUnionTypeDef,
     CreateDeploymentJobResponseTypeDef,
     DeploymentJobTypeDef,
     SyncDeploymentJobResponseTypeDef,
     FinishedWorldsSummaryTypeDef,
+    LaunchConfigOutputTypeDef,
     LaunchConfigTypeDef,
     DescribeDeploymentJobResponseTypeDef,
+    CreateDeploymentJobRequestRequestTypeDef,
     ListDeploymentJobsResponseTypeDef,
     DescribeWorldGenerationJobResponseTypeDef,
+    RobotApplicationConfigOutputTypeDef,
+    SimulationApplicationConfigOutputTypeDef,
     RobotApplicationConfigTypeDef,
     SimulationApplicationConfigTypeDef,
-    CreateSimulationJobRequestRequestTypeDef,
     CreateSimulationJobResponseTypeDef,
     DescribeSimulationJobResponseTypeDef,
-    SimulationJobRequestTypeDef,
+    SimulationJobRequestOutputTypeDef,
     SimulationJobTypeDef,
+    RobotApplicationConfigUnionTypeDef,
+    SimulationApplicationConfigUnionTypeDef,
+    SimulationJobRequestTypeDef,
     FailedCreateSimulationJobRequestTypeDef,
-    StartSimulationJobBatchRequestRequestTypeDef,
     BatchDescribeSimulationJobResponseTypeDef,
+    CreateSimulationJobRequestRequestTypeDef,
+    SimulationJobRequestUnionTypeDef,
     DescribeSimulationJobBatchResponseTypeDef,
     StartSimulationJobBatchResponseTypeDef,
+    StartSimulationJobBatchRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BatchDeleteWorldsRequestRequestTypeDef:
+def get_value() -> BatchDeleteWorldsRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-robomaker-2.5.2/README.md` & `types-aiobotocore-robomaker-2.5.2.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-robomaker"></a>
 
 # types-aiobotocore-robomaker
 
 [![PyPI - types-aiobotocore-robomaker](https://img.shields.io/pypi/v/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-robomaker?color=blue)](https://pypistats.org/packages/types-aiobotocore-robomaker)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-robomaker)](https://pepy.tech/project/types-aiobotocore-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.RoboMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [types-aiobotocore-robomaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/).
 
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
@@ -342,106 +342,108 @@
 )
 
 
 def check_value(value: ArchitectureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_robomaker.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
-    BatchDeleteWorldsResponseTypeDef,
+    ResponseMetadataTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
     BatchPolicyTypeDef,
     CancelDeploymentJobRequestRequestTypeDef,
     CancelSimulationJobBatchRequestRequestTypeDef,
     CancelSimulationJobRequestRequestTypeDef,
     CancelWorldExportJobRequestRequestTypeDef,
     CancelWorldGenerationJobRequestRequestTypeDef,
     ComputeResponseTypeDef,
     ComputeTypeDef,
     CreateFleetRequestRequestTypeDef,
-    CreateFleetResponseTypeDef,
     EnvironmentTypeDef,
     RobotSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
-    CreateRobotResponseTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
-    DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
     TemplateLocationTypeDef,
-    CreateWorldTemplateResponseTypeDef,
+    DataSourceConfigOutputTypeDef,
+    DataSourceConfigTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
+    DeploymentLaunchConfigOutputTypeDef,
     DeploymentLaunchConfigTypeDef,
     S3ObjectTypeDef,
     DeregisterRobotRequestRequestTypeDef,
-    DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobRequestRequestTypeDef,
     DescribeFleetRequestRequestTypeDef,
     RobotTypeDef,
     DescribeRobotApplicationRequestRequestTypeDef,
     DescribeRobotRequestRequestTypeDef,
-    DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationRequestRequestTypeDef,
     DescribeSimulationJobBatchRequestRequestTypeDef,
     SimulationJobSummaryTypeDef,
     DescribeSimulationJobRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeWorldExportJobRequestRequestTypeDef,
     DescribeWorldGenerationJobRequestRequestTypeDef,
     DescribeWorldRequestRequestTypeDef,
-    DescribeWorldResponseTypeDef,
     DescribeWorldTemplateRequestRequestTypeDef,
-    DescribeWorldTemplateResponseTypeDef,
     WorldFailureTypeDef,
     FilterTypeDef,
     FleetTypeDef,
     GetWorldTemplateBodyRequestRequestTypeDef,
-    GetWorldTemplateBodyResponseTypeDef,
+    PaginatorConfigTypeDef,
     SimulationJobBatchSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
     ListWorldTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     WorldSummaryTypeDef,
-    PaginatorConfigTypeDef,
     PortMappingTypeDef,
     ProgressDetailTypeDef,
     RegisterRobotRequestRequestTypeDef,
-    RegisterRobotResponseTypeDef,
-    ResponseMetadataTypeDef,
     RestartSimulationJobRequestRequestTypeDef,
     ToolTypeDef,
     UploadConfigurationTypeDef,
     WorldConfigTypeDef,
+    VPCConfigOutputTypeDef,
     SyncDeploymentJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    BatchDeleteWorldsResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    CreateRobotResponseTypeDef,
+    CreateWorldTemplateResponseTypeDef,
+    DeregisterRobotResponseTypeDef,
+    DescribeRobotResponseTypeDef,
+    DescribeWorldResponseTypeDef,
+    DescribeWorldTemplateResponseTypeDef,
+    GetWorldTemplateBodyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterRobotResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
     RobotApplicationSummaryTypeDef,
     CreateRobotApplicationRequestRequestTypeDef,
     UpdateRobotApplicationRequestRequestTypeDef,
     CreateRobotApplicationResponseTypeDef,
     CreateRobotApplicationVersionResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
@@ -458,76 +460,89 @@
     DescribeWorldExportJobResponseTypeDef,
     WorldExportJobSummaryTypeDef,
     CreateWorldGenerationJobRequestRequestTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     WorldGenerationJobSummaryTypeDef,
     CreateWorldTemplateRequestRequestTypeDef,
     UpdateWorldTemplateRequestRequestTypeDef,
+    DataSourceConfigUnionTypeDef,
     DataSourceTypeDef,
+    DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
     FailureSummaryTypeDef,
-    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
     ListDeploymentJobsRequestRequestTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
-    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
     ListRobotApplicationsRequestRequestTypeDef,
-    ListRobotsRequestListRobotsPaginateTypeDef,
     ListRobotsRequestRequestTypeDef,
-    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
     ListSimulationApplicationsRequestRequestTypeDef,
-    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
     ListSimulationJobBatchesRequestRequestTypeDef,
-    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
     ListSimulationJobsRequestRequestTypeDef,
-    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
     ListWorldExportJobsRequestRequestTypeDef,
-    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
     ListWorldGenerationJobsRequestRequestTypeDef,
-    ListWorldsRequestListWorldsPaginateTypeDef,
     ListWorldsRequestRequestTypeDef,
     ListFleetsResponseTypeDef,
+    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
+    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
+    ListRobotsRequestListRobotsPaginateTypeDef,
+    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
+    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
+    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
+    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
+    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
+    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
+    ListWorldsRequestListWorldsPaginateTypeDef,
     ListSimulationJobBatchesResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     ListWorldsResponseTypeDef,
+    PortForwardingConfigOutputTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
+    VPCConfigUnionTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
     ListWorldExportJobsResponseTypeDef,
     ListWorldGenerationJobsResponseTypeDef,
-    CreateDeploymentJobRequestRequestTypeDef,
+    DeploymentApplicationConfigUnionTypeDef,
     CreateDeploymentJobResponseTypeDef,
     DeploymentJobTypeDef,
     SyncDeploymentJobResponseTypeDef,
     FinishedWorldsSummaryTypeDef,
+    LaunchConfigOutputTypeDef,
     LaunchConfigTypeDef,
     DescribeDeploymentJobResponseTypeDef,
+    CreateDeploymentJobRequestRequestTypeDef,
     ListDeploymentJobsResponseTypeDef,
     DescribeWorldGenerationJobResponseTypeDef,
+    RobotApplicationConfigOutputTypeDef,
+    SimulationApplicationConfigOutputTypeDef,
     RobotApplicationConfigTypeDef,
     SimulationApplicationConfigTypeDef,
-    CreateSimulationJobRequestRequestTypeDef,
     CreateSimulationJobResponseTypeDef,
     DescribeSimulationJobResponseTypeDef,
-    SimulationJobRequestTypeDef,
+    SimulationJobRequestOutputTypeDef,
     SimulationJobTypeDef,
+    RobotApplicationConfigUnionTypeDef,
+    SimulationApplicationConfigUnionTypeDef,
+    SimulationJobRequestTypeDef,
     FailedCreateSimulationJobRequestTypeDef,
-    StartSimulationJobBatchRequestRequestTypeDef,
     BatchDescribeSimulationJobResponseTypeDef,
+    CreateSimulationJobRequestRequestTypeDef,
+    SimulationJobRequestUnionTypeDef,
     DescribeSimulationJobBatchResponseTypeDef,
     StartSimulationJobBatchResponseTypeDef,
+    StartSimulationJobBatchRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BatchDeleteWorldsRequestRequestTypeDef:
+def get_value() -> BatchDeleteWorldsRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-robomaker-2.5.2/setup.py` & `types-aiobotocore-robomaker-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-robomaker",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_robomaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.RoboMaker 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore robomaker type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore robomaker type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_robomaker": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/"
```

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/__init__.py` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/__init__.pyi` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/__main__.py` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RoboMaker 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.RoboMaker 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker\nOther"
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

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/client.py` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     CreateRobotResponseTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     CreateSimulationJobResponseTypeDef,
     CreateWorldExportJobResponseTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     CreateWorldTemplateResponseTypeDef,
-    DataSourceConfigTypeDef,
-    DeploymentApplicationConfigTypeDef,
+    DataSourceConfigUnionTypeDef,
+    DeploymentApplicationConfigUnionTypeDef,
     DeploymentConfigTypeDef,
     DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     DescribeFleetResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationResponseTypeDef,
@@ -80,27 +80,27 @@
     ListWorldGenerationJobsResponseTypeDef,
     ListWorldsResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     RegisterRobotResponseTypeDef,
     RenderingEngineTypeDef,
-    RobotApplicationConfigTypeDef,
+    RobotApplicationConfigUnionTypeDef,
     RobotSoftwareSuiteTypeDef,
-    SimulationApplicationConfigTypeDef,
-    SimulationJobRequestTypeDef,
+    SimulationApplicationConfigUnionTypeDef,
+    SimulationJobRequestUnionTypeDef,
     SimulationSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     StartSimulationJobBatchResponseTypeDef,
     SyncDeploymentJobResponseTypeDef,
     TemplateLocationTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
-    VPCConfigTypeDef,
+    VPCConfigUnionTypeDef,
     WorldCountTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -224,15 +224,15 @@
         """
 
     async def create_deployment_job(
         self,
         *,
         clientRequestToken: str,
         fleet: str,
-        deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigTypeDef],
+        deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigUnionTypeDef],
         deploymentConfig: DeploymentConfigTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeploymentJobResponseTypeDef:
         """
         Deploys a specific version of a robot application to robots in a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_deployment_job)
@@ -333,19 +333,19 @@
         *,
         maxJobDurationInSeconds: int,
         iamRole: str,
         clientRequestToken: str = ...,
         outputLocation: OutputLocationTypeDef = ...,
         loggingConfig: LoggingConfigTypeDef = ...,
         failureBehavior: FailureBehaviorType = ...,
-        robotApplications: Sequence[RobotApplicationConfigTypeDef] = ...,
-        simulationApplications: Sequence[SimulationApplicationConfigTypeDef] = ...,
-        dataSources: Sequence[DataSourceConfigTypeDef] = ...,
+        robotApplications: Sequence[RobotApplicationConfigUnionTypeDef] = ...,
+        simulationApplications: Sequence[SimulationApplicationConfigUnionTypeDef] = ...,
+        dataSources: Sequence[DataSourceConfigUnionTypeDef] = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfig: VPCConfigTypeDef = ...,
+        vpcConfig: VPCConfigUnionTypeDef = ...,
         compute: ComputeTypeDef = ...
     ) -> CreateSimulationJobResponseTypeDef:
         """
         Creates a simulation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_simulation_job)
@@ -718,15 +718,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.restart_simulation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#restart_simulation_job)
         """
 
     async def start_simulation_job_batch(
         self,
         *,
-        createSimulationJobRequests: Sequence[SimulationJobRequestTypeDef],
+        createSimulationJobRequests: Sequence[SimulationJobRequestUnionTypeDef],
         clientRequestToken: str = ...,
         batchPolicy: BatchPolicyTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSimulationJobBatchResponseTypeDef:
         """
         Starts a new simulation job batch.
```

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/client.pyi` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     CreateRobotResponseTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     CreateSimulationJobResponseTypeDef,
     CreateWorldExportJobResponseTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     CreateWorldTemplateResponseTypeDef,
-    DataSourceConfigTypeDef,
-    DeploymentApplicationConfigTypeDef,
+    DataSourceConfigUnionTypeDef,
+    DeploymentApplicationConfigUnionTypeDef,
     DeploymentConfigTypeDef,
     DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     DescribeFleetResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationResponseTypeDef,
@@ -80,27 +80,27 @@
     ListWorldGenerationJobsResponseTypeDef,
     ListWorldsResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     RegisterRobotResponseTypeDef,
     RenderingEngineTypeDef,
-    RobotApplicationConfigTypeDef,
+    RobotApplicationConfigUnionTypeDef,
     RobotSoftwareSuiteTypeDef,
-    SimulationApplicationConfigTypeDef,
-    SimulationJobRequestTypeDef,
+    SimulationApplicationConfigUnionTypeDef,
+    SimulationJobRequestUnionTypeDef,
     SimulationSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     StartSimulationJobBatchResponseTypeDef,
     SyncDeploymentJobResponseTypeDef,
     TemplateLocationTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
-    VPCConfigTypeDef,
+    VPCConfigUnionTypeDef,
     WorldCountTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -210,15 +210,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#close)
         """
     async def create_deployment_job(
         self,
         *,
         clientRequestToken: str,
         fleet: str,
-        deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigTypeDef],
+        deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigUnionTypeDef],
         deploymentConfig: DeploymentConfigTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeploymentJobResponseTypeDef:
         """
         Deploys a specific version of a robot application to robots in a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_deployment_job)
@@ -312,19 +312,19 @@
         *,
         maxJobDurationInSeconds: int,
         iamRole: str,
         clientRequestToken: str = ...,
         outputLocation: OutputLocationTypeDef = ...,
         loggingConfig: LoggingConfigTypeDef = ...,
         failureBehavior: FailureBehaviorType = ...,
-        robotApplications: Sequence[RobotApplicationConfigTypeDef] = ...,
-        simulationApplications: Sequence[SimulationApplicationConfigTypeDef] = ...,
-        dataSources: Sequence[DataSourceConfigTypeDef] = ...,
+        robotApplications: Sequence[RobotApplicationConfigUnionTypeDef] = ...,
+        simulationApplications: Sequence[SimulationApplicationConfigUnionTypeDef] = ...,
+        dataSources: Sequence[DataSourceConfigUnionTypeDef] = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfig: VPCConfigTypeDef = ...,
+        vpcConfig: VPCConfigUnionTypeDef = ...,
         compute: ComputeTypeDef = ...
     ) -> CreateSimulationJobResponseTypeDef:
         """
         Creates a simulation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_simulation_job)
@@ -660,15 +660,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.restart_simulation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#restart_simulation_job)
         """
     async def start_simulation_job_batch(
         self,
         *,
-        createSimulationJobRequests: Sequence[SimulationJobRequestTypeDef],
+        createSimulationJobRequests: Sequence[SimulationJobRequestUnionTypeDef],
         clientRequestToken: str = ...,
         batchPolicy: BatchPolicyTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSimulationJobBatchResponseTypeDef:
         """
         Starts a new simulation job batch.
```

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/literals.py` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/literals.pyi` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/paginator.py` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listdeploymentjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListDeploymentJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listdeploymentjobspaginator)
         """
 
 
@@ -110,15 +110,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listfleetspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListFleets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listfleetspaginator)
         """
 
 
@@ -129,15 +129,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRobotApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobotApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listrobotapplicationspaginator)
         """
 
 
@@ -147,15 +147,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listrobotspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRobotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listrobotspaginator)
         """
 
 
@@ -166,15 +166,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSimulationApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationapplicationspaginator)
         """
 
 
@@ -184,15 +184,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobbatchespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSimulationJobBatchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobBatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobbatchespaginator)
         """
 
 
@@ -202,15 +202,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSimulationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobspaginator)
         """
 
 
@@ -220,15 +220,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorldExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldexportjobspaginator)
         """
 
 
@@ -238,30 +238,30 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldgenerationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorldGenerationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldGenerationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldgenerationjobspaginator)
         """
 
 
 class ListWorldTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorldTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldtemplatespaginator)
         """
 
 
@@ -271,13 +271,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorldsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorlds.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldspaginator)
         """
```

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/paginator.pyi` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listdeploymentjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListDeploymentJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listdeploymentjobspaginator)
         """
 
 class ListFleetsPaginator(AioPaginator):
@@ -106,15 +106,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listfleetspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListFleets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listfleetspaginator)
         """
 
 class ListRobotApplicationsPaginator(AioPaginator):
@@ -124,15 +124,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRobotApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobotApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listrobotapplicationspaginator)
         """
 
 class ListRobotsPaginator(AioPaginator):
@@ -141,15 +141,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listrobotspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRobotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListRobots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listrobotspaginator)
         """
 
 class ListSimulationApplicationsPaginator(AioPaginator):
@@ -159,15 +159,15 @@
     """
 
     def paginate(
         self,
         *,
         versionQualifier: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSimulationApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationapplicationspaginator)
         """
 
 class ListSimulationJobBatchesPaginator(AioPaginator):
@@ -176,15 +176,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobbatchespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSimulationJobBatchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobBatches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobbatchespaginator)
         """
 
 class ListSimulationJobsPaginator(AioPaginator):
@@ -193,15 +193,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSimulationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListSimulationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listsimulationjobspaginator)
         """
 
 class ListWorldExportJobsPaginator(AioPaginator):
@@ -210,15 +210,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorldExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldexportjobspaginator)
         """
 
 class ListWorldGenerationJobsPaginator(AioPaginator):
@@ -227,29 +227,29 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldgenerationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorldGenerationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldGenerationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldgenerationjobspaginator)
         """
 
 class ListWorldTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorldTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorldTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldtemplatespaginator)
         """
 
 class ListWorldsPaginator(AioPaginator):
@@ -258,13 +258,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWorldsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Paginator.ListWorlds.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/paginators/#listworldspaginator)
         """
```

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/type_defs.py` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_robomaker.type_defs import BatchDeleteWorldsRequestRequestTypeDef
 
-    data: BatchDeleteWorldsRequestRequestTypeDef = {...}
+    data: BatchDeleteWorldsRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ArchitectureType,
     ComputeTypeType,
     DataSourceTypeType,
     DeploymentJobErrorCodeType,
     DeploymentStatusType,
@@ -46,96 +46,98 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchDeleteWorldsRequestRequestTypeDef",
-    "BatchDeleteWorldsResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     "BatchPolicyTypeDef",
     "CancelDeploymentJobRequestRequestTypeDef",
     "CancelSimulationJobBatchRequestRequestTypeDef",
     "CancelSimulationJobRequestRequestTypeDef",
     "CancelWorldExportJobRequestRequestTypeDef",
     "CancelWorldGenerationJobRequestRequestTypeDef",
     "ComputeResponseTypeDef",
     "ComputeTypeDef",
     "CreateFleetRequestRequestTypeDef",
-    "CreateFleetResponseTypeDef",
     "EnvironmentTypeDef",
     "RobotSoftwareSuiteTypeDef",
     "SourceConfigTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
-    "CreateRobotResponseTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
-    "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
     "TemplateLocationTypeDef",
-    "CreateWorldTemplateResponseTypeDef",
+    "DataSourceConfigOutputTypeDef",
+    "DataSourceConfigTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
+    "DeploymentLaunchConfigOutputTypeDef",
     "DeploymentLaunchConfigTypeDef",
     "S3ObjectTypeDef",
     "DeregisterRobotRequestRequestTypeDef",
-    "DeregisterRobotResponseTypeDef",
     "DescribeDeploymentJobRequestRequestTypeDef",
     "DescribeFleetRequestRequestTypeDef",
     "RobotTypeDef",
     "DescribeRobotApplicationRequestRequestTypeDef",
     "DescribeRobotRequestRequestTypeDef",
-    "DescribeRobotResponseTypeDef",
     "DescribeSimulationApplicationRequestRequestTypeDef",
     "DescribeSimulationJobBatchRequestRequestTypeDef",
     "SimulationJobSummaryTypeDef",
     "DescribeSimulationJobRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeWorldExportJobRequestRequestTypeDef",
     "DescribeWorldGenerationJobRequestRequestTypeDef",
     "DescribeWorldRequestRequestTypeDef",
-    "DescribeWorldResponseTypeDef",
     "DescribeWorldTemplateRequestRequestTypeDef",
-    "DescribeWorldTemplateResponseTypeDef",
     "WorldFailureTypeDef",
     "FilterTypeDef",
     "FleetTypeDef",
     "GetWorldTemplateBodyRequestRequestTypeDef",
-    "GetWorldTemplateBodyResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "SimulationJobBatchSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
     "ListWorldTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "WorldSummaryTypeDef",
-    "PaginatorConfigTypeDef",
     "PortMappingTypeDef",
     "ProgressDetailTypeDef",
     "RegisterRobotRequestRequestTypeDef",
-    "RegisterRobotResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RestartSimulationJobRequestRequestTypeDef",
     "ToolTypeDef",
     "UploadConfigurationTypeDef",
     "WorldConfigTypeDef",
+    "VPCConfigOutputTypeDef",
     "SyncDeploymentJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "BatchDeleteWorldsResponseTypeDef",
+    "CreateFleetResponseTypeDef",
+    "CreateRobotResponseTypeDef",
+    "CreateWorldTemplateResponseTypeDef",
+    "DeregisterRobotResponseTypeDef",
+    "DescribeRobotResponseTypeDef",
+    "DescribeWorldResponseTypeDef",
+    "DescribeWorldTemplateResponseTypeDef",
+    "GetWorldTemplateBodyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterRobotResponseTypeDef",
     "UpdateWorldTemplateResponseTypeDef",
     "RobotApplicationSummaryTypeDef",
     "CreateRobotApplicationRequestRequestTypeDef",
     "UpdateRobotApplicationRequestRequestTypeDef",
     "CreateRobotApplicationResponseTypeDef",
     "CreateRobotApplicationVersionResponseTypeDef",
     "DescribeRobotApplicationResponseTypeDef",
@@ -152,86 +154,102 @@
     "DescribeWorldExportJobResponseTypeDef",
     "WorldExportJobSummaryTypeDef",
     "CreateWorldGenerationJobRequestRequestTypeDef",
     "CreateWorldGenerationJobResponseTypeDef",
     "WorldGenerationJobSummaryTypeDef",
     "CreateWorldTemplateRequestRequestTypeDef",
     "UpdateWorldTemplateRequestRequestTypeDef",
+    "DataSourceConfigUnionTypeDef",
     "DataSourceTypeDef",
+    "DeploymentApplicationConfigOutputTypeDef",
     "DeploymentApplicationConfigTypeDef",
     "DeploymentConfigTypeDef",
     "DescribeFleetResponseTypeDef",
     "ListRobotsResponseTypeDef",
     "ListSimulationJobsResponseTypeDef",
     "FailureSummaryTypeDef",
-    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
     "ListDeploymentJobsRequestRequestTypeDef",
-    "ListFleetsRequestListFleetsPaginateTypeDef",
     "ListFleetsRequestRequestTypeDef",
-    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
     "ListRobotApplicationsRequestRequestTypeDef",
-    "ListRobotsRequestListRobotsPaginateTypeDef",
     "ListRobotsRequestRequestTypeDef",
-    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
     "ListSimulationApplicationsRequestRequestTypeDef",
-    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
     "ListSimulationJobBatchesRequestRequestTypeDef",
-    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
     "ListSimulationJobsRequestRequestTypeDef",
-    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     "ListWorldExportJobsRequestRequestTypeDef",
-    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     "ListWorldGenerationJobsRequestRequestTypeDef",
-    "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListWorldsRequestRequestTypeDef",
     "ListFleetsResponseTypeDef",
+    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
+    "ListFleetsRequestListFleetsPaginateTypeDef",
+    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
+    "ListRobotsRequestListRobotsPaginateTypeDef",
+    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
+    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
+    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
+    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
+    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
+    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
+    "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListSimulationJobBatchesResponseTypeDef",
     "ListWorldTemplatesResponseTypeDef",
     "ListWorldsResponseTypeDef",
+    "PortForwardingConfigOutputTypeDef",
     "PortForwardingConfigTypeDef",
     "RobotDeploymentTypeDef",
+    "VPCConfigUnionTypeDef",
     "ListRobotApplicationsResponseTypeDef",
     "ListSimulationApplicationsResponseTypeDef",
     "ListWorldExportJobsResponseTypeDef",
     "ListWorldGenerationJobsResponseTypeDef",
-    "CreateDeploymentJobRequestRequestTypeDef",
+    "DeploymentApplicationConfigUnionTypeDef",
     "CreateDeploymentJobResponseTypeDef",
     "DeploymentJobTypeDef",
     "SyncDeploymentJobResponseTypeDef",
     "FinishedWorldsSummaryTypeDef",
+    "LaunchConfigOutputTypeDef",
     "LaunchConfigTypeDef",
     "DescribeDeploymentJobResponseTypeDef",
+    "CreateDeploymentJobRequestRequestTypeDef",
     "ListDeploymentJobsResponseTypeDef",
     "DescribeWorldGenerationJobResponseTypeDef",
+    "RobotApplicationConfigOutputTypeDef",
+    "SimulationApplicationConfigOutputTypeDef",
     "RobotApplicationConfigTypeDef",
     "SimulationApplicationConfigTypeDef",
-    "CreateSimulationJobRequestRequestTypeDef",
     "CreateSimulationJobResponseTypeDef",
     "DescribeSimulationJobResponseTypeDef",
-    "SimulationJobRequestTypeDef",
+    "SimulationJobRequestOutputTypeDef",
     "SimulationJobTypeDef",
+    "RobotApplicationConfigUnionTypeDef",
+    "SimulationApplicationConfigUnionTypeDef",
+    "SimulationJobRequestTypeDef",
     "FailedCreateSimulationJobRequestTypeDef",
-    "StartSimulationJobBatchRequestRequestTypeDef",
     "BatchDescribeSimulationJobResponseTypeDef",
+    "CreateSimulationJobRequestRequestTypeDef",
+    "SimulationJobRequestUnionTypeDef",
     "DescribeSimulationJobBatchResponseTypeDef",
     "StartSimulationJobBatchResponseTypeDef",
+    "StartSimulationJobBatchRequestRequestTypeDef",
 )
 
 BatchDeleteWorldsRequestRequestTypeDef = TypedDict(
     "BatchDeleteWorldsRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
     },
 )
 
-BatchDeleteWorldsResponseTypeDef = TypedDict(
-    "BatchDeleteWorldsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "unprocessedWorlds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BatchDescribeSimulationJobRequestRequestTypeDef = TypedDict(
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     {
         "jobs": Sequence[str],
@@ -319,25 +337,14 @@
 
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
 
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "uri": str,
     },
     total=False,
 )
@@ -415,27 +422,14 @@
 
 class CreateRobotRequestRequestTypeDef(
     _RequiredCreateRobotRequestRequestTypeDef, _OptionalCreateRobotRequestRequestTypeDef
 ):
     pass
 
 
-CreateRobotResponseTypeDef = TypedDict(
-    "CreateRobotResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "createdAt": datetime,
-        "greengrassGroupId": str,
-        "architecture": ArchitectureType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RenderingEngineTypeDef = TypedDict(
     "RenderingEngineTypeDef",
     {
         "name": Literal["OGRE"],
         "version": str,
     },
     total=False,
@@ -470,36 +464,14 @@
 class CreateSimulationApplicationVersionRequestRequestTypeDef(
     _RequiredCreateSimulationApplicationVersionRequestRequestTypeDef,
     _OptionalCreateSimulationApplicationVersionRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDataSourceConfigTypeDef = TypedDict(
-    "_RequiredDataSourceConfigTypeDef",
-    {
-        "name": str,
-        "s3Bucket": str,
-        "s3Keys": Sequence[str],
-    },
-)
-_OptionalDataSourceConfigTypeDef = TypedDict(
-    "_OptionalDataSourceConfigTypeDef",
-    {
-        "type": DataSourceTypeType,
-        "destination": str,
-    },
-    total=False,
-)
-
-
-class DataSourceConfigTypeDef(_RequiredDataSourceConfigTypeDef, _OptionalDataSourceConfigTypeDef):
-    pass
-
-
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "recordAllRosTopics": bool,
     },
     total=False,
 )
@@ -557,26 +529,60 @@
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
 
-CreateWorldTemplateResponseTypeDef = TypedDict(
-    "CreateWorldTemplateResponseTypeDef",
+_RequiredDataSourceConfigOutputTypeDef = TypedDict(
+    "_RequiredDataSourceConfigOutputTypeDef",
     {
-        "arn": str,
-        "clientRequestToken": str,
-        "createdAt": datetime,
         "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "s3Bucket": str,
+        "s3Keys": List[str],
+    },
+)
+_OptionalDataSourceConfigOutputTypeDef = TypedDict(
+    "_OptionalDataSourceConfigOutputTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
     },
+    total=False,
 )
 
+
+class DataSourceConfigOutputTypeDef(
+    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
+):
+    pass
+
+
+_RequiredDataSourceConfigTypeDef = TypedDict(
+    "_RequiredDataSourceConfigTypeDef",
+    {
+        "name": str,
+        "s3Bucket": str,
+        "s3Keys": Sequence[str],
+    },
+)
+_OptionalDataSourceConfigTypeDef = TypedDict(
+    "_OptionalDataSourceConfigTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
+    },
+    total=False,
+)
+
+
+class DataSourceConfigTypeDef(_RequiredDataSourceConfigTypeDef, _OptionalDataSourceConfigTypeDef):
+    pass
+
+
 S3KeyOutputTypeDef = TypedDict(
     "S3KeyOutputTypeDef",
     {
         "s3Key": str,
         "etag": str,
     },
     total=False,
@@ -643,14 +649,38 @@
 DeleteWorldTemplateRequestRequestTypeDef = TypedDict(
     "DeleteWorldTemplateRequestRequestTypeDef",
     {
         "template": str,
     },
 )
 
+_RequiredDeploymentLaunchConfigOutputTypeDef = TypedDict(
+    "_RequiredDeploymentLaunchConfigOutputTypeDef",
+    {
+        "packageName": str,
+        "launchFile": str,
+    },
+)
+_OptionalDeploymentLaunchConfigOutputTypeDef = TypedDict(
+    "_OptionalDeploymentLaunchConfigOutputTypeDef",
+    {
+        "preLaunchFile": str,
+        "postLaunchFile": str,
+        "environmentVariables": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class DeploymentLaunchConfigOutputTypeDef(
+    _RequiredDeploymentLaunchConfigOutputTypeDef, _OptionalDeploymentLaunchConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredDeploymentLaunchConfigTypeDef = TypedDict(
     "_RequiredDeploymentLaunchConfigTypeDef",
     {
         "packageName": str,
         "launchFile": str,
     },
 )
@@ -695,23 +725,14 @@
     "DeregisterRobotRequestRequestTypeDef",
     {
         "fleet": str,
         "robot": str,
     },
 )
 
-DeregisterRobotResponseTypeDef = TypedDict(
-    "DeregisterRobotResponseTypeDef",
-    {
-        "fleet": str,
-        "robot": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeploymentJobRequestRequestTypeDef = TypedDict(
     "DescribeDeploymentJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
@@ -763,31 +784,14 @@
 DescribeRobotRequestRequestTypeDef = TypedDict(
     "DescribeRobotRequestRequestTypeDef",
     {
         "robot": str,
     },
 )
 
-DescribeRobotResponseTypeDef = TypedDict(
-    "DescribeRobotResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "fleetArn": str,
-        "status": RobotStatusType,
-        "greengrassGroupId": str,
-        "createdAt": datetime,
-        "architecture": ArchitectureType,
-        "lastDeploymentJob": str,
-        "lastDeploymentTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSimulationApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalDescribeSimulationApplicationRequestRequestTypeDef = TypedDict(
@@ -862,48 +866,21 @@
 DescribeWorldRequestRequestTypeDef = TypedDict(
     "DescribeWorldRequestRequestTypeDef",
     {
         "world": str,
     },
 )
 
-DescribeWorldResponseTypeDef = TypedDict(
-    "DescribeWorldResponseTypeDef",
-    {
-        "arn": str,
-        "generationJob": str,
-        "template": str,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-        "worldDescriptionBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeWorldTemplateRequestRequestTypeDef = TypedDict(
     "DescribeWorldTemplateRequestRequestTypeDef",
     {
         "template": str,
     },
 )
 
-DescribeWorldTemplateResponseTypeDef = TypedDict(
-    "DescribeWorldTemplateResponseTypeDef",
-    {
-        "arn": str,
-        "clientRequestToken": str,
-        "name": str,
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "tags": Dict[str, str],
-        "version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorldFailureTypeDef = TypedDict(
     "WorldFailureTypeDef",
     {
         "failureCode": WorldGenerationJobErrorCodeType,
         "sampleFailureReason": str,
         "failureCount": int,
     },
@@ -937,20 +914,22 @@
     {
         "template": str,
         "generationJob": str,
     },
     total=False,
 )
 
-GetWorldTemplateBodyResponseTypeDef = TypedDict(
-    "GetWorldTemplateBodyResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "templateBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
 SimulationJobBatchSummaryTypeDef = TypedDict(
     "SimulationJobBatchSummaryTypeDef",
     {
         "arn": str,
         "lastUpdatedAt": datetime,
@@ -966,30 +945,14 @@
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
-ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = TypedDict(
-    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorldTemplatesRequestRequestTypeDef = TypedDict(
     "ListWorldTemplatesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -1014,24 +977,14 @@
         "createdAt": datetime,
         "generationJob": str,
         "template": str,
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
 _RequiredPortMappingTypeDef = TypedDict(
     "_RequiredPortMappingTypeDef",
     {
         "jobPort": int,
         "applicationPort": int,
     },
 )
@@ -1063,34 +1016,14 @@
     "RegisterRobotRequestRequestTypeDef",
     {
         "fleet": str,
         "robot": str,
     },
 )
 
-RegisterRobotResponseTypeDef = TypedDict(
-    "RegisterRobotResponseTypeDef",
-    {
-        "fleet": str,
-        "robot": str,
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
 RestartSimulationJobRequestRequestTypeDef = TypedDict(
     "RestartSimulationJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
@@ -1129,14 +1062,34 @@
     "WorldConfigTypeDef",
     {
         "world": str,
     },
     total=False,
 )
 
+_RequiredVPCConfigOutputTypeDef = TypedDict(
+    "_RequiredVPCConfigOutputTypeDef",
+    {
+        "subnets": List[str],
+    },
+)
+_OptionalVPCConfigOutputTypeDef = TypedDict(
+    "_OptionalVPCConfigOutputTypeDef",
+    {
+        "securityGroups": List[str],
+        "assignPublicIp": bool,
+    },
+    total=False,
+)
+
+
+class VPCConfigOutputTypeDef(_RequiredVPCConfigOutputTypeDef, _OptionalVPCConfigOutputTypeDef):
+    pass
+
+
 SyncDeploymentJobRequestRequestTypeDef = TypedDict(
     "SyncDeploymentJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
         "fleet": str,
     },
 )
@@ -1153,22 +1106,144 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+BatchDeleteWorldsResponseTypeDef = TypedDict(
+    "BatchDeleteWorldsResponseTypeDef",
+    {
+        "unprocessedWorlds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "createdAt": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRobotResponseTypeDef = TypedDict(
+    "CreateRobotResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "createdAt": datetime,
+        "greengrassGroupId": str,
+        "architecture": ArchitectureType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorldTemplateResponseTypeDef = TypedDict(
+    "CreateWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "clientRequestToken": str,
+        "createdAt": datetime,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterRobotResponseTypeDef = TypedDict(
+    "DeregisterRobotResponseTypeDef",
+    {
+        "fleet": str,
+        "robot": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRobotResponseTypeDef = TypedDict(
+    "DescribeRobotResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "fleetArn": str,
+        "status": RobotStatusType,
+        "greengrassGroupId": str,
+        "createdAt": datetime,
+        "architecture": ArchitectureType,
+        "lastDeploymentJob": str,
+        "lastDeploymentTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorldResponseTypeDef = TypedDict(
+    "DescribeWorldResponseTypeDef",
+    {
+        "arn": str,
+        "generationJob": str,
+        "template": str,
+        "createdAt": datetime,
+        "tags": Dict[str, str],
+        "worldDescriptionBody": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorldTemplateResponseTypeDef = TypedDict(
+    "DescribeWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "clientRequestToken": str,
+        "name": str,
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "tags": Dict[str, str],
+        "version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorldTemplateBodyResponseTypeDef = TypedDict(
+    "GetWorldTemplateBodyResponseTypeDef",
+    {
+        "templateBody": str,
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
+RegisterRobotResponseTypeDef = TypedDict(
+    "RegisterRobotResponseTypeDef",
+    {
+        "fleet": str,
+        "robot": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateWorldTemplateResponseTypeDef = TypedDict(
     "UpdateWorldTemplateResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RobotApplicationSummaryTypeDef = TypedDict(
     "RobotApplicationSummaryTypeDef",
     {
         "name": str,
@@ -1238,30 +1313,30 @@
         "version": str,
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRobotApplicationVersionResponseTypeDef = TypedDict(
     "CreateRobotApplicationVersionResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRobotApplicationResponseTypeDef = TypedDict(
     "DescribeRobotApplicationResponseTypeDef",
     {
         "arn": str,
@@ -1270,30 +1345,30 @@
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
         "imageDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRobotApplicationResponseTypeDef = TypedDict(
     "UpdateRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSimulationApplicationRequestRequestTypeDef",
     {
         "name": str,
@@ -1330,15 +1405,15 @@
         "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSimulationApplicationVersionResponseTypeDef = TypedDict(
     "CreateSimulationApplicationVersionResponseTypeDef",
     {
         "arn": str,
@@ -1347,15 +1422,15 @@
         "sources": List[SourceTypeDef],
         "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationApplicationResponseTypeDef = TypedDict(
     "DescribeSimulationApplicationResponseTypeDef",
     {
         "arn": str,
@@ -1366,15 +1441,15 @@
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
         "imageDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SimulationApplicationSummaryTypeDef = TypedDict(
     "SimulationApplicationSummaryTypeDef",
     {
         "name": str,
@@ -1423,15 +1498,15 @@
         "sources": List[SourceTypeDef],
         "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWorldExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorldExportJobRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
@@ -1463,15 +1538,15 @@
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldExportJobErrorCodeType,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorldExportJobResponseTypeDef = TypedDict(
     "DescribeWorldExportJobResponseTypeDef",
     {
         "arn": str,
@@ -1480,15 +1555,15 @@
         "failureCode": WorldExportJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
         "worlds": List[str],
         "outputLocation": OutputLocationTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorldExportJobSummaryTypeDef = TypedDict(
     "WorldExportJobSummaryTypeDef",
     {
         "arn": str,
@@ -1533,15 +1608,15 @@
         "createdAt": datetime,
         "failureCode": WorldGenerationJobErrorCodeType,
         "clientRequestToken": str,
         "template": str,
         "worldCount": WorldCountTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorldGenerationJobSummaryTypeDef = TypedDict(
     "WorldGenerationJobSummaryTypeDef",
     {
         "arn": str,
@@ -1587,26 +1662,36 @@
 class UpdateWorldTemplateRequestRequestTypeDef(
     _RequiredUpdateWorldTemplateRequestRequestTypeDef,
     _OptionalUpdateWorldTemplateRequestRequestTypeDef,
 ):
     pass
 
 
+DataSourceConfigUnionTypeDef = Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "name": str,
         "s3Bucket": str,
         "s3Keys": List[S3KeyOutputTypeDef],
         "type": DataSourceTypeType,
         "destination": str,
     },
     total=False,
 )
 
+DeploymentApplicationConfigOutputTypeDef = TypedDict(
+    "DeploymentApplicationConfigOutputTypeDef",
+    {
+        "application": str,
+        "applicationVersion": str,
+        "launchConfig": DeploymentLaunchConfigOutputTypeDef,
+    },
+)
+
 DeploymentApplicationConfigTypeDef = TypedDict(
     "DeploymentApplicationConfigTypeDef",
     {
         "application": str,
         "applicationVersion": str,
         "launchConfig": DeploymentLaunchConfigTypeDef,
     },
@@ -1630,279 +1715,295 @@
         "arn": str,
         "robots": List[RobotTypeDef],
         "createdAt": datetime,
         "lastDeploymentStatus": DeploymentStatusType,
         "lastDeploymentJob": str,
         "lastDeploymentTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRobotsResponseTypeDef = TypedDict(
     "ListRobotsResponseTypeDef",
     {
         "robots": List[RobotTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSimulationJobsResponseTypeDef = TypedDict(
     "ListSimulationJobsResponseTypeDef",
     {
         "simulationJobSummaries": List[SimulationJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailureSummaryTypeDef = TypedDict(
     "FailureSummaryTypeDef",
     {
         "totalFailureCount": int,
         "failures": List[WorldFailureTypeDef],
     },
     total=False,
 )
 
-ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = TypedDict(
-    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
+ListDeploymentJobsRequestRequestTypeDef = TypedDict(
+    "ListDeploymentJobsRequestRequestTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-ListDeploymentJobsRequestRequestTypeDef = TypedDict(
-    "ListDeploymentJobsRequestRequestTypeDef",
+ListFleetsRequestRequestTypeDef = TypedDict(
+    "ListFleetsRequestRequestTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
         "nextToken": str,
         "maxResults": int,
+        "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
-    "ListFleetsRequestListFleetsPaginateTypeDef",
+ListRobotApplicationsRequestRequestTypeDef = TypedDict(
+    "ListRobotApplicationsRequestRequestTypeDef",
     {
+        "versionQualifier": str,
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListFleetsRequestRequestTypeDef = TypedDict(
-    "ListFleetsRequestRequestTypeDef",
+ListRobotsRequestRequestTypeDef = TypedDict(
+    "ListRobotsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = TypedDict(
-    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
+ListSimulationApplicationsRequestRequestTypeDef = TypedDict(
+    "ListSimulationApplicationsRequestRequestTypeDef",
     {
         "versionQualifier": str,
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListRobotApplicationsRequestRequestTypeDef = TypedDict(
-    "ListRobotApplicationsRequestRequestTypeDef",
+ListSimulationJobBatchesRequestRequestTypeDef = TypedDict(
+    "ListSimulationJobBatchesRequestRequestTypeDef",
     {
-        "versionQualifier": str,
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListRobotsRequestListRobotsPaginateTypeDef = TypedDict(
-    "ListRobotsRequestListRobotsPaginateTypeDef",
+ListSimulationJobsRequestRequestTypeDef = TypedDict(
+    "ListSimulationJobsRequestRequestTypeDef",
     {
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListRobotsRequestRequestTypeDef = TypedDict(
-    "ListRobotsRequestRequestTypeDef",
+ListWorldExportJobsRequestRequestTypeDef = TypedDict(
+    "ListWorldExportJobsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = TypedDict(
-    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
+ListWorldGenerationJobsRequestRequestTypeDef = TypedDict(
+    "ListWorldGenerationJobsRequestRequestTypeDef",
     {
-        "versionQualifier": str,
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListSimulationApplicationsRequestRequestTypeDef = TypedDict(
-    "ListSimulationApplicationsRequestRequestTypeDef",
+ListWorldsRequestRequestTypeDef = TypedDict(
+    "ListWorldsRequestRequestTypeDef",
     {
-        "versionQualifier": str,
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = TypedDict(
-    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
+ListFleetsResponseTypeDef = TypedDict(
+    "ListFleetsResponseTypeDef",
+    {
+        "fleetDetails": List[FleetTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = TypedDict(
+    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobBatchesRequestRequestTypeDef = TypedDict(
-    "ListSimulationJobBatchesRequestRequestTypeDef",
+ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
+    "ListFleetsRequestListFleetsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = TypedDict(
-    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
+ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = TypedDict(
+    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
     {
+        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobsRequestRequestTypeDef = TypedDict(
-    "ListSimulationJobsRequestRequestTypeDef",
+ListRobotsRequestListRobotsPaginateTypeDef = TypedDict(
+    "ListRobotsRequestListRobotsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = TypedDict(
-    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
+ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = TypedDict(
+    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
     {
+        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldExportJobsRequestRequestTypeDef = TypedDict(
-    "ListWorldExportJobsRequestRequestTypeDef",
+ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = TypedDict(
+    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = TypedDict(
-    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
+ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = TypedDict(
+    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldGenerationJobsRequestRequestTypeDef = TypedDict(
-    "ListWorldGenerationJobsRequestRequestTypeDef",
+ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = TypedDict(
+    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldsRequestListWorldsPaginateTypeDef = TypedDict(
-    "ListWorldsRequestListWorldsPaginateTypeDef",
+ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = TypedDict(
+    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldsRequestRequestTypeDef = TypedDict(
-    "ListWorldsRequestRequestTypeDef",
+ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = TypedDict(
+    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
-        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListFleetsResponseTypeDef = TypedDict(
-    "ListFleetsResponseTypeDef",
+ListWorldsRequestListWorldsPaginateTypeDef = TypedDict(
+    "ListWorldsRequestListWorldsPaginateTypeDef",
     {
-        "fleetDetails": List[FleetTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListSimulationJobBatchesResponseTypeDef = TypedDict(
     "ListSimulationJobBatchesResponseTypeDef",
     {
         "simulationJobBatchSummaries": List[SimulationJobBatchSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldTemplatesResponseTypeDef = TypedDict(
     "ListWorldTemplatesResponseTypeDef",
     {
         "templateSummaries": List[TemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldsResponseTypeDef = TypedDict(
     "ListWorldsResponseTypeDef",
     {
         "worldSummaries": List[WorldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PortForwardingConfigOutputTypeDef = TypedDict(
+    "PortForwardingConfigOutputTypeDef",
+    {
+        "portMappings": List[PortMappingTypeDef],
     },
+    total=False,
 )
 
 PortForwardingConfigTypeDef = TypedDict(
     "PortForwardingConfigTypeDef",
     {
-        "portMappings": List[PortMappingTypeDef],
+        "portMappings": Sequence[PortMappingTypeDef],
     },
     total=False,
 )
 
 RobotDeploymentTypeDef = TypedDict(
     "RobotDeploymentTypeDef",
     {
@@ -1913,98 +2014,77 @@
         "progressDetail": ProgressDetailTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
     },
     total=False,
 )
 
+VPCConfigUnionTypeDef = Union[VPCConfigTypeDef, VPCConfigOutputTypeDef]
 ListRobotApplicationsResponseTypeDef = TypedDict(
     "ListRobotApplicationsResponseTypeDef",
     {
         "robotApplicationSummaries": List[RobotApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSimulationApplicationsResponseTypeDef = TypedDict(
     "ListSimulationApplicationsResponseTypeDef",
     {
         "simulationApplicationSummaries": List[SimulationApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldExportJobsResponseTypeDef = TypedDict(
     "ListWorldExportJobsResponseTypeDef",
     {
         "worldExportJobSummaries": List[WorldExportJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldGenerationJobsResponseTypeDef = TypedDict(
     "ListWorldGenerationJobsResponseTypeDef",
     {
         "worldGenerationJobSummaries": List[WorldGenerationJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "fleet": str,
-        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
-    },
-)
-_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDeploymentJobRequestRequestTypeDef(
-    _RequiredCreateDeploymentJobRequestRequestTypeDef,
-    _OptionalCreateDeploymentJobRequestRequestTypeDef,
-):
-    pass
-
-
+DeploymentApplicationConfigUnionTypeDef = Union[
+    DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef
+]
 CreateDeploymentJobResponseTypeDef = TypedDict(
     "CreateDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "deploymentConfig": DeploymentConfigTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentJobTypeDef = TypedDict(
     "DeploymentJobTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "deploymentConfig": DeploymentConfigTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
     },
     total=False,
 )
@@ -2012,68 +2092,106 @@
 SyncDeploymentJobResponseTypeDef = TypedDict(
     "SyncDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentConfig": DeploymentConfigTypeDef,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FinishedWorldsSummaryTypeDef = TypedDict(
     "FinishedWorldsSummaryTypeDef",
     {
         "finishedCount": int,
         "succeededWorlds": List[str],
         "failureSummary": FailureSummaryTypeDef,
     },
     total=False,
 )
 
+LaunchConfigOutputTypeDef = TypedDict(
+    "LaunchConfigOutputTypeDef",
+    {
+        "packageName": str,
+        "launchFile": str,
+        "environmentVariables": Dict[str, str],
+        "portForwardingConfig": PortForwardingConfigOutputTypeDef,
+        "streamUI": bool,
+        "command": List[str],
+    },
+    total=False,
+)
+
 LaunchConfigTypeDef = TypedDict(
     "LaunchConfigTypeDef",
     {
         "packageName": str,
         "launchFile": str,
-        "environmentVariables": Dict[str, str],
+        "environmentVariables": Mapping[str, str],
         "portForwardingConfig": PortForwardingConfigTypeDef,
         "streamUI": bool,
-        "command": List[str],
+        "command": Sequence[str],
     },
     total=False,
 )
 
 DescribeDeploymentJobResponseTypeDef = TypedDict(
     "DescribeDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentConfig": DeploymentConfigTypeDef,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "robotDeploymentSummary": List[RobotDeploymentTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "fleet": str,
+        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigUnionTypeDef],
+    },
+)
+_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "deploymentConfig": DeploymentConfigTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDeploymentJobRequestRequestTypeDef(
+    _RequiredCreateDeploymentJobRequestRequestTypeDef,
+    _OptionalCreateDeploymentJobRequestRequestTypeDef,
+):
+    pass
+
+
 ListDeploymentJobsResponseTypeDef = TypedDict(
     "ListDeploymentJobsResponseTypeDef",
     {
         "deploymentJobs": List[DeploymentJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorldGenerationJobResponseTypeDef = TypedDict(
     "DescribeWorldGenerationJobResponseTypeDef",
     {
         "arn": str,
@@ -2083,99 +2201,121 @@
         "failureReason": str,
         "clientRequestToken": str,
         "template": str,
         "worldCount": WorldCountTypeDef,
         "finishedWorldsSummary": FinishedWorldsSummaryTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRobotApplicationConfigTypeDef = TypedDict(
-    "_RequiredRobotApplicationConfigTypeDef",
+_RequiredRobotApplicationConfigOutputTypeDef = TypedDict(
+    "_RequiredRobotApplicationConfigOutputTypeDef",
     {
         "application": str,
-        "launchConfig": LaunchConfigTypeDef,
+        "launchConfig": LaunchConfigOutputTypeDef,
     },
 )
-_OptionalRobotApplicationConfigTypeDef = TypedDict(
-    "_OptionalRobotApplicationConfigTypeDef",
+_OptionalRobotApplicationConfigOutputTypeDef = TypedDict(
+    "_OptionalRobotApplicationConfigOutputTypeDef",
     {
         "applicationVersion": str,
         "uploadConfigurations": List[UploadConfigurationTypeDef],
         "useDefaultUploadConfigurations": bool,
         "tools": List[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
 
-class RobotApplicationConfigTypeDef(
-    _RequiredRobotApplicationConfigTypeDef, _OptionalRobotApplicationConfigTypeDef
+class RobotApplicationConfigOutputTypeDef(
+    _RequiredRobotApplicationConfigOutputTypeDef, _OptionalRobotApplicationConfigOutputTypeDef
 ):
     pass
 
 
-_RequiredSimulationApplicationConfigTypeDef = TypedDict(
-    "_RequiredSimulationApplicationConfigTypeDef",
+_RequiredSimulationApplicationConfigOutputTypeDef = TypedDict(
+    "_RequiredSimulationApplicationConfigOutputTypeDef",
     {
         "application": str,
-        "launchConfig": LaunchConfigTypeDef,
+        "launchConfig": LaunchConfigOutputTypeDef,
     },
 )
-_OptionalSimulationApplicationConfigTypeDef = TypedDict(
-    "_OptionalSimulationApplicationConfigTypeDef",
+_OptionalSimulationApplicationConfigOutputTypeDef = TypedDict(
+    "_OptionalSimulationApplicationConfigOutputTypeDef",
     {
         "applicationVersion": str,
         "uploadConfigurations": List[UploadConfigurationTypeDef],
         "worldConfigs": List[WorldConfigTypeDef],
         "useDefaultUploadConfigurations": bool,
         "tools": List[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
 
-class SimulationApplicationConfigTypeDef(
-    _RequiredSimulationApplicationConfigTypeDef, _OptionalSimulationApplicationConfigTypeDef
+class SimulationApplicationConfigOutputTypeDef(
+    _RequiredSimulationApplicationConfigOutputTypeDef,
+    _OptionalSimulationApplicationConfigOutputTypeDef,
 ):
     pass
 
 
-_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSimulationJobRequestRequestTypeDef",
+_RequiredRobotApplicationConfigTypeDef = TypedDict(
+    "_RequiredRobotApplicationConfigTypeDef",
     {
-        "maxJobDurationInSeconds": int,
-        "iamRole": str,
+        "application": str,
+        "launchConfig": LaunchConfigTypeDef,
     },
 )
-_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSimulationJobRequestRequestTypeDef",
+_OptionalRobotApplicationConfigTypeDef = TypedDict(
+    "_OptionalRobotApplicationConfigTypeDef",
     {
-        "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
-        "failureBehavior": FailureBehaviorType,
-        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
-        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
-        "dataSources": Sequence[DataSourceConfigTypeDef],
-        "tags": Mapping[str, str],
-        "vpcConfig": VPCConfigTypeDef,
-        "compute": ComputeTypeDef,
+        "applicationVersion": str,
+        "uploadConfigurations": Sequence[UploadConfigurationTypeDef],
+        "useDefaultUploadConfigurations": bool,
+        "tools": Sequence[ToolTypeDef],
+        "useDefaultTools": bool,
     },
     total=False,
 )
 
 
-class CreateSimulationJobRequestRequestTypeDef(
-    _RequiredCreateSimulationJobRequestRequestTypeDef,
-    _OptionalCreateSimulationJobRequestRequestTypeDef,
+class RobotApplicationConfigTypeDef(
+    _RequiredRobotApplicationConfigTypeDef, _OptionalRobotApplicationConfigTypeDef
+):
+    pass
+
+
+_RequiredSimulationApplicationConfigTypeDef = TypedDict(
+    "_RequiredSimulationApplicationConfigTypeDef",
+    {
+        "application": str,
+        "launchConfig": LaunchConfigTypeDef,
+    },
+)
+_OptionalSimulationApplicationConfigTypeDef = TypedDict(
+    "_OptionalSimulationApplicationConfigTypeDef",
+    {
+        "applicationVersion": str,
+        "uploadConfigurations": Sequence[UploadConfigurationTypeDef],
+        "worldConfigs": Sequence[WorldConfigTypeDef],
+        "useDefaultUploadConfigurations": bool,
+        "tools": Sequence[ToolTypeDef],
+        "useDefaultTools": bool,
+    },
+    total=False,
+)
+
+
+class SimulationApplicationConfigTypeDef(
+    _RequiredSimulationApplicationConfigTypeDef, _OptionalSimulationApplicationConfigTypeDef
 ):
     pass
 
 
 CreateSimulationJobResponseTypeDef = TypedDict(
     "CreateSimulationJobResponseTypeDef",
     {
@@ -2187,21 +2327,21 @@
         "failureCode": SimulationJobErrorCodeType,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "compute": ComputeResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationJobResponseTypeDef = TypedDict(
     "DescribeSimulationJobResponseTypeDef",
     {
         "arn": str,
@@ -2214,52 +2354,52 @@
         "failureReason": str,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSimulationJobRequestTypeDef = TypedDict(
-    "_RequiredSimulationJobRequestTypeDef",
+_RequiredSimulationJobRequestOutputTypeDef = TypedDict(
+    "_RequiredSimulationJobRequestOutputTypeDef",
     {
         "maxJobDurationInSeconds": int,
     },
 )
-_OptionalSimulationJobRequestTypeDef = TypedDict(
-    "_OptionalSimulationJobRequestTypeDef",
+_OptionalSimulationJobRequestOutputTypeDef = TypedDict(
+    "_OptionalSimulationJobRequestOutputTypeDef",
     {
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "iamRole": str,
         "failureBehavior": FailureBehaviorType,
         "useDefaultApplications": bool,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
-        "dataSources": List[DataSourceConfigTypeDef],
-        "vpcConfig": VPCConfigTypeDef,
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
+        "dataSources": List[DataSourceConfigOutputTypeDef],
+        "vpcConfig": VPCConfigOutputTypeDef,
         "compute": ComputeTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class SimulationJobRequestTypeDef(
-    _RequiredSimulationJobRequestTypeDef, _OptionalSimulationJobRequestTypeDef
+class SimulationJobRequestOutputTypeDef(
+    _RequiredSimulationJobRequestOutputTypeDef, _OptionalSimulationJobRequestOutputTypeDef
 ):
     pass
 
 
 SimulationJobTypeDef = TypedDict(
     "SimulationJobTypeDef",
     {
@@ -2273,98 +2413,169 @@
         "failureReason": str,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
     },
     total=False,
 )
 
+RobotApplicationConfigUnionTypeDef = Union[
+    RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef
+]
+SimulationApplicationConfigUnionTypeDef = Union[
+    SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef
+]
+_RequiredSimulationJobRequestTypeDef = TypedDict(
+    "_RequiredSimulationJobRequestTypeDef",
+    {
+        "maxJobDurationInSeconds": int,
+    },
+)
+_OptionalSimulationJobRequestTypeDef = TypedDict(
+    "_OptionalSimulationJobRequestTypeDef",
+    {
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
+        "iamRole": str,
+        "failureBehavior": FailureBehaviorType,
+        "useDefaultApplications": bool,
+        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
+        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
+        "dataSources": Sequence[DataSourceConfigTypeDef],
+        "vpcConfig": VPCConfigTypeDef,
+        "compute": ComputeTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class SimulationJobRequestTypeDef(
+    _RequiredSimulationJobRequestTypeDef, _OptionalSimulationJobRequestTypeDef
+):
+    pass
+
+
 FailedCreateSimulationJobRequestTypeDef = TypedDict(
     "FailedCreateSimulationJobRequestTypeDef",
     {
-        "request": SimulationJobRequestTypeDef,
+        "request": SimulationJobRequestOutputTypeDef,
         "failureReason": str,
         "failureCode": SimulationJobErrorCodeType,
         "failedAt": datetime,
     },
     total=False,
 )
 
-_RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
-    "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
+BatchDescribeSimulationJobResponseTypeDef = TypedDict(
+    "BatchDescribeSimulationJobResponseTypeDef",
     {
-        "createSimulationJobRequests": Sequence[SimulationJobRequestTypeDef],
+        "jobs": List[SimulationJobTypeDef],
+        "unprocessedJobs": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
-    "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
+
+_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSimulationJobRequestRequestTypeDef",
+    {
+        "maxJobDurationInSeconds": int,
+        "iamRole": str,
+    },
+)
+_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSimulationJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
-        "batchPolicy": BatchPolicyTypeDef,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
+        "failureBehavior": FailureBehaviorType,
+        "robotApplications": Sequence[RobotApplicationConfigUnionTypeDef],
+        "simulationApplications": Sequence[SimulationApplicationConfigUnionTypeDef],
+        "dataSources": Sequence[DataSourceConfigUnionTypeDef],
         "tags": Mapping[str, str],
+        "vpcConfig": VPCConfigTypeDef,
+        "compute": ComputeTypeDef,
     },
     total=False,
 )
 
 
-class StartSimulationJobBatchRequestRequestTypeDef(
-    _RequiredStartSimulationJobBatchRequestRequestTypeDef,
-    _OptionalStartSimulationJobBatchRequestRequestTypeDef,
+class CreateSimulationJobRequestRequestTypeDef(
+    _RequiredCreateSimulationJobRequestRequestTypeDef,
+    _OptionalCreateSimulationJobRequestRequestTypeDef,
 ):
     pass
 
 
-BatchDescribeSimulationJobResponseTypeDef = TypedDict(
-    "BatchDescribeSimulationJobResponseTypeDef",
-    {
-        "jobs": List[SimulationJobTypeDef],
-        "unprocessedJobs": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+SimulationJobRequestUnionTypeDef = Union[
+    SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef
+]
 DescribeSimulationJobBatchResponseTypeDef = TypedDict(
     "DescribeSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "lastUpdatedAt": datetime,
         "createdAt": datetime,
         "clientRequestToken": str,
         "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
-        "pendingRequests": List[SimulationJobRequestTypeDef],
+        "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSimulationJobBatchResponseTypeDef = TypedDict(
     "StartSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "createdAt": datetime,
         "clientRequestToken": str,
         "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
-        "pendingRequests": List[SimulationJobRequestTypeDef],
+        "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
+    "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
+    {
+        "createSimulationJobRequests": Sequence[SimulationJobRequestUnionTypeDef],
     },
 )
+_OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
+    "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "batchPolicy": BatchPolicyTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class StartSimulationJobBatchRequestRequestTypeDef(
+    _RequiredStartSimulationJobBatchRequestRequestTypeDef,
+    _OptionalStartSimulationJobBatchRequestRequestTypeDef,
+):
+    pass
```

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker/type_defs.pyi` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_robomaker.type_defs import BatchDeleteWorldsRequestRequestTypeDef
 
-    data: BatchDeleteWorldsRequestRequestTypeDef = {...}
+    data: BatchDeleteWorldsRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ArchitectureType,
     ComputeTypeType,
     DataSourceTypeType,
     DeploymentJobErrorCodeType,
     DeploymentStatusType,
@@ -45,96 +45,98 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchDeleteWorldsRequestRequestTypeDef",
-    "BatchDeleteWorldsResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     "BatchPolicyTypeDef",
     "CancelDeploymentJobRequestRequestTypeDef",
     "CancelSimulationJobBatchRequestRequestTypeDef",
     "CancelSimulationJobRequestRequestTypeDef",
     "CancelWorldExportJobRequestRequestTypeDef",
     "CancelWorldGenerationJobRequestRequestTypeDef",
     "ComputeResponseTypeDef",
     "ComputeTypeDef",
     "CreateFleetRequestRequestTypeDef",
-    "CreateFleetResponseTypeDef",
     "EnvironmentTypeDef",
     "RobotSoftwareSuiteTypeDef",
     "SourceConfigTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
-    "CreateRobotResponseTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
-    "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
     "TemplateLocationTypeDef",
-    "CreateWorldTemplateResponseTypeDef",
+    "DataSourceConfigOutputTypeDef",
+    "DataSourceConfigTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
+    "DeploymentLaunchConfigOutputTypeDef",
     "DeploymentLaunchConfigTypeDef",
     "S3ObjectTypeDef",
     "DeregisterRobotRequestRequestTypeDef",
-    "DeregisterRobotResponseTypeDef",
     "DescribeDeploymentJobRequestRequestTypeDef",
     "DescribeFleetRequestRequestTypeDef",
     "RobotTypeDef",
     "DescribeRobotApplicationRequestRequestTypeDef",
     "DescribeRobotRequestRequestTypeDef",
-    "DescribeRobotResponseTypeDef",
     "DescribeSimulationApplicationRequestRequestTypeDef",
     "DescribeSimulationJobBatchRequestRequestTypeDef",
     "SimulationJobSummaryTypeDef",
     "DescribeSimulationJobRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "DescribeWorldExportJobRequestRequestTypeDef",
     "DescribeWorldGenerationJobRequestRequestTypeDef",
     "DescribeWorldRequestRequestTypeDef",
-    "DescribeWorldResponseTypeDef",
     "DescribeWorldTemplateRequestRequestTypeDef",
-    "DescribeWorldTemplateResponseTypeDef",
     "WorldFailureTypeDef",
     "FilterTypeDef",
     "FleetTypeDef",
     "GetWorldTemplateBodyRequestRequestTypeDef",
-    "GetWorldTemplateBodyResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "SimulationJobBatchSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
     "ListWorldTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "WorldSummaryTypeDef",
-    "PaginatorConfigTypeDef",
     "PortMappingTypeDef",
     "ProgressDetailTypeDef",
     "RegisterRobotRequestRequestTypeDef",
-    "RegisterRobotResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RestartSimulationJobRequestRequestTypeDef",
     "ToolTypeDef",
     "UploadConfigurationTypeDef",
     "WorldConfigTypeDef",
+    "VPCConfigOutputTypeDef",
     "SyncDeploymentJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "BatchDeleteWorldsResponseTypeDef",
+    "CreateFleetResponseTypeDef",
+    "CreateRobotResponseTypeDef",
+    "CreateWorldTemplateResponseTypeDef",
+    "DeregisterRobotResponseTypeDef",
+    "DescribeRobotResponseTypeDef",
+    "DescribeWorldResponseTypeDef",
+    "DescribeWorldTemplateResponseTypeDef",
+    "GetWorldTemplateBodyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterRobotResponseTypeDef",
     "UpdateWorldTemplateResponseTypeDef",
     "RobotApplicationSummaryTypeDef",
     "CreateRobotApplicationRequestRequestTypeDef",
     "UpdateRobotApplicationRequestRequestTypeDef",
     "CreateRobotApplicationResponseTypeDef",
     "CreateRobotApplicationVersionResponseTypeDef",
     "DescribeRobotApplicationResponseTypeDef",
@@ -151,86 +153,102 @@
     "DescribeWorldExportJobResponseTypeDef",
     "WorldExportJobSummaryTypeDef",
     "CreateWorldGenerationJobRequestRequestTypeDef",
     "CreateWorldGenerationJobResponseTypeDef",
     "WorldGenerationJobSummaryTypeDef",
     "CreateWorldTemplateRequestRequestTypeDef",
     "UpdateWorldTemplateRequestRequestTypeDef",
+    "DataSourceConfigUnionTypeDef",
     "DataSourceTypeDef",
+    "DeploymentApplicationConfigOutputTypeDef",
     "DeploymentApplicationConfigTypeDef",
     "DeploymentConfigTypeDef",
     "DescribeFleetResponseTypeDef",
     "ListRobotsResponseTypeDef",
     "ListSimulationJobsResponseTypeDef",
     "FailureSummaryTypeDef",
-    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
     "ListDeploymentJobsRequestRequestTypeDef",
-    "ListFleetsRequestListFleetsPaginateTypeDef",
     "ListFleetsRequestRequestTypeDef",
-    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
     "ListRobotApplicationsRequestRequestTypeDef",
-    "ListRobotsRequestListRobotsPaginateTypeDef",
     "ListRobotsRequestRequestTypeDef",
-    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
     "ListSimulationApplicationsRequestRequestTypeDef",
-    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
     "ListSimulationJobBatchesRequestRequestTypeDef",
-    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
     "ListSimulationJobsRequestRequestTypeDef",
-    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     "ListWorldExportJobsRequestRequestTypeDef",
-    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     "ListWorldGenerationJobsRequestRequestTypeDef",
-    "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListWorldsRequestRequestTypeDef",
     "ListFleetsResponseTypeDef",
+    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
+    "ListFleetsRequestListFleetsPaginateTypeDef",
+    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
+    "ListRobotsRequestListRobotsPaginateTypeDef",
+    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
+    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
+    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
+    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
+    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
+    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
+    "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListSimulationJobBatchesResponseTypeDef",
     "ListWorldTemplatesResponseTypeDef",
     "ListWorldsResponseTypeDef",
+    "PortForwardingConfigOutputTypeDef",
     "PortForwardingConfigTypeDef",
     "RobotDeploymentTypeDef",
+    "VPCConfigUnionTypeDef",
     "ListRobotApplicationsResponseTypeDef",
     "ListSimulationApplicationsResponseTypeDef",
     "ListWorldExportJobsResponseTypeDef",
     "ListWorldGenerationJobsResponseTypeDef",
-    "CreateDeploymentJobRequestRequestTypeDef",
+    "DeploymentApplicationConfigUnionTypeDef",
     "CreateDeploymentJobResponseTypeDef",
     "DeploymentJobTypeDef",
     "SyncDeploymentJobResponseTypeDef",
     "FinishedWorldsSummaryTypeDef",
+    "LaunchConfigOutputTypeDef",
     "LaunchConfigTypeDef",
     "DescribeDeploymentJobResponseTypeDef",
+    "CreateDeploymentJobRequestRequestTypeDef",
     "ListDeploymentJobsResponseTypeDef",
     "DescribeWorldGenerationJobResponseTypeDef",
+    "RobotApplicationConfigOutputTypeDef",
+    "SimulationApplicationConfigOutputTypeDef",
     "RobotApplicationConfigTypeDef",
     "SimulationApplicationConfigTypeDef",
-    "CreateSimulationJobRequestRequestTypeDef",
     "CreateSimulationJobResponseTypeDef",
     "DescribeSimulationJobResponseTypeDef",
-    "SimulationJobRequestTypeDef",
+    "SimulationJobRequestOutputTypeDef",
     "SimulationJobTypeDef",
+    "RobotApplicationConfigUnionTypeDef",
+    "SimulationApplicationConfigUnionTypeDef",
+    "SimulationJobRequestTypeDef",
     "FailedCreateSimulationJobRequestTypeDef",
-    "StartSimulationJobBatchRequestRequestTypeDef",
     "BatchDescribeSimulationJobResponseTypeDef",
+    "CreateSimulationJobRequestRequestTypeDef",
+    "SimulationJobRequestUnionTypeDef",
     "DescribeSimulationJobBatchResponseTypeDef",
     "StartSimulationJobBatchResponseTypeDef",
+    "StartSimulationJobBatchRequestRequestTypeDef",
 )
 
 BatchDeleteWorldsRequestRequestTypeDef = TypedDict(
     "BatchDeleteWorldsRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
     },
 )
 
-BatchDeleteWorldsResponseTypeDef = TypedDict(
-    "BatchDeleteWorldsResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "unprocessedWorlds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BatchDescribeSimulationJobRequestRequestTypeDef = TypedDict(
     "BatchDescribeSimulationJobRequestRequestTypeDef",
     {
         "jobs": Sequence[str],
@@ -316,25 +334,14 @@
 )
 
 class CreateFleetRequestRequestTypeDef(
     _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
 ):
     pass
 
-CreateFleetResponseTypeDef = TypedDict(
-    "CreateFleetResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "uri": str,
     },
     total=False,
 )
@@ -408,27 +415,14 @@
 )
 
 class CreateRobotRequestRequestTypeDef(
     _RequiredCreateRobotRequestRequestTypeDef, _OptionalCreateRobotRequestRequestTypeDef
 ):
     pass
 
-CreateRobotResponseTypeDef = TypedDict(
-    "CreateRobotResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "createdAt": datetime,
-        "greengrassGroupId": str,
-        "architecture": ArchitectureType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RenderingEngineTypeDef = TypedDict(
     "RenderingEngineTypeDef",
     {
         "name": Literal["OGRE"],
         "version": str,
     },
     total=False,
@@ -461,34 +455,14 @@
 
 class CreateSimulationApplicationVersionRequestRequestTypeDef(
     _RequiredCreateSimulationApplicationVersionRequestRequestTypeDef,
     _OptionalCreateSimulationApplicationVersionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDataSourceConfigTypeDef = TypedDict(
-    "_RequiredDataSourceConfigTypeDef",
-    {
-        "name": str,
-        "s3Bucket": str,
-        "s3Keys": Sequence[str],
-    },
-)
-_OptionalDataSourceConfigTypeDef = TypedDict(
-    "_OptionalDataSourceConfigTypeDef",
-    {
-        "type": DataSourceTypeType,
-        "destination": str,
-    },
-    total=False,
-)
-
-class DataSourceConfigTypeDef(_RequiredDataSourceConfigTypeDef, _OptionalDataSourceConfigTypeDef):
-    pass
-
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "recordAllRosTopics": bool,
     },
     total=False,
 )
@@ -544,25 +518,55 @@
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
 
-CreateWorldTemplateResponseTypeDef = TypedDict(
-    "CreateWorldTemplateResponseTypeDef",
+_RequiredDataSourceConfigOutputTypeDef = TypedDict(
+    "_RequiredDataSourceConfigOutputTypeDef",
     {
-        "arn": str,
-        "clientRequestToken": str,
-        "createdAt": datetime,
         "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "s3Bucket": str,
+        "s3Keys": List[str],
     },
 )
+_OptionalDataSourceConfigOutputTypeDef = TypedDict(
+    "_OptionalDataSourceConfigOutputTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
+    },
+    total=False,
+)
+
+class DataSourceConfigOutputTypeDef(
+    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
+):
+    pass
+
+_RequiredDataSourceConfigTypeDef = TypedDict(
+    "_RequiredDataSourceConfigTypeDef",
+    {
+        "name": str,
+        "s3Bucket": str,
+        "s3Keys": Sequence[str],
+    },
+)
+_OptionalDataSourceConfigTypeDef = TypedDict(
+    "_OptionalDataSourceConfigTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
+    },
+    total=False,
+)
+
+class DataSourceConfigTypeDef(_RequiredDataSourceConfigTypeDef, _OptionalDataSourceConfigTypeDef):
+    pass
 
 S3KeyOutputTypeDef = TypedDict(
     "S3KeyOutputTypeDef",
     {
         "s3Key": str,
         "etag": str,
     },
@@ -626,14 +630,36 @@
 DeleteWorldTemplateRequestRequestTypeDef = TypedDict(
     "DeleteWorldTemplateRequestRequestTypeDef",
     {
         "template": str,
     },
 )
 
+_RequiredDeploymentLaunchConfigOutputTypeDef = TypedDict(
+    "_RequiredDeploymentLaunchConfigOutputTypeDef",
+    {
+        "packageName": str,
+        "launchFile": str,
+    },
+)
+_OptionalDeploymentLaunchConfigOutputTypeDef = TypedDict(
+    "_OptionalDeploymentLaunchConfigOutputTypeDef",
+    {
+        "preLaunchFile": str,
+        "postLaunchFile": str,
+        "environmentVariables": Dict[str, str],
+    },
+    total=False,
+)
+
+class DeploymentLaunchConfigOutputTypeDef(
+    _RequiredDeploymentLaunchConfigOutputTypeDef, _OptionalDeploymentLaunchConfigOutputTypeDef
+):
+    pass
+
 _RequiredDeploymentLaunchConfigTypeDef = TypedDict(
     "_RequiredDeploymentLaunchConfigTypeDef",
     {
         "packageName": str,
         "launchFile": str,
     },
 )
@@ -674,23 +700,14 @@
     "DeregisterRobotRequestRequestTypeDef",
     {
         "fleet": str,
         "robot": str,
     },
 )
 
-DeregisterRobotResponseTypeDef = TypedDict(
-    "DeregisterRobotResponseTypeDef",
-    {
-        "fleet": str,
-        "robot": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDeploymentJobRequestRequestTypeDef = TypedDict(
     "DescribeDeploymentJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
@@ -740,31 +757,14 @@
 DescribeRobotRequestRequestTypeDef = TypedDict(
     "DescribeRobotRequestRequestTypeDef",
     {
         "robot": str,
     },
 )
 
-DescribeRobotResponseTypeDef = TypedDict(
-    "DescribeRobotResponseTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "fleetArn": str,
-        "status": RobotStatusType,
-        "greengrassGroupId": str,
-        "createdAt": datetime,
-        "architecture": ArchitectureType,
-        "lastDeploymentJob": str,
-        "lastDeploymentTime": datetime,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSimulationApplicationRequestRequestTypeDef",
     {
         "application": str,
     },
 )
 _OptionalDescribeSimulationApplicationRequestRequestTypeDef = TypedDict(
@@ -837,48 +837,21 @@
 DescribeWorldRequestRequestTypeDef = TypedDict(
     "DescribeWorldRequestRequestTypeDef",
     {
         "world": str,
     },
 )
 
-DescribeWorldResponseTypeDef = TypedDict(
-    "DescribeWorldResponseTypeDef",
-    {
-        "arn": str,
-        "generationJob": str,
-        "template": str,
-        "createdAt": datetime,
-        "tags": Dict[str, str],
-        "worldDescriptionBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeWorldTemplateRequestRequestTypeDef = TypedDict(
     "DescribeWorldTemplateRequestRequestTypeDef",
     {
         "template": str,
     },
 )
 
-DescribeWorldTemplateResponseTypeDef = TypedDict(
-    "DescribeWorldTemplateResponseTypeDef",
-    {
-        "arn": str,
-        "clientRequestToken": str,
-        "name": str,
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "tags": Dict[str, str],
-        "version": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorldFailureTypeDef = TypedDict(
     "WorldFailureTypeDef",
     {
         "failureCode": WorldGenerationJobErrorCodeType,
         "sampleFailureReason": str,
         "failureCount": int,
     },
@@ -912,20 +885,22 @@
     {
         "template": str,
         "generationJob": str,
     },
     total=False,
 )
 
-GetWorldTemplateBodyResponseTypeDef = TypedDict(
-    "GetWorldTemplateBodyResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "templateBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
 SimulationJobBatchSummaryTypeDef = TypedDict(
     "SimulationJobBatchSummaryTypeDef",
     {
         "arn": str,
         "lastUpdatedAt": datetime,
@@ -941,30 +916,14 @@
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
-ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = TypedDict(
-    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWorldTemplatesRequestRequestTypeDef = TypedDict(
     "ListWorldTemplatesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -989,24 +948,14 @@
         "createdAt": datetime,
         "generationJob": str,
         "template": str,
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
 _RequiredPortMappingTypeDef = TypedDict(
     "_RequiredPortMappingTypeDef",
     {
         "jobPort": int,
         "applicationPort": int,
     },
 )
@@ -1036,34 +985,14 @@
     "RegisterRobotRequestRequestTypeDef",
     {
         "fleet": str,
         "robot": str,
     },
 )
 
-RegisterRobotResponseTypeDef = TypedDict(
-    "RegisterRobotResponseTypeDef",
-    {
-        "fleet": str,
-        "robot": str,
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
 RestartSimulationJobRequestRequestTypeDef = TypedDict(
     "RestartSimulationJobRequestRequestTypeDef",
     {
         "job": str,
     },
 )
 
@@ -1100,14 +1029,32 @@
     "WorldConfigTypeDef",
     {
         "world": str,
     },
     total=False,
 )
 
+_RequiredVPCConfigOutputTypeDef = TypedDict(
+    "_RequiredVPCConfigOutputTypeDef",
+    {
+        "subnets": List[str],
+    },
+)
+_OptionalVPCConfigOutputTypeDef = TypedDict(
+    "_OptionalVPCConfigOutputTypeDef",
+    {
+        "securityGroups": List[str],
+        "assignPublicIp": bool,
+    },
+    total=False,
+)
+
+class VPCConfigOutputTypeDef(_RequiredVPCConfigOutputTypeDef, _OptionalVPCConfigOutputTypeDef):
+    pass
+
 SyncDeploymentJobRequestRequestTypeDef = TypedDict(
     "SyncDeploymentJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
         "fleet": str,
     },
 )
@@ -1124,22 +1071,144 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
+BatchDeleteWorldsResponseTypeDef = TypedDict(
+    "BatchDeleteWorldsResponseTypeDef",
+    {
+        "unprocessedWorlds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetResponseTypeDef = TypedDict(
+    "CreateFleetResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "createdAt": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRobotResponseTypeDef = TypedDict(
+    "CreateRobotResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "createdAt": datetime,
+        "greengrassGroupId": str,
+        "architecture": ArchitectureType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorldTemplateResponseTypeDef = TypedDict(
+    "CreateWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "clientRequestToken": str,
+        "createdAt": datetime,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeregisterRobotResponseTypeDef = TypedDict(
+    "DeregisterRobotResponseTypeDef",
+    {
+        "fleet": str,
+        "robot": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRobotResponseTypeDef = TypedDict(
+    "DescribeRobotResponseTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "fleetArn": str,
+        "status": RobotStatusType,
+        "greengrassGroupId": str,
+        "createdAt": datetime,
+        "architecture": ArchitectureType,
+        "lastDeploymentJob": str,
+        "lastDeploymentTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorldResponseTypeDef = TypedDict(
+    "DescribeWorldResponseTypeDef",
+    {
+        "arn": str,
+        "generationJob": str,
+        "template": str,
+        "createdAt": datetime,
+        "tags": Dict[str, str],
+        "worldDescriptionBody": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeWorldTemplateResponseTypeDef = TypedDict(
+    "DescribeWorldTemplateResponseTypeDef",
+    {
+        "arn": str,
+        "clientRequestToken": str,
+        "name": str,
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "tags": Dict[str, str],
+        "version": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorldTemplateBodyResponseTypeDef = TypedDict(
+    "GetWorldTemplateBodyResponseTypeDef",
+    {
+        "templateBody": str,
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
+RegisterRobotResponseTypeDef = TypedDict(
+    "RegisterRobotResponseTypeDef",
+    {
+        "fleet": str,
+        "robot": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateWorldTemplateResponseTypeDef = TypedDict(
     "UpdateWorldTemplateResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RobotApplicationSummaryTypeDef = TypedDict(
     "RobotApplicationSummaryTypeDef",
     {
         "name": str,
@@ -1205,30 +1274,30 @@
         "version": str,
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRobotApplicationVersionResponseTypeDef = TypedDict(
     "CreateRobotApplicationVersionResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRobotApplicationResponseTypeDef = TypedDict(
     "DescribeRobotApplicationResponseTypeDef",
     {
         "arn": str,
@@ -1237,30 +1306,30 @@
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
         "imageDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRobotApplicationResponseTypeDef = TypedDict(
     "UpdateRobotApplicationResponseTypeDef",
     {
         "arn": str,
         "name": str,
         "version": str,
         "sources": List[SourceTypeDef],
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSimulationApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSimulationApplicationRequestRequestTypeDef",
     {
         "name": str,
@@ -1295,15 +1364,15 @@
         "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSimulationApplicationVersionResponseTypeDef = TypedDict(
     "CreateSimulationApplicationVersionResponseTypeDef",
     {
         "arn": str,
@@ -1312,15 +1381,15 @@
         "sources": List[SourceTypeDef],
         "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationApplicationResponseTypeDef = TypedDict(
     "DescribeSimulationApplicationResponseTypeDef",
     {
         "arn": str,
@@ -1331,15 +1400,15 @@
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "revisionId": str,
         "lastUpdatedAt": datetime,
         "tags": Dict[str, str],
         "environment": EnvironmentTypeDef,
         "imageDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SimulationApplicationSummaryTypeDef = TypedDict(
     "SimulationApplicationSummaryTypeDef",
     {
         "name": str,
@@ -1386,15 +1455,15 @@
         "sources": List[SourceTypeDef],
         "simulationSoftwareSuite": SimulationSoftwareSuiteTypeDef,
         "robotSoftwareSuite": RobotSoftwareSuiteTypeDef,
         "renderingEngine": RenderingEngineTypeDef,
         "lastUpdatedAt": datetime,
         "revisionId": str,
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWorldExportJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorldExportJobRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
@@ -1424,15 +1493,15 @@
         "status": WorldExportJobStatusType,
         "createdAt": datetime,
         "failureCode": WorldExportJobErrorCodeType,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorldExportJobResponseTypeDef = TypedDict(
     "DescribeWorldExportJobResponseTypeDef",
     {
         "arn": str,
@@ -1441,15 +1510,15 @@
         "failureCode": WorldExportJobErrorCodeType,
         "failureReason": str,
         "clientRequestToken": str,
         "worlds": List[str],
         "outputLocation": OutputLocationTypeDef,
         "iamRole": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorldExportJobSummaryTypeDef = TypedDict(
     "WorldExportJobSummaryTypeDef",
     {
         "arn": str,
@@ -1492,15 +1561,15 @@
         "createdAt": datetime,
         "failureCode": WorldGenerationJobErrorCodeType,
         "clientRequestToken": str,
         "template": str,
         "worldCount": WorldCountTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorldGenerationJobSummaryTypeDef = TypedDict(
     "WorldGenerationJobSummaryTypeDef",
     {
         "arn": str,
@@ -1544,26 +1613,36 @@
 
 class UpdateWorldTemplateRequestRequestTypeDef(
     _RequiredUpdateWorldTemplateRequestRequestTypeDef,
     _OptionalUpdateWorldTemplateRequestRequestTypeDef,
 ):
     pass
 
+DataSourceConfigUnionTypeDef = Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "name": str,
         "s3Bucket": str,
         "s3Keys": List[S3KeyOutputTypeDef],
         "type": DataSourceTypeType,
         "destination": str,
     },
     total=False,
 )
 
+DeploymentApplicationConfigOutputTypeDef = TypedDict(
+    "DeploymentApplicationConfigOutputTypeDef",
+    {
+        "application": str,
+        "applicationVersion": str,
+        "launchConfig": DeploymentLaunchConfigOutputTypeDef,
+    },
+)
+
 DeploymentApplicationConfigTypeDef = TypedDict(
     "DeploymentApplicationConfigTypeDef",
     {
         "application": str,
         "applicationVersion": str,
         "launchConfig": DeploymentLaunchConfigTypeDef,
     },
@@ -1587,279 +1666,295 @@
         "arn": str,
         "robots": List[RobotTypeDef],
         "createdAt": datetime,
         "lastDeploymentStatus": DeploymentStatusType,
         "lastDeploymentJob": str,
         "lastDeploymentTime": datetime,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRobotsResponseTypeDef = TypedDict(
     "ListRobotsResponseTypeDef",
     {
         "robots": List[RobotTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSimulationJobsResponseTypeDef = TypedDict(
     "ListSimulationJobsResponseTypeDef",
     {
         "simulationJobSummaries": List[SimulationJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailureSummaryTypeDef = TypedDict(
     "FailureSummaryTypeDef",
     {
         "totalFailureCount": int,
         "failures": List[WorldFailureTypeDef],
     },
     total=False,
 )
 
-ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = TypedDict(
-    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
+ListDeploymentJobsRequestRequestTypeDef = TypedDict(
+    "ListDeploymentJobsRequestRequestTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-ListDeploymentJobsRequestRequestTypeDef = TypedDict(
-    "ListDeploymentJobsRequestRequestTypeDef",
+ListFleetsRequestRequestTypeDef = TypedDict(
+    "ListFleetsRequestRequestTypeDef",
     {
-        "filters": Sequence[FilterTypeDef],
         "nextToken": str,
         "maxResults": int,
+        "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
-    "ListFleetsRequestListFleetsPaginateTypeDef",
+ListRobotApplicationsRequestRequestTypeDef = TypedDict(
+    "ListRobotApplicationsRequestRequestTypeDef",
     {
+        "versionQualifier": str,
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListFleetsRequestRequestTypeDef = TypedDict(
-    "ListFleetsRequestRequestTypeDef",
+ListRobotsRequestRequestTypeDef = TypedDict(
+    "ListRobotsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = TypedDict(
-    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
+ListSimulationApplicationsRequestRequestTypeDef = TypedDict(
+    "ListSimulationApplicationsRequestRequestTypeDef",
     {
         "versionQualifier": str,
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListRobotApplicationsRequestRequestTypeDef = TypedDict(
-    "ListRobotApplicationsRequestRequestTypeDef",
+ListSimulationJobBatchesRequestRequestTypeDef = TypedDict(
+    "ListSimulationJobBatchesRequestRequestTypeDef",
     {
-        "versionQualifier": str,
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListRobotsRequestListRobotsPaginateTypeDef = TypedDict(
-    "ListRobotsRequestListRobotsPaginateTypeDef",
+ListSimulationJobsRequestRequestTypeDef = TypedDict(
+    "ListSimulationJobsRequestRequestTypeDef",
     {
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListRobotsRequestRequestTypeDef = TypedDict(
-    "ListRobotsRequestRequestTypeDef",
+ListWorldExportJobsRequestRequestTypeDef = TypedDict(
+    "ListWorldExportJobsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = TypedDict(
-    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
+ListWorldGenerationJobsRequestRequestTypeDef = TypedDict(
+    "ListWorldGenerationJobsRequestRequestTypeDef",
     {
-        "versionQualifier": str,
+        "nextToken": str,
+        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListSimulationApplicationsRequestRequestTypeDef = TypedDict(
-    "ListSimulationApplicationsRequestRequestTypeDef",
+ListWorldsRequestRequestTypeDef = TypedDict(
+    "ListWorldsRequestRequestTypeDef",
     {
-        "versionQualifier": str,
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = TypedDict(
-    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
+ListFleetsResponseTypeDef = TypedDict(
+    "ListFleetsResponseTypeDef",
+    {
+        "fleetDetails": List[FleetTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef = TypedDict(
+    "ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobBatchesRequestRequestTypeDef = TypedDict(
-    "ListSimulationJobBatchesRequestRequestTypeDef",
+ListFleetsRequestListFleetsPaginateTypeDef = TypedDict(
+    "ListFleetsRequestListFleetsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = TypedDict(
-    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
+ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef = TypedDict(
+    "ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef",
     {
+        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListSimulationJobsRequestRequestTypeDef = TypedDict(
-    "ListSimulationJobsRequestRequestTypeDef",
+ListRobotsRequestListRobotsPaginateTypeDef = TypedDict(
+    "ListRobotsRequestListRobotsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = TypedDict(
-    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
+ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef = TypedDict(
+    "ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef",
     {
+        "versionQualifier": str,
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldExportJobsRequestRequestTypeDef = TypedDict(
-    "ListWorldExportJobsRequestRequestTypeDef",
+ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef = TypedDict(
+    "ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = TypedDict(
-    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
+ListSimulationJobsRequestListSimulationJobsPaginateTypeDef = TypedDict(
+    "ListSimulationJobsRequestListSimulationJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldGenerationJobsRequestRequestTypeDef = TypedDict(
-    "ListWorldGenerationJobsRequestRequestTypeDef",
+ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef = TypedDict(
+    "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
         "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldsRequestListWorldsPaginateTypeDef = TypedDict(
-    "ListWorldsRequestListWorldsPaginateTypeDef",
+ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef = TypedDict(
+    "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWorldsRequestRequestTypeDef = TypedDict(
-    "ListWorldsRequestRequestTypeDef",
+ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef = TypedDict(
+    "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
-        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListFleetsResponseTypeDef = TypedDict(
-    "ListFleetsResponseTypeDef",
+ListWorldsRequestListWorldsPaginateTypeDef = TypedDict(
+    "ListWorldsRequestListWorldsPaginateTypeDef",
     {
-        "fleetDetails": List[FleetTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListSimulationJobBatchesResponseTypeDef = TypedDict(
     "ListSimulationJobBatchesResponseTypeDef",
     {
         "simulationJobBatchSummaries": List[SimulationJobBatchSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldTemplatesResponseTypeDef = TypedDict(
     "ListWorldTemplatesResponseTypeDef",
     {
         "templateSummaries": List[TemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldsResponseTypeDef = TypedDict(
     "ListWorldsResponseTypeDef",
     {
         "worldSummaries": List[WorldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PortForwardingConfigOutputTypeDef = TypedDict(
+    "PortForwardingConfigOutputTypeDef",
+    {
+        "portMappings": List[PortMappingTypeDef],
+    },
+    total=False,
+)
+
 PortForwardingConfigTypeDef = TypedDict(
     "PortForwardingConfigTypeDef",
     {
-        "portMappings": List[PortMappingTypeDef],
+        "portMappings": Sequence[PortMappingTypeDef],
     },
     total=False,
 )
 
 RobotDeploymentTypeDef = TypedDict(
     "RobotDeploymentTypeDef",
     {
@@ -1870,96 +1965,77 @@
         "progressDetail": ProgressDetailTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
     },
     total=False,
 )
 
+VPCConfigUnionTypeDef = Union[VPCConfigTypeDef, VPCConfigOutputTypeDef]
 ListRobotApplicationsResponseTypeDef = TypedDict(
     "ListRobotApplicationsResponseTypeDef",
     {
         "robotApplicationSummaries": List[RobotApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSimulationApplicationsResponseTypeDef = TypedDict(
     "ListSimulationApplicationsResponseTypeDef",
     {
         "simulationApplicationSummaries": List[SimulationApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldExportJobsResponseTypeDef = TypedDict(
     "ListWorldExportJobsResponseTypeDef",
     {
         "worldExportJobSummaries": List[WorldExportJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorldGenerationJobsResponseTypeDef = TypedDict(
     "ListWorldGenerationJobsResponseTypeDef",
     {
         "worldGenerationJobSummaries": List[WorldGenerationJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "fleet": str,
-        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
-    },
-)
-_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "tags": Mapping[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateDeploymentJobRequestRequestTypeDef(
-    _RequiredCreateDeploymentJobRequestRequestTypeDef,
-    _OptionalCreateDeploymentJobRequestRequestTypeDef,
-):
-    pass
-
+DeploymentApplicationConfigUnionTypeDef = Union[
+    DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef
+]
 CreateDeploymentJobResponseTypeDef = TypedDict(
     "CreateDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "deploymentConfig": DeploymentConfigTypeDef,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentJobTypeDef = TypedDict(
     "DeploymentJobTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "deploymentConfig": DeploymentConfigTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
     },
     total=False,
 )
@@ -1967,68 +2043,104 @@
 SyncDeploymentJobResponseTypeDef = TypedDict(
     "SyncDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentConfig": DeploymentConfigTypeDef,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FinishedWorldsSummaryTypeDef = TypedDict(
     "FinishedWorldsSummaryTypeDef",
     {
         "finishedCount": int,
         "succeededWorlds": List[str],
         "failureSummary": FailureSummaryTypeDef,
     },
     total=False,
 )
 
+LaunchConfigOutputTypeDef = TypedDict(
+    "LaunchConfigOutputTypeDef",
+    {
+        "packageName": str,
+        "launchFile": str,
+        "environmentVariables": Dict[str, str],
+        "portForwardingConfig": PortForwardingConfigOutputTypeDef,
+        "streamUI": bool,
+        "command": List[str],
+    },
+    total=False,
+)
+
 LaunchConfigTypeDef = TypedDict(
     "LaunchConfigTypeDef",
     {
         "packageName": str,
         "launchFile": str,
-        "environmentVariables": Dict[str, str],
+        "environmentVariables": Mapping[str, str],
         "portForwardingConfig": PortForwardingConfigTypeDef,
         "streamUI": bool,
-        "command": List[str],
+        "command": Sequence[str],
     },
     total=False,
 )
 
 DescribeDeploymentJobResponseTypeDef = TypedDict(
     "DescribeDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentConfig": DeploymentConfigTypeDef,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "robotDeploymentSummary": List[RobotDeploymentTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "fleet": str,
+        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigUnionTypeDef],
+    },
+)
+_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "deploymentConfig": DeploymentConfigTypeDef,
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
+class CreateDeploymentJobRequestRequestTypeDef(
+    _RequiredCreateDeploymentJobRequestRequestTypeDef,
+    _OptionalCreateDeploymentJobRequestRequestTypeDef,
+):
+    pass
+
 ListDeploymentJobsResponseTypeDef = TypedDict(
     "ListDeploymentJobsResponseTypeDef",
     {
         "deploymentJobs": List[DeploymentJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorldGenerationJobResponseTypeDef = TypedDict(
     "DescribeWorldGenerationJobResponseTypeDef",
     {
         "arn": str,
@@ -2038,94 +2150,114 @@
         "failureReason": str,
         "clientRequestToken": str,
         "template": str,
         "worldCount": WorldCountTypeDef,
         "finishedWorldsSummary": FinishedWorldsSummaryTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRobotApplicationConfigTypeDef = TypedDict(
-    "_RequiredRobotApplicationConfigTypeDef",
+_RequiredRobotApplicationConfigOutputTypeDef = TypedDict(
+    "_RequiredRobotApplicationConfigOutputTypeDef",
     {
         "application": str,
-        "launchConfig": LaunchConfigTypeDef,
+        "launchConfig": LaunchConfigOutputTypeDef,
     },
 )
-_OptionalRobotApplicationConfigTypeDef = TypedDict(
-    "_OptionalRobotApplicationConfigTypeDef",
+_OptionalRobotApplicationConfigOutputTypeDef = TypedDict(
+    "_OptionalRobotApplicationConfigOutputTypeDef",
     {
         "applicationVersion": str,
         "uploadConfigurations": List[UploadConfigurationTypeDef],
         "useDefaultUploadConfigurations": bool,
         "tools": List[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
-class RobotApplicationConfigTypeDef(
-    _RequiredRobotApplicationConfigTypeDef, _OptionalRobotApplicationConfigTypeDef
+class RobotApplicationConfigOutputTypeDef(
+    _RequiredRobotApplicationConfigOutputTypeDef, _OptionalRobotApplicationConfigOutputTypeDef
 ):
     pass
 
-_RequiredSimulationApplicationConfigTypeDef = TypedDict(
-    "_RequiredSimulationApplicationConfigTypeDef",
+_RequiredSimulationApplicationConfigOutputTypeDef = TypedDict(
+    "_RequiredSimulationApplicationConfigOutputTypeDef",
     {
         "application": str,
-        "launchConfig": LaunchConfigTypeDef,
+        "launchConfig": LaunchConfigOutputTypeDef,
     },
 )
-_OptionalSimulationApplicationConfigTypeDef = TypedDict(
-    "_OptionalSimulationApplicationConfigTypeDef",
+_OptionalSimulationApplicationConfigOutputTypeDef = TypedDict(
+    "_OptionalSimulationApplicationConfigOutputTypeDef",
     {
         "applicationVersion": str,
         "uploadConfigurations": List[UploadConfigurationTypeDef],
         "worldConfigs": List[WorldConfigTypeDef],
         "useDefaultUploadConfigurations": bool,
         "tools": List[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
-class SimulationApplicationConfigTypeDef(
-    _RequiredSimulationApplicationConfigTypeDef, _OptionalSimulationApplicationConfigTypeDef
+class SimulationApplicationConfigOutputTypeDef(
+    _RequiredSimulationApplicationConfigOutputTypeDef,
+    _OptionalSimulationApplicationConfigOutputTypeDef,
 ):
     pass
 
-_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSimulationJobRequestRequestTypeDef",
+_RequiredRobotApplicationConfigTypeDef = TypedDict(
+    "_RequiredRobotApplicationConfigTypeDef",
     {
-        "maxJobDurationInSeconds": int,
-        "iamRole": str,
+        "application": str,
+        "launchConfig": LaunchConfigTypeDef,
     },
 )
-_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSimulationJobRequestRequestTypeDef",
+_OptionalRobotApplicationConfigTypeDef = TypedDict(
+    "_OptionalRobotApplicationConfigTypeDef",
     {
-        "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
-        "failureBehavior": FailureBehaviorType,
-        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
-        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
-        "dataSources": Sequence[DataSourceConfigTypeDef],
-        "tags": Mapping[str, str],
-        "vpcConfig": VPCConfigTypeDef,
-        "compute": ComputeTypeDef,
+        "applicationVersion": str,
+        "uploadConfigurations": Sequence[UploadConfigurationTypeDef],
+        "useDefaultUploadConfigurations": bool,
+        "tools": Sequence[ToolTypeDef],
+        "useDefaultTools": bool,
     },
     total=False,
 )
 
-class CreateSimulationJobRequestRequestTypeDef(
-    _RequiredCreateSimulationJobRequestRequestTypeDef,
-    _OptionalCreateSimulationJobRequestRequestTypeDef,
+class RobotApplicationConfigTypeDef(
+    _RequiredRobotApplicationConfigTypeDef, _OptionalRobotApplicationConfigTypeDef
+):
+    pass
+
+_RequiredSimulationApplicationConfigTypeDef = TypedDict(
+    "_RequiredSimulationApplicationConfigTypeDef",
+    {
+        "application": str,
+        "launchConfig": LaunchConfigTypeDef,
+    },
+)
+_OptionalSimulationApplicationConfigTypeDef = TypedDict(
+    "_OptionalSimulationApplicationConfigTypeDef",
+    {
+        "applicationVersion": str,
+        "uploadConfigurations": Sequence[UploadConfigurationTypeDef],
+        "worldConfigs": Sequence[WorldConfigTypeDef],
+        "useDefaultUploadConfigurations": bool,
+        "tools": Sequence[ToolTypeDef],
+        "useDefaultTools": bool,
+    },
+    total=False,
+)
+
+class SimulationApplicationConfigTypeDef(
+    _RequiredSimulationApplicationConfigTypeDef, _OptionalSimulationApplicationConfigTypeDef
 ):
     pass
 
 CreateSimulationJobResponseTypeDef = TypedDict(
     "CreateSimulationJobResponseTypeDef",
     {
         "arn": str,
@@ -2136,21 +2268,21 @@
         "failureCode": SimulationJobErrorCodeType,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "compute": ComputeResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSimulationJobResponseTypeDef = TypedDict(
     "DescribeSimulationJobResponseTypeDef",
     {
         "arn": str,
@@ -2163,51 +2295,51 @@
         "failureReason": str,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSimulationJobRequestTypeDef = TypedDict(
-    "_RequiredSimulationJobRequestTypeDef",
+_RequiredSimulationJobRequestOutputTypeDef = TypedDict(
+    "_RequiredSimulationJobRequestOutputTypeDef",
     {
         "maxJobDurationInSeconds": int,
     },
 )
-_OptionalSimulationJobRequestTypeDef = TypedDict(
-    "_OptionalSimulationJobRequestTypeDef",
+_OptionalSimulationJobRequestOutputTypeDef = TypedDict(
+    "_OptionalSimulationJobRequestOutputTypeDef",
     {
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "iamRole": str,
         "failureBehavior": FailureBehaviorType,
         "useDefaultApplications": bool,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
-        "dataSources": List[DataSourceConfigTypeDef],
-        "vpcConfig": VPCConfigTypeDef,
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
+        "dataSources": List[DataSourceConfigOutputTypeDef],
+        "vpcConfig": VPCConfigOutputTypeDef,
         "compute": ComputeTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-class SimulationJobRequestTypeDef(
-    _RequiredSimulationJobRequestTypeDef, _OptionalSimulationJobRequestTypeDef
+class SimulationJobRequestOutputTypeDef(
+    _RequiredSimulationJobRequestOutputTypeDef, _OptionalSimulationJobRequestOutputTypeDef
 ):
     pass
 
 SimulationJobTypeDef = TypedDict(
     "SimulationJobTypeDef",
     {
         "arn": str,
@@ -2220,96 +2352,164 @@
         "failureReason": str,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
     },
     total=False,
 )
 
+RobotApplicationConfigUnionTypeDef = Union[
+    RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef
+]
+SimulationApplicationConfigUnionTypeDef = Union[
+    SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef
+]
+_RequiredSimulationJobRequestTypeDef = TypedDict(
+    "_RequiredSimulationJobRequestTypeDef",
+    {
+        "maxJobDurationInSeconds": int,
+    },
+)
+_OptionalSimulationJobRequestTypeDef = TypedDict(
+    "_OptionalSimulationJobRequestTypeDef",
+    {
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
+        "iamRole": str,
+        "failureBehavior": FailureBehaviorType,
+        "useDefaultApplications": bool,
+        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
+        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
+        "dataSources": Sequence[DataSourceConfigTypeDef],
+        "vpcConfig": VPCConfigTypeDef,
+        "compute": ComputeTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class SimulationJobRequestTypeDef(
+    _RequiredSimulationJobRequestTypeDef, _OptionalSimulationJobRequestTypeDef
+):
+    pass
+
 FailedCreateSimulationJobRequestTypeDef = TypedDict(
     "FailedCreateSimulationJobRequestTypeDef",
     {
-        "request": SimulationJobRequestTypeDef,
+        "request": SimulationJobRequestOutputTypeDef,
         "failureReason": str,
         "failureCode": SimulationJobErrorCodeType,
         "failedAt": datetime,
     },
     total=False,
 )
 
-_RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
-    "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
+BatchDescribeSimulationJobResponseTypeDef = TypedDict(
+    "BatchDescribeSimulationJobResponseTypeDef",
     {
-        "createSimulationJobRequests": Sequence[SimulationJobRequestTypeDef],
+        "jobs": List[SimulationJobTypeDef],
+        "unprocessedJobs": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
-    "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
+
+_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSimulationJobRequestRequestTypeDef",
+    {
+        "maxJobDurationInSeconds": int,
+        "iamRole": str,
+    },
+)
+_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSimulationJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
-        "batchPolicy": BatchPolicyTypeDef,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
+        "failureBehavior": FailureBehaviorType,
+        "robotApplications": Sequence[RobotApplicationConfigUnionTypeDef],
+        "simulationApplications": Sequence[SimulationApplicationConfigUnionTypeDef],
+        "dataSources": Sequence[DataSourceConfigUnionTypeDef],
         "tags": Mapping[str, str],
+        "vpcConfig": VPCConfigTypeDef,
+        "compute": ComputeTypeDef,
     },
     total=False,
 )
 
-class StartSimulationJobBatchRequestRequestTypeDef(
-    _RequiredStartSimulationJobBatchRequestRequestTypeDef,
-    _OptionalStartSimulationJobBatchRequestRequestTypeDef,
+class CreateSimulationJobRequestRequestTypeDef(
+    _RequiredCreateSimulationJobRequestRequestTypeDef,
+    _OptionalCreateSimulationJobRequestRequestTypeDef,
 ):
     pass
 
-BatchDescribeSimulationJobResponseTypeDef = TypedDict(
-    "BatchDescribeSimulationJobResponseTypeDef",
-    {
-        "jobs": List[SimulationJobTypeDef],
-        "unprocessedJobs": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+SimulationJobRequestUnionTypeDef = Union[
+    SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef
+]
 DescribeSimulationJobBatchResponseTypeDef = TypedDict(
     "DescribeSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "lastUpdatedAt": datetime,
         "createdAt": datetime,
         "clientRequestToken": str,
         "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
-        "pendingRequests": List[SimulationJobRequestTypeDef],
+        "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSimulationJobBatchResponseTypeDef = TypedDict(
     "StartSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "createdAt": datetime,
         "clientRequestToken": str,
         "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
-        "pendingRequests": List[SimulationJobRequestTypeDef],
+        "pendingRequests": List[SimulationJobRequestOutputTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
+    "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
+    {
+        "createSimulationJobRequests": Sequence[SimulationJobRequestUnionTypeDef],
     },
 )
+_OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
+    "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "batchPolicy": BatchPolicyTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class StartSimulationJobBatchRequestRequestTypeDef(
+    _RequiredStartSimulationJobBatchRequestRequestTypeDef,
+    _OptionalStartSimulationJobBatchRequestRequestTypeDef,
+):
+    pass
```

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker.egg-info/PKG-INFO` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-robomaker
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.RoboMaker 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.RoboMaker 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore robomaker type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore robomaker type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-robomaker"></a>
 
 # types-aiobotocore-robomaker
 
 [![PyPI - types-aiobotocore-robomaker](https://img.shields.io/pypi/v/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-robomaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-robomaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-robomaker?color=blue)](https://pypistats.org/packages/types-aiobotocore-robomaker)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-robomaker)](https://pepy.tech/project/types-aiobotocore-robomaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.RoboMaker 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
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
 [types-aiobotocore-robomaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/).
 
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
@@ -375,106 +374,108 @@
 )
 
 
 def check_value(value: ArchitectureType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_robomaker.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_robomaker.type_defs import (
     BatchDeleteWorldsRequestRequestTypeDef,
-    BatchDeleteWorldsResponseTypeDef,
+    ResponseMetadataTypeDef,
     BatchDescribeSimulationJobRequestRequestTypeDef,
     BatchPolicyTypeDef,
     CancelDeploymentJobRequestRequestTypeDef,
     CancelSimulationJobBatchRequestRequestTypeDef,
     CancelSimulationJobRequestRequestTypeDef,
     CancelWorldExportJobRequestRequestTypeDef,
     CancelWorldGenerationJobRequestRequestTypeDef,
     ComputeResponseTypeDef,
     ComputeTypeDef,
     CreateFleetRequestRequestTypeDef,
-    CreateFleetResponseTypeDef,
     EnvironmentTypeDef,
     RobotSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     SourceTypeDef,
     CreateRobotApplicationVersionRequestRequestTypeDef,
     CreateRobotRequestRequestTypeDef,
-    CreateRobotResponseTypeDef,
     RenderingEngineTypeDef,
     SimulationSoftwareSuiteTypeDef,
     CreateSimulationApplicationVersionRequestRequestTypeDef,
-    DataSourceConfigTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     VPCConfigTypeDef,
     VPCConfigResponseTypeDef,
     WorldCountTypeDef,
     TemplateLocationTypeDef,
-    CreateWorldTemplateResponseTypeDef,
+    DataSourceConfigOutputTypeDef,
+    DataSourceConfigTypeDef,
     S3KeyOutputTypeDef,
     DeleteFleetRequestRequestTypeDef,
     DeleteRobotApplicationRequestRequestTypeDef,
     DeleteRobotRequestRequestTypeDef,
     DeleteSimulationApplicationRequestRequestTypeDef,
     DeleteWorldTemplateRequestRequestTypeDef,
+    DeploymentLaunchConfigOutputTypeDef,
     DeploymentLaunchConfigTypeDef,
     S3ObjectTypeDef,
     DeregisterRobotRequestRequestTypeDef,
-    DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobRequestRequestTypeDef,
     DescribeFleetRequestRequestTypeDef,
     RobotTypeDef,
     DescribeRobotApplicationRequestRequestTypeDef,
     DescribeRobotRequestRequestTypeDef,
-    DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationRequestRequestTypeDef,
     DescribeSimulationJobBatchRequestRequestTypeDef,
     SimulationJobSummaryTypeDef,
     DescribeSimulationJobRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     DescribeWorldExportJobRequestRequestTypeDef,
     DescribeWorldGenerationJobRequestRequestTypeDef,
     DescribeWorldRequestRequestTypeDef,
-    DescribeWorldResponseTypeDef,
     DescribeWorldTemplateRequestRequestTypeDef,
-    DescribeWorldTemplateResponseTypeDef,
     WorldFailureTypeDef,
     FilterTypeDef,
     FleetTypeDef,
     GetWorldTemplateBodyRequestRequestTypeDef,
-    GetWorldTemplateBodyResponseTypeDef,
+    PaginatorConfigTypeDef,
     SimulationJobBatchSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
     ListWorldTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     WorldSummaryTypeDef,
-    PaginatorConfigTypeDef,
     PortMappingTypeDef,
     ProgressDetailTypeDef,
     RegisterRobotRequestRequestTypeDef,
-    RegisterRobotResponseTypeDef,
-    ResponseMetadataTypeDef,
     RestartSimulationJobRequestRequestTypeDef,
     ToolTypeDef,
     UploadConfigurationTypeDef,
     WorldConfigTypeDef,
+    VPCConfigOutputTypeDef,
     SyncDeploymentJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    BatchDeleteWorldsResponseTypeDef,
+    CreateFleetResponseTypeDef,
+    CreateRobotResponseTypeDef,
+    CreateWorldTemplateResponseTypeDef,
+    DeregisterRobotResponseTypeDef,
+    DescribeRobotResponseTypeDef,
+    DescribeWorldResponseTypeDef,
+    DescribeWorldTemplateResponseTypeDef,
+    GetWorldTemplateBodyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterRobotResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
     RobotApplicationSummaryTypeDef,
     CreateRobotApplicationRequestRequestTypeDef,
     UpdateRobotApplicationRequestRequestTypeDef,
     CreateRobotApplicationResponseTypeDef,
     CreateRobotApplicationVersionResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
@@ -491,76 +492,89 @@
     DescribeWorldExportJobResponseTypeDef,
     WorldExportJobSummaryTypeDef,
     CreateWorldGenerationJobRequestRequestTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     WorldGenerationJobSummaryTypeDef,
     CreateWorldTemplateRequestRequestTypeDef,
     UpdateWorldTemplateRequestRequestTypeDef,
+    DataSourceConfigUnionTypeDef,
     DataSourceTypeDef,
+    DeploymentApplicationConfigOutputTypeDef,
     DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DescribeFleetResponseTypeDef,
     ListRobotsResponseTypeDef,
     ListSimulationJobsResponseTypeDef,
     FailureSummaryTypeDef,
-    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
     ListDeploymentJobsRequestRequestTypeDef,
-    ListFleetsRequestListFleetsPaginateTypeDef,
     ListFleetsRequestRequestTypeDef,
-    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
     ListRobotApplicationsRequestRequestTypeDef,
-    ListRobotsRequestListRobotsPaginateTypeDef,
     ListRobotsRequestRequestTypeDef,
-    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
     ListSimulationApplicationsRequestRequestTypeDef,
-    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
     ListSimulationJobBatchesRequestRequestTypeDef,
-    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
     ListSimulationJobsRequestRequestTypeDef,
-    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
     ListWorldExportJobsRequestRequestTypeDef,
-    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
     ListWorldGenerationJobsRequestRequestTypeDef,
-    ListWorldsRequestListWorldsPaginateTypeDef,
     ListWorldsRequestRequestTypeDef,
     ListFleetsResponseTypeDef,
+    ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef,
+    ListFleetsRequestListFleetsPaginateTypeDef,
+    ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef,
+    ListRobotsRequestListRobotsPaginateTypeDef,
+    ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef,
+    ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef,
+    ListSimulationJobsRequestListSimulationJobsPaginateTypeDef,
+    ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef,
+    ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef,
+    ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef,
+    ListWorldsRequestListWorldsPaginateTypeDef,
     ListSimulationJobBatchesResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     ListWorldsResponseTypeDef,
+    PortForwardingConfigOutputTypeDef,
     PortForwardingConfigTypeDef,
     RobotDeploymentTypeDef,
+    VPCConfigUnionTypeDef,
     ListRobotApplicationsResponseTypeDef,
     ListSimulationApplicationsResponseTypeDef,
     ListWorldExportJobsResponseTypeDef,
     ListWorldGenerationJobsResponseTypeDef,
-    CreateDeploymentJobRequestRequestTypeDef,
+    DeploymentApplicationConfigUnionTypeDef,
     CreateDeploymentJobResponseTypeDef,
     DeploymentJobTypeDef,
     SyncDeploymentJobResponseTypeDef,
     FinishedWorldsSummaryTypeDef,
+    LaunchConfigOutputTypeDef,
     LaunchConfigTypeDef,
     DescribeDeploymentJobResponseTypeDef,
+    CreateDeploymentJobRequestRequestTypeDef,
     ListDeploymentJobsResponseTypeDef,
     DescribeWorldGenerationJobResponseTypeDef,
+    RobotApplicationConfigOutputTypeDef,
+    SimulationApplicationConfigOutputTypeDef,
     RobotApplicationConfigTypeDef,
     SimulationApplicationConfigTypeDef,
-    CreateSimulationJobRequestRequestTypeDef,
     CreateSimulationJobResponseTypeDef,
     DescribeSimulationJobResponseTypeDef,
-    SimulationJobRequestTypeDef,
+    SimulationJobRequestOutputTypeDef,
     SimulationJobTypeDef,
+    RobotApplicationConfigUnionTypeDef,
+    SimulationApplicationConfigUnionTypeDef,
+    SimulationJobRequestTypeDef,
     FailedCreateSimulationJobRequestTypeDef,
-    StartSimulationJobBatchRequestRequestTypeDef,
     BatchDescribeSimulationJobResponseTypeDef,
+    CreateSimulationJobRequestRequestTypeDef,
+    SimulationJobRequestUnionTypeDef,
     DescribeSimulationJobBatchResponseTypeDef,
     StartSimulationJobBatchResponseTypeDef,
+    StartSimulationJobBatchRequestRequestTypeDef,
 )
 
 
-def get_structure() -> BatchDeleteWorldsRequestRequestTypeDef:
+def get_value() -> BatchDeleteWorldsRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-robomaker-2.5.2/types_aiobotocore_robomaker.egg-info/SOURCES.txt` & `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*


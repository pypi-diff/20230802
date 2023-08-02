# Comparing `tmp/types-aiobotocore-codedeploy-2.5.2.tar.gz` & `tmp/types-aiobotocore-codedeploy-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codedeploy-2.5.2.tar", last modified: Sat Jul  8 01:43:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-codedeploy-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
```

## Comparing `types-aiobotocore-codedeploy-2.5.2.tar` & `types-aiobotocore-codedeploy-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.861869 types-aiobotocore-codedeploy-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-07-08 01:43:23.861869 types-aiobotocore-codedeploy-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20641 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:23.861869 types-aiobotocore-codedeploy-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.857869 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48531 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48465 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14447 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50701 2023-07-08 01:27:33.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50668 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:31.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-08 01:27:32.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.861869 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-07-08 01:43:23.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-08 01:43:23.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:23.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:23.000000 types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.569625 types-aiobotocore-codedeploy-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-08-02 14:52:02.565625 types-aiobotocore-codedeploy-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21198 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.569625 types-aiobotocore-codedeploy-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.565625 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48641 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48575 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-08-02 14:35:06.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14447 2023-08-02 14:35:06.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-08-02 14:35:05.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53972 2023-08-02 14:35:07.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53939 2023-08-02 14:35:06.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-02 14:35:05.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-02 14:35:05.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.565625 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-08-02 14:52:02.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-02 14:52:02.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:02.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codedeploy-2.5.2/LICENSE` & `types-aiobotocore-codedeploy-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2/PKG-INFO` & `types-aiobotocore-codedeploy-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codedeploy
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeDeploy 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeDeploy 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codedeploy type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codedeploy type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codedeploy"></a>
 
 # types-aiobotocore-codedeploy
 
 [![PyPI - types-aiobotocore-codedeploy](https://img.shields.io/pypi/v/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codedeploy?color=blue)](https://pypistats.org/packages/types-aiobotocore-codedeploy)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codedeploy)](https://pepy.tech/project/types-aiobotocore-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeDeploy 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [types-aiobotocore-codedeploy docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -407,176 +406,193 @@
 )
 
 
 def check_value(value: ApplicationRevisionSortByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codedeploy.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codedeploy.type_defs import (
     TagTypeDef,
     AlarmTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
+    AutoRollbackConfigurationOutputTypeDef,
     AutoRollbackConfigurationTypeDef,
     AutoScalingGroupTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetApplicationsInputRequestTypeDef,
     BatchGetDeploymentGroupsInputRequestTypeDef,
     BatchGetDeploymentInstancesInputRequestTypeDef,
     BatchGetDeploymentTargetsInputRequestTypeDef,
     BatchGetDeploymentsInputRequestTypeDef,
     BatchGetOnPremisesInstancesInputRequestTypeDef,
     BlueInstanceTerminationOptionTypeDef,
     DeploymentReadyOptionTypeDef,
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
-    CreateApplicationOutputTypeDef,
     MinimumHealthyHostsTypeDef,
-    CreateDeploymentConfigOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
     ECSServiceTypeDef,
     TagFilterTypeDef,
-    TriggerConfigTypeDef,
-    CreateDeploymentGroupOutputTypeDef,
-    CreateDeploymentOutputTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
-    DeleteGitHubAccountTokenOutputTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
     LastDeploymentInfoTypeDef,
+    TriggerConfigOutputTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
     TargetGroupInfoTypeDef,
     ELBInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
     GenericRevisionInfoTypeDef,
     GetApplicationInputRequestTypeDef,
     GetDeploymentConfigInputRequestTypeDef,
     GetDeploymentGroupInputRequestTypeDef,
     WaiterConfigTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetDeploymentInstanceInputRequestTypeDef,
     GetDeploymentTargetInputRequestTypeDef,
     GetOnPremisesInstanceInputRequestTypeDef,
     GitHubLocationTypeDef,
     LambdaFunctionInfoTypeDef,
-    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
-    ListApplicationsOutputTypeDef,
-    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
     ListDeploymentConfigsInputRequestTypeDef,
-    ListDeploymentConfigsOutputTypeDef,
-    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     ListDeploymentGroupsInputRequestTypeDef,
-    ListDeploymentGroupsOutputTypeDef,
-    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     ListDeploymentInstancesInputRequestTypeDef,
-    ListDeploymentInstancesOutputTypeDef,
-    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
     ListDeploymentTargetsInputRequestTypeDef,
-    ListDeploymentTargetsOutputTypeDef,
-    TimeRangeTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
-    ListGitHubAccountTokenNamesOutputTypeDef,
-    ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
-    PutLifecycleEventHookExecutionStatusOutputTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
-    StopDeploymentOutputTypeDef,
+    TrafficRouteOutputTypeDef,
     TrafficRouteTypeDef,
     TimeBasedCanaryTypeDef,
     TimeBasedLinearTypeDef,
+    TimestampTypeDef,
+    TriggerConfigTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
     InstanceInfoTypeDef,
-    ListTagsForResourceOutputTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
+    AutoRollbackConfigurationUnionTypeDef,
     BatchGetApplicationsOutputTypeDef,
-    GetApplicationOutputTypeDef,
+    CreateApplicationOutputTypeDef,
+    CreateDeploymentConfigOutputTypeDef,
+    CreateDeploymentGroupOutputTypeDef,
+    CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
+    DeleteGitHubAccountTokenOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetApplicationOutputTypeDef,
+    ListApplicationsOutputTypeDef,
+    ListDeploymentConfigsOutputTypeDef,
+    ListDeploymentGroupsOutputTypeDef,
+    ListDeploymentInstancesOutputTypeDef,
+    ListDeploymentTargetsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListGitHubAccountTokenNamesOutputTypeDef,
+    ListOnPremisesInstancesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PutLifecycleEventHookExecutionStatusOutputTypeDef,
+    StopDeploymentOutputTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
     BlueGreenDeploymentConfigurationTypeDef,
+    EC2TagSetOutputTypeDef,
     EC2TagSetTypeDef,
-    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListOnPremisesInstancesInputRequestTypeDef,
+    OnPremisesTagSetOutputTypeDef,
     OnPremisesTagSetTypeDef,
     LifecycleEventTypeDef,
     ECSTaskSetTypeDef,
     GetDeploymentInputDeploymentSuccessfulWaitTypeDef,
-    ListDeploymentsInputListDeploymentsPaginateTypeDef,
-    ListDeploymentsInputRequestTypeDef,
+    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
+    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
+    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
+    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
+    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     RevisionLocationTypeDef,
+    TargetGroupPairInfoOutputTypeDef,
     TargetGroupPairInfoTypeDef,
     TrafficRoutingConfigTypeDef,
+    TimeRangeTypeDef,
+    TriggerConfigUnionTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
     GetOnPremisesInstanceOutputTypeDef,
+    AlarmConfigurationUnionTypeDef,
+    TargetInstancesOutputTypeDef,
+    EC2TagSetUnionTypeDef,
     TargetInstancesTypeDef,
+    OnPremisesTagSetUnionTypeDef,
     CloudFormationTargetTypeDef,
     InstanceSummaryTypeDef,
     InstanceTargetTypeDef,
     LambdaTargetTypeDef,
     ECSTargetTypeDef,
     BatchGetApplicationRevisionsInputRequestTypeDef,
     GetApplicationRevisionInputRequestTypeDef,
     GetApplicationRevisionOutputTypeDef,
     ListApplicationRevisionsOutputTypeDef,
     RegisterApplicationRevisionInputRequestTypeDef,
     RevisionInfoTypeDef,
+    LoadBalancerInfoOutputTypeDef,
     LoadBalancerInfoTypeDef,
     CreateDeploymentConfigInputRequestTypeDef,
     DeploymentConfigInfoTypeDef,
+    ListDeploymentsInputListDeploymentsPaginateTypeDef,
+    ListDeploymentsInputRequestTypeDef,
     CreateDeploymentInputRequestTypeDef,
+    TargetInstancesUnionTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
     DeploymentTargetTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
-    CreateDeploymentGroupInputRequestTypeDef,
     DeploymentGroupInfoTypeDef,
     DeploymentInfoTypeDef,
+    CreateDeploymentGroupInputRequestTypeDef,
+    LoadBalancerInfoUnionTypeDef,
     UpdateDeploymentGroupInputRequestTypeDef,
     GetDeploymentConfigOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     GetDeploymentTargetOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
     GetDeploymentOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codedeploy-2.5.2/README.md` & `types-aiobotocore-codedeploy-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-codedeploy"></a>
 
 # types-aiobotocore-codedeploy
 
 [![PyPI - types-aiobotocore-codedeploy](https://img.shields.io/pypi/v/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codedeploy?color=blue)](https://pypistats.org/packages/types-aiobotocore-codedeploy)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codedeploy)](https://pepy.tech/project/types-aiobotocore-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeDeploy 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [types-aiobotocore-codedeploy docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -374,176 +374,193 @@
 )
 
 
 def check_value(value: ApplicationRevisionSortByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codedeploy.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codedeploy.type_defs import (
     TagTypeDef,
     AlarmTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
+    AutoRollbackConfigurationOutputTypeDef,
     AutoRollbackConfigurationTypeDef,
     AutoScalingGroupTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetApplicationsInputRequestTypeDef,
     BatchGetDeploymentGroupsInputRequestTypeDef,
     BatchGetDeploymentInstancesInputRequestTypeDef,
     BatchGetDeploymentTargetsInputRequestTypeDef,
     BatchGetDeploymentsInputRequestTypeDef,
     BatchGetOnPremisesInstancesInputRequestTypeDef,
     BlueInstanceTerminationOptionTypeDef,
     DeploymentReadyOptionTypeDef,
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
-    CreateApplicationOutputTypeDef,
     MinimumHealthyHostsTypeDef,
-    CreateDeploymentConfigOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
     ECSServiceTypeDef,
     TagFilterTypeDef,
-    TriggerConfigTypeDef,
-    CreateDeploymentGroupOutputTypeDef,
-    CreateDeploymentOutputTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
-    DeleteGitHubAccountTokenOutputTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
     LastDeploymentInfoTypeDef,
+    TriggerConfigOutputTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
     TargetGroupInfoTypeDef,
     ELBInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
     GenericRevisionInfoTypeDef,
     GetApplicationInputRequestTypeDef,
     GetDeploymentConfigInputRequestTypeDef,
     GetDeploymentGroupInputRequestTypeDef,
     WaiterConfigTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetDeploymentInstanceInputRequestTypeDef,
     GetDeploymentTargetInputRequestTypeDef,
     GetOnPremisesInstanceInputRequestTypeDef,
     GitHubLocationTypeDef,
     LambdaFunctionInfoTypeDef,
-    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
-    ListApplicationsOutputTypeDef,
-    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
     ListDeploymentConfigsInputRequestTypeDef,
-    ListDeploymentConfigsOutputTypeDef,
-    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     ListDeploymentGroupsInputRequestTypeDef,
-    ListDeploymentGroupsOutputTypeDef,
-    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     ListDeploymentInstancesInputRequestTypeDef,
-    ListDeploymentInstancesOutputTypeDef,
-    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
     ListDeploymentTargetsInputRequestTypeDef,
-    ListDeploymentTargetsOutputTypeDef,
-    TimeRangeTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
-    ListGitHubAccountTokenNamesOutputTypeDef,
-    ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
-    PutLifecycleEventHookExecutionStatusOutputTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
-    StopDeploymentOutputTypeDef,
+    TrafficRouteOutputTypeDef,
     TrafficRouteTypeDef,
     TimeBasedCanaryTypeDef,
     TimeBasedLinearTypeDef,
+    TimestampTypeDef,
+    TriggerConfigTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
     InstanceInfoTypeDef,
-    ListTagsForResourceOutputTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
+    AutoRollbackConfigurationUnionTypeDef,
     BatchGetApplicationsOutputTypeDef,
-    GetApplicationOutputTypeDef,
+    CreateApplicationOutputTypeDef,
+    CreateDeploymentConfigOutputTypeDef,
+    CreateDeploymentGroupOutputTypeDef,
+    CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
+    DeleteGitHubAccountTokenOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetApplicationOutputTypeDef,
+    ListApplicationsOutputTypeDef,
+    ListDeploymentConfigsOutputTypeDef,
+    ListDeploymentGroupsOutputTypeDef,
+    ListDeploymentInstancesOutputTypeDef,
+    ListDeploymentTargetsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListGitHubAccountTokenNamesOutputTypeDef,
+    ListOnPremisesInstancesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PutLifecycleEventHookExecutionStatusOutputTypeDef,
+    StopDeploymentOutputTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
     BlueGreenDeploymentConfigurationTypeDef,
+    EC2TagSetOutputTypeDef,
     EC2TagSetTypeDef,
-    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListOnPremisesInstancesInputRequestTypeDef,
+    OnPremisesTagSetOutputTypeDef,
     OnPremisesTagSetTypeDef,
     LifecycleEventTypeDef,
     ECSTaskSetTypeDef,
     GetDeploymentInputDeploymentSuccessfulWaitTypeDef,
-    ListDeploymentsInputListDeploymentsPaginateTypeDef,
-    ListDeploymentsInputRequestTypeDef,
+    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
+    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
+    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
+    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
+    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     RevisionLocationTypeDef,
+    TargetGroupPairInfoOutputTypeDef,
     TargetGroupPairInfoTypeDef,
     TrafficRoutingConfigTypeDef,
+    TimeRangeTypeDef,
+    TriggerConfigUnionTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
     GetOnPremisesInstanceOutputTypeDef,
+    AlarmConfigurationUnionTypeDef,
+    TargetInstancesOutputTypeDef,
+    EC2TagSetUnionTypeDef,
     TargetInstancesTypeDef,
+    OnPremisesTagSetUnionTypeDef,
     CloudFormationTargetTypeDef,
     InstanceSummaryTypeDef,
     InstanceTargetTypeDef,
     LambdaTargetTypeDef,
     ECSTargetTypeDef,
     BatchGetApplicationRevisionsInputRequestTypeDef,
     GetApplicationRevisionInputRequestTypeDef,
     GetApplicationRevisionOutputTypeDef,
     ListApplicationRevisionsOutputTypeDef,
     RegisterApplicationRevisionInputRequestTypeDef,
     RevisionInfoTypeDef,
+    LoadBalancerInfoOutputTypeDef,
     LoadBalancerInfoTypeDef,
     CreateDeploymentConfigInputRequestTypeDef,
     DeploymentConfigInfoTypeDef,
+    ListDeploymentsInputListDeploymentsPaginateTypeDef,
+    ListDeploymentsInputRequestTypeDef,
     CreateDeploymentInputRequestTypeDef,
+    TargetInstancesUnionTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
     DeploymentTargetTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
-    CreateDeploymentGroupInputRequestTypeDef,
     DeploymentGroupInfoTypeDef,
     DeploymentInfoTypeDef,
+    CreateDeploymentGroupInputRequestTypeDef,
+    LoadBalancerInfoUnionTypeDef,
     UpdateDeploymentGroupInputRequestTypeDef,
     GetDeploymentConfigOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     GetDeploymentTargetOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
     GetDeploymentOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codedeploy-2.5.2/setup.py` & `types-aiobotocore-codedeploy-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codedeploy",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_codedeploy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeDeploy 2.5.2 service generated with"
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
-    keywords="aiobotocore codedeploy type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore codedeploy type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codedeploy": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/"
```

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/__init__.py` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/__init__.pyi` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/__main__.py` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeDeploy 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CodeDeploy 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy\nOther"
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

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/client.py` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     ListDeploymentInstancesPaginator,
     ListDeploymentsPaginator,
     ListDeploymentTargetsPaginator,
     ListGitHubAccountTokenNamesPaginator,
     ListOnPremisesInstancesPaginator,
 )
 from .type_defs import (
-    AlarmConfigurationTypeDef,
-    AutoRollbackConfigurationTypeDef,
+    AlarmConfigurationUnionTypeDef,
+    AutoRollbackConfigurationUnionTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
     BatchGetApplicationsOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
@@ -61,15 +61,15 @@
     CreateDeploymentConfigOutputTypeDef,
     CreateDeploymentGroupOutputTypeDef,
     CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
     DeleteGitHubAccountTokenOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
-    EC2TagSetTypeDef,
+    EC2TagSetUnionTypeDef,
     ECSServiceTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationOutputTypeDef,
     GetApplicationRevisionOutputTypeDef,
     GetDeploymentConfigOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
@@ -82,26 +82,26 @@
     ListDeploymentGroupsOutputTypeDef,
     ListDeploymentInstancesOutputTypeDef,
     ListDeploymentsOutputTypeDef,
     ListDeploymentTargetsOutputTypeDef,
     ListGitHubAccountTokenNamesOutputTypeDef,
     ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoadBalancerInfoTypeDef,
+    LoadBalancerInfoUnionTypeDef,
     MinimumHealthyHostsTypeDef,
-    OnPremisesTagSetTypeDef,
+    OnPremisesTagSetUnionTypeDef,
     PutLifecycleEventHookExecutionStatusOutputTypeDef,
     RevisionLocationTypeDef,
     StopDeploymentOutputTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
-    TargetInstancesTypeDef,
+    TargetInstancesUnionTypeDef,
     TimeRangeTypeDef,
     TrafficRoutingConfigTypeDef,
-    TriggerConfigTypeDef,
+    TriggerConfigUnionTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
 )
 from .waiter import DeploymentSuccessfulWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -379,19 +379,19 @@
         *,
         applicationName: str,
         deploymentGroupName: str = ...,
         revision: RevisionLocationTypeDef = ...,
         deploymentConfigName: str = ...,
         description: str = ...,
         ignoreApplicationStopFailures: bool = ...,
-        targetInstances: TargetInstancesTypeDef = ...,
-        autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
+        targetInstances: TargetInstancesUnionTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
         updateOutdatedInstancesOnly: bool = ...,
         fileExistsBehavior: FileExistsBehaviorType = ...,
-        overrideAlarmConfiguration: AlarmConfigurationTypeDef = ...
+        overrideAlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> CreateDeploymentOutputTypeDef:
         """
         Deploys an application revision through the specified deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment)
         """
@@ -417,24 +417,24 @@
         applicationName: str,
         deploymentGroupName: str,
         serviceRoleArn: str,
         deploymentConfigName: str = ...,
         ec2TagFilters: Sequence[EC2TagFilterTypeDef] = ...,
         onPremisesInstanceTagFilters: Sequence[TagFilterTypeDef] = ...,
         autoScalingGroups: Sequence[str] = ...,
-        triggerConfigurations: Sequence[TriggerConfigTypeDef] = ...,
-        alarmConfiguration: AlarmConfigurationTypeDef = ...,
-        autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
+        triggerConfigurations: Sequence[TriggerConfigUnionTypeDef] = ...,
+        alarmConfiguration: AlarmConfigurationUnionTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
-        loadBalancerInfo: LoadBalancerInfoTypeDef = ...,
-        ec2TagSet: EC2TagSetTypeDef = ...,
+        loadBalancerInfo: LoadBalancerInfoUnionTypeDef = ...,
+        ec2TagSet: EC2TagSetUnionTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
-        onPremisesTagSet: OnPremisesTagSetTypeDef = ...,
+        onPremisesTagSet: OnPremisesTagSetUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDeploymentGroupOutputTypeDef:
         """
         Creates a deployment group to which application revisions are deployed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment_group)
@@ -816,24 +816,24 @@
         currentDeploymentGroupName: str,
         newDeploymentGroupName: str = ...,
         deploymentConfigName: str = ...,
         ec2TagFilters: Sequence[EC2TagFilterTypeDef] = ...,
         onPremisesInstanceTagFilters: Sequence[TagFilterTypeDef] = ...,
         autoScalingGroups: Sequence[str] = ...,
         serviceRoleArn: str = ...,
-        triggerConfigurations: Sequence[TriggerConfigTypeDef] = ...,
-        alarmConfiguration: AlarmConfigurationTypeDef = ...,
-        autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
+        triggerConfigurations: Sequence[TriggerConfigUnionTypeDef] = ...,
+        alarmConfiguration: AlarmConfigurationUnionTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
-        loadBalancerInfo: LoadBalancerInfoTypeDef = ...,
-        ec2TagSet: EC2TagSetTypeDef = ...,
+        loadBalancerInfo: LoadBalancerInfoUnionTypeDef = ...,
+        ec2TagSet: EC2TagSetUnionTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
-        onPremisesTagSet: OnPremisesTagSetTypeDef = ...
+        onPremisesTagSet: OnPremisesTagSetUnionTypeDef = ...
     ) -> UpdateDeploymentGroupOutputTypeDef:
         """
         Changes information about a deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.update_deployment_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#update_deployment_group)
         """
```

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/client.pyi` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     ListDeploymentInstancesPaginator,
     ListDeploymentsPaginator,
     ListDeploymentTargetsPaginator,
     ListGitHubAccountTokenNamesPaginator,
     ListOnPremisesInstancesPaginator,
 )
 from .type_defs import (
-    AlarmConfigurationTypeDef,
-    AutoRollbackConfigurationTypeDef,
+    AlarmConfigurationUnionTypeDef,
+    AutoRollbackConfigurationUnionTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
     BatchGetApplicationsOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
@@ -61,15 +61,15 @@
     CreateDeploymentConfigOutputTypeDef,
     CreateDeploymentGroupOutputTypeDef,
     CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
     DeleteGitHubAccountTokenOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
-    EC2TagSetTypeDef,
+    EC2TagSetUnionTypeDef,
     ECSServiceTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationOutputTypeDef,
     GetApplicationRevisionOutputTypeDef,
     GetDeploymentConfigOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
@@ -82,26 +82,26 @@
     ListDeploymentGroupsOutputTypeDef,
     ListDeploymentInstancesOutputTypeDef,
     ListDeploymentsOutputTypeDef,
     ListDeploymentTargetsOutputTypeDef,
     ListGitHubAccountTokenNamesOutputTypeDef,
     ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoadBalancerInfoTypeDef,
+    LoadBalancerInfoUnionTypeDef,
     MinimumHealthyHostsTypeDef,
-    OnPremisesTagSetTypeDef,
+    OnPremisesTagSetUnionTypeDef,
     PutLifecycleEventHookExecutionStatusOutputTypeDef,
     RevisionLocationTypeDef,
     StopDeploymentOutputTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
-    TargetInstancesTypeDef,
+    TargetInstancesUnionTypeDef,
     TimeRangeTypeDef,
     TrafficRoutingConfigTypeDef,
-    TriggerConfigTypeDef,
+    TriggerConfigUnionTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
 )
 from .waiter import DeploymentSuccessfulWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -362,19 +362,19 @@
         *,
         applicationName: str,
         deploymentGroupName: str = ...,
         revision: RevisionLocationTypeDef = ...,
         deploymentConfigName: str = ...,
         description: str = ...,
         ignoreApplicationStopFailures: bool = ...,
-        targetInstances: TargetInstancesTypeDef = ...,
-        autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
+        targetInstances: TargetInstancesUnionTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
         updateOutdatedInstancesOnly: bool = ...,
         fileExistsBehavior: FileExistsBehaviorType = ...,
-        overrideAlarmConfiguration: AlarmConfigurationTypeDef = ...
+        overrideAlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
     ) -> CreateDeploymentOutputTypeDef:
         """
         Deploys an application revision through the specified deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment)
         """
@@ -398,24 +398,24 @@
         applicationName: str,
         deploymentGroupName: str,
         serviceRoleArn: str,
         deploymentConfigName: str = ...,
         ec2TagFilters: Sequence[EC2TagFilterTypeDef] = ...,
         onPremisesInstanceTagFilters: Sequence[TagFilterTypeDef] = ...,
         autoScalingGroups: Sequence[str] = ...,
-        triggerConfigurations: Sequence[TriggerConfigTypeDef] = ...,
-        alarmConfiguration: AlarmConfigurationTypeDef = ...,
-        autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
+        triggerConfigurations: Sequence[TriggerConfigUnionTypeDef] = ...,
+        alarmConfiguration: AlarmConfigurationUnionTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
-        loadBalancerInfo: LoadBalancerInfoTypeDef = ...,
-        ec2TagSet: EC2TagSetTypeDef = ...,
+        loadBalancerInfo: LoadBalancerInfoUnionTypeDef = ...,
+        ec2TagSet: EC2TagSetUnionTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
-        onPremisesTagSet: OnPremisesTagSetTypeDef = ...,
+        onPremisesTagSet: OnPremisesTagSetUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDeploymentGroupOutputTypeDef:
         """
         Creates a deployment group to which application revisions are deployed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment_group)
@@ -762,24 +762,24 @@
         currentDeploymentGroupName: str,
         newDeploymentGroupName: str = ...,
         deploymentConfigName: str = ...,
         ec2TagFilters: Sequence[EC2TagFilterTypeDef] = ...,
         onPremisesInstanceTagFilters: Sequence[TagFilterTypeDef] = ...,
         autoScalingGroups: Sequence[str] = ...,
         serviceRoleArn: str = ...,
-        triggerConfigurations: Sequence[TriggerConfigTypeDef] = ...,
-        alarmConfiguration: AlarmConfigurationTypeDef = ...,
-        autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
+        triggerConfigurations: Sequence[TriggerConfigUnionTypeDef] = ...,
+        alarmConfiguration: AlarmConfigurationUnionTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
-        loadBalancerInfo: LoadBalancerInfoTypeDef = ...,
-        ec2TagSet: EC2TagSetTypeDef = ...,
+        loadBalancerInfo: LoadBalancerInfoUnionTypeDef = ...,
+        ec2TagSet: EC2TagSetUnionTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
-        onPremisesTagSet: OnPremisesTagSetTypeDef = ...
+        onPremisesTagSet: OnPremisesTagSetUnionTypeDef = ...
     ) -> UpdateDeploymentGroupOutputTypeDef:
         """
         Changes information about a deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.update_deployment_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#update_deployment_group)
         """
```

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/literals.py` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/literals.pyi` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/paginator.py` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -74,25 +74,22 @@
     "ListDeploymentInstancesPaginator",
     "ListDeploymentTargetsPaginator",
     "ListDeploymentsPaginator",
     "ListGitHubAccountTokenNamesPaginator",
     "ListOnPremisesInstancesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListApplicationRevisionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listapplicationrevisionspaginator)
     """
 
     def paginate(
@@ -100,153 +97,145 @@
         *,
         applicationName: str,
         sortBy: ApplicationRevisionSortByType = ...,
         sortOrder: SortOrderType = ...,
         s3Bucket: str = ...,
         s3KeyPrefix: str = ...,
         deployed: ListStateFilterActionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationRevisionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listapplicationrevisionspaginator)
         """
 
-
 class ListApplicationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listapplicationspaginator)
         """
 
-
 class ListDeploymentConfigsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentConfigsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentconfigspaginator)
         """
 
-
 class ListDeploymentGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentgroupspaginator)
     """
 
     def paginate(
-        self, *, applicationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, applicationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentgroupspaginator)
         """
 
-
 class ListDeploymentInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         deploymentId: str,
         instanceStatusFilter: Sequence[InstanceStatusType] = ...,
         instanceTypeFilter: Sequence[InstanceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentinstancespaginator)
         """
 
-
 class ListDeploymentTargetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymenttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         deploymentId: str = ...,
         targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentTargetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymenttargetspaginator)
         """
 
-
 class ListDeploymentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
         self,
         *,
         applicationName: str = ...,
         deploymentGroupName: str = ...,
         externalId: str = ...,
         includeOnlyStatuses: Sequence[DeploymentStatusType] = ...,
         createTimeRange: TimeRangeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentspaginator)
         """
 
-
 class ListGitHubAccountTokenNamesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listgithubaccounttokennamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGitHubAccountTokenNamesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listgithubaccounttokennamespaginator)
         """
 
-
 class ListOnPremisesInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listonpremisesinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOnPremisesInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listonpremisesinstancespaginator)
         """
```

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/paginator.pyi` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,22 +74,25 @@
     "ListDeploymentInstancesPaginator",
     "ListDeploymentTargetsPaginator",
     "ListDeploymentsPaginator",
     "ListGitHubAccountTokenNamesPaginator",
     "ListOnPremisesInstancesPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListApplicationRevisionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listapplicationrevisionspaginator)
     """
 
     def paginate(
@@ -97,145 +100,153 @@
         *,
         applicationName: str,
         sortBy: ApplicationRevisionSortByType = ...,
         sortOrder: SortOrderType = ...,
         s3Bucket: str = ...,
         s3KeyPrefix: str = ...,
         deployed: ListStateFilterActionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationRevisionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplicationRevisions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listapplicationrevisionspaginator)
         """
 
+
 class ListApplicationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApplicationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListApplications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listapplicationspaginator)
         """
 
+
 class ListDeploymentConfigsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentConfigsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentconfigspaginator)
         """
 
+
 class ListDeploymentGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentgroupspaginator)
     """
 
     def paginate(
-        self, *, applicationName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, applicationName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentgroupspaginator)
         """
 
+
 class ListDeploymentInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         deploymentId: str,
         instanceStatusFilter: Sequence[InstanceStatusType] = ...,
         instanceTypeFilter: Sequence[InstanceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentinstancespaginator)
         """
 
+
 class ListDeploymentTargetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymenttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         deploymentId: str = ...,
         targetFilters: Mapping[TargetFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentTargetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeploymentTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymenttargetspaginator)
         """
 
+
 class ListDeploymentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentspaginator)
     """
 
     def paginate(
         self,
         *,
         applicationName: str = ...,
         deploymentGroupName: str = ...,
         externalId: str = ...,
         includeOnlyStatuses: Sequence[DeploymentStatusType] = ...,
         createTimeRange: TimeRangeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDeploymentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listdeploymentspaginator)
         """
 
+
 class ListGitHubAccountTokenNamesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listgithubaccounttokennamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGitHubAccountTokenNamesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListGitHubAccountTokenNames.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listgithubaccounttokennamespaginator)
         """
 
+
 class ListOnPremisesInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listonpremisesinstancespaginator)
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOnPremisesInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Paginator.ListOnPremisesInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/paginators/#listonpremisesinstancespaginator)
         """
```

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/type_defs.py` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codedeploy.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -52,157 +52,173 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
     "AlarmTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
+    "AutoRollbackConfigurationOutputTypeDef",
     "AutoRollbackConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetApplicationsInputRequestTypeDef",
     "BatchGetDeploymentGroupsInputRequestTypeDef",
     "BatchGetDeploymentInstancesInputRequestTypeDef",
     "BatchGetDeploymentTargetsInputRequestTypeDef",
     "BatchGetDeploymentsInputRequestTypeDef",
     "BatchGetOnPremisesInstancesInputRequestTypeDef",
     "BlueInstanceTerminationOptionTypeDef",
     "DeploymentReadyOptionTypeDef",
     "GreenFleetProvisioningOptionTypeDef",
     "ContinueDeploymentInputRequestTypeDef",
-    "CreateApplicationOutputTypeDef",
     "MinimumHealthyHostsTypeDef",
-    "CreateDeploymentConfigOutputTypeDef",
     "DeploymentStyleTypeDef",
     "EC2TagFilterTypeDef",
     "ECSServiceTypeDef",
     "TagFilterTypeDef",
-    "TriggerConfigTypeDef",
-    "CreateDeploymentGroupOutputTypeDef",
-    "CreateDeploymentOutputTypeDef",
     "DeleteApplicationInputRequestTypeDef",
     "DeleteDeploymentConfigInputRequestTypeDef",
     "DeleteDeploymentGroupInputRequestTypeDef",
     "DeleteGitHubAccountTokenInputRequestTypeDef",
-    "DeleteGitHubAccountTokenOutputTypeDef",
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     "LastDeploymentInfoTypeDef",
+    "TriggerConfigOutputTypeDef",
     "DeploymentOverviewTypeDef",
     "ErrorInformationTypeDef",
     "RelatedDeploymentsTypeDef",
     "RollbackInfoTypeDef",
     "DeregisterOnPremisesInstanceInputRequestTypeDef",
     "DiagnosticsTypeDef",
     "TargetGroupInfoTypeDef",
     "ELBInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GenericRevisionInfoTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetDeploymentConfigInputRequestTypeDef",
     "GetDeploymentGroupInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetDeploymentInputRequestTypeDef",
     "GetDeploymentInstanceInputRequestTypeDef",
     "GetDeploymentTargetInputRequestTypeDef",
     "GetOnPremisesInstanceInputRequestTypeDef",
     "GitHubLocationTypeDef",
     "LambdaFunctionInfoTypeDef",
-    "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationRevisionsInputRequestTypeDef",
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListApplicationsInputRequestTypeDef",
-    "ListApplicationsOutputTypeDef",
-    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
     "ListDeploymentConfigsInputRequestTypeDef",
-    "ListDeploymentConfigsOutputTypeDef",
-    "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     "ListDeploymentGroupsInputRequestTypeDef",
-    "ListDeploymentGroupsOutputTypeDef",
-    "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
     "ListDeploymentInstancesInputRequestTypeDef",
-    "ListDeploymentInstancesOutputTypeDef",
-    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
     "ListDeploymentTargetsInputRequestTypeDef",
-    "ListDeploymentTargetsOutputTypeDef",
-    "TimeRangeTypeDef",
-    "ListDeploymentsOutputTypeDef",
-    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
-    "ListGitHubAccountTokenNamesOutputTypeDef",
-    "ListOnPremisesInstancesOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
-    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
     "RawStringTypeDef",
     "RegisterOnPremisesInstanceInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "S3LocationTypeDef",
     "SkipWaitTimeForInstanceTerminationInputRequestTypeDef",
     "StopDeploymentInputRequestTypeDef",
-    "StopDeploymentOutputTypeDef",
+    "TrafficRouteOutputTypeDef",
     "TrafficRouteTypeDef",
     "TimeBasedCanaryTypeDef",
     "TimeBasedLinearTypeDef",
+    "TimestampTypeDef",
+    "TriggerConfigTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApplicationInputRequestTypeDef",
     "AddTagsToOnPremisesInstancesInputRequestTypeDef",
     "CreateApplicationInputRequestTypeDef",
     "InstanceInfoTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
+    "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
+    "AutoRollbackConfigurationUnionTypeDef",
     "BatchGetApplicationsOutputTypeDef",
-    "GetApplicationOutputTypeDef",
+    "CreateApplicationOutputTypeDef",
+    "CreateDeploymentConfigOutputTypeDef",
+    "CreateDeploymentGroupOutputTypeDef",
+    "CreateDeploymentOutputTypeDef",
     "DeleteDeploymentGroupOutputTypeDef",
+    "DeleteGitHubAccountTokenOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetApplicationOutputTypeDef",
+    "ListApplicationsOutputTypeDef",
+    "ListDeploymentConfigsOutputTypeDef",
+    "ListDeploymentGroupsOutputTypeDef",
+    "ListDeploymentInstancesOutputTypeDef",
+    "ListDeploymentTargetsOutputTypeDef",
+    "ListDeploymentsOutputTypeDef",
+    "ListGitHubAccountTokenNamesOutputTypeDef",
+    "ListOnPremisesInstancesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
+    "StopDeploymentOutputTypeDef",
     "UpdateDeploymentGroupOutputTypeDef",
     "BlueGreenDeploymentConfigurationTypeDef",
+    "EC2TagSetOutputTypeDef",
     "EC2TagSetTypeDef",
-    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "ListOnPremisesInstancesInputRequestTypeDef",
+    "OnPremisesTagSetOutputTypeDef",
     "OnPremisesTagSetTypeDef",
     "LifecycleEventTypeDef",
     "ECSTaskSetTypeDef",
     "GetDeploymentInputDeploymentSuccessfulWaitTypeDef",
-    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
-    "ListDeploymentsInputRequestTypeDef",
+    "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
+    "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
+    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
+    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "RevisionLocationTypeDef",
+    "TargetGroupPairInfoOutputTypeDef",
     "TargetGroupPairInfoTypeDef",
     "TrafficRoutingConfigTypeDef",
+    "TimeRangeTypeDef",
+    "TriggerConfigUnionTypeDef",
     "BatchGetOnPremisesInstancesOutputTypeDef",
     "GetOnPremisesInstanceOutputTypeDef",
+    "AlarmConfigurationUnionTypeDef",
+    "TargetInstancesOutputTypeDef",
+    "EC2TagSetUnionTypeDef",
     "TargetInstancesTypeDef",
+    "OnPremisesTagSetUnionTypeDef",
     "CloudFormationTargetTypeDef",
     "InstanceSummaryTypeDef",
     "InstanceTargetTypeDef",
     "LambdaTargetTypeDef",
     "ECSTargetTypeDef",
     "BatchGetApplicationRevisionsInputRequestTypeDef",
     "GetApplicationRevisionInputRequestTypeDef",
     "GetApplicationRevisionOutputTypeDef",
     "ListApplicationRevisionsOutputTypeDef",
     "RegisterApplicationRevisionInputRequestTypeDef",
     "RevisionInfoTypeDef",
+    "LoadBalancerInfoOutputTypeDef",
     "LoadBalancerInfoTypeDef",
     "CreateDeploymentConfigInputRequestTypeDef",
     "DeploymentConfigInfoTypeDef",
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    "ListDeploymentsInputRequestTypeDef",
     "CreateDeploymentInputRequestTypeDef",
+    "TargetInstancesUnionTypeDef",
     "BatchGetDeploymentInstancesOutputTypeDef",
     "GetDeploymentInstanceOutputTypeDef",
     "DeploymentTargetTypeDef",
     "BatchGetApplicationRevisionsOutputTypeDef",
-    "CreateDeploymentGroupInputRequestTypeDef",
     "DeploymentGroupInfoTypeDef",
     "DeploymentInfoTypeDef",
+    "CreateDeploymentGroupInputRequestTypeDef",
+    "LoadBalancerInfoUnionTypeDef",
     "UpdateDeploymentGroupInputRequestTypeDef",
     "GetDeploymentConfigOutputTypeDef",
     "BatchGetDeploymentTargetsOutputTypeDef",
     "GetDeploymentTargetOutputTypeDef",
     "BatchGetDeploymentGroupsOutputTypeDef",
     "GetDeploymentGroupOutputTypeDef",
     "BatchGetDeploymentsOutputTypeDef",
@@ -244,32 +260,52 @@
         "linkedToGitHub": bool,
         "gitHubAccountName": str,
         "computePlatform": ComputePlatformType,
     },
     total=False,
 )
 
+AutoRollbackConfigurationOutputTypeDef = TypedDict(
+    "AutoRollbackConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "events": List[AutoRollbackEventType],
+    },
+    total=False,
+)
+
 AutoRollbackConfigurationTypeDef = TypedDict(
     "AutoRollbackConfigurationTypeDef",
     {
         "enabled": bool,
-        "events": List[AutoRollbackEventType],
+        "events": Sequence[AutoRollbackEventType],
     },
     total=False,
 )
 
 AutoScalingGroupTypeDef = TypedDict(
     "AutoScalingGroupTypeDef",
     {
         "name": str,
         "hook": str,
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
 BatchGetApplicationsInputRequestTypeDef = TypedDict(
     "BatchGetApplicationsInputRequestTypeDef",
     {
         "applicationNames": Sequence[str],
     },
 )
 
@@ -343,39 +379,23 @@
     {
         "deploymentId": str,
         "deploymentWaitType": DeploymentWaitTypeType,
     },
     total=False,
 )
 
-CreateApplicationOutputTypeDef = TypedDict(
-    "CreateApplicationOutputTypeDef",
-    {
-        "applicationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MinimumHealthyHostsTypeDef = TypedDict(
     "MinimumHealthyHostsTypeDef",
     {
         "type": MinimumHealthyHostsTypeType,
         "value": int,
     },
     total=False,
 )
 
-CreateDeploymentConfigOutputTypeDef = TypedDict(
-    "CreateDeploymentConfigOutputTypeDef",
-    {
-        "deploymentConfigId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentStyleTypeDef = TypedDict(
     "DeploymentStyleTypeDef",
     {
         "deploymentType": DeploymentTypeType,
         "deploymentOption": DeploymentOptionType,
     },
     total=False,
@@ -406,40 +426,14 @@
         "Key": str,
         "Value": str,
         "Type": TagFilterTypeType,
     },
     total=False,
 )
 
-TriggerConfigTypeDef = TypedDict(
-    "TriggerConfigTypeDef",
-    {
-        "triggerName": str,
-        "triggerTargetArn": str,
-        "triggerEvents": List[TriggerEventTypeType],
-    },
-    total=False,
-)
-
-CreateDeploymentGroupOutputTypeDef = TypedDict(
-    "CreateDeploymentGroupOutputTypeDef",
-    {
-        "deploymentGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDeploymentOutputTypeDef = TypedDict(
-    "CreateDeploymentOutputTypeDef",
-    {
-        "deploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationInputRequestTypeDef = TypedDict(
     "DeleteApplicationInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 
@@ -462,22 +456,14 @@
     "DeleteGitHubAccountTokenInputRequestTypeDef",
     {
         "tokenName": str,
     },
     total=False,
 )
 
-DeleteGitHubAccountTokenOutputTypeDef = TypedDict(
-    "DeleteGitHubAccountTokenOutputTypeDef",
-    {
-        "tokenName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteResourcesByExternalIdInputRequestTypeDef = TypedDict(
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     {
         "externalId": str,
     },
     total=False,
 )
@@ -489,14 +475,24 @@
         "status": DeploymentStatusType,
         "endTime": datetime,
         "createTime": datetime,
     },
     total=False,
 )
 
+TriggerConfigOutputTypeDef = TypedDict(
+    "TriggerConfigOutputTypeDef",
+    {
+        "triggerName": str,
+        "triggerTargetArn": str,
+        "triggerEvents": List[TriggerEventTypeType],
+    },
+    total=False,
+)
+
 DeploymentOverviewTypeDef = TypedDict(
     "DeploymentOverviewTypeDef",
     {
         "Pending": int,
         "InProgress": int,
         "Succeeded": int,
         "Failed": int,
@@ -564,21 +560,14 @@
     "ELBInfoTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GenericRevisionInfoTypeDef = TypedDict(
     "GenericRevisionInfoTypeDef",
     {
         "description": str,
         "deploymentGroups": List[str],
         "firstUsedTime": datetime,
         "lastUsedTime": datetime,
@@ -666,41 +655,24 @@
         "currentVersion": str,
         "targetVersion": str,
         "targetVersionWeight": float,
     },
     total=False,
 )
 
-_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
-    {
-        "applicationName": str,
-    },
-)
-_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "sortBy": ApplicationRevisionSortByType,
-        "sortOrder": SortOrderType,
-        "s3Bucket": str,
-        "s3KeyPrefix": str,
-        "deployed": ListStateFilterActionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
-    _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-    _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListApplicationRevisionsInputRequestTypeDef = TypedDict(
     "_RequiredListApplicationRevisionsInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListApplicationRevisionsInputRequestTypeDef = TypedDict(
@@ -712,150 +684,56 @@
         "s3KeyPrefix": str,
         "deployed": ListStateFilterActionType,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListApplicationRevisionsInputRequestTypeDef(
     _RequiredListApplicationRevisionsInputRequestTypeDef,
     _OptionalListApplicationRevisionsInputRequestTypeDef,
 ):
     pass
 
-
-ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListApplicationsInputRequestTypeDef = TypedDict(
     "ListApplicationsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListApplicationsOutputTypeDef = TypedDict(
-    "ListApplicationsOutputTypeDef",
-    {
-        "applications": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = TypedDict(
-    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeploymentConfigsInputRequestTypeDef = TypedDict(
     "ListDeploymentConfigsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListDeploymentConfigsOutputTypeDef = TypedDict(
-    "ListDeploymentConfigsOutputTypeDef",
-    {
-        "deploymentConfigsList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    {
-        "applicationName": str,
-    },
-)
-_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
-    _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-    _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDeploymentGroupsInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentGroupsInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListDeploymentGroupsInputRequestTypeDef = TypedDict(
     "_OptionalListDeploymentGroupsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListDeploymentGroupsInputRequestTypeDef(
     _RequiredListDeploymentGroupsInputRequestTypeDef,
     _OptionalListDeploymentGroupsInputRequestTypeDef,
 ):
     pass
 
-
-ListDeploymentGroupsOutputTypeDef = TypedDict(
-    "ListDeploymentGroupsOutputTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    {
-        "deploymentId": str,
-    },
-)
-_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    {
-        "instanceStatusFilter": Sequence[InstanceStatusType],
-        "instanceTypeFilter": Sequence[InstanceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
-    _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-    _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDeploymentInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentInstancesInputRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
 _OptionalListDeploymentInstancesInputRequestTypeDef = TypedDict(
@@ -864,161 +742,67 @@
         "nextToken": str,
         "instanceStatusFilter": Sequence[InstanceStatusType],
         "instanceTypeFilter": Sequence[InstanceTypeType],
     },
     total=False,
 )
 
-
 class ListDeploymentInstancesInputRequestTypeDef(
     _RequiredListDeploymentInstancesInputRequestTypeDef,
     _OptionalListDeploymentInstancesInputRequestTypeDef,
 ):
     pass
 
-
-ListDeploymentInstancesOutputTypeDef = TypedDict(
-    "ListDeploymentInstancesOutputTypeDef",
-    {
-        "instancesList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
-    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
-    {
-        "deploymentId": str,
-        "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeploymentTargetsInputRequestTypeDef = TypedDict(
     "ListDeploymentTargetsInputRequestTypeDef",
     {
         "deploymentId": str,
         "nextToken": str,
         "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
     },
     total=False,
 )
 
-ListDeploymentTargetsOutputTypeDef = TypedDict(
-    "ListDeploymentTargetsOutputTypeDef",
-    {
-        "targetIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "start": Union[datetime, str],
-        "end": Union[datetime, str],
-    },
-    total=False,
-)
-
-ListDeploymentsOutputTypeDef = TypedDict(
-    "ListDeploymentsOutputTypeDef",
-    {
-        "deployments": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = TypedDict(
-    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGitHubAccountTokenNamesInputRequestTypeDef = TypedDict(
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListGitHubAccountTokenNamesOutputTypeDef = TypedDict(
-    "ListGitHubAccountTokenNamesOutputTypeDef",
-    {
-        "tokenNameList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListOnPremisesInstancesOutputTypeDef = TypedDict(
-    "ListOnPremisesInstancesOutputTypeDef",
-    {
-        "instanceNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
     "_OptionalListTagsForResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
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
 PutLifecycleEventHookExecutionStatusInputRequestTypeDef = TypedDict(
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     {
         "deploymentId": str,
         "lifecycleEventHookExecutionId": str,
         "status": LifecycleEventStatusType,
     },
     total=False,
 )
 
-PutLifecycleEventHookExecutionStatusOutputTypeDef = TypedDict(
-    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
-    {
-        "lifecycleEventHookExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RawStringTypeDef = TypedDict(
     "RawStringTypeDef",
     {
         "content": str,
         "sha256": str,
     },
     total=False,
@@ -1035,33 +819,20 @@
     {
         "iamSessionArn": str,
         "iamUserArn": str,
     },
     total=False,
 )
 
-
 class RegisterOnPremisesInstanceInputRequestTypeDef(
     _RequiredRegisterOnPremisesInstanceInputRequestTypeDef,
     _OptionalRegisterOnPremisesInstanceInputRequestTypeDef,
 ):
     pass
 
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
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "bundleType": BundleTypeType,
         "version": str,
@@ -1088,34 +859,31 @@
     "_OptionalStopDeploymentInputRequestTypeDef",
     {
         "autoRollbackEnabled": bool,
     },
     total=False,
 )
 
-
 class StopDeploymentInputRequestTypeDef(
     _RequiredStopDeploymentInputRequestTypeDef, _OptionalStopDeploymentInputRequestTypeDef
 ):
     pass
 
-
-StopDeploymentOutputTypeDef = TypedDict(
-    "StopDeploymentOutputTypeDef",
+TrafficRouteOutputTypeDef = TypedDict(
+    "TrafficRouteOutputTypeDef",
     {
-        "status": StopStatusType,
-        "statusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "listenerArns": List[str],
     },
+    total=False,
 )
 
 TrafficRouteTypeDef = TypedDict(
     "TrafficRouteTypeDef",
     {
-        "listenerArns": List[str],
+        "listenerArns": Sequence[str],
     },
     total=False,
 )
 
 TimeBasedCanaryTypeDef = TypedDict(
     "TimeBasedCanaryTypeDef",
     {
@@ -1130,14 +898,25 @@
     {
         "linearPercentage": int,
         "linearInterval": int,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
+TriggerConfigTypeDef = TypedDict(
+    "TriggerConfigTypeDef",
+    {
+        "triggerName": str,
+        "triggerTargetArn": str,
+        "triggerEvents": Sequence[TriggerEventTypeType],
+    },
+    total=False,
+)
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1170,44 +949,33 @@
     {
         "computePlatform": ComputePlatformType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateApplicationInputRequestTypeDef(
     _RequiredCreateApplicationInputRequestTypeDef, _OptionalCreateApplicationInputRequestTypeDef
 ):
     pass
 
-
 InstanceInfoTypeDef = TypedDict(
     "InstanceInfoTypeDef",
     {
         "instanceName": str,
         "iamSessionArn": str,
         "iamUserArn": str,
         "instanceArn": str,
         "registerTime": datetime,
         "deregisterTime": datetime,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
         "instanceNames": Sequence[str],
     },
 )
@@ -1216,98 +984,263 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+AlarmConfigurationOutputTypeDef = TypedDict(
+    "AlarmConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "ignorePollAlarmFailure": bool,
+        "alarms": List[AlarmTypeDef],
+    },
+    total=False,
+)
+
 AlarmConfigurationTypeDef = TypedDict(
     "AlarmConfigurationTypeDef",
     {
         "enabled": bool,
         "ignorePollAlarmFailure": bool,
-        "alarms": List[AlarmTypeDef],
+        "alarms": Sequence[AlarmTypeDef],
     },
     total=False,
 )
 
+AutoRollbackConfigurationUnionTypeDef = Union[
+    AutoRollbackConfigurationTypeDef, AutoRollbackConfigurationOutputTypeDef
+]
 BatchGetApplicationsOutputTypeDef = TypedDict(
     "BatchGetApplicationsOutputTypeDef",
     {
         "applicationsInfo": List[ApplicationInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetApplicationOutputTypeDef = TypedDict(
-    "GetApplicationOutputTypeDef",
+CreateApplicationOutputTypeDef = TypedDict(
+    "CreateApplicationOutputTypeDef",
     {
-        "application": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "applicationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentConfigOutputTypeDef = TypedDict(
+    "CreateDeploymentConfigOutputTypeDef",
+    {
+        "deploymentConfigId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentGroupOutputTypeDef = TypedDict(
+    "CreateDeploymentGroupOutputTypeDef",
+    {
+        "deploymentGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentOutputTypeDef = TypedDict(
+    "CreateDeploymentOutputTypeDef",
+    {
+        "deploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDeploymentGroupOutputTypeDef = TypedDict(
     "DeleteDeploymentGroupOutputTypeDef",
     {
         "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGitHubAccountTokenOutputTypeDef = TypedDict(
+    "DeleteGitHubAccountTokenOutputTypeDef",
+    {
+        "tokenName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApplicationOutputTypeDef = TypedDict(
+    "GetApplicationOutputTypeDef",
+    {
+        "application": ApplicationInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsOutputTypeDef = TypedDict(
+    "ListApplicationsOutputTypeDef",
+    {
+        "applications": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentConfigsOutputTypeDef = TypedDict(
+    "ListDeploymentConfigsOutputTypeDef",
+    {
+        "deploymentConfigsList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentGroupsOutputTypeDef = TypedDict(
+    "ListDeploymentGroupsOutputTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentInstancesOutputTypeDef = TypedDict(
+    "ListDeploymentInstancesOutputTypeDef",
+    {
+        "instancesList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentTargetsOutputTypeDef = TypedDict(
+    "ListDeploymentTargetsOutputTypeDef",
+    {
+        "targetIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentsOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputTypeDef",
+    {
+        "deployments": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGitHubAccountTokenNamesOutputTypeDef = TypedDict(
+    "ListGitHubAccountTokenNamesOutputTypeDef",
+    {
+        "tokenNameList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOnPremisesInstancesOutputTypeDef = TypedDict(
+    "ListOnPremisesInstancesOutputTypeDef",
+    {
+        "instanceNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutLifecycleEventHookExecutionStatusOutputTypeDef = TypedDict(
+    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
+    {
+        "lifecycleEventHookExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDeploymentOutputTypeDef = TypedDict(
+    "StopDeploymentOutputTypeDef",
+    {
+        "status": StopStatusType,
+        "statusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDeploymentGroupOutputTypeDef = TypedDict(
     "UpdateDeploymentGroupOutputTypeDef",
     {
         "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BlueGreenDeploymentConfigurationTypeDef = TypedDict(
     "BlueGreenDeploymentConfigurationTypeDef",
     {
         "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionTypeDef,
         "deploymentReadyOption": DeploymentReadyOptionTypeDef,
         "greenFleetProvisioningOption": GreenFleetProvisioningOptionTypeDef,
     },
     total=False,
 )
 
-EC2TagSetTypeDef = TypedDict(
-    "EC2TagSetTypeDef",
+EC2TagSetOutputTypeDef = TypedDict(
+    "EC2TagSetOutputTypeDef",
     {
         "ec2TagSetList": List[List[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
-ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
-    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
+EC2TagSetTypeDef = TypedDict(
+    "EC2TagSetTypeDef",
     {
-        "registrationStatus": RegistrationStatusType,
-        "tagFilters": Sequence[TagFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ec2TagSetList": Sequence[Sequence[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
 ListOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "ListOnPremisesInstancesInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
         "tagFilters": Sequence[TagFilterTypeDef],
         "nextToken": str,
     },
     total=False,
 )
 
+OnPremisesTagSetOutputTypeDef = TypedDict(
+    "OnPremisesTagSetOutputTypeDef",
+    {
+        "onPremisesTagSetList": List[List[TagFilterTypeDef]],
+    },
+    total=False,
+)
+
 OnPremisesTagSetTypeDef = TypedDict(
     "OnPremisesTagSetTypeDef",
     {
-        "onPremisesTagSetList": List[List[TagFilterTypeDef]],
+        "onPremisesTagSetList": Sequence[Sequence[TagFilterTypeDef]],
     },
     total=False,
 )
 
 LifecycleEventTypeDef = TypedDict(
     "LifecycleEventTypeDef",
     {
@@ -1345,44 +1278,127 @@
     "_OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetDeploymentInputDeploymentSuccessfulWaitTypeDef(
     _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
     _OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
 ):
     pass
 
-
-ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
-    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     {
         "applicationName": str,
-        "deploymentGroupName": str,
-        "externalId": str,
-        "includeOnlyStatuses": Sequence[DeploymentStatusType],
-        "createTimeRange": TimeRangeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+)
+_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    {
+        "sortBy": ApplicationRevisionSortByType,
+        "sortOrder": SortOrderType,
+        "s3Bucket": str,
+        "s3KeyPrefix": str,
+        "deployed": ListStateFilterActionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListDeploymentsInputRequestTypeDef = TypedDict(
-    "ListDeploymentsInputRequestTypeDef",
+class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
+    _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+):
+    pass
+
+ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = TypedDict(
+    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     {
         "applicationName": str,
-        "deploymentGroupName": str,
-        "externalId": str,
-        "includeOnlyStatuses": Sequence[DeploymentStatusType],
-        "createTimeRange": TimeRangeTypeDef,
-        "nextToken": str,
+    },
+)
+_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
+    _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+    _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    {
+        "deploymentId": str,
+    },
+)
+_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    {
+        "instanceStatusFilter": Sequence[InstanceStatusType],
+        "instanceTypeFilter": Sequence[InstanceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
+    _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+    _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+):
+    pass
+
+ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
+    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
+    {
+        "deploymentId": str,
+        "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = TypedDict(
+    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
+    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
+    {
+        "registrationStatus": RegistrationStatusType,
+        "tagFilters": Sequence[TagFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 RevisionLocationTypeDef = TypedDict(
     "RevisionLocationTypeDef",
     {
@@ -1391,18 +1407,28 @@
         "gitHubLocation": GitHubLocationTypeDef,
         "string": RawStringTypeDef,
         "appSpecContent": AppSpecContentTypeDef,
     },
     total=False,
 )
 
+TargetGroupPairInfoOutputTypeDef = TypedDict(
+    "TargetGroupPairInfoOutputTypeDef",
+    {
+        "targetGroups": List[TargetGroupInfoTypeDef],
+        "prodTrafficRoute": TrafficRouteOutputTypeDef,
+        "testTrafficRoute": TrafficRouteOutputTypeDef,
+    },
+    total=False,
+)
+
 TargetGroupPairInfoTypeDef = TypedDict(
     "TargetGroupPairInfoTypeDef",
     {
-        "targetGroups": List[TargetGroupInfoTypeDef],
+        "targetGroups": Sequence[TargetGroupInfoTypeDef],
         "prodTrafficRoute": TrafficRouteTypeDef,
         "testTrafficRoute": TrafficRouteTypeDef,
     },
     total=False,
 )
 
 TrafficRoutingConfigTypeDef = TypedDict(
@@ -1411,40 +1437,63 @@
         "type": TrafficRoutingTypeType,
         "timeBasedCanary": TimeBasedCanaryTypeDef,
         "timeBasedLinear": TimeBasedLinearTypeDef,
     },
     total=False,
 )
 
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "start": TimestampTypeDef,
+        "end": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TriggerConfigUnionTypeDef = Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
 BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
     "BatchGetOnPremisesInstancesOutputTypeDef",
     {
         "instanceInfos": List[InstanceInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOnPremisesInstanceOutputTypeDef = TypedDict(
     "GetOnPremisesInstanceOutputTypeDef",
     {
         "instanceInfo": InstanceInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TargetInstancesTypeDef = TypedDict(
-    "TargetInstancesTypeDef",
+AlarmConfigurationUnionTypeDef = Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef]
+TargetInstancesOutputTypeDef = TypedDict(
+    "TargetInstancesOutputTypeDef",
     {
         "tagFilters": List[EC2TagFilterTypeDef],
         "autoScalingGroups": List[str],
+        "ec2TagSet": EC2TagSetOutputTypeDef,
+    },
+    total=False,
+)
+
+EC2TagSetUnionTypeDef = Union[EC2TagSetTypeDef, EC2TagSetOutputTypeDef]
+TargetInstancesTypeDef = TypedDict(
+    "TargetInstancesTypeDef",
+    {
+        "tagFilters": Sequence[EC2TagFilterTypeDef],
+        "autoScalingGroups": Sequence[str],
         "ec2TagSet": EC2TagSetTypeDef,
     },
     total=False,
 )
 
+OnPremisesTagSetUnionTypeDef = Union[OnPremisesTagSetTypeDef, OnPremisesTagSetOutputTypeDef]
 CloudFormationTargetTypeDef = TypedDict(
     "CloudFormationTargetTypeDef",
     {
         "deploymentId": str,
         "targetId": str,
         "lastUpdatedAt": datetime,
         "lifecycleEvents": List[LifecycleEventTypeDef],
@@ -1528,24 +1577,24 @@
 
 GetApplicationRevisionOutputTypeDef = TypedDict(
     "GetApplicationRevisionOutputTypeDef",
     {
         "applicationName": str,
         "revision": RevisionLocationTypeDef,
         "revisionInfo": GenericRevisionInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationRevisionsOutputTypeDef = TypedDict(
     "ListApplicationRevisionsOutputTypeDef",
     {
         "revisions": List[RevisionLocationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterApplicationRevisionInputRequestTypeDef = TypedDict(
     "_RequiredRegisterApplicationRevisionInputRequestTypeDef",
     {
         "applicationName": str,
@@ -1556,37 +1605,45 @@
     "_OptionalRegisterApplicationRevisionInputRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class RegisterApplicationRevisionInputRequestTypeDef(
     _RequiredRegisterApplicationRevisionInputRequestTypeDef,
     _OptionalRegisterApplicationRevisionInputRequestTypeDef,
 ):
     pass
 
-
 RevisionInfoTypeDef = TypedDict(
     "RevisionInfoTypeDef",
     {
         "revisionLocation": RevisionLocationTypeDef,
         "genericRevisionInfo": GenericRevisionInfoTypeDef,
     },
     total=False,
 )
 
-LoadBalancerInfoTypeDef = TypedDict(
-    "LoadBalancerInfoTypeDef",
+LoadBalancerInfoOutputTypeDef = TypedDict(
+    "LoadBalancerInfoOutputTypeDef",
     {
         "elbInfoList": List[ELBInfoTypeDef],
         "targetGroupInfoList": List[TargetGroupInfoTypeDef],
-        "targetGroupPairInfoList": List[TargetGroupPairInfoTypeDef],
+        "targetGroupPairInfoList": List[TargetGroupPairInfoOutputTypeDef],
+    },
+    total=False,
+)
+
+LoadBalancerInfoTypeDef = TypedDict(
+    "LoadBalancerInfoTypeDef",
+    {
+        "elbInfoList": Sequence[ELBInfoTypeDef],
+        "targetGroupInfoList": Sequence[TargetGroupInfoTypeDef],
+        "targetGroupPairInfoList": Sequence[TargetGroupPairInfoTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateDeploymentConfigInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentConfigInputRequestTypeDef",
     {
@@ -1599,35 +1656,59 @@
         "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
         "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
         "computePlatform": ComputePlatformType,
     },
     total=False,
 )
 
-
 class CreateDeploymentConfigInputRequestTypeDef(
     _RequiredCreateDeploymentConfigInputRequestTypeDef,
     _OptionalCreateDeploymentConfigInputRequestTypeDef,
 ):
     pass
 
-
 DeploymentConfigInfoTypeDef = TypedDict(
     "DeploymentConfigInfoTypeDef",
     {
         "deploymentConfigId": str,
         "deploymentConfigName": str,
         "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
         "createTime": datetime,
         "computePlatform": ComputePlatformType,
         "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
     },
     total=False,
 )
 
+ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "externalId": str,
+        "includeOnlyStatuses": Sequence[DeploymentStatusType],
+        "createTimeRange": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDeploymentsInputRequestTypeDef = TypedDict(
+    "ListDeploymentsInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "externalId": str,
+        "includeOnlyStatuses": Sequence[DeploymentStatusType],
+        "createTimeRange": TimeRangeTypeDef,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 _RequiredCreateDeploymentInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalCreateDeploymentInputRequestTypeDef = TypedDict(
@@ -1643,35 +1724,34 @@
         "updateOutdatedInstancesOnly": bool,
         "fileExistsBehavior": FileExistsBehaviorType,
         "overrideAlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateDeploymentInputRequestTypeDef(
     _RequiredCreateDeploymentInputRequestTypeDef, _OptionalCreateDeploymentInputRequestTypeDef
 ):
     pass
 
-
+TargetInstancesUnionTypeDef = Union[TargetInstancesTypeDef, TargetInstancesOutputTypeDef]
 BatchGetDeploymentInstancesOutputTypeDef = TypedDict(
     "BatchGetDeploymentInstancesOutputTypeDef",
     {
         "instancesSummary": List[InstanceSummaryTypeDef],
         "errorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentInstanceOutputTypeDef = TypedDict(
     "GetDeploymentInstanceOutputTypeDef",
     {
         "instanceSummary": InstanceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentTargetTypeDef = TypedDict(
     "DeploymentTargetTypeDef",
     {
         "deploymentTargetType": DeploymentTargetTypeType,
@@ -1685,79 +1765,41 @@
 
 BatchGetApplicationRevisionsOutputTypeDef = TypedDict(
     "BatchGetApplicationRevisionsOutputTypeDef",
     {
         "applicationName": str,
         "errorMessage": str,
         "revisions": List[RevisionInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentGroupInputRequestTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroupName": str,
-        "serviceRoleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentGroupInputRequestTypeDef",
-    {
-        "deploymentConfigName": str,
-        "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
-        "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
-        "autoScalingGroups": Sequence[str],
-        "triggerConfigurations": Sequence[TriggerConfigTypeDef],
-        "alarmConfiguration": AlarmConfigurationTypeDef,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
-        "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
-        "deploymentStyle": DeploymentStyleTypeDef,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
-        "ec2TagSet": EC2TagSetTypeDef,
-        "ecsServices": Sequence[ECSServiceTypeDef],
-        "onPremisesTagSet": OnPremisesTagSetTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateDeploymentGroupInputRequestTypeDef(
-    _RequiredCreateDeploymentGroupInputRequestTypeDef,
-    _OptionalCreateDeploymentGroupInputRequestTypeDef,
-):
-    pass
-
 
 DeploymentGroupInfoTypeDef = TypedDict(
     "DeploymentGroupInfoTypeDef",
     {
         "applicationName": str,
         "deploymentGroupId": str,
         "deploymentGroupName": str,
         "deploymentConfigName": str,
         "ec2TagFilters": List[EC2TagFilterTypeDef],
         "onPremisesInstanceTagFilters": List[TagFilterTypeDef],
         "autoScalingGroups": List[AutoScalingGroupTypeDef],
         "serviceRoleArn": str,
         "targetRevision": RevisionLocationTypeDef,
-        "triggerConfigurations": List[TriggerConfigTypeDef],
-        "alarmConfiguration": AlarmConfigurationTypeDef,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
+        "triggerConfigurations": List[TriggerConfigOutputTypeDef],
+        "alarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
         "deploymentStyle": DeploymentStyleTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
         "lastSuccessfulDeployment": LastDeploymentInfoTypeDef,
         "lastAttemptedDeployment": LastDeploymentInfoTypeDef,
-        "ec2TagSet": EC2TagSetTypeDef,
-        "onPremisesTagSet": OnPremisesTagSetTypeDef,
+        "ec2TagSet": EC2TagSetOutputTypeDef,
+        "onPremisesTagSet": OnPremisesTagSetOutputTypeDef,
         "computePlatform": ComputePlatformType,
         "ecsServices": List[ECSServiceTypeDef],
     },
     total=False,
 )
 
 DeploymentInfoTypeDef = TypedDict(
@@ -1774,33 +1816,70 @@
         "createTime": datetime,
         "startTime": datetime,
         "completeTime": datetime,
         "deploymentOverview": DeploymentOverviewTypeDef,
         "description": str,
         "creator": DeploymentCreatorType,
         "ignoreApplicationStopFailures": bool,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
         "updateOutdatedInstancesOnly": bool,
         "rollbackInfo": RollbackInfoTypeDef,
         "deploymentStyle": DeploymentStyleTypeDef,
-        "targetInstances": TargetInstancesTypeDef,
+        "targetInstances": TargetInstancesOutputTypeDef,
         "instanceTerminationWaitTimeStarted": bool,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
         "additionalDeploymentStatusInfo": str,
         "fileExistsBehavior": FileExistsBehaviorType,
         "deploymentStatusMessages": List[str],
         "computePlatform": ComputePlatformType,
         "externalId": str,
         "relatedDeployments": RelatedDeploymentsTypeDef,
-        "overrideAlarmConfiguration": AlarmConfigurationTypeDef,
+        "overrideAlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentGroupInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "serviceRoleArn": str,
+    },
+)
+_OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentGroupInputRequestTypeDef",
+    {
+        "deploymentConfigName": str,
+        "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
+        "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
+        "autoScalingGroups": Sequence[str],
+        "triggerConfigurations": Sequence[TriggerConfigUnionTypeDef],
+        "alarmConfiguration": AlarmConfigurationTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
+        "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
+        "deploymentStyle": DeploymentStyleTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "ec2TagSet": EC2TagSetTypeDef,
+        "ecsServices": Sequence[ECSServiceTypeDef],
+        "onPremisesTagSet": OnPremisesTagSetTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateDeploymentGroupInputRequestTypeDef(
+    _RequiredCreateDeploymentGroupInputRequestTypeDef,
+    _OptionalCreateDeploymentGroupInputRequestTypeDef,
+):
+    pass
+
+LoadBalancerInfoUnionTypeDef = Union[LoadBalancerInfoTypeDef, LoadBalancerInfoOutputTypeDef]
 _RequiredUpdateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentGroupInputRequestTypeDef",
     {
         "applicationName": str,
         "currentDeploymentGroupName": str,
     },
 )
@@ -1809,85 +1888,83 @@
     {
         "newDeploymentGroupName": str,
         "deploymentConfigName": str,
         "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
         "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
         "autoScalingGroups": Sequence[str],
         "serviceRoleArn": str,
-        "triggerConfigurations": Sequence[TriggerConfigTypeDef],
+        "triggerConfigurations": Sequence[TriggerConfigUnionTypeDef],
         "alarmConfiguration": AlarmConfigurationTypeDef,
         "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
         "deploymentStyle": DeploymentStyleTypeDef,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
         "loadBalancerInfo": LoadBalancerInfoTypeDef,
         "ec2TagSet": EC2TagSetTypeDef,
         "ecsServices": Sequence[ECSServiceTypeDef],
         "onPremisesTagSet": OnPremisesTagSetTypeDef,
     },
     total=False,
 )
 
-
 class UpdateDeploymentGroupInputRequestTypeDef(
     _RequiredUpdateDeploymentGroupInputRequestTypeDef,
     _OptionalUpdateDeploymentGroupInputRequestTypeDef,
 ):
     pass
 
-
 GetDeploymentConfigOutputTypeDef = TypedDict(
     "GetDeploymentConfigOutputTypeDef",
     {
         "deploymentConfigInfo": DeploymentConfigInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDeploymentTargetsOutputTypeDef = TypedDict(
     "BatchGetDeploymentTargetsOutputTypeDef",
     {
         "deploymentTargets": List[DeploymentTargetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentTargetOutputTypeDef = TypedDict(
     "GetDeploymentTargetOutputTypeDef",
     {
         "deploymentTarget": DeploymentTargetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDeploymentGroupsOutputTypeDef = TypedDict(
     "BatchGetDeploymentGroupsOutputTypeDef",
     {
         "deploymentGroupsInfo": List[DeploymentGroupInfoTypeDef],
         "errorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentGroupOutputTypeDef = TypedDict(
     "GetDeploymentGroupOutputTypeDef",
     {
         "deploymentGroupInfo": DeploymentGroupInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDeploymentsOutputTypeDef = TypedDict(
     "BatchGetDeploymentsOutputTypeDef",
     {
         "deploymentsInfo": List[DeploymentInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentOutputTypeDef = TypedDict(
     "GetDeploymentOutputTypeDef",
     {
         "deploymentInfo": DeploymentInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/type_defs.pyi` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codedeploy.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -52,156 +52,174 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
     "AlarmTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
+    "AutoRollbackConfigurationOutputTypeDef",
     "AutoRollbackConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetApplicationsInputRequestTypeDef",
     "BatchGetDeploymentGroupsInputRequestTypeDef",
     "BatchGetDeploymentInstancesInputRequestTypeDef",
     "BatchGetDeploymentTargetsInputRequestTypeDef",
     "BatchGetDeploymentsInputRequestTypeDef",
     "BatchGetOnPremisesInstancesInputRequestTypeDef",
     "BlueInstanceTerminationOptionTypeDef",
     "DeploymentReadyOptionTypeDef",
     "GreenFleetProvisioningOptionTypeDef",
     "ContinueDeploymentInputRequestTypeDef",
-    "CreateApplicationOutputTypeDef",
     "MinimumHealthyHostsTypeDef",
-    "CreateDeploymentConfigOutputTypeDef",
     "DeploymentStyleTypeDef",
     "EC2TagFilterTypeDef",
     "ECSServiceTypeDef",
     "TagFilterTypeDef",
-    "TriggerConfigTypeDef",
-    "CreateDeploymentGroupOutputTypeDef",
-    "CreateDeploymentOutputTypeDef",
     "DeleteApplicationInputRequestTypeDef",
     "DeleteDeploymentConfigInputRequestTypeDef",
     "DeleteDeploymentGroupInputRequestTypeDef",
     "DeleteGitHubAccountTokenInputRequestTypeDef",
-    "DeleteGitHubAccountTokenOutputTypeDef",
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     "LastDeploymentInfoTypeDef",
+    "TriggerConfigOutputTypeDef",
     "DeploymentOverviewTypeDef",
     "ErrorInformationTypeDef",
     "RelatedDeploymentsTypeDef",
     "RollbackInfoTypeDef",
     "DeregisterOnPremisesInstanceInputRequestTypeDef",
     "DiagnosticsTypeDef",
     "TargetGroupInfoTypeDef",
     "ELBInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GenericRevisionInfoTypeDef",
     "GetApplicationInputRequestTypeDef",
     "GetDeploymentConfigInputRequestTypeDef",
     "GetDeploymentGroupInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetDeploymentInputRequestTypeDef",
     "GetDeploymentInstanceInputRequestTypeDef",
     "GetDeploymentTargetInputRequestTypeDef",
     "GetOnPremisesInstanceInputRequestTypeDef",
     "GitHubLocationTypeDef",
     "LambdaFunctionInfoTypeDef",
-    "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationRevisionsInputRequestTypeDef",
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListApplicationsInputRequestTypeDef",
-    "ListApplicationsOutputTypeDef",
-    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
     "ListDeploymentConfigsInputRequestTypeDef",
-    "ListDeploymentConfigsOutputTypeDef",
-    "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     "ListDeploymentGroupsInputRequestTypeDef",
-    "ListDeploymentGroupsOutputTypeDef",
-    "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
     "ListDeploymentInstancesInputRequestTypeDef",
-    "ListDeploymentInstancesOutputTypeDef",
-    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
     "ListDeploymentTargetsInputRequestTypeDef",
-    "ListDeploymentTargetsOutputTypeDef",
-    "TimeRangeTypeDef",
-    "ListDeploymentsOutputTypeDef",
-    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
-    "ListGitHubAccountTokenNamesOutputTypeDef",
-    "ListOnPremisesInstancesOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
-    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
     "RawStringTypeDef",
     "RegisterOnPremisesInstanceInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "S3LocationTypeDef",
     "SkipWaitTimeForInstanceTerminationInputRequestTypeDef",
     "StopDeploymentInputRequestTypeDef",
-    "StopDeploymentOutputTypeDef",
+    "TrafficRouteOutputTypeDef",
     "TrafficRouteTypeDef",
     "TimeBasedCanaryTypeDef",
     "TimeBasedLinearTypeDef",
+    "TimestampTypeDef",
+    "TriggerConfigTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApplicationInputRequestTypeDef",
     "AddTagsToOnPremisesInstancesInputRequestTypeDef",
     "CreateApplicationInputRequestTypeDef",
     "InstanceInfoTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
+    "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
+    "AutoRollbackConfigurationUnionTypeDef",
     "BatchGetApplicationsOutputTypeDef",
-    "GetApplicationOutputTypeDef",
+    "CreateApplicationOutputTypeDef",
+    "CreateDeploymentConfigOutputTypeDef",
+    "CreateDeploymentGroupOutputTypeDef",
+    "CreateDeploymentOutputTypeDef",
     "DeleteDeploymentGroupOutputTypeDef",
+    "DeleteGitHubAccountTokenOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetApplicationOutputTypeDef",
+    "ListApplicationsOutputTypeDef",
+    "ListDeploymentConfigsOutputTypeDef",
+    "ListDeploymentGroupsOutputTypeDef",
+    "ListDeploymentInstancesOutputTypeDef",
+    "ListDeploymentTargetsOutputTypeDef",
+    "ListDeploymentsOutputTypeDef",
+    "ListGitHubAccountTokenNamesOutputTypeDef",
+    "ListOnPremisesInstancesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
+    "StopDeploymentOutputTypeDef",
     "UpdateDeploymentGroupOutputTypeDef",
     "BlueGreenDeploymentConfigurationTypeDef",
+    "EC2TagSetOutputTypeDef",
     "EC2TagSetTypeDef",
-    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "ListOnPremisesInstancesInputRequestTypeDef",
+    "OnPremisesTagSetOutputTypeDef",
     "OnPremisesTagSetTypeDef",
     "LifecycleEventTypeDef",
     "ECSTaskSetTypeDef",
     "GetDeploymentInputDeploymentSuccessfulWaitTypeDef",
-    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
-    "ListDeploymentsInputRequestTypeDef",
+    "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
+    "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
+    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
+    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "RevisionLocationTypeDef",
+    "TargetGroupPairInfoOutputTypeDef",
     "TargetGroupPairInfoTypeDef",
     "TrafficRoutingConfigTypeDef",
+    "TimeRangeTypeDef",
+    "TriggerConfigUnionTypeDef",
     "BatchGetOnPremisesInstancesOutputTypeDef",
     "GetOnPremisesInstanceOutputTypeDef",
+    "AlarmConfigurationUnionTypeDef",
+    "TargetInstancesOutputTypeDef",
+    "EC2TagSetUnionTypeDef",
     "TargetInstancesTypeDef",
+    "OnPremisesTagSetUnionTypeDef",
     "CloudFormationTargetTypeDef",
     "InstanceSummaryTypeDef",
     "InstanceTargetTypeDef",
     "LambdaTargetTypeDef",
     "ECSTargetTypeDef",
     "BatchGetApplicationRevisionsInputRequestTypeDef",
     "GetApplicationRevisionInputRequestTypeDef",
     "GetApplicationRevisionOutputTypeDef",
     "ListApplicationRevisionsOutputTypeDef",
     "RegisterApplicationRevisionInputRequestTypeDef",
     "RevisionInfoTypeDef",
+    "LoadBalancerInfoOutputTypeDef",
     "LoadBalancerInfoTypeDef",
     "CreateDeploymentConfigInputRequestTypeDef",
     "DeploymentConfigInfoTypeDef",
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    "ListDeploymentsInputRequestTypeDef",
     "CreateDeploymentInputRequestTypeDef",
+    "TargetInstancesUnionTypeDef",
     "BatchGetDeploymentInstancesOutputTypeDef",
     "GetDeploymentInstanceOutputTypeDef",
     "DeploymentTargetTypeDef",
     "BatchGetApplicationRevisionsOutputTypeDef",
-    "CreateDeploymentGroupInputRequestTypeDef",
     "DeploymentGroupInfoTypeDef",
     "DeploymentInfoTypeDef",
+    "CreateDeploymentGroupInputRequestTypeDef",
+    "LoadBalancerInfoUnionTypeDef",
     "UpdateDeploymentGroupInputRequestTypeDef",
     "GetDeploymentConfigOutputTypeDef",
     "BatchGetDeploymentTargetsOutputTypeDef",
     "GetDeploymentTargetOutputTypeDef",
     "BatchGetDeploymentGroupsOutputTypeDef",
     "GetDeploymentGroupOutputTypeDef",
     "BatchGetDeploymentsOutputTypeDef",
@@ -243,32 +261,52 @@
         "linkedToGitHub": bool,
         "gitHubAccountName": str,
         "computePlatform": ComputePlatformType,
     },
     total=False,
 )
 
+AutoRollbackConfigurationOutputTypeDef = TypedDict(
+    "AutoRollbackConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "events": List[AutoRollbackEventType],
+    },
+    total=False,
+)
+
 AutoRollbackConfigurationTypeDef = TypedDict(
     "AutoRollbackConfigurationTypeDef",
     {
         "enabled": bool,
-        "events": List[AutoRollbackEventType],
+        "events": Sequence[AutoRollbackEventType],
     },
     total=False,
 )
 
 AutoScalingGroupTypeDef = TypedDict(
     "AutoScalingGroupTypeDef",
     {
         "name": str,
         "hook": str,
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
 BatchGetApplicationsInputRequestTypeDef = TypedDict(
     "BatchGetApplicationsInputRequestTypeDef",
     {
         "applicationNames": Sequence[str],
     },
 )
 
@@ -342,39 +380,23 @@
     {
         "deploymentId": str,
         "deploymentWaitType": DeploymentWaitTypeType,
     },
     total=False,
 )
 
-CreateApplicationOutputTypeDef = TypedDict(
-    "CreateApplicationOutputTypeDef",
-    {
-        "applicationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MinimumHealthyHostsTypeDef = TypedDict(
     "MinimumHealthyHostsTypeDef",
     {
         "type": MinimumHealthyHostsTypeType,
         "value": int,
     },
     total=False,
 )
 
-CreateDeploymentConfigOutputTypeDef = TypedDict(
-    "CreateDeploymentConfigOutputTypeDef",
-    {
-        "deploymentConfigId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentStyleTypeDef = TypedDict(
     "DeploymentStyleTypeDef",
     {
         "deploymentType": DeploymentTypeType,
         "deploymentOption": DeploymentOptionType,
     },
     total=False,
@@ -405,40 +427,14 @@
         "Key": str,
         "Value": str,
         "Type": TagFilterTypeType,
     },
     total=False,
 )
 
-TriggerConfigTypeDef = TypedDict(
-    "TriggerConfigTypeDef",
-    {
-        "triggerName": str,
-        "triggerTargetArn": str,
-        "triggerEvents": List[TriggerEventTypeType],
-    },
-    total=False,
-)
-
-CreateDeploymentGroupOutputTypeDef = TypedDict(
-    "CreateDeploymentGroupOutputTypeDef",
-    {
-        "deploymentGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDeploymentOutputTypeDef = TypedDict(
-    "CreateDeploymentOutputTypeDef",
-    {
-        "deploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteApplicationInputRequestTypeDef = TypedDict(
     "DeleteApplicationInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 
@@ -461,22 +457,14 @@
     "DeleteGitHubAccountTokenInputRequestTypeDef",
     {
         "tokenName": str,
     },
     total=False,
 )
 
-DeleteGitHubAccountTokenOutputTypeDef = TypedDict(
-    "DeleteGitHubAccountTokenOutputTypeDef",
-    {
-        "tokenName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteResourcesByExternalIdInputRequestTypeDef = TypedDict(
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     {
         "externalId": str,
     },
     total=False,
 )
@@ -488,14 +476,24 @@
         "status": DeploymentStatusType,
         "endTime": datetime,
         "createTime": datetime,
     },
     total=False,
 )
 
+TriggerConfigOutputTypeDef = TypedDict(
+    "TriggerConfigOutputTypeDef",
+    {
+        "triggerName": str,
+        "triggerTargetArn": str,
+        "triggerEvents": List[TriggerEventTypeType],
+    },
+    total=False,
+)
+
 DeploymentOverviewTypeDef = TypedDict(
     "DeploymentOverviewTypeDef",
     {
         "Pending": int,
         "InProgress": int,
         "Succeeded": int,
         "Failed": int,
@@ -563,21 +561,14 @@
     "ELBInfoTypeDef",
     {
         "name": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GenericRevisionInfoTypeDef = TypedDict(
     "GenericRevisionInfoTypeDef",
     {
         "description": str,
         "deploymentGroups": List[str],
         "firstUsedTime": datetime,
         "lastUsedTime": datetime,
@@ -665,39 +656,24 @@
         "currentVersion": str,
         "targetVersion": str,
         "targetVersionWeight": float,
     },
     total=False,
 )
 
-_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
-    {
-        "applicationName": str,
-    },
-)
-_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "sortBy": ApplicationRevisionSortByType,
-        "sortOrder": SortOrderType,
-        "s3Bucket": str,
-        "s3KeyPrefix": str,
-        "deployed": ListStateFilterActionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
-    _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-    _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListApplicationRevisionsInputRequestTypeDef = TypedDict(
     "_RequiredListApplicationRevisionsInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListApplicationRevisionsInputRequestTypeDef = TypedDict(
@@ -709,141 +685,59 @@
         "s3KeyPrefix": str,
         "deployed": ListStateFilterActionType,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListApplicationRevisionsInputRequestTypeDef(
     _RequiredListApplicationRevisionsInputRequestTypeDef,
     _OptionalListApplicationRevisionsInputRequestTypeDef,
 ):
     pass
 
-ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsInputListApplicationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListApplicationsInputRequestTypeDef = TypedDict(
     "ListApplicationsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListApplicationsOutputTypeDef = TypedDict(
-    "ListApplicationsOutputTypeDef",
-    {
-        "applications": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = TypedDict(
-    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDeploymentConfigsInputRequestTypeDef = TypedDict(
     "ListDeploymentConfigsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListDeploymentConfigsOutputTypeDef = TypedDict(
-    "ListDeploymentConfigsOutputTypeDef",
-    {
-        "deploymentConfigsList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    {
-        "applicationName": str,
-    },
-)
-_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
-    _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-    _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDeploymentGroupsInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentGroupsInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalListDeploymentGroupsInputRequestTypeDef = TypedDict(
     "_OptionalListDeploymentGroupsInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListDeploymentGroupsInputRequestTypeDef(
     _RequiredListDeploymentGroupsInputRequestTypeDef,
     _OptionalListDeploymentGroupsInputRequestTypeDef,
 ):
     pass
 
-ListDeploymentGroupsOutputTypeDef = TypedDict(
-    "ListDeploymentGroupsOutputTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroups": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    {
-        "deploymentId": str,
-    },
-)
-_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
-    {
-        "instanceStatusFilter": Sequence[InstanceStatusType],
-        "instanceTypeFilter": Sequence[InstanceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
-    _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-    _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
-):
-    pass
 
 _RequiredListDeploymentInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListDeploymentInstancesInputRequestTypeDef",
     {
         "deploymentId": str,
     },
 )
@@ -853,157 +747,71 @@
         "nextToken": str,
         "instanceStatusFilter": Sequence[InstanceStatusType],
         "instanceTypeFilter": Sequence[InstanceTypeType],
     },
     total=False,
 )
 
+
 class ListDeploymentInstancesInputRequestTypeDef(
     _RequiredListDeploymentInstancesInputRequestTypeDef,
     _OptionalListDeploymentInstancesInputRequestTypeDef,
 ):
     pass
 
-ListDeploymentInstancesOutputTypeDef = TypedDict(
-    "ListDeploymentInstancesOutputTypeDef",
-    {
-        "instancesList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
-    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
-    {
-        "deploymentId": str,
-        "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListDeploymentTargetsInputRequestTypeDef = TypedDict(
     "ListDeploymentTargetsInputRequestTypeDef",
     {
         "deploymentId": str,
         "nextToken": str,
         "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
     },
     total=False,
 )
 
-ListDeploymentTargetsOutputTypeDef = TypedDict(
-    "ListDeploymentTargetsOutputTypeDef",
-    {
-        "targetIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "start": Union[datetime, str],
-        "end": Union[datetime, str],
-    },
-    total=False,
-)
-
-ListDeploymentsOutputTypeDef = TypedDict(
-    "ListDeploymentsOutputTypeDef",
-    {
-        "deployments": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = TypedDict(
-    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGitHubAccountTokenNamesInputRequestTypeDef = TypedDict(
     "ListGitHubAccountTokenNamesInputRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
 
-ListGitHubAccountTokenNamesOutputTypeDef = TypedDict(
-    "ListGitHubAccountTokenNamesOutputTypeDef",
-    {
-        "tokenNameList": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListOnPremisesInstancesOutputTypeDef = TypedDict(
-    "ListOnPremisesInstancesOutputTypeDef",
-    {
-        "instanceNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
     "_OptionalListTagsForResourceInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
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
 
 PutLifecycleEventHookExecutionStatusInputRequestTypeDef = TypedDict(
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     {
         "deploymentId": str,
         "lifecycleEventHookExecutionId": str,
         "status": LifecycleEventStatusType,
     },
     total=False,
 )
 
-PutLifecycleEventHookExecutionStatusOutputTypeDef = TypedDict(
-    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
-    {
-        "lifecycleEventHookExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RawStringTypeDef = TypedDict(
     "RawStringTypeDef",
     {
         "content": str,
         "sha256": str,
     },
     total=False,
@@ -1020,30 +828,21 @@
     {
         "iamSessionArn": str,
         "iamUserArn": str,
     },
     total=False,
 )
 
+
 class RegisterOnPremisesInstanceInputRequestTypeDef(
     _RequiredRegisterOnPremisesInstanceInputRequestTypeDef,
     _OptionalRegisterOnPremisesInstanceInputRequestTypeDef,
 ):
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
 
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "bundleType": BundleTypeType,
@@ -1071,32 +870,33 @@
     "_OptionalStopDeploymentInputRequestTypeDef",
     {
         "autoRollbackEnabled": bool,
     },
     total=False,
 )
 
+
 class StopDeploymentInputRequestTypeDef(
     _RequiredStopDeploymentInputRequestTypeDef, _OptionalStopDeploymentInputRequestTypeDef
 ):
     pass
 
-StopDeploymentOutputTypeDef = TypedDict(
-    "StopDeploymentOutputTypeDef",
+
+TrafficRouteOutputTypeDef = TypedDict(
+    "TrafficRouteOutputTypeDef",
     {
-        "status": StopStatusType,
-        "statusMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "listenerArns": List[str],
     },
+    total=False,
 )
 
 TrafficRouteTypeDef = TypedDict(
     "TrafficRouteTypeDef",
     {
-        "listenerArns": List[str],
+        "listenerArns": Sequence[str],
     },
     total=False,
 )
 
 TimeBasedCanaryTypeDef = TypedDict(
     "TimeBasedCanaryTypeDef",
     {
@@ -1111,14 +911,25 @@
     {
         "linearPercentage": int,
         "linearInterval": int,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
+TriggerConfigTypeDef = TypedDict(
+    "TriggerConfigTypeDef",
+    {
+        "triggerName": str,
+        "triggerTargetArn": str,
+        "triggerEvents": Sequence[TriggerEventTypeType],
+    },
+    total=False,
+)
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1151,42 +962,35 @@
     {
         "computePlatform": ComputePlatformType,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateApplicationInputRequestTypeDef(
     _RequiredCreateApplicationInputRequestTypeDef, _OptionalCreateApplicationInputRequestTypeDef
 ):
     pass
 
+
 InstanceInfoTypeDef = TypedDict(
     "InstanceInfoTypeDef",
     {
         "instanceName": str,
         "iamSessionArn": str,
         "iamUserArn": str,
         "instanceArn": str,
         "registerTime": datetime,
         "deregisterTime": datetime,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsFromOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
         "instanceNames": Sequence[str],
     },
 )
@@ -1195,98 +999,263 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+AlarmConfigurationOutputTypeDef = TypedDict(
+    "AlarmConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+        "ignorePollAlarmFailure": bool,
+        "alarms": List[AlarmTypeDef],
+    },
+    total=False,
+)
+
 AlarmConfigurationTypeDef = TypedDict(
     "AlarmConfigurationTypeDef",
     {
         "enabled": bool,
         "ignorePollAlarmFailure": bool,
-        "alarms": List[AlarmTypeDef],
+        "alarms": Sequence[AlarmTypeDef],
     },
     total=False,
 )
 
+AutoRollbackConfigurationUnionTypeDef = Union[
+    AutoRollbackConfigurationTypeDef, AutoRollbackConfigurationOutputTypeDef
+]
 BatchGetApplicationsOutputTypeDef = TypedDict(
     "BatchGetApplicationsOutputTypeDef",
     {
         "applicationsInfo": List[ApplicationInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetApplicationOutputTypeDef = TypedDict(
-    "GetApplicationOutputTypeDef",
+CreateApplicationOutputTypeDef = TypedDict(
+    "CreateApplicationOutputTypeDef",
     {
-        "application": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "applicationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentConfigOutputTypeDef = TypedDict(
+    "CreateDeploymentConfigOutputTypeDef",
+    {
+        "deploymentConfigId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentGroupOutputTypeDef = TypedDict(
+    "CreateDeploymentGroupOutputTypeDef",
+    {
+        "deploymentGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentOutputTypeDef = TypedDict(
+    "CreateDeploymentOutputTypeDef",
+    {
+        "deploymentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDeploymentGroupOutputTypeDef = TypedDict(
     "DeleteDeploymentGroupOutputTypeDef",
     {
         "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteGitHubAccountTokenOutputTypeDef = TypedDict(
+    "DeleteGitHubAccountTokenOutputTypeDef",
+    {
+        "tokenName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApplicationOutputTypeDef = TypedDict(
+    "GetApplicationOutputTypeDef",
+    {
+        "application": ApplicationInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsOutputTypeDef = TypedDict(
+    "ListApplicationsOutputTypeDef",
+    {
+        "applications": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentConfigsOutputTypeDef = TypedDict(
+    "ListDeploymentConfigsOutputTypeDef",
+    {
+        "deploymentConfigsList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentGroupsOutputTypeDef = TypedDict(
+    "ListDeploymentGroupsOutputTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroups": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentInstancesOutputTypeDef = TypedDict(
+    "ListDeploymentInstancesOutputTypeDef",
+    {
+        "instancesList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentTargetsOutputTypeDef = TypedDict(
+    "ListDeploymentTargetsOutputTypeDef",
+    {
+        "targetIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDeploymentsOutputTypeDef = TypedDict(
+    "ListDeploymentsOutputTypeDef",
+    {
+        "deployments": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListGitHubAccountTokenNamesOutputTypeDef = TypedDict(
+    "ListGitHubAccountTokenNamesOutputTypeDef",
+    {
+        "tokenNameList": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOnPremisesInstancesOutputTypeDef = TypedDict(
+    "ListOnPremisesInstancesOutputTypeDef",
+    {
+        "instanceNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutLifecycleEventHookExecutionStatusOutputTypeDef = TypedDict(
+    "PutLifecycleEventHookExecutionStatusOutputTypeDef",
+    {
+        "lifecycleEventHookExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDeploymentOutputTypeDef = TypedDict(
+    "StopDeploymentOutputTypeDef",
+    {
+        "status": StopStatusType,
+        "statusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDeploymentGroupOutputTypeDef = TypedDict(
     "UpdateDeploymentGroupOutputTypeDef",
     {
         "hooksNotCleanedUp": List[AutoScalingGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BlueGreenDeploymentConfigurationTypeDef = TypedDict(
     "BlueGreenDeploymentConfigurationTypeDef",
     {
         "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionTypeDef,
         "deploymentReadyOption": DeploymentReadyOptionTypeDef,
         "greenFleetProvisioningOption": GreenFleetProvisioningOptionTypeDef,
     },
     total=False,
 )
 
-EC2TagSetTypeDef = TypedDict(
-    "EC2TagSetTypeDef",
+EC2TagSetOutputTypeDef = TypedDict(
+    "EC2TagSetOutputTypeDef",
     {
         "ec2TagSetList": List[List[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
-ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
-    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
+EC2TagSetTypeDef = TypedDict(
+    "EC2TagSetTypeDef",
     {
-        "registrationStatus": RegistrationStatusType,
-        "tagFilters": Sequence[TagFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ec2TagSetList": Sequence[Sequence[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
 ListOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "ListOnPremisesInstancesInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
         "tagFilters": Sequence[TagFilterTypeDef],
         "nextToken": str,
     },
     total=False,
 )
 
+OnPremisesTagSetOutputTypeDef = TypedDict(
+    "OnPremisesTagSetOutputTypeDef",
+    {
+        "onPremisesTagSetList": List[List[TagFilterTypeDef]],
+    },
+    total=False,
+)
+
 OnPremisesTagSetTypeDef = TypedDict(
     "OnPremisesTagSetTypeDef",
     {
-        "onPremisesTagSetList": List[List[TagFilterTypeDef]],
+        "onPremisesTagSetList": Sequence[Sequence[TagFilterTypeDef]],
     },
     total=False,
 )
 
 LifecycleEventTypeDef = TypedDict(
     "LifecycleEventTypeDef",
     {
@@ -1324,42 +1293,135 @@
     "_OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetDeploymentInputDeploymentSuccessfulWaitTypeDef(
     _RequiredGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
     _OptionalGetDeploymentInputDeploymentSuccessfulWaitTypeDef,
 ):
     pass
 
-ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
-    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+
+_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     {
         "applicationName": str,
-        "deploymentGroupName": str,
-        "externalId": str,
-        "includeOnlyStatuses": Sequence[DeploymentStatusType],
-        "createTimeRange": TimeRangeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+)
+_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
+    {
+        "sortBy": ApplicationRevisionSortByType,
+        "sortOrder": SortOrderType,
+        "s3Bucket": str,
+        "s3KeyPrefix": str,
+        "deployed": ListStateFilterActionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListDeploymentsInputRequestTypeDef = TypedDict(
-    "ListDeploymentsInputRequestTypeDef",
+
+class ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef(
+    _RequiredListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    _OptionalListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+):
+    pass
+
+
+ListApplicationsInputListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsInputListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef = TypedDict(
+    "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     {
         "applicationName": str,
-        "deploymentGroupName": str,
-        "externalId": str,
-        "includeOnlyStatuses": Sequence[DeploymentStatusType],
-        "createTimeRange": TimeRangeTypeDef,
-        "nextToken": str,
+    },
+)
+_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef(
+    _RequiredListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+    _OptionalListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    {
+        "deploymentId": str,
+    },
+)
+_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
+    {
+        "instanceStatusFilter": Sequence[InstanceStatusType],
+        "instanceTypeFilter": Sequence[InstanceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef(
+    _RequiredListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+    _OptionalListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+):
+    pass
+
+
+ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef = TypedDict(
+    "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
+    {
+        "deploymentId": str,
+        "targetFilters": Mapping[TargetFilterNameType, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef = TypedDict(
+    "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef = TypedDict(
+    "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
+    {
+        "registrationStatus": RegistrationStatusType,
+        "tagFilters": Sequence[TagFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 RevisionLocationTypeDef = TypedDict(
     "RevisionLocationTypeDef",
     {
@@ -1368,18 +1430,28 @@
         "gitHubLocation": GitHubLocationTypeDef,
         "string": RawStringTypeDef,
         "appSpecContent": AppSpecContentTypeDef,
     },
     total=False,
 )
 
+TargetGroupPairInfoOutputTypeDef = TypedDict(
+    "TargetGroupPairInfoOutputTypeDef",
+    {
+        "targetGroups": List[TargetGroupInfoTypeDef],
+        "prodTrafficRoute": TrafficRouteOutputTypeDef,
+        "testTrafficRoute": TrafficRouteOutputTypeDef,
+    },
+    total=False,
+)
+
 TargetGroupPairInfoTypeDef = TypedDict(
     "TargetGroupPairInfoTypeDef",
     {
-        "targetGroups": List[TargetGroupInfoTypeDef],
+        "targetGroups": Sequence[TargetGroupInfoTypeDef],
         "prodTrafficRoute": TrafficRouteTypeDef,
         "testTrafficRoute": TrafficRouteTypeDef,
     },
     total=False,
 )
 
 TrafficRoutingConfigTypeDef = TypedDict(
@@ -1388,40 +1460,63 @@
         "type": TrafficRoutingTypeType,
         "timeBasedCanary": TimeBasedCanaryTypeDef,
         "timeBasedLinear": TimeBasedLinearTypeDef,
     },
     total=False,
 )
 
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
+    {
+        "start": TimestampTypeDef,
+        "end": TimestampTypeDef,
+    },
+    total=False,
+)
+
+TriggerConfigUnionTypeDef = Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
 BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
     "BatchGetOnPremisesInstancesOutputTypeDef",
     {
         "instanceInfos": List[InstanceInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOnPremisesInstanceOutputTypeDef = TypedDict(
     "GetOnPremisesInstanceOutputTypeDef",
     {
         "instanceInfo": InstanceInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TargetInstancesTypeDef = TypedDict(
-    "TargetInstancesTypeDef",
+AlarmConfigurationUnionTypeDef = Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef]
+TargetInstancesOutputTypeDef = TypedDict(
+    "TargetInstancesOutputTypeDef",
     {
         "tagFilters": List[EC2TagFilterTypeDef],
         "autoScalingGroups": List[str],
+        "ec2TagSet": EC2TagSetOutputTypeDef,
+    },
+    total=False,
+)
+
+EC2TagSetUnionTypeDef = Union[EC2TagSetTypeDef, EC2TagSetOutputTypeDef]
+TargetInstancesTypeDef = TypedDict(
+    "TargetInstancesTypeDef",
+    {
+        "tagFilters": Sequence[EC2TagFilterTypeDef],
+        "autoScalingGroups": Sequence[str],
         "ec2TagSet": EC2TagSetTypeDef,
     },
     total=False,
 )
 
+OnPremisesTagSetUnionTypeDef = Union[OnPremisesTagSetTypeDef, OnPremisesTagSetOutputTypeDef]
 CloudFormationTargetTypeDef = TypedDict(
     "CloudFormationTargetTypeDef",
     {
         "deploymentId": str,
         "targetId": str,
         "lastUpdatedAt": datetime,
         "lifecycleEvents": List[LifecycleEventTypeDef],
@@ -1505,24 +1600,24 @@
 
 GetApplicationRevisionOutputTypeDef = TypedDict(
     "GetApplicationRevisionOutputTypeDef",
     {
         "applicationName": str,
         "revision": RevisionLocationTypeDef,
         "revisionInfo": GenericRevisionInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationRevisionsOutputTypeDef = TypedDict(
     "ListApplicationRevisionsOutputTypeDef",
     {
         "revisions": List[RevisionLocationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterApplicationRevisionInputRequestTypeDef = TypedDict(
     "_RequiredRegisterApplicationRevisionInputRequestTypeDef",
     {
         "applicationName": str,
@@ -1533,35 +1628,47 @@
     "_OptionalRegisterApplicationRevisionInputRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class RegisterApplicationRevisionInputRequestTypeDef(
     _RequiredRegisterApplicationRevisionInputRequestTypeDef,
     _OptionalRegisterApplicationRevisionInputRequestTypeDef,
 ):
     pass
 
+
 RevisionInfoTypeDef = TypedDict(
     "RevisionInfoTypeDef",
     {
         "revisionLocation": RevisionLocationTypeDef,
         "genericRevisionInfo": GenericRevisionInfoTypeDef,
     },
     total=False,
 )
 
-LoadBalancerInfoTypeDef = TypedDict(
-    "LoadBalancerInfoTypeDef",
+LoadBalancerInfoOutputTypeDef = TypedDict(
+    "LoadBalancerInfoOutputTypeDef",
     {
         "elbInfoList": List[ELBInfoTypeDef],
         "targetGroupInfoList": List[TargetGroupInfoTypeDef],
-        "targetGroupPairInfoList": List[TargetGroupPairInfoTypeDef],
+        "targetGroupPairInfoList": List[TargetGroupPairInfoOutputTypeDef],
+    },
+    total=False,
+)
+
+LoadBalancerInfoTypeDef = TypedDict(
+    "LoadBalancerInfoTypeDef",
+    {
+        "elbInfoList": Sequence[ELBInfoTypeDef],
+        "targetGroupInfoList": Sequence[TargetGroupInfoTypeDef],
+        "targetGroupPairInfoList": Sequence[TargetGroupPairInfoTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateDeploymentConfigInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentConfigInputRequestTypeDef",
     {
@@ -1574,33 +1681,61 @@
         "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
         "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
         "computePlatform": ComputePlatformType,
     },
     total=False,
 )
 
+
 class CreateDeploymentConfigInputRequestTypeDef(
     _RequiredCreateDeploymentConfigInputRequestTypeDef,
     _OptionalCreateDeploymentConfigInputRequestTypeDef,
 ):
     pass
 
+
 DeploymentConfigInfoTypeDef = TypedDict(
     "DeploymentConfigInfoTypeDef",
     {
         "deploymentConfigId": str,
         "deploymentConfigName": str,
         "minimumHealthyHosts": MinimumHealthyHostsTypeDef,
         "createTime": datetime,
         "computePlatform": ComputePlatformType,
         "trafficRoutingConfig": TrafficRoutingConfigTypeDef,
     },
     total=False,
 )
 
+ListDeploymentsInputListDeploymentsPaginateTypeDef = TypedDict(
+    "ListDeploymentsInputListDeploymentsPaginateTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "externalId": str,
+        "includeOnlyStatuses": Sequence[DeploymentStatusType],
+        "createTimeRange": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDeploymentsInputRequestTypeDef = TypedDict(
+    "ListDeploymentsInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "externalId": str,
+        "includeOnlyStatuses": Sequence[DeploymentStatusType],
+        "createTimeRange": TimeRangeTypeDef,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 _RequiredCreateDeploymentInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 _OptionalCreateDeploymentInputRequestTypeDef = TypedDict(
@@ -1616,33 +1751,36 @@
         "updateOutdatedInstancesOnly": bool,
         "fileExistsBehavior": FileExistsBehaviorType,
         "overrideAlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateDeploymentInputRequestTypeDef(
     _RequiredCreateDeploymentInputRequestTypeDef, _OptionalCreateDeploymentInputRequestTypeDef
 ):
     pass
 
+
+TargetInstancesUnionTypeDef = Union[TargetInstancesTypeDef, TargetInstancesOutputTypeDef]
 BatchGetDeploymentInstancesOutputTypeDef = TypedDict(
     "BatchGetDeploymentInstancesOutputTypeDef",
     {
         "instancesSummary": List[InstanceSummaryTypeDef],
         "errorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentInstanceOutputTypeDef = TypedDict(
     "GetDeploymentInstanceOutputTypeDef",
     {
         "instanceSummary": InstanceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploymentTargetTypeDef = TypedDict(
     "DeploymentTargetTypeDef",
     {
         "deploymentTargetType": DeploymentTargetTypeType,
@@ -1656,77 +1794,41 @@
 
 BatchGetApplicationRevisionsOutputTypeDef = TypedDict(
     "BatchGetApplicationRevisionsOutputTypeDef",
     {
         "applicationName": str,
         "errorMessage": str,
         "revisions": List[RevisionInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentGroupInputRequestTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroupName": str,
-        "serviceRoleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentGroupInputRequestTypeDef",
-    {
-        "deploymentConfigName": str,
-        "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
-        "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
-        "autoScalingGroups": Sequence[str],
-        "triggerConfigurations": Sequence[TriggerConfigTypeDef],
-        "alarmConfiguration": AlarmConfigurationTypeDef,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
-        "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
-        "deploymentStyle": DeploymentStyleTypeDef,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
-        "ec2TagSet": EC2TagSetTypeDef,
-        "ecsServices": Sequence[ECSServiceTypeDef],
-        "onPremisesTagSet": OnPremisesTagSetTypeDef,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateDeploymentGroupInputRequestTypeDef(
-    _RequiredCreateDeploymentGroupInputRequestTypeDef,
-    _OptionalCreateDeploymentGroupInputRequestTypeDef,
-):
-    pass
 
 DeploymentGroupInfoTypeDef = TypedDict(
     "DeploymentGroupInfoTypeDef",
     {
         "applicationName": str,
         "deploymentGroupId": str,
         "deploymentGroupName": str,
         "deploymentConfigName": str,
         "ec2TagFilters": List[EC2TagFilterTypeDef],
         "onPremisesInstanceTagFilters": List[TagFilterTypeDef],
         "autoScalingGroups": List[AutoScalingGroupTypeDef],
         "serviceRoleArn": str,
         "targetRevision": RevisionLocationTypeDef,
-        "triggerConfigurations": List[TriggerConfigTypeDef],
-        "alarmConfiguration": AlarmConfigurationTypeDef,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
+        "triggerConfigurations": List[TriggerConfigOutputTypeDef],
+        "alarmConfiguration": AlarmConfigurationOutputTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
         "deploymentStyle": DeploymentStyleTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
         "lastSuccessfulDeployment": LastDeploymentInfoTypeDef,
         "lastAttemptedDeployment": LastDeploymentInfoTypeDef,
-        "ec2TagSet": EC2TagSetTypeDef,
-        "onPremisesTagSet": OnPremisesTagSetTypeDef,
+        "ec2TagSet": EC2TagSetOutputTypeDef,
+        "onPremisesTagSet": OnPremisesTagSetOutputTypeDef,
         "computePlatform": ComputePlatformType,
         "ecsServices": List[ECSServiceTypeDef],
     },
     total=False,
 )
 
 DeploymentInfoTypeDef = TypedDict(
@@ -1743,33 +1845,72 @@
         "createTime": datetime,
         "startTime": datetime,
         "completeTime": datetime,
         "deploymentOverview": DeploymentOverviewTypeDef,
         "description": str,
         "creator": DeploymentCreatorType,
         "ignoreApplicationStopFailures": bool,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
         "updateOutdatedInstancesOnly": bool,
         "rollbackInfo": RollbackInfoTypeDef,
         "deploymentStyle": DeploymentStyleTypeDef,
-        "targetInstances": TargetInstancesTypeDef,
+        "targetInstances": TargetInstancesOutputTypeDef,
         "instanceTerminationWaitTimeStarted": bool,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
         "additionalDeploymentStatusInfo": str,
         "fileExistsBehavior": FileExistsBehaviorType,
         "deploymentStatusMessages": List[str],
         "computePlatform": ComputePlatformType,
         "externalId": str,
         "relatedDeployments": RelatedDeploymentsTypeDef,
-        "overrideAlarmConfiguration": AlarmConfigurationTypeDef,
+        "overrideAlarmConfiguration": AlarmConfigurationOutputTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentGroupInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "serviceRoleArn": str,
+    },
+)
+_OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentGroupInputRequestTypeDef",
+    {
+        "deploymentConfigName": str,
+        "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
+        "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
+        "autoScalingGroups": Sequence[str],
+        "triggerConfigurations": Sequence[TriggerConfigUnionTypeDef],
+        "alarmConfiguration": AlarmConfigurationTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
+        "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
+        "deploymentStyle": DeploymentStyleTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "ec2TagSet": EC2TagSetTypeDef,
+        "ecsServices": Sequence[ECSServiceTypeDef],
+        "onPremisesTagSet": OnPremisesTagSetTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateDeploymentGroupInputRequestTypeDef(
+    _RequiredCreateDeploymentGroupInputRequestTypeDef,
+    _OptionalCreateDeploymentGroupInputRequestTypeDef,
+):
+    pass
+
+
+LoadBalancerInfoUnionTypeDef = Union[LoadBalancerInfoTypeDef, LoadBalancerInfoOutputTypeDef]
 _RequiredUpdateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentGroupInputRequestTypeDef",
     {
         "applicationName": str,
         "currentDeploymentGroupName": str,
     },
 )
@@ -1778,83 +1919,85 @@
     {
         "newDeploymentGroupName": str,
         "deploymentConfigName": str,
         "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
         "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
         "autoScalingGroups": Sequence[str],
         "serviceRoleArn": str,
-        "triggerConfigurations": Sequence[TriggerConfigTypeDef],
+        "triggerConfigurations": Sequence[TriggerConfigUnionTypeDef],
         "alarmConfiguration": AlarmConfigurationTypeDef,
         "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
         "deploymentStyle": DeploymentStyleTypeDef,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
         "loadBalancerInfo": LoadBalancerInfoTypeDef,
         "ec2TagSet": EC2TagSetTypeDef,
         "ecsServices": Sequence[ECSServiceTypeDef],
         "onPremisesTagSet": OnPremisesTagSetTypeDef,
     },
     total=False,
 )
 
+
 class UpdateDeploymentGroupInputRequestTypeDef(
     _RequiredUpdateDeploymentGroupInputRequestTypeDef,
     _OptionalUpdateDeploymentGroupInputRequestTypeDef,
 ):
     pass
 
+
 GetDeploymentConfigOutputTypeDef = TypedDict(
     "GetDeploymentConfigOutputTypeDef",
     {
         "deploymentConfigInfo": DeploymentConfigInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDeploymentTargetsOutputTypeDef = TypedDict(
     "BatchGetDeploymentTargetsOutputTypeDef",
     {
         "deploymentTargets": List[DeploymentTargetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentTargetOutputTypeDef = TypedDict(
     "GetDeploymentTargetOutputTypeDef",
     {
         "deploymentTarget": DeploymentTargetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDeploymentGroupsOutputTypeDef = TypedDict(
     "BatchGetDeploymentGroupsOutputTypeDef",
     {
         "deploymentGroupsInfo": List[DeploymentGroupInfoTypeDef],
         "errorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentGroupOutputTypeDef = TypedDict(
     "GetDeploymentGroupOutputTypeDef",
     {
         "deploymentGroupInfo": DeploymentGroupInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetDeploymentsOutputTypeDef = TypedDict(
     "BatchGetDeploymentsOutputTypeDef",
     {
         "deploymentsInfo": List[DeploymentInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentOutputTypeDef = TypedDict(
     "GetDeploymentOutputTypeDef",
     {
         "deploymentInfo": DeploymentInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/waiter.py` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy/waiter.pyi` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/PKG-INFO` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codedeploy
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeDeploy 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeDeploy 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codedeploy type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codedeploy type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codedeploy"></a>
 
 # types-aiobotocore-codedeploy
 
 [![PyPI - types-aiobotocore-codedeploy](https://img.shields.io/pypi/v/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codedeploy.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codedeploy)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codedeploy?color=blue)](https://pypistats.org/packages/types-aiobotocore-codedeploy)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codedeploy)](https://pepy.tech/project/types-aiobotocore-codedeploy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeDeploy 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
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
 [types-aiobotocore-codedeploy docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
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
@@ -407,176 +406,193 @@
 )
 
 
 def check_value(value: ApplicationRevisionSortByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codedeploy.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codedeploy.type_defs import (
     TagTypeDef,
     AlarmTypeDef,
     AppSpecContentTypeDef,
     ApplicationInfoTypeDef,
+    AutoRollbackConfigurationOutputTypeDef,
     AutoRollbackConfigurationTypeDef,
     AutoScalingGroupTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetApplicationsInputRequestTypeDef,
     BatchGetDeploymentGroupsInputRequestTypeDef,
     BatchGetDeploymentInstancesInputRequestTypeDef,
     BatchGetDeploymentTargetsInputRequestTypeDef,
     BatchGetDeploymentsInputRequestTypeDef,
     BatchGetOnPremisesInstancesInputRequestTypeDef,
     BlueInstanceTerminationOptionTypeDef,
     DeploymentReadyOptionTypeDef,
     GreenFleetProvisioningOptionTypeDef,
     ContinueDeploymentInputRequestTypeDef,
-    CreateApplicationOutputTypeDef,
     MinimumHealthyHostsTypeDef,
-    CreateDeploymentConfigOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
     ECSServiceTypeDef,
     TagFilterTypeDef,
-    TriggerConfigTypeDef,
-    CreateDeploymentGroupOutputTypeDef,
-    CreateDeploymentOutputTypeDef,
     DeleteApplicationInputRequestTypeDef,
     DeleteDeploymentConfigInputRequestTypeDef,
     DeleteDeploymentGroupInputRequestTypeDef,
     DeleteGitHubAccountTokenInputRequestTypeDef,
-    DeleteGitHubAccountTokenOutputTypeDef,
     DeleteResourcesByExternalIdInputRequestTypeDef,
     LastDeploymentInfoTypeDef,
+    TriggerConfigOutputTypeDef,
     DeploymentOverviewTypeDef,
     ErrorInformationTypeDef,
     RelatedDeploymentsTypeDef,
     RollbackInfoTypeDef,
     DeregisterOnPremisesInstanceInputRequestTypeDef,
     DiagnosticsTypeDef,
     TargetGroupInfoTypeDef,
     ELBInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
     GenericRevisionInfoTypeDef,
     GetApplicationInputRequestTypeDef,
     GetDeploymentConfigInputRequestTypeDef,
     GetDeploymentGroupInputRequestTypeDef,
     WaiterConfigTypeDef,
     GetDeploymentInputRequestTypeDef,
     GetDeploymentInstanceInputRequestTypeDef,
     GetDeploymentTargetInputRequestTypeDef,
     GetOnPremisesInstanceInputRequestTypeDef,
     GitHubLocationTypeDef,
     LambdaFunctionInfoTypeDef,
-    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationRevisionsInputRequestTypeDef,
-    ListApplicationsInputListApplicationsPaginateTypeDef,
     ListApplicationsInputRequestTypeDef,
-    ListApplicationsOutputTypeDef,
-    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
     ListDeploymentConfigsInputRequestTypeDef,
-    ListDeploymentConfigsOutputTypeDef,
-    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
     ListDeploymentGroupsInputRequestTypeDef,
-    ListDeploymentGroupsOutputTypeDef,
-    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
     ListDeploymentInstancesInputRequestTypeDef,
-    ListDeploymentInstancesOutputTypeDef,
-    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
     ListDeploymentTargetsInputRequestTypeDef,
-    ListDeploymentTargetsOutputTypeDef,
-    TimeRangeTypeDef,
-    ListDeploymentsOutputTypeDef,
-    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
     ListGitHubAccountTokenNamesInputRequestTypeDef,
-    ListGitHubAccountTokenNamesOutputTypeDef,
-    ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutLifecycleEventHookExecutionStatusInputRequestTypeDef,
-    PutLifecycleEventHookExecutionStatusOutputTypeDef,
     RawStringTypeDef,
     RegisterOnPremisesInstanceInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     S3LocationTypeDef,
     SkipWaitTimeForInstanceTerminationInputRequestTypeDef,
     StopDeploymentInputRequestTypeDef,
-    StopDeploymentOutputTypeDef,
+    TrafficRouteOutputTypeDef,
     TrafficRouteTypeDef,
     TimeBasedCanaryTypeDef,
     TimeBasedLinearTypeDef,
+    TimestampTypeDef,
+    TriggerConfigTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApplicationInputRequestTypeDef,
     AddTagsToOnPremisesInstancesInputRequestTypeDef,
     CreateApplicationInputRequestTypeDef,
     InstanceInfoTypeDef,
-    ListTagsForResourceOutputTypeDef,
     RemoveTagsFromOnPremisesInstancesInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    AlarmConfigurationOutputTypeDef,
     AlarmConfigurationTypeDef,
+    AutoRollbackConfigurationUnionTypeDef,
     BatchGetApplicationsOutputTypeDef,
-    GetApplicationOutputTypeDef,
+    CreateApplicationOutputTypeDef,
+    CreateDeploymentConfigOutputTypeDef,
+    CreateDeploymentGroupOutputTypeDef,
+    CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
+    DeleteGitHubAccountTokenOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetApplicationOutputTypeDef,
+    ListApplicationsOutputTypeDef,
+    ListDeploymentConfigsOutputTypeDef,
+    ListDeploymentGroupsOutputTypeDef,
+    ListDeploymentInstancesOutputTypeDef,
+    ListDeploymentTargetsOutputTypeDef,
+    ListDeploymentsOutputTypeDef,
+    ListGitHubAccountTokenNamesOutputTypeDef,
+    ListOnPremisesInstancesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PutLifecycleEventHookExecutionStatusOutputTypeDef,
+    StopDeploymentOutputTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
     BlueGreenDeploymentConfigurationTypeDef,
+    EC2TagSetOutputTypeDef,
     EC2TagSetTypeDef,
-    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     ListOnPremisesInstancesInputRequestTypeDef,
+    OnPremisesTagSetOutputTypeDef,
     OnPremisesTagSetTypeDef,
     LifecycleEventTypeDef,
     ECSTaskSetTypeDef,
     GetDeploymentInputDeploymentSuccessfulWaitTypeDef,
-    ListDeploymentsInputListDeploymentsPaginateTypeDef,
-    ListDeploymentsInputRequestTypeDef,
+    ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef,
+    ListApplicationsInputListApplicationsPaginateTypeDef,
+    ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef,
+    ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef,
+    ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef,
+    ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef,
+    ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef,
+    ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef,
     RevisionLocationTypeDef,
+    TargetGroupPairInfoOutputTypeDef,
     TargetGroupPairInfoTypeDef,
     TrafficRoutingConfigTypeDef,
+    TimeRangeTypeDef,
+    TriggerConfigUnionTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
     GetOnPremisesInstanceOutputTypeDef,
+    AlarmConfigurationUnionTypeDef,
+    TargetInstancesOutputTypeDef,
+    EC2TagSetUnionTypeDef,
     TargetInstancesTypeDef,
+    OnPremisesTagSetUnionTypeDef,
     CloudFormationTargetTypeDef,
     InstanceSummaryTypeDef,
     InstanceTargetTypeDef,
     LambdaTargetTypeDef,
     ECSTargetTypeDef,
     BatchGetApplicationRevisionsInputRequestTypeDef,
     GetApplicationRevisionInputRequestTypeDef,
     GetApplicationRevisionOutputTypeDef,
     ListApplicationRevisionsOutputTypeDef,
     RegisterApplicationRevisionInputRequestTypeDef,
     RevisionInfoTypeDef,
+    LoadBalancerInfoOutputTypeDef,
     LoadBalancerInfoTypeDef,
     CreateDeploymentConfigInputRequestTypeDef,
     DeploymentConfigInfoTypeDef,
+    ListDeploymentsInputListDeploymentsPaginateTypeDef,
+    ListDeploymentsInputRequestTypeDef,
     CreateDeploymentInputRequestTypeDef,
+    TargetInstancesUnionTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
     DeploymentTargetTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
-    CreateDeploymentGroupInputRequestTypeDef,
     DeploymentGroupInfoTypeDef,
     DeploymentInfoTypeDef,
+    CreateDeploymentGroupInputRequestTypeDef,
+    LoadBalancerInfoUnionTypeDef,
     UpdateDeploymentGroupInputRequestTypeDef,
     GetDeploymentConfigOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     GetDeploymentTargetOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
     GetDeploymentOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codedeploy-2.5.2/types_aiobotocore_codedeploy.egg-info/SOURCES.txt` & `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


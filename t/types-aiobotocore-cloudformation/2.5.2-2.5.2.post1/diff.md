# Comparing `tmp/types-aiobotocore-cloudformation-2.5.2.tar.gz` & `tmp/types-aiobotocore-cloudformation-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudformation-2.5.2.tar", last modified: Sat Jul  8 01:43:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudformation-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:00 2023, max compression
```

## Comparing `types-aiobotocore-cloudformation-2.5.2.tar` & `types-aiobotocore-cloudformation-2.5.2.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.449823 types-aiobotocore-cloudformation-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:56.000000 types-aiobotocore-cloudformation-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30039 2023-07-08 01:43:21.449823 types-aiobotocore-cloudformation-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28446 2023-07-08 01:26:56.000000 types-aiobotocore-cloudformation-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:21.449823 types-aiobotocore-cloudformation-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 01:26:56.000000 types-aiobotocore-cloudformation-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.449823 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-07-08 01:26:56.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-08 01:26:56.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:26:56.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68293 2023-07-08 01:26:57.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68193 2023-07-08 01:26:56.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-07-08 01:26:57.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-07-08 01:26:57.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18058 2023-07-08 01:26:57.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18042 2023-07-08 01:26:57.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:56.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25564 2023-07-08 01:26:57.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    25517 2023-07-08 01:26:57.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    90394 2023-07-08 01:27:00.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    90281 2023-07-08 01:26:59.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:56.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-07-08 01:26:57.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-08 01:26:57.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.449823 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30039 2023-07-08 01:43:21.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-08 01:43:21.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:21.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:43:21.000000 types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.989637 types-aiobotocore-cloudformation-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    30136 2023-08-02 14:51:59.985637 types-aiobotocore-cloudformation-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28590 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:59.989637 types-aiobotocore-cloudformation-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.981637 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68373 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68273 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18030 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25423 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    91368 2023-08-02 14:34:30.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91255 2023-08-02 14:34:29.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.985637 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30136 2023-08-02 14:51:59.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 14:51:59.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:51:59.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/LICENSE` & `types-aiobotocore-cloudformation-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2/PKG-INFO` & `types-aiobotocore-cloudformation-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudformation
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudFormation 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudFormation 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudformation type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudformation type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudformation"></a>
 
 # types-aiobotocore-cloudformation
 
 [![PyPI - types-aiobotocore-cloudformation](https://img.shields.io/pypi/v/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudformation?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudformation)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudformation)](https://pepy.tech/project/types-aiobotocore-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudFormation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
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
 [types-aiobotocore-cloudformation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +77,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -550,177 +549,180 @@
 )
 
 
 def check_value(value: AccountFilterTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudformation.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudformation.type_defs import (
     AccountGateResultTypeDef,
     AccountLimitTypeDef,
     LoggingConfigTypeDef,
-    ActivateTypeOutputTypeDef,
+    ResponseMetadataTypeDef,
     AutoDeploymentTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeConfigurationDetailsTypeDef,
     CancelUpdateStackInputRequestTypeDef,
     CancelUpdateStackInputStackCancelUpdateTypeDef,
     ChangeSetHookResourceTargetDetailsTypeDef,
     ChangeSetSummaryTypeDef,
     ContinueUpdateRollbackInputRequestTypeDef,
     ParameterTypeDef,
     ResourceToImportTypeDef,
     TagTypeDef,
-    CreateChangeSetOutputTypeDef,
     DeploymentTargetsTypeDef,
     StackSetOperationPreferencesTypeDef,
-    CreateStackInstancesOutputTypeDef,
-    CreateStackOutputTypeDef,
     ManagedExecutionTypeDef,
-    CreateStackSetOutputTypeDef,
     DeactivateTypeInputRequestTypeDef,
     DeleteChangeSetInputRequestTypeDef,
     DeleteStackInputRequestTypeDef,
     DeleteStackInputStackDeleteTypeDef,
-    DeleteStackInstancesOutputTypeDef,
     DeleteStackSetInputRequestTypeDef,
+    DeploymentTargetsOutputTypeDef,
     DeregisterTypeInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     DescribeChangeSetHooksInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
     DescribeChangeSetInputRequestTypeDef,
     DescribeOrganizationsAccessInputRequestTypeDef,
-    DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherInputRequestTypeDef,
-    DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusInputRequestTypeDef,
-    DescribeStackDriftDetectionStatusOutputTypeDef,
-    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
     DescribeStackEventsInputRequestTypeDef,
     StackEventTypeDef,
     DescribeStackInstanceInputRequestTypeDef,
     DescribeStackResourceDriftsInputRequestTypeDef,
     DescribeStackResourceInputRequestTypeDef,
     DescribeStackResourcesInputRequestTypeDef,
     DescribeStackSetInputRequestTypeDef,
     DescribeStackSetOperationInputRequestTypeDef,
-    DescribeStacksInputDescribeStacksPaginateTypeDef,
     DescribeStacksInputRequestTypeDef,
     DescribeTypeInputRequestTypeDef,
     RequiredActivatedTypeTypeDef,
     DescribeTypeRegistrationInputRequestTypeDef,
-    DescribeTypeRegistrationOutputTypeDef,
     DetectStackDriftInputRequestTypeDef,
-    DetectStackDriftOutputTypeDef,
     DetectStackResourceDriftInputRequestTypeDef,
-    DetectStackSetDriftOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EstimateTemplateCostOutputTypeDef,
     ExecuteChangeSetInputRequestTypeDef,
     ExportTypeDef,
     GetStackPolicyInputRequestTypeDef,
-    GetStackPolicyOutputTypeDef,
     GetTemplateInputRequestTypeDef,
-    GetTemplateOutputTypeDef,
     GetTemplateSummaryInputRequestTypeDef,
     ResourceIdentifierSummaryTypeDef,
-    ImportStacksToStackSetOutputTypeDef,
-    ListChangeSetsInputListChangeSetsPaginateTypeDef,
     ListChangeSetsInputRequestTypeDef,
-    ListExportsInputListExportsPaginateTypeDef,
     ListExportsInputRequestTypeDef,
-    ListImportsInputListImportsPaginateTypeDef,
     ListImportsInputRequestTypeDef,
-    ListImportsOutputTypeDef,
     StackInstanceFilterTypeDef,
-    ListStackResourcesInputListStackResourcesPaginateTypeDef,
     ListStackResourcesInputRequestTypeDef,
     OperationResultFilterTypeDef,
-    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
     ListStackSetOperationsInputRequestTypeDef,
-    ListStackSetsInputListStackSetsPaginateTypeDef,
     ListStackSetsInputRequestTypeDef,
-    ListStacksInputListStacksPaginateTypeDef,
     ListStacksInputRequestTypeDef,
     ListTypeRegistrationsInputRequestTypeDef,
-    ListTypeRegistrationsOutputTypeDef,
     ListTypeVersionsInputRequestTypeDef,
     TypeVersionSummaryTypeDef,
     TypeFiltersTypeDef,
     TypeSummaryTypeDef,
-    ModuleInfoResponseMetadataTypeDef,
     ModuleInfoTypeDef,
     OutputTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     PhysicalResourceIdContextKeyValuePairTypeDef,
     PropertyDifferenceTypeDef,
     PublishTypeInputRequestTypeDef,
-    PublishTypeOutputTypeDef,
     RecordHandlerProgressInputRequestTypeDef,
     RegisterPublisherInputRequestTypeDef,
-    RegisterPublisherOutputTypeDef,
-    RegisterTypeOutputTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
     RollbackTriggerTypeDef,
     RollbackStackInputRequestTypeDef,
-    RollbackStackOutputTypeDef,
     SetStackPolicyInputRequestTypeDef,
     SetTypeConfigurationInputRequestTypeDef,
-    SetTypeConfigurationOutputTypeDef,
     SetTypeDefaultVersionInputRequestTypeDef,
     SignalResourceInputRequestTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
     StackDriftInformationSummaryTypeDef,
     StackDriftInformationTypeDef,
     StackInstanceComprehensiveStatusTypeDef,
     StackResourceDriftInformationTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryTypeDef,
     StackSetDriftDetectionDetailsTypeDef,
+    StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationStatusDetailsTypeDef,
     StopStackSetOperationInputRequestTypeDef,
     TemplateParameterTypeDef,
     TestTypeInputRequestTypeDef,
-    TestTypeOutputTypeDef,
-    UpdateStackInstancesOutputTypeDef,
-    UpdateStackOutputTypeDef,
-    UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionInputRequestTypeDef,
-    UpdateTerminationProtectionOutputTypeDef,
     ValidateTemplateInputRequestTypeDef,
     StackSetOperationResultSummaryTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
     ActivateTypeInputRequestTypeDef,
     RegisterTypeInputRequestTypeDef,
+    ActivateTypeOutputTypeDef,
+    CreateChangeSetOutputTypeDef,
+    CreateStackInstancesOutputTypeDef,
+    CreateStackOutputTypeDef,
+    CreateStackSetOutputTypeDef,
+    DeleteStackInstancesOutputTypeDef,
+    DescribeAccountLimitsOutputTypeDef,
+    DescribeOrganizationsAccessOutputTypeDef,
+    DescribePublisherOutputTypeDef,
+    DescribeStackDriftDetectionStatusOutputTypeDef,
+    DescribeTypeRegistrationOutputTypeDef,
+    DetectStackDriftOutputTypeDef,
+    DetectStackSetDriftOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EstimateTemplateCostOutputTypeDef,
+    GetStackPolicyOutputTypeDef,
+    GetTemplateOutputTypeDef,
+    ImportStacksToStackSetOutputTypeDef,
+    ListImportsOutputTypeDef,
+    ListTypeRegistrationsOutputTypeDef,
+    ModuleInfoResponseTypeDef,
+    PublishTypeOutputTypeDef,
+    RegisterPublisherOutputTypeDef,
+    RegisterTypeOutputTypeDef,
+    RollbackStackOutputTypeDef,
+    SetTypeConfigurationOutputTypeDef,
+    StackDriftInformationResponseTypeDef,
+    StackResourceDriftInformationResponseTypeDef,
+    StackResourceDriftInformationSummaryResponseTypeDef,
+    TestTypeOutputTypeDef,
+    UpdateStackInstancesOutputTypeDef,
+    UpdateStackOutputTypeDef,
+    UpdateStackSetOutputTypeDef,
+    UpdateTerminationProtectionOutputTypeDef,
     BatchDescribeTypeConfigurationsErrorTypeDef,
     BatchDescribeTypeConfigurationsInputRequestTypeDef,
     ChangeSetHookTargetDetailsTypeDef,
     ListChangeSetsOutputTypeDef,
     EstimateTemplateCostInputRequestTypeDef,
     CreateStackInstancesInputRequestTypeDef,
     DeleteStackInstancesInputRequestTypeDef,
     DetectStackSetDriftInputRequestTypeDef,
     ImportStacksToStackSetInputRequestTypeDef,
     UpdateStackInstancesInputRequestTypeDef,
     CreateStackSetInputRequestTypeDef,
     StackSetSummaryTypeDef,
     UpdateStackSetInputRequestTypeDef,
+    DeploymentTargetsUnionTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
+    DescribeStacksInputDescribeStacksPaginateTypeDef,
+    ListChangeSetsInputListChangeSetsPaginateTypeDef,
+    ListExportsInputListExportsPaginateTypeDef,
+    ListImportsInputListImportsPaginateTypeDef,
+    ListStackResourcesInputListStackResourcesPaginateTypeDef,
+    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    ListStackSetsInputListStackSetsPaginateTypeDef,
+    ListStacksInputListStacksPaginateTypeDef,
     DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     DescribeStacksInputStackCreateCompleteWaitTypeDef,
     DescribeStacksInputStackDeleteCompleteWaitTypeDef,
     DescribeStacksInputStackExistsWaitTypeDef,
     DescribeStacksInputStackImportCompleteWaitTypeDef,
     DescribeStacksInputStackRollbackCompleteWaitTypeDef,
     DescribeStacksInputStackUpdateCompleteWaitTypeDef,
@@ -735,38 +737,40 @@
     ListTypeVersionsOutputTypeDef,
     ListTypesInputListTypesPaginateTypeDef,
     ListTypesInputRequestTypeDef,
     ListTypesOutputTypeDef,
     ParameterDeclarationTypeDef,
     StackResourceDriftTypeDef,
     ResourceChangeDetailTypeDef,
-    RollbackConfigurationResponseMetadataTypeDef,
+    RollbackConfigurationOutputTypeDef,
     RollbackConfigurationTypeDef,
     StackSummaryTypeDef,
     StackInstanceSummaryTypeDef,
     StackInstanceTypeDef,
     StackResourceDetailTypeDef,
     StackResourceTypeDef,
     StackResourceSummaryTypeDef,
     StackSetTypeDef,
+    StackSetOperationPreferencesUnionTypeDef,
     StackSetOperationSummaryTypeDef,
     StackSetOperationTypeDef,
     ValidateTemplateOutputTypeDef,
     ListStackSetOperationResultsOutputTypeDef,
     BatchDescribeTypeConfigurationsOutputTypeDef,
     ChangeSetHookTypeDef,
     ListStackSetsOutputTypeDef,
     GetTemplateSummaryOutputTypeDef,
     DescribeStackResourceDriftsOutputTypeDef,
     DetectStackResourceDriftOutputTypeDef,
     ResourceChangeTypeDef,
+    StackTypeDef,
     CreateChangeSetInputRequestTypeDef,
     CreateStackInputRequestTypeDef,
     CreateStackInputServiceResourceCreateStackTypeDef,
-    StackTypeDef,
+    RollbackConfigurationUnionTypeDef,
     UpdateStackInputRequestTypeDef,
     UpdateStackInputStackUpdateTypeDef,
     ListStacksOutputTypeDef,
     ListStackInstancesOutputTypeDef,
     DescribeStackInstanceOutputTypeDef,
     DescribeStackResourceOutputTypeDef,
     DescribeStackResourcesOutputTypeDef,
@@ -777,15 +781,15 @@
     DescribeChangeSetHooksOutputTypeDef,
     ChangeTypeDef,
     DescribeStacksOutputTypeDef,
     DescribeChangeSetOutputTypeDef,
 )
 
 
-def get_structure() -> AccountGateResultTypeDef:
+def get_value() -> AccountGateResultTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/README.md` & `types-aiobotocore-cloudformation-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cloudformation"></a>
 
 # types-aiobotocore-cloudformation
 
 [![PyPI - types-aiobotocore-cloudformation](https://img.shields.io/pypi/v/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudformation?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudformation)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudformation)](https://pepy.tech/project/types-aiobotocore-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudFormation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
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
 [types-aiobotocore-cloudformation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -45,15 +45,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -517,177 +517,180 @@
 )
 
 
 def check_value(value: AccountFilterTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudformation.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudformation.type_defs import (
     AccountGateResultTypeDef,
     AccountLimitTypeDef,
     LoggingConfigTypeDef,
-    ActivateTypeOutputTypeDef,
+    ResponseMetadataTypeDef,
     AutoDeploymentTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeConfigurationDetailsTypeDef,
     CancelUpdateStackInputRequestTypeDef,
     CancelUpdateStackInputStackCancelUpdateTypeDef,
     ChangeSetHookResourceTargetDetailsTypeDef,
     ChangeSetSummaryTypeDef,
     ContinueUpdateRollbackInputRequestTypeDef,
     ParameterTypeDef,
     ResourceToImportTypeDef,
     TagTypeDef,
-    CreateChangeSetOutputTypeDef,
     DeploymentTargetsTypeDef,
     StackSetOperationPreferencesTypeDef,
-    CreateStackInstancesOutputTypeDef,
-    CreateStackOutputTypeDef,
     ManagedExecutionTypeDef,
-    CreateStackSetOutputTypeDef,
     DeactivateTypeInputRequestTypeDef,
     DeleteChangeSetInputRequestTypeDef,
     DeleteStackInputRequestTypeDef,
     DeleteStackInputStackDeleteTypeDef,
-    DeleteStackInstancesOutputTypeDef,
     DeleteStackSetInputRequestTypeDef,
+    DeploymentTargetsOutputTypeDef,
     DeregisterTypeInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     DescribeChangeSetHooksInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
     DescribeChangeSetInputRequestTypeDef,
     DescribeOrganizationsAccessInputRequestTypeDef,
-    DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherInputRequestTypeDef,
-    DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusInputRequestTypeDef,
-    DescribeStackDriftDetectionStatusOutputTypeDef,
-    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
     DescribeStackEventsInputRequestTypeDef,
     StackEventTypeDef,
     DescribeStackInstanceInputRequestTypeDef,
     DescribeStackResourceDriftsInputRequestTypeDef,
     DescribeStackResourceInputRequestTypeDef,
     DescribeStackResourcesInputRequestTypeDef,
     DescribeStackSetInputRequestTypeDef,
     DescribeStackSetOperationInputRequestTypeDef,
-    DescribeStacksInputDescribeStacksPaginateTypeDef,
     DescribeStacksInputRequestTypeDef,
     DescribeTypeInputRequestTypeDef,
     RequiredActivatedTypeTypeDef,
     DescribeTypeRegistrationInputRequestTypeDef,
-    DescribeTypeRegistrationOutputTypeDef,
     DetectStackDriftInputRequestTypeDef,
-    DetectStackDriftOutputTypeDef,
     DetectStackResourceDriftInputRequestTypeDef,
-    DetectStackSetDriftOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EstimateTemplateCostOutputTypeDef,
     ExecuteChangeSetInputRequestTypeDef,
     ExportTypeDef,
     GetStackPolicyInputRequestTypeDef,
-    GetStackPolicyOutputTypeDef,
     GetTemplateInputRequestTypeDef,
-    GetTemplateOutputTypeDef,
     GetTemplateSummaryInputRequestTypeDef,
     ResourceIdentifierSummaryTypeDef,
-    ImportStacksToStackSetOutputTypeDef,
-    ListChangeSetsInputListChangeSetsPaginateTypeDef,
     ListChangeSetsInputRequestTypeDef,
-    ListExportsInputListExportsPaginateTypeDef,
     ListExportsInputRequestTypeDef,
-    ListImportsInputListImportsPaginateTypeDef,
     ListImportsInputRequestTypeDef,
-    ListImportsOutputTypeDef,
     StackInstanceFilterTypeDef,
-    ListStackResourcesInputListStackResourcesPaginateTypeDef,
     ListStackResourcesInputRequestTypeDef,
     OperationResultFilterTypeDef,
-    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
     ListStackSetOperationsInputRequestTypeDef,
-    ListStackSetsInputListStackSetsPaginateTypeDef,
     ListStackSetsInputRequestTypeDef,
-    ListStacksInputListStacksPaginateTypeDef,
     ListStacksInputRequestTypeDef,
     ListTypeRegistrationsInputRequestTypeDef,
-    ListTypeRegistrationsOutputTypeDef,
     ListTypeVersionsInputRequestTypeDef,
     TypeVersionSummaryTypeDef,
     TypeFiltersTypeDef,
     TypeSummaryTypeDef,
-    ModuleInfoResponseMetadataTypeDef,
     ModuleInfoTypeDef,
     OutputTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     PhysicalResourceIdContextKeyValuePairTypeDef,
     PropertyDifferenceTypeDef,
     PublishTypeInputRequestTypeDef,
-    PublishTypeOutputTypeDef,
     RecordHandlerProgressInputRequestTypeDef,
     RegisterPublisherInputRequestTypeDef,
-    RegisterPublisherOutputTypeDef,
-    RegisterTypeOutputTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
     RollbackTriggerTypeDef,
     RollbackStackInputRequestTypeDef,
-    RollbackStackOutputTypeDef,
     SetStackPolicyInputRequestTypeDef,
     SetTypeConfigurationInputRequestTypeDef,
-    SetTypeConfigurationOutputTypeDef,
     SetTypeDefaultVersionInputRequestTypeDef,
     SignalResourceInputRequestTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
     StackDriftInformationSummaryTypeDef,
     StackDriftInformationTypeDef,
     StackInstanceComprehensiveStatusTypeDef,
     StackResourceDriftInformationTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryTypeDef,
     StackSetDriftDetectionDetailsTypeDef,
+    StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationStatusDetailsTypeDef,
     StopStackSetOperationInputRequestTypeDef,
     TemplateParameterTypeDef,
     TestTypeInputRequestTypeDef,
-    TestTypeOutputTypeDef,
-    UpdateStackInstancesOutputTypeDef,
-    UpdateStackOutputTypeDef,
-    UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionInputRequestTypeDef,
-    UpdateTerminationProtectionOutputTypeDef,
     ValidateTemplateInputRequestTypeDef,
     StackSetOperationResultSummaryTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
     ActivateTypeInputRequestTypeDef,
     RegisterTypeInputRequestTypeDef,
+    ActivateTypeOutputTypeDef,
+    CreateChangeSetOutputTypeDef,
+    CreateStackInstancesOutputTypeDef,
+    CreateStackOutputTypeDef,
+    CreateStackSetOutputTypeDef,
+    DeleteStackInstancesOutputTypeDef,
+    DescribeAccountLimitsOutputTypeDef,
+    DescribeOrganizationsAccessOutputTypeDef,
+    DescribePublisherOutputTypeDef,
+    DescribeStackDriftDetectionStatusOutputTypeDef,
+    DescribeTypeRegistrationOutputTypeDef,
+    DetectStackDriftOutputTypeDef,
+    DetectStackSetDriftOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EstimateTemplateCostOutputTypeDef,
+    GetStackPolicyOutputTypeDef,
+    GetTemplateOutputTypeDef,
+    ImportStacksToStackSetOutputTypeDef,
+    ListImportsOutputTypeDef,
+    ListTypeRegistrationsOutputTypeDef,
+    ModuleInfoResponseTypeDef,
+    PublishTypeOutputTypeDef,
+    RegisterPublisherOutputTypeDef,
+    RegisterTypeOutputTypeDef,
+    RollbackStackOutputTypeDef,
+    SetTypeConfigurationOutputTypeDef,
+    StackDriftInformationResponseTypeDef,
+    StackResourceDriftInformationResponseTypeDef,
+    StackResourceDriftInformationSummaryResponseTypeDef,
+    TestTypeOutputTypeDef,
+    UpdateStackInstancesOutputTypeDef,
+    UpdateStackOutputTypeDef,
+    UpdateStackSetOutputTypeDef,
+    UpdateTerminationProtectionOutputTypeDef,
     BatchDescribeTypeConfigurationsErrorTypeDef,
     BatchDescribeTypeConfigurationsInputRequestTypeDef,
     ChangeSetHookTargetDetailsTypeDef,
     ListChangeSetsOutputTypeDef,
     EstimateTemplateCostInputRequestTypeDef,
     CreateStackInstancesInputRequestTypeDef,
     DeleteStackInstancesInputRequestTypeDef,
     DetectStackSetDriftInputRequestTypeDef,
     ImportStacksToStackSetInputRequestTypeDef,
     UpdateStackInstancesInputRequestTypeDef,
     CreateStackSetInputRequestTypeDef,
     StackSetSummaryTypeDef,
     UpdateStackSetInputRequestTypeDef,
+    DeploymentTargetsUnionTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
+    DescribeStacksInputDescribeStacksPaginateTypeDef,
+    ListChangeSetsInputListChangeSetsPaginateTypeDef,
+    ListExportsInputListExportsPaginateTypeDef,
+    ListImportsInputListImportsPaginateTypeDef,
+    ListStackResourcesInputListStackResourcesPaginateTypeDef,
+    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    ListStackSetsInputListStackSetsPaginateTypeDef,
+    ListStacksInputListStacksPaginateTypeDef,
     DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     DescribeStacksInputStackCreateCompleteWaitTypeDef,
     DescribeStacksInputStackDeleteCompleteWaitTypeDef,
     DescribeStacksInputStackExistsWaitTypeDef,
     DescribeStacksInputStackImportCompleteWaitTypeDef,
     DescribeStacksInputStackRollbackCompleteWaitTypeDef,
     DescribeStacksInputStackUpdateCompleteWaitTypeDef,
@@ -702,38 +705,40 @@
     ListTypeVersionsOutputTypeDef,
     ListTypesInputListTypesPaginateTypeDef,
     ListTypesInputRequestTypeDef,
     ListTypesOutputTypeDef,
     ParameterDeclarationTypeDef,
     StackResourceDriftTypeDef,
     ResourceChangeDetailTypeDef,
-    RollbackConfigurationResponseMetadataTypeDef,
+    RollbackConfigurationOutputTypeDef,
     RollbackConfigurationTypeDef,
     StackSummaryTypeDef,
     StackInstanceSummaryTypeDef,
     StackInstanceTypeDef,
     StackResourceDetailTypeDef,
     StackResourceTypeDef,
     StackResourceSummaryTypeDef,
     StackSetTypeDef,
+    StackSetOperationPreferencesUnionTypeDef,
     StackSetOperationSummaryTypeDef,
     StackSetOperationTypeDef,
     ValidateTemplateOutputTypeDef,
     ListStackSetOperationResultsOutputTypeDef,
     BatchDescribeTypeConfigurationsOutputTypeDef,
     ChangeSetHookTypeDef,
     ListStackSetsOutputTypeDef,
     GetTemplateSummaryOutputTypeDef,
     DescribeStackResourceDriftsOutputTypeDef,
     DetectStackResourceDriftOutputTypeDef,
     ResourceChangeTypeDef,
+    StackTypeDef,
     CreateChangeSetInputRequestTypeDef,
     CreateStackInputRequestTypeDef,
     CreateStackInputServiceResourceCreateStackTypeDef,
-    StackTypeDef,
+    RollbackConfigurationUnionTypeDef,
     UpdateStackInputRequestTypeDef,
     UpdateStackInputStackUpdateTypeDef,
     ListStacksOutputTypeDef,
     ListStackInstancesOutputTypeDef,
     DescribeStackInstanceOutputTypeDef,
     DescribeStackResourceOutputTypeDef,
     DescribeStackResourcesOutputTypeDef,
@@ -744,15 +749,15 @@
     DescribeChangeSetHooksOutputTypeDef,
     ChangeTypeDef,
     DescribeStacksOutputTypeDef,
     DescribeChangeSetOutputTypeDef,
 )
 
 
-def get_structure() -> AccountGateResultTypeDef:
+def get_value() -> AccountGateResultTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/setup.py` & `types-aiobotocore-cloudformation-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudformation",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cloudformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudFormation 2.5.2 service generated with"
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
-    keywords="aiobotocore cloudformation type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cloudformation type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudformation": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/"
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/__init__.py` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,17 @@
     StackUpdateCompleteWaiter,
     TypeRegistrationCompleteWaiter,
 )
 
 Client = CloudFormationClient
 
 
+ServiceResource = CloudFormationServiceResource
+
+
 __all__ = (
     "ChangeSetCreateCompleteWaiter",
     "Client",
     "CloudFormationClient",
     "CloudFormationServiceResource",
     "DescribeAccountLimitsPaginator",
     "DescribeChangeSetPaginator",
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/__init__.pyi` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,16 @@
     StackRollbackCompleteWaiter,
     StackUpdateCompleteWaiter,
     TypeRegistrationCompleteWaiter,
 )
 
 Client = CloudFormationClient
 
+ServiceResource = CloudFormationServiceResource
+
 __all__ = (
     "ChangeSetCreateCompleteWaiter",
     "Client",
     "CloudFormationClient",
     "CloudFormationServiceResource",
     "DescribeAccountLimitsPaginator",
     "DescribeChangeSetPaginator",
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/__main__.py` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudFormation 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CloudFormation 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation\nOther"
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

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/client.py` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     AutoDeploymentTypeDef,
     BatchDescribeTypeConfigurationsOutputTypeDef,
     CreateChangeSetOutputTypeDef,
     CreateStackInstancesOutputTypeDef,
     CreateStackOutputTypeDef,
     CreateStackSetOutputTypeDef,
     DeleteStackInstancesOutputTypeDef,
-    DeploymentTargetsTypeDef,
+    DeploymentTargetsUnionTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeChangeSetHooksOutputTypeDef,
     DescribeChangeSetOutputTypeDef,
     DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusOutputTypeDef,
     DescribeStackEventsOutputTypeDef,
@@ -109,19 +109,19 @@
     ManagedExecutionTypeDef,
     OperationResultFilterTypeDef,
     ParameterTypeDef,
     PublishTypeOutputTypeDef,
     RegisterPublisherOutputTypeDef,
     RegisterTypeOutputTypeDef,
     ResourceToImportTypeDef,
-    RollbackConfigurationTypeDef,
+    RollbackConfigurationUnionTypeDef,
     RollbackStackOutputTypeDef,
     SetTypeConfigurationOutputTypeDef,
     StackInstanceFilterTypeDef,
-    StackSetOperationPreferencesTypeDef,
+    StackSetOperationPreferencesUnionTypeDef,
     TagTypeDef,
     TestTypeOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeFiltersTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
     UpdateStackSetOutputTypeDef,
@@ -290,15 +290,15 @@
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         UsePreviousTemplate: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         Description: str = ...,
         ChangeSetType: ChangeSetTypeType = ...,
         ResourcesToImport: Sequence[ResourceToImportTypeDef] = ...,
         IncludeNestedStacks: bool = ...,
@@ -316,15 +316,15 @@
         self,
         *,
         StackName: str,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         DisableRollback: bool = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
         TimeoutInMinutes: int = ...,
         NotificationARNs: Sequence[str] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
@@ -342,17 +342,17 @@
 
     async def create_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> CreateStackInstancesOutputTypeDef:
         """
         Creates stack instances for the specified accounts, within the specified Amazon
         Web Services Regions.
 
@@ -433,16 +433,16 @@
     async def delete_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         RetainStacks: bool,
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> DeleteStackInstancesOutputTypeDef:
         """
         Deletes stack instances for the specified accounts, in the specified Amazon Web
         Services Regions.
 
@@ -689,15 +689,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#detect_stack_resource_drift)
         """
 
     async def detect_stack_set_drift(
         self,
         *,
         StackSetName: str,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> DetectStackSetDriftOutputTypeDef:
         """
         Detect drift on a stack set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.detect_stack_set_drift)
@@ -789,15 +789,15 @@
     async def import_stacks_to_stack_set(
         self,
         *,
         StackSetName: str,
         StackIds: Sequence[str] = ...,
         StackIdsUrl: str = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> ImportStacksToStackSetOutputTypeDef:
         """
         Import existing stacks into a new stack sets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.import_stacks_to_stack_set)
@@ -1141,15 +1141,15 @@
         UsePreviousTemplate: bool = ...,
         StackPolicyDuringUpdateBody: str = ...,
         StackPolicyDuringUpdateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
         ClientRequestToken: str = ...
     ) -> UpdateStackOutputTypeDef:
@@ -1162,17 +1162,17 @@
 
     async def update_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> UpdateStackInstancesOutputTypeDef:
         """
         Updates the parameter values for stack instances for the specified accounts,
         within the specified Amazon Web Services Regions.
 
@@ -1187,18 +1187,18 @@
         Description: str = ...,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         UsePreviousTemplate: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
         AdministrationRoleARN: str = ...,
         ExecutionRoleName: str = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
         PermissionModel: PermissionModelsType = ...,
         AutoDeployment: AutoDeploymentTypeDef = ...,
         OperationId: str = ...,
         Accounts: Sequence[str] = ...,
         Regions: Sequence[str] = ...,
         CallAs: CallAsType = ...,
         ManagedExecution: ManagedExecutionTypeDef = ...
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/client.pyi` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     AutoDeploymentTypeDef,
     BatchDescribeTypeConfigurationsOutputTypeDef,
     CreateChangeSetOutputTypeDef,
     CreateStackInstancesOutputTypeDef,
     CreateStackOutputTypeDef,
     CreateStackSetOutputTypeDef,
     DeleteStackInstancesOutputTypeDef,
-    DeploymentTargetsTypeDef,
+    DeploymentTargetsUnionTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeChangeSetHooksOutputTypeDef,
     DescribeChangeSetOutputTypeDef,
     DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusOutputTypeDef,
     DescribeStackEventsOutputTypeDef,
@@ -109,19 +109,19 @@
     ManagedExecutionTypeDef,
     OperationResultFilterTypeDef,
     ParameterTypeDef,
     PublishTypeOutputTypeDef,
     RegisterPublisherOutputTypeDef,
     RegisterTypeOutputTypeDef,
     ResourceToImportTypeDef,
-    RollbackConfigurationTypeDef,
+    RollbackConfigurationUnionTypeDef,
     RollbackStackOutputTypeDef,
     SetTypeConfigurationOutputTypeDef,
     StackInstanceFilterTypeDef,
-    StackSetOperationPreferencesTypeDef,
+    StackSetOperationPreferencesUnionTypeDef,
     TagTypeDef,
     TestTypeOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeFiltersTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
     UpdateStackSetOutputTypeDef,
@@ -278,15 +278,15 @@
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         UsePreviousTemplate: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         Description: str = ...,
         ChangeSetType: ChangeSetTypeType = ...,
         ResourcesToImport: Sequence[ResourceToImportTypeDef] = ...,
         IncludeNestedStacks: bool = ...,
@@ -303,15 +303,15 @@
         self,
         *,
         StackName: str,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         DisableRollback: bool = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
         TimeoutInMinutes: int = ...,
         NotificationARNs: Sequence[str] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
@@ -328,17 +328,17 @@
         """
     async def create_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> CreateStackInstancesOutputTypeDef:
         """
         Creates stack instances for the specified accounts, within the specified Amazon
         Web Services Regions.
 
@@ -413,16 +413,16 @@
     async def delete_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         RetainStacks: bool,
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> DeleteStackInstancesOutputTypeDef:
         """
         Deletes stack instances for the specified accounts, in the specified Amazon Web
         Services Regions.
 
@@ -648,15 +648,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.detect_stack_resource_drift)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#detect_stack_resource_drift)
         """
     async def detect_stack_set_drift(
         self,
         *,
         StackSetName: str,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> DetectStackSetDriftOutputTypeDef:
         """
         Detect drift on a stack set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.detect_stack_set_drift)
@@ -741,15 +741,15 @@
     async def import_stacks_to_stack_set(
         self,
         *,
         StackSetName: str,
         StackIds: Sequence[str] = ...,
         StackIdsUrl: str = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> ImportStacksToStackSetOutputTypeDef:
         """
         Import existing stacks into a new stack sets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.import_stacks_to_stack_set)
@@ -1069,15 +1069,15 @@
         UsePreviousTemplate: bool = ...,
         StackPolicyDuringUpdateBody: str = ...,
         StackPolicyDuringUpdateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
         ClientRequestToken: str = ...
     ) -> UpdateStackOutputTypeDef:
@@ -1089,17 +1089,17 @@
         """
     async def update_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> UpdateStackInstancesOutputTypeDef:
         """
         Updates the parameter values for stack instances for the specified accounts,
         within the specified Amazon Web Services Regions.
 
@@ -1113,18 +1113,18 @@
         Description: str = ...,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         UsePreviousTemplate: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
         AdministrationRoleARN: str = ...,
         ExecutionRoleName: str = ...,
-        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
         PermissionModel: PermissionModelsType = ...,
         AutoDeployment: AutoDeploymentTypeDef = ...,
         OperationId: str = ...,
         Accounts: Sequence[str] = ...,
         Regions: Sequence[str] = ...,
         CallAs: CallAsType = ...,
         ManagedExecution: ManagedExecutionTypeDef = ...
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/literals.py` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/literals.pyi` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/paginator.py` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 class DescribeAccountLimitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describeaccountlimitspaginator)
         """
 
 
@@ -131,90 +131,90 @@
     """
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeChangeSetOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describechangesetpaginator)
         """
 
 
 class DescribeStackEventsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackeventspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeStackEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackeventspaginator)
         """
 
 
 class DescribeStacksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackspaginator)
         """
 
 
 class ListChangeSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listchangesetspaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListChangeSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listchangesetspaginator)
         """
 
 
 class ListExportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listexportspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listexportspaginator)
         """
 
 
 class ListImportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listimportspaginator)
     """
 
     def paginate(
-        self, *, ExportName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ExportName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListImportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listimportspaginator)
         """
 
 
@@ -228,30 +228,30 @@
         self,
         *,
         StackSetName: str,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
         StackInstanceAccount: str = ...,
         StackInstanceRegion: str = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStackInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackinstancespaginator)
         """
 
 
 class ListStackResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackresourcespaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStackResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackresourcespaginator)
         """
 
 
@@ -264,15 +264,15 @@
     def paginate(
         self,
         *,
         StackSetName: str,
         OperationId: str,
         CallAs: CallAsType = ...,
         Filters: Sequence[OperationResultFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStackSetOperationResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationresultspaginator)
         """
 
 
@@ -283,15 +283,15 @@
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStackSetOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
 
@@ -302,15 +302,15 @@
     """
 
     def paginate(
         self,
         *,
         Status: StackSetStatusType = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStackSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetspaginator)
         """
 
 
@@ -320,15 +320,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackspaginator)
     """
 
     def paginate(
         self,
         *,
         StackStatusFilter: Sequence[StackStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackspaginator)
         """
 
 
@@ -342,13 +342,13 @@
         self,
         *,
         Visibility: VisibilityType = ...,
         ProvisioningType: ProvisioningTypeType = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
         Type: RegistryTypeType = ...,
         Filters: TypeFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listtypespaginator)
         """
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/paginator.pyi` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 class DescribeAccountLimitsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describeaccountlimitspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAccountLimitsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeAccountLimits.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describeaccountlimitspaginator)
         """
 
 class DescribeChangeSetPaginator(AioPaginator):
@@ -127,85 +127,85 @@
     """
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeChangeSetOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describechangesetpaginator)
         """
 
 class DescribeStackEventsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackeventspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeStackEventsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStackEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackeventspaginator)
         """
 
 class DescribeStacksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
-        self, *, StackName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackspaginator)
         """
 
 class ListChangeSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listchangesetspaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListChangeSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListChangeSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listchangesetspaginator)
         """
 
 class ListExportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listexportspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listexportspaginator)
         """
 
 class ListImportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listimportspaginator)
     """
 
     def paginate(
-        self, *, ExportName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ExportName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListImportsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListImports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listimportspaginator)
         """
 
 class ListStackInstancesPaginator(AioPaginator):
@@ -218,29 +218,29 @@
         self,
         *,
         StackSetName: str,
         Filters: Sequence[StackInstanceFilterTypeDef] = ...,
         StackInstanceAccount: str = ...,
         StackInstanceRegion: str = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStackInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackinstancespaginator)
         """
 
 class ListStackResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackresourcespaginator)
     """
 
     def paginate(
-        self, *, StackName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, StackName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStackResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackresourcespaginator)
         """
 
 class ListStackSetOperationResultsPaginator(AioPaginator):
@@ -252,15 +252,15 @@
     def paginate(
         self,
         *,
         StackSetName: str,
         OperationId: str,
         CallAs: CallAsType = ...,
         Filters: Sequence[OperationResultFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStackSetOperationResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperationResults.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationresultspaginator)
         """
 
 class ListStackSetOperationsPaginator(AioPaginator):
@@ -270,15 +270,15 @@
     """
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStackSetOperationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
 class ListStackSetsPaginator(AioPaginator):
@@ -288,15 +288,15 @@
     """
 
     def paginate(
         self,
         *,
         Status: StackSetStatusType = ...,
         CallAs: CallAsType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStackSetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetspaginator)
         """
 
 class ListStacksPaginator(AioPaginator):
@@ -305,15 +305,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackspaginator)
     """
 
     def paginate(
         self,
         *,
         StackStatusFilter: Sequence[StackStatusType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStacksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststackspaginator)
         """
 
 class ListTypesPaginator(AioPaginator):
@@ -326,13 +326,13 @@
         self,
         *,
         Visibility: VisibilityType = ...,
         ProvisioningType: ProvisioningTypeType = ...,
         DeprecatedStatus: DeprecatedStatusType = ...,
         Type: RegistryTypeType = ...,
         Filters: TypeFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#listtypespaginator)
         """
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/service_resource.py` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     HookFailureModeType,
     HookStatusType,
     OnFailureType,
     ResourceStatusType,
     StackStatusType,
 )
 from .type_defs import (
-    ModuleInfoResponseMetadataTypeDef,
+    ModuleInfoResponseTypeDef,
     OutputTypeDef,
     ParameterTypeDef,
-    RollbackConfigurationResponseMetadataTypeDef,
     RollbackConfigurationTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
+    RollbackConfigurationUnionTypeDef,
+    StackDriftInformationResponseTypeDef,
+    StackResourceDriftInformationResponseTypeDef,
+    StackResourceDriftInformationSummaryResponseTypeDef,
     TagTypeDef,
     UpdateStackOutputTypeDef,
 )
 
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
@@ -264,28 +264,28 @@
     stack_name: Awaitable[str]
     change_set_id: Awaitable[str]
     description: Awaitable[str]
     parameters: Awaitable[List[ParameterTypeDef]]
     creation_time: Awaitable[datetime]
     deletion_time: Awaitable[datetime]
     last_updated_time: Awaitable[datetime]
-    rollback_configuration: Awaitable[RollbackConfigurationResponseMetadataTypeDef]
+    rollback_configuration: Awaitable[RollbackConfigurationTypeDef]
     stack_status: Awaitable[StackStatusType]
     stack_status_reason: Awaitable[str]
     disable_rollback: Awaitable[bool]
     notification_arns: Awaitable[List[str]]
     timeout_in_minutes: Awaitable[int]
     capabilities: Awaitable[List[CapabilityType]]
     outputs: Awaitable[List[OutputTypeDef]]
     role_arn: Awaitable[str]
     tags: Awaitable[List[TagTypeDef]]
     enable_termination_protection: Awaitable[bool]
     parent_id: Awaitable[str]
     root_id: Awaitable[str]
-    drift_information: Awaitable[StackDriftInformationResponseMetadataTypeDef]
+    drift_information: Awaitable[StackDriftInformationResponseTypeDef]
     name: str
     events: StackEventsCollection
     resource_summaries: StackResourceSummariesCollection
 
     async def Resource(self, logical_id: str) -> "_StackResource":
         """
         Creates a StackResource resource.
@@ -384,16 +384,16 @@
     physical_resource_id: Awaitable[str]
     resource_type: Awaitable[str]
     last_updated_timestamp: Awaitable[datetime]
     resource_status: Awaitable[ResourceStatusType]
     resource_status_reason: Awaitable[str]
     description: Awaitable[str]
     metadata: Awaitable[str]
-    drift_information: Awaitable[StackResourceDriftInformationResponseMetadataTypeDef]
-    module_info: Awaitable[ModuleInfoResponseMetadataTypeDef]
+    drift_information: Awaitable[StackResourceDriftInformationResponseTypeDef]
+    module_info: Awaitable[ModuleInfoResponseTypeDef]
     stack_name: str
     logical_id: str
 
     async def Stack(self) -> _Stack:
         """
         Creates a Stack resource.
 
@@ -439,16 +439,16 @@
 
     logical_resource_id: Awaitable[str]
     physical_resource_id: Awaitable[str]
     resource_type: Awaitable[str]
     last_updated_timestamp: Awaitable[datetime]
     resource_status: Awaitable[ResourceStatusType]
     resource_status_reason: Awaitable[str]
-    drift_information: Awaitable[StackResourceDriftInformationSummaryResponseMetadataTypeDef]
-    module_info: Awaitable[ModuleInfoResponseMetadataTypeDef]
+    drift_information: Awaitable[StackResourceDriftInformationSummaryResponseTypeDef]
+    module_info: Awaitable[ModuleInfoResponseTypeDef]
     stack_name: str
     logical_id: str
 
     async def Resource(self) -> _StackResource:
         """
         Creates a StackResource resource.
 
@@ -517,15 +517,15 @@
         self,
         *,
         StackName: str,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         DisableRollback: bool = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
         TimeoutInMinutes: int = ...,
         NotificationARNs: Sequence[str] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/service_resource.pyi` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,22 @@
     HookFailureModeType,
     HookStatusType,
     OnFailureType,
     ResourceStatusType,
     StackStatusType,
 )
 from .type_defs import (
-    ModuleInfoResponseMetadataTypeDef,
+    ModuleInfoResponseTypeDef,
     OutputTypeDef,
     ParameterTypeDef,
-    RollbackConfigurationResponseMetadataTypeDef,
     RollbackConfigurationTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
+    RollbackConfigurationUnionTypeDef,
+    StackDriftInformationResponseTypeDef,
+    StackResourceDriftInformationResponseTypeDef,
+    StackResourceDriftInformationSummaryResponseTypeDef,
     TagTypeDef,
     UpdateStackOutputTypeDef,
 )
 
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
@@ -239,28 +239,28 @@
     stack_name: Awaitable[str]
     change_set_id: Awaitable[str]
     description: Awaitable[str]
     parameters: Awaitable[List[ParameterTypeDef]]
     creation_time: Awaitable[datetime]
     deletion_time: Awaitable[datetime]
     last_updated_time: Awaitable[datetime]
-    rollback_configuration: Awaitable[RollbackConfigurationResponseMetadataTypeDef]
+    rollback_configuration: Awaitable[RollbackConfigurationTypeDef]
     stack_status: Awaitable[StackStatusType]
     stack_status_reason: Awaitable[str]
     disable_rollback: Awaitable[bool]
     notification_arns: Awaitable[List[str]]
     timeout_in_minutes: Awaitable[int]
     capabilities: Awaitable[List[CapabilityType]]
     outputs: Awaitable[List[OutputTypeDef]]
     role_arn: Awaitable[str]
     tags: Awaitable[List[TagTypeDef]]
     enable_termination_protection: Awaitable[bool]
     parent_id: Awaitable[str]
     root_id: Awaitable[str]
-    drift_information: Awaitable[StackDriftInformationResponseMetadataTypeDef]
+    drift_information: Awaitable[StackDriftInformationResponseTypeDef]
     name: str
     events: StackEventsCollection
     resource_summaries: StackResourceSummariesCollection
 
     async def Resource(self, logical_id: str) -> "_StackResource":
         """
         Creates a StackResource resource.
@@ -351,16 +351,16 @@
     physical_resource_id: Awaitable[str]
     resource_type: Awaitable[str]
     last_updated_timestamp: Awaitable[datetime]
     resource_status: Awaitable[ResourceStatusType]
     resource_status_reason: Awaitable[str]
     description: Awaitable[str]
     metadata: Awaitable[str]
-    drift_information: Awaitable[StackResourceDriftInformationResponseMetadataTypeDef]
-    module_info: Awaitable[ModuleInfoResponseMetadataTypeDef]
+    drift_information: Awaitable[StackResourceDriftInformationResponseTypeDef]
+    module_info: Awaitable[ModuleInfoResponseTypeDef]
     stack_name: str
     logical_id: str
 
     async def Stack(self) -> _Stack:
         """
         Creates a Stack resource.
 
@@ -401,16 +401,16 @@
 
     logical_resource_id: Awaitable[str]
     physical_resource_id: Awaitable[str]
     resource_type: Awaitable[str]
     last_updated_timestamp: Awaitable[datetime]
     resource_status: Awaitable[ResourceStatusType]
     resource_status_reason: Awaitable[str]
-    drift_information: Awaitable[StackResourceDriftInformationSummaryResponseMetadataTypeDef]
-    module_info: Awaitable[ModuleInfoResponseMetadataTypeDef]
+    drift_information: Awaitable[StackResourceDriftInformationSummaryResponseTypeDef]
+    module_info: Awaitable[ModuleInfoResponseTypeDef]
     stack_name: str
     logical_id: str
 
     async def Resource(self) -> _StackResource:
         """
         Creates a StackResource resource.
 
@@ -471,15 +471,15 @@
         self,
         *,
         StackName: str,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         DisableRollback: bool = ...,
-        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
         TimeoutInMinutes: int = ...,
         NotificationARNs: Sequence[str] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/type_defs.py` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudformation.type_defs import AccountGateResultTypeDef
 
-    data: AccountGateResultTypeDef = {...}
+    data: AccountGateResultTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountFilterTypeType,
     AccountGateStatusType,
     CallAsType,
     CapabilityType,
     CategoryType,
@@ -74,170 +74,172 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountGateResultTypeDef",
     "AccountLimitTypeDef",
     "LoggingConfigTypeDef",
-    "ActivateTypeOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AutoDeploymentTypeDef",
     "TypeConfigurationIdentifierTypeDef",
     "TypeConfigurationDetailsTypeDef",
     "CancelUpdateStackInputRequestTypeDef",
     "CancelUpdateStackInputStackCancelUpdateTypeDef",
     "ChangeSetHookResourceTargetDetailsTypeDef",
     "ChangeSetSummaryTypeDef",
     "ContinueUpdateRollbackInputRequestTypeDef",
     "ParameterTypeDef",
     "ResourceToImportTypeDef",
     "TagTypeDef",
-    "CreateChangeSetOutputTypeDef",
     "DeploymentTargetsTypeDef",
     "StackSetOperationPreferencesTypeDef",
-    "CreateStackInstancesOutputTypeDef",
-    "CreateStackOutputTypeDef",
     "ManagedExecutionTypeDef",
-    "CreateStackSetOutputTypeDef",
     "DeactivateTypeInputRequestTypeDef",
     "DeleteChangeSetInputRequestTypeDef",
     "DeleteStackInputRequestTypeDef",
     "DeleteStackInputStackDeleteTypeDef",
-    "DeleteStackInstancesOutputTypeDef",
     "DeleteStackSetInputRequestTypeDef",
+    "DeploymentTargetsOutputTypeDef",
     "DeregisterTypeInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "DescribeChangeSetHooksInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
     "DescribeChangeSetInputRequestTypeDef",
     "DescribeOrganizationsAccessInputRequestTypeDef",
-    "DescribeOrganizationsAccessOutputTypeDef",
     "DescribePublisherInputRequestTypeDef",
-    "DescribePublisherOutputTypeDef",
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
     "DescribeStackEventsInputRequestTypeDef",
     "StackEventTypeDef",
     "DescribeStackInstanceInputRequestTypeDef",
     "DescribeStackResourceDriftsInputRequestTypeDef",
     "DescribeStackResourceInputRequestTypeDef",
     "DescribeStackResourcesInputRequestTypeDef",
     "DescribeStackSetInputRequestTypeDef",
     "DescribeStackSetOperationInputRequestTypeDef",
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
     "DescribeStacksInputRequestTypeDef",
     "DescribeTypeInputRequestTypeDef",
     "RequiredActivatedTypeTypeDef",
     "DescribeTypeRegistrationInputRequestTypeDef",
-    "DescribeTypeRegistrationOutputTypeDef",
     "DetectStackDriftInputRequestTypeDef",
-    "DetectStackDriftOutputTypeDef",
     "DetectStackResourceDriftInputRequestTypeDef",
-    "DetectStackSetDriftOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EstimateTemplateCostOutputTypeDef",
     "ExecuteChangeSetInputRequestTypeDef",
     "ExportTypeDef",
     "GetStackPolicyInputRequestTypeDef",
-    "GetStackPolicyOutputTypeDef",
     "GetTemplateInputRequestTypeDef",
-    "GetTemplateOutputTypeDef",
     "GetTemplateSummaryInputRequestTypeDef",
     "ResourceIdentifierSummaryTypeDef",
-    "ImportStacksToStackSetOutputTypeDef",
-    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
     "ListChangeSetsInputRequestTypeDef",
-    "ListExportsInputListExportsPaginateTypeDef",
     "ListExportsInputRequestTypeDef",
-    "ListImportsInputListImportsPaginateTypeDef",
     "ListImportsInputRequestTypeDef",
-    "ListImportsOutputTypeDef",
     "StackInstanceFilterTypeDef",
-    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
     "ListStackResourcesInputRequestTypeDef",
     "OperationResultFilterTypeDef",
-    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
     "ListStackSetOperationsInputRequestTypeDef",
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
     "ListStackSetsInputRequestTypeDef",
-    "ListStacksInputListStacksPaginateTypeDef",
     "ListStacksInputRequestTypeDef",
     "ListTypeRegistrationsInputRequestTypeDef",
-    "ListTypeRegistrationsOutputTypeDef",
     "ListTypeVersionsInputRequestTypeDef",
     "TypeVersionSummaryTypeDef",
     "TypeFiltersTypeDef",
     "TypeSummaryTypeDef",
-    "ModuleInfoResponseMetadataTypeDef",
     "ModuleInfoTypeDef",
     "OutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterConstraintsTypeDef",
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     "PropertyDifferenceTypeDef",
     "PublishTypeInputRequestTypeDef",
-    "PublishTypeOutputTypeDef",
     "RecordHandlerProgressInputRequestTypeDef",
     "RegisterPublisherInputRequestTypeDef",
-    "RegisterPublisherOutputTypeDef",
-    "RegisterTypeOutputTypeDef",
     "ResourceTargetDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
     "RollbackTriggerTypeDef",
     "RollbackStackInputRequestTypeDef",
-    "RollbackStackOutputTypeDef",
     "SetStackPolicyInputRequestTypeDef",
     "SetTypeConfigurationInputRequestTypeDef",
-    "SetTypeConfigurationOutputTypeDef",
     "SetTypeDefaultVersionInputRequestTypeDef",
     "SignalResourceInputRequestTypeDef",
-    "StackDriftInformationResponseMetadataTypeDef",
     "StackDriftInformationSummaryTypeDef",
     "StackDriftInformationTypeDef",
     "StackInstanceComprehensiveStatusTypeDef",
     "StackResourceDriftInformationTypeDef",
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
     "StackResourceDriftInformationSummaryTypeDef",
     "StackSetDriftDetectionDetailsTypeDef",
+    "StackSetOperationPreferencesOutputTypeDef",
     "StackSetOperationStatusDetailsTypeDef",
     "StopStackSetOperationInputRequestTypeDef",
     "TemplateParameterTypeDef",
     "TestTypeInputRequestTypeDef",
-    "TestTypeOutputTypeDef",
-    "UpdateStackInstancesOutputTypeDef",
-    "UpdateStackOutputTypeDef",
-    "UpdateStackSetOutputTypeDef",
     "UpdateTerminationProtectionInputRequestTypeDef",
-    "UpdateTerminationProtectionOutputTypeDef",
     "ValidateTemplateInputRequestTypeDef",
     "StackSetOperationResultSummaryTypeDef",
-    "DescribeAccountLimitsOutputTypeDef",
     "ActivateTypeInputRequestTypeDef",
     "RegisterTypeInputRequestTypeDef",
+    "ActivateTypeOutputTypeDef",
+    "CreateChangeSetOutputTypeDef",
+    "CreateStackInstancesOutputTypeDef",
+    "CreateStackOutputTypeDef",
+    "CreateStackSetOutputTypeDef",
+    "DeleteStackInstancesOutputTypeDef",
+    "DescribeAccountLimitsOutputTypeDef",
+    "DescribeOrganizationsAccessOutputTypeDef",
+    "DescribePublisherOutputTypeDef",
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    "DescribeTypeRegistrationOutputTypeDef",
+    "DetectStackDriftOutputTypeDef",
+    "DetectStackSetDriftOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EstimateTemplateCostOutputTypeDef",
+    "GetStackPolicyOutputTypeDef",
+    "GetTemplateOutputTypeDef",
+    "ImportStacksToStackSetOutputTypeDef",
+    "ListImportsOutputTypeDef",
+    "ListTypeRegistrationsOutputTypeDef",
+    "ModuleInfoResponseTypeDef",
+    "PublishTypeOutputTypeDef",
+    "RegisterPublisherOutputTypeDef",
+    "RegisterTypeOutputTypeDef",
+    "RollbackStackOutputTypeDef",
+    "SetTypeConfigurationOutputTypeDef",
+    "StackDriftInformationResponseTypeDef",
+    "StackResourceDriftInformationResponseTypeDef",
+    "StackResourceDriftInformationSummaryResponseTypeDef",
+    "TestTypeOutputTypeDef",
+    "UpdateStackInstancesOutputTypeDef",
+    "UpdateStackOutputTypeDef",
+    "UpdateStackSetOutputTypeDef",
+    "UpdateTerminationProtectionOutputTypeDef",
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     "ChangeSetHookTargetDetailsTypeDef",
     "ListChangeSetsOutputTypeDef",
     "EstimateTemplateCostInputRequestTypeDef",
     "CreateStackInstancesInputRequestTypeDef",
     "DeleteStackInstancesInputRequestTypeDef",
     "DetectStackSetDriftInputRequestTypeDef",
     "ImportStacksToStackSetInputRequestTypeDef",
     "UpdateStackInstancesInputRequestTypeDef",
     "CreateStackSetInputRequestTypeDef",
     "StackSetSummaryTypeDef",
     "UpdateStackSetInputRequestTypeDef",
+    "DeploymentTargetsUnionTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
+    "ListExportsInputListExportsPaginateTypeDef",
+    "ListImportsInputListImportsPaginateTypeDef",
+    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
+    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    "ListStacksInputListStacksPaginateTypeDef",
     "DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackDeleteCompleteWaitTypeDef",
     "DescribeStacksInputStackExistsWaitTypeDef",
     "DescribeStacksInputStackImportCompleteWaitTypeDef",
     "DescribeStacksInputStackRollbackCompleteWaitTypeDef",
     "DescribeStacksInputStackUpdateCompleteWaitTypeDef",
@@ -252,38 +254,40 @@
     "ListTypeVersionsOutputTypeDef",
     "ListTypesInputListTypesPaginateTypeDef",
     "ListTypesInputRequestTypeDef",
     "ListTypesOutputTypeDef",
     "ParameterDeclarationTypeDef",
     "StackResourceDriftTypeDef",
     "ResourceChangeDetailTypeDef",
-    "RollbackConfigurationResponseMetadataTypeDef",
+    "RollbackConfigurationOutputTypeDef",
     "RollbackConfigurationTypeDef",
     "StackSummaryTypeDef",
     "StackInstanceSummaryTypeDef",
     "StackInstanceTypeDef",
     "StackResourceDetailTypeDef",
     "StackResourceTypeDef",
     "StackResourceSummaryTypeDef",
     "StackSetTypeDef",
+    "StackSetOperationPreferencesUnionTypeDef",
     "StackSetOperationSummaryTypeDef",
     "StackSetOperationTypeDef",
     "ValidateTemplateOutputTypeDef",
     "ListStackSetOperationResultsOutputTypeDef",
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     "ChangeSetHookTypeDef",
     "ListStackSetsOutputTypeDef",
     "GetTemplateSummaryOutputTypeDef",
     "DescribeStackResourceDriftsOutputTypeDef",
     "DetectStackResourceDriftOutputTypeDef",
     "ResourceChangeTypeDef",
+    "StackTypeDef",
     "CreateChangeSetInputRequestTypeDef",
     "CreateStackInputRequestTypeDef",
     "CreateStackInputServiceResourceCreateStackTypeDef",
-    "StackTypeDef",
+    "RollbackConfigurationUnionTypeDef",
     "UpdateStackInputRequestTypeDef",
     "UpdateStackInputStackUpdateTypeDef",
     "ListStacksOutputTypeDef",
     "ListStackInstancesOutputTypeDef",
     "DescribeStackInstanceOutputTypeDef",
     "DescribeStackResourceOutputTypeDef",
     "DescribeStackResourcesOutputTypeDef",
@@ -319,19 +323,22 @@
     "LoggingConfigTypeDef",
     {
         "LogRoleArn": str,
         "LogGroupName": str,
     },
 )
 
-ActivateTypeOutputTypeDef = TypedDict(
-    "ActivateTypeOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AutoDeploymentTypeDef = TypedDict(
     "AutoDeploymentTypeDef",
     {
         "Enabled": bool,
@@ -376,21 +383,19 @@
     "_OptionalCancelUpdateStackInputRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class CancelUpdateStackInputRequestTypeDef(
     _RequiredCancelUpdateStackInputRequestTypeDef, _OptionalCancelUpdateStackInputRequestTypeDef
 ):
     pass
 
-
 CancelUpdateStackInputStackCancelUpdateTypeDef = TypedDict(
     "CancelUpdateStackInputStackCancelUpdateTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
@@ -436,22 +441,20 @@
         "RoleARN": str,
         "ResourcesToSkip": Sequence[str],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class ContinueUpdateRollbackInputRequestTypeDef(
     _RequiredContinueUpdateRollbackInputRequestTypeDef,
     _OptionalContinueUpdateRollbackInputRequestTypeDef,
 ):
     pass
 
-
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "ParameterKey": str,
         "ParameterValue": str,
         "UsePreviousValue": bool,
         "ResolvedValue": str,
@@ -472,23 +475,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateChangeSetOutputTypeDef = TypedDict(
-    "CreateChangeSetOutputTypeDef",
-    {
-        "Id": str,
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentTargetsTypeDef = TypedDict(
     "DeploymentTargetsTypeDef",
     {
         "Accounts": Sequence[str],
         "AccountsUrl": str,
         "OrganizationalUnitIds": Sequence[str],
         "AccountFilterType": AccountFilterTypeType,
@@ -505,46 +499,22 @@
         "FailureTolerancePercentage": int,
         "MaxConcurrentCount": int,
         "MaxConcurrentPercentage": int,
     },
     total=False,
 )
 
-CreateStackInstancesOutputTypeDef = TypedDict(
-    "CreateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStackOutputTypeDef = TypedDict(
-    "CreateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ManagedExecutionTypeDef = TypedDict(
     "ManagedExecutionTypeDef",
     {
         "Active": bool,
     },
     total=False,
 )
 
-CreateStackSetOutputTypeDef = TypedDict(
-    "CreateStackSetOutputTypeDef",
-    {
-        "StackSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeactivateTypeInputRequestTypeDef = TypedDict(
     "DeactivateTypeInputRequestTypeDef",
     {
         "TypeName": str,
         "Type": ThirdPartyTypeType,
         "Arn": str,
     },
@@ -561,21 +531,19 @@
     "_OptionalDeleteChangeSetInputRequestTypeDef",
     {
         "StackName": str,
     },
     total=False,
 )
 
-
 class DeleteChangeSetInputRequestTypeDef(
     _RequiredDeleteChangeSetInputRequestTypeDef, _OptionalDeleteChangeSetInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteStackInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStackInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalDeleteStackInputRequestTypeDef = TypedDict(
@@ -584,75 +552,76 @@
         "RetainResources": Sequence[str],
         "RoleARN": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteStackInputRequestTypeDef(
     _RequiredDeleteStackInputRequestTypeDef, _OptionalDeleteStackInputRequestTypeDef
 ):
     pass
 
-
 DeleteStackInputStackDeleteTypeDef = TypedDict(
     "DeleteStackInputStackDeleteTypeDef",
     {
         "RetainResources": Sequence[str],
         "RoleARN": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-DeleteStackInstancesOutputTypeDef = TypedDict(
-    "DeleteStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteStackSetInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalDeleteStackSetInputRequestTypeDef = TypedDict(
     "_OptionalDeleteStackSetInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-
 class DeleteStackSetInputRequestTypeDef(
     _RequiredDeleteStackSetInputRequestTypeDef, _OptionalDeleteStackSetInputRequestTypeDef
 ):
     pass
 
+DeploymentTargetsOutputTypeDef = TypedDict(
+    "DeploymentTargetsOutputTypeDef",
+    {
+        "Accounts": List[str],
+        "AccountsUrl": str,
+        "OrganizationalUnitIds": List[str],
+        "AccountFilterType": AccountFilterTypeType,
+    },
+    total=False,
+)
 
 DeregisterTypeInputRequestTypeDef = TypedDict(
     "DeregisterTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
     },
     total=False,
 )
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
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
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -673,54 +642,29 @@
         "StackName": str,
         "NextToken": str,
         "LogicalResourceId": str,
     },
     total=False,
 )
 
-
 class DescribeChangeSetHooksInputRequestTypeDef(
     _RequiredDescribeChangeSetHooksInputRequestTypeDef,
     _OptionalDescribeChangeSetHooksInputRequestTypeDef,
 ):
     pass
 
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "ChangeSetName": str,
-    },
-)
-_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
-    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputRequestTypeDef = TypedDict(
@@ -728,86 +672,42 @@
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeChangeSetInputRequestTypeDef(
     _RequiredDescribeChangeSetInputRequestTypeDef, _OptionalDescribeChangeSetInputRequestTypeDef
 ):
     pass
 
-
 DescribeOrganizationsAccessInputRequestTypeDef = TypedDict(
     "DescribeOrganizationsAccessInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-DescribeOrganizationsAccessOutputTypeDef = TypedDict(
-    "DescribeOrganizationsAccessOutputTypeDef",
-    {
-        "Status": OrganizationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribePublisherInputRequestTypeDef = TypedDict(
     "DescribePublisherInputRequestTypeDef",
     {
         "PublisherId": str,
     },
     total=False,
 )
 
-DescribePublisherOutputTypeDef = TypedDict(
-    "DescribePublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "PublisherStatus": PublisherStatusType,
-        "IdentityProvider": IdentityProviderType,
-        "PublisherProfile": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeStackDriftDetectionStatusInputRequestTypeDef = TypedDict(
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
     {
         "StackDriftDetectionId": str,
     },
 )
 
-DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    {
-        "StackId": str,
-        "StackDriftDetectionId": str,
-        "StackDriftStatus": StackDriftStatusType,
-        "DetectionStatus": StackDriftDetectionStatusType,
-        "DetectionStatusReason": str,
-        "DriftedStackResourceCount": int,
-        "Timestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStackEventsInputRequestTypeDef = TypedDict(
     "DescribeStackEventsInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
@@ -837,19 +737,17 @@
         "HookStatusReason": str,
         "HookInvocationPoint": Literal["PRE_PROVISION"],
         "HookFailureMode": HookFailureModeType,
     },
     total=False,
 )
 
-
 class StackEventTypeDef(_RequiredStackEventTypeDef, _OptionalStackEventTypeDef):
     pass
 
-
 _RequiredDescribeStackInstanceInputRequestTypeDef = TypedDict(
     "_RequiredDescribeStackInstanceInputRequestTypeDef",
     {
         "StackSetName": str,
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
     },
@@ -858,22 +756,20 @@
     "_OptionalDescribeStackInstanceInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-
 class DescribeStackInstanceInputRequestTypeDef(
     _RequiredDescribeStackInstanceInputRequestTypeDef,
     _OptionalDescribeStackInstanceInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeStackResourceDriftsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeStackResourceDriftsInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalDescribeStackResourceDriftsInputRequestTypeDef = TypedDict(
@@ -882,22 +778,20 @@
         "StackResourceDriftStatusFilters": Sequence[StackResourceDriftStatusType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeStackResourceDriftsInputRequestTypeDef(
     _RequiredDescribeStackResourceDriftsInputRequestTypeDef,
     _OptionalDescribeStackResourceDriftsInputRequestTypeDef,
 ):
     pass
 
-
 DescribeStackResourceInputRequestTypeDef = TypedDict(
     "DescribeStackResourceInputRequestTypeDef",
     {
         "StackName": str,
         "LogicalResourceId": str,
     },
 )
@@ -922,21 +816,19 @@
     "_OptionalDescribeStackSetInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-
 class DescribeStackSetInputRequestTypeDef(
     _RequiredDescribeStackSetInputRequestTypeDef, _OptionalDescribeStackSetInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeStackSetOperationInputRequestTypeDef = TypedDict(
     "_RequiredDescribeStackSetOperationInputRequestTypeDef",
     {
         "StackSetName": str,
         "OperationId": str,
     },
 )
@@ -944,31 +836,20 @@
     "_OptionalDescribeStackSetOperationInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-
 class DescribeStackSetOperationInputRequestTypeDef(
     _RequiredDescribeStackSetOperationInputRequestTypeDef,
     _OptionalDescribeStackSetOperationInputRequestTypeDef,
 ):
     pass
 
-
-DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStacksInputRequestTypeDef = TypedDict(
     "DescribeStacksInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
@@ -1001,85 +882,41 @@
 DescribeTypeRegistrationInputRequestTypeDef = TypedDict(
     "DescribeTypeRegistrationInputRequestTypeDef",
     {
         "RegistrationToken": str,
     },
 )
 
-DescribeTypeRegistrationOutputTypeDef = TypedDict(
-    "DescribeTypeRegistrationOutputTypeDef",
-    {
-        "ProgressStatus": RegistrationStatusType,
-        "Description": str,
-        "TypeArn": str,
-        "TypeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDetectStackDriftInputRequestTypeDef = TypedDict(
     "_RequiredDetectStackDriftInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalDetectStackDriftInputRequestTypeDef = TypedDict(
     "_OptionalDetectStackDriftInputRequestTypeDef",
     {
         "LogicalResourceIds": Sequence[str],
     },
     total=False,
 )
 
-
 class DetectStackDriftInputRequestTypeDef(
     _RequiredDetectStackDriftInputRequestTypeDef, _OptionalDetectStackDriftInputRequestTypeDef
 ):
     pass
 
-
-DetectStackDriftOutputTypeDef = TypedDict(
-    "DetectStackDriftOutputTypeDef",
-    {
-        "StackDriftDetectionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DetectStackResourceDriftInputRequestTypeDef = TypedDict(
     "DetectStackResourceDriftInputRequestTypeDef",
     {
         "StackName": str,
         "LogicalResourceId": str,
     },
 )
 
-DetectStackSetDriftOutputTypeDef = TypedDict(
-    "DetectStackSetDriftOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EstimateTemplateCostOutputTypeDef = TypedDict(
-    "EstimateTemplateCostOutputTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExecuteChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredExecuteChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalExecuteChangeSetInputRequestTypeDef = TypedDict(
@@ -1088,21 +925,19 @@
         "StackName": str,
         "ClientRequestToken": str,
         "DisableRollback": bool,
     },
     total=False,
 )
 
-
 class ExecuteChangeSetInputRequestTypeDef(
     _RequiredExecuteChangeSetInputRequestTypeDef, _OptionalExecuteChangeSetInputRequestTypeDef
 ):
     pass
 
-
 ExportTypeDef = TypedDict(
     "ExportTypeDef",
     {
         "ExportingStackId": str,
         "Name": str,
         "Value": str,
     },
@@ -1112,41 +947,24 @@
 GetStackPolicyInputRequestTypeDef = TypedDict(
     "GetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 
-GetStackPolicyOutputTypeDef = TypedDict(
-    "GetStackPolicyOutputTypeDef",
-    {
-        "StackPolicyBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTemplateInputRequestTypeDef = TypedDict(
     "GetTemplateInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
         "TemplateStage": TemplateStageType,
     },
     total=False,
 )
 
-GetTemplateOutputTypeDef = TypedDict(
-    "GetTemplateOutputTypeDef",
-    {
-        "TemplateBody": Dict[str, Any],
-        "StagesAvailable": List[TemplateStageType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTemplateSummaryInputRequestTypeDef = TypedDict(
     "GetTemplateSummaryInputRequestTypeDef",
     {
         "TemplateBody": str,
         "TemplateURL": str,
         "StackName": str,
         "StackSetName": str,
@@ -1161,217 +979,97 @@
         "ResourceType": str,
         "LogicalResourceIds": List[str],
         "ResourceIdentifiers": List[str],
     },
     total=False,
 )
 
-ImportStacksToStackSetOutputTypeDef = TypedDict(
-    "ImportStacksToStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListChangeSetsInputListChangeSetsPaginateTypeDef(
-    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
-    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListChangeSetsInputRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListChangeSetsInputRequestTypeDef = TypedDict(
     "_OptionalListChangeSetsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChangeSetsInputRequestTypeDef(
     _RequiredListChangeSetsInputRequestTypeDef, _OptionalListChangeSetsInputRequestTypeDef
 ):
     pass
 
-
-ListExportsInputListExportsPaginateTypeDef = TypedDict(
-    "ListExportsInputListExportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExportsInputRequestTypeDef = TypedDict(
     "ListExportsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_RequiredListImportsInputListImportsPaginateTypeDef",
-    {
-        "ExportName": str,
-    },
-)
-_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_OptionalListImportsInputListImportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListImportsInputListImportsPaginateTypeDef(
-    _RequiredListImportsInputListImportsPaginateTypeDef,
-    _OptionalListImportsInputListImportsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListImportsInputRequestTypeDef = TypedDict(
     "_RequiredListImportsInputRequestTypeDef",
     {
         "ExportName": str,
     },
 )
 _OptionalListImportsInputRequestTypeDef = TypedDict(
     "_OptionalListImportsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListImportsInputRequestTypeDef(
     _RequiredListImportsInputRequestTypeDef, _OptionalListImportsInputRequestTypeDef
 ):
     pass
 
-
-ListImportsOutputTypeDef = TypedDict(
-    "ListImportsOutputTypeDef",
-    {
-        "Imports": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StackInstanceFilterTypeDef = TypedDict(
     "StackInstanceFilterTypeDef",
     {
         "Name": StackInstanceFilterNameType,
         "Values": str,
     },
     total=False,
 )
 
-_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStackResourcesInputListStackResourcesPaginateTypeDef(
-    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
-    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStackResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListStackResourcesInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListStackResourcesInputRequestTypeDef = TypedDict(
     "_OptionalListStackResourcesInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListStackResourcesInputRequestTypeDef(
     _RequiredListStackResourcesInputRequestTypeDef, _OptionalListStackResourcesInputRequestTypeDef
 ):
     pass
 
-
 OperationResultFilterTypeDef = TypedDict(
     "OperationResultFilterTypeDef",
     {
         "Name": Literal["OPERATION_RESULT_STATUS"],
         "Values": str,
     },
     total=False,
 )
 
-_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "StackSetName": str,
-    },
-)
-_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
-    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStackSetOperationsInputRequestTypeDef = TypedDict(
     "_RequiredListStackSetOperationsInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackSetOperationsInputRequestTypeDef = TypedDict(
@@ -1380,52 +1078,31 @@
         "NextToken": str,
         "MaxResults": int,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-
 class ListStackSetOperationsInputRequestTypeDef(
     _RequiredListStackSetOperationsInputRequestTypeDef,
     _OptionalListStackSetOperationsInputRequestTypeDef,
 ):
     pass
 
-
-ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
-    {
-        "Status": StackSetStatusType,
-        "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStackSetsInputRequestTypeDef = TypedDict(
     "ListStackSetsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Status": StackSetStatusType,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-ListStacksInputListStacksPaginateTypeDef = TypedDict(
-    "ListStacksInputListStacksPaginateTypeDef",
-    {
-        "StackStatusFilter": Sequence[StackStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStacksInputRequestTypeDef = TypedDict(
     "ListStacksInputRequestTypeDef",
     {
         "NextToken": str,
         "StackStatusFilter": Sequence[StackStatusType],
     },
     total=False,
@@ -1440,23 +1117,14 @@
         "RegistrationStatusFilter": RegistrationStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTypeRegistrationsOutputTypeDef = TypedDict(
-    "ListTypeRegistrationsOutputTypeDef",
-    {
-        "RegistrationTokenList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTypeVersionsInputRequestTypeDef = TypedDict(
     "ListTypeVersionsInputRequestTypeDef",
     {
         "Type": RegistryTypeType,
         "TypeName": str,
         "Arn": str,
         "MaxResults": int,
@@ -1508,23 +1176,14 @@
         "PublisherIdentity": IdentityProviderType,
         "PublisherName": str,
         "IsActivated": bool,
     },
     total=False,
 )
 
-ModuleInfoResponseMetadataTypeDef = TypedDict(
-    "ModuleInfoResponseMetadataTypeDef",
-    {
-        "TypeHierarchy": str,
-        "LogicalIdHierarchy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ModuleInfoTypeDef = TypedDict(
     "ModuleInfoTypeDef",
     {
         "TypeHierarchy": str,
         "LogicalIdHierarchy": str,
     },
     total=False,
@@ -1537,24 +1196,14 @@
         "OutputValue": str,
         "Description": str,
         "ExportName": str,
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
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
     },
     total=False,
 )
@@ -1584,22 +1233,14 @@
         "Arn": str,
         "TypeName": str,
         "PublicVersionNumber": str,
     },
     total=False,
 )
 
-PublishTypeOutputTypeDef = TypedDict(
-    "PublishTypeOutputTypeDef",
-    {
-        "PublicTypeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecordHandlerProgressInputRequestTypeDef = TypedDict(
     "_RequiredRecordHandlerProgressInputRequestTypeDef",
     {
         "BearerToken": str,
         "OperationStatus": OperationStatusType,
     },
 )
@@ -1611,68 +1252,39 @@
         "ErrorCode": HandlerErrorCodeType,
         "ResourceModel": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class RecordHandlerProgressInputRequestTypeDef(
     _RequiredRecordHandlerProgressInputRequestTypeDef,
     _OptionalRecordHandlerProgressInputRequestTypeDef,
 ):
     pass
 
-
 RegisterPublisherInputRequestTypeDef = TypedDict(
     "RegisterPublisherInputRequestTypeDef",
     {
         "AcceptTermsAndConditions": bool,
         "ConnectionArn": str,
     },
     total=False,
 )
 
-RegisterPublisherOutputTypeDef = TypedDict(
-    "RegisterPublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTypeOutputTypeDef = TypedDict(
-    "RegisterTypeOutputTypeDef",
-    {
-        "RegistrationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceTargetDefinitionTypeDef = TypedDict(
     "ResourceTargetDefinitionTypeDef",
     {
         "Attribute": ResourceAttributeType,
         "Name": str,
         "RequiresRecreation": RequiresRecreationType,
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
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
         "Type": str,
     },
 )
@@ -1688,29 +1300,19 @@
     {
         "RoleARN": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class RollbackStackInputRequestTypeDef(
     _RequiredRollbackStackInputRequestTypeDef, _OptionalRollbackStackInputRequestTypeDef
 ):
     pass
 
-
-RollbackStackOutputTypeDef = TypedDict(
-    "RollbackStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSetStackPolicyInputRequestTypeDef = TypedDict(
     "_RequiredSetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalSetStackPolicyInputRequestTypeDef = TypedDict(
@@ -1718,21 +1320,19 @@
     {
         "StackPolicyBody": str,
         "StackPolicyURL": str,
     },
     total=False,
 )
 
-
 class SetStackPolicyInputRequestTypeDef(
     _RequiredSetStackPolicyInputRequestTypeDef, _OptionalSetStackPolicyInputRequestTypeDef
 ):
     pass
 
-
 _RequiredSetTypeConfigurationInputRequestTypeDef = TypedDict(
     "_RequiredSetTypeConfigurationInputRequestTypeDef",
     {
         "Configuration": str,
     },
 )
 _OptionalSetTypeConfigurationInputRequestTypeDef = TypedDict(
@@ -1742,30 +1342,20 @@
         "ConfigurationAlias": str,
         "TypeName": str,
         "Type": ThirdPartyTypeType,
     },
     total=False,
 )
 
-
 class SetTypeConfigurationInputRequestTypeDef(
     _RequiredSetTypeConfigurationInputRequestTypeDef,
     _OptionalSetTypeConfigurationInputRequestTypeDef,
 ):
     pass
 
-
-SetTypeConfigurationOutputTypeDef = TypedDict(
-    "SetTypeConfigurationOutputTypeDef",
-    {
-        "ConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetTypeDefaultVersionInputRequestTypeDef = TypedDict(
     "SetTypeDefaultVersionInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
@@ -1779,65 +1369,52 @@
         "StackName": str,
         "LogicalResourceId": str,
         "UniqueId": str,
         "Status": ResourceSignalStatusType,
     },
 )
 
-StackDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackDriftInformationResponseMetadataTypeDef",
-    {
-        "StackDriftStatus": StackDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStackDriftInformationSummaryTypeDef = TypedDict(
     "_RequiredStackDriftInformationSummaryTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
     },
 )
 _OptionalStackDriftInformationSummaryTypeDef = TypedDict(
     "_OptionalStackDriftInformationSummaryTypeDef",
     {
         "LastCheckTimestamp": datetime,
     },
     total=False,
 )
 
-
 class StackDriftInformationSummaryTypeDef(
     _RequiredStackDriftInformationSummaryTypeDef, _OptionalStackDriftInformationSummaryTypeDef
 ):
     pass
 
-
 _RequiredStackDriftInformationTypeDef = TypedDict(
     "_RequiredStackDriftInformationTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
     },
 )
 _OptionalStackDriftInformationTypeDef = TypedDict(
     "_OptionalStackDriftInformationTypeDef",
     {
         "LastCheckTimestamp": datetime,
     },
     total=False,
 )
 
-
 class StackDriftInformationTypeDef(
     _RequiredStackDriftInformationTypeDef, _OptionalStackDriftInformationTypeDef
 ):
     pass
 
-
 StackInstanceComprehensiveStatusTypeDef = TypedDict(
     "StackInstanceComprehensiveStatusTypeDef",
     {
         "DetailedStatus": StackInstanceDetailedStatusType,
     },
     total=False,
 )
@@ -1852,61 +1429,39 @@
     "_OptionalStackResourceDriftInformationTypeDef",
     {
         "LastCheckTimestamp": datetime,
     },
     total=False,
 )
 
-
 class StackResourceDriftInformationTypeDef(
     _RequiredStackResourceDriftInformationTypeDef, _OptionalStackResourceDriftInformationTypeDef
 ):
     pass
 
-
-StackResourceDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StackResourceDriftInformationSummaryResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStackResourceDriftInformationSummaryTypeDef = TypedDict(
     "_RequiredStackResourceDriftInformationSummaryTypeDef",
     {
         "StackResourceDriftStatus": StackResourceDriftStatusType,
     },
 )
 _OptionalStackResourceDriftInformationSummaryTypeDef = TypedDict(
     "_OptionalStackResourceDriftInformationSummaryTypeDef",
     {
         "LastCheckTimestamp": datetime,
     },
     total=False,
 )
 
-
 class StackResourceDriftInformationSummaryTypeDef(
     _RequiredStackResourceDriftInformationSummaryTypeDef,
     _OptionalStackResourceDriftInformationSummaryTypeDef,
 ):
     pass
 
-
 StackSetDriftDetectionDetailsTypeDef = TypedDict(
     "StackSetDriftDetectionDetailsTypeDef",
     {
         "DriftStatus": StackSetDriftStatusType,
         "DriftDetectionStatus": StackSetDriftDetectionStatusType,
         "LastDriftCheckTimestamp": datetime,
         "TotalStackInstancesCount": int,
@@ -1914,14 +1469,27 @@
         "InSyncStackInstancesCount": int,
         "InProgressStackInstancesCount": int,
         "FailedStackInstancesCount": int,
     },
     total=False,
 )
 
+StackSetOperationPreferencesOutputTypeDef = TypedDict(
+    "StackSetOperationPreferencesOutputTypeDef",
+    {
+        "RegionConcurrencyType": RegionConcurrencyTypeType,
+        "RegionOrder": List[str],
+        "FailureToleranceCount": int,
+        "FailureTolerancePercentage": int,
+        "MaxConcurrentCount": int,
+        "MaxConcurrentPercentage": int,
+    },
+    total=False,
+)
+
 StackSetOperationStatusDetailsTypeDef = TypedDict(
     "StackSetOperationStatusDetailsTypeDef",
     {
         "FailedStackInstancesCount": int,
     },
     total=False,
 )
@@ -1937,22 +1505,20 @@
     "_OptionalStopStackSetOperationInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-
 class StopStackSetOperationInputRequestTypeDef(
     _RequiredStopStackSetOperationInputRequestTypeDef,
     _OptionalStopStackSetOperationInputRequestTypeDef,
 ):
     pass
 
-
 TemplateParameterTypeDef = TypedDict(
     "TemplateParameterTypeDef",
     {
         "ParameterKey": str,
         "DefaultValue": str,
         "NoEcho": bool,
         "Description": str,
@@ -1968,62 +1534,22 @@
         "TypeName": str,
         "VersionId": str,
         "LogDeliveryBucket": str,
     },
     total=False,
 )
 
-TestTypeOutputTypeDef = TypedDict(
-    "TestTypeOutputTypeDef",
-    {
-        "TypeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackInstancesOutputTypeDef = TypedDict(
-    "UpdateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackOutputTypeDef = TypedDict(
-    "UpdateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackSetOutputTypeDef = TypedDict(
-    "UpdateStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateTerminationProtectionInputRequestTypeDef = TypedDict(
     "UpdateTerminationProtectionInputRequestTypeDef",
     {
         "EnableTerminationProtection": bool,
         "StackName": str,
     },
 )
 
-UpdateTerminationProtectionOutputTypeDef = TypedDict(
-    "UpdateTerminationProtectionOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ValidateTemplateInputRequestTypeDef = TypedDict(
     "ValidateTemplateInputRequestTypeDef",
     {
         "TemplateBody": str,
         "TemplateURL": str,
     },
     total=False,
@@ -2038,23 +1564,14 @@
         "StatusReason": str,
         "AccountGateResult": AccountGateResultTypeDef,
         "OrganizationalUnitId": str,
     },
     total=False,
 )
 
-DescribeAccountLimitsOutputTypeDef = TypedDict(
-    "DescribeAccountLimitsOutputTypeDef",
-    {
-        "AccountLimits": List[AccountLimitTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActivateTypeInputRequestTypeDef = TypedDict(
     "ActivateTypeInputRequestTypeDef",
     {
         "Type": ThirdPartyTypeType,
         "PublicTypeArn": str,
         "PublisherId": str,
         "TypeName": str,
@@ -2082,20 +1599,310 @@
         "LoggingConfig": LoggingConfigTypeDef,
         "ExecutionRoleArn": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class RegisterTypeInputRequestTypeDef(
     _RequiredRegisterTypeInputRequestTypeDef, _OptionalRegisterTypeInputRequestTypeDef
 ):
     pass
 
+ActivateTypeOutputTypeDef = TypedDict(
+    "ActivateTypeOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChangeSetOutputTypeDef = TypedDict(
+    "CreateChangeSetOutputTypeDef",
+    {
+        "Id": str,
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackInstancesOutputTypeDef = TypedDict(
+    "CreateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackOutputTypeDef = TypedDict(
+    "CreateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackSetOutputTypeDef = TypedDict(
+    "CreateStackSetOutputTypeDef",
+    {
+        "StackSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteStackInstancesOutputTypeDef = TypedDict(
+    "DeleteStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountLimitsOutputTypeDef = TypedDict(
+    "DescribeAccountLimitsOutputTypeDef",
+    {
+        "AccountLimits": List[AccountLimitTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationsAccessOutputTypeDef = TypedDict(
+    "DescribeOrganizationsAccessOutputTypeDef",
+    {
+        "Status": OrganizationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePublisherOutputTypeDef = TypedDict(
+    "DescribePublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "PublisherStatus": PublisherStatusType,
+        "IdentityProvider": IdentityProviderType,
+        "PublisherProfile": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    {
+        "StackId": str,
+        "StackDriftDetectionId": str,
+        "StackDriftStatus": StackDriftStatusType,
+        "DetectionStatus": StackDriftDetectionStatusType,
+        "DetectionStatusReason": str,
+        "DriftedStackResourceCount": int,
+        "Timestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTypeRegistrationOutputTypeDef = TypedDict(
+    "DescribeTypeRegistrationOutputTypeDef",
+    {
+        "ProgressStatus": RegistrationStatusType,
+        "Description": str,
+        "TypeArn": str,
+        "TypeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectStackDriftOutputTypeDef = TypedDict(
+    "DetectStackDriftOutputTypeDef",
+    {
+        "StackDriftDetectionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectStackSetDriftOutputTypeDef = TypedDict(
+    "DetectStackSetDriftOutputTypeDef",
+    {
+        "OperationId": str,
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
+EstimateTemplateCostOutputTypeDef = TypedDict(
+    "EstimateTemplateCostOutputTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetStackPolicyOutputTypeDef = TypedDict(
+    "GetStackPolicyOutputTypeDef",
+    {
+        "StackPolicyBody": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemplateOutputTypeDef = TypedDict(
+    "GetTemplateOutputTypeDef",
+    {
+        "TemplateBody": Dict[str, Any],
+        "StagesAvailable": List["TemplateStageType"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportStacksToStackSetOutputTypeDef = TypedDict(
+    "ImportStacksToStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListImportsOutputTypeDef = TypedDict(
+    "ListImportsOutputTypeDef",
+    {
+        "Imports": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTypeRegistrationsOutputTypeDef = TypedDict(
+    "ListTypeRegistrationsOutputTypeDef",
+    {
+        "RegistrationTokenList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModuleInfoResponseTypeDef = TypedDict(
+    "ModuleInfoResponseTypeDef",
+    {
+        "TypeHierarchy": str,
+        "LogicalIdHierarchy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishTypeOutputTypeDef = TypedDict(
+    "PublishTypeOutputTypeDef",
+    {
+        "PublicTypeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterPublisherOutputTypeDef = TypedDict(
+    "RegisterPublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterTypeOutputTypeDef = TypedDict(
+    "RegisterTypeOutputTypeDef",
+    {
+        "RegistrationToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackStackOutputTypeDef = TypedDict(
+    "RollbackStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetTypeConfigurationOutputTypeDef = TypedDict(
+    "SetTypeConfigurationOutputTypeDef",
+    {
+        "ConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackDriftInformationResponseTypeDef = TypedDict(
+    "StackDriftInformationResponseTypeDef",
+    {
+        "StackDriftStatus": StackDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackResourceDriftInformationResponseTypeDef = TypedDict(
+    "StackResourceDriftInformationResponseTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackResourceDriftInformationSummaryResponseTypeDef = TypedDict(
+    "StackResourceDriftInformationSummaryResponseTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestTypeOutputTypeDef = TypedDict(
+    "TestTypeOutputTypeDef",
+    {
+        "TypeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackInstancesOutputTypeDef = TypedDict(
+    "UpdateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackOutputTypeDef = TypedDict(
+    "UpdateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackSetOutputTypeDef = TypedDict(
+    "UpdateStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTerminationProtectionOutputTypeDef = TypedDict(
+    "UpdateTerminationProtectionOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 BatchDescribeTypeConfigurationsErrorTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "TypeConfigurationIdentifier": TypeConfigurationIdentifierTypeDef,
@@ -2120,15 +1927,15 @@
 )
 
 ListChangeSetsOutputTypeDef = TypedDict(
     "ListChangeSetsOutputTypeDef",
     {
         "Summaries": List[ChangeSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EstimateTemplateCostInputRequestTypeDef = TypedDict(
     "EstimateTemplateCostInputRequestTypeDef",
     {
         "TemplateBody": str,
@@ -2154,22 +1961,20 @@
         "OperationPreferences": StackSetOperationPreferencesTypeDef,
         "OperationId": str,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-
 class CreateStackInstancesInputRequestTypeDef(
     _RequiredCreateStackInstancesInputRequestTypeDef,
     _OptionalCreateStackInstancesInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStackInstancesInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStackInstancesInputRequestTypeDef",
     {
         "StackSetName": str,
         "Regions": Sequence[str],
         "RetainStacks": bool,
     },
@@ -2182,22 +1987,20 @@
         "OperationPreferences": StackSetOperationPreferencesTypeDef,
         "OperationId": str,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-
 class DeleteStackInstancesInputRequestTypeDef(
     _RequiredDeleteStackInstancesInputRequestTypeDef,
     _OptionalDeleteStackInstancesInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDetectStackSetDriftInputRequestTypeDef = TypedDict(
     "_RequiredDetectStackSetDriftInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalDetectStackSetDriftInputRequestTypeDef = TypedDict(
@@ -2206,21 +2009,19 @@
         "OperationPreferences": StackSetOperationPreferencesTypeDef,
         "OperationId": str,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-
 class DetectStackSetDriftInputRequestTypeDef(
     _RequiredDetectStackSetDriftInputRequestTypeDef, _OptionalDetectStackSetDriftInputRequestTypeDef
 ):
     pass
 
-
 _RequiredImportStacksToStackSetInputRequestTypeDef = TypedDict(
     "_RequiredImportStacksToStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalImportStacksToStackSetInputRequestTypeDef = TypedDict(
@@ -2232,22 +2033,20 @@
         "OperationPreferences": StackSetOperationPreferencesTypeDef,
         "OperationId": str,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-
 class ImportStacksToStackSetInputRequestTypeDef(
     _RequiredImportStacksToStackSetInputRequestTypeDef,
     _OptionalImportStacksToStackSetInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateStackInstancesInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStackInstancesInputRequestTypeDef",
     {
         "StackSetName": str,
         "Regions": Sequence[str],
     },
 )
@@ -2260,22 +2059,20 @@
         "OperationPreferences": StackSetOperationPreferencesTypeDef,
         "OperationId": str,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-
 class UpdateStackInstancesInputRequestTypeDef(
     _RequiredUpdateStackInstancesInputRequestTypeDef,
     _OptionalUpdateStackInstancesInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateStackSetInputRequestTypeDef = TypedDict(
     "_RequiredCreateStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalCreateStackSetInputRequestTypeDef = TypedDict(
@@ -2295,21 +2092,19 @@
         "CallAs": CallAsType,
         "ClientRequestToken": str,
         "ManagedExecution": ManagedExecutionTypeDef,
     },
     total=False,
 )
 
-
 class CreateStackSetInputRequestTypeDef(
     _RequiredCreateStackSetInputRequestTypeDef, _OptionalCreateStackSetInputRequestTypeDef
 ):
     pass
 
-
 StackSetSummaryTypeDef = TypedDict(
     "StackSetSummaryTypeDef",
     {
         "StackSetName": str,
         "StackSetId": str,
         "Description": str,
         "Status": StackSetStatusType,
@@ -2349,20 +2144,174 @@
         "Regions": Sequence[str],
         "CallAs": CallAsType,
         "ManagedExecution": ManagedExecutionTypeDef,
     },
     total=False,
 )
 
-
 class UpdateStackSetInputRequestTypeDef(
     _RequiredUpdateStackSetInputRequestTypeDef, _OptionalUpdateStackSetInputRequestTypeDef
 ):
     pass
 
+DeploymentTargetsUnionTypeDef = Union[DeploymentTargetsTypeDef, DeploymentTargetsOutputTypeDef]
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "ChangeSetName": str,
+    },
+)
+_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
+    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+):
+    pass
+
+DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListChangeSetsInputListChangeSetsPaginateTypeDef(
+    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
+    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
+):
+    pass
+
+ListExportsInputListExportsPaginateTypeDef = TypedDict(
+    "ListExportsInputListExportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_RequiredListImportsInputListImportsPaginateTypeDef",
+    {
+        "ExportName": str,
+    },
+)
+_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_OptionalListImportsInputListImportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListImportsInputListImportsPaginateTypeDef(
+    _RequiredListImportsInputListImportsPaginateTypeDef,
+    _OptionalListImportsInputListImportsPaginateTypeDef,
+):
+    pass
+
+_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStackResourcesInputListStackResourcesPaginateTypeDef(
+    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
+    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "StackSetName": str,
+    },
+)
+_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "CallAs": CallAsType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
+    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+):
+    pass
+
+ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    {
+        "Status": StackSetStatusType,
+        "CallAs": CallAsType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListStacksInputListStacksPaginateTypeDef = TypedDict(
+    "ListStacksInputListStacksPaginateTypeDef",
+    {
+        "StackStatusFilter": Sequence[StackStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 _RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     {
         "ChangeSetName": str,
     },
 )
@@ -2372,22 +2321,20 @@
         "StackName": str,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef(
     _RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     _OptionalDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
 ):
     pass
 
-
 DescribeStacksInputStackCreateCompleteWaitTypeDef = TypedDict(
     "DescribeStacksInputStackCreateCompleteWaitTypeDef",
     {
         "StackName": str,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
@@ -2454,28 +2401,26 @@
     "_OptionalDescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef(
     _RequiredDescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef,
     _OptionalDescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef,
 ):
     pass
 
-
 DescribeStackEventsOutputTypeDef = TypedDict(
     "DescribeStackEventsOutputTypeDef",
     {
         "StackEvents": List[StackEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTypeOutputTypeDef = TypedDict(
     "DescribeTypeOutputTypeDef",
     {
         "Arn": str,
@@ -2501,24 +2446,24 @@
         "PublisherId": str,
         "OriginalTypeName": str,
         "OriginalTypeArn": str,
         "PublicVersionNumber": str,
         "LatestPublicVersion": str,
         "IsActivated": bool,
         "AutoUpdate": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "Exports": List[ExportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_RequiredListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "StackSetName": str,
@@ -2527,27 +2472,25 @@
 _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_OptionalListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "Filters": Sequence[StackInstanceFilterTypeDef],
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListStackInstancesInputListStackInstancesPaginateTypeDef(
     _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef,
     _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListStackInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListStackInstancesInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackInstancesInputRequestTypeDef = TypedDict(
@@ -2559,46 +2502,42 @@
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-
 class ListStackInstancesInputRequestTypeDef(
     _RequiredListStackInstancesInputRequestTypeDef, _OptionalListStackInstancesInputRequestTypeDef
 ):
     pass
 
-
 _RequiredListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef = TypedDict(
     "_RequiredListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     {
         "StackSetName": str,
         "OperationId": str,
     },
 )
 _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef = TypedDict(
     "_OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     {
         "CallAs": CallAsType,
         "Filters": Sequence[OperationResultFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef(
     _RequiredListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
     _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListStackSetOperationResultsInputRequestTypeDef = TypedDict(
     "_RequiredListStackSetOperationResultsInputRequestTypeDef",
     {
         "StackSetName": str,
         "OperationId": str,
     },
 )
@@ -2609,40 +2548,38 @@
         "MaxResults": int,
         "CallAs": CallAsType,
         "Filters": Sequence[OperationResultFilterTypeDef],
     },
     total=False,
 )
 
-
 class ListStackSetOperationResultsInputRequestTypeDef(
     _RequiredListStackSetOperationResultsInputRequestTypeDef,
     _OptionalListStackSetOperationResultsInputRequestTypeDef,
 ):
     pass
 
-
 ListTypeVersionsOutputTypeDef = TypedDict(
     "ListTypeVersionsOutputTypeDef",
     {
         "TypeVersionSummaries": List[TypeVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTypesInputListTypesPaginateTypeDef = TypedDict(
     "ListTypesInputListTypesPaginateTypeDef",
     {
         "Visibility": VisibilityType,
         "ProvisioningType": ProvisioningTypeType,
         "DeprecatedStatus": DeprecatedStatusType,
         "Type": RegistryTypeType,
         "Filters": TypeFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTypesInputRequestTypeDef = TypedDict(
     "ListTypesInputRequestTypeDef",
     {
@@ -2658,15 +2595,15 @@
 )
 
 ListTypesOutputTypeDef = TypedDict(
     "ListTypesOutputTypeDef",
     {
         "TypeSummaries": List[TypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ParameterDeclarationTypeDef = TypedDict(
     "ParameterDeclarationTypeDef",
     {
         "ParameterKey": str,
@@ -2698,48 +2635,46 @@
         "ActualProperties": str,
         "PropertyDifferences": List[PropertyDifferenceTypeDef],
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
-
 class StackResourceDriftTypeDef(
     _RequiredStackResourceDriftTypeDef, _OptionalStackResourceDriftTypeDef
 ):
     pass
 
-
 ResourceChangeDetailTypeDef = TypedDict(
     "ResourceChangeDetailTypeDef",
     {
         "Target": ResourceTargetDefinitionTypeDef,
         "Evaluation": EvaluationTypeType,
         "ChangeSource": ChangeSourceType,
         "CausingEntity": str,
     },
     total=False,
 )
 
-RollbackConfigurationResponseMetadataTypeDef = TypedDict(
-    "RollbackConfigurationResponseMetadataTypeDef",
+RollbackConfigurationOutputTypeDef = TypedDict(
+    "RollbackConfigurationOutputTypeDef",
     {
         "RollbackTriggers": List[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
-        "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
+        "RollbackTriggers": List[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredStackSummaryTypeDef = TypedDict(
     "_RequiredStackSummaryTypeDef",
     {
         "StackName": str,
         "CreationTime": datetime,
@@ -2757,19 +2692,17 @@
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationSummaryTypeDef,
     },
     total=False,
 )
 
-
 class StackSummaryTypeDef(_RequiredStackSummaryTypeDef, _OptionalStackSummaryTypeDef):
     pass
 
-
 StackInstanceSummaryTypeDef = TypedDict(
     "StackInstanceSummaryTypeDef",
     {
         "StackSetId": str,
         "Region": str,
         "Account": str,
         "StackId": str,
@@ -2823,21 +2756,19 @@
         "Metadata": str,
         "DriftInformation": StackResourceDriftInformationTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
-
 class StackResourceDetailTypeDef(
     _RequiredStackResourceDetailTypeDef, _OptionalStackResourceDetailTypeDef
 ):
     pass
 
-
 _RequiredStackResourceTypeDef = TypedDict(
     "_RequiredStackResourceTypeDef",
     {
         "LogicalResourceId": str,
         "ResourceType": str,
         "Timestamp": datetime,
         "ResourceStatus": ResourceStatusType,
@@ -2853,19 +2784,17 @@
         "Description": str,
         "DriftInformation": StackResourceDriftInformationTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
-
 class StackResourceTypeDef(_RequiredStackResourceTypeDef, _OptionalStackResourceTypeDef):
     pass
 
-
 _RequiredStackResourceSummaryTypeDef = TypedDict(
     "_RequiredStackResourceSummaryTypeDef",
     {
         "LogicalResourceId": str,
         "ResourceType": str,
         "LastUpdatedTimestamp": datetime,
         "ResourceStatus": ResourceStatusType,
@@ -2878,21 +2807,19 @@
         "ResourceStatusReason": str,
         "DriftInformation": StackResourceDriftInformationSummaryTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
-
 class StackResourceSummaryTypeDef(
     _RequiredStackResourceSummaryTypeDef, _OptionalStackResourceSummaryTypeDef
 ):
     pass
 
-
 StackSetTypeDef = TypedDict(
     "StackSetTypeDef",
     {
         "StackSetName": str,
         "StackSetId": str,
         "Description": str,
         "Status": StackSetStatusType,
@@ -2909,43 +2836,46 @@
         "OrganizationalUnitIds": List[str],
         "ManagedExecution": ManagedExecutionTypeDef,
         "Regions": List[str],
     },
     total=False,
 )
 
+StackSetOperationPreferencesUnionTypeDef = Union[
+    StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+]
 StackSetOperationSummaryTypeDef = TypedDict(
     "StackSetOperationSummaryTypeDef",
     {
         "OperationId": str,
         "Action": StackSetOperationActionType,
         "Status": StackSetOperationStatusType,
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
-        "OperationPreferences": StackSetOperationPreferencesTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
     },
     total=False,
 )
 
 StackSetOperationTypeDef = TypedDict(
     "StackSetOperationTypeDef",
     {
         "OperationId": str,
         "StackSetId": str,
         "Action": StackSetOperationActionType,
         "Status": StackSetOperationStatusType,
-        "OperationPreferences": StackSetOperationPreferencesTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
         "RetainStacks": bool,
         "AdministrationRoleARN": str,
         "ExecutionRoleName": str,
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
-        "DeploymentTargets": DeploymentTargetsTypeDef,
+        "DeploymentTargets": DeploymentTargetsOutputTypeDef,
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
     },
     total=False,
 )
 
@@ -2953,34 +2883,34 @@
     "ValidateTemplateOutputTypeDef",
     {
         "Parameters": List[TemplateParameterTypeDef],
         "Description": str,
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "DeclaredTransforms": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackSetOperationResultsOutputTypeDef = TypedDict(
     "ListStackSetOperationResultsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationResultSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDescribeTypeConfigurationsOutputTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     {
         "Errors": List[BatchDescribeTypeConfigurationsErrorTypeDef],
         "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierTypeDef],
         "TypeConfigurations": List[TypeConfigurationDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeSetHookTypeDef = TypedDict(
     "ChangeSetHookTypeDef",
     {
         "InvocationPoint": Literal["PRE_PROVISION"],
@@ -2994,15 +2924,15 @@
 )
 
 ListStackSetsOutputTypeDef = TypedDict(
     "ListStackSetsOutputTypeDef",
     {
         "Summaries": List[StackSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTemplateSummaryOutputTypeDef = TypedDict(
     "GetTemplateSummaryOutputTypeDef",
     {
         "Parameters": List[ParameterDeclarationTypeDef],
@@ -3010,32 +2940,32 @@
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "ResourceTypes": List[str],
         "Version": str,
         "Metadata": str,
         "DeclaredTransforms": List[str],
         "ResourceIdentifierSummaries": List[ResourceIdentifierSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourceDriftsOutputTypeDef = TypedDict(
     "DescribeStackResourceDriftsOutputTypeDef",
     {
         "StackResourceDrifts": List[StackResourceDriftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectStackResourceDriftOutputTypeDef = TypedDict(
     "DetectStackResourceDriftOutputTypeDef",
     {
         "StackResourceDrift": StackResourceDriftTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -3047,14 +2977,51 @@
         "Details": List[ResourceChangeDetailTypeDef],
         "ChangeSetId": str,
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
+_RequiredStackTypeDef = TypedDict(
+    "_RequiredStackTypeDef",
+    {
+        "StackName": str,
+        "CreationTime": datetime,
+        "StackStatus": StackStatusType,
+    },
+)
+_OptionalStackTypeDef = TypedDict(
+    "_OptionalStackTypeDef",
+    {
+        "StackId": str,
+        "ChangeSetId": str,
+        "Description": str,
+        "Parameters": List[ParameterTypeDef],
+        "DeletionTime": datetime,
+        "LastUpdatedTime": datetime,
+        "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
+        "StackStatusReason": str,
+        "DisableRollback": bool,
+        "NotificationARNs": List[str],
+        "TimeoutInMinutes": int,
+        "Capabilities": List[CapabilityType],
+        "Outputs": List[OutputTypeDef],
+        "RoleARN": str,
+        "Tags": List[TagTypeDef],
+        "EnableTerminationProtection": bool,
+        "ParentId": str,
+        "RootId": str,
+        "DriftInformation": StackDriftInformationTypeDef,
+    },
+    total=False,
+)
+
+class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
+    pass
+
 _RequiredCreateChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredCreateChangeSetInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
     },
 )
@@ -3077,21 +3044,19 @@
         "ResourcesToImport": Sequence[ResourceToImportTypeDef],
         "IncludeNestedStacks": bool,
         "OnStackFailure": OnStackFailureType,
     },
     total=False,
 )
 
-
 class CreateChangeSetInputRequestTypeDef(
     _RequiredCreateChangeSetInputRequestTypeDef, _OptionalCreateChangeSetInputRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateStackInputRequestTypeDef = TypedDict(
     "_RequiredCreateStackInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalCreateStackInputRequestTypeDef = TypedDict(
@@ -3113,21 +3078,19 @@
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "EnableTerminationProtection": bool,
     },
     total=False,
 )
 
-
 class CreateStackInputRequestTypeDef(
     _RequiredCreateStackInputRequestTypeDef, _OptionalCreateStackInputRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateStackInputServiceResourceCreateStackTypeDef = TypedDict(
     "_RequiredCreateStackInputServiceResourceCreateStackTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalCreateStackInputServiceResourceCreateStackTypeDef = TypedDict(
@@ -3149,61 +3112,23 @@
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "EnableTerminationProtection": bool,
     },
     total=False,
 )
 
-
 class CreateStackInputServiceResourceCreateStackTypeDef(
     _RequiredCreateStackInputServiceResourceCreateStackTypeDef,
     _OptionalCreateStackInputServiceResourceCreateStackTypeDef,
 ):
     pass
 
-
-_RequiredStackTypeDef = TypedDict(
-    "_RequiredStackTypeDef",
-    {
-        "StackName": str,
-        "CreationTime": datetime,
-        "StackStatus": StackStatusType,
-    },
-)
-_OptionalStackTypeDef = TypedDict(
-    "_OptionalStackTypeDef",
-    {
-        "StackId": str,
-        "ChangeSetId": str,
-        "Description": str,
-        "Parameters": List[ParameterTypeDef],
-        "DeletionTime": datetime,
-        "LastUpdatedTime": datetime,
-        "RollbackConfiguration": RollbackConfigurationTypeDef,
-        "StackStatusReason": str,
-        "DisableRollback": bool,
-        "NotificationARNs": List[str],
-        "TimeoutInMinutes": int,
-        "Capabilities": List[CapabilityType],
-        "Outputs": List[OutputTypeDef],
-        "RoleARN": str,
-        "Tags": List[TagTypeDef],
-        "EnableTerminationProtection": bool,
-        "ParentId": str,
-        "RootId": str,
-        "DriftInformation": StackDriftInformationTypeDef,
-    },
-    total=False,
-)
-
-
-class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
-    pass
-
-
+RollbackConfigurationUnionTypeDef = Union[
+    RollbackConfigurationTypeDef, RollbackConfigurationOutputTypeDef
+]
 _RequiredUpdateStackInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStackInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalUpdateStackInputRequestTypeDef = TypedDict(
@@ -3225,21 +3150,19 @@
         "Tags": Sequence[TagTypeDef],
         "DisableRollback": bool,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class UpdateStackInputRequestTypeDef(
     _RequiredUpdateStackInputRequestTypeDef, _OptionalUpdateStackInputRequestTypeDef
 ):
     pass
 
-
 UpdateStackInputStackUpdateTypeDef = TypedDict(
     "UpdateStackInputStackUpdateTypeDef",
     {
         "TemplateBody": str,
         "TemplateURL": str,
         "UsePreviousTemplate": bool,
         "StackPolicyDuringUpdateBody": str,
@@ -3260,96 +3183,96 @@
 )
 
 ListStacksOutputTypeDef = TypedDict(
     "ListStacksOutputTypeDef",
     {
         "StackSummaries": List[StackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackInstancesOutputTypeDef = TypedDict(
     "ListStackInstancesOutputTypeDef",
     {
         "Summaries": List[StackInstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackInstanceOutputTypeDef = TypedDict(
     "DescribeStackInstanceOutputTypeDef",
     {
         "StackInstance": StackInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourceOutputTypeDef = TypedDict(
     "DescribeStackResourceOutputTypeDef",
     {
         "StackResourceDetail": StackResourceDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourcesOutputTypeDef = TypedDict(
     "DescribeStackResourcesOutputTypeDef",
     {
         "StackResources": List[StackResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackResourcesOutputTypeDef = TypedDict(
     "ListStackResourcesOutputTypeDef",
     {
         "StackResourceSummaries": List[StackResourceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSetOutputTypeDef = TypedDict(
     "DescribeStackSetOutputTypeDef",
     {
         "StackSet": StackSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackSetOperationsOutputTypeDef = TypedDict(
     "ListStackSetOperationsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSetOperationOutputTypeDef = TypedDict(
     "DescribeStackSetOperationOutputTypeDef",
     {
         "StackSetOperation": StackSetOperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetHooksOutputTypeDef = TypedDict(
     "DescribeChangeSetHooksOutputTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetName": str,
         "Hooks": List[ChangeSetHookTypeDef],
         "Status": ChangeSetHooksStatusType,
         "NextToken": str,
         "StackId": str,
         "StackName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeTypeDef = TypedDict(
     "ChangeTypeDef",
     {
         "Type": Literal["Resource"],
@@ -3360,15 +3283,15 @@
 )
 
 DescribeStacksOutputTypeDef = TypedDict(
     "DescribeStacksOutputTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetOutputTypeDef = TypedDict(
     "DescribeChangeSetOutputTypeDef",
     {
         "ChangeSetName": str,
@@ -3378,19 +3301,19 @@
         "Description": str,
         "Parameters": List[ParameterTypeDef],
         "CreationTime": datetime,
         "ExecutionStatus": ExecutionStatusType,
         "Status": ChangeSetStatusType,
         "StatusReason": str,
         "NotificationARNs": List[str],
-        "RollbackConfiguration": RollbackConfigurationTypeDef,
+        "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
         "Capabilities": List[CapabilityType],
         "Tags": List[TagTypeDef],
         "Changes": List[ChangeTypeDef],
         "NextToken": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
         "OnStackFailure": OnStackFailureType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/type_defs.pyi` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudformation.type_defs import AccountGateResultTypeDef
 
-    data: AccountGateResultTypeDef = {...}
+    data: AccountGateResultTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountFilterTypeType,
     AccountGateStatusType,
     CallAsType,
     CapabilityType,
     CategoryType,
@@ -74,169 +74,173 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountGateResultTypeDef",
     "AccountLimitTypeDef",
     "LoggingConfigTypeDef",
-    "ActivateTypeOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AutoDeploymentTypeDef",
     "TypeConfigurationIdentifierTypeDef",
     "TypeConfigurationDetailsTypeDef",
     "CancelUpdateStackInputRequestTypeDef",
     "CancelUpdateStackInputStackCancelUpdateTypeDef",
     "ChangeSetHookResourceTargetDetailsTypeDef",
     "ChangeSetSummaryTypeDef",
     "ContinueUpdateRollbackInputRequestTypeDef",
     "ParameterTypeDef",
     "ResourceToImportTypeDef",
     "TagTypeDef",
-    "CreateChangeSetOutputTypeDef",
     "DeploymentTargetsTypeDef",
     "StackSetOperationPreferencesTypeDef",
-    "CreateStackInstancesOutputTypeDef",
-    "CreateStackOutputTypeDef",
     "ManagedExecutionTypeDef",
-    "CreateStackSetOutputTypeDef",
     "DeactivateTypeInputRequestTypeDef",
     "DeleteChangeSetInputRequestTypeDef",
     "DeleteStackInputRequestTypeDef",
     "DeleteStackInputStackDeleteTypeDef",
-    "DeleteStackInstancesOutputTypeDef",
     "DeleteStackSetInputRequestTypeDef",
+    "DeploymentTargetsOutputTypeDef",
     "DeregisterTypeInputRequestTypeDef",
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "DescribeChangeSetHooksInputRequestTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
     "DescribeChangeSetInputRequestTypeDef",
     "DescribeOrganizationsAccessInputRequestTypeDef",
-    "DescribeOrganizationsAccessOutputTypeDef",
     "DescribePublisherInputRequestTypeDef",
-    "DescribePublisherOutputTypeDef",
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
     "DescribeStackEventsInputRequestTypeDef",
     "StackEventTypeDef",
     "DescribeStackInstanceInputRequestTypeDef",
     "DescribeStackResourceDriftsInputRequestTypeDef",
     "DescribeStackResourceInputRequestTypeDef",
     "DescribeStackResourcesInputRequestTypeDef",
     "DescribeStackSetInputRequestTypeDef",
     "DescribeStackSetOperationInputRequestTypeDef",
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
     "DescribeStacksInputRequestTypeDef",
     "DescribeTypeInputRequestTypeDef",
     "RequiredActivatedTypeTypeDef",
     "DescribeTypeRegistrationInputRequestTypeDef",
-    "DescribeTypeRegistrationOutputTypeDef",
     "DetectStackDriftInputRequestTypeDef",
-    "DetectStackDriftOutputTypeDef",
     "DetectStackResourceDriftInputRequestTypeDef",
-    "DetectStackSetDriftOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EstimateTemplateCostOutputTypeDef",
     "ExecuteChangeSetInputRequestTypeDef",
     "ExportTypeDef",
     "GetStackPolicyInputRequestTypeDef",
-    "GetStackPolicyOutputTypeDef",
     "GetTemplateInputRequestTypeDef",
-    "GetTemplateOutputTypeDef",
     "GetTemplateSummaryInputRequestTypeDef",
     "ResourceIdentifierSummaryTypeDef",
-    "ImportStacksToStackSetOutputTypeDef",
-    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
     "ListChangeSetsInputRequestTypeDef",
-    "ListExportsInputListExportsPaginateTypeDef",
     "ListExportsInputRequestTypeDef",
-    "ListImportsInputListImportsPaginateTypeDef",
     "ListImportsInputRequestTypeDef",
-    "ListImportsOutputTypeDef",
     "StackInstanceFilterTypeDef",
-    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
     "ListStackResourcesInputRequestTypeDef",
     "OperationResultFilterTypeDef",
-    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
     "ListStackSetOperationsInputRequestTypeDef",
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
     "ListStackSetsInputRequestTypeDef",
-    "ListStacksInputListStacksPaginateTypeDef",
     "ListStacksInputRequestTypeDef",
     "ListTypeRegistrationsInputRequestTypeDef",
-    "ListTypeRegistrationsOutputTypeDef",
     "ListTypeVersionsInputRequestTypeDef",
     "TypeVersionSummaryTypeDef",
     "TypeFiltersTypeDef",
     "TypeSummaryTypeDef",
-    "ModuleInfoResponseMetadataTypeDef",
     "ModuleInfoTypeDef",
     "OutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterConstraintsTypeDef",
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     "PropertyDifferenceTypeDef",
     "PublishTypeInputRequestTypeDef",
-    "PublishTypeOutputTypeDef",
     "RecordHandlerProgressInputRequestTypeDef",
     "RegisterPublisherInputRequestTypeDef",
-    "RegisterPublisherOutputTypeDef",
-    "RegisterTypeOutputTypeDef",
     "ResourceTargetDefinitionTypeDef",
-    "ResponseMetadataTypeDef",
     "RollbackTriggerTypeDef",
     "RollbackStackInputRequestTypeDef",
-    "RollbackStackOutputTypeDef",
     "SetStackPolicyInputRequestTypeDef",
     "SetTypeConfigurationInputRequestTypeDef",
-    "SetTypeConfigurationOutputTypeDef",
     "SetTypeDefaultVersionInputRequestTypeDef",
     "SignalResourceInputRequestTypeDef",
-    "StackDriftInformationResponseMetadataTypeDef",
     "StackDriftInformationSummaryTypeDef",
     "StackDriftInformationTypeDef",
     "StackInstanceComprehensiveStatusTypeDef",
     "StackResourceDriftInformationTypeDef",
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
     "StackResourceDriftInformationSummaryTypeDef",
     "StackSetDriftDetectionDetailsTypeDef",
+    "StackSetOperationPreferencesOutputTypeDef",
     "StackSetOperationStatusDetailsTypeDef",
     "StopStackSetOperationInputRequestTypeDef",
     "TemplateParameterTypeDef",
     "TestTypeInputRequestTypeDef",
-    "TestTypeOutputTypeDef",
-    "UpdateStackInstancesOutputTypeDef",
-    "UpdateStackOutputTypeDef",
-    "UpdateStackSetOutputTypeDef",
     "UpdateTerminationProtectionInputRequestTypeDef",
-    "UpdateTerminationProtectionOutputTypeDef",
     "ValidateTemplateInputRequestTypeDef",
     "StackSetOperationResultSummaryTypeDef",
-    "DescribeAccountLimitsOutputTypeDef",
     "ActivateTypeInputRequestTypeDef",
     "RegisterTypeInputRequestTypeDef",
+    "ActivateTypeOutputTypeDef",
+    "CreateChangeSetOutputTypeDef",
+    "CreateStackInstancesOutputTypeDef",
+    "CreateStackOutputTypeDef",
+    "CreateStackSetOutputTypeDef",
+    "DeleteStackInstancesOutputTypeDef",
+    "DescribeAccountLimitsOutputTypeDef",
+    "DescribeOrganizationsAccessOutputTypeDef",
+    "DescribePublisherOutputTypeDef",
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    "DescribeTypeRegistrationOutputTypeDef",
+    "DetectStackDriftOutputTypeDef",
+    "DetectStackSetDriftOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EstimateTemplateCostOutputTypeDef",
+    "GetStackPolicyOutputTypeDef",
+    "GetTemplateOutputTypeDef",
+    "ImportStacksToStackSetOutputTypeDef",
+    "ListImportsOutputTypeDef",
+    "ListTypeRegistrationsOutputTypeDef",
+    "ModuleInfoResponseTypeDef",
+    "PublishTypeOutputTypeDef",
+    "RegisterPublisherOutputTypeDef",
+    "RegisterTypeOutputTypeDef",
+    "RollbackStackOutputTypeDef",
+    "SetTypeConfigurationOutputTypeDef",
+    "StackDriftInformationResponseTypeDef",
+    "StackResourceDriftInformationResponseTypeDef",
+    "StackResourceDriftInformationSummaryResponseTypeDef",
+    "TestTypeOutputTypeDef",
+    "UpdateStackInstancesOutputTypeDef",
+    "UpdateStackOutputTypeDef",
+    "UpdateStackSetOutputTypeDef",
+    "UpdateTerminationProtectionOutputTypeDef",
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     "BatchDescribeTypeConfigurationsInputRequestTypeDef",
     "ChangeSetHookTargetDetailsTypeDef",
     "ListChangeSetsOutputTypeDef",
     "EstimateTemplateCostInputRequestTypeDef",
     "CreateStackInstancesInputRequestTypeDef",
     "DeleteStackInstancesInputRequestTypeDef",
     "DetectStackSetDriftInputRequestTypeDef",
     "ImportStacksToStackSetInputRequestTypeDef",
     "UpdateStackInstancesInputRequestTypeDef",
     "CreateStackSetInputRequestTypeDef",
     "StackSetSummaryTypeDef",
     "UpdateStackSetInputRequestTypeDef",
+    "DeploymentTargetsUnionTypeDef",
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    "ListChangeSetsInputListChangeSetsPaginateTypeDef",
+    "ListExportsInputListExportsPaginateTypeDef",
+    "ListImportsInputListImportsPaginateTypeDef",
+    "ListStackResourcesInputListStackResourcesPaginateTypeDef",
+    "ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    "ListStacksInputListStacksPaginateTypeDef",
     "DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackCreateCompleteWaitTypeDef",
     "DescribeStacksInputStackDeleteCompleteWaitTypeDef",
     "DescribeStacksInputStackExistsWaitTypeDef",
     "DescribeStacksInputStackImportCompleteWaitTypeDef",
     "DescribeStacksInputStackRollbackCompleteWaitTypeDef",
     "DescribeStacksInputStackUpdateCompleteWaitTypeDef",
@@ -251,38 +255,40 @@
     "ListTypeVersionsOutputTypeDef",
     "ListTypesInputListTypesPaginateTypeDef",
     "ListTypesInputRequestTypeDef",
     "ListTypesOutputTypeDef",
     "ParameterDeclarationTypeDef",
     "StackResourceDriftTypeDef",
     "ResourceChangeDetailTypeDef",
-    "RollbackConfigurationResponseMetadataTypeDef",
+    "RollbackConfigurationOutputTypeDef",
     "RollbackConfigurationTypeDef",
     "StackSummaryTypeDef",
     "StackInstanceSummaryTypeDef",
     "StackInstanceTypeDef",
     "StackResourceDetailTypeDef",
     "StackResourceTypeDef",
     "StackResourceSummaryTypeDef",
     "StackSetTypeDef",
+    "StackSetOperationPreferencesUnionTypeDef",
     "StackSetOperationSummaryTypeDef",
     "StackSetOperationTypeDef",
     "ValidateTemplateOutputTypeDef",
     "ListStackSetOperationResultsOutputTypeDef",
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     "ChangeSetHookTypeDef",
     "ListStackSetsOutputTypeDef",
     "GetTemplateSummaryOutputTypeDef",
     "DescribeStackResourceDriftsOutputTypeDef",
     "DetectStackResourceDriftOutputTypeDef",
     "ResourceChangeTypeDef",
+    "StackTypeDef",
     "CreateChangeSetInputRequestTypeDef",
     "CreateStackInputRequestTypeDef",
     "CreateStackInputServiceResourceCreateStackTypeDef",
-    "StackTypeDef",
+    "RollbackConfigurationUnionTypeDef",
     "UpdateStackInputRequestTypeDef",
     "UpdateStackInputStackUpdateTypeDef",
     "ListStacksOutputTypeDef",
     "ListStackInstancesOutputTypeDef",
     "DescribeStackInstanceOutputTypeDef",
     "DescribeStackResourceOutputTypeDef",
     "DescribeStackResourcesOutputTypeDef",
@@ -318,19 +324,22 @@
     "LoggingConfigTypeDef",
     {
         "LogRoleArn": str,
         "LogGroupName": str,
     },
 )
 
-ActivateTypeOutputTypeDef = TypedDict(
-    "ActivateTypeOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AutoDeploymentTypeDef = TypedDict(
     "AutoDeploymentTypeDef",
     {
         "Enabled": bool,
@@ -375,19 +384,21 @@
     "_OptionalCancelUpdateStackInputRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class CancelUpdateStackInputRequestTypeDef(
     _RequiredCancelUpdateStackInputRequestTypeDef, _OptionalCancelUpdateStackInputRequestTypeDef
 ):
     pass
 
+
 CancelUpdateStackInputStackCancelUpdateTypeDef = TypedDict(
     "CancelUpdateStackInputStackCancelUpdateTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
@@ -433,20 +444,22 @@
         "RoleARN": str,
         "ResourcesToSkip": Sequence[str],
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class ContinueUpdateRollbackInputRequestTypeDef(
     _RequiredContinueUpdateRollbackInputRequestTypeDef,
     _OptionalContinueUpdateRollbackInputRequestTypeDef,
 ):
     pass
 
+
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "ParameterKey": str,
         "ParameterValue": str,
         "UsePreviousValue": bool,
         "ResolvedValue": str,
@@ -467,23 +480,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateChangeSetOutputTypeDef = TypedDict(
-    "CreateChangeSetOutputTypeDef",
-    {
-        "Id": str,
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeploymentTargetsTypeDef = TypedDict(
     "DeploymentTargetsTypeDef",
     {
         "Accounts": Sequence[str],
         "AccountsUrl": str,
         "OrganizationalUnitIds": Sequence[str],
         "AccountFilterType": AccountFilterTypeType,
@@ -500,46 +504,22 @@
         "FailureTolerancePercentage": int,
         "MaxConcurrentCount": int,
         "MaxConcurrentPercentage": int,
     },
     total=False,
 )
 
-CreateStackInstancesOutputTypeDef = TypedDict(
-    "CreateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStackOutputTypeDef = TypedDict(
-    "CreateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ManagedExecutionTypeDef = TypedDict(
     "ManagedExecutionTypeDef",
     {
         "Active": bool,
     },
     total=False,
 )
 
-CreateStackSetOutputTypeDef = TypedDict(
-    "CreateStackSetOutputTypeDef",
-    {
-        "StackSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeactivateTypeInputRequestTypeDef = TypedDict(
     "DeactivateTypeInputRequestTypeDef",
     {
         "TypeName": str,
         "Type": ThirdPartyTypeType,
         "Arn": str,
     },
@@ -556,19 +536,21 @@
     "_OptionalDeleteChangeSetInputRequestTypeDef",
     {
         "StackName": str,
     },
     total=False,
 )
 
+
 class DeleteChangeSetInputRequestTypeDef(
     _RequiredDeleteChangeSetInputRequestTypeDef, _OptionalDeleteChangeSetInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteStackInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStackInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalDeleteStackInputRequestTypeDef = TypedDict(
@@ -577,71 +559,80 @@
         "RetainResources": Sequence[str],
         "RoleARN": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteStackInputRequestTypeDef(
     _RequiredDeleteStackInputRequestTypeDef, _OptionalDeleteStackInputRequestTypeDef
 ):
     pass
 
+
 DeleteStackInputStackDeleteTypeDef = TypedDict(
     "DeleteStackInputStackDeleteTypeDef",
     {
         "RetainResources": Sequence[str],
         "RoleARN": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-DeleteStackInstancesOutputTypeDef = TypedDict(
-    "DeleteStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteStackSetInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalDeleteStackSetInputRequestTypeDef = TypedDict(
     "_OptionalDeleteStackSetInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+
 class DeleteStackSetInputRequestTypeDef(
     _RequiredDeleteStackSetInputRequestTypeDef, _OptionalDeleteStackSetInputRequestTypeDef
 ):
     pass
 
+
+DeploymentTargetsOutputTypeDef = TypedDict(
+    "DeploymentTargetsOutputTypeDef",
+    {
+        "Accounts": List[str],
+        "AccountsUrl": str,
+        "OrganizationalUnitIds": List[str],
+        "AccountFilterType": AccountFilterTypeType,
+    },
+    total=False,
+)
+
 DeregisterTypeInputRequestTypeDef = TypedDict(
     "DeregisterTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
     },
     total=False,
 )
 
-DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
-    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
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
 
 DescribeAccountLimitsInputRequestTypeDef = TypedDict(
     "DescribeAccountLimitsInputRequestTypeDef",
     {
@@ -662,50 +653,31 @@
         "StackName": str,
         "NextToken": str,
         "LogicalResourceId": str,
     },
     total=False,
 )
 
+
 class DescribeChangeSetHooksInputRequestTypeDef(
     _RequiredDescribeChangeSetHooksInputRequestTypeDef,
     _OptionalDescribeChangeSetHooksInputRequestTypeDef,
 ):
     pass
 
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "ChangeSetName": str,
-    },
-)
-_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
-    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
-    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputRequestTypeDef = TypedDict(
@@ -713,84 +685,44 @@
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeChangeSetInputRequestTypeDef(
     _RequiredDescribeChangeSetInputRequestTypeDef, _OptionalDescribeChangeSetInputRequestTypeDef
 ):
     pass
 
+
 DescribeOrganizationsAccessInputRequestTypeDef = TypedDict(
     "DescribeOrganizationsAccessInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-DescribeOrganizationsAccessOutputTypeDef = TypedDict(
-    "DescribeOrganizationsAccessOutputTypeDef",
-    {
-        "Status": OrganizationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribePublisherInputRequestTypeDef = TypedDict(
     "DescribePublisherInputRequestTypeDef",
     {
         "PublisherId": str,
     },
     total=False,
 )
 
-DescribePublisherOutputTypeDef = TypedDict(
-    "DescribePublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "PublisherStatus": PublisherStatusType,
-        "IdentityProvider": IdentityProviderType,
-        "PublisherProfile": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeStackDriftDetectionStatusInputRequestTypeDef = TypedDict(
     "DescribeStackDriftDetectionStatusInputRequestTypeDef",
     {
         "StackDriftDetectionId": str,
     },
 )
 
-DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
-    "DescribeStackDriftDetectionStatusOutputTypeDef",
-    {
-        "StackId": str,
-        "StackDriftDetectionId": str,
-        "StackDriftStatus": StackDriftStatusType,
-        "DetectionStatus": StackDriftDetectionStatusType,
-        "DetectionStatusReason": str,
-        "DriftedStackResourceCount": int,
-        "Timestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
-    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeStackEventsInputRequestTypeDef = TypedDict(
     "DescribeStackEventsInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
     total=False,
@@ -820,17 +752,19 @@
         "HookStatusReason": str,
         "HookInvocationPoint": Literal["PRE_PROVISION"],
         "HookFailureMode": HookFailureModeType,
     },
     total=False,
 )
 
+
 class StackEventTypeDef(_RequiredStackEventTypeDef, _OptionalStackEventTypeDef):
     pass
 
+
 _RequiredDescribeStackInstanceInputRequestTypeDef = TypedDict(
     "_RequiredDescribeStackInstanceInputRequestTypeDef",
     {
         "StackSetName": str,
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
     },
@@ -839,20 +773,22 @@
     "_OptionalDescribeStackInstanceInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+
 class DescribeStackInstanceInputRequestTypeDef(
     _RequiredDescribeStackInstanceInputRequestTypeDef,
     _OptionalDescribeStackInstanceInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeStackResourceDriftsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeStackResourceDriftsInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalDescribeStackResourceDriftsInputRequestTypeDef = TypedDict(
@@ -861,20 +797,22 @@
         "StackResourceDriftStatusFilters": Sequence[StackResourceDriftStatusType],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeStackResourceDriftsInputRequestTypeDef(
     _RequiredDescribeStackResourceDriftsInputRequestTypeDef,
     _OptionalDescribeStackResourceDriftsInputRequestTypeDef,
 ):
     pass
 
+
 DescribeStackResourceInputRequestTypeDef = TypedDict(
     "DescribeStackResourceInputRequestTypeDef",
     {
         "StackName": str,
         "LogicalResourceId": str,
     },
 )
@@ -899,19 +837,21 @@
     "_OptionalDescribeStackSetInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+
 class DescribeStackSetInputRequestTypeDef(
     _RequiredDescribeStackSetInputRequestTypeDef, _OptionalDescribeStackSetInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeStackSetOperationInputRequestTypeDef = TypedDict(
     "_RequiredDescribeStackSetOperationInputRequestTypeDef",
     {
         "StackSetName": str,
         "OperationId": str,
     },
 )
@@ -919,28 +859,21 @@
     "_OptionalDescribeStackSetOperationInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+
 class DescribeStackSetOperationInputRequestTypeDef(
     _RequiredDescribeStackSetOperationInputRequestTypeDef,
     _OptionalDescribeStackSetOperationInputRequestTypeDef,
 ):
     pass
 
-DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
-    "DescribeStacksInputDescribeStacksPaginateTypeDef",
-    {
-        "StackName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeStacksInputRequestTypeDef = TypedDict(
     "DescribeStacksInputRequestTypeDef",
     {
         "StackName": str,
         "NextToken": str,
     },
@@ -974,83 +907,43 @@
 DescribeTypeRegistrationInputRequestTypeDef = TypedDict(
     "DescribeTypeRegistrationInputRequestTypeDef",
     {
         "RegistrationToken": str,
     },
 )
 
-DescribeTypeRegistrationOutputTypeDef = TypedDict(
-    "DescribeTypeRegistrationOutputTypeDef",
-    {
-        "ProgressStatus": RegistrationStatusType,
-        "Description": str,
-        "TypeArn": str,
-        "TypeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDetectStackDriftInputRequestTypeDef = TypedDict(
     "_RequiredDetectStackDriftInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalDetectStackDriftInputRequestTypeDef = TypedDict(
     "_OptionalDetectStackDriftInputRequestTypeDef",
     {
         "LogicalResourceIds": Sequence[str],
     },
     total=False,
 )
 
+
 class DetectStackDriftInputRequestTypeDef(
     _RequiredDetectStackDriftInputRequestTypeDef, _OptionalDetectStackDriftInputRequestTypeDef
 ):
     pass
 
-DetectStackDriftOutputTypeDef = TypedDict(
-    "DetectStackDriftOutputTypeDef",
-    {
-        "StackDriftDetectionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DetectStackResourceDriftInputRequestTypeDef = TypedDict(
     "DetectStackResourceDriftInputRequestTypeDef",
     {
         "StackName": str,
         "LogicalResourceId": str,
     },
 )
 
-DetectStackSetDriftOutputTypeDef = TypedDict(
-    "DetectStackSetDriftOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EstimateTemplateCostOutputTypeDef = TypedDict(
-    "EstimateTemplateCostOutputTypeDef",
-    {
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredExecuteChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredExecuteChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalExecuteChangeSetInputRequestTypeDef = TypedDict(
@@ -1059,19 +952,21 @@
         "StackName": str,
         "ClientRequestToken": str,
         "DisableRollback": bool,
     },
     total=False,
 )
 
+
 class ExecuteChangeSetInputRequestTypeDef(
     _RequiredExecuteChangeSetInputRequestTypeDef, _OptionalExecuteChangeSetInputRequestTypeDef
 ):
     pass
 
+
 ExportTypeDef = TypedDict(
     "ExportTypeDef",
     {
         "ExportingStackId": str,
         "Name": str,
         "Value": str,
     },
@@ -1081,41 +976,24 @@
 GetStackPolicyInputRequestTypeDef = TypedDict(
     "GetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 
-GetStackPolicyOutputTypeDef = TypedDict(
-    "GetStackPolicyOutputTypeDef",
-    {
-        "StackPolicyBody": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTemplateInputRequestTypeDef = TypedDict(
     "GetTemplateInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
         "TemplateStage": TemplateStageType,
     },
     total=False,
 )
 
-GetTemplateOutputTypeDef = TypedDict(
-    "GetTemplateOutputTypeDef",
-    {
-        "TemplateBody": Dict[str, Any],
-        "StagesAvailable": List[TemplateStageType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTemplateSummaryInputRequestTypeDef = TypedDict(
     "GetTemplateSummaryInputRequestTypeDef",
     {
         "TemplateBody": str,
         "TemplateURL": str,
         "StackName": str,
         "StackSetName": str,
@@ -1130,203 +1008,103 @@
         "ResourceType": str,
         "LogicalResourceIds": List[str],
         "ResourceIdentifiers": List[str],
     },
     total=False,
 )
 
-ImportStacksToStackSetOutputTypeDef = TypedDict(
-    "ImportStacksToStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
-    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListChangeSetsInputListChangeSetsPaginateTypeDef(
-    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
-    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListChangeSetsInputRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListChangeSetsInputRequestTypeDef = TypedDict(
     "_OptionalListChangeSetsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChangeSetsInputRequestTypeDef(
     _RequiredListChangeSetsInputRequestTypeDef, _OptionalListChangeSetsInputRequestTypeDef
 ):
     pass
 
-ListExportsInputListExportsPaginateTypeDef = TypedDict(
-    "ListExportsInputListExportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListExportsInputRequestTypeDef = TypedDict(
     "ListExportsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_RequiredListImportsInputListImportsPaginateTypeDef",
-    {
-        "ExportName": str,
-    },
-)
-_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
-    "_OptionalListImportsInputListImportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListImportsInputListImportsPaginateTypeDef(
-    _RequiredListImportsInputListImportsPaginateTypeDef,
-    _OptionalListImportsInputListImportsPaginateTypeDef,
-):
-    pass
-
 _RequiredListImportsInputRequestTypeDef = TypedDict(
     "_RequiredListImportsInputRequestTypeDef",
     {
         "ExportName": str,
     },
 )
 _OptionalListImportsInputRequestTypeDef = TypedDict(
     "_OptionalListImportsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListImportsInputRequestTypeDef(
     _RequiredListImportsInputRequestTypeDef, _OptionalListImportsInputRequestTypeDef
 ):
     pass
 
-ListImportsOutputTypeDef = TypedDict(
-    "ListImportsOutputTypeDef",
-    {
-        "Imports": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 StackInstanceFilterTypeDef = TypedDict(
     "StackInstanceFilterTypeDef",
     {
         "Name": StackInstanceFilterNameType,
         "Values": str,
     },
     total=False,
 )
 
-_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "StackName": str,
-    },
-)
-_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStackResourcesInputListStackResourcesPaginateTypeDef(
-    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
-    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListStackResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListStackResourcesInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalListStackResourcesInputRequestTypeDef = TypedDict(
     "_OptionalListStackResourcesInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListStackResourcesInputRequestTypeDef(
     _RequiredListStackResourcesInputRequestTypeDef, _OptionalListStackResourcesInputRequestTypeDef
 ):
     pass
 
+
 OperationResultFilterTypeDef = TypedDict(
     "OperationResultFilterTypeDef",
     {
         "Name": Literal["OPERATION_RESULT_STATUS"],
         "Values": str,
     },
     total=False,
 )
 
-_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "StackSetName": str,
-    },
-)
-_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
-    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
-    {
-        "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
-    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListStackSetOperationsInputRequestTypeDef = TypedDict(
     "_RequiredListStackSetOperationsInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackSetOperationsInputRequestTypeDef = TypedDict(
@@ -1335,50 +1113,33 @@
         "NextToken": str,
         "MaxResults": int,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+
 class ListStackSetOperationsInputRequestTypeDef(
     _RequiredListStackSetOperationsInputRequestTypeDef,
     _OptionalListStackSetOperationsInputRequestTypeDef,
 ):
     pass
 
-ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
-    "ListStackSetsInputListStackSetsPaginateTypeDef",
-    {
-        "Status": StackSetStatusType,
-        "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListStackSetsInputRequestTypeDef = TypedDict(
     "ListStackSetsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Status": StackSetStatusType,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
-ListStacksInputListStacksPaginateTypeDef = TypedDict(
-    "ListStacksInputListStacksPaginateTypeDef",
-    {
-        "StackStatusFilter": Sequence[StackStatusType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStacksInputRequestTypeDef = TypedDict(
     "ListStacksInputRequestTypeDef",
     {
         "NextToken": str,
         "StackStatusFilter": Sequence[StackStatusType],
     },
     total=False,
@@ -1393,23 +1154,14 @@
         "RegistrationStatusFilter": RegistrationStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListTypeRegistrationsOutputTypeDef = TypedDict(
-    "ListTypeRegistrationsOutputTypeDef",
-    {
-        "RegistrationTokenList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTypeVersionsInputRequestTypeDef = TypedDict(
     "ListTypeVersionsInputRequestTypeDef",
     {
         "Type": RegistryTypeType,
         "TypeName": str,
         "Arn": str,
         "MaxResults": int,
@@ -1461,23 +1213,14 @@
         "PublisherIdentity": IdentityProviderType,
         "PublisherName": str,
         "IsActivated": bool,
     },
     total=False,
 )
 
-ModuleInfoResponseMetadataTypeDef = TypedDict(
-    "ModuleInfoResponseMetadataTypeDef",
-    {
-        "TypeHierarchy": str,
-        "LogicalIdHierarchy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ModuleInfoTypeDef = TypedDict(
     "ModuleInfoTypeDef",
     {
         "TypeHierarchy": str,
         "LogicalIdHierarchy": str,
     },
     total=False,
@@ -1490,24 +1233,14 @@
         "OutputValue": str,
         "Description": str,
         "ExportName": str,
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
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
     },
     total=False,
 )
@@ -1537,22 +1270,14 @@
         "Arn": str,
         "TypeName": str,
         "PublicVersionNumber": str,
     },
     total=False,
 )
 
-PublishTypeOutputTypeDef = TypedDict(
-    "PublishTypeOutputTypeDef",
-    {
-        "PublicTypeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecordHandlerProgressInputRequestTypeDef = TypedDict(
     "_RequiredRecordHandlerProgressInputRequestTypeDef",
     {
         "BearerToken": str,
         "OperationStatus": OperationStatusType,
     },
 )
@@ -1564,66 +1289,41 @@
         "ErrorCode": HandlerErrorCodeType,
         "ResourceModel": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class RecordHandlerProgressInputRequestTypeDef(
     _RequiredRecordHandlerProgressInputRequestTypeDef,
     _OptionalRecordHandlerProgressInputRequestTypeDef,
 ):
     pass
 
+
 RegisterPublisherInputRequestTypeDef = TypedDict(
     "RegisterPublisherInputRequestTypeDef",
     {
         "AcceptTermsAndConditions": bool,
         "ConnectionArn": str,
     },
     total=False,
 )
 
-RegisterPublisherOutputTypeDef = TypedDict(
-    "RegisterPublisherOutputTypeDef",
-    {
-        "PublisherId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterTypeOutputTypeDef = TypedDict(
-    "RegisterTypeOutputTypeDef",
-    {
-        "RegistrationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResourceTargetDefinitionTypeDef = TypedDict(
     "ResourceTargetDefinitionTypeDef",
     {
         "Attribute": ResourceAttributeType,
         "Name": str,
         "RequiresRecreation": RequiresRecreationType,
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
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
         "Type": str,
     },
 )
@@ -1639,26 +1339,20 @@
     {
         "RoleARN": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class RollbackStackInputRequestTypeDef(
     _RequiredRollbackStackInputRequestTypeDef, _OptionalRollbackStackInputRequestTypeDef
 ):
     pass
 
-RollbackStackOutputTypeDef = TypedDict(
-    "RollbackStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredSetStackPolicyInputRequestTypeDef = TypedDict(
     "_RequiredSetStackPolicyInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
@@ -1667,19 +1361,21 @@
     {
         "StackPolicyBody": str,
         "StackPolicyURL": str,
     },
     total=False,
 )
 
+
 class SetStackPolicyInputRequestTypeDef(
     _RequiredSetStackPolicyInputRequestTypeDef, _OptionalSetStackPolicyInputRequestTypeDef
 ):
     pass
 
+
 _RequiredSetTypeConfigurationInputRequestTypeDef = TypedDict(
     "_RequiredSetTypeConfigurationInputRequestTypeDef",
     {
         "Configuration": str,
     },
 )
 _OptionalSetTypeConfigurationInputRequestTypeDef = TypedDict(
@@ -1689,27 +1385,21 @@
         "ConfigurationAlias": str,
         "TypeName": str,
         "Type": ThirdPartyTypeType,
     },
     total=False,
 )
 
+
 class SetTypeConfigurationInputRequestTypeDef(
     _RequiredSetTypeConfigurationInputRequestTypeDef,
     _OptionalSetTypeConfigurationInputRequestTypeDef,
 ):
     pass
 
-SetTypeConfigurationOutputTypeDef = TypedDict(
-    "SetTypeConfigurationOutputTypeDef",
-    {
-        "ConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 SetTypeDefaultVersionInputRequestTypeDef = TypedDict(
     "SetTypeDefaultVersionInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
@@ -1724,61 +1414,56 @@
         "StackName": str,
         "LogicalResourceId": str,
         "UniqueId": str,
         "Status": ResourceSignalStatusType,
     },
 )
 
-StackDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackDriftInformationResponseMetadataTypeDef",
-    {
-        "StackDriftStatus": StackDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStackDriftInformationSummaryTypeDef = TypedDict(
     "_RequiredStackDriftInformationSummaryTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
     },
 )
 _OptionalStackDriftInformationSummaryTypeDef = TypedDict(
     "_OptionalStackDriftInformationSummaryTypeDef",
     {
         "LastCheckTimestamp": datetime,
     },
     total=False,
 )
 
+
 class StackDriftInformationSummaryTypeDef(
     _RequiredStackDriftInformationSummaryTypeDef, _OptionalStackDriftInformationSummaryTypeDef
 ):
     pass
 
+
 _RequiredStackDriftInformationTypeDef = TypedDict(
     "_RequiredStackDriftInformationTypeDef",
     {
         "StackDriftStatus": StackDriftStatusType,
     },
 )
 _OptionalStackDriftInformationTypeDef = TypedDict(
     "_OptionalStackDriftInformationTypeDef",
     {
         "LastCheckTimestamp": datetime,
     },
     total=False,
 )
 
+
 class StackDriftInformationTypeDef(
     _RequiredStackDriftInformationTypeDef, _OptionalStackDriftInformationTypeDef
 ):
     pass
 
+
 StackInstanceComprehensiveStatusTypeDef = TypedDict(
     "StackInstanceComprehensiveStatusTypeDef",
     {
         "DetailedStatus": StackInstanceDetailedStatusType,
     },
     total=False,
 )
@@ -1793,36 +1478,20 @@
     "_OptionalStackResourceDriftInformationTypeDef",
     {
         "LastCheckTimestamp": datetime,
     },
     total=False,
 )
 
+
 class StackResourceDriftInformationTypeDef(
     _RequiredStackResourceDriftInformationTypeDef, _OptionalStackResourceDriftInformationTypeDef
 ):
     pass
 
-StackResourceDriftInformationResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StackResourceDriftInformationSummaryResponseMetadataTypeDef = TypedDict(
-    "StackResourceDriftInformationSummaryResponseMetadataTypeDef",
-    {
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "LastCheckTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStackResourceDriftInformationSummaryTypeDef = TypedDict(
     "_RequiredStackResourceDriftInformationSummaryTypeDef",
     {
         "StackResourceDriftStatus": StackResourceDriftStatusType,
     },
 )
@@ -1830,20 +1499,22 @@
     "_OptionalStackResourceDriftInformationSummaryTypeDef",
     {
         "LastCheckTimestamp": datetime,
     },
     total=False,
 )
 
+
 class StackResourceDriftInformationSummaryTypeDef(
     _RequiredStackResourceDriftInformationSummaryTypeDef,
     _OptionalStackResourceDriftInformationSummaryTypeDef,
 ):
     pass
 
+
 StackSetDriftDetectionDetailsTypeDef = TypedDict(
     "StackSetDriftDetectionDetailsTypeDef",
     {
         "DriftStatus": StackSetDriftStatusType,
         "DriftDetectionStatus": StackSetDriftDetectionStatusType,
         "LastDriftCheckTimestamp": datetime,
         "TotalStackInstancesCount": int,
@@ -1851,14 +1522,27 @@
         "InSyncStackInstancesCount": int,
         "InProgressStackInstancesCount": int,
         "FailedStackInstancesCount": int,
     },
     total=False,
 )
 
+StackSetOperationPreferencesOutputTypeDef = TypedDict(
+    "StackSetOperationPreferencesOutputTypeDef",
+    {
+        "RegionConcurrencyType": RegionConcurrencyTypeType,
+        "RegionOrder": List[str],
+        "FailureToleranceCount": int,
+        "FailureTolerancePercentage": int,
+        "MaxConcurrentCount": int,
+        "MaxConcurrentPercentage": int,
+    },
+    total=False,
+)
+
 StackSetOperationStatusDetailsTypeDef = TypedDict(
     "StackSetOperationStatusDetailsTypeDef",
     {
         "FailedStackInstancesCount": int,
     },
     total=False,
 )
@@ -1874,20 +1558,22 @@
     "_OptionalStopStackSetOperationInputRequestTypeDef",
     {
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+
 class StopStackSetOperationInputRequestTypeDef(
     _RequiredStopStackSetOperationInputRequestTypeDef,
     _OptionalStopStackSetOperationInputRequestTypeDef,
 ):
     pass
 
+
 TemplateParameterTypeDef = TypedDict(
     "TemplateParameterTypeDef",
     {
         "ParameterKey": str,
         "DefaultValue": str,
         "NoEcho": bool,
         "Description": str,
@@ -1903,62 +1589,22 @@
         "TypeName": str,
         "VersionId": str,
         "LogDeliveryBucket": str,
     },
     total=False,
 )
 
-TestTypeOutputTypeDef = TypedDict(
-    "TestTypeOutputTypeDef",
-    {
-        "TypeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackInstancesOutputTypeDef = TypedDict(
-    "UpdateStackInstancesOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackOutputTypeDef = TypedDict(
-    "UpdateStackOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStackSetOutputTypeDef = TypedDict(
-    "UpdateStackSetOutputTypeDef",
-    {
-        "OperationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateTerminationProtectionInputRequestTypeDef = TypedDict(
     "UpdateTerminationProtectionInputRequestTypeDef",
     {
         "EnableTerminationProtection": bool,
         "StackName": str,
     },
 )
 
-UpdateTerminationProtectionOutputTypeDef = TypedDict(
-    "UpdateTerminationProtectionOutputTypeDef",
-    {
-        "StackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ValidateTemplateInputRequestTypeDef = TypedDict(
     "ValidateTemplateInputRequestTypeDef",
     {
         "TemplateBody": str,
         "TemplateURL": str,
     },
     total=False,
@@ -1973,23 +1619,14 @@
         "StatusReason": str,
         "AccountGateResult": AccountGateResultTypeDef,
         "OrganizationalUnitId": str,
     },
     total=False,
 )
 
-DescribeAccountLimitsOutputTypeDef = TypedDict(
-    "DescribeAccountLimitsOutputTypeDef",
-    {
-        "AccountLimits": List[AccountLimitTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActivateTypeInputRequestTypeDef = TypedDict(
     "ActivateTypeInputRequestTypeDef",
     {
         "Type": ThirdPartyTypeType,
         "PublicTypeArn": str,
         "PublisherId": str,
         "TypeName": str,
@@ -2017,19 +1654,313 @@
         "LoggingConfig": LoggingConfigTypeDef,
         "ExecutionRoleArn": str,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class RegisterTypeInputRequestTypeDef(
     _RequiredRegisterTypeInputRequestTypeDef, _OptionalRegisterTypeInputRequestTypeDef
 ):
     pass
 
+
+ActivateTypeOutputTypeDef = TypedDict(
+    "ActivateTypeOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChangeSetOutputTypeDef = TypedDict(
+    "CreateChangeSetOutputTypeDef",
+    {
+        "Id": str,
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackInstancesOutputTypeDef = TypedDict(
+    "CreateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackOutputTypeDef = TypedDict(
+    "CreateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStackSetOutputTypeDef = TypedDict(
+    "CreateStackSetOutputTypeDef",
+    {
+        "StackSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteStackInstancesOutputTypeDef = TypedDict(
+    "DeleteStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountLimitsOutputTypeDef = TypedDict(
+    "DescribeAccountLimitsOutputTypeDef",
+    {
+        "AccountLimits": List[AccountLimitTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationsAccessOutputTypeDef = TypedDict(
+    "DescribeOrganizationsAccessOutputTypeDef",
+    {
+        "Status": OrganizationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePublisherOutputTypeDef = TypedDict(
+    "DescribePublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "PublisherStatus": PublisherStatusType,
+        "IdentityProvider": IdentityProviderType,
+        "PublisherProfile": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStackDriftDetectionStatusOutputTypeDef = TypedDict(
+    "DescribeStackDriftDetectionStatusOutputTypeDef",
+    {
+        "StackId": str,
+        "StackDriftDetectionId": str,
+        "StackDriftStatus": StackDriftStatusType,
+        "DetectionStatus": StackDriftDetectionStatusType,
+        "DetectionStatusReason": str,
+        "DriftedStackResourceCount": int,
+        "Timestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTypeRegistrationOutputTypeDef = TypedDict(
+    "DescribeTypeRegistrationOutputTypeDef",
+    {
+        "ProgressStatus": RegistrationStatusType,
+        "Description": str,
+        "TypeArn": str,
+        "TypeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectStackDriftOutputTypeDef = TypedDict(
+    "DetectStackDriftOutputTypeDef",
+    {
+        "StackDriftDetectionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DetectStackSetDriftOutputTypeDef = TypedDict(
+    "DetectStackSetDriftOutputTypeDef",
+    {
+        "OperationId": str,
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
+EstimateTemplateCostOutputTypeDef = TypedDict(
+    "EstimateTemplateCostOutputTypeDef",
+    {
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetStackPolicyOutputTypeDef = TypedDict(
+    "GetStackPolicyOutputTypeDef",
+    {
+        "StackPolicyBody": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTemplateOutputTypeDef = TypedDict(
+    "GetTemplateOutputTypeDef",
+    {
+        "TemplateBody": Dict[str, Any],
+        "StagesAvailable": List["TemplateStageType"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportStacksToStackSetOutputTypeDef = TypedDict(
+    "ImportStacksToStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListImportsOutputTypeDef = TypedDict(
+    "ListImportsOutputTypeDef",
+    {
+        "Imports": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTypeRegistrationsOutputTypeDef = TypedDict(
+    "ListTypeRegistrationsOutputTypeDef",
+    {
+        "RegistrationTokenList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModuleInfoResponseTypeDef = TypedDict(
+    "ModuleInfoResponseTypeDef",
+    {
+        "TypeHierarchy": str,
+        "LogicalIdHierarchy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishTypeOutputTypeDef = TypedDict(
+    "PublishTypeOutputTypeDef",
+    {
+        "PublicTypeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterPublisherOutputTypeDef = TypedDict(
+    "RegisterPublisherOutputTypeDef",
+    {
+        "PublisherId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterTypeOutputTypeDef = TypedDict(
+    "RegisterTypeOutputTypeDef",
+    {
+        "RegistrationToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackStackOutputTypeDef = TypedDict(
+    "RollbackStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetTypeConfigurationOutputTypeDef = TypedDict(
+    "SetTypeConfigurationOutputTypeDef",
+    {
+        "ConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackDriftInformationResponseTypeDef = TypedDict(
+    "StackDriftInformationResponseTypeDef",
+    {
+        "StackDriftStatus": StackDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackResourceDriftInformationResponseTypeDef = TypedDict(
+    "StackResourceDriftInformationResponseTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StackResourceDriftInformationSummaryResponseTypeDef = TypedDict(
+    "StackResourceDriftInformationSummaryResponseTypeDef",
+    {
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "LastCheckTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestTypeOutputTypeDef = TypedDict(
+    "TestTypeOutputTypeDef",
+    {
+        "TypeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackInstancesOutputTypeDef = TypedDict(
+    "UpdateStackInstancesOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackOutputTypeDef = TypedDict(
+    "UpdateStackOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStackSetOutputTypeDef = TypedDict(
+    "UpdateStackSetOutputTypeDef",
+    {
+        "OperationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTerminationProtectionOutputTypeDef = TypedDict(
+    "UpdateTerminationProtectionOutputTypeDef",
+    {
+        "StackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchDescribeTypeConfigurationsErrorTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "TypeConfigurationIdentifier": TypeConfigurationIdentifierTypeDef,
     },
@@ -2053,15 +1984,15 @@
 )
 
 ListChangeSetsOutputTypeDef = TypedDict(
     "ListChangeSetsOutputTypeDef",
     {
         "Summaries": List[ChangeSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EstimateTemplateCostInputRequestTypeDef = TypedDict(
     "EstimateTemplateCostInputRequestTypeDef",
     {
         "TemplateBody": str,
@@ -2087,20 +2018,22 @@
         "OperationPreferences": StackSetOperationPreferencesTypeDef,
         "OperationId": str,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+
 class CreateStackInstancesInputRequestTypeDef(
     _RequiredCreateStackInstancesInputRequestTypeDef,
     _OptionalCreateStackInstancesInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStackInstancesInputRequestTypeDef = TypedDict(
     "_RequiredDeleteStackInstancesInputRequestTypeDef",
     {
         "StackSetName": str,
         "Regions": Sequence[str],
         "RetainStacks": bool,
     },
@@ -2113,20 +2046,22 @@
         "OperationPreferences": StackSetOperationPreferencesTypeDef,
         "OperationId": str,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+
 class DeleteStackInstancesInputRequestTypeDef(
     _RequiredDeleteStackInstancesInputRequestTypeDef,
     _OptionalDeleteStackInstancesInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDetectStackSetDriftInputRequestTypeDef = TypedDict(
     "_RequiredDetectStackSetDriftInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalDetectStackSetDriftInputRequestTypeDef = TypedDict(
@@ -2135,19 +2070,21 @@
         "OperationPreferences": StackSetOperationPreferencesTypeDef,
         "OperationId": str,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+
 class DetectStackSetDriftInputRequestTypeDef(
     _RequiredDetectStackSetDriftInputRequestTypeDef, _OptionalDetectStackSetDriftInputRequestTypeDef
 ):
     pass
 
+
 _RequiredImportStacksToStackSetInputRequestTypeDef = TypedDict(
     "_RequiredImportStacksToStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalImportStacksToStackSetInputRequestTypeDef = TypedDict(
@@ -2159,20 +2096,22 @@
         "OperationPreferences": StackSetOperationPreferencesTypeDef,
         "OperationId": str,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+
 class ImportStacksToStackSetInputRequestTypeDef(
     _RequiredImportStacksToStackSetInputRequestTypeDef,
     _OptionalImportStacksToStackSetInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateStackInstancesInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStackInstancesInputRequestTypeDef",
     {
         "StackSetName": str,
         "Regions": Sequence[str],
     },
 )
@@ -2185,20 +2124,22 @@
         "OperationPreferences": StackSetOperationPreferencesTypeDef,
         "OperationId": str,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+
 class UpdateStackInstancesInputRequestTypeDef(
     _RequiredUpdateStackInstancesInputRequestTypeDef,
     _OptionalUpdateStackInstancesInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateStackSetInputRequestTypeDef = TypedDict(
     "_RequiredCreateStackSetInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalCreateStackSetInputRequestTypeDef = TypedDict(
@@ -2218,19 +2159,21 @@
         "CallAs": CallAsType,
         "ClientRequestToken": str,
         "ManagedExecution": ManagedExecutionTypeDef,
     },
     total=False,
 )
 
+
 class CreateStackSetInputRequestTypeDef(
     _RequiredCreateStackSetInputRequestTypeDef, _OptionalCreateStackSetInputRequestTypeDef
 ):
     pass
 
+
 StackSetSummaryTypeDef = TypedDict(
     "StackSetSummaryTypeDef",
     {
         "StackSetName": str,
         "StackSetId": str,
         "Description": str,
         "Status": StackSetStatusType,
@@ -2270,19 +2213,187 @@
         "Regions": Sequence[str],
         "CallAs": CallAsType,
         "ManagedExecution": ManagedExecutionTypeDef,
     },
     total=False,
 )
 
+
 class UpdateStackSetInputRequestTypeDef(
     _RequiredUpdateStackSetInputRequestTypeDef, _OptionalUpdateStackSetInputRequestTypeDef
 ):
     pass
 
+
+DeploymentTargetsUnionTypeDef = Union[DeploymentTargetsTypeDef, DeploymentTargetsOutputTypeDef]
+DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
+    "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "ChangeSetName": str,
+    },
+)
+_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
+    "_OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeChangeSetInputDescribeChangeSetPaginateTypeDef(
+    _RequiredDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    _OptionalDescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+):
+    pass
+
+
+DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
+    "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeStacksInputDescribeStacksPaginateTypeDef = TypedDict(
+    "DescribeStacksInputDescribeStacksPaginateTypeDef",
+    {
+        "StackName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_RequiredListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef = TypedDict(
+    "_OptionalListChangeSetsInputListChangeSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListChangeSetsInputListChangeSetsPaginateTypeDef(
+    _RequiredListChangeSetsInputListChangeSetsPaginateTypeDef,
+    _OptionalListChangeSetsInputListChangeSetsPaginateTypeDef,
+):
+    pass
+
+
+ListExportsInputListExportsPaginateTypeDef = TypedDict(
+    "ListExportsInputListExportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_RequiredListImportsInputListImportsPaginateTypeDef",
+    {
+        "ExportName": str,
+    },
+)
+_OptionalListImportsInputListImportsPaginateTypeDef = TypedDict(
+    "_OptionalListImportsInputListImportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListImportsInputListImportsPaginateTypeDef(
+    _RequiredListImportsInputListImportsPaginateTypeDef,
+    _OptionalListImportsInputListImportsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "StackName": str,
+    },
+)
+_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListStackResourcesInputListStackResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStackResourcesInputListStackResourcesPaginateTypeDef(
+    _RequiredListStackResourcesInputListStackResourcesPaginateTypeDef,
+    _OptionalListStackResourcesInputListStackResourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "StackSetName": str,
+    },
+)
+_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef = TypedDict(
+    "_OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef",
+    {
+        "CallAs": CallAsType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef(
+    _RequiredListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    _OptionalListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+):
+    pass
+
+
+ListStackSetsInputListStackSetsPaginateTypeDef = TypedDict(
+    "ListStackSetsInputListStackSetsPaginateTypeDef",
+    {
+        "Status": StackSetStatusType,
+        "CallAs": CallAsType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListStacksInputListStacksPaginateTypeDef = TypedDict(
+    "ListStacksInputListStacksPaginateTypeDef",
+    {
+        "StackStatusFilter": Sequence[StackStatusType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     {
         "ChangeSetName": str,
     },
 )
 _OptionalDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
@@ -2291,20 +2402,22 @@
         "StackName": str,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef(
     _RequiredDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     _OptionalDescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
 ):
     pass
 
+
 DescribeStacksInputStackCreateCompleteWaitTypeDef = TypedDict(
     "DescribeStacksInputStackCreateCompleteWaitTypeDef",
     {
         "StackName": str,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
@@ -2371,26 +2484,28 @@
     "_OptionalDescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef(
     _RequiredDescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef,
     _OptionalDescribeTypeRegistrationInputTypeRegistrationCompleteWaitTypeDef,
 ):
     pass
 
+
 DescribeStackEventsOutputTypeDef = TypedDict(
     "DescribeStackEventsOutputTypeDef",
     {
         "StackEvents": List[StackEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTypeOutputTypeDef = TypedDict(
     "DescribeTypeOutputTypeDef",
     {
         "Arn": str,
@@ -2416,24 +2531,24 @@
         "PublisherId": str,
         "OriginalTypeName": str,
         "OriginalTypeArn": str,
         "PublicVersionNumber": str,
         "LatestPublicVersion": str,
         "IsActivated": bool,
         "AutoUpdate": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExportsOutputTypeDef = TypedDict(
     "ListExportsOutputTypeDef",
     {
         "Exports": List[ExportTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_RequiredListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "StackSetName": str,
@@ -2442,25 +2557,27 @@
 _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef = TypedDict(
     "_OptionalListStackInstancesInputListStackInstancesPaginateTypeDef",
     {
         "Filters": Sequence[StackInstanceFilterTypeDef],
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "CallAs": CallAsType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListStackInstancesInputListStackInstancesPaginateTypeDef(
     _RequiredListStackInstancesInputListStackInstancesPaginateTypeDef,
     _OptionalListStackInstancesInputListStackInstancesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListStackInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListStackInstancesInputRequestTypeDef",
     {
         "StackSetName": str,
     },
 )
 _OptionalListStackInstancesInputRequestTypeDef = TypedDict(
@@ -2472,42 +2589,46 @@
         "StackInstanceAccount": str,
         "StackInstanceRegion": str,
         "CallAs": CallAsType,
     },
     total=False,
 )
 
+
 class ListStackInstancesInputRequestTypeDef(
     _RequiredListStackInstancesInputRequestTypeDef, _OptionalListStackInstancesInputRequestTypeDef
 ):
     pass
 
+
 _RequiredListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef = TypedDict(
     "_RequiredListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     {
         "StackSetName": str,
         "OperationId": str,
     },
 )
 _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef = TypedDict(
     "_OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     {
         "CallAs": CallAsType,
         "Filters": Sequence[OperationResultFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef(
     _RequiredListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
     _OptionalListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListStackSetOperationResultsInputRequestTypeDef = TypedDict(
     "_RequiredListStackSetOperationResultsInputRequestTypeDef",
     {
         "StackSetName": str,
         "OperationId": str,
     },
 )
@@ -2518,38 +2639,40 @@
         "MaxResults": int,
         "CallAs": CallAsType,
         "Filters": Sequence[OperationResultFilterTypeDef],
     },
     total=False,
 )
 
+
 class ListStackSetOperationResultsInputRequestTypeDef(
     _RequiredListStackSetOperationResultsInputRequestTypeDef,
     _OptionalListStackSetOperationResultsInputRequestTypeDef,
 ):
     pass
 
+
 ListTypeVersionsOutputTypeDef = TypedDict(
     "ListTypeVersionsOutputTypeDef",
     {
         "TypeVersionSummaries": List[TypeVersionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTypesInputListTypesPaginateTypeDef = TypedDict(
     "ListTypesInputListTypesPaginateTypeDef",
     {
         "Visibility": VisibilityType,
         "ProvisioningType": ProvisioningTypeType,
         "DeprecatedStatus": DeprecatedStatusType,
         "Type": RegistryTypeType,
         "Filters": TypeFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListTypesInputRequestTypeDef = TypedDict(
     "ListTypesInputRequestTypeDef",
     {
@@ -2565,15 +2688,15 @@
 )
 
 ListTypesOutputTypeDef = TypedDict(
     "ListTypesOutputTypeDef",
     {
         "TypeSummaries": List[TypeSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ParameterDeclarationTypeDef = TypedDict(
     "ParameterDeclarationTypeDef",
     {
         "ParameterKey": str,
@@ -2605,46 +2728,48 @@
         "ActualProperties": str,
         "PropertyDifferences": List[PropertyDifferenceTypeDef],
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
+
 class StackResourceDriftTypeDef(
     _RequiredStackResourceDriftTypeDef, _OptionalStackResourceDriftTypeDef
 ):
     pass
 
+
 ResourceChangeDetailTypeDef = TypedDict(
     "ResourceChangeDetailTypeDef",
     {
         "Target": ResourceTargetDefinitionTypeDef,
         "Evaluation": EvaluationTypeType,
         "ChangeSource": ChangeSourceType,
         "CausingEntity": str,
     },
     total=False,
 )
 
-RollbackConfigurationResponseMetadataTypeDef = TypedDict(
-    "RollbackConfigurationResponseMetadataTypeDef",
+RollbackConfigurationOutputTypeDef = TypedDict(
+    "RollbackConfigurationOutputTypeDef",
     {
         "RollbackTriggers": List[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
-        "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
+        "RollbackTriggers": List[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredStackSummaryTypeDef = TypedDict(
     "_RequiredStackSummaryTypeDef",
     {
         "StackName": str,
         "CreationTime": datetime,
@@ -2662,17 +2787,19 @@
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationSummaryTypeDef,
     },
     total=False,
 )
 
+
 class StackSummaryTypeDef(_RequiredStackSummaryTypeDef, _OptionalStackSummaryTypeDef):
     pass
 
+
 StackInstanceSummaryTypeDef = TypedDict(
     "StackInstanceSummaryTypeDef",
     {
         "StackSetId": str,
         "Region": str,
         "Account": str,
         "StackId": str,
@@ -2726,19 +2853,21 @@
         "Metadata": str,
         "DriftInformation": StackResourceDriftInformationTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
+
 class StackResourceDetailTypeDef(
     _RequiredStackResourceDetailTypeDef, _OptionalStackResourceDetailTypeDef
 ):
     pass
 
+
 _RequiredStackResourceTypeDef = TypedDict(
     "_RequiredStackResourceTypeDef",
     {
         "LogicalResourceId": str,
         "ResourceType": str,
         "Timestamp": datetime,
         "ResourceStatus": ResourceStatusType,
@@ -2754,17 +2883,19 @@
         "Description": str,
         "DriftInformation": StackResourceDriftInformationTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
+
 class StackResourceTypeDef(_RequiredStackResourceTypeDef, _OptionalStackResourceTypeDef):
     pass
 
+
 _RequiredStackResourceSummaryTypeDef = TypedDict(
     "_RequiredStackResourceSummaryTypeDef",
     {
         "LogicalResourceId": str,
         "ResourceType": str,
         "LastUpdatedTimestamp": datetime,
         "ResourceStatus": ResourceStatusType,
@@ -2777,19 +2908,21 @@
         "ResourceStatusReason": str,
         "DriftInformation": StackResourceDriftInformationSummaryTypeDef,
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
+
 class StackResourceSummaryTypeDef(
     _RequiredStackResourceSummaryTypeDef, _OptionalStackResourceSummaryTypeDef
 ):
     pass
 
+
 StackSetTypeDef = TypedDict(
     "StackSetTypeDef",
     {
         "StackSetName": str,
         "StackSetId": str,
         "Description": str,
         "Status": StackSetStatusType,
@@ -2806,43 +2939,46 @@
         "OrganizationalUnitIds": List[str],
         "ManagedExecution": ManagedExecutionTypeDef,
         "Regions": List[str],
     },
     total=False,
 )
 
+StackSetOperationPreferencesUnionTypeDef = Union[
+    StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
+]
 StackSetOperationSummaryTypeDef = TypedDict(
     "StackSetOperationSummaryTypeDef",
     {
         "OperationId": str,
         "Action": StackSetOperationActionType,
         "Status": StackSetOperationStatusType,
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
-        "OperationPreferences": StackSetOperationPreferencesTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
     },
     total=False,
 )
 
 StackSetOperationTypeDef = TypedDict(
     "StackSetOperationTypeDef",
     {
         "OperationId": str,
         "StackSetId": str,
         "Action": StackSetOperationActionType,
         "Status": StackSetOperationStatusType,
-        "OperationPreferences": StackSetOperationPreferencesTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
         "RetainStacks": bool,
         "AdministrationRoleARN": str,
         "ExecutionRoleName": str,
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
-        "DeploymentTargets": DeploymentTargetsTypeDef,
+        "DeploymentTargets": DeploymentTargetsOutputTypeDef,
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
     },
     total=False,
 )
 
@@ -2850,34 +2986,34 @@
     "ValidateTemplateOutputTypeDef",
     {
         "Parameters": List[TemplateParameterTypeDef],
         "Description": str,
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "DeclaredTransforms": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackSetOperationResultsOutputTypeDef = TypedDict(
     "ListStackSetOperationResultsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationResultSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDescribeTypeConfigurationsOutputTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     {
         "Errors": List[BatchDescribeTypeConfigurationsErrorTypeDef],
         "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierTypeDef],
         "TypeConfigurations": List[TypeConfigurationDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeSetHookTypeDef = TypedDict(
     "ChangeSetHookTypeDef",
     {
         "InvocationPoint": Literal["PRE_PROVISION"],
@@ -2891,15 +3027,15 @@
 )
 
 ListStackSetsOutputTypeDef = TypedDict(
     "ListStackSetsOutputTypeDef",
     {
         "Summaries": List[StackSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTemplateSummaryOutputTypeDef = TypedDict(
     "GetTemplateSummaryOutputTypeDef",
     {
         "Parameters": List[ParameterDeclarationTypeDef],
@@ -2907,32 +3043,32 @@
         "Capabilities": List[CapabilityType],
         "CapabilitiesReason": str,
         "ResourceTypes": List[str],
         "Version": str,
         "Metadata": str,
         "DeclaredTransforms": List[str],
         "ResourceIdentifierSummaries": List[ResourceIdentifierSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourceDriftsOutputTypeDef = TypedDict(
     "DescribeStackResourceDriftsOutputTypeDef",
     {
         "StackResourceDrifts": List[StackResourceDriftTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectStackResourceDriftOutputTypeDef = TypedDict(
     "DetectStackResourceDriftOutputTypeDef",
     {
         "StackResourceDrift": StackResourceDriftTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
@@ -2944,14 +3080,53 @@
         "Details": List[ResourceChangeDetailTypeDef],
         "ChangeSetId": str,
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
+_RequiredStackTypeDef = TypedDict(
+    "_RequiredStackTypeDef",
+    {
+        "StackName": str,
+        "CreationTime": datetime,
+        "StackStatus": StackStatusType,
+    },
+)
+_OptionalStackTypeDef = TypedDict(
+    "_OptionalStackTypeDef",
+    {
+        "StackId": str,
+        "ChangeSetId": str,
+        "Description": str,
+        "Parameters": List[ParameterTypeDef],
+        "DeletionTime": datetime,
+        "LastUpdatedTime": datetime,
+        "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
+        "StackStatusReason": str,
+        "DisableRollback": bool,
+        "NotificationARNs": List[str],
+        "TimeoutInMinutes": int,
+        "Capabilities": List[CapabilityType],
+        "Outputs": List[OutputTypeDef],
+        "RoleARN": str,
+        "Tags": List[TagTypeDef],
+        "EnableTerminationProtection": bool,
+        "ParentId": str,
+        "RootId": str,
+        "DriftInformation": StackDriftInformationTypeDef,
+    },
+    total=False,
+)
+
+
+class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
+    pass
+
+
 _RequiredCreateChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredCreateChangeSetInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
     },
 )
@@ -2974,19 +3149,21 @@
         "ResourcesToImport": Sequence[ResourceToImportTypeDef],
         "IncludeNestedStacks": bool,
         "OnStackFailure": OnStackFailureType,
     },
     total=False,
 )
 
+
 class CreateChangeSetInputRequestTypeDef(
     _RequiredCreateChangeSetInputRequestTypeDef, _OptionalCreateChangeSetInputRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateStackInputRequestTypeDef = TypedDict(
     "_RequiredCreateStackInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalCreateStackInputRequestTypeDef = TypedDict(
@@ -3008,19 +3185,21 @@
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "EnableTerminationProtection": bool,
     },
     total=False,
 )
 
+
 class CreateStackInputRequestTypeDef(
     _RequiredCreateStackInputRequestTypeDef, _OptionalCreateStackInputRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateStackInputServiceResourceCreateStackTypeDef = TypedDict(
     "_RequiredCreateStackInputServiceResourceCreateStackTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalCreateStackInputServiceResourceCreateStackTypeDef = TypedDict(
@@ -3042,57 +3221,25 @@
         "Tags": Sequence[TagTypeDef],
         "ClientRequestToken": str,
         "EnableTerminationProtection": bool,
     },
     total=False,
 )
 
+
 class CreateStackInputServiceResourceCreateStackTypeDef(
     _RequiredCreateStackInputServiceResourceCreateStackTypeDef,
     _OptionalCreateStackInputServiceResourceCreateStackTypeDef,
 ):
     pass
 
-_RequiredStackTypeDef = TypedDict(
-    "_RequiredStackTypeDef",
-    {
-        "StackName": str,
-        "CreationTime": datetime,
-        "StackStatus": StackStatusType,
-    },
-)
-_OptionalStackTypeDef = TypedDict(
-    "_OptionalStackTypeDef",
-    {
-        "StackId": str,
-        "ChangeSetId": str,
-        "Description": str,
-        "Parameters": List[ParameterTypeDef],
-        "DeletionTime": datetime,
-        "LastUpdatedTime": datetime,
-        "RollbackConfiguration": RollbackConfigurationTypeDef,
-        "StackStatusReason": str,
-        "DisableRollback": bool,
-        "NotificationARNs": List[str],
-        "TimeoutInMinutes": int,
-        "Capabilities": List[CapabilityType],
-        "Outputs": List[OutputTypeDef],
-        "RoleARN": str,
-        "Tags": List[TagTypeDef],
-        "EnableTerminationProtection": bool,
-        "ParentId": str,
-        "RootId": str,
-        "DriftInformation": StackDriftInformationTypeDef,
-    },
-    total=False,
-)
-
-class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
-    pass
 
+RollbackConfigurationUnionTypeDef = Union[
+    RollbackConfigurationTypeDef, RollbackConfigurationOutputTypeDef
+]
 _RequiredUpdateStackInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStackInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalUpdateStackInputRequestTypeDef = TypedDict(
@@ -3114,19 +3261,21 @@
         "Tags": Sequence[TagTypeDef],
         "DisableRollback": bool,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class UpdateStackInputRequestTypeDef(
     _RequiredUpdateStackInputRequestTypeDef, _OptionalUpdateStackInputRequestTypeDef
 ):
     pass
 
+
 UpdateStackInputStackUpdateTypeDef = TypedDict(
     "UpdateStackInputStackUpdateTypeDef",
     {
         "TemplateBody": str,
         "TemplateURL": str,
         "UsePreviousTemplate": bool,
         "StackPolicyDuringUpdateBody": str,
@@ -3147,96 +3296,96 @@
 )
 
 ListStacksOutputTypeDef = TypedDict(
     "ListStacksOutputTypeDef",
     {
         "StackSummaries": List[StackSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackInstancesOutputTypeDef = TypedDict(
     "ListStackInstancesOutputTypeDef",
     {
         "Summaries": List[StackInstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackInstanceOutputTypeDef = TypedDict(
     "DescribeStackInstanceOutputTypeDef",
     {
         "StackInstance": StackInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourceOutputTypeDef = TypedDict(
     "DescribeStackResourceOutputTypeDef",
     {
         "StackResourceDetail": StackResourceDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackResourcesOutputTypeDef = TypedDict(
     "DescribeStackResourcesOutputTypeDef",
     {
         "StackResources": List[StackResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackResourcesOutputTypeDef = TypedDict(
     "ListStackResourcesOutputTypeDef",
     {
         "StackResourceSummaries": List[StackResourceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSetOutputTypeDef = TypedDict(
     "DescribeStackSetOutputTypeDef",
     {
         "StackSet": StackSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStackSetOperationsOutputTypeDef = TypedDict(
     "ListStackSetOperationsOutputTypeDef",
     {
         "Summaries": List[StackSetOperationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStackSetOperationOutputTypeDef = TypedDict(
     "DescribeStackSetOperationOutputTypeDef",
     {
         "StackSetOperation": StackSetOperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetHooksOutputTypeDef = TypedDict(
     "DescribeChangeSetHooksOutputTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetName": str,
         "Hooks": List[ChangeSetHookTypeDef],
         "Status": ChangeSetHooksStatusType,
         "NextToken": str,
         "StackId": str,
         "StackName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeTypeDef = TypedDict(
     "ChangeTypeDef",
     {
         "Type": Literal["Resource"],
@@ -3247,15 +3396,15 @@
 )
 
 DescribeStacksOutputTypeDef = TypedDict(
     "DescribeStacksOutputTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetOutputTypeDef = TypedDict(
     "DescribeChangeSetOutputTypeDef",
     {
         "ChangeSetName": str,
@@ -3265,19 +3414,19 @@
         "Description": str,
         "Parameters": List[ParameterTypeDef],
         "CreationTime": datetime,
         "ExecutionStatus": ExecutionStatusType,
         "Status": ChangeSetStatusType,
         "StatusReason": str,
         "NotificationARNs": List[str],
-        "RollbackConfiguration": RollbackConfigurationTypeDef,
+        "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
         "Capabilities": List[CapabilityType],
         "Tags": List[TagTypeDef],
         "Changes": List[ChangeTypeDef],
         "NextToken": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
         "OnStackFailure": OnStackFailureType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/waiter.py` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation/waiter.pyi` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation.egg-info/PKG-INFO` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudformation
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudFormation 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudFormation 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudformation type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudformation type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudformation"></a>
 
 # types-aiobotocore-cloudformation
 
 [![PyPI - types-aiobotocore-cloudformation](https://img.shields.io/pypi/v/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudformation.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudformation?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudformation)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudformation)](https://pepy.tech/project/types-aiobotocore-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudFormation 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
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
 [types-aiobotocore-cloudformation docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +77,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -550,177 +549,180 @@
 )
 
 
 def check_value(value: AccountFilterTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudformation.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudformation.type_defs import (
     AccountGateResultTypeDef,
     AccountLimitTypeDef,
     LoggingConfigTypeDef,
-    ActivateTypeOutputTypeDef,
+    ResponseMetadataTypeDef,
     AutoDeploymentTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeConfigurationDetailsTypeDef,
     CancelUpdateStackInputRequestTypeDef,
     CancelUpdateStackInputStackCancelUpdateTypeDef,
     ChangeSetHookResourceTargetDetailsTypeDef,
     ChangeSetSummaryTypeDef,
     ContinueUpdateRollbackInputRequestTypeDef,
     ParameterTypeDef,
     ResourceToImportTypeDef,
     TagTypeDef,
-    CreateChangeSetOutputTypeDef,
     DeploymentTargetsTypeDef,
     StackSetOperationPreferencesTypeDef,
-    CreateStackInstancesOutputTypeDef,
-    CreateStackOutputTypeDef,
     ManagedExecutionTypeDef,
-    CreateStackSetOutputTypeDef,
     DeactivateTypeInputRequestTypeDef,
     DeleteChangeSetInputRequestTypeDef,
     DeleteStackInputRequestTypeDef,
     DeleteStackInputStackDeleteTypeDef,
-    DeleteStackInstancesOutputTypeDef,
     DeleteStackSetInputRequestTypeDef,
+    DeploymentTargetsOutputTypeDef,
     DeregisterTypeInputRequestTypeDef,
-    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAccountLimitsInputRequestTypeDef,
     DescribeChangeSetHooksInputRequestTypeDef,
     WaiterConfigTypeDef,
-    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
     DescribeChangeSetInputRequestTypeDef,
     DescribeOrganizationsAccessInputRequestTypeDef,
-    DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherInputRequestTypeDef,
-    DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusInputRequestTypeDef,
-    DescribeStackDriftDetectionStatusOutputTypeDef,
-    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
     DescribeStackEventsInputRequestTypeDef,
     StackEventTypeDef,
     DescribeStackInstanceInputRequestTypeDef,
     DescribeStackResourceDriftsInputRequestTypeDef,
     DescribeStackResourceInputRequestTypeDef,
     DescribeStackResourcesInputRequestTypeDef,
     DescribeStackSetInputRequestTypeDef,
     DescribeStackSetOperationInputRequestTypeDef,
-    DescribeStacksInputDescribeStacksPaginateTypeDef,
     DescribeStacksInputRequestTypeDef,
     DescribeTypeInputRequestTypeDef,
     RequiredActivatedTypeTypeDef,
     DescribeTypeRegistrationInputRequestTypeDef,
-    DescribeTypeRegistrationOutputTypeDef,
     DetectStackDriftInputRequestTypeDef,
-    DetectStackDriftOutputTypeDef,
     DetectStackResourceDriftInputRequestTypeDef,
-    DetectStackSetDriftOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EstimateTemplateCostOutputTypeDef,
     ExecuteChangeSetInputRequestTypeDef,
     ExportTypeDef,
     GetStackPolicyInputRequestTypeDef,
-    GetStackPolicyOutputTypeDef,
     GetTemplateInputRequestTypeDef,
-    GetTemplateOutputTypeDef,
     GetTemplateSummaryInputRequestTypeDef,
     ResourceIdentifierSummaryTypeDef,
-    ImportStacksToStackSetOutputTypeDef,
-    ListChangeSetsInputListChangeSetsPaginateTypeDef,
     ListChangeSetsInputRequestTypeDef,
-    ListExportsInputListExportsPaginateTypeDef,
     ListExportsInputRequestTypeDef,
-    ListImportsInputListImportsPaginateTypeDef,
     ListImportsInputRequestTypeDef,
-    ListImportsOutputTypeDef,
     StackInstanceFilterTypeDef,
-    ListStackResourcesInputListStackResourcesPaginateTypeDef,
     ListStackResourcesInputRequestTypeDef,
     OperationResultFilterTypeDef,
-    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
     ListStackSetOperationsInputRequestTypeDef,
-    ListStackSetsInputListStackSetsPaginateTypeDef,
     ListStackSetsInputRequestTypeDef,
-    ListStacksInputListStacksPaginateTypeDef,
     ListStacksInputRequestTypeDef,
     ListTypeRegistrationsInputRequestTypeDef,
-    ListTypeRegistrationsOutputTypeDef,
     ListTypeVersionsInputRequestTypeDef,
     TypeVersionSummaryTypeDef,
     TypeFiltersTypeDef,
     TypeSummaryTypeDef,
-    ModuleInfoResponseMetadataTypeDef,
     ModuleInfoTypeDef,
     OutputTypeDef,
-    PaginatorConfigTypeDef,
     ParameterConstraintsTypeDef,
     PhysicalResourceIdContextKeyValuePairTypeDef,
     PropertyDifferenceTypeDef,
     PublishTypeInputRequestTypeDef,
-    PublishTypeOutputTypeDef,
     RecordHandlerProgressInputRequestTypeDef,
     RegisterPublisherInputRequestTypeDef,
-    RegisterPublisherOutputTypeDef,
-    RegisterTypeOutputTypeDef,
     ResourceTargetDefinitionTypeDef,
-    ResponseMetadataTypeDef,
     RollbackTriggerTypeDef,
     RollbackStackInputRequestTypeDef,
-    RollbackStackOutputTypeDef,
     SetStackPolicyInputRequestTypeDef,
     SetTypeConfigurationInputRequestTypeDef,
-    SetTypeConfigurationOutputTypeDef,
     SetTypeDefaultVersionInputRequestTypeDef,
     SignalResourceInputRequestTypeDef,
-    StackDriftInformationResponseMetadataTypeDef,
     StackDriftInformationSummaryTypeDef,
     StackDriftInformationTypeDef,
     StackInstanceComprehensiveStatusTypeDef,
     StackResourceDriftInformationTypeDef,
-    StackResourceDriftInformationResponseMetadataTypeDef,
-    StackResourceDriftInformationSummaryResponseMetadataTypeDef,
     StackResourceDriftInformationSummaryTypeDef,
     StackSetDriftDetectionDetailsTypeDef,
+    StackSetOperationPreferencesOutputTypeDef,
     StackSetOperationStatusDetailsTypeDef,
     StopStackSetOperationInputRequestTypeDef,
     TemplateParameterTypeDef,
     TestTypeInputRequestTypeDef,
-    TestTypeOutputTypeDef,
-    UpdateStackInstancesOutputTypeDef,
-    UpdateStackOutputTypeDef,
-    UpdateStackSetOutputTypeDef,
     UpdateTerminationProtectionInputRequestTypeDef,
-    UpdateTerminationProtectionOutputTypeDef,
     ValidateTemplateInputRequestTypeDef,
     StackSetOperationResultSummaryTypeDef,
-    DescribeAccountLimitsOutputTypeDef,
     ActivateTypeInputRequestTypeDef,
     RegisterTypeInputRequestTypeDef,
+    ActivateTypeOutputTypeDef,
+    CreateChangeSetOutputTypeDef,
+    CreateStackInstancesOutputTypeDef,
+    CreateStackOutputTypeDef,
+    CreateStackSetOutputTypeDef,
+    DeleteStackInstancesOutputTypeDef,
+    DescribeAccountLimitsOutputTypeDef,
+    DescribeOrganizationsAccessOutputTypeDef,
+    DescribePublisherOutputTypeDef,
+    DescribeStackDriftDetectionStatusOutputTypeDef,
+    DescribeTypeRegistrationOutputTypeDef,
+    DetectStackDriftOutputTypeDef,
+    DetectStackSetDriftOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EstimateTemplateCostOutputTypeDef,
+    GetStackPolicyOutputTypeDef,
+    GetTemplateOutputTypeDef,
+    ImportStacksToStackSetOutputTypeDef,
+    ListImportsOutputTypeDef,
+    ListTypeRegistrationsOutputTypeDef,
+    ModuleInfoResponseTypeDef,
+    PublishTypeOutputTypeDef,
+    RegisterPublisherOutputTypeDef,
+    RegisterTypeOutputTypeDef,
+    RollbackStackOutputTypeDef,
+    SetTypeConfigurationOutputTypeDef,
+    StackDriftInformationResponseTypeDef,
+    StackResourceDriftInformationResponseTypeDef,
+    StackResourceDriftInformationSummaryResponseTypeDef,
+    TestTypeOutputTypeDef,
+    UpdateStackInstancesOutputTypeDef,
+    UpdateStackOutputTypeDef,
+    UpdateStackSetOutputTypeDef,
+    UpdateTerminationProtectionOutputTypeDef,
     BatchDescribeTypeConfigurationsErrorTypeDef,
     BatchDescribeTypeConfigurationsInputRequestTypeDef,
     ChangeSetHookTargetDetailsTypeDef,
     ListChangeSetsOutputTypeDef,
     EstimateTemplateCostInputRequestTypeDef,
     CreateStackInstancesInputRequestTypeDef,
     DeleteStackInstancesInputRequestTypeDef,
     DetectStackSetDriftInputRequestTypeDef,
     ImportStacksToStackSetInputRequestTypeDef,
     UpdateStackInstancesInputRequestTypeDef,
     CreateStackSetInputRequestTypeDef,
     StackSetSummaryTypeDef,
     UpdateStackSetInputRequestTypeDef,
+    DeploymentTargetsUnionTypeDef,
+    DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef,
+    DescribeChangeSetInputDescribeChangeSetPaginateTypeDef,
+    DescribeStackEventsInputDescribeStackEventsPaginateTypeDef,
+    DescribeStacksInputDescribeStacksPaginateTypeDef,
+    ListChangeSetsInputListChangeSetsPaginateTypeDef,
+    ListExportsInputListExportsPaginateTypeDef,
+    ListImportsInputListImportsPaginateTypeDef,
+    ListStackResourcesInputListStackResourcesPaginateTypeDef,
+    ListStackSetOperationsInputListStackSetOperationsPaginateTypeDef,
+    ListStackSetsInputListStackSetsPaginateTypeDef,
+    ListStacksInputListStacksPaginateTypeDef,
     DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef,
     DescribeStacksInputStackCreateCompleteWaitTypeDef,
     DescribeStacksInputStackDeleteCompleteWaitTypeDef,
     DescribeStacksInputStackExistsWaitTypeDef,
     DescribeStacksInputStackImportCompleteWaitTypeDef,
     DescribeStacksInputStackRollbackCompleteWaitTypeDef,
     DescribeStacksInputStackUpdateCompleteWaitTypeDef,
@@ -735,38 +737,40 @@
     ListTypeVersionsOutputTypeDef,
     ListTypesInputListTypesPaginateTypeDef,
     ListTypesInputRequestTypeDef,
     ListTypesOutputTypeDef,
     ParameterDeclarationTypeDef,
     StackResourceDriftTypeDef,
     ResourceChangeDetailTypeDef,
-    RollbackConfigurationResponseMetadataTypeDef,
+    RollbackConfigurationOutputTypeDef,
     RollbackConfigurationTypeDef,
     StackSummaryTypeDef,
     StackInstanceSummaryTypeDef,
     StackInstanceTypeDef,
     StackResourceDetailTypeDef,
     StackResourceTypeDef,
     StackResourceSummaryTypeDef,
     StackSetTypeDef,
+    StackSetOperationPreferencesUnionTypeDef,
     StackSetOperationSummaryTypeDef,
     StackSetOperationTypeDef,
     ValidateTemplateOutputTypeDef,
     ListStackSetOperationResultsOutputTypeDef,
     BatchDescribeTypeConfigurationsOutputTypeDef,
     ChangeSetHookTypeDef,
     ListStackSetsOutputTypeDef,
     GetTemplateSummaryOutputTypeDef,
     DescribeStackResourceDriftsOutputTypeDef,
     DetectStackResourceDriftOutputTypeDef,
     ResourceChangeTypeDef,
+    StackTypeDef,
     CreateChangeSetInputRequestTypeDef,
     CreateStackInputRequestTypeDef,
     CreateStackInputServiceResourceCreateStackTypeDef,
-    StackTypeDef,
+    RollbackConfigurationUnionTypeDef,
     UpdateStackInputRequestTypeDef,
     UpdateStackInputStackUpdateTypeDef,
     ListStacksOutputTypeDef,
     ListStackInstancesOutputTypeDef,
     DescribeStackInstanceOutputTypeDef,
     DescribeStackResourceOutputTypeDef,
     DescribeStackResourcesOutputTypeDef,
@@ -777,15 +781,15 @@
     DescribeChangeSetHooksOutputTypeDef,
     ChangeTypeDef,
     DescribeStacksOutputTypeDef,
     DescribeChangeSetOutputTypeDef,
 )
 
 
-def get_structure() -> AccountGateResultTypeDef:
+def get_value() -> AccountGateResultTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudformation-2.5.2/types_aiobotocore_cloudformation.egg-info/SOURCES.txt` & `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-codepipeline-2.5.2.tar.gz` & `tmp/types-aiobotocore-codepipeline-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codepipeline-2.5.2.tar", last modified: Sat Jul  8 01:43:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-codepipeline-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:04 2023, max compression
```

## Comparing `types-aiobotocore-codepipeline-2.5.2.tar` & `types-aiobotocore-codepipeline-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:25.101893 types-aiobotocore-codepipeline-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19520 2023-07-08 01:43:25.093893 types-aiobotocore-codepipeline-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:25.101893 types-aiobotocore-codepipeline-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:25.093893 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34324 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46263 2023-07-08 01:27:40.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46202 2023-07-08 01:27:39.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:38.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:25.093893 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19520 2023-07-08 01:43:24.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:24.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:24.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:24.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:24.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:24.000000 types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.677619 types-aiobotocore-codepipeline-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20005 2023-08-02 14:52:04.677619 types-aiobotocore-codepipeline-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18467 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.677619 types-aiobotocore-codepipeline-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:35:11.000000 types-aiobotocore-codepipeline-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.673619 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34423 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34369 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51697 2023-08-02 14:35:14.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51626 2023-08-02 14:35:13.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.677619 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20005 2023-08-02 14:52:04.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:04.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:04.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codepipeline-2.5.2/LICENSE` & `types-aiobotocore-codepipeline-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.2/PKG-INFO` & `types-aiobotocore-codepipeline-2.5.2.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codepipeline
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodePipeline 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodePipeline 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codepipeline type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codepipeline type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codepipeline"></a>
 
 # types-aiobotocore-codepipeline
 
 [![PyPI - types-aiobotocore-codepipeline](https://img.shields.io/pypi/v/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codepipeline?color=blue)](https://pypistats.org/packages/types-aiobotocore-codepipeline)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codepipeline)](https://pepy.tech/project/types-aiobotocore-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodePipeline 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [types-aiobotocore-codepipeline docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/).
 
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
@@ -348,168 +347,183 @@
 )
 
 
 def check_value(value: ActionCategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codepipeline.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
-    AcknowledgeJobOutputTypeDef,
+    ResponseMetadataTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
-    AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionConfigurationTypeDef,
     ActionContextTypeDef,
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
     ActionExecutionResultTypeDef,
     ErrorDetailsTypeDef,
-    ActionRevisionTypeDef,
+    ActionRevisionOutputTypeDef,
+    TimestampTypeDef,
     ActionTypeArtifactDetailsTypeDef,
     ActionTypeIdentifierTypeDef,
-    ActionTypePermissionsTypeDef,
+    ActionTypePermissionsOutputTypeDef,
     ActionTypePropertyTypeDef,
     ActionTypeUrlsTypeDef,
+    ActionTypePermissionsTypeDef,
     ActionTypeSettingsTypeDef,
     ArtifactDetailsTypeDef,
     ApprovalResultTypeDef,
     S3LocationTypeDef,
     S3ArtifactLocationTypeDef,
     ArtifactRevisionTypeDef,
     EncryptionKeyTypeDef,
     BlockerDeclarationTypeDef,
     TagTypeDef,
-    CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
     ExecutionTriggerTypeDef,
-    JobWorkerExecutorConfigurationTypeDef,
+    JobWorkerExecutorConfigurationOutputTypeDef,
     LambdaExecutorConfigurationTypeDef,
+    JobWorkerExecutorConfigurationTypeDef,
     FailureDetailsTypeDef,
     GetActionTypeInputRequestTypeDef,
     GetJobDetailsInputRequestTypeDef,
     GetPipelineExecutionInputRequestTypeDef,
     GetPipelineInputRequestTypeDef,
     PipelineMetadataTypeDef,
     GetPipelineStateInputRequestTypeDef,
     GetThirdPartyJobDetailsInputRequestTypeDef,
-    ListActionTypesInputListActionTypesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListActionTypesInputRequestTypeDef,
-    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
     ListPipelineExecutionsInputRequestTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineSummaryTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListWebhooksInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     StageContextTypeDef,
     SourceRevisionTypeDef,
     StopExecutionTriggerTypeDef,
     ThirdPartyJobTypeDef,
-    PutActionRevisionOutputTypeDef,
-    PutApprovalResultOutputTypeDef,
     RegisterWebhookWithThirdPartyInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     RetryStageExecutionInputRequestTypeDef,
-    RetryStageExecutionOutputTypeDef,
     StageExecutionTypeDef,
     TransitionStateTypeDef,
     StartPipelineExecutionInputRequestTypeDef,
-    StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionInputRequestTypeDef,
-    StopPipelineExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     WebhookAuthConfigurationTypeDef,
     WebhookFilterRuleTypeDef,
+    AcknowledgeJobOutputTypeDef,
+    AcknowledgeThirdPartyJobOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    PutActionRevisionOutputTypeDef,
+    PutApprovalResultOutputTypeDef,
+    RetryStageExecutionOutputTypeDef,
+    StartPipelineExecutionOutputTypeDef,
+    StopPipelineExecutionOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
+    ActionDeclarationOutputTypeDef,
     ActionDeclarationTypeDef,
-    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
-    PutActionRevisionInputRequestTypeDef,
+    ActionRevisionTypeDef,
+    CurrentRevisionTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
     PipelineExecutionTypeDef,
     ArtifactStoreTypeDef,
     CreateCustomActionTypeInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
-    PutJobSuccessResultInputRequestTypeDef,
-    PutThirdPartyJobSuccessResultInputRequestTypeDef,
+    ExecutorConfigurationOutputTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
+    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+    ListActionTypesInputListActionTypesPaginateTypeDef,
+    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListPipelinesOutputTypeDef,
     PipelineContextTypeDef,
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
+    WebhookDefinitionOutputTypeDef,
     WebhookDefinitionTypeDef,
+    StageDeclarationOutputTypeDef,
     StageDeclarationTypeDef,
     ActionStateTypeDef,
+    ActionRevisionUnionTypeDef,
+    PutActionRevisionInputRequestTypeDef,
+    PutJobSuccessResultInputRequestTypeDef,
+    PutThirdPartyJobSuccessResultInputRequestTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ActionExecutionInputTypeDef,
     ActionExecutionOutputTypeDef,
     ArtifactTypeDef,
     GetPipelineExecutionOutputTypeDef,
+    ActionTypeExecutorOutputTypeDef,
     ActionTypeExecutorTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListWebhookItemTypeDef,
     PutWebhookInputRequestTypeDef,
+    WebhookDefinitionUnionTypeDef,
+    PipelineDeclarationOutputTypeDef,
     PipelineDeclarationTypeDef,
     StageStateTypeDef,
     ActionExecutionDetailTypeDef,
     JobDataTypeDef,
     ThirdPartyJobDataTypeDef,
+    ActionTypeDeclarationOutputTypeDef,
     ActionTypeDeclarationTypeDef,
     ListWebhooksOutputTypeDef,
     PutWebhookOutputTypeDef,
-    CreatePipelineInputRequestTypeDef,
     CreatePipelineOutputTypeDef,
     GetPipelineOutputTypeDef,
-    UpdatePipelineInputRequestTypeDef,
     UpdatePipelineOutputTypeDef,
+    CreatePipelineInputRequestTypeDef,
+    PipelineDeclarationUnionTypeDef,
+    UpdatePipelineInputRequestTypeDef,
     GetPipelineStateOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     JobDetailsTypeDef,
     JobTypeDef,
     ThirdPartyJobDetailsTypeDef,
     GetActionTypeOutputTypeDef,
+    ActionTypeDeclarationUnionTypeDef,
     UpdateActionTypeInputRequestTypeDef,
     GetJobDetailsOutputTypeDef,
     PollForJobsOutputTypeDef,
     GetThirdPartyJobDetailsOutputTypeDef,
 )
 
 
-def get_structure() -> AWSSessionCredentialsTypeDef:
+def get_value() -> AWSSessionCredentialsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codepipeline-2.5.2/README.md` & `types-aiobotocore-codepipeline-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-codepipeline"></a>
 
 # types-aiobotocore-codepipeline
 
 [![PyPI - types-aiobotocore-codepipeline](https://img.shields.io/pypi/v/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codepipeline?color=blue)](https://pypistats.org/packages/types-aiobotocore-codepipeline)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codepipeline)](https://pepy.tech/project/types-aiobotocore-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodePipeline 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [types-aiobotocore-codepipeline docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/).
 
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
@@ -315,168 +315,183 @@
 )
 
 
 def check_value(value: ActionCategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codepipeline.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
-    AcknowledgeJobOutputTypeDef,
+    ResponseMetadataTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
-    AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionConfigurationTypeDef,
     ActionContextTypeDef,
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
     ActionExecutionResultTypeDef,
     ErrorDetailsTypeDef,
-    ActionRevisionTypeDef,
+    ActionRevisionOutputTypeDef,
+    TimestampTypeDef,
     ActionTypeArtifactDetailsTypeDef,
     ActionTypeIdentifierTypeDef,
-    ActionTypePermissionsTypeDef,
+    ActionTypePermissionsOutputTypeDef,
     ActionTypePropertyTypeDef,
     ActionTypeUrlsTypeDef,
+    ActionTypePermissionsTypeDef,
     ActionTypeSettingsTypeDef,
     ArtifactDetailsTypeDef,
     ApprovalResultTypeDef,
     S3LocationTypeDef,
     S3ArtifactLocationTypeDef,
     ArtifactRevisionTypeDef,
     EncryptionKeyTypeDef,
     BlockerDeclarationTypeDef,
     TagTypeDef,
-    CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
     ExecutionTriggerTypeDef,
-    JobWorkerExecutorConfigurationTypeDef,
+    JobWorkerExecutorConfigurationOutputTypeDef,
     LambdaExecutorConfigurationTypeDef,
+    JobWorkerExecutorConfigurationTypeDef,
     FailureDetailsTypeDef,
     GetActionTypeInputRequestTypeDef,
     GetJobDetailsInputRequestTypeDef,
     GetPipelineExecutionInputRequestTypeDef,
     GetPipelineInputRequestTypeDef,
     PipelineMetadataTypeDef,
     GetPipelineStateInputRequestTypeDef,
     GetThirdPartyJobDetailsInputRequestTypeDef,
-    ListActionTypesInputListActionTypesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListActionTypesInputRequestTypeDef,
-    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
     ListPipelineExecutionsInputRequestTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineSummaryTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListWebhooksInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     StageContextTypeDef,
     SourceRevisionTypeDef,
     StopExecutionTriggerTypeDef,
     ThirdPartyJobTypeDef,
-    PutActionRevisionOutputTypeDef,
-    PutApprovalResultOutputTypeDef,
     RegisterWebhookWithThirdPartyInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     RetryStageExecutionInputRequestTypeDef,
-    RetryStageExecutionOutputTypeDef,
     StageExecutionTypeDef,
     TransitionStateTypeDef,
     StartPipelineExecutionInputRequestTypeDef,
-    StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionInputRequestTypeDef,
-    StopPipelineExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     WebhookAuthConfigurationTypeDef,
     WebhookFilterRuleTypeDef,
+    AcknowledgeJobOutputTypeDef,
+    AcknowledgeThirdPartyJobOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    PutActionRevisionOutputTypeDef,
+    PutApprovalResultOutputTypeDef,
+    RetryStageExecutionOutputTypeDef,
+    StartPipelineExecutionOutputTypeDef,
+    StopPipelineExecutionOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
+    ActionDeclarationOutputTypeDef,
     ActionDeclarationTypeDef,
-    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
-    PutActionRevisionInputRequestTypeDef,
+    ActionRevisionTypeDef,
+    CurrentRevisionTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
     PipelineExecutionTypeDef,
     ArtifactStoreTypeDef,
     CreateCustomActionTypeInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
-    PutJobSuccessResultInputRequestTypeDef,
-    PutThirdPartyJobSuccessResultInputRequestTypeDef,
+    ExecutorConfigurationOutputTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
+    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+    ListActionTypesInputListActionTypesPaginateTypeDef,
+    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListPipelinesOutputTypeDef,
     PipelineContextTypeDef,
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
+    WebhookDefinitionOutputTypeDef,
     WebhookDefinitionTypeDef,
+    StageDeclarationOutputTypeDef,
     StageDeclarationTypeDef,
     ActionStateTypeDef,
+    ActionRevisionUnionTypeDef,
+    PutActionRevisionInputRequestTypeDef,
+    PutJobSuccessResultInputRequestTypeDef,
+    PutThirdPartyJobSuccessResultInputRequestTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ActionExecutionInputTypeDef,
     ActionExecutionOutputTypeDef,
     ArtifactTypeDef,
     GetPipelineExecutionOutputTypeDef,
+    ActionTypeExecutorOutputTypeDef,
     ActionTypeExecutorTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListWebhookItemTypeDef,
     PutWebhookInputRequestTypeDef,
+    WebhookDefinitionUnionTypeDef,
+    PipelineDeclarationOutputTypeDef,
     PipelineDeclarationTypeDef,
     StageStateTypeDef,
     ActionExecutionDetailTypeDef,
     JobDataTypeDef,
     ThirdPartyJobDataTypeDef,
+    ActionTypeDeclarationOutputTypeDef,
     ActionTypeDeclarationTypeDef,
     ListWebhooksOutputTypeDef,
     PutWebhookOutputTypeDef,
-    CreatePipelineInputRequestTypeDef,
     CreatePipelineOutputTypeDef,
     GetPipelineOutputTypeDef,
-    UpdatePipelineInputRequestTypeDef,
     UpdatePipelineOutputTypeDef,
+    CreatePipelineInputRequestTypeDef,
+    PipelineDeclarationUnionTypeDef,
+    UpdatePipelineInputRequestTypeDef,
     GetPipelineStateOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     JobDetailsTypeDef,
     JobTypeDef,
     ThirdPartyJobDetailsTypeDef,
     GetActionTypeOutputTypeDef,
+    ActionTypeDeclarationUnionTypeDef,
     UpdateActionTypeInputRequestTypeDef,
     GetJobDetailsOutputTypeDef,
     PollForJobsOutputTypeDef,
     GetThirdPartyJobDetailsOutputTypeDef,
 )
 
 
-def get_structure() -> AWSSessionCredentialsTypeDef:
+def get_value() -> AWSSessionCredentialsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codepipeline-2.5.2/setup.py` & `types-aiobotocore-codepipeline-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codepipeline",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_codepipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodePipeline 2.5.2 service generated with"
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
-    keywords="aiobotocore codepipeline type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore codepipeline type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codepipeline": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/"
```

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/__init__.py` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/__init__.pyi` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/__main__.py` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodePipeline 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CodePipeline 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline\nOther"
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

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/client.py` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     ListWebhooksPaginator,
 )
 from .type_defs import (
     AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionExecutionFilterTypeDef,
-    ActionRevisionTypeDef,
-    ActionTypeDeclarationTypeDef,
+    ActionRevisionUnionTypeDef,
+    ActionTypeDeclarationUnionTypeDef,
     ActionTypeIdTypeDef,
     ActionTypeSettingsTypeDef,
     ApprovalResultTypeDef,
     ArtifactDetailsTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     CreatePipelineOutputTypeDef,
     CurrentRevisionTypeDef,
@@ -54,26 +54,26 @@
     GetThirdPartyJobDetailsOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListPipelinesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWebhooksOutputTypeDef,
-    PipelineDeclarationTypeDef,
+    PipelineDeclarationUnionTypeDef,
     PollForJobsOutputTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     PutActionRevisionOutputTypeDef,
     PutApprovalResultOutputTypeDef,
     PutWebhookOutputTypeDef,
     RetryStageExecutionOutputTypeDef,
     StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionOutputTypeDef,
     TagTypeDef,
     UpdatePipelineOutputTypeDef,
-    WebhookDefinitionTypeDef,
+    WebhookDefinitionUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -199,15 +199,15 @@
         the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#create_custom_action_type)
         """
 
     async def create_pipeline(
-        self, *, pipeline: PipelineDeclarationTypeDef, tags: Sequence[TagTypeDef] = ...
+        self, *, pipeline: PipelineDeclarationUnionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineOutputTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#create_pipeline)
         """
@@ -443,15 +443,15 @@
 
     async def put_action_revision(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
-        actionRevision: ActionRevisionTypeDef
+        actionRevision: ActionRevisionUnionTypeDef
     ) -> PutActionRevisionOutputTypeDef:
         """
         Provides information to CodePipeline about new revisions to a source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_action_revision)
         """
@@ -523,15 +523,15 @@
         worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_third_party_job_success_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_third_party_job_success_result)
         """
 
     async def put_webhook(
-        self, *, webhook: WebhookDefinitionTypeDef, tags: Sequence[TagTypeDef] = ...
+        self, *, webhook: WebhookDefinitionUnionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> PutWebhookOutputTypeDef:
         """
         Defines a webhook and returns a unique webhook URL generated by CodePipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_webhook)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_webhook)
         """
@@ -593,26 +593,26 @@
         Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#untag_resource)
         """
 
     async def update_action_type(
-        self, *, actionType: ActionTypeDeclarationTypeDef
+        self, *, actionType: ActionTypeDeclarationUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an action type that was created with any supported integration model,
         where the action type is to be used by customers of the action type provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_action_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#update_action_type)
         """
 
     async def update_pipeline(
-        self, *, pipeline: PipelineDeclarationTypeDef
+        self, *, pipeline: PipelineDeclarationUnionTypeDef
     ) -> UpdatePipelineOutputTypeDef:
         """
         Updates a specified pipeline with edits or changes to its structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/client.pyi` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     ListWebhooksPaginator,
 )
 from .type_defs import (
     AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionExecutionFilterTypeDef,
-    ActionRevisionTypeDef,
-    ActionTypeDeclarationTypeDef,
+    ActionRevisionUnionTypeDef,
+    ActionTypeDeclarationUnionTypeDef,
     ActionTypeIdTypeDef,
     ActionTypeSettingsTypeDef,
     ApprovalResultTypeDef,
     ArtifactDetailsTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     CreatePipelineOutputTypeDef,
     CurrentRevisionTypeDef,
@@ -54,26 +54,26 @@
     GetThirdPartyJobDetailsOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListPipelinesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWebhooksOutputTypeDef,
-    PipelineDeclarationTypeDef,
+    PipelineDeclarationUnionTypeDef,
     PollForJobsOutputTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     PutActionRevisionOutputTypeDef,
     PutApprovalResultOutputTypeDef,
     PutWebhookOutputTypeDef,
     RetryStageExecutionOutputTypeDef,
     StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionOutputTypeDef,
     TagTypeDef,
     UpdatePipelineOutputTypeDef,
-    WebhookDefinitionTypeDef,
+    WebhookDefinitionUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -189,15 +189,15 @@
         Creates a new custom action that can be used in all pipelines associated with
         the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#create_custom_action_type)
         """
     async def create_pipeline(
-        self, *, pipeline: PipelineDeclarationTypeDef, tags: Sequence[TagTypeDef] = ...
+        self, *, pipeline: PipelineDeclarationUnionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineOutputTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#create_pipeline)
         """
@@ -411,15 +411,15 @@
         """
     async def put_action_revision(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
-        actionRevision: ActionRevisionTypeDef
+        actionRevision: ActionRevisionUnionTypeDef
     ) -> PutActionRevisionOutputTypeDef:
         """
         Provides information to CodePipeline about new revisions to a source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_action_revision)
         """
@@ -485,15 +485,15 @@
         Represents the success of a third party job as returned to the pipeline by a job
         worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_third_party_job_success_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_third_party_job_success_result)
         """
     async def put_webhook(
-        self, *, webhook: WebhookDefinitionTypeDef, tags: Sequence[TagTypeDef] = ...
+        self, *, webhook: WebhookDefinitionUnionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> PutWebhookOutputTypeDef:
         """
         Defines a webhook and returns a unique webhook URL generated by CodePipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_webhook)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_webhook)
         """
@@ -548,25 +548,25 @@
         """
         Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#untag_resource)
         """
     async def update_action_type(
-        self, *, actionType: ActionTypeDeclarationTypeDef
+        self, *, actionType: ActionTypeDeclarationUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an action type that was created with any supported integration model,
         where the action type is to be used by customers of the action type provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_action_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#update_action_type)
         """
     async def update_pipeline(
-        self, *, pipeline: PipelineDeclarationTypeDef
+        self, *, pipeline: PipelineDeclarationUnionTypeDef
     ) -> UpdatePipelineOutputTypeDef:
         """
         Updates a specified pipeline with edits or changes to its structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/literals.py` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/literals.pyi` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/paginator.py` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -52,114 +52,106 @@
     "ListActionTypesPaginator",
     "ListPipelineExecutionsPaginator",
     "ListPipelinesPaginator",
     "ListTagsForResourcePaginator",
     "ListWebhooksPaginator",
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
 class ListActionExecutionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionExecutions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listactionexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         pipelineName: str,
         filter: ActionExecutionFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListActionExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listactionexecutionspaginator)
         """
 
-
 class ListActionTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listactiontypespaginator)
     """
 
     def paginate(
         self,
         *,
         actionOwnerFilter: ActionOwnerType = ...,
         regionFilter: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListActionTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listactiontypespaginator)
         """
 
-
 class ListPipelineExecutionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listpipelineexecutionspaginator)
     """
 
     def paginate(
-        self, *, pipelineName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pipelineName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPipelineExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listpipelineexecutionspaginator)
         """
 
-
 class ListPipelinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPipelinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listpipelinespaginator)
         """
 
-
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listtagsforresourcepaginator)
         """
 
-
 class ListWebhooksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listwebhookspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWebhooksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listwebhookspaginator)
         """
```

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/paginator.pyi` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,106 +52,114 @@
     "ListActionTypesPaginator",
     "ListPipelineExecutionsPaginator",
     "ListPipelinesPaginator",
     "ListTagsForResourcePaginator",
     "ListWebhooksPaginator",
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
 class ListActionExecutionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionExecutions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listactionexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         pipelineName: str,
         filter: ActionExecutionFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListActionExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listactionexecutionspaginator)
         """
 
+
 class ListActionTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listactiontypespaginator)
     """
 
     def paginate(
         self,
         *,
         actionOwnerFilter: ActionOwnerType = ...,
         regionFilter: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListActionTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListActionTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listactiontypespaginator)
         """
 
+
 class ListPipelineExecutionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listpipelineexecutionspaginator)
     """
 
     def paginate(
-        self, *, pipelineName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, pipelineName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPipelineExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelineExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listpipelineexecutionspaginator)
         """
 
+
 class ListPipelinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPipelinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListPipelines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listpipelinespaginator)
         """
 
+
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listtagsforresourcepaginator)
         """
 
+
 class ListWebhooksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listwebhookspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWebhooksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Paginator.ListWebhooks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/paginators/#listwebhookspaginator)
         """
```

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/type_defs.py` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codepipeline.type_defs import AWSSessionCredentialsTypeDef
 
-    data: AWSSessionCredentialsTypeDef = {...}
+    data: AWSSessionCredentialsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -40,149 +40,164 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AWSSessionCredentialsTypeDef",
     "AcknowledgeJobInputRequestTypeDef",
-    "AcknowledgeJobOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
-    "AcknowledgeThirdPartyJobOutputTypeDef",
     "ActionConfigurationPropertyTypeDef",
     "ActionConfigurationTypeDef",
     "ActionContextTypeDef",
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "ActionExecutionFilterTypeDef",
     "ActionExecutionResultTypeDef",
     "ErrorDetailsTypeDef",
-    "ActionRevisionTypeDef",
+    "ActionRevisionOutputTypeDef",
+    "TimestampTypeDef",
     "ActionTypeArtifactDetailsTypeDef",
     "ActionTypeIdentifierTypeDef",
-    "ActionTypePermissionsTypeDef",
+    "ActionTypePermissionsOutputTypeDef",
     "ActionTypePropertyTypeDef",
     "ActionTypeUrlsTypeDef",
+    "ActionTypePermissionsTypeDef",
     "ActionTypeSettingsTypeDef",
     "ArtifactDetailsTypeDef",
     "ApprovalResultTypeDef",
     "S3LocationTypeDef",
     "S3ArtifactLocationTypeDef",
     "ArtifactRevisionTypeDef",
     "EncryptionKeyTypeDef",
     "BlockerDeclarationTypeDef",
     "TagTypeDef",
-    "CurrentRevisionTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
     "ExecutionTriggerTypeDef",
-    "JobWorkerExecutorConfigurationTypeDef",
+    "JobWorkerExecutorConfigurationOutputTypeDef",
     "LambdaExecutorConfigurationTypeDef",
+    "JobWorkerExecutorConfigurationTypeDef",
     "FailureDetailsTypeDef",
     "GetActionTypeInputRequestTypeDef",
     "GetJobDetailsInputRequestTypeDef",
     "GetPipelineExecutionInputRequestTypeDef",
     "GetPipelineInputRequestTypeDef",
     "PipelineMetadataTypeDef",
     "GetPipelineStateInputRequestTypeDef",
     "GetThirdPartyJobDetailsInputRequestTypeDef",
-    "ListActionTypesInputListActionTypesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListActionTypesInputRequestTypeDef",
-    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
     "ListPipelineExecutionsInputRequestTypeDef",
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineSummaryTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListWebhooksInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "StageContextTypeDef",
     "SourceRevisionTypeDef",
     "StopExecutionTriggerTypeDef",
     "ThirdPartyJobTypeDef",
-    "PutActionRevisionOutputTypeDef",
-    "PutApprovalResultOutputTypeDef",
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryStageExecutionInputRequestTypeDef",
-    "RetryStageExecutionOutputTypeDef",
     "StageExecutionTypeDef",
     "TransitionStateTypeDef",
     "StartPipelineExecutionInputRequestTypeDef",
-    "StartPipelineExecutionOutputTypeDef",
     "StopPipelineExecutionInputRequestTypeDef",
-    "StopPipelineExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "WebhookAuthConfigurationTypeDef",
     "WebhookFilterRuleTypeDef",
+    "AcknowledgeJobOutputTypeDef",
+    "AcknowledgeThirdPartyJobOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "PutActionRevisionOutputTypeDef",
+    "PutApprovalResultOutputTypeDef",
+    "RetryStageExecutionOutputTypeDef",
+    "StartPipelineExecutionOutputTypeDef",
+    "StopPipelineExecutionOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
+    "ActionDeclarationOutputTypeDef",
     "ActionDeclarationTypeDef",
-    "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionExecutionTypeDef",
-    "PutActionRevisionInputRequestTypeDef",
+    "ActionRevisionTypeDef",
+    "CurrentRevisionTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
     "PipelineExecutionTypeDef",
     "ArtifactStoreTypeDef",
     "CreateCustomActionTypeInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
-    "PutJobSuccessResultInputRequestTypeDef",
-    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
+    "ExecutorConfigurationOutputTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
+    "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    "ListActionTypesInputListActionTypesPaginateTypeDef",
+    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListPipelinesOutputTypeDef",
     "PipelineContextTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
+    "WebhookDefinitionOutputTypeDef",
     "WebhookDefinitionTypeDef",
+    "StageDeclarationOutputTypeDef",
     "StageDeclarationTypeDef",
     "ActionStateTypeDef",
+    "ActionRevisionUnionTypeDef",
+    "PutActionRevisionInputRequestTypeDef",
+    "PutJobSuccessResultInputRequestTypeDef",
+    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "CreateCustomActionTypeOutputTypeDef",
     "ListActionTypesOutputTypeDef",
     "ActionExecutionInputTypeDef",
     "ActionExecutionOutputTypeDef",
     "ArtifactTypeDef",
     "GetPipelineExecutionOutputTypeDef",
+    "ActionTypeExecutorOutputTypeDef",
     "ActionTypeExecutorTypeDef",
     "ListPipelineExecutionsOutputTypeDef",
     "ListWebhookItemTypeDef",
     "PutWebhookInputRequestTypeDef",
+    "WebhookDefinitionUnionTypeDef",
+    "PipelineDeclarationOutputTypeDef",
     "PipelineDeclarationTypeDef",
     "StageStateTypeDef",
     "ActionExecutionDetailTypeDef",
     "JobDataTypeDef",
     "ThirdPartyJobDataTypeDef",
+    "ActionTypeDeclarationOutputTypeDef",
     "ActionTypeDeclarationTypeDef",
     "ListWebhooksOutputTypeDef",
     "PutWebhookOutputTypeDef",
-    "CreatePipelineInputRequestTypeDef",
     "CreatePipelineOutputTypeDef",
     "GetPipelineOutputTypeDef",
-    "UpdatePipelineInputRequestTypeDef",
     "UpdatePipelineOutputTypeDef",
+    "CreatePipelineInputRequestTypeDef",
+    "PipelineDeclarationUnionTypeDef",
+    "UpdatePipelineInputRequestTypeDef",
     "GetPipelineStateOutputTypeDef",
     "ListActionExecutionsOutputTypeDef",
     "JobDetailsTypeDef",
     "JobTypeDef",
     "ThirdPartyJobDetailsTypeDef",
     "GetActionTypeOutputTypeDef",
+    "ActionTypeDeclarationUnionTypeDef",
     "UpdateActionTypeInputRequestTypeDef",
     "GetJobDetailsOutputTypeDef",
     "PollForJobsOutputTypeDef",
     "GetThirdPartyJobDetailsOutputTypeDef",
 )
 
 AWSSessionCredentialsTypeDef = TypedDict(
@@ -198,39 +213,34 @@
     "AcknowledgeJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
     },
 )
 
-AcknowledgeJobOutputTypeDef = TypedDict(
-    "AcknowledgeJobOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "status": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AcknowledgeThirdPartyJobInputRequestTypeDef = TypedDict(
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
         "clientToken": str,
     },
 )
 
-AcknowledgeThirdPartyJobOutputTypeDef = TypedDict(
-    "AcknowledgeThirdPartyJobOutputTypeDef",
-    {
-        "status": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredActionConfigurationPropertyTypeDef = TypedDict(
     "_RequiredActionConfigurationPropertyTypeDef",
     {
         "name": str,
         "required": bool,
         "key": bool,
         "secret": bool,
@@ -317,23 +327,24 @@
     {
         "code": str,
         "message": str,
     },
     total=False,
 )
 
-ActionRevisionTypeDef = TypedDict(
-    "ActionRevisionTypeDef",
+ActionRevisionOutputTypeDef = TypedDict(
+    "ActionRevisionOutputTypeDef",
     {
         "revisionId": str,
         "revisionChangeId": str,
         "created": datetime,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 ActionTypeArtifactDetailsTypeDef = TypedDict(
     "ActionTypeArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
@@ -344,16 +355,16 @@
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
     },
 )
 
-ActionTypePermissionsTypeDef = TypedDict(
-    "ActionTypePermissionsTypeDef",
+ActionTypePermissionsOutputTypeDef = TypedDict(
+    "ActionTypePermissionsOutputTypeDef",
     {
         "allowedAccounts": List[str],
     },
 )
 
 _RequiredActionTypePropertyTypeDef = TypedDict(
     "_RequiredActionTypePropertyTypeDef",
@@ -387,14 +398,21 @@
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
     },
     total=False,
 )
 
+ActionTypePermissionsTypeDef = TypedDict(
+    "ActionTypePermissionsTypeDef",
+    {
+        "allowedAccounts": Sequence[str],
+    },
+)
+
 ActionTypeSettingsTypeDef = TypedDict(
     "ActionTypeSettingsTypeDef",
     {
         "thirdPartyConfigurationUrl": str,
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
@@ -468,35 +486,14 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-_RequiredCurrentRevisionTypeDef = TypedDict(
-    "_RequiredCurrentRevisionTypeDef",
-    {
-        "revision": str,
-        "changeIdentifier": str,
-    },
-)
-_OptionalCurrentRevisionTypeDef = TypedDict(
-    "_OptionalCurrentRevisionTypeDef",
-    {
-        "created": Union[datetime, str],
-        "revisionSummary": str,
-    },
-    total=False,
-)
-
-
-class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
-    pass
-
-
 DeleteCustomActionTypeInputRequestTypeDef = TypedDict(
     "DeleteCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
     },
@@ -530,21 +527,14 @@
         "pipelineName": str,
         "stageName": str,
         "transitionType": StageTransitionTypeType,
         "reason": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableStageTransitionInputRequestTypeDef = TypedDict(
     "EnableStageTransitionInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "transitionType": StageTransitionTypeType,
     },
@@ -565,30 +555,39 @@
     {
         "triggerType": TriggerTypeType,
         "triggerDetail": str,
     },
     total=False,
 )
 
-JobWorkerExecutorConfigurationTypeDef = TypedDict(
-    "JobWorkerExecutorConfigurationTypeDef",
+JobWorkerExecutorConfigurationOutputTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationOutputTypeDef",
     {
         "pollingAccounts": List[str],
         "pollingServicePrincipals": List[str],
     },
     total=False,
 )
 
 LambdaExecutorConfigurationTypeDef = TypedDict(
     "LambdaExecutorConfigurationTypeDef",
     {
         "lambdaFunctionArn": str,
     },
 )
 
+JobWorkerExecutorConfigurationTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationTypeDef",
+    {
+        "pollingAccounts": Sequence[str],
+        "pollingServicePrincipals": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredFailureDetailsTypeDef = TypedDict(
     "_RequiredFailureDetailsTypeDef",
     {
         "type": FailureTypeType,
         "message": str,
     },
 )
@@ -673,56 +672,34 @@
     "GetThirdPartyJobDetailsInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
     },
 )
 
-ListActionTypesInputListActionTypesPaginateTypeDef = TypedDict(
-    "ListActionTypesInputListActionTypesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "actionOwnerFilter": ActionOwnerType,
-        "regionFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListActionTypesInputRequestTypeDef = TypedDict(
     "ListActionTypesInputRequestTypeDef",
     {
         "actionOwnerFilter": ActionOwnerType,
         "nextToken": str,
         "regionFilter": str,
     },
     total=False,
 )
 
-_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "pipelineName": str,
-    },
-)
-_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(
-    _RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-    _OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPipelineExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListPipelineExecutionsInputRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 _OptionalListPipelineExecutionsInputRequestTypeDef = TypedDict(
@@ -738,22 +715,14 @@
 class ListPipelineExecutionsInputRequestTypeDef(
     _RequiredListPipelineExecutionsInputRequestTypeDef,
     _OptionalListPipelineExecutionsInputRequestTypeDef,
 ):
     pass
 
 
-ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesInputRequestTypeDef = TypedDict(
     "ListPipelinesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -766,36 +735,14 @@
         "version": int,
         "created": datetime,
         "updated": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -810,41 +757,23 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
-ListWebhooksInputListWebhooksPaginateTypeDef = TypedDict(
-    "ListWebhooksInputListWebhooksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWebhooksInputRequestTypeDef = TypedDict(
     "ListWebhooksInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
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
 StageContextTypeDef = TypedDict(
     "StageContextTypeDef",
     {
         "name": str,
     },
     total=False,
 )
@@ -883,68 +812,32 @@
     {
         "clientId": str,
         "jobId": str,
     },
     total=False,
 )
 
-PutActionRevisionOutputTypeDef = TypedDict(
-    "PutActionRevisionOutputTypeDef",
-    {
-        "newRevision": bool,
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutApprovalResultOutputTypeDef = TypedDict(
-    "PutApprovalResultOutputTypeDef",
-    {
-        "approvedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterWebhookWithThirdPartyInputRequestTypeDef = TypedDict(
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
     {
         "webhookName": str,
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
 RetryStageExecutionInputRequestTypeDef = TypedDict(
     "RetryStageExecutionInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "pipelineExecutionId": str,
         "retryMode": Literal["FAILED_ACTIONS"],
     },
 )
 
-RetryStageExecutionOutputTypeDef = TypedDict(
-    "RetryStageExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StageExecutionTypeDef = TypedDict(
     "StageExecutionTypeDef",
     {
         "pipelineExecutionId": str,
         "status": StageExecutionStatusType,
     },
 )
@@ -978,22 +871,14 @@
 class StartPipelineExecutionInputRequestTypeDef(
     _RequiredStartPipelineExecutionInputRequestTypeDef,
     _OptionalStartPipelineExecutionInputRequestTypeDef,
 ):
     pass
 
 
-StartPipelineExecutionOutputTypeDef = TypedDict(
-    "StartPipelineExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopPipelineExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStopPipelineExecutionInputRequestTypeDef",
     {
         "pipelineName": str,
         "pipelineExecutionId": str,
     },
 )
@@ -1010,22 +895,14 @@
 class StopPipelineExecutionInputRequestTypeDef(
     _RequiredStopPipelineExecutionInputRequestTypeDef,
     _OptionalStopPipelineExecutionInputRequestTypeDef,
 ):
     pass
 
 
-StopPipelineExecutionOutputTypeDef = TypedDict(
-    "StopPipelineExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1056,14 +933,78 @@
 
 class WebhookFilterRuleTypeDef(
     _RequiredWebhookFilterRuleTypeDef, _OptionalWebhookFilterRuleTypeDef
 ):
     pass
 
 
+AcknowledgeJobOutputTypeDef = TypedDict(
+    "AcknowledgeJobOutputTypeDef",
+    {
+        "status": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AcknowledgeThirdPartyJobOutputTypeDef = TypedDict(
+    "AcknowledgeThirdPartyJobOutputTypeDef",
+    {
+        "status": JobStatusType,
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
+PutActionRevisionOutputTypeDef = TypedDict(
+    "PutActionRevisionOutputTypeDef",
+    {
+        "newRevision": bool,
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutApprovalResultOutputTypeDef = TypedDict(
+    "PutApprovalResultOutputTypeDef",
+    {
+        "approvedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetryStageExecutionOutputTypeDef = TypedDict(
+    "RetryStageExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartPipelineExecutionOutputTypeDef = TypedDict(
+    "StartPipelineExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopPipelineExecutionOutputTypeDef = TypedDict(
+    "StopPipelineExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPollForJobsInputRequestTypeDef = TypedDict(
     "_RequiredPollForJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
 _OptionalPollForJobsInputRequestTypeDef = TypedDict(
@@ -1100,61 +1041,66 @@
 class PollForThirdPartyJobsInputRequestTypeDef(
     _RequiredPollForThirdPartyJobsInputRequestTypeDef,
     _OptionalPollForThirdPartyJobsInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredActionDeclarationTypeDef = TypedDict(
-    "_RequiredActionDeclarationTypeDef",
+_RequiredActionDeclarationOutputTypeDef = TypedDict(
+    "_RequiredActionDeclarationOutputTypeDef",
     {
         "name": str,
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
-_OptionalActionDeclarationTypeDef = TypedDict(
-    "_OptionalActionDeclarationTypeDef",
+_OptionalActionDeclarationOutputTypeDef = TypedDict(
+    "_OptionalActionDeclarationOutputTypeDef",
     {
         "runOrder": int,
-        "configuration": Mapping[str, str],
-        "outputArtifacts": Sequence[OutputArtifactTypeDef],
-        "inputArtifacts": Sequence[InputArtifactTypeDef],
+        "configuration": Dict[str, str],
+        "outputArtifacts": List[OutputArtifactTypeDef],
+        "inputArtifacts": List[InputArtifactTypeDef],
         "roleArn": str,
         "region": str,
         "namespace": str,
     },
     total=False,
 )
 
 
-class ActionDeclarationTypeDef(
-    _RequiredActionDeclarationTypeDef, _OptionalActionDeclarationTypeDef
+class ActionDeclarationOutputTypeDef(
+    _RequiredActionDeclarationOutputTypeDef, _OptionalActionDeclarationOutputTypeDef
 ):
     pass
 
 
-_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+_RequiredActionDeclarationTypeDef = TypedDict(
+    "_RequiredActionDeclarationTypeDef",
     {
-        "pipelineName": str,
+        "name": str,
+        "actionTypeId": ActionTypeIdTypeDef,
     },
 )
-_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+_OptionalActionDeclarationTypeDef = TypedDict(
+    "_OptionalActionDeclarationTypeDef",
     {
-        "filter": ActionExecutionFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "runOrder": int,
+        "configuration": Mapping[str, str],
+        "outputArtifacts": Sequence[OutputArtifactTypeDef],
+        "inputArtifacts": Sequence[InputArtifactTypeDef],
+        "roleArn": str,
+        "region": str,
+        "namespace": str,
     },
     total=False,
 )
 
 
-class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(
-    _RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef,
-    _OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+class ActionDeclarationTypeDef(
+    _RequiredActionDeclarationTypeDef, _OptionalActionDeclarationTypeDef
 ):
     pass
 
 
 _RequiredListActionExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListActionExecutionsInputRequestTypeDef",
     {
@@ -1192,24 +1138,44 @@
         "externalExecutionUrl": str,
         "percentComplete": int,
         "errorDetails": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
-PutActionRevisionInputRequestTypeDef = TypedDict(
-    "PutActionRevisionInputRequestTypeDef",
+ActionRevisionTypeDef = TypedDict(
+    "ActionRevisionTypeDef",
     {
-        "pipelineName": str,
-        "stageName": str,
-        "actionName": str,
-        "actionRevision": ActionRevisionTypeDef,
+        "revisionId": str,
+        "revisionChangeId": str,
+        "created": TimestampTypeDef,
     },
 )
 
+_RequiredCurrentRevisionTypeDef = TypedDict(
+    "_RequiredCurrentRevisionTypeDef",
+    {
+        "revision": str,
+        "changeIdentifier": str,
+    },
+)
+_OptionalCurrentRevisionTypeDef = TypedDict(
+    "_OptionalCurrentRevisionTypeDef",
+    {
+        "created": TimestampTypeDef,
+        "revisionSummary": str,
+    },
+    total=False,
+)
+
+
+class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
+    pass
+
+
 _RequiredActionTypeTypeDef = TypedDict(
     "_RequiredActionTypeTypeDef",
     {
         "id": ActionTypeIdTypeDef,
         "inputArtifactDetails": ArtifactDetailsTypeDef,
         "outputArtifactDetails": ArtifactDetailsTypeDef,
     },
@@ -1319,107 +1285,160 @@
 
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": List[TagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_RequiredPutJobSuccessResultInputRequestTypeDef",
+ExecutorConfigurationOutputTypeDef = TypedDict(
+    "ExecutorConfigurationOutputTypeDef",
+    {
+        "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
+        "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+ExecutorConfigurationTypeDef = TypedDict(
+    "ExecutorConfigurationTypeDef",
+    {
+        "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
+        "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationTypeDef,
+    },
+    total=False,
+)
+
+PutJobFailureResultInputRequestTypeDef = TypedDict(
+    "PutJobFailureResultInputRequestTypeDef",
     {
         "jobId": str,
+        "failureDetails": FailureDetailsTypeDef,
     },
 )
-_OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_OptionalPutJobSuccessResultInputRequestTypeDef",
+
+PutThirdPartyJobFailureResultInputRequestTypeDef = TypedDict(
+    "PutThirdPartyJobFailureResultInputRequestTypeDef",
     {
-        "currentRevision": CurrentRevisionTypeDef,
-        "continuationToken": str,
-        "executionDetails": ExecutionDetailsTypeDef,
-        "outputVariables": Mapping[str, str],
+        "jobId": str,
+        "clientToken": str,
+        "failureDetails": FailureDetailsTypeDef,
+    },
+)
+
+_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    {
+        "pipelineName": str,
+    },
+)
+_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    {
+        "filter": ActionExecutionFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class PutJobSuccessResultInputRequestTypeDef(
-    _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
+class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(
+    _RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+    _OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
+ListActionTypesInputListActionTypesPaginateTypeDef = TypedDict(
+    "ListActionTypesInputListActionTypesPaginateTypeDef",
     {
-        "jobId": str,
-        "clientToken": str,
+        "actionOwnerFilter": ActionOwnerType,
+        "regionFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef",
+
+_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
     {
-        "currentRevision": CurrentRevisionTypeDef,
-        "continuationToken": str,
-        "executionDetails": ExecutionDetailsTypeDef,
+        "pipelineName": str,
+    },
+)
+_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class PutThirdPartyJobSuccessResultInputRequestTypeDef(
-    _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
-    _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
+class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(
+    _RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+    _OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
 ):
     pass
 
 
-ExecutorConfigurationTypeDef = TypedDict(
-    "ExecutorConfigurationTypeDef",
+ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
     {
-        "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
-        "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-PutJobFailureResultInputRequestTypeDef = TypedDict(
-    "PutJobFailureResultInputRequestTypeDef",
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     {
-        "jobId": str,
-        "failureDetails": FailureDetailsTypeDef,
+        "resourceArn": str,
     },
 )
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-PutThirdPartyJobFailureResultInputRequestTypeDef = TypedDict(
-    "PutThirdPartyJobFailureResultInputRequestTypeDef",
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+ListWebhooksInputListWebhooksPaginateTypeDef = TypedDict(
+    "ListWebhooksInputListWebhooksPaginateTypeDef",
     {
-        "jobId": str,
-        "clientToken": str,
-        "failureDetails": FailureDetailsTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelines": List[PipelineSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PipelineContextTypeDef = TypedDict(
     "PipelineContextTypeDef",
     {
         "pipelineName": str,
@@ -1445,30 +1464,64 @@
     total=False,
 )
 
 PollForThirdPartyJobsOutputTypeDef = TypedDict(
     "PollForThirdPartyJobsOutputTypeDef",
     {
         "jobs": List[ThirdPartyJobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+WebhookDefinitionOutputTypeDef = TypedDict(
+    "WebhookDefinitionOutputTypeDef",
+    {
+        "name": str,
+        "targetPipeline": str,
+        "targetAction": str,
+        "filters": List[WebhookFilterRuleTypeDef],
+        "authentication": WebhookAuthenticationTypeType,
+        "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
     },
 )
 
 WebhookDefinitionTypeDef = TypedDict(
     "WebhookDefinitionTypeDef",
     {
         "name": str,
         "targetPipeline": str,
         "targetAction": str,
-        "filters": List[WebhookFilterRuleTypeDef],
+        "filters": Sequence[WebhookFilterRuleTypeDef],
         "authentication": WebhookAuthenticationTypeType,
         "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
     },
 )
 
+_RequiredStageDeclarationOutputTypeDef = TypedDict(
+    "_RequiredStageDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "actions": List[ActionDeclarationOutputTypeDef],
+    },
+)
+_OptionalStageDeclarationOutputTypeDef = TypedDict(
+    "_OptionalStageDeclarationOutputTypeDef",
+    {
+        "blockers": List[BlockerDeclarationTypeDef],
+    },
+    total=False,
+)
+
+
+class StageDeclarationOutputTypeDef(
+    _RequiredStageDeclarationOutputTypeDef, _OptionalStageDeclarationOutputTypeDef
+):
+    pass
+
+
 _RequiredStageDeclarationTypeDef = TypedDict(
     "_RequiredStageDeclarationTypeDef",
     {
         "name": str,
         "actions": Sequence[ActionDeclarationTypeDef],
     },
 )
@@ -1485,37 +1538,97 @@
     pass
 
 
 ActionStateTypeDef = TypedDict(
     "ActionStateTypeDef",
     {
         "actionName": str,
-        "currentRevision": ActionRevisionTypeDef,
+        "currentRevision": ActionRevisionOutputTypeDef,
         "latestExecution": ActionExecutionTypeDef,
         "entityUrl": str,
         "revisionUrl": str,
     },
     total=False,
 )
 
+ActionRevisionUnionTypeDef = Union[ActionRevisionTypeDef, ActionRevisionOutputTypeDef]
+PutActionRevisionInputRequestTypeDef = TypedDict(
+    "PutActionRevisionInputRequestTypeDef",
+    {
+        "pipelineName": str,
+        "stageName": str,
+        "actionName": str,
+        "actionRevision": ActionRevisionTypeDef,
+    },
+)
+
+_RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_RequiredPutJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+    },
+)
+_OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_OptionalPutJobSuccessResultInputRequestTypeDef",
+    {
+        "currentRevision": CurrentRevisionTypeDef,
+        "continuationToken": str,
+        "executionDetails": ExecutionDetailsTypeDef,
+        "outputVariables": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class PutJobSuccessResultInputRequestTypeDef(
+    _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
+):
+    pass
+
+
+_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+        "clientToken": str,
+    },
+)
+_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "currentRevision": CurrentRevisionTypeDef,
+        "continuationToken": str,
+        "executionDetails": ExecutionDetailsTypeDef,
+    },
+    total=False,
+)
+
+
+class PutThirdPartyJobSuccessResultInputRequestTypeDef(
+    _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
+    _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
+):
+    pass
+
+
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListActionTypesOutputTypeDef = TypedDict(
     "ListActionTypesOutputTypeDef",
     {
         "actionTypes": List[ActionTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActionExecutionInputTypeDef = TypedDict(
     "ActionExecutionInputTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
@@ -1549,18 +1662,41 @@
     total=False,
 )
 
 GetPipelineExecutionOutputTypeDef = TypedDict(
     "GetPipelineExecutionOutputTypeDef",
     {
         "pipelineExecution": PipelineExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredActionTypeExecutorOutputTypeDef = TypedDict(
+    "_RequiredActionTypeExecutorOutputTypeDef",
+    {
+        "configuration": ExecutorConfigurationOutputTypeDef,
+        "type": ExecutorTypeType,
+    },
+)
+_OptionalActionTypeExecutorOutputTypeDef = TypedDict(
+    "_OptionalActionTypeExecutorOutputTypeDef",
+    {
+        "policyStatementsTemplate": str,
+        "jobTimeout": int,
     },
+    total=False,
 )
 
+
+class ActionTypeExecutorOutputTypeDef(
+    _RequiredActionTypeExecutorOutputTypeDef, _OptionalActionTypeExecutorOutputTypeDef
+):
+    pass
+
+
 _RequiredActionTypeExecutorTypeDef = TypedDict(
     "_RequiredActionTypeExecutorTypeDef",
     {
         "configuration": ExecutorConfigurationTypeDef,
         "type": ExecutorTypeType,
     },
 )
@@ -1581,22 +1717,22 @@
 
 
 ListPipelineExecutionsOutputTypeDef = TypedDict(
     "ListPipelineExecutionsOutputTypeDef",
     {
         "pipelineExecutionSummaries": List[PipelineExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListWebhookItemTypeDef = TypedDict(
     "_RequiredListWebhookItemTypeDef",
     {
-        "definition": WebhookDefinitionTypeDef,
+        "definition": WebhookDefinitionOutputTypeDef,
         "url": str,
     },
 )
 _OptionalListWebhookItemTypeDef = TypedDict(
     "_OptionalListWebhookItemTypeDef",
     {
         "errorMessage": str,
@@ -1630,14 +1766,40 @@
 
 class PutWebhookInputRequestTypeDef(
     _RequiredPutWebhookInputRequestTypeDef, _OptionalPutWebhookInputRequestTypeDef
 ):
     pass
 
 
+WebhookDefinitionUnionTypeDef = Union[WebhookDefinitionTypeDef, WebhookDefinitionOutputTypeDef]
+_RequiredPipelineDeclarationOutputTypeDef = TypedDict(
+    "_RequiredPipelineDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "roleArn": str,
+        "stages": List[StageDeclarationOutputTypeDef],
+    },
+)
+_OptionalPipelineDeclarationOutputTypeDef = TypedDict(
+    "_OptionalPipelineDeclarationOutputTypeDef",
+    {
+        "artifactStore": ArtifactStoreTypeDef,
+        "artifactStores": Dict[str, ArtifactStoreTypeDef],
+        "version": int,
+    },
+    total=False,
+)
+
+
+class PipelineDeclarationOutputTypeDef(
+    _RequiredPipelineDeclarationOutputTypeDef, _OptionalPipelineDeclarationOutputTypeDef
+):
+    pass
+
+
 _RequiredPipelineDeclarationTypeDef = TypedDict(
     "_RequiredPipelineDeclarationTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": Sequence[StageDeclarationTypeDef],
     },
@@ -1714,29 +1876,56 @@
         "artifactCredentials": AWSSessionCredentialsTypeDef,
         "continuationToken": str,
         "encryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
+_RequiredActionTypeDeclarationOutputTypeDef = TypedDict(
+    "_RequiredActionTypeDeclarationOutputTypeDef",
+    {
+        "executor": ActionTypeExecutorOutputTypeDef,
+        "id": ActionTypeIdentifierTypeDef,
+        "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
+        "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
+    },
+)
+_OptionalActionTypeDeclarationOutputTypeDef = TypedDict(
+    "_OptionalActionTypeDeclarationOutputTypeDef",
+    {
+        "description": str,
+        "permissions": ActionTypePermissionsOutputTypeDef,
+        "properties": List[ActionTypePropertyTypeDef],
+        "urls": ActionTypeUrlsTypeDef,
+    },
+    total=False,
+)
+
+
+class ActionTypeDeclarationOutputTypeDef(
+    _RequiredActionTypeDeclarationOutputTypeDef, _OptionalActionTypeDeclarationOutputTypeDef
+):
+    pass
+
+
 _RequiredActionTypeDeclarationTypeDef = TypedDict(
     "_RequiredActionTypeDeclarationTypeDef",
     {
         "executor": ActionTypeExecutorTypeDef,
         "id": ActionTypeIdentifierTypeDef,
         "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
         "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
     },
 )
 _OptionalActionTypeDeclarationTypeDef = TypedDict(
     "_OptionalActionTypeDeclarationTypeDef",
     {
         "description": str,
         "permissions": ActionTypePermissionsTypeDef,
-        "properties": List[ActionTypePropertyTypeDef],
+        "properties": Sequence[ActionTypePropertyTypeDef],
         "urls": ActionTypeUrlsTypeDef,
     },
     total=False,
 )
 
 
 class ActionTypeDeclarationTypeDef(
@@ -1746,23 +1935,49 @@
 
 
 ListWebhooksOutputTypeDef = TypedDict(
     "ListWebhooksOutputTypeDef",
     {
         "webhooks": List[ListWebhookItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutWebhookOutputTypeDef = TypedDict(
     "PutWebhookOutputTypeDef",
     {
         "webhook": ListWebhookItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePipelineOutputTypeDef = TypedDict(
+    "CreatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPipelineOutputTypeDef = TypedDict(
+    "GetPipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "metadata": PipelineMetadataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePipelineOutputTypeDef = TypedDict(
+    "UpdatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
@@ -1779,65 +1994,42 @@
 
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
 
-CreatePipelineOutputTypeDef = TypedDict(
-    "CreatePipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetPipelineOutputTypeDef = TypedDict(
-    "GetPipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "metadata": PipelineMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+PipelineDeclarationUnionTypeDef = Union[
+    PipelineDeclarationTypeDef, PipelineDeclarationOutputTypeDef
+]
 UpdatePipelineInputRequestTypeDef = TypedDict(
     "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 
-UpdatePipelineOutputTypeDef = TypedDict(
-    "UpdatePipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPipelineStateOutputTypeDef = TypedDict(
     "GetPipelineStateOutputTypeDef",
     {
         "pipelineName": str,
         "pipelineVersion": int,
         "stageStates": List[StageStateTypeDef],
         "created": datetime,
         "updated": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListActionExecutionsOutputTypeDef = TypedDict(
     "ListActionExecutionsOutputTypeDef",
     {
         "actionExecutionDetails": List[ActionExecutionDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobDetailsTypeDef = TypedDict(
     "JobDetailsTypeDef",
     {
         "id": str,
@@ -1867,42 +2059,45 @@
     },
     total=False,
 )
 
 GetActionTypeOutputTypeDef = TypedDict(
     "GetActionTypeOutputTypeDef",
     {
-        "actionType": ActionTypeDeclarationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "actionType": ActionTypeDeclarationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ActionTypeDeclarationUnionTypeDef = Union[
+    ActionTypeDeclarationTypeDef, ActionTypeDeclarationOutputTypeDef
+]
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
     },
 )
 
 GetJobDetailsOutputTypeDef = TypedDict(
     "GetJobDetailsOutputTypeDef",
     {
         "jobDetails": JobDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PollForJobsOutputTypeDef = TypedDict(
     "PollForJobsOutputTypeDef",
     {
         "jobs": List[JobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetThirdPartyJobDetailsOutputTypeDef = TypedDict(
     "GetThirdPartyJobDetailsOutputTypeDef",
     {
         "jobDetails": ThirdPartyJobDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline/type_defs.pyi` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_codepipeline.type_defs import AWSSessionCredentialsTypeDef
 
-    data: AWSSessionCredentialsTypeDef = {...}
+    data: AWSSessionCredentialsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -39,149 +39,164 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AWSSessionCredentialsTypeDef",
     "AcknowledgeJobInputRequestTypeDef",
-    "AcknowledgeJobOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
-    "AcknowledgeThirdPartyJobOutputTypeDef",
     "ActionConfigurationPropertyTypeDef",
     "ActionConfigurationTypeDef",
     "ActionContextTypeDef",
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "ActionExecutionFilterTypeDef",
     "ActionExecutionResultTypeDef",
     "ErrorDetailsTypeDef",
-    "ActionRevisionTypeDef",
+    "ActionRevisionOutputTypeDef",
+    "TimestampTypeDef",
     "ActionTypeArtifactDetailsTypeDef",
     "ActionTypeIdentifierTypeDef",
-    "ActionTypePermissionsTypeDef",
+    "ActionTypePermissionsOutputTypeDef",
     "ActionTypePropertyTypeDef",
     "ActionTypeUrlsTypeDef",
+    "ActionTypePermissionsTypeDef",
     "ActionTypeSettingsTypeDef",
     "ArtifactDetailsTypeDef",
     "ApprovalResultTypeDef",
     "S3LocationTypeDef",
     "S3ArtifactLocationTypeDef",
     "ArtifactRevisionTypeDef",
     "EncryptionKeyTypeDef",
     "BlockerDeclarationTypeDef",
     "TagTypeDef",
-    "CurrentRevisionTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
     "ExecutionTriggerTypeDef",
-    "JobWorkerExecutorConfigurationTypeDef",
+    "JobWorkerExecutorConfigurationOutputTypeDef",
     "LambdaExecutorConfigurationTypeDef",
+    "JobWorkerExecutorConfigurationTypeDef",
     "FailureDetailsTypeDef",
     "GetActionTypeInputRequestTypeDef",
     "GetJobDetailsInputRequestTypeDef",
     "GetPipelineExecutionInputRequestTypeDef",
     "GetPipelineInputRequestTypeDef",
     "PipelineMetadataTypeDef",
     "GetPipelineStateInputRequestTypeDef",
     "GetThirdPartyJobDetailsInputRequestTypeDef",
-    "ListActionTypesInputListActionTypesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListActionTypesInputRequestTypeDef",
-    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
     "ListPipelineExecutionsInputRequestTypeDef",
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineSummaryTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListWebhooksInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "StageContextTypeDef",
     "SourceRevisionTypeDef",
     "StopExecutionTriggerTypeDef",
     "ThirdPartyJobTypeDef",
-    "PutActionRevisionOutputTypeDef",
-    "PutApprovalResultOutputTypeDef",
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RetryStageExecutionInputRequestTypeDef",
-    "RetryStageExecutionOutputTypeDef",
     "StageExecutionTypeDef",
     "TransitionStateTypeDef",
     "StartPipelineExecutionInputRequestTypeDef",
-    "StartPipelineExecutionOutputTypeDef",
     "StopPipelineExecutionInputRequestTypeDef",
-    "StopPipelineExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "WebhookAuthConfigurationTypeDef",
     "WebhookFilterRuleTypeDef",
+    "AcknowledgeJobOutputTypeDef",
+    "AcknowledgeThirdPartyJobOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "PutActionRevisionOutputTypeDef",
+    "PutApprovalResultOutputTypeDef",
+    "RetryStageExecutionOutputTypeDef",
+    "StartPipelineExecutionOutputTypeDef",
+    "StopPipelineExecutionOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
+    "ActionDeclarationOutputTypeDef",
     "ActionDeclarationTypeDef",
-    "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionExecutionTypeDef",
-    "PutActionRevisionInputRequestTypeDef",
+    "ActionRevisionTypeDef",
+    "CurrentRevisionTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
     "PipelineExecutionTypeDef",
     "ArtifactStoreTypeDef",
     "CreateCustomActionTypeInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
-    "PutJobSuccessResultInputRequestTypeDef",
-    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
+    "ExecutorConfigurationOutputTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
+    "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    "ListActionTypesInputListActionTypesPaginateTypeDef",
+    "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListPipelinesOutputTypeDef",
     "PipelineContextTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
+    "WebhookDefinitionOutputTypeDef",
     "WebhookDefinitionTypeDef",
+    "StageDeclarationOutputTypeDef",
     "StageDeclarationTypeDef",
     "ActionStateTypeDef",
+    "ActionRevisionUnionTypeDef",
+    "PutActionRevisionInputRequestTypeDef",
+    "PutJobSuccessResultInputRequestTypeDef",
+    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "CreateCustomActionTypeOutputTypeDef",
     "ListActionTypesOutputTypeDef",
     "ActionExecutionInputTypeDef",
     "ActionExecutionOutputTypeDef",
     "ArtifactTypeDef",
     "GetPipelineExecutionOutputTypeDef",
+    "ActionTypeExecutorOutputTypeDef",
     "ActionTypeExecutorTypeDef",
     "ListPipelineExecutionsOutputTypeDef",
     "ListWebhookItemTypeDef",
     "PutWebhookInputRequestTypeDef",
+    "WebhookDefinitionUnionTypeDef",
+    "PipelineDeclarationOutputTypeDef",
     "PipelineDeclarationTypeDef",
     "StageStateTypeDef",
     "ActionExecutionDetailTypeDef",
     "JobDataTypeDef",
     "ThirdPartyJobDataTypeDef",
+    "ActionTypeDeclarationOutputTypeDef",
     "ActionTypeDeclarationTypeDef",
     "ListWebhooksOutputTypeDef",
     "PutWebhookOutputTypeDef",
-    "CreatePipelineInputRequestTypeDef",
     "CreatePipelineOutputTypeDef",
     "GetPipelineOutputTypeDef",
-    "UpdatePipelineInputRequestTypeDef",
     "UpdatePipelineOutputTypeDef",
+    "CreatePipelineInputRequestTypeDef",
+    "PipelineDeclarationUnionTypeDef",
+    "UpdatePipelineInputRequestTypeDef",
     "GetPipelineStateOutputTypeDef",
     "ListActionExecutionsOutputTypeDef",
     "JobDetailsTypeDef",
     "JobTypeDef",
     "ThirdPartyJobDetailsTypeDef",
     "GetActionTypeOutputTypeDef",
+    "ActionTypeDeclarationUnionTypeDef",
     "UpdateActionTypeInputRequestTypeDef",
     "GetJobDetailsOutputTypeDef",
     "PollForJobsOutputTypeDef",
     "GetThirdPartyJobDetailsOutputTypeDef",
 )
 
 AWSSessionCredentialsTypeDef = TypedDict(
@@ -197,39 +212,34 @@
     "AcknowledgeJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
     },
 )
 
-AcknowledgeJobOutputTypeDef = TypedDict(
-    "AcknowledgeJobOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "status": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AcknowledgeThirdPartyJobInputRequestTypeDef = TypedDict(
     "AcknowledgeThirdPartyJobInputRequestTypeDef",
     {
         "jobId": str,
         "nonce": str,
         "clientToken": str,
     },
 )
 
-AcknowledgeThirdPartyJobOutputTypeDef = TypedDict(
-    "AcknowledgeThirdPartyJobOutputTypeDef",
-    {
-        "status": JobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredActionConfigurationPropertyTypeDef = TypedDict(
     "_RequiredActionConfigurationPropertyTypeDef",
     {
         "name": str,
         "required": bool,
         "key": bool,
         "secret": bool,
@@ -314,23 +324,24 @@
     {
         "code": str,
         "message": str,
     },
     total=False,
 )
 
-ActionRevisionTypeDef = TypedDict(
-    "ActionRevisionTypeDef",
+ActionRevisionOutputTypeDef = TypedDict(
+    "ActionRevisionOutputTypeDef",
     {
         "revisionId": str,
         "revisionChangeId": str,
         "created": datetime,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 ActionTypeArtifactDetailsTypeDef = TypedDict(
     "ActionTypeArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
@@ -341,16 +352,16 @@
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
     },
 )
 
-ActionTypePermissionsTypeDef = TypedDict(
-    "ActionTypePermissionsTypeDef",
+ActionTypePermissionsOutputTypeDef = TypedDict(
+    "ActionTypePermissionsOutputTypeDef",
     {
         "allowedAccounts": List[str],
     },
 )
 
 _RequiredActionTypePropertyTypeDef = TypedDict(
     "_RequiredActionTypePropertyTypeDef",
@@ -382,14 +393,21 @@
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
     },
     total=False,
 )
 
+ActionTypePermissionsTypeDef = TypedDict(
+    "ActionTypePermissionsTypeDef",
+    {
+        "allowedAccounts": Sequence[str],
+    },
+)
+
 ActionTypeSettingsTypeDef = TypedDict(
     "ActionTypeSettingsTypeDef",
     {
         "thirdPartyConfigurationUrl": str,
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
@@ -463,33 +481,14 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-_RequiredCurrentRevisionTypeDef = TypedDict(
-    "_RequiredCurrentRevisionTypeDef",
-    {
-        "revision": str,
-        "changeIdentifier": str,
-    },
-)
-_OptionalCurrentRevisionTypeDef = TypedDict(
-    "_OptionalCurrentRevisionTypeDef",
-    {
-        "created": Union[datetime, str],
-        "revisionSummary": str,
-    },
-    total=False,
-)
-
-class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
-    pass
-
 DeleteCustomActionTypeInputRequestTypeDef = TypedDict(
     "DeleteCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
     },
@@ -523,21 +522,14 @@
         "pipelineName": str,
         "stageName": str,
         "transitionType": StageTransitionTypeType,
         "reason": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableStageTransitionInputRequestTypeDef = TypedDict(
     "EnableStageTransitionInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "transitionType": StageTransitionTypeType,
     },
@@ -558,30 +550,39 @@
     {
         "triggerType": TriggerTypeType,
         "triggerDetail": str,
     },
     total=False,
 )
 
-JobWorkerExecutorConfigurationTypeDef = TypedDict(
-    "JobWorkerExecutorConfigurationTypeDef",
+JobWorkerExecutorConfigurationOutputTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationOutputTypeDef",
     {
         "pollingAccounts": List[str],
         "pollingServicePrincipals": List[str],
     },
     total=False,
 )
 
 LambdaExecutorConfigurationTypeDef = TypedDict(
     "LambdaExecutorConfigurationTypeDef",
     {
         "lambdaFunctionArn": str,
     },
 )
 
+JobWorkerExecutorConfigurationTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationTypeDef",
+    {
+        "pollingAccounts": Sequence[str],
+        "pollingServicePrincipals": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredFailureDetailsTypeDef = TypedDict(
     "_RequiredFailureDetailsTypeDef",
     {
         "type": FailureTypeType,
         "message": str,
     },
 )
@@ -662,54 +663,34 @@
     "GetThirdPartyJobDetailsInputRequestTypeDef",
     {
         "jobId": str,
         "clientToken": str,
     },
 )
 
-ListActionTypesInputListActionTypesPaginateTypeDef = TypedDict(
-    "ListActionTypesInputListActionTypesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "actionOwnerFilter": ActionOwnerType,
-        "regionFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListActionTypesInputRequestTypeDef = TypedDict(
     "ListActionTypesInputRequestTypeDef",
     {
         "actionOwnerFilter": ActionOwnerType,
         "nextToken": str,
         "regionFilter": str,
     },
     total=False,
 )
 
-_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "pipelineName": str,
-    },
-)
-_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(
-    _RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-    _OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPipelineExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListPipelineExecutionsInputRequestTypeDef",
     {
         "pipelineName": str,
     },
 )
 _OptionalListPipelineExecutionsInputRequestTypeDef = TypedDict(
@@ -723,22 +704,14 @@
 
 class ListPipelineExecutionsInputRequestTypeDef(
     _RequiredListPipelineExecutionsInputRequestTypeDef,
     _OptionalListPipelineExecutionsInputRequestTypeDef,
 ):
     pass
 
-ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesInputRequestTypeDef = TypedDict(
     "ListPipelinesInputRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -751,34 +724,14 @@
         "version": int,
         "created": datetime,
         "updated": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -791,41 +744,23 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-ListWebhooksInputListWebhooksPaginateTypeDef = TypedDict(
-    "ListWebhooksInputListWebhooksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListWebhooksInputRequestTypeDef = TypedDict(
     "ListWebhooksInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
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
 StageContextTypeDef = TypedDict(
     "StageContextTypeDef",
     {
         "name": str,
     },
     total=False,
 )
@@ -862,68 +797,32 @@
     {
         "clientId": str,
         "jobId": str,
     },
     total=False,
 )
 
-PutActionRevisionOutputTypeDef = TypedDict(
-    "PutActionRevisionOutputTypeDef",
-    {
-        "newRevision": bool,
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutApprovalResultOutputTypeDef = TypedDict(
-    "PutApprovalResultOutputTypeDef",
-    {
-        "approvedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RegisterWebhookWithThirdPartyInputRequestTypeDef = TypedDict(
     "RegisterWebhookWithThirdPartyInputRequestTypeDef",
     {
         "webhookName": str,
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
 RetryStageExecutionInputRequestTypeDef = TypedDict(
     "RetryStageExecutionInputRequestTypeDef",
     {
         "pipelineName": str,
         "stageName": str,
         "pipelineExecutionId": str,
         "retryMode": Literal["FAILED_ACTIONS"],
     },
 )
 
-RetryStageExecutionOutputTypeDef = TypedDict(
-    "RetryStageExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StageExecutionTypeDef = TypedDict(
     "StageExecutionTypeDef",
     {
         "pipelineExecutionId": str,
         "status": StageExecutionStatusType,
     },
 )
@@ -955,22 +854,14 @@
 
 class StartPipelineExecutionInputRequestTypeDef(
     _RequiredStartPipelineExecutionInputRequestTypeDef,
     _OptionalStartPipelineExecutionInputRequestTypeDef,
 ):
     pass
 
-StartPipelineExecutionOutputTypeDef = TypedDict(
-    "StartPipelineExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopPipelineExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStopPipelineExecutionInputRequestTypeDef",
     {
         "pipelineName": str,
         "pipelineExecutionId": str,
     },
 )
@@ -985,22 +876,14 @@
 
 class StopPipelineExecutionInputRequestTypeDef(
     _RequiredStopPipelineExecutionInputRequestTypeDef,
     _OptionalStopPipelineExecutionInputRequestTypeDef,
 ):
     pass
 
-StopPipelineExecutionOutputTypeDef = TypedDict(
-    "StopPipelineExecutionOutputTypeDef",
-    {
-        "pipelineExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1029,14 +912,78 @@
 )
 
 class WebhookFilterRuleTypeDef(
     _RequiredWebhookFilterRuleTypeDef, _OptionalWebhookFilterRuleTypeDef
 ):
     pass
 
+AcknowledgeJobOutputTypeDef = TypedDict(
+    "AcknowledgeJobOutputTypeDef",
+    {
+        "status": JobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AcknowledgeThirdPartyJobOutputTypeDef = TypedDict(
+    "AcknowledgeThirdPartyJobOutputTypeDef",
+    {
+        "status": JobStatusType,
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
+PutActionRevisionOutputTypeDef = TypedDict(
+    "PutActionRevisionOutputTypeDef",
+    {
+        "newRevision": bool,
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutApprovalResultOutputTypeDef = TypedDict(
+    "PutApprovalResultOutputTypeDef",
+    {
+        "approvedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RetryStageExecutionOutputTypeDef = TypedDict(
+    "RetryStageExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartPipelineExecutionOutputTypeDef = TypedDict(
+    "StartPipelineExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopPipelineExecutionOutputTypeDef = TypedDict(
+    "StopPipelineExecutionOutputTypeDef",
+    {
+        "pipelineExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPollForJobsInputRequestTypeDef = TypedDict(
     "_RequiredPollForJobsInputRequestTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
 _OptionalPollForJobsInputRequestTypeDef = TypedDict(
@@ -1069,58 +1016,63 @@
 
 class PollForThirdPartyJobsInputRequestTypeDef(
     _RequiredPollForThirdPartyJobsInputRequestTypeDef,
     _OptionalPollForThirdPartyJobsInputRequestTypeDef,
 ):
     pass
 
-_RequiredActionDeclarationTypeDef = TypedDict(
-    "_RequiredActionDeclarationTypeDef",
+_RequiredActionDeclarationOutputTypeDef = TypedDict(
+    "_RequiredActionDeclarationOutputTypeDef",
     {
         "name": str,
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
-_OptionalActionDeclarationTypeDef = TypedDict(
-    "_OptionalActionDeclarationTypeDef",
+_OptionalActionDeclarationOutputTypeDef = TypedDict(
+    "_OptionalActionDeclarationOutputTypeDef",
     {
         "runOrder": int,
-        "configuration": Mapping[str, str],
-        "outputArtifacts": Sequence[OutputArtifactTypeDef],
-        "inputArtifacts": Sequence[InputArtifactTypeDef],
+        "configuration": Dict[str, str],
+        "outputArtifacts": List[OutputArtifactTypeDef],
+        "inputArtifacts": List[InputArtifactTypeDef],
         "roleArn": str,
         "region": str,
         "namespace": str,
     },
     total=False,
 )
 
-class ActionDeclarationTypeDef(
-    _RequiredActionDeclarationTypeDef, _OptionalActionDeclarationTypeDef
+class ActionDeclarationOutputTypeDef(
+    _RequiredActionDeclarationOutputTypeDef, _OptionalActionDeclarationOutputTypeDef
 ):
     pass
 
-_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+_RequiredActionDeclarationTypeDef = TypedDict(
+    "_RequiredActionDeclarationTypeDef",
     {
-        "pipelineName": str,
+        "name": str,
+        "actionTypeId": ActionTypeIdTypeDef,
     },
 )
-_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+_OptionalActionDeclarationTypeDef = TypedDict(
+    "_OptionalActionDeclarationTypeDef",
     {
-        "filter": ActionExecutionFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "runOrder": int,
+        "configuration": Mapping[str, str],
+        "outputArtifacts": Sequence[OutputArtifactTypeDef],
+        "inputArtifacts": Sequence[InputArtifactTypeDef],
+        "roleArn": str,
+        "region": str,
+        "namespace": str,
     },
     total=False,
 )
 
-class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(
-    _RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef,
-    _OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+class ActionDeclarationTypeDef(
+    _RequiredActionDeclarationTypeDef, _OptionalActionDeclarationTypeDef
 ):
     pass
 
 _RequiredListActionExecutionsInputRequestTypeDef = TypedDict(
     "_RequiredListActionExecutionsInputRequestTypeDef",
     {
         "pipelineName": str,
@@ -1155,24 +1107,42 @@
         "externalExecutionUrl": str,
         "percentComplete": int,
         "errorDetails": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
-PutActionRevisionInputRequestTypeDef = TypedDict(
-    "PutActionRevisionInputRequestTypeDef",
+ActionRevisionTypeDef = TypedDict(
+    "ActionRevisionTypeDef",
     {
-        "pipelineName": str,
-        "stageName": str,
-        "actionName": str,
-        "actionRevision": ActionRevisionTypeDef,
+        "revisionId": str,
+        "revisionChangeId": str,
+        "created": TimestampTypeDef,
+    },
+)
+
+_RequiredCurrentRevisionTypeDef = TypedDict(
+    "_RequiredCurrentRevisionTypeDef",
+    {
+        "revision": str,
+        "changeIdentifier": str,
+    },
+)
+_OptionalCurrentRevisionTypeDef = TypedDict(
+    "_OptionalCurrentRevisionTypeDef",
+    {
+        "created": TimestampTypeDef,
+        "revisionSummary": str,
     },
+    total=False,
 )
 
+class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
+    pass
+
 _RequiredActionTypeTypeDef = TypedDict(
     "_RequiredActionTypeTypeDef",
     {
         "id": ActionTypeIdTypeDef,
         "inputArtifactDetails": ArtifactDetailsTypeDef,
         "outputArtifactDetails": ArtifactDetailsTypeDef,
     },
@@ -1276,103 +1246,154 @@
     pass
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": List[TagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_RequiredPutJobSuccessResultInputRequestTypeDef",
+ExecutorConfigurationOutputTypeDef = TypedDict(
+    "ExecutorConfigurationOutputTypeDef",
+    {
+        "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
+        "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+ExecutorConfigurationTypeDef = TypedDict(
+    "ExecutorConfigurationTypeDef",
+    {
+        "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
+        "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationTypeDef,
+    },
+    total=False,
+)
+
+PutJobFailureResultInputRequestTypeDef = TypedDict(
+    "PutJobFailureResultInputRequestTypeDef",
     {
         "jobId": str,
+        "failureDetails": FailureDetailsTypeDef,
     },
 )
-_OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_OptionalPutJobSuccessResultInputRequestTypeDef",
+
+PutThirdPartyJobFailureResultInputRequestTypeDef = TypedDict(
+    "PutThirdPartyJobFailureResultInputRequestTypeDef",
     {
-        "currentRevision": CurrentRevisionTypeDef,
-        "continuationToken": str,
-        "executionDetails": ExecutionDetailsTypeDef,
-        "outputVariables": Mapping[str, str],
+        "jobId": str,
+        "clientToken": str,
+        "failureDetails": FailureDetailsTypeDef,
+    },
+)
+
+_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    {
+        "pipelineName": str,
+    },
+)
+_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef",
+    {
+        "filter": ActionExecutionFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class PutJobSuccessResultInputRequestTypeDef(
-    _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
+class ListActionExecutionsInputListActionExecutionsPaginateTypeDef(
+    _RequiredListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+    _OptionalListActionExecutionsInputListActionExecutionsPaginateTypeDef,
 ):
     pass
 
-_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
+ListActionTypesInputListActionTypesPaginateTypeDef = TypedDict(
+    "ListActionTypesInputListActionTypesPaginateTypeDef",
     {
-        "jobId": str,
-        "clientToken": str,
+        "actionOwnerFilter": ActionOwnerType,
+        "regionFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef",
+
+_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
     {
-        "currentRevision": CurrentRevisionTypeDef,
-        "continuationToken": str,
-        "executionDetails": ExecutionDetailsTypeDef,
+        "pipelineName": str,
+    },
+)
+_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class PutThirdPartyJobSuccessResultInputRequestTypeDef(
-    _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
-    _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
+class ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef(
+    _RequiredListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+    _OptionalListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
 ):
     pass
 
-ExecutorConfigurationTypeDef = TypedDict(
-    "ExecutorConfigurationTypeDef",
+ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
     {
-        "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
-        "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-PutJobFailureResultInputRequestTypeDef = TypedDict(
-    "PutJobFailureResultInputRequestTypeDef",
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     {
-        "jobId": str,
-        "failureDetails": FailureDetailsTypeDef,
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-PutThirdPartyJobFailureResultInputRequestTypeDef = TypedDict(
-    "PutThirdPartyJobFailureResultInputRequestTypeDef",
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+ListWebhooksInputListWebhooksPaginateTypeDef = TypedDict(
+    "ListWebhooksInputListWebhooksPaginateTypeDef",
     {
-        "jobId": str,
-        "clientToken": str,
-        "failureDetails": FailureDetailsTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelines": List[PipelineSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PipelineContextTypeDef = TypedDict(
     "PipelineContextTypeDef",
     {
         "pipelineName": str,
@@ -1398,30 +1419,62 @@
     total=False,
 )
 
 PollForThirdPartyJobsOutputTypeDef = TypedDict(
     "PollForThirdPartyJobsOutputTypeDef",
     {
         "jobs": List[ThirdPartyJobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+WebhookDefinitionOutputTypeDef = TypedDict(
+    "WebhookDefinitionOutputTypeDef",
+    {
+        "name": str,
+        "targetPipeline": str,
+        "targetAction": str,
+        "filters": List[WebhookFilterRuleTypeDef],
+        "authentication": WebhookAuthenticationTypeType,
+        "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
     },
 )
 
 WebhookDefinitionTypeDef = TypedDict(
     "WebhookDefinitionTypeDef",
     {
         "name": str,
         "targetPipeline": str,
         "targetAction": str,
-        "filters": List[WebhookFilterRuleTypeDef],
+        "filters": Sequence[WebhookFilterRuleTypeDef],
         "authentication": WebhookAuthenticationTypeType,
         "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
     },
 )
 
+_RequiredStageDeclarationOutputTypeDef = TypedDict(
+    "_RequiredStageDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "actions": List[ActionDeclarationOutputTypeDef],
+    },
+)
+_OptionalStageDeclarationOutputTypeDef = TypedDict(
+    "_OptionalStageDeclarationOutputTypeDef",
+    {
+        "blockers": List[BlockerDeclarationTypeDef],
+    },
+    total=False,
+)
+
+class StageDeclarationOutputTypeDef(
+    _RequiredStageDeclarationOutputTypeDef, _OptionalStageDeclarationOutputTypeDef
+):
+    pass
+
 _RequiredStageDeclarationTypeDef = TypedDict(
     "_RequiredStageDeclarationTypeDef",
     {
         "name": str,
         "actions": Sequence[ActionDeclarationTypeDef],
     },
 )
@@ -1436,37 +1489,93 @@
 class StageDeclarationTypeDef(_RequiredStageDeclarationTypeDef, _OptionalStageDeclarationTypeDef):
     pass
 
 ActionStateTypeDef = TypedDict(
     "ActionStateTypeDef",
     {
         "actionName": str,
-        "currentRevision": ActionRevisionTypeDef,
+        "currentRevision": ActionRevisionOutputTypeDef,
         "latestExecution": ActionExecutionTypeDef,
         "entityUrl": str,
         "revisionUrl": str,
     },
     total=False,
 )
 
+ActionRevisionUnionTypeDef = Union[ActionRevisionTypeDef, ActionRevisionOutputTypeDef]
+PutActionRevisionInputRequestTypeDef = TypedDict(
+    "PutActionRevisionInputRequestTypeDef",
+    {
+        "pipelineName": str,
+        "stageName": str,
+        "actionName": str,
+        "actionRevision": ActionRevisionTypeDef,
+    },
+)
+
+_RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_RequiredPutJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+    },
+)
+_OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_OptionalPutJobSuccessResultInputRequestTypeDef",
+    {
+        "currentRevision": CurrentRevisionTypeDef,
+        "continuationToken": str,
+        "executionDetails": ExecutionDetailsTypeDef,
+        "outputVariables": Mapping[str, str],
+    },
+    total=False,
+)
+
+class PutJobSuccessResultInputRequestTypeDef(
+    _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
+):
+    pass
+
+_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+        "clientToken": str,
+    },
+)
+_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "currentRevision": CurrentRevisionTypeDef,
+        "continuationToken": str,
+        "executionDetails": ExecutionDetailsTypeDef,
+    },
+    total=False,
+)
+
+class PutThirdPartyJobSuccessResultInputRequestTypeDef(
+    _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
+    _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
+):
+    pass
+
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListActionTypesOutputTypeDef = TypedDict(
     "ListActionTypesOutputTypeDef",
     {
         "actionTypes": List[ActionTypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActionExecutionInputTypeDef = TypedDict(
     "ActionExecutionInputTypeDef",
     {
         "actionTypeId": ActionTypeIdTypeDef,
@@ -1500,18 +1609,39 @@
     total=False,
 )
 
 GetPipelineExecutionOutputTypeDef = TypedDict(
     "GetPipelineExecutionOutputTypeDef",
     {
         "pipelineExecution": PipelineExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredActionTypeExecutorOutputTypeDef = TypedDict(
+    "_RequiredActionTypeExecutorOutputTypeDef",
+    {
+        "configuration": ExecutorConfigurationOutputTypeDef,
+        "type": ExecutorTypeType,
+    },
+)
+_OptionalActionTypeExecutorOutputTypeDef = TypedDict(
+    "_OptionalActionTypeExecutorOutputTypeDef",
+    {
+        "policyStatementsTemplate": str,
+        "jobTimeout": int,
+    },
+    total=False,
+)
+
+class ActionTypeExecutorOutputTypeDef(
+    _RequiredActionTypeExecutorOutputTypeDef, _OptionalActionTypeExecutorOutputTypeDef
+):
+    pass
+
 _RequiredActionTypeExecutorTypeDef = TypedDict(
     "_RequiredActionTypeExecutorTypeDef",
     {
         "configuration": ExecutorConfigurationTypeDef,
         "type": ExecutorTypeType,
     },
 )
@@ -1530,22 +1660,22 @@
     pass
 
 ListPipelineExecutionsOutputTypeDef = TypedDict(
     "ListPipelineExecutionsOutputTypeDef",
     {
         "pipelineExecutionSummaries": List[PipelineExecutionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListWebhookItemTypeDef = TypedDict(
     "_RequiredListWebhookItemTypeDef",
     {
-        "definition": WebhookDefinitionTypeDef,
+        "definition": WebhookDefinitionOutputTypeDef,
         "url": str,
     },
 )
 _OptionalListWebhookItemTypeDef = TypedDict(
     "_OptionalListWebhookItemTypeDef",
     {
         "errorMessage": str,
@@ -1575,14 +1705,38 @@
 )
 
 class PutWebhookInputRequestTypeDef(
     _RequiredPutWebhookInputRequestTypeDef, _OptionalPutWebhookInputRequestTypeDef
 ):
     pass
 
+WebhookDefinitionUnionTypeDef = Union[WebhookDefinitionTypeDef, WebhookDefinitionOutputTypeDef]
+_RequiredPipelineDeclarationOutputTypeDef = TypedDict(
+    "_RequiredPipelineDeclarationOutputTypeDef",
+    {
+        "name": str,
+        "roleArn": str,
+        "stages": List[StageDeclarationOutputTypeDef],
+    },
+)
+_OptionalPipelineDeclarationOutputTypeDef = TypedDict(
+    "_OptionalPipelineDeclarationOutputTypeDef",
+    {
+        "artifactStore": ArtifactStoreTypeDef,
+        "artifactStores": Dict[str, ArtifactStoreTypeDef],
+        "version": int,
+    },
+    total=False,
+)
+
+class PipelineDeclarationOutputTypeDef(
+    _RequiredPipelineDeclarationOutputTypeDef, _OptionalPipelineDeclarationOutputTypeDef
+):
+    pass
+
 _RequiredPipelineDeclarationTypeDef = TypedDict(
     "_RequiredPipelineDeclarationTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": Sequence[StageDeclarationTypeDef],
     },
@@ -1657,29 +1811,54 @@
         "artifactCredentials": AWSSessionCredentialsTypeDef,
         "continuationToken": str,
         "encryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
+_RequiredActionTypeDeclarationOutputTypeDef = TypedDict(
+    "_RequiredActionTypeDeclarationOutputTypeDef",
+    {
+        "executor": ActionTypeExecutorOutputTypeDef,
+        "id": ActionTypeIdentifierTypeDef,
+        "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
+        "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
+    },
+)
+_OptionalActionTypeDeclarationOutputTypeDef = TypedDict(
+    "_OptionalActionTypeDeclarationOutputTypeDef",
+    {
+        "description": str,
+        "permissions": ActionTypePermissionsOutputTypeDef,
+        "properties": List[ActionTypePropertyTypeDef],
+        "urls": ActionTypeUrlsTypeDef,
+    },
+    total=False,
+)
+
+class ActionTypeDeclarationOutputTypeDef(
+    _RequiredActionTypeDeclarationOutputTypeDef, _OptionalActionTypeDeclarationOutputTypeDef
+):
+    pass
+
 _RequiredActionTypeDeclarationTypeDef = TypedDict(
     "_RequiredActionTypeDeclarationTypeDef",
     {
         "executor": ActionTypeExecutorTypeDef,
         "id": ActionTypeIdentifierTypeDef,
         "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
         "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
     },
 )
 _OptionalActionTypeDeclarationTypeDef = TypedDict(
     "_OptionalActionTypeDeclarationTypeDef",
     {
         "description": str,
         "permissions": ActionTypePermissionsTypeDef,
-        "properties": List[ActionTypePropertyTypeDef],
+        "properties": Sequence[ActionTypePropertyTypeDef],
         "urls": ActionTypeUrlsTypeDef,
     },
     total=False,
 )
 
 class ActionTypeDeclarationTypeDef(
     _RequiredActionTypeDeclarationTypeDef, _OptionalActionTypeDeclarationTypeDef
@@ -1687,23 +1866,49 @@
     pass
 
 ListWebhooksOutputTypeDef = TypedDict(
     "ListWebhooksOutputTypeDef",
     {
         "webhooks": List[ListWebhookItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutWebhookOutputTypeDef = TypedDict(
     "PutWebhookOutputTypeDef",
     {
         "webhook": ListWebhookItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePipelineOutputTypeDef = TypedDict(
+    "CreatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPipelineOutputTypeDef = TypedDict(
+    "GetPipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "metadata": PipelineMetadataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePipelineOutputTypeDef = TypedDict(
+    "UpdatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
@@ -1718,65 +1923,42 @@
 )
 
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
-CreatePipelineOutputTypeDef = TypedDict(
-    "CreatePipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetPipelineOutputTypeDef = TypedDict(
-    "GetPipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "metadata": PipelineMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+PipelineDeclarationUnionTypeDef = Union[
+    PipelineDeclarationTypeDef, PipelineDeclarationOutputTypeDef
+]
 UpdatePipelineInputRequestTypeDef = TypedDict(
     "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 
-UpdatePipelineOutputTypeDef = TypedDict(
-    "UpdatePipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPipelineStateOutputTypeDef = TypedDict(
     "GetPipelineStateOutputTypeDef",
     {
         "pipelineName": str,
         "pipelineVersion": int,
         "stageStates": List[StageStateTypeDef],
         "created": datetime,
         "updated": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListActionExecutionsOutputTypeDef = TypedDict(
     "ListActionExecutionsOutputTypeDef",
     {
         "actionExecutionDetails": List[ActionExecutionDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 JobDetailsTypeDef = TypedDict(
     "JobDetailsTypeDef",
     {
         "id": str,
@@ -1806,42 +1988,45 @@
     },
     total=False,
 )
 
 GetActionTypeOutputTypeDef = TypedDict(
     "GetActionTypeOutputTypeDef",
     {
-        "actionType": ActionTypeDeclarationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "actionType": ActionTypeDeclarationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ActionTypeDeclarationUnionTypeDef = Union[
+    ActionTypeDeclarationTypeDef, ActionTypeDeclarationOutputTypeDef
+]
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
     },
 )
 
 GetJobDetailsOutputTypeDef = TypedDict(
     "GetJobDetailsOutputTypeDef",
     {
         "jobDetails": JobDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PollForJobsOutputTypeDef = TypedDict(
     "PollForJobsOutputTypeDef",
     {
         "jobs": List[JobTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetThirdPartyJobDetailsOutputTypeDef = TypedDict(
     "GetThirdPartyJobDetailsOutputTypeDef",
     {
         "jobDetails": ThirdPartyJobDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/PKG-INFO` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codepipeline
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodePipeline 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodePipeline 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codepipeline type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codepipeline type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codepipeline"></a>
 
 # types-aiobotocore-codepipeline
 
 [![PyPI - types-aiobotocore-codepipeline](https://img.shields.io/pypi/v/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codepipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codepipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codepipeline?color=blue)](https://pypistats.org/packages/types-aiobotocore-codepipeline)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codepipeline)](https://pepy.tech/project/types-aiobotocore-codepipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodePipeline 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
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
 [types-aiobotocore-codepipeline docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/).
 
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
@@ -348,168 +347,183 @@
 )
 
 
 def check_value(value: ActionCategoryType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codepipeline.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codepipeline.type_defs import (
     AWSSessionCredentialsTypeDef,
     AcknowledgeJobInputRequestTypeDef,
-    AcknowledgeJobOutputTypeDef,
+    ResponseMetadataTypeDef,
     AcknowledgeThirdPartyJobInputRequestTypeDef,
-    AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionConfigurationTypeDef,
     ActionContextTypeDef,
     ActionTypeIdTypeDef,
     InputArtifactTypeDef,
     OutputArtifactTypeDef,
     ActionExecutionFilterTypeDef,
     ActionExecutionResultTypeDef,
     ErrorDetailsTypeDef,
-    ActionRevisionTypeDef,
+    ActionRevisionOutputTypeDef,
+    TimestampTypeDef,
     ActionTypeArtifactDetailsTypeDef,
     ActionTypeIdentifierTypeDef,
-    ActionTypePermissionsTypeDef,
+    ActionTypePermissionsOutputTypeDef,
     ActionTypePropertyTypeDef,
     ActionTypeUrlsTypeDef,
+    ActionTypePermissionsTypeDef,
     ActionTypeSettingsTypeDef,
     ArtifactDetailsTypeDef,
     ApprovalResultTypeDef,
     S3LocationTypeDef,
     S3ArtifactLocationTypeDef,
     ArtifactRevisionTypeDef,
     EncryptionKeyTypeDef,
     BlockerDeclarationTypeDef,
     TagTypeDef,
-    CurrentRevisionTypeDef,
     DeleteCustomActionTypeInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
     DeleteWebhookInputRequestTypeDef,
     DeregisterWebhookWithThirdPartyInputRequestTypeDef,
     DisableStageTransitionInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableStageTransitionInputRequestTypeDef,
     ExecutionDetailsTypeDef,
     ExecutionTriggerTypeDef,
-    JobWorkerExecutorConfigurationTypeDef,
+    JobWorkerExecutorConfigurationOutputTypeDef,
     LambdaExecutorConfigurationTypeDef,
+    JobWorkerExecutorConfigurationTypeDef,
     FailureDetailsTypeDef,
     GetActionTypeInputRequestTypeDef,
     GetJobDetailsInputRequestTypeDef,
     GetPipelineExecutionInputRequestTypeDef,
     GetPipelineInputRequestTypeDef,
     PipelineMetadataTypeDef,
     GetPipelineStateInputRequestTypeDef,
     GetThirdPartyJobDetailsInputRequestTypeDef,
-    ListActionTypesInputListActionTypesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListActionTypesInputRequestTypeDef,
-    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
     ListPipelineExecutionsInputRequestTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineSummaryTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListWebhooksInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     StageContextTypeDef,
     SourceRevisionTypeDef,
     StopExecutionTriggerTypeDef,
     ThirdPartyJobTypeDef,
-    PutActionRevisionOutputTypeDef,
-    PutApprovalResultOutputTypeDef,
     RegisterWebhookWithThirdPartyInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     RetryStageExecutionInputRequestTypeDef,
-    RetryStageExecutionOutputTypeDef,
     StageExecutionTypeDef,
     TransitionStateTypeDef,
     StartPipelineExecutionInputRequestTypeDef,
-    StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionInputRequestTypeDef,
-    StopPipelineExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     WebhookAuthConfigurationTypeDef,
     WebhookFilterRuleTypeDef,
+    AcknowledgeJobOutputTypeDef,
+    AcknowledgeThirdPartyJobOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    PutActionRevisionOutputTypeDef,
+    PutApprovalResultOutputTypeDef,
+    RetryStageExecutionOutputTypeDef,
+    StartPipelineExecutionOutputTypeDef,
+    StopPipelineExecutionOutputTypeDef,
     PollForJobsInputRequestTypeDef,
     PollForThirdPartyJobsInputRequestTypeDef,
+    ActionDeclarationOutputTypeDef,
     ActionDeclarationTypeDef,
-    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
     ListActionExecutionsInputRequestTypeDef,
     ActionExecutionTypeDef,
-    PutActionRevisionInputRequestTypeDef,
+    ActionRevisionTypeDef,
+    CurrentRevisionTypeDef,
     ActionTypeTypeDef,
     PutApprovalResultInputRequestTypeDef,
     ArtifactDetailTypeDef,
     ArtifactLocationTypeDef,
     PipelineExecutionTypeDef,
     ArtifactStoreTypeDef,
     CreateCustomActionTypeInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
-    PutJobSuccessResultInputRequestTypeDef,
-    PutThirdPartyJobSuccessResultInputRequestTypeDef,
+    ExecutorConfigurationOutputTypeDef,
     ExecutorConfigurationTypeDef,
     PutJobFailureResultInputRequestTypeDef,
     PutThirdPartyJobFailureResultInputRequestTypeDef,
+    ListActionExecutionsInputListActionExecutionsPaginateTypeDef,
+    ListActionTypesInputListActionTypesPaginateTypeDef,
+    ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListWebhooksInputListWebhooksPaginateTypeDef,
     ListPipelinesOutputTypeDef,
     PipelineContextTypeDef,
     PipelineExecutionSummaryTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
+    WebhookDefinitionOutputTypeDef,
     WebhookDefinitionTypeDef,
+    StageDeclarationOutputTypeDef,
     StageDeclarationTypeDef,
     ActionStateTypeDef,
+    ActionRevisionUnionTypeDef,
+    PutActionRevisionInputRequestTypeDef,
+    PutJobSuccessResultInputRequestTypeDef,
+    PutThirdPartyJobSuccessResultInputRequestTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ActionExecutionInputTypeDef,
     ActionExecutionOutputTypeDef,
     ArtifactTypeDef,
     GetPipelineExecutionOutputTypeDef,
+    ActionTypeExecutorOutputTypeDef,
     ActionTypeExecutorTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListWebhookItemTypeDef,
     PutWebhookInputRequestTypeDef,
+    WebhookDefinitionUnionTypeDef,
+    PipelineDeclarationOutputTypeDef,
     PipelineDeclarationTypeDef,
     StageStateTypeDef,
     ActionExecutionDetailTypeDef,
     JobDataTypeDef,
     ThirdPartyJobDataTypeDef,
+    ActionTypeDeclarationOutputTypeDef,
     ActionTypeDeclarationTypeDef,
     ListWebhooksOutputTypeDef,
     PutWebhookOutputTypeDef,
-    CreatePipelineInputRequestTypeDef,
     CreatePipelineOutputTypeDef,
     GetPipelineOutputTypeDef,
-    UpdatePipelineInputRequestTypeDef,
     UpdatePipelineOutputTypeDef,
+    CreatePipelineInputRequestTypeDef,
+    PipelineDeclarationUnionTypeDef,
+    UpdatePipelineInputRequestTypeDef,
     GetPipelineStateOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     JobDetailsTypeDef,
     JobTypeDef,
     ThirdPartyJobDetailsTypeDef,
     GetActionTypeOutputTypeDef,
+    ActionTypeDeclarationUnionTypeDef,
     UpdateActionTypeInputRequestTypeDef,
     GetJobDetailsOutputTypeDef,
     PollForJobsOutputTypeDef,
     GetThirdPartyJobDetailsOutputTypeDef,
 )
 
 
-def get_structure() -> AWSSessionCredentialsTypeDef:
+def get_value() -> AWSSessionCredentialsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codepipeline-2.5.2/types_aiobotocore_codepipeline.egg-info/SOURCES.txt` & `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*


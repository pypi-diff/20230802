# Comparing `tmp/types-aiobotocore-imagebuilder-2.5.2.tar.gz` & `tmp/types-aiobotocore-imagebuilder-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-imagebuilder-2.5.2.tar", last modified: Sat Jul  8 01:43:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-imagebuilder-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
```

## Comparing `types-aiobotocore-imagebuilder-2.5.2.tar` & `types-aiobotocore-imagebuilder-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.090253 types-aiobotocore-imagebuilder-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:09.000000 types-aiobotocore-imagebuilder-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19842 2023-07-08 01:43:44.082253 types-aiobotocore-imagebuilder-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-07-08 01:32:09.000000 types-aiobotocore-imagebuilder-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:44.090253 types-aiobotocore-imagebuilder-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:32:09.000000 types-aiobotocore-imagebuilder-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.082253 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-08 01:32:09.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-08 01:32:09.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:32:09.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44284 2023-07-08 01:32:10.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    44219 2023-07-08 01:32:10.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-08 01:32:10.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-07-08 01:32:10.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:09.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    66695 2023-07-08 01:32:11.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-07-08 01:32:11.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:09.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.082253 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19842 2023-07-08 01:43:43.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-08 01:43:43.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:43.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:43.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:43.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:43.000000 types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.033570 types-aiobotocore-imagebuilder-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20308 2023-08-02 14:52:24.033570 types-aiobotocore-imagebuilder-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18770 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.033570 types-aiobotocore-imagebuilder-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.033570 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44344 2023-08-02 14:40:09.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44279 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-08-02 14:40:10.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-08-02 14:40:10.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    71029 2023-08-02 14:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70968 2023-08-02 14:40:11.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.033570 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20308 2023-08-02 14:52:23.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:52:23.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:23.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:23.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:23.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:23.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2/LICENSE` & `types-aiobotocore-imagebuilder-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.5.2/PKG-INFO` & `types-aiobotocore-imagebuilder-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-imagebuilder
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.imagebuilder 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.imagebuilder 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore imagebuilder type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore imagebuilder type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-imagebuilder"></a>
 
 # types-aiobotocore-imagebuilder
 
 [![PyPI - types-aiobotocore-imagebuilder](https://img.shields.io/pypi/v/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-imagebuilder?color=blue)](https://pypistats.org/packages/types-aiobotocore-imagebuilder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-imagebuilder)](https://pepy.tech/project/types-aiobotocore-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.imagebuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [types-aiobotocore-imagebuilder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/).
 
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
@@ -299,143 +298,150 @@
 )
 
 
 def check_value(value: BuildTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_imagebuilder.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_imagebuilder.type_defs import (
     SeverityCountsTypeDef,
     SystemsManagerAgentTypeDef,
+    LaunchPermissionConfigurationOutputTypeDef,
     LaunchPermissionConfigurationTypeDef,
     ImageStateTypeDef,
     CancelImageCreationRequestRequestTypeDef,
-    CancelImageCreationResponseTypeDef,
+    ResponseMetadataTypeDef,
+    ComponentParameterOutputTypeDef,
     ComponentParameterTypeDef,
     ComponentParameterDetailTypeDef,
     ComponentStateTypeDef,
     ComponentVersionTypeDef,
     TargetContainerRepositoryTypeDef,
     ContainerRecipeSummaryTypeDef,
     ContainerTypeDef,
     CreateComponentRequestRequestTypeDef,
-    CreateComponentResponseTypeDef,
-    CreateContainerRecipeResponseTypeDef,
-    CreateDistributionConfigurationResponseTypeDef,
     ImageTestsConfigurationTypeDef,
     ScheduleTypeDef,
-    CreateImagePipelineResponseTypeDef,
-    CreateImageRecipeResponseTypeDef,
-    CreateImageResponseTypeDef,
     InstanceMetadataOptionsTypeDef,
-    CreateInfrastructureConfigurationResponseTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteComponentRequestRequestTypeDef,
-    DeleteComponentResponseTypeDef,
     DeleteContainerRecipeRequestRequestTypeDef,
-    DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationRequestRequestTypeDef,
-    DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineRequestRequestTypeDef,
-    DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeRequestRequestTypeDef,
-    DeleteImageRecipeResponseTypeDef,
     DeleteImageRequestRequestTypeDef,
-    DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationRequestRequestTypeDef,
-    DeleteInfrastructureConfigurationResponseTypeDef,
     DistributionConfigurationSummaryTypeDef,
     LaunchTemplateConfigurationTypeDef,
     S3ExportConfigurationTypeDef,
     EbsInstanceBlockDeviceSpecificationTypeDef,
+    EcrConfigurationOutputTypeDef,
     EcrConfigurationTypeDef,
     FastLaunchLaunchTemplateSpecificationTypeDef,
     FastLaunchSnapshotConfigurationTypeDef,
     FilterTypeDef,
     GetComponentPolicyRequestRequestTypeDef,
-    GetComponentPolicyResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetContainerRecipePolicyRequestRequestTypeDef,
-    GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeRequestRequestTypeDef,
     GetDistributionConfigurationRequestRequestTypeDef,
     GetImagePipelineRequestRequestTypeDef,
     GetImagePolicyRequestRequestTypeDef,
-    GetImagePolicyResponseTypeDef,
     GetImageRecipePolicyRequestRequestTypeDef,
-    GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeRequestRequestTypeDef,
     GetImageRequestRequestTypeDef,
     GetInfrastructureConfigurationRequestRequestTypeDef,
     GetWorkflowExecutionRequestRequestTypeDef,
-    GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionRequestRequestTypeDef,
-    GetWorkflowStepExecutionResponseTypeDef,
     ImagePackageTypeDef,
     ImageRecipeSummaryTypeDef,
     ImageScanFindingsFilterTypeDef,
     ImageScanStateTypeDef,
     ImageVersionTypeDef,
     ImportComponentRequestRequestTypeDef,
-    ImportComponentResponseTypeDef,
     ImportVmImageRequestRequestTypeDef,
-    ImportVmImageResponseTypeDef,
     InfrastructureConfigurationSummaryTypeDef,
     ListComponentBuildVersionsRequestRequestTypeDef,
     ListImagePackagesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkflowExecutionsRequestRequestTypeDef,
     WorkflowExecutionMetadataTypeDef,
     ListWorkflowStepExecutionsRequestRequestTypeDef,
     WorkflowStepMetadataTypeDef,
     S3LogsTypeDef,
     VulnerablePackageTypeDef,
     PutComponentPolicyRequestRequestTypeDef,
-    PutComponentPolicyResponseTypeDef,
     PutContainerRecipePolicyRequestRequestTypeDef,
-    PutContainerRecipePolicyResponseTypeDef,
     PutImagePolicyRequestRequestTypeDef,
-    PutImagePolicyResponseTypeDef,
     PutImageRecipePolicyRequestRequestTypeDef,
-    PutImageRecipePolicyResponseTypeDef,
     RemediationRecommendationTypeDef,
-    ResponseMetadataTypeDef,
     StartImagePipelineExecutionRequestRequestTypeDef,
-    StartImagePipelineExecutionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateDistributionConfigurationResponseTypeDef,
-    UpdateImagePipelineResponseTypeDef,
-    UpdateInfrastructureConfigurationResponseTypeDef,
     AccountAggregationTypeDef,
     ImageAggregationTypeDef,
     ImagePipelineAggregationTypeDef,
     VulnerabilityIdAggregationTypeDef,
     AdditionalInstanceConfigurationTypeDef,
+    AmiDistributionConfigurationOutputTypeDef,
     AmiDistributionConfigurationTypeDef,
     AmiTypeDef,
+    CancelImageCreationResponseTypeDef,
+    CreateComponentResponseTypeDef,
+    CreateContainerRecipeResponseTypeDef,
+    CreateDistributionConfigurationResponseTypeDef,
+    CreateImagePipelineResponseTypeDef,
+    CreateImageRecipeResponseTypeDef,
+    CreateImageResponseTypeDef,
+    CreateInfrastructureConfigurationResponseTypeDef,
+    DeleteComponentResponseTypeDef,
+    DeleteContainerRecipeResponseTypeDef,
+    DeleteDistributionConfigurationResponseTypeDef,
+    DeleteImagePipelineResponseTypeDef,
+    DeleteImageRecipeResponseTypeDef,
+    DeleteImageResponseTypeDef,
+    DeleteInfrastructureConfigurationResponseTypeDef,
+    GetComponentPolicyResponseTypeDef,
+    GetContainerRecipePolicyResponseTypeDef,
+    GetImagePolicyResponseTypeDef,
+    GetImageRecipePolicyResponseTypeDef,
+    GetWorkflowExecutionResponseTypeDef,
+    GetWorkflowStepExecutionResponseTypeDef,
+    ImportComponentResponseTypeDef,
+    ImportVmImageResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutComponentPolicyResponseTypeDef,
+    PutContainerRecipePolicyResponseTypeDef,
+    PutImagePolicyResponseTypeDef,
+    PutImageRecipePolicyResponseTypeDef,
+    StartImagePipelineExecutionResponseTypeDef,
+    UpdateDistributionConfigurationResponseTypeDef,
+    UpdateImagePipelineResponseTypeDef,
+    UpdateInfrastructureConfigurationResponseTypeDef,
+    ComponentConfigurationOutputTypeDef,
     ComponentConfigurationTypeDef,
     ComponentSummaryTypeDef,
     ComponentTypeDef,
     ListComponentsResponseTypeDef,
+    ContainerDistributionConfigurationOutputTypeDef,
     ContainerDistributionConfigurationTypeDef,
     ListContainerRecipesResponseTypeDef,
     CvssScoreDetailsTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
     InstanceBlockDeviceMappingTypeDef,
+    ImageScanningConfigurationOutputTypeDef,
     ImageScanningConfigurationTypeDef,
     FastLaunchConfigurationTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListContainerRecipesRequestRequestTypeDef,
     ListDistributionConfigurationsRequestRequestTypeDef,
     ListImageBuildVersionsRequestRequestTypeDef,
     ListImagePipelineImagesRequestRequestTypeDef,
@@ -452,51 +458,57 @@
     ListWorkflowExecutionsResponseTypeDef,
     ListWorkflowStepExecutionsResponseTypeDef,
     LoggingTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ImageScanFindingAggregationTypeDef,
     OutputResourcesTypeDef,
+    ComponentConfigurationUnionTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     GetComponentResponseTypeDef,
     InspectorScoreDetailsTypeDef,
-    CreateImageRecipeRequestRequestTypeDef,
     ImageRecipeTypeDef,
+    InstanceConfigurationOutputTypeDef,
     InstanceConfigurationTypeDef,
+    ImagePipelineTypeDef,
     CreateImagePipelineRequestRequestTypeDef,
     CreateImageRequestRequestTypeDef,
-    ImagePipelineTypeDef,
+    ImageScanningConfigurationUnionTypeDef,
     UpdateImagePipelineRequestRequestTypeDef,
+    DistributionOutputTypeDef,
     DistributionTypeDef,
     CreateInfrastructureConfigurationRequestRequestTypeDef,
     InfrastructureConfigurationTypeDef,
     UpdateInfrastructureConfigurationRequestRequestTypeDef,
     ListImageScanFindingAggregationsResponseTypeDef,
     ImageSummaryTypeDef,
+    CreateImageRecipeRequestRequestTypeDef,
     ImageScanFindingTypeDef,
     GetImageRecipeResponseTypeDef,
     ContainerRecipeTypeDef,
     CreateContainerRecipeRequestRequestTypeDef,
+    InstanceConfigurationUnionTypeDef,
     GetImagePipelineResponseTypeDef,
     ListImagePipelinesResponseTypeDef,
-    CreateDistributionConfigurationRequestRequestTypeDef,
     DistributionConfigurationTypeDef,
-    UpdateDistributionConfigurationRequestRequestTypeDef,
+    DistributionUnionTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePipelineImagesResponseTypeDef,
     ListImageScanFindingsResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
     ImageTypeDef,
+    CreateDistributionConfigurationRequestRequestTypeDef,
+    UpdateDistributionConfigurationRequestRequestTypeDef,
     GetImageResponseTypeDef,
 )
 
 
-def get_structure() -> SeverityCountsTypeDef:
+def get_value() -> SeverityCountsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2/README.md` & `types-aiobotocore-imagebuilder-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-imagebuilder"></a>
 
 # types-aiobotocore-imagebuilder
 
 [![PyPI - types-aiobotocore-imagebuilder](https://img.shields.io/pypi/v/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-imagebuilder?color=blue)](https://pypistats.org/packages/types-aiobotocore-imagebuilder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-imagebuilder)](https://pepy.tech/project/types-aiobotocore-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.imagebuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [types-aiobotocore-imagebuilder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/).
 
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
@@ -266,143 +266,150 @@
 )
 
 
 def check_value(value: BuildTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_imagebuilder.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_imagebuilder.type_defs import (
     SeverityCountsTypeDef,
     SystemsManagerAgentTypeDef,
+    LaunchPermissionConfigurationOutputTypeDef,
     LaunchPermissionConfigurationTypeDef,
     ImageStateTypeDef,
     CancelImageCreationRequestRequestTypeDef,
-    CancelImageCreationResponseTypeDef,
+    ResponseMetadataTypeDef,
+    ComponentParameterOutputTypeDef,
     ComponentParameterTypeDef,
     ComponentParameterDetailTypeDef,
     ComponentStateTypeDef,
     ComponentVersionTypeDef,
     TargetContainerRepositoryTypeDef,
     ContainerRecipeSummaryTypeDef,
     ContainerTypeDef,
     CreateComponentRequestRequestTypeDef,
-    CreateComponentResponseTypeDef,
-    CreateContainerRecipeResponseTypeDef,
-    CreateDistributionConfigurationResponseTypeDef,
     ImageTestsConfigurationTypeDef,
     ScheduleTypeDef,
-    CreateImagePipelineResponseTypeDef,
-    CreateImageRecipeResponseTypeDef,
-    CreateImageResponseTypeDef,
     InstanceMetadataOptionsTypeDef,
-    CreateInfrastructureConfigurationResponseTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteComponentRequestRequestTypeDef,
-    DeleteComponentResponseTypeDef,
     DeleteContainerRecipeRequestRequestTypeDef,
-    DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationRequestRequestTypeDef,
-    DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineRequestRequestTypeDef,
-    DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeRequestRequestTypeDef,
-    DeleteImageRecipeResponseTypeDef,
     DeleteImageRequestRequestTypeDef,
-    DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationRequestRequestTypeDef,
-    DeleteInfrastructureConfigurationResponseTypeDef,
     DistributionConfigurationSummaryTypeDef,
     LaunchTemplateConfigurationTypeDef,
     S3ExportConfigurationTypeDef,
     EbsInstanceBlockDeviceSpecificationTypeDef,
+    EcrConfigurationOutputTypeDef,
     EcrConfigurationTypeDef,
     FastLaunchLaunchTemplateSpecificationTypeDef,
     FastLaunchSnapshotConfigurationTypeDef,
     FilterTypeDef,
     GetComponentPolicyRequestRequestTypeDef,
-    GetComponentPolicyResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetContainerRecipePolicyRequestRequestTypeDef,
-    GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeRequestRequestTypeDef,
     GetDistributionConfigurationRequestRequestTypeDef,
     GetImagePipelineRequestRequestTypeDef,
     GetImagePolicyRequestRequestTypeDef,
-    GetImagePolicyResponseTypeDef,
     GetImageRecipePolicyRequestRequestTypeDef,
-    GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeRequestRequestTypeDef,
     GetImageRequestRequestTypeDef,
     GetInfrastructureConfigurationRequestRequestTypeDef,
     GetWorkflowExecutionRequestRequestTypeDef,
-    GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionRequestRequestTypeDef,
-    GetWorkflowStepExecutionResponseTypeDef,
     ImagePackageTypeDef,
     ImageRecipeSummaryTypeDef,
     ImageScanFindingsFilterTypeDef,
     ImageScanStateTypeDef,
     ImageVersionTypeDef,
     ImportComponentRequestRequestTypeDef,
-    ImportComponentResponseTypeDef,
     ImportVmImageRequestRequestTypeDef,
-    ImportVmImageResponseTypeDef,
     InfrastructureConfigurationSummaryTypeDef,
     ListComponentBuildVersionsRequestRequestTypeDef,
     ListImagePackagesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkflowExecutionsRequestRequestTypeDef,
     WorkflowExecutionMetadataTypeDef,
     ListWorkflowStepExecutionsRequestRequestTypeDef,
     WorkflowStepMetadataTypeDef,
     S3LogsTypeDef,
     VulnerablePackageTypeDef,
     PutComponentPolicyRequestRequestTypeDef,
-    PutComponentPolicyResponseTypeDef,
     PutContainerRecipePolicyRequestRequestTypeDef,
-    PutContainerRecipePolicyResponseTypeDef,
     PutImagePolicyRequestRequestTypeDef,
-    PutImagePolicyResponseTypeDef,
     PutImageRecipePolicyRequestRequestTypeDef,
-    PutImageRecipePolicyResponseTypeDef,
     RemediationRecommendationTypeDef,
-    ResponseMetadataTypeDef,
     StartImagePipelineExecutionRequestRequestTypeDef,
-    StartImagePipelineExecutionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateDistributionConfigurationResponseTypeDef,
-    UpdateImagePipelineResponseTypeDef,
-    UpdateInfrastructureConfigurationResponseTypeDef,
     AccountAggregationTypeDef,
     ImageAggregationTypeDef,
     ImagePipelineAggregationTypeDef,
     VulnerabilityIdAggregationTypeDef,
     AdditionalInstanceConfigurationTypeDef,
+    AmiDistributionConfigurationOutputTypeDef,
     AmiDistributionConfigurationTypeDef,
     AmiTypeDef,
+    CancelImageCreationResponseTypeDef,
+    CreateComponentResponseTypeDef,
+    CreateContainerRecipeResponseTypeDef,
+    CreateDistributionConfigurationResponseTypeDef,
+    CreateImagePipelineResponseTypeDef,
+    CreateImageRecipeResponseTypeDef,
+    CreateImageResponseTypeDef,
+    CreateInfrastructureConfigurationResponseTypeDef,
+    DeleteComponentResponseTypeDef,
+    DeleteContainerRecipeResponseTypeDef,
+    DeleteDistributionConfigurationResponseTypeDef,
+    DeleteImagePipelineResponseTypeDef,
+    DeleteImageRecipeResponseTypeDef,
+    DeleteImageResponseTypeDef,
+    DeleteInfrastructureConfigurationResponseTypeDef,
+    GetComponentPolicyResponseTypeDef,
+    GetContainerRecipePolicyResponseTypeDef,
+    GetImagePolicyResponseTypeDef,
+    GetImageRecipePolicyResponseTypeDef,
+    GetWorkflowExecutionResponseTypeDef,
+    GetWorkflowStepExecutionResponseTypeDef,
+    ImportComponentResponseTypeDef,
+    ImportVmImageResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutComponentPolicyResponseTypeDef,
+    PutContainerRecipePolicyResponseTypeDef,
+    PutImagePolicyResponseTypeDef,
+    PutImageRecipePolicyResponseTypeDef,
+    StartImagePipelineExecutionResponseTypeDef,
+    UpdateDistributionConfigurationResponseTypeDef,
+    UpdateImagePipelineResponseTypeDef,
+    UpdateInfrastructureConfigurationResponseTypeDef,
+    ComponentConfigurationOutputTypeDef,
     ComponentConfigurationTypeDef,
     ComponentSummaryTypeDef,
     ComponentTypeDef,
     ListComponentsResponseTypeDef,
+    ContainerDistributionConfigurationOutputTypeDef,
     ContainerDistributionConfigurationTypeDef,
     ListContainerRecipesResponseTypeDef,
     CvssScoreDetailsTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
     InstanceBlockDeviceMappingTypeDef,
+    ImageScanningConfigurationOutputTypeDef,
     ImageScanningConfigurationTypeDef,
     FastLaunchConfigurationTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListContainerRecipesRequestRequestTypeDef,
     ListDistributionConfigurationsRequestRequestTypeDef,
     ListImageBuildVersionsRequestRequestTypeDef,
     ListImagePipelineImagesRequestRequestTypeDef,
@@ -419,51 +426,57 @@
     ListWorkflowExecutionsResponseTypeDef,
     ListWorkflowStepExecutionsResponseTypeDef,
     LoggingTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ImageScanFindingAggregationTypeDef,
     OutputResourcesTypeDef,
+    ComponentConfigurationUnionTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     GetComponentResponseTypeDef,
     InspectorScoreDetailsTypeDef,
-    CreateImageRecipeRequestRequestTypeDef,
     ImageRecipeTypeDef,
+    InstanceConfigurationOutputTypeDef,
     InstanceConfigurationTypeDef,
+    ImagePipelineTypeDef,
     CreateImagePipelineRequestRequestTypeDef,
     CreateImageRequestRequestTypeDef,
-    ImagePipelineTypeDef,
+    ImageScanningConfigurationUnionTypeDef,
     UpdateImagePipelineRequestRequestTypeDef,
+    DistributionOutputTypeDef,
     DistributionTypeDef,
     CreateInfrastructureConfigurationRequestRequestTypeDef,
     InfrastructureConfigurationTypeDef,
     UpdateInfrastructureConfigurationRequestRequestTypeDef,
     ListImageScanFindingAggregationsResponseTypeDef,
     ImageSummaryTypeDef,
+    CreateImageRecipeRequestRequestTypeDef,
     ImageScanFindingTypeDef,
     GetImageRecipeResponseTypeDef,
     ContainerRecipeTypeDef,
     CreateContainerRecipeRequestRequestTypeDef,
+    InstanceConfigurationUnionTypeDef,
     GetImagePipelineResponseTypeDef,
     ListImagePipelinesResponseTypeDef,
-    CreateDistributionConfigurationRequestRequestTypeDef,
     DistributionConfigurationTypeDef,
-    UpdateDistributionConfigurationRequestRequestTypeDef,
+    DistributionUnionTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePipelineImagesResponseTypeDef,
     ListImageScanFindingsResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
     ImageTypeDef,
+    CreateDistributionConfigurationRequestRequestTypeDef,
+    UpdateDistributionConfigurationRequestRequestTypeDef,
     GetImageResponseTypeDef,
 )
 
 
-def get_structure() -> SeverityCountsTypeDef:
+def get_value() -> SeverityCountsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2/setup.py` & `types-aiobotocore-imagebuilder-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-imagebuilder",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_imagebuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.imagebuilder 2.5.2 service generated with"
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
-    keywords="aiobotocore imagebuilder type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore imagebuilder type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_imagebuilder": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/"
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/__main__.py` & `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.imagebuilder 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.imagebuilder 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder\nOther"
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

### Comparing `types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/client.py` & `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ComponentTypeType, OwnershipType, PipelineStatusType, PlatformType
 from .type_defs import (
     AdditionalInstanceConfigurationTypeDef,
     CancelImageCreationResponseTypeDef,
-    ComponentConfigurationTypeDef,
+    ComponentConfigurationUnionTypeDef,
     CreateComponentResponseTypeDef,
     CreateContainerRecipeResponseTypeDef,
     CreateDistributionConfigurationResponseTypeDef,
     CreateImagePipelineResponseTypeDef,
     CreateImageRecipeResponseTypeDef,
     CreateImageResponseTypeDef,
     CreateInfrastructureConfigurationResponseTypeDef,
     DeleteComponentResponseTypeDef,
     DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeResponseTypeDef,
     DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationResponseTypeDef,
-    DistributionTypeDef,
+    DistributionUnionTypeDef,
     FilterTypeDef,
     GetComponentPolicyResponseTypeDef,
     GetComponentResponseTypeDef,
     GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
     GetImagePipelineResponseTypeDef,
@@ -51,20 +51,20 @@
     GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeResponseTypeDef,
     GetImageResponseTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionResponseTypeDef,
     ImageScanFindingsFilterTypeDef,
-    ImageScanningConfigurationTypeDef,
+    ImageScanningConfigurationUnionTypeDef,
     ImageTestsConfigurationTypeDef,
     ImportComponentResponseTypeDef,
     ImportVmImageResponseTypeDef,
     InstanceBlockDeviceMappingTypeDef,
-    InstanceConfigurationTypeDef,
+    InstanceConfigurationUnionTypeDef,
     InstanceMetadataOptionsTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListContainerRecipesResponseTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePackagesResponseTypeDef,
@@ -197,20 +197,20 @@
 
     async def create_container_recipe(
         self,
         *,
         containerType: Literal["DOCKER"],
         name: str,
         semanticVersion: str,
-        components: Sequence[ComponentConfigurationTypeDef],
+        components: Sequence[ComponentConfigurationUnionTypeDef],
         parentImage: str,
         targetRepository: TargetContainerRepositoryTypeDef,
         clientToken: str,
         description: str = ...,
-        instanceConfiguration: InstanceConfigurationTypeDef = ...,
+        instanceConfiguration: InstanceConfigurationUnionTypeDef = ...,
         dockerfileTemplateData: str = ...,
         dockerfileTemplateUri: str = ...,
         platformOverride: PlatformType = ...,
         imageOsVersionOverride: str = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         kmsKeyId: str = ...
@@ -222,15 +222,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_container_recipe)
         """
 
     async def create_distribution_configuration(
         self,
         *,
         name: str,
-        distributions: Sequence[DistributionTypeDef],
+        distributions: Sequence[DistributionUnionTypeDef],
         clientToken: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDistributionConfigurationResponseTypeDef:
         """
         Creates a new distribution configuration.
 
@@ -245,15 +245,15 @@
         clientToken: str,
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
+        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
     ) -> CreateImageResponseTypeDef:
         """
         Creates a new image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image)
         """
@@ -269,29 +269,29 @@
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
+        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
     ) -> CreateImagePipelineResponseTypeDef:
         """
         Creates a new image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image_pipeline)
         """
 
     async def create_image_recipe(
         self,
         *,
         name: str,
         semanticVersion: str,
-        components: Sequence[ComponentConfigurationTypeDef],
+        components: Sequence[ComponentConfigurationUnionTypeDef],
         parentImage: str,
         clientToken: str,
         description: str = ...,
         blockDeviceMappings: Sequence[InstanceBlockDeviceMappingTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...
@@ -839,15 +839,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#untag_resource)
         """
 
     async def update_distribution_configuration(
         self,
         *,
         distributionConfigurationArn: str,
-        distributions: Sequence[DistributionTypeDef],
+        distributions: Sequence[DistributionUnionTypeDef],
         clientToken: str,
         description: str = ...
     ) -> UpdateDistributionConfigurationResponseTypeDef:
         """
         Updates a new distribution configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_distribution_configuration)
@@ -864,15 +864,15 @@
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
-        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
+        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
     ) -> UpdateImagePipelineResponseTypeDef:
         """
         Updates an image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_image_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#update_image_pipeline)
         """
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/client.pyi` & `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ComponentTypeType, OwnershipType, PipelineStatusType, PlatformType
 from .type_defs import (
     AdditionalInstanceConfigurationTypeDef,
     CancelImageCreationResponseTypeDef,
-    ComponentConfigurationTypeDef,
+    ComponentConfigurationUnionTypeDef,
     CreateComponentResponseTypeDef,
     CreateContainerRecipeResponseTypeDef,
     CreateDistributionConfigurationResponseTypeDef,
     CreateImagePipelineResponseTypeDef,
     CreateImageRecipeResponseTypeDef,
     CreateImageResponseTypeDef,
     CreateInfrastructureConfigurationResponseTypeDef,
     DeleteComponentResponseTypeDef,
     DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeResponseTypeDef,
     DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationResponseTypeDef,
-    DistributionTypeDef,
+    DistributionUnionTypeDef,
     FilterTypeDef,
     GetComponentPolicyResponseTypeDef,
     GetComponentResponseTypeDef,
     GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
     GetImagePipelineResponseTypeDef,
@@ -51,20 +51,20 @@
     GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeResponseTypeDef,
     GetImageResponseTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionResponseTypeDef,
     ImageScanFindingsFilterTypeDef,
-    ImageScanningConfigurationTypeDef,
+    ImageScanningConfigurationUnionTypeDef,
     ImageTestsConfigurationTypeDef,
     ImportComponentResponseTypeDef,
     ImportVmImageResponseTypeDef,
     InstanceBlockDeviceMappingTypeDef,
-    InstanceConfigurationTypeDef,
+    InstanceConfigurationUnionTypeDef,
     InstanceMetadataOptionsTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListContainerRecipesResponseTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePackagesResponseTypeDef,
@@ -188,20 +188,20 @@
         """
     async def create_container_recipe(
         self,
         *,
         containerType: Literal["DOCKER"],
         name: str,
         semanticVersion: str,
-        components: Sequence[ComponentConfigurationTypeDef],
+        components: Sequence[ComponentConfigurationUnionTypeDef],
         parentImage: str,
         targetRepository: TargetContainerRepositoryTypeDef,
         clientToken: str,
         description: str = ...,
-        instanceConfiguration: InstanceConfigurationTypeDef = ...,
+        instanceConfiguration: InstanceConfigurationUnionTypeDef = ...,
         dockerfileTemplateData: str = ...,
         dockerfileTemplateUri: str = ...,
         platformOverride: PlatformType = ...,
         imageOsVersionOverride: str = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         kmsKeyId: str = ...
@@ -212,15 +212,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_container_recipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_container_recipe)
         """
     async def create_distribution_configuration(
         self,
         *,
         name: str,
-        distributions: Sequence[DistributionTypeDef],
+        distributions: Sequence[DistributionUnionTypeDef],
         clientToken: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDistributionConfigurationResponseTypeDef:
         """
         Creates a new distribution configuration.
 
@@ -234,15 +234,15 @@
         clientToken: str,
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
+        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
     ) -> CreateImageResponseTypeDef:
         """
         Creates a new image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image)
         """
@@ -257,28 +257,28 @@
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
+        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
     ) -> CreateImagePipelineResponseTypeDef:
         """
         Creates a new image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image_pipeline)
         """
     async def create_image_recipe(
         self,
         *,
         name: str,
         semanticVersion: str,
-        components: Sequence[ComponentConfigurationTypeDef],
+        components: Sequence[ComponentConfigurationUnionTypeDef],
         parentImage: str,
         clientToken: str,
         description: str = ...,
         blockDeviceMappings: Sequence[InstanceBlockDeviceMappingTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...
@@ -778,15 +778,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#untag_resource)
         """
     async def update_distribution_configuration(
         self,
         *,
         distributionConfigurationArn: str,
-        distributions: Sequence[DistributionTypeDef],
+        distributions: Sequence[DistributionUnionTypeDef],
         clientToken: str,
         description: str = ...
     ) -> UpdateDistributionConfigurationResponseTypeDef:
         """
         Updates a new distribution configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_distribution_configuration)
@@ -802,15 +802,15 @@
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
-        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
+        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
     ) -> UpdateImagePipelineResponseTypeDef:
         """
         Updates an image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_image_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#update_image_pipeline)
         """
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/literals.py` & `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/literals.pyi` & `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/type_defs.py` & `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_imagebuilder.type_defs import SeverityCountsTypeDef
 
-    data: SeverityCountsTypeDef = {...}
+    data: SeverityCountsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BuildTypeType,
     ComponentTypeType,
     DiskImageFormatType,
     EbsVolumeTypeType,
     ImageScanStatusType,
@@ -43,132 +43,139 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "SeverityCountsTypeDef",
     "SystemsManagerAgentTypeDef",
+    "LaunchPermissionConfigurationOutputTypeDef",
     "LaunchPermissionConfigurationTypeDef",
     "ImageStateTypeDef",
     "CancelImageCreationRequestRequestTypeDef",
-    "CancelImageCreationResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "ComponentParameterOutputTypeDef",
     "ComponentParameterTypeDef",
     "ComponentParameterDetailTypeDef",
     "ComponentStateTypeDef",
     "ComponentVersionTypeDef",
     "TargetContainerRepositoryTypeDef",
     "ContainerRecipeSummaryTypeDef",
     "ContainerTypeDef",
     "CreateComponentRequestRequestTypeDef",
-    "CreateComponentResponseTypeDef",
-    "CreateContainerRecipeResponseTypeDef",
-    "CreateDistributionConfigurationResponseTypeDef",
     "ImageTestsConfigurationTypeDef",
     "ScheduleTypeDef",
-    "CreateImagePipelineResponseTypeDef",
-    "CreateImageRecipeResponseTypeDef",
-    "CreateImageResponseTypeDef",
     "InstanceMetadataOptionsTypeDef",
-    "CreateInfrastructureConfigurationResponseTypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DeleteComponentRequestRequestTypeDef",
-    "DeleteComponentResponseTypeDef",
     "DeleteContainerRecipeRequestRequestTypeDef",
-    "DeleteContainerRecipeResponseTypeDef",
     "DeleteDistributionConfigurationRequestRequestTypeDef",
-    "DeleteDistributionConfigurationResponseTypeDef",
     "DeleteImagePipelineRequestRequestTypeDef",
-    "DeleteImagePipelineResponseTypeDef",
     "DeleteImageRecipeRequestRequestTypeDef",
-    "DeleteImageRecipeResponseTypeDef",
     "DeleteImageRequestRequestTypeDef",
-    "DeleteImageResponseTypeDef",
     "DeleteInfrastructureConfigurationRequestRequestTypeDef",
-    "DeleteInfrastructureConfigurationResponseTypeDef",
     "DistributionConfigurationSummaryTypeDef",
     "LaunchTemplateConfigurationTypeDef",
     "S3ExportConfigurationTypeDef",
     "EbsInstanceBlockDeviceSpecificationTypeDef",
+    "EcrConfigurationOutputTypeDef",
     "EcrConfigurationTypeDef",
     "FastLaunchLaunchTemplateSpecificationTypeDef",
     "FastLaunchSnapshotConfigurationTypeDef",
     "FilterTypeDef",
     "GetComponentPolicyRequestRequestTypeDef",
-    "GetComponentPolicyResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetContainerRecipePolicyRequestRequestTypeDef",
-    "GetContainerRecipePolicyResponseTypeDef",
     "GetContainerRecipeRequestRequestTypeDef",
     "GetDistributionConfigurationRequestRequestTypeDef",
     "GetImagePipelineRequestRequestTypeDef",
     "GetImagePolicyRequestRequestTypeDef",
-    "GetImagePolicyResponseTypeDef",
     "GetImageRecipePolicyRequestRequestTypeDef",
-    "GetImageRecipePolicyResponseTypeDef",
     "GetImageRecipeRequestRequestTypeDef",
     "GetImageRequestRequestTypeDef",
     "GetInfrastructureConfigurationRequestRequestTypeDef",
     "GetWorkflowExecutionRequestRequestTypeDef",
-    "GetWorkflowExecutionResponseTypeDef",
     "GetWorkflowStepExecutionRequestRequestTypeDef",
-    "GetWorkflowStepExecutionResponseTypeDef",
     "ImagePackageTypeDef",
     "ImageRecipeSummaryTypeDef",
     "ImageScanFindingsFilterTypeDef",
     "ImageScanStateTypeDef",
     "ImageVersionTypeDef",
     "ImportComponentRequestRequestTypeDef",
-    "ImportComponentResponseTypeDef",
     "ImportVmImageRequestRequestTypeDef",
-    "ImportVmImageResponseTypeDef",
     "InfrastructureConfigurationSummaryTypeDef",
     "ListComponentBuildVersionsRequestRequestTypeDef",
     "ListImagePackagesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWorkflowExecutionsRequestRequestTypeDef",
     "WorkflowExecutionMetadataTypeDef",
     "ListWorkflowStepExecutionsRequestRequestTypeDef",
     "WorkflowStepMetadataTypeDef",
     "S3LogsTypeDef",
     "VulnerablePackageTypeDef",
     "PutComponentPolicyRequestRequestTypeDef",
-    "PutComponentPolicyResponseTypeDef",
     "PutContainerRecipePolicyRequestRequestTypeDef",
-    "PutContainerRecipePolicyResponseTypeDef",
     "PutImagePolicyRequestRequestTypeDef",
-    "PutImagePolicyResponseTypeDef",
     "PutImageRecipePolicyRequestRequestTypeDef",
-    "PutImageRecipePolicyResponseTypeDef",
     "RemediationRecommendationTypeDef",
-    "ResponseMetadataTypeDef",
     "StartImagePipelineExecutionRequestRequestTypeDef",
-    "StartImagePipelineExecutionResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateDistributionConfigurationResponseTypeDef",
-    "UpdateImagePipelineResponseTypeDef",
-    "UpdateInfrastructureConfigurationResponseTypeDef",
     "AccountAggregationTypeDef",
     "ImageAggregationTypeDef",
     "ImagePipelineAggregationTypeDef",
     "VulnerabilityIdAggregationTypeDef",
     "AdditionalInstanceConfigurationTypeDef",
+    "AmiDistributionConfigurationOutputTypeDef",
     "AmiDistributionConfigurationTypeDef",
     "AmiTypeDef",
+    "CancelImageCreationResponseTypeDef",
+    "CreateComponentResponseTypeDef",
+    "CreateContainerRecipeResponseTypeDef",
+    "CreateDistributionConfigurationResponseTypeDef",
+    "CreateImagePipelineResponseTypeDef",
+    "CreateImageRecipeResponseTypeDef",
+    "CreateImageResponseTypeDef",
+    "CreateInfrastructureConfigurationResponseTypeDef",
+    "DeleteComponentResponseTypeDef",
+    "DeleteContainerRecipeResponseTypeDef",
+    "DeleteDistributionConfigurationResponseTypeDef",
+    "DeleteImagePipelineResponseTypeDef",
+    "DeleteImageRecipeResponseTypeDef",
+    "DeleteImageResponseTypeDef",
+    "DeleteInfrastructureConfigurationResponseTypeDef",
+    "GetComponentPolicyResponseTypeDef",
+    "GetContainerRecipePolicyResponseTypeDef",
+    "GetImagePolicyResponseTypeDef",
+    "GetImageRecipePolicyResponseTypeDef",
+    "GetWorkflowExecutionResponseTypeDef",
+    "GetWorkflowStepExecutionResponseTypeDef",
+    "ImportComponentResponseTypeDef",
+    "ImportVmImageResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutComponentPolicyResponseTypeDef",
+    "PutContainerRecipePolicyResponseTypeDef",
+    "PutImagePolicyResponseTypeDef",
+    "PutImageRecipePolicyResponseTypeDef",
+    "StartImagePipelineExecutionResponseTypeDef",
+    "UpdateDistributionConfigurationResponseTypeDef",
+    "UpdateImagePipelineResponseTypeDef",
+    "UpdateInfrastructureConfigurationResponseTypeDef",
+    "ComponentConfigurationOutputTypeDef",
     "ComponentConfigurationTypeDef",
     "ComponentSummaryTypeDef",
     "ComponentTypeDef",
     "ListComponentsResponseTypeDef",
+    "ContainerDistributionConfigurationOutputTypeDef",
     "ContainerDistributionConfigurationTypeDef",
     "ListContainerRecipesResponseTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDistributionConfigurationsResponseTypeDef",
     "InstanceBlockDeviceMappingTypeDef",
+    "ImageScanningConfigurationOutputTypeDef",
     "ImageScanningConfigurationTypeDef",
     "FastLaunchConfigurationTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListContainerRecipesRequestRequestTypeDef",
     "ListDistributionConfigurationsRequestRequestTypeDef",
     "ListImageBuildVersionsRequestRequestTypeDef",
     "ListImagePipelineImagesRequestRequestTypeDef",
@@ -185,46 +192,52 @@
     "ListWorkflowExecutionsResponseTypeDef",
     "ListWorkflowStepExecutionsResponseTypeDef",
     "LoggingTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "ImageScanFindingAggregationTypeDef",
     "OutputResourcesTypeDef",
+    "ComponentConfigurationUnionTypeDef",
     "ListComponentBuildVersionsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "InspectorScoreDetailsTypeDef",
-    "CreateImageRecipeRequestRequestTypeDef",
     "ImageRecipeTypeDef",
+    "InstanceConfigurationOutputTypeDef",
     "InstanceConfigurationTypeDef",
+    "ImagePipelineTypeDef",
     "CreateImagePipelineRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
-    "ImagePipelineTypeDef",
+    "ImageScanningConfigurationUnionTypeDef",
     "UpdateImagePipelineRequestRequestTypeDef",
+    "DistributionOutputTypeDef",
     "DistributionTypeDef",
     "CreateInfrastructureConfigurationRequestRequestTypeDef",
     "InfrastructureConfigurationTypeDef",
     "UpdateInfrastructureConfigurationRequestRequestTypeDef",
     "ListImageScanFindingAggregationsResponseTypeDef",
     "ImageSummaryTypeDef",
+    "CreateImageRecipeRequestRequestTypeDef",
     "ImageScanFindingTypeDef",
     "GetImageRecipeResponseTypeDef",
     "ContainerRecipeTypeDef",
     "CreateContainerRecipeRequestRequestTypeDef",
+    "InstanceConfigurationUnionTypeDef",
     "GetImagePipelineResponseTypeDef",
     "ListImagePipelinesResponseTypeDef",
-    "CreateDistributionConfigurationRequestRequestTypeDef",
     "DistributionConfigurationTypeDef",
-    "UpdateDistributionConfigurationRequestRequestTypeDef",
+    "DistributionUnionTypeDef",
     "GetInfrastructureConfigurationResponseTypeDef",
     "ListImageBuildVersionsResponseTypeDef",
     "ListImagePipelineImagesResponseTypeDef",
     "ListImageScanFindingsResponseTypeDef",
     "GetContainerRecipeResponseTypeDef",
     "GetDistributionConfigurationResponseTypeDef",
     "ImageTypeDef",
+    "CreateDistributionConfigurationRequestRequestTypeDef",
+    "UpdateDistributionConfigurationRequestRequestTypeDef",
     "GetImageResponseTypeDef",
 )
 
 SeverityCountsTypeDef = TypedDict(
     "SeverityCountsTypeDef",
     {
         "all": int,
@@ -239,14 +252,25 @@
     "SystemsManagerAgentTypeDef",
     {
         "uninstallAfterBuild": bool,
     },
     total=False,
 )
 
+LaunchPermissionConfigurationOutputTypeDef = TypedDict(
+    "LaunchPermissionConfigurationOutputTypeDef",
+    {
+        "userIds": List[str],
+        "userGroups": List[str],
+        "organizationArns": List[str],
+        "organizationalUnitArns": List[str],
+    },
+    total=False,
+)
+
 LaunchPermissionConfigurationTypeDef = TypedDict(
     "LaunchPermissionConfigurationTypeDef",
     {
         "userIds": Sequence[str],
         "userGroups": Sequence[str],
         "organizationArns": Sequence[str],
         "organizationalUnitArns": Sequence[str],
@@ -267,21 +291,30 @@
     "CancelImageCreationRequestRequestTypeDef",
     {
         "imageBuildVersionArn": str,
         "clientToken": str,
     },
 )
 
-CancelImageCreationResponseTypeDef = TypedDict(
-    "CancelImageCreationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "requestId": str,
-        "clientToken": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+ComponentParameterOutputTypeDef = TypedDict(
+    "ComponentParameterOutputTypeDef",
+    {
+        "name": str,
+        "value": List[str],
     },
 )
 
 ComponentParameterTypeDef = TypedDict(
     "ComponentParameterTypeDef",
     {
         "name": str,
@@ -395,44 +428,14 @@
 
 class CreateComponentRequestRequestTypeDef(
     _RequiredCreateComponentRequestRequestTypeDef, _OptionalCreateComponentRequestRequestTypeDef
 ):
     pass
 
 
-CreateComponentResponseTypeDef = TypedDict(
-    "CreateComponentResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "componentBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateContainerRecipeResponseTypeDef = TypedDict(
-    "CreateContainerRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "containerRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDistributionConfigurationResponseTypeDef = TypedDict(
-    "CreateDistributionConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "distributionConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImageTestsConfigurationTypeDef = TypedDict(
     "ImageTestsConfigurationTypeDef",
     {
         "imageTestsEnabled": bool,
         "timeoutMinutes": int,
     },
     total=False,
@@ -444,63 +447,23 @@
         "scheduleExpression": str,
         "timezone": str,
         "pipelineExecutionStartCondition": PipelineExecutionStartConditionType,
     },
     total=False,
 )
 
-CreateImagePipelineResponseTypeDef = TypedDict(
-    "CreateImagePipelineResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imagePipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateImageRecipeResponseTypeDef = TypedDict(
-    "CreateImageRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imageRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateImageResponseTypeDef = TypedDict(
-    "CreateImageResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InstanceMetadataOptionsTypeDef = TypedDict(
     "InstanceMetadataOptionsTypeDef",
     {
         "httpTokens": str,
         "httpPutResponseHopLimit": int,
     },
     total=False,
 )
 
-CreateInfrastructureConfigurationResponseTypeDef = TypedDict(
-    "CreateInfrastructureConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "infrastructureConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CvssScoreAdjustmentTypeDef = TypedDict(
     "CvssScoreAdjustmentTypeDef",
     {
         "metric": str,
         "reason": str,
     },
     total=False,
@@ -520,119 +483,56 @@
 DeleteComponentRequestRequestTypeDef = TypedDict(
     "DeleteComponentRequestRequestTypeDef",
     {
         "componentBuildVersionArn": str,
     },
 )
 
-DeleteComponentResponseTypeDef = TypedDict(
-    "DeleteComponentResponseTypeDef",
-    {
-        "requestId": str,
-        "componentBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteContainerRecipeRequestRequestTypeDef = TypedDict(
     "DeleteContainerRecipeRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
     },
 )
 
-DeleteContainerRecipeResponseTypeDef = TypedDict(
-    "DeleteContainerRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "containerRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteDistributionConfigurationRequestRequestTypeDef",
     {
         "distributionConfigurationArn": str,
     },
 )
 
-DeleteDistributionConfigurationResponseTypeDef = TypedDict(
-    "DeleteDistributionConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "distributionConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImagePipelineRequestRequestTypeDef = TypedDict(
     "DeleteImagePipelineRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
     },
 )
 
-DeleteImagePipelineResponseTypeDef = TypedDict(
-    "DeleteImagePipelineResponseTypeDef",
-    {
-        "requestId": str,
-        "imagePipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImageRecipeRequestRequestTypeDef = TypedDict(
     "DeleteImageRecipeRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
     },
 )
 
-DeleteImageRecipeResponseTypeDef = TypedDict(
-    "DeleteImageRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "imageRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImageRequestRequestTypeDef = TypedDict(
     "DeleteImageRequestRequestTypeDef",
     {
         "imageBuildVersionArn": str,
     },
 )
 
-DeleteImageResponseTypeDef = TypedDict(
-    "DeleteImageResponseTypeDef",
-    {
-        "requestId": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteInfrastructureConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteInfrastructureConfigurationRequestRequestTypeDef",
     {
         "infrastructureConfigurationArn": str,
     },
 )
 
-DeleteInfrastructureConfigurationResponseTypeDef = TypedDict(
-    "DeleteInfrastructureConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "infrastructureConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DistributionConfigurationSummaryTypeDef = TypedDict(
     "DistributionConfigurationSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
         "dateCreated": str,
@@ -699,14 +599,23 @@
         "volumeSize": int,
         "volumeType": EbsVolumeTypeType,
         "throughput": int,
     },
     total=False,
 )
 
+EcrConfigurationOutputTypeDef = TypedDict(
+    "EcrConfigurationOutputTypeDef",
+    {
+        "repositoryName": str,
+        "containerTags": List[str],
+    },
+    total=False,
+)
+
 EcrConfigurationTypeDef = TypedDict(
     "EcrConfigurationTypeDef",
     {
         "repositoryName": str,
         "containerTags": Sequence[str],
     },
     total=False,
@@ -742,46 +651,28 @@
 GetComponentPolicyRequestRequestTypeDef = TypedDict(
     "GetComponentPolicyRequestRequestTypeDef",
     {
         "componentArn": str,
     },
 )
 
-GetComponentPolicyResponseTypeDef = TypedDict(
-    "GetComponentPolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetComponentRequestRequestTypeDef = TypedDict(
     "GetComponentRequestRequestTypeDef",
     {
         "componentBuildVersionArn": str,
     },
 )
 
 GetContainerRecipePolicyRequestRequestTypeDef = TypedDict(
     "GetContainerRecipePolicyRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
     },
 )
 
-GetContainerRecipePolicyResponseTypeDef = TypedDict(
-    "GetContainerRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetContainerRecipeRequestRequestTypeDef = TypedDict(
     "GetContainerRecipeRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
     },
 )
 
@@ -802,39 +693,21 @@
 GetImagePolicyRequestRequestTypeDef = TypedDict(
     "GetImagePolicyRequestRequestTypeDef",
     {
         "imageArn": str,
     },
 )
 
-GetImagePolicyResponseTypeDef = TypedDict(
-    "GetImagePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetImageRecipePolicyRequestRequestTypeDef = TypedDict(
     "GetImageRecipePolicyRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
     },
 )
 
-GetImageRecipePolicyResponseTypeDef = TypedDict(
-    "GetImageRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetImageRecipeRequestRequestTypeDef = TypedDict(
     "GetImageRecipeRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
     },
 )
 
@@ -855,65 +728,21 @@
 GetWorkflowExecutionRequestRequestTypeDef = TypedDict(
     "GetWorkflowExecutionRequestRequestTypeDef",
     {
         "workflowExecutionId": str,
     },
 )
 
-GetWorkflowExecutionResponseTypeDef = TypedDict(
-    "GetWorkflowExecutionResponseTypeDef",
-    {
-        "requestId": str,
-        "workflowBuildVersionArn": str,
-        "workflowExecutionId": str,
-        "imageBuildVersionArn": str,
-        "type": WorkflowTypeType,
-        "status": WorkflowExecutionStatusType,
-        "message": str,
-        "totalStepCount": int,
-        "totalStepsSucceeded": int,
-        "totalStepsFailed": int,
-        "totalStepsSkipped": int,
-        "startTime": str,
-        "endTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkflowStepExecutionRequestRequestTypeDef = TypedDict(
     "GetWorkflowStepExecutionRequestRequestTypeDef",
     {
         "stepExecutionId": str,
     },
 )
 
-GetWorkflowStepExecutionResponseTypeDef = TypedDict(
-    "GetWorkflowStepExecutionResponseTypeDef",
-    {
-        "requestId": str,
-        "stepExecutionId": str,
-        "workflowBuildVersionArn": str,
-        "workflowExecutionId": str,
-        "imageBuildVersionArn": str,
-        "name": str,
-        "description": str,
-        "action": str,
-        "status": WorkflowStepExecutionStatusType,
-        "rollbackStatus": WorkflowStepExecutionRollbackStatusType,
-        "message": str,
-        "inputs": str,
-        "outputs": str,
-        "startTime": str,
-        "endTime": str,
-        "onFailure": str,
-        "timeoutSeconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImagePackageTypeDef = TypedDict(
     "ImagePackageTypeDef",
     {
         "packageName": str,
         "packageVersion": str,
     },
     total=False,
@@ -995,24 +824,14 @@
 
 class ImportComponentRequestRequestTypeDef(
     _RequiredImportComponentRequestRequestTypeDef, _OptionalImportComponentRequestRequestTypeDef
 ):
     pass
 
 
-ImportComponentResponseTypeDef = TypedDict(
-    "ImportComponentResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "componentBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredImportVmImageRequestRequestTypeDef = TypedDict(
     "_RequiredImportVmImageRequestRequestTypeDef",
     {
         "name": str,
         "semanticVersion": str,
         "platform": PlatformType,
         "vmImportTaskId": str,
@@ -1032,24 +851,14 @@
 
 class ImportVmImageRequestRequestTypeDef(
     _RequiredImportVmImageRequestRequestTypeDef, _OptionalImportVmImageRequestRequestTypeDef
 ):
     pass
 
 
-ImportVmImageResponseTypeDef = TypedDict(
-    "ImportVmImageResponseTypeDef",
-    {
-        "requestId": str,
-        "imageArn": str,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InfrastructureConfigurationSummaryTypeDef = TypedDict(
     "InfrastructureConfigurationSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
         "dateCreated": str,
@@ -1110,22 +919,14 @@
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
 _RequiredListWorkflowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkflowExecutionsRequestRequestTypeDef",
     {
         "imageBuildVersionArn": str,
     },
 )
 _OptionalListWorkflowExecutionsRequestRequestTypeDef = TypedDict(
@@ -1234,112 +1035,55 @@
     "PutComponentPolicyRequestRequestTypeDef",
     {
         "componentArn": str,
         "policy": str,
     },
 )
 
-PutComponentPolicyResponseTypeDef = TypedDict(
-    "PutComponentPolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "componentArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutContainerRecipePolicyRequestRequestTypeDef = TypedDict(
     "PutContainerRecipePolicyRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
         "policy": str,
     },
 )
 
-PutContainerRecipePolicyResponseTypeDef = TypedDict(
-    "PutContainerRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "containerRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutImagePolicyRequestRequestTypeDef = TypedDict(
     "PutImagePolicyRequestRequestTypeDef",
     {
         "imageArn": str,
         "policy": str,
     },
 )
 
-PutImagePolicyResponseTypeDef = TypedDict(
-    "PutImagePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "imageArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutImageRecipePolicyRequestRequestTypeDef = TypedDict(
     "PutImageRecipePolicyRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
         "policy": str,
     },
 )
 
-PutImageRecipePolicyResponseTypeDef = TypedDict(
-    "PutImageRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "imageRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemediationRecommendationTypeDef = TypedDict(
     "RemediationRecommendationTypeDef",
     {
         "text": str,
         "url": str,
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
 StartImagePipelineExecutionRequestRequestTypeDef = TypedDict(
     "StartImagePipelineExecutionRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
         "clientToken": str,
     },
 )
 
-StartImagePipelineExecutionResponseTypeDef = TypedDict(
-    "StartImagePipelineExecutionResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1348,44 +1092,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateDistributionConfigurationResponseTypeDef = TypedDict(
-    "UpdateDistributionConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "distributionConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateImagePipelineResponseTypeDef = TypedDict(
-    "UpdateImagePipelineResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imagePipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateInfrastructureConfigurationResponseTypeDef = TypedDict(
-    "UpdateInfrastructureConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "infrastructureConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AccountAggregationTypeDef = TypedDict(
     "AccountAggregationTypeDef",
     {
         "accountId": str,
         "severityCounts": SeverityCountsTypeDef,
     },
     total=False,
@@ -1423,14 +1137,27 @@
     {
         "systemsManagerAgent": SystemsManagerAgentTypeDef,
         "userDataOverride": str,
     },
     total=False,
 )
 
+AmiDistributionConfigurationOutputTypeDef = TypedDict(
+    "AmiDistributionConfigurationOutputTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "targetAccountIds": List[str],
+        "amiTags": Dict[str, str],
+        "kmsKeyId": str,
+        "launchPermission": LaunchPermissionConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 AmiDistributionConfigurationTypeDef = TypedDict(
     "AmiDistributionConfigurationTypeDef",
     {
         "name": str,
         "description": str,
         "targetAccountIds": Sequence[str],
         "amiTags": Mapping[str, str],
@@ -1449,14 +1176,362 @@
         "description": str,
         "state": ImageStateTypeDef,
         "accountId": str,
     },
     total=False,
 )
 
+CancelImageCreationResponseTypeDef = TypedDict(
+    "CancelImageCreationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateComponentResponseTypeDef = TypedDict(
+    "CreateComponentResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "componentBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateContainerRecipeResponseTypeDef = TypedDict(
+    "CreateContainerRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "containerRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDistributionConfigurationResponseTypeDef = TypedDict(
+    "CreateDistributionConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "distributionConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImagePipelineResponseTypeDef = TypedDict(
+    "CreateImagePipelineResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imagePipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImageRecipeResponseTypeDef = TypedDict(
+    "CreateImageRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImageResponseTypeDef = TypedDict(
+    "CreateImageResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateInfrastructureConfigurationResponseTypeDef = TypedDict(
+    "CreateInfrastructureConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "infrastructureConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteComponentResponseTypeDef = TypedDict(
+    "DeleteComponentResponseTypeDef",
+    {
+        "requestId": str,
+        "componentBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteContainerRecipeResponseTypeDef = TypedDict(
+    "DeleteContainerRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "containerRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDistributionConfigurationResponseTypeDef = TypedDict(
+    "DeleteDistributionConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "distributionConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImagePipelineResponseTypeDef = TypedDict(
+    "DeleteImagePipelineResponseTypeDef",
+    {
+        "requestId": str,
+        "imagePipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImageRecipeResponseTypeDef = TypedDict(
+    "DeleteImageRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "imageRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImageResponseTypeDef = TypedDict(
+    "DeleteImageResponseTypeDef",
+    {
+        "requestId": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteInfrastructureConfigurationResponseTypeDef = TypedDict(
+    "DeleteInfrastructureConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "infrastructureConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComponentPolicyResponseTypeDef = TypedDict(
+    "GetComponentPolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContainerRecipePolicyResponseTypeDef = TypedDict(
+    "GetContainerRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImagePolicyResponseTypeDef = TypedDict(
+    "GetImagePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImageRecipePolicyResponseTypeDef = TypedDict(
+    "GetImageRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkflowExecutionResponseTypeDef = TypedDict(
+    "GetWorkflowExecutionResponseTypeDef",
+    {
+        "requestId": str,
+        "workflowBuildVersionArn": str,
+        "workflowExecutionId": str,
+        "imageBuildVersionArn": str,
+        "type": WorkflowTypeType,
+        "status": WorkflowExecutionStatusType,
+        "message": str,
+        "totalStepCount": int,
+        "totalStepsSucceeded": int,
+        "totalStepsFailed": int,
+        "totalStepsSkipped": int,
+        "startTime": str,
+        "endTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkflowStepExecutionResponseTypeDef = TypedDict(
+    "GetWorkflowStepExecutionResponseTypeDef",
+    {
+        "requestId": str,
+        "stepExecutionId": str,
+        "workflowBuildVersionArn": str,
+        "workflowExecutionId": str,
+        "imageBuildVersionArn": str,
+        "name": str,
+        "description": str,
+        "action": str,
+        "status": WorkflowStepExecutionStatusType,
+        "rollbackStatus": WorkflowStepExecutionRollbackStatusType,
+        "message": str,
+        "inputs": str,
+        "outputs": str,
+        "startTime": str,
+        "endTime": str,
+        "onFailure": str,
+        "timeoutSeconds": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportComponentResponseTypeDef = TypedDict(
+    "ImportComponentResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "componentBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportVmImageResponseTypeDef = TypedDict(
+    "ImportVmImageResponseTypeDef",
+    {
+        "requestId": str,
+        "imageArn": str,
+        "clientToken": str,
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
+PutComponentPolicyResponseTypeDef = TypedDict(
+    "PutComponentPolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "componentArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutContainerRecipePolicyResponseTypeDef = TypedDict(
+    "PutContainerRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "containerRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutImagePolicyResponseTypeDef = TypedDict(
+    "PutImagePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "imageArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutImageRecipePolicyResponseTypeDef = TypedDict(
+    "PutImageRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "imageRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartImagePipelineExecutionResponseTypeDef = TypedDict(
+    "StartImagePipelineExecutionResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDistributionConfigurationResponseTypeDef = TypedDict(
+    "UpdateDistributionConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "distributionConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateImagePipelineResponseTypeDef = TypedDict(
+    "UpdateImagePipelineResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imagePipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateInfrastructureConfigurationResponseTypeDef = TypedDict(
+    "UpdateInfrastructureConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "infrastructureConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredComponentConfigurationOutputTypeDef = TypedDict(
+    "_RequiredComponentConfigurationOutputTypeDef",
+    {
+        "componentArn": str,
+    },
+)
+_OptionalComponentConfigurationOutputTypeDef = TypedDict(
+    "_OptionalComponentConfigurationOutputTypeDef",
+    {
+        "parameters": List[ComponentParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class ComponentConfigurationOutputTypeDef(
+    _RequiredComponentConfigurationOutputTypeDef, _OptionalComponentConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredComponentConfigurationTypeDef = TypedDict(
     "_RequiredComponentConfigurationTypeDef",
     {
         "componentArn": str,
     },
 )
 _OptionalComponentConfigurationTypeDef = TypedDict(
@@ -1522,18 +1597,41 @@
 
 ListComponentsResponseTypeDef = TypedDict(
     "ListComponentsResponseTypeDef",
     {
         "requestId": str,
         "componentVersionList": List[ComponentVersionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredContainerDistributionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredContainerDistributionConfigurationOutputTypeDef",
+    {
+        "targetRepository": TargetContainerRepositoryTypeDef,
+    },
+)
+_OptionalContainerDistributionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalContainerDistributionConfigurationOutputTypeDef",
+    {
+        "description": str,
+        "containerTags": List[str],
     },
+    total=False,
 )
 
+
+class ContainerDistributionConfigurationOutputTypeDef(
+    _RequiredContainerDistributionConfigurationOutputTypeDef,
+    _OptionalContainerDistributionConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredContainerDistributionConfigurationTypeDef = TypedDict(
     "_RequiredContainerDistributionConfigurationTypeDef",
     {
         "targetRepository": TargetContainerRepositoryTypeDef,
     },
 )
 _OptionalContainerDistributionConfigurationTypeDef = TypedDict(
@@ -1555,15 +1653,15 @@
 
 ListContainerRecipesResponseTypeDef = TypedDict(
     "ListContainerRecipesResponseTypeDef",
     {
         "requestId": str,
         "containerRecipeSummaryList": List[ContainerRecipeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CvssScoreDetailsTypeDef = TypedDict(
     "CvssScoreDetailsTypeDef",
     {
         "scoreSource": str,
@@ -1578,29 +1676,38 @@
 
 ListDistributionConfigurationsResponseTypeDef = TypedDict(
     "ListDistributionConfigurationsResponseTypeDef",
     {
         "requestId": str,
         "distributionConfigurationSummaryList": List[DistributionConfigurationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceBlockDeviceMappingTypeDef = TypedDict(
     "InstanceBlockDeviceMappingTypeDef",
     {
         "deviceName": str,
         "ebs": EbsInstanceBlockDeviceSpecificationTypeDef,
         "virtualName": str,
         "noDevice": str,
     },
     total=False,
 )
 
+ImageScanningConfigurationOutputTypeDef = TypedDict(
+    "ImageScanningConfigurationOutputTypeDef",
+    {
+        "imageScanningEnabled": bool,
+        "ecrConfiguration": EcrConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ImageScanningConfigurationTypeDef = TypedDict(
     "ImageScanningConfigurationTypeDef",
     {
         "imageScanningEnabled": bool,
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
     total=False,
@@ -1766,25 +1873,25 @@
 
 ListImagePackagesResponseTypeDef = TypedDict(
     "ListImagePackagesResponseTypeDef",
     {
         "requestId": str,
         "imagePackageList": List[ImagePackageTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageRecipesResponseTypeDef = TypedDict(
     "ListImageRecipesResponseTypeDef",
     {
         "requestId": str,
         "imageRecipeSummaryList": List[ImageRecipeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageScanFindingsRequestRequestTypeDef = TypedDict(
     "ListImageScanFindingsRequestRequestTypeDef",
     {
         "filters": Sequence[ImageScanFindingsFilterTypeDef],
@@ -1796,51 +1903,51 @@
 
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
         "requestId": str,
         "imageVersionList": List[ImageVersionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInfrastructureConfigurationsResponseTypeDef = TypedDict(
     "ListInfrastructureConfigurationsResponseTypeDef",
     {
         "requestId": str,
         "infrastructureConfigurationSummaryList": List[InfrastructureConfigurationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowExecutionsResponseTypeDef = TypedDict(
     "ListWorkflowExecutionsResponseTypeDef",
     {
         "requestId": str,
         "workflowExecutions": List[WorkflowExecutionMetadataTypeDef],
         "imageBuildVersionArn": str,
         "message": str,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowStepExecutionsResponseTypeDef = TypedDict(
     "ListWorkflowStepExecutionsResponseTypeDef",
     {
         "requestId": str,
         "steps": List[WorkflowStepMetadataTypeDef],
         "workflowBuildVersionArn": str,
         "workflowExecutionId": str,
         "imageBuildVersionArn": str,
         "message": str,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "s3Logs": S3LogsTypeDef,
@@ -1901,100 +2008,108 @@
     {
         "amis": List[AmiTypeDef],
         "containers": List[ContainerTypeDef],
     },
     total=False,
 )
 
+ComponentConfigurationUnionTypeDef = Union[
+    ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef
+]
 ListComponentBuildVersionsResponseTypeDef = TypedDict(
     "ListComponentBuildVersionsResponseTypeDef",
     {
         "requestId": str,
         "componentSummaryList": List[ComponentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComponentResponseTypeDef = TypedDict(
     "GetComponentResponseTypeDef",
     {
         "requestId": str,
         "component": ComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InspectorScoreDetailsTypeDef = TypedDict(
     "InspectorScoreDetailsTypeDef",
     {
         "adjustedCvss": CvssScoreDetailsTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateImageRecipeRequestRequestTypeDef",
-    {
-        "name": str,
-        "semanticVersion": str,
-        "components": Sequence[ComponentConfigurationTypeDef],
-        "parentImage": str,
-        "clientToken": str,
-    },
-)
-_OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateImageRecipeRequestRequestTypeDef",
-    {
-        "description": str,
-        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
-        "tags": Mapping[str, str],
-        "workingDirectory": str,
-        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateImageRecipeRequestRequestTypeDef(
-    _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
-):
-    pass
-
-
 ImageRecipeTypeDef = TypedDict(
     "ImageRecipeTypeDef",
     {
         "arn": str,
         "type": ImageTypeType,
         "name": str,
         "description": str,
         "platform": PlatformType,
         "owner": str,
         "version": str,
-        "components": List[ComponentConfigurationTypeDef],
+        "components": List[ComponentConfigurationOutputTypeDef],
         "parentImage": str,
         "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
         "dateCreated": str,
         "tags": Dict[str, str],
         "workingDirectory": str,
         "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
     },
     total=False,
 )
 
+InstanceConfigurationOutputTypeDef = TypedDict(
+    "InstanceConfigurationOutputTypeDef",
+    {
+        "image": str,
+        "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
+    },
+    total=False,
+)
+
 InstanceConfigurationTypeDef = TypedDict(
     "InstanceConfigurationTypeDef",
     {
         "image": str,
         "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
     },
     total=False,
 )
 
+ImagePipelineTypeDef = TypedDict(
+    "ImagePipelineTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "platform": PlatformType,
+        "enhancedImageMetadataEnabled": bool,
+        "imageRecipeArn": str,
+        "containerRecipeArn": str,
+        "infrastructureConfigurationArn": str,
+        "distributionConfigurationArn": str,
+        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
+        "schedule": ScheduleTypeDef,
+        "status": PipelineStatusType,
+        "dateCreated": str,
+        "dateUpdated": str,
+        "dateLastRun": str,
+        "dateNextRun": str,
+        "tags": Dict[str, str],
+        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImagePipelineRequestRequestTypeDef",
     {
         "name": str,
         "infrastructureConfigurationArn": str,
         "clientToken": str,
     },
@@ -2048,39 +2163,17 @@
 
 class CreateImageRequestRequestTypeDef(
     _RequiredCreateImageRequestRequestTypeDef, _OptionalCreateImageRequestRequestTypeDef
 ):
     pass
 
 
-ImagePipelineTypeDef = TypedDict(
-    "ImagePipelineTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "platform": PlatformType,
-        "enhancedImageMetadataEnabled": bool,
-        "imageRecipeArn": str,
-        "containerRecipeArn": str,
-        "infrastructureConfigurationArn": str,
-        "distributionConfigurationArn": str,
-        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
-        "schedule": ScheduleTypeDef,
-        "status": PipelineStatusType,
-        "dateCreated": str,
-        "dateUpdated": str,
-        "dateLastRun": str,
-        "dateNextRun": str,
-        "tags": Dict[str, str],
-        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
-    },
-    total=False,
-)
-
+ImageScanningConfigurationUnionTypeDef = Union[
+    ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
+]
 _RequiredUpdateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImagePipelineRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
         "infrastructureConfigurationArn": str,
         "clientToken": str,
     },
@@ -2105,14 +2198,40 @@
 class UpdateImagePipelineRequestRequestTypeDef(
     _RequiredUpdateImagePipelineRequestRequestTypeDef,
     _OptionalUpdateImagePipelineRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDistributionOutputTypeDef = TypedDict(
+    "_RequiredDistributionOutputTypeDef",
+    {
+        "region": str,
+    },
+)
+_OptionalDistributionOutputTypeDef = TypedDict(
+    "_OptionalDistributionOutputTypeDef",
+    {
+        "amiDistributionConfiguration": AmiDistributionConfigurationOutputTypeDef,
+        "containerDistributionConfiguration": ContainerDistributionConfigurationOutputTypeDef,
+        "licenseConfigurationArns": List[str],
+        "launchTemplateConfigurations": List[LaunchTemplateConfigurationTypeDef],
+        "s3ExportConfiguration": S3ExportConfigurationTypeDef,
+        "fastLaunchConfigurations": List[FastLaunchConfigurationTypeDef],
+    },
+    total=False,
+)
+
+
+class DistributionOutputTypeDef(
+    _RequiredDistributionOutputTypeDef, _OptionalDistributionOutputTypeDef
+):
+    pass
+
+
 _RequiredDistributionTypeDef = TypedDict(
     "_RequiredDistributionTypeDef",
     {
         "region": str,
     },
 )
 _OptionalDistributionTypeDef = TypedDict(
@@ -2226,15 +2345,15 @@
 ListImageScanFindingAggregationsResponseTypeDef = TypedDict(
     "ListImageScanFindingAggregationsResponseTypeDef",
     {
         "requestId": str,
         "aggregationType": str,
         "responses": List[ImageScanFindingAggregationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageSummaryTypeDef = TypedDict(
     "ImageSummaryTypeDef",
     {
         "arn": str,
@@ -2250,14 +2369,43 @@
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
     },
     total=False,
 )
 
+_RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateImageRecipeRequestRequestTypeDef",
+    {
+        "name": str,
+        "semanticVersion": str,
+        "components": Sequence[ComponentConfigurationUnionTypeDef],
+        "parentImage": str,
+        "clientToken": str,
+    },
+)
+_OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateImageRecipeRequestRequestTypeDef",
+    {
+        "description": str,
+        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
+        "tags": Mapping[str, str],
+        "workingDirectory": str,
+        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateImageRecipeRequestRequestTypeDef(
+    _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
+):
+    pass
+
+
 ImageScanFindingTypeDef = TypedDict(
     "ImageScanFindingTypeDef",
     {
         "awsAccountId": str,
         "imageBuildVersionArn": str,
         "imagePipelineArn": str,
         "type": str,
@@ -2276,30 +2424,30 @@
 )
 
 GetImageRecipeResponseTypeDef = TypedDict(
     "GetImageRecipeResponseTypeDef",
     {
         "requestId": str,
         "imageRecipe": ImageRecipeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ContainerRecipeTypeDef = TypedDict(
     "ContainerRecipeTypeDef",
     {
         "arn": str,
         "containerType": Literal["DOCKER"],
         "name": str,
         "description": str,
         "platform": PlatformType,
         "owner": str,
         "version": str,
-        "components": List[ComponentConfigurationTypeDef],
-        "instanceConfiguration": InstanceConfigurationTypeDef,
+        "components": List[ComponentConfigurationOutputTypeDef],
+        "instanceConfiguration": InstanceConfigurationOutputTypeDef,
         "dockerfileTemplateData": str,
         "kmsKeyId": str,
         "encrypted": bool,
         "parentImage": str,
         "dateCreated": str,
         "tags": Dict[str, str],
         "workingDirectory": str,
@@ -2310,15 +2458,15 @@
 
 _RequiredCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerRecipeRequestRequestTypeDef",
     {
         "containerType": Literal["DOCKER"],
         "name": str,
         "semanticVersion": str,
-        "components": Sequence[ComponentConfigurationTypeDef],
+        "components": Sequence[ComponentConfigurationUnionTypeDef],
         "parentImage": str,
         "targetRepository": TargetContainerRepositoryTypeDef,
         "clientToken": str,
     },
 )
 _OptionalCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerRecipeRequestRequestTypeDef",
@@ -2340,163 +2488,118 @@
 class CreateContainerRecipeRequestRequestTypeDef(
     _RequiredCreateContainerRecipeRequestRequestTypeDef,
     _OptionalCreateContainerRecipeRequestRequestTypeDef,
 ):
     pass
 
 
+InstanceConfigurationUnionTypeDef = Union[
+    InstanceConfigurationTypeDef, InstanceConfigurationOutputTypeDef
+]
 GetImagePipelineResponseTypeDef = TypedDict(
     "GetImagePipelineResponseTypeDef",
     {
         "requestId": str,
         "imagePipeline": ImagePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImagePipelinesResponseTypeDef = TypedDict(
     "ListImagePipelinesResponseTypeDef",
     {
         "requestId": str,
         "imagePipelineList": List[ImagePipelineTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "name": str,
-        "distributions": Sequence[DistributionTypeDef],
-        "clientToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
 
 _RequiredDistributionConfigurationTypeDef = TypedDict(
     "_RequiredDistributionConfigurationTypeDef",
     {
         "timeoutMinutes": int,
     },
 )
 _OptionalDistributionConfigurationTypeDef = TypedDict(
     "_OptionalDistributionConfigurationTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
-        "distributions": List[DistributionTypeDef],
+        "distributions": List[DistributionOutputTypeDef],
         "dateCreated": str,
         "dateUpdated": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
 class DistributionConfigurationTypeDef(
     _RequiredDistributionConfigurationTypeDef, _OptionalDistributionConfigurationTypeDef
 ):
     pass
 
 
-_RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "distributionConfigurationArn": str,
-        "distributions": Sequence[DistributionTypeDef],
-        "clientToken": str,
-    },
-)
-_OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-
-class UpdateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredUpdateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalUpdateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
+DistributionUnionTypeDef = Union[DistributionTypeDef, DistributionOutputTypeDef]
 GetInfrastructureConfigurationResponseTypeDef = TypedDict(
     "GetInfrastructureConfigurationResponseTypeDef",
     {
         "requestId": str,
         "infrastructureConfiguration": InfrastructureConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageBuildVersionsResponseTypeDef = TypedDict(
     "ListImageBuildVersionsResponseTypeDef",
     {
         "requestId": str,
         "imageSummaryList": List[ImageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImagePipelineImagesResponseTypeDef = TypedDict(
     "ListImagePipelineImagesResponseTypeDef",
     {
         "requestId": str,
         "imageSummaryList": List[ImageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageScanFindingsResponseTypeDef = TypedDict(
     "ListImageScanFindingsResponseTypeDef",
     {
         "requestId": str,
         "findings": List[ImageScanFindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContainerRecipeResponseTypeDef = TypedDict(
     "GetContainerRecipeResponseTypeDef",
     {
         "requestId": str,
         "containerRecipe": ContainerRecipeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDistributionConfigurationResponseTypeDef = TypedDict(
     "GetDistributionConfigurationResponseTypeDef",
     {
         "requestId": str,
         "distributionConfiguration": DistributionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "arn": str,
@@ -2516,20 +2619,69 @@
         "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
         "dateCreated": str,
         "outputResources": OutputResourcesTypeDef,
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
         "scanState": ImageScanStateTypeDef,
-        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
+        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "name": str,
+        "distributions": Sequence[DistributionUnionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "distributionConfigurationArn": str,
+        "distributions": Sequence[DistributionUnionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
     },
     total=False,
 )
 
+
+class UpdateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredUpdateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalUpdateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 GetImageResponseTypeDef = TypedDict(
     "GetImageResponseTypeDef",
     {
         "requestId": str,
         "image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder/type_defs.pyi` & `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_imagebuilder.type_defs import SeverityCountsTypeDef
 
-    data: SeverityCountsTypeDef = {...}
+    data: SeverityCountsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BuildTypeType,
     ComponentTypeType,
     DiskImageFormatType,
     EbsVolumeTypeType,
     ImageScanStatusType,
@@ -42,132 +42,139 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "SeverityCountsTypeDef",
     "SystemsManagerAgentTypeDef",
+    "LaunchPermissionConfigurationOutputTypeDef",
     "LaunchPermissionConfigurationTypeDef",
     "ImageStateTypeDef",
     "CancelImageCreationRequestRequestTypeDef",
-    "CancelImageCreationResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "ComponentParameterOutputTypeDef",
     "ComponentParameterTypeDef",
     "ComponentParameterDetailTypeDef",
     "ComponentStateTypeDef",
     "ComponentVersionTypeDef",
     "TargetContainerRepositoryTypeDef",
     "ContainerRecipeSummaryTypeDef",
     "ContainerTypeDef",
     "CreateComponentRequestRequestTypeDef",
-    "CreateComponentResponseTypeDef",
-    "CreateContainerRecipeResponseTypeDef",
-    "CreateDistributionConfigurationResponseTypeDef",
     "ImageTestsConfigurationTypeDef",
     "ScheduleTypeDef",
-    "CreateImagePipelineResponseTypeDef",
-    "CreateImageRecipeResponseTypeDef",
-    "CreateImageResponseTypeDef",
     "InstanceMetadataOptionsTypeDef",
-    "CreateInfrastructureConfigurationResponseTypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DeleteComponentRequestRequestTypeDef",
-    "DeleteComponentResponseTypeDef",
     "DeleteContainerRecipeRequestRequestTypeDef",
-    "DeleteContainerRecipeResponseTypeDef",
     "DeleteDistributionConfigurationRequestRequestTypeDef",
-    "DeleteDistributionConfigurationResponseTypeDef",
     "DeleteImagePipelineRequestRequestTypeDef",
-    "DeleteImagePipelineResponseTypeDef",
     "DeleteImageRecipeRequestRequestTypeDef",
-    "DeleteImageRecipeResponseTypeDef",
     "DeleteImageRequestRequestTypeDef",
-    "DeleteImageResponseTypeDef",
     "DeleteInfrastructureConfigurationRequestRequestTypeDef",
-    "DeleteInfrastructureConfigurationResponseTypeDef",
     "DistributionConfigurationSummaryTypeDef",
     "LaunchTemplateConfigurationTypeDef",
     "S3ExportConfigurationTypeDef",
     "EbsInstanceBlockDeviceSpecificationTypeDef",
+    "EcrConfigurationOutputTypeDef",
     "EcrConfigurationTypeDef",
     "FastLaunchLaunchTemplateSpecificationTypeDef",
     "FastLaunchSnapshotConfigurationTypeDef",
     "FilterTypeDef",
     "GetComponentPolicyRequestRequestTypeDef",
-    "GetComponentPolicyResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetContainerRecipePolicyRequestRequestTypeDef",
-    "GetContainerRecipePolicyResponseTypeDef",
     "GetContainerRecipeRequestRequestTypeDef",
     "GetDistributionConfigurationRequestRequestTypeDef",
     "GetImagePipelineRequestRequestTypeDef",
     "GetImagePolicyRequestRequestTypeDef",
-    "GetImagePolicyResponseTypeDef",
     "GetImageRecipePolicyRequestRequestTypeDef",
-    "GetImageRecipePolicyResponseTypeDef",
     "GetImageRecipeRequestRequestTypeDef",
     "GetImageRequestRequestTypeDef",
     "GetInfrastructureConfigurationRequestRequestTypeDef",
     "GetWorkflowExecutionRequestRequestTypeDef",
-    "GetWorkflowExecutionResponseTypeDef",
     "GetWorkflowStepExecutionRequestRequestTypeDef",
-    "GetWorkflowStepExecutionResponseTypeDef",
     "ImagePackageTypeDef",
     "ImageRecipeSummaryTypeDef",
     "ImageScanFindingsFilterTypeDef",
     "ImageScanStateTypeDef",
     "ImageVersionTypeDef",
     "ImportComponentRequestRequestTypeDef",
-    "ImportComponentResponseTypeDef",
     "ImportVmImageRequestRequestTypeDef",
-    "ImportVmImageResponseTypeDef",
     "InfrastructureConfigurationSummaryTypeDef",
     "ListComponentBuildVersionsRequestRequestTypeDef",
     "ListImagePackagesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWorkflowExecutionsRequestRequestTypeDef",
     "WorkflowExecutionMetadataTypeDef",
     "ListWorkflowStepExecutionsRequestRequestTypeDef",
     "WorkflowStepMetadataTypeDef",
     "S3LogsTypeDef",
     "VulnerablePackageTypeDef",
     "PutComponentPolicyRequestRequestTypeDef",
-    "PutComponentPolicyResponseTypeDef",
     "PutContainerRecipePolicyRequestRequestTypeDef",
-    "PutContainerRecipePolicyResponseTypeDef",
     "PutImagePolicyRequestRequestTypeDef",
-    "PutImagePolicyResponseTypeDef",
     "PutImageRecipePolicyRequestRequestTypeDef",
-    "PutImageRecipePolicyResponseTypeDef",
     "RemediationRecommendationTypeDef",
-    "ResponseMetadataTypeDef",
     "StartImagePipelineExecutionRequestRequestTypeDef",
-    "StartImagePipelineExecutionResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateDistributionConfigurationResponseTypeDef",
-    "UpdateImagePipelineResponseTypeDef",
-    "UpdateInfrastructureConfigurationResponseTypeDef",
     "AccountAggregationTypeDef",
     "ImageAggregationTypeDef",
     "ImagePipelineAggregationTypeDef",
     "VulnerabilityIdAggregationTypeDef",
     "AdditionalInstanceConfigurationTypeDef",
+    "AmiDistributionConfigurationOutputTypeDef",
     "AmiDistributionConfigurationTypeDef",
     "AmiTypeDef",
+    "CancelImageCreationResponseTypeDef",
+    "CreateComponentResponseTypeDef",
+    "CreateContainerRecipeResponseTypeDef",
+    "CreateDistributionConfigurationResponseTypeDef",
+    "CreateImagePipelineResponseTypeDef",
+    "CreateImageRecipeResponseTypeDef",
+    "CreateImageResponseTypeDef",
+    "CreateInfrastructureConfigurationResponseTypeDef",
+    "DeleteComponentResponseTypeDef",
+    "DeleteContainerRecipeResponseTypeDef",
+    "DeleteDistributionConfigurationResponseTypeDef",
+    "DeleteImagePipelineResponseTypeDef",
+    "DeleteImageRecipeResponseTypeDef",
+    "DeleteImageResponseTypeDef",
+    "DeleteInfrastructureConfigurationResponseTypeDef",
+    "GetComponentPolicyResponseTypeDef",
+    "GetContainerRecipePolicyResponseTypeDef",
+    "GetImagePolicyResponseTypeDef",
+    "GetImageRecipePolicyResponseTypeDef",
+    "GetWorkflowExecutionResponseTypeDef",
+    "GetWorkflowStepExecutionResponseTypeDef",
+    "ImportComponentResponseTypeDef",
+    "ImportVmImageResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutComponentPolicyResponseTypeDef",
+    "PutContainerRecipePolicyResponseTypeDef",
+    "PutImagePolicyResponseTypeDef",
+    "PutImageRecipePolicyResponseTypeDef",
+    "StartImagePipelineExecutionResponseTypeDef",
+    "UpdateDistributionConfigurationResponseTypeDef",
+    "UpdateImagePipelineResponseTypeDef",
+    "UpdateInfrastructureConfigurationResponseTypeDef",
+    "ComponentConfigurationOutputTypeDef",
     "ComponentConfigurationTypeDef",
     "ComponentSummaryTypeDef",
     "ComponentTypeDef",
     "ListComponentsResponseTypeDef",
+    "ContainerDistributionConfigurationOutputTypeDef",
     "ContainerDistributionConfigurationTypeDef",
     "ListContainerRecipesResponseTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDistributionConfigurationsResponseTypeDef",
     "InstanceBlockDeviceMappingTypeDef",
+    "ImageScanningConfigurationOutputTypeDef",
     "ImageScanningConfigurationTypeDef",
     "FastLaunchConfigurationTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListContainerRecipesRequestRequestTypeDef",
     "ListDistributionConfigurationsRequestRequestTypeDef",
     "ListImageBuildVersionsRequestRequestTypeDef",
     "ListImagePipelineImagesRequestRequestTypeDef",
@@ -184,46 +191,52 @@
     "ListWorkflowExecutionsResponseTypeDef",
     "ListWorkflowStepExecutionsResponseTypeDef",
     "LoggingTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "ImageScanFindingAggregationTypeDef",
     "OutputResourcesTypeDef",
+    "ComponentConfigurationUnionTypeDef",
     "ListComponentBuildVersionsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "InspectorScoreDetailsTypeDef",
-    "CreateImageRecipeRequestRequestTypeDef",
     "ImageRecipeTypeDef",
+    "InstanceConfigurationOutputTypeDef",
     "InstanceConfigurationTypeDef",
+    "ImagePipelineTypeDef",
     "CreateImagePipelineRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
-    "ImagePipelineTypeDef",
+    "ImageScanningConfigurationUnionTypeDef",
     "UpdateImagePipelineRequestRequestTypeDef",
+    "DistributionOutputTypeDef",
     "DistributionTypeDef",
     "CreateInfrastructureConfigurationRequestRequestTypeDef",
     "InfrastructureConfigurationTypeDef",
     "UpdateInfrastructureConfigurationRequestRequestTypeDef",
     "ListImageScanFindingAggregationsResponseTypeDef",
     "ImageSummaryTypeDef",
+    "CreateImageRecipeRequestRequestTypeDef",
     "ImageScanFindingTypeDef",
     "GetImageRecipeResponseTypeDef",
     "ContainerRecipeTypeDef",
     "CreateContainerRecipeRequestRequestTypeDef",
+    "InstanceConfigurationUnionTypeDef",
     "GetImagePipelineResponseTypeDef",
     "ListImagePipelinesResponseTypeDef",
-    "CreateDistributionConfigurationRequestRequestTypeDef",
     "DistributionConfigurationTypeDef",
-    "UpdateDistributionConfigurationRequestRequestTypeDef",
+    "DistributionUnionTypeDef",
     "GetInfrastructureConfigurationResponseTypeDef",
     "ListImageBuildVersionsResponseTypeDef",
     "ListImagePipelineImagesResponseTypeDef",
     "ListImageScanFindingsResponseTypeDef",
     "GetContainerRecipeResponseTypeDef",
     "GetDistributionConfigurationResponseTypeDef",
     "ImageTypeDef",
+    "CreateDistributionConfigurationRequestRequestTypeDef",
+    "UpdateDistributionConfigurationRequestRequestTypeDef",
     "GetImageResponseTypeDef",
 )
 
 SeverityCountsTypeDef = TypedDict(
     "SeverityCountsTypeDef",
     {
         "all": int,
@@ -238,14 +251,25 @@
     "SystemsManagerAgentTypeDef",
     {
         "uninstallAfterBuild": bool,
     },
     total=False,
 )
 
+LaunchPermissionConfigurationOutputTypeDef = TypedDict(
+    "LaunchPermissionConfigurationOutputTypeDef",
+    {
+        "userIds": List[str],
+        "userGroups": List[str],
+        "organizationArns": List[str],
+        "organizationalUnitArns": List[str],
+    },
+    total=False,
+)
+
 LaunchPermissionConfigurationTypeDef = TypedDict(
     "LaunchPermissionConfigurationTypeDef",
     {
         "userIds": Sequence[str],
         "userGroups": Sequence[str],
         "organizationArns": Sequence[str],
         "organizationalUnitArns": Sequence[str],
@@ -266,21 +290,30 @@
     "CancelImageCreationRequestRequestTypeDef",
     {
         "imageBuildVersionArn": str,
         "clientToken": str,
     },
 )
 
-CancelImageCreationResponseTypeDef = TypedDict(
-    "CancelImageCreationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "requestId": str,
-        "clientToken": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+ComponentParameterOutputTypeDef = TypedDict(
+    "ComponentParameterOutputTypeDef",
+    {
+        "name": str,
+        "value": List[str],
     },
 )
 
 ComponentParameterTypeDef = TypedDict(
     "ComponentParameterTypeDef",
     {
         "name": str,
@@ -390,44 +423,14 @@
 )
 
 class CreateComponentRequestRequestTypeDef(
     _RequiredCreateComponentRequestRequestTypeDef, _OptionalCreateComponentRequestRequestTypeDef
 ):
     pass
 
-CreateComponentResponseTypeDef = TypedDict(
-    "CreateComponentResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "componentBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateContainerRecipeResponseTypeDef = TypedDict(
-    "CreateContainerRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "containerRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDistributionConfigurationResponseTypeDef = TypedDict(
-    "CreateDistributionConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "distributionConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImageTestsConfigurationTypeDef = TypedDict(
     "ImageTestsConfigurationTypeDef",
     {
         "imageTestsEnabled": bool,
         "timeoutMinutes": int,
     },
     total=False,
@@ -439,63 +442,23 @@
         "scheduleExpression": str,
         "timezone": str,
         "pipelineExecutionStartCondition": PipelineExecutionStartConditionType,
     },
     total=False,
 )
 
-CreateImagePipelineResponseTypeDef = TypedDict(
-    "CreateImagePipelineResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imagePipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateImageRecipeResponseTypeDef = TypedDict(
-    "CreateImageRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imageRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateImageResponseTypeDef = TypedDict(
-    "CreateImageResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InstanceMetadataOptionsTypeDef = TypedDict(
     "InstanceMetadataOptionsTypeDef",
     {
         "httpTokens": str,
         "httpPutResponseHopLimit": int,
     },
     total=False,
 )
 
-CreateInfrastructureConfigurationResponseTypeDef = TypedDict(
-    "CreateInfrastructureConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "infrastructureConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CvssScoreAdjustmentTypeDef = TypedDict(
     "CvssScoreAdjustmentTypeDef",
     {
         "metric": str,
         "reason": str,
     },
     total=False,
@@ -515,119 +478,56 @@
 DeleteComponentRequestRequestTypeDef = TypedDict(
     "DeleteComponentRequestRequestTypeDef",
     {
         "componentBuildVersionArn": str,
     },
 )
 
-DeleteComponentResponseTypeDef = TypedDict(
-    "DeleteComponentResponseTypeDef",
-    {
-        "requestId": str,
-        "componentBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteContainerRecipeRequestRequestTypeDef = TypedDict(
     "DeleteContainerRecipeRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
     },
 )
 
-DeleteContainerRecipeResponseTypeDef = TypedDict(
-    "DeleteContainerRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "containerRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDistributionConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteDistributionConfigurationRequestRequestTypeDef",
     {
         "distributionConfigurationArn": str,
     },
 )
 
-DeleteDistributionConfigurationResponseTypeDef = TypedDict(
-    "DeleteDistributionConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "distributionConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImagePipelineRequestRequestTypeDef = TypedDict(
     "DeleteImagePipelineRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
     },
 )
 
-DeleteImagePipelineResponseTypeDef = TypedDict(
-    "DeleteImagePipelineResponseTypeDef",
-    {
-        "requestId": str,
-        "imagePipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImageRecipeRequestRequestTypeDef = TypedDict(
     "DeleteImageRecipeRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
     },
 )
 
-DeleteImageRecipeResponseTypeDef = TypedDict(
-    "DeleteImageRecipeResponseTypeDef",
-    {
-        "requestId": str,
-        "imageRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteImageRequestRequestTypeDef = TypedDict(
     "DeleteImageRequestRequestTypeDef",
     {
         "imageBuildVersionArn": str,
     },
 )
 
-DeleteImageResponseTypeDef = TypedDict(
-    "DeleteImageResponseTypeDef",
-    {
-        "requestId": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteInfrastructureConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteInfrastructureConfigurationRequestRequestTypeDef",
     {
         "infrastructureConfigurationArn": str,
     },
 )
 
-DeleteInfrastructureConfigurationResponseTypeDef = TypedDict(
-    "DeleteInfrastructureConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "infrastructureConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DistributionConfigurationSummaryTypeDef = TypedDict(
     "DistributionConfigurationSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
         "dateCreated": str,
@@ -690,14 +590,23 @@
         "volumeSize": int,
         "volumeType": EbsVolumeTypeType,
         "throughput": int,
     },
     total=False,
 )
 
+EcrConfigurationOutputTypeDef = TypedDict(
+    "EcrConfigurationOutputTypeDef",
+    {
+        "repositoryName": str,
+        "containerTags": List[str],
+    },
+    total=False,
+)
+
 EcrConfigurationTypeDef = TypedDict(
     "EcrConfigurationTypeDef",
     {
         "repositoryName": str,
         "containerTags": Sequence[str],
     },
     total=False,
@@ -733,46 +642,28 @@
 GetComponentPolicyRequestRequestTypeDef = TypedDict(
     "GetComponentPolicyRequestRequestTypeDef",
     {
         "componentArn": str,
     },
 )
 
-GetComponentPolicyResponseTypeDef = TypedDict(
-    "GetComponentPolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetComponentRequestRequestTypeDef = TypedDict(
     "GetComponentRequestRequestTypeDef",
     {
         "componentBuildVersionArn": str,
     },
 )
 
 GetContainerRecipePolicyRequestRequestTypeDef = TypedDict(
     "GetContainerRecipePolicyRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
     },
 )
 
-GetContainerRecipePolicyResponseTypeDef = TypedDict(
-    "GetContainerRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetContainerRecipeRequestRequestTypeDef = TypedDict(
     "GetContainerRecipeRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
     },
 )
 
@@ -793,39 +684,21 @@
 GetImagePolicyRequestRequestTypeDef = TypedDict(
     "GetImagePolicyRequestRequestTypeDef",
     {
         "imageArn": str,
     },
 )
 
-GetImagePolicyResponseTypeDef = TypedDict(
-    "GetImagePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetImageRecipePolicyRequestRequestTypeDef = TypedDict(
     "GetImageRecipePolicyRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
     },
 )
 
-GetImageRecipePolicyResponseTypeDef = TypedDict(
-    "GetImageRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetImageRecipeRequestRequestTypeDef = TypedDict(
     "GetImageRecipeRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
     },
 )
 
@@ -846,65 +719,21 @@
 GetWorkflowExecutionRequestRequestTypeDef = TypedDict(
     "GetWorkflowExecutionRequestRequestTypeDef",
     {
         "workflowExecutionId": str,
     },
 )
 
-GetWorkflowExecutionResponseTypeDef = TypedDict(
-    "GetWorkflowExecutionResponseTypeDef",
-    {
-        "requestId": str,
-        "workflowBuildVersionArn": str,
-        "workflowExecutionId": str,
-        "imageBuildVersionArn": str,
-        "type": WorkflowTypeType,
-        "status": WorkflowExecutionStatusType,
-        "message": str,
-        "totalStepCount": int,
-        "totalStepsSucceeded": int,
-        "totalStepsFailed": int,
-        "totalStepsSkipped": int,
-        "startTime": str,
-        "endTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkflowStepExecutionRequestRequestTypeDef = TypedDict(
     "GetWorkflowStepExecutionRequestRequestTypeDef",
     {
         "stepExecutionId": str,
     },
 )
 
-GetWorkflowStepExecutionResponseTypeDef = TypedDict(
-    "GetWorkflowStepExecutionResponseTypeDef",
-    {
-        "requestId": str,
-        "stepExecutionId": str,
-        "workflowBuildVersionArn": str,
-        "workflowExecutionId": str,
-        "imageBuildVersionArn": str,
-        "name": str,
-        "description": str,
-        "action": str,
-        "status": WorkflowStepExecutionStatusType,
-        "rollbackStatus": WorkflowStepExecutionRollbackStatusType,
-        "message": str,
-        "inputs": str,
-        "outputs": str,
-        "startTime": str,
-        "endTime": str,
-        "onFailure": str,
-        "timeoutSeconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImagePackageTypeDef = TypedDict(
     "ImagePackageTypeDef",
     {
         "packageName": str,
         "packageVersion": str,
     },
     total=False,
@@ -984,24 +813,14 @@
 )
 
 class ImportComponentRequestRequestTypeDef(
     _RequiredImportComponentRequestRequestTypeDef, _OptionalImportComponentRequestRequestTypeDef
 ):
     pass
 
-ImportComponentResponseTypeDef = TypedDict(
-    "ImportComponentResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "componentBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredImportVmImageRequestRequestTypeDef = TypedDict(
     "_RequiredImportVmImageRequestRequestTypeDef",
     {
         "name": str,
         "semanticVersion": str,
         "platform": PlatformType,
         "vmImportTaskId": str,
@@ -1019,24 +838,14 @@
 )
 
 class ImportVmImageRequestRequestTypeDef(
     _RequiredImportVmImageRequestRequestTypeDef, _OptionalImportVmImageRequestRequestTypeDef
 ):
     pass
 
-ImportVmImageResponseTypeDef = TypedDict(
-    "ImportVmImageResponseTypeDef",
-    {
-        "requestId": str,
-        "imageArn": str,
-        "clientToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InfrastructureConfigurationSummaryTypeDef = TypedDict(
     "InfrastructureConfigurationSummaryTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
         "dateCreated": str,
@@ -1093,22 +902,14 @@
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
 _RequiredListWorkflowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListWorkflowExecutionsRequestRequestTypeDef",
     {
         "imageBuildVersionArn": str,
     },
 )
 _OptionalListWorkflowExecutionsRequestRequestTypeDef = TypedDict(
@@ -1213,112 +1014,55 @@
     "PutComponentPolicyRequestRequestTypeDef",
     {
         "componentArn": str,
         "policy": str,
     },
 )
 
-PutComponentPolicyResponseTypeDef = TypedDict(
-    "PutComponentPolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "componentArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutContainerRecipePolicyRequestRequestTypeDef = TypedDict(
     "PutContainerRecipePolicyRequestRequestTypeDef",
     {
         "containerRecipeArn": str,
         "policy": str,
     },
 )
 
-PutContainerRecipePolicyResponseTypeDef = TypedDict(
-    "PutContainerRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "containerRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutImagePolicyRequestRequestTypeDef = TypedDict(
     "PutImagePolicyRequestRequestTypeDef",
     {
         "imageArn": str,
         "policy": str,
     },
 )
 
-PutImagePolicyResponseTypeDef = TypedDict(
-    "PutImagePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "imageArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutImageRecipePolicyRequestRequestTypeDef = TypedDict(
     "PutImageRecipePolicyRequestRequestTypeDef",
     {
         "imageRecipeArn": str,
         "policy": str,
     },
 )
 
-PutImageRecipePolicyResponseTypeDef = TypedDict(
-    "PutImageRecipePolicyResponseTypeDef",
-    {
-        "requestId": str,
-        "imageRecipeArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemediationRecommendationTypeDef = TypedDict(
     "RemediationRecommendationTypeDef",
     {
         "text": str,
         "url": str,
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
 StartImagePipelineExecutionRequestRequestTypeDef = TypedDict(
     "StartImagePipelineExecutionRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
         "clientToken": str,
     },
 )
 
-StartImagePipelineExecutionResponseTypeDef = TypedDict(
-    "StartImagePipelineExecutionResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imageBuildVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1327,44 +1071,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateDistributionConfigurationResponseTypeDef = TypedDict(
-    "UpdateDistributionConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "distributionConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateImagePipelineResponseTypeDef = TypedDict(
-    "UpdateImagePipelineResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "imagePipelineArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateInfrastructureConfigurationResponseTypeDef = TypedDict(
-    "UpdateInfrastructureConfigurationResponseTypeDef",
-    {
-        "requestId": str,
-        "clientToken": str,
-        "infrastructureConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AccountAggregationTypeDef = TypedDict(
     "AccountAggregationTypeDef",
     {
         "accountId": str,
         "severityCounts": SeverityCountsTypeDef,
     },
     total=False,
@@ -1402,14 +1116,27 @@
     {
         "systemsManagerAgent": SystemsManagerAgentTypeDef,
         "userDataOverride": str,
     },
     total=False,
 )
 
+AmiDistributionConfigurationOutputTypeDef = TypedDict(
+    "AmiDistributionConfigurationOutputTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "targetAccountIds": List[str],
+        "amiTags": Dict[str, str],
+        "kmsKeyId": str,
+        "launchPermission": LaunchPermissionConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 AmiDistributionConfigurationTypeDef = TypedDict(
     "AmiDistributionConfigurationTypeDef",
     {
         "name": str,
         "description": str,
         "targetAccountIds": Sequence[str],
         "amiTags": Mapping[str, str],
@@ -1428,14 +1155,360 @@
         "description": str,
         "state": ImageStateTypeDef,
         "accountId": str,
     },
     total=False,
 )
 
+CancelImageCreationResponseTypeDef = TypedDict(
+    "CancelImageCreationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateComponentResponseTypeDef = TypedDict(
+    "CreateComponentResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "componentBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateContainerRecipeResponseTypeDef = TypedDict(
+    "CreateContainerRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "containerRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDistributionConfigurationResponseTypeDef = TypedDict(
+    "CreateDistributionConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "distributionConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImagePipelineResponseTypeDef = TypedDict(
+    "CreateImagePipelineResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imagePipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImageRecipeResponseTypeDef = TypedDict(
+    "CreateImageRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateImageResponseTypeDef = TypedDict(
+    "CreateImageResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateInfrastructureConfigurationResponseTypeDef = TypedDict(
+    "CreateInfrastructureConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "infrastructureConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteComponentResponseTypeDef = TypedDict(
+    "DeleteComponentResponseTypeDef",
+    {
+        "requestId": str,
+        "componentBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteContainerRecipeResponseTypeDef = TypedDict(
+    "DeleteContainerRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "containerRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDistributionConfigurationResponseTypeDef = TypedDict(
+    "DeleteDistributionConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "distributionConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImagePipelineResponseTypeDef = TypedDict(
+    "DeleteImagePipelineResponseTypeDef",
+    {
+        "requestId": str,
+        "imagePipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImageRecipeResponseTypeDef = TypedDict(
+    "DeleteImageRecipeResponseTypeDef",
+    {
+        "requestId": str,
+        "imageRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteImageResponseTypeDef = TypedDict(
+    "DeleteImageResponseTypeDef",
+    {
+        "requestId": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteInfrastructureConfigurationResponseTypeDef = TypedDict(
+    "DeleteInfrastructureConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "infrastructureConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComponentPolicyResponseTypeDef = TypedDict(
+    "GetComponentPolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContainerRecipePolicyResponseTypeDef = TypedDict(
+    "GetContainerRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImagePolicyResponseTypeDef = TypedDict(
+    "GetImagePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImageRecipePolicyResponseTypeDef = TypedDict(
+    "GetImageRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkflowExecutionResponseTypeDef = TypedDict(
+    "GetWorkflowExecutionResponseTypeDef",
+    {
+        "requestId": str,
+        "workflowBuildVersionArn": str,
+        "workflowExecutionId": str,
+        "imageBuildVersionArn": str,
+        "type": WorkflowTypeType,
+        "status": WorkflowExecutionStatusType,
+        "message": str,
+        "totalStepCount": int,
+        "totalStepsSucceeded": int,
+        "totalStepsFailed": int,
+        "totalStepsSkipped": int,
+        "startTime": str,
+        "endTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkflowStepExecutionResponseTypeDef = TypedDict(
+    "GetWorkflowStepExecutionResponseTypeDef",
+    {
+        "requestId": str,
+        "stepExecutionId": str,
+        "workflowBuildVersionArn": str,
+        "workflowExecutionId": str,
+        "imageBuildVersionArn": str,
+        "name": str,
+        "description": str,
+        "action": str,
+        "status": WorkflowStepExecutionStatusType,
+        "rollbackStatus": WorkflowStepExecutionRollbackStatusType,
+        "message": str,
+        "inputs": str,
+        "outputs": str,
+        "startTime": str,
+        "endTime": str,
+        "onFailure": str,
+        "timeoutSeconds": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportComponentResponseTypeDef = TypedDict(
+    "ImportComponentResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "componentBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportVmImageResponseTypeDef = TypedDict(
+    "ImportVmImageResponseTypeDef",
+    {
+        "requestId": str,
+        "imageArn": str,
+        "clientToken": str,
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
+PutComponentPolicyResponseTypeDef = TypedDict(
+    "PutComponentPolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "componentArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutContainerRecipePolicyResponseTypeDef = TypedDict(
+    "PutContainerRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "containerRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutImagePolicyResponseTypeDef = TypedDict(
+    "PutImagePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "imageArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutImageRecipePolicyResponseTypeDef = TypedDict(
+    "PutImageRecipePolicyResponseTypeDef",
+    {
+        "requestId": str,
+        "imageRecipeArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartImagePipelineExecutionResponseTypeDef = TypedDict(
+    "StartImagePipelineExecutionResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imageBuildVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDistributionConfigurationResponseTypeDef = TypedDict(
+    "UpdateDistributionConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "distributionConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateImagePipelineResponseTypeDef = TypedDict(
+    "UpdateImagePipelineResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "imagePipelineArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateInfrastructureConfigurationResponseTypeDef = TypedDict(
+    "UpdateInfrastructureConfigurationResponseTypeDef",
+    {
+        "requestId": str,
+        "clientToken": str,
+        "infrastructureConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredComponentConfigurationOutputTypeDef = TypedDict(
+    "_RequiredComponentConfigurationOutputTypeDef",
+    {
+        "componentArn": str,
+    },
+)
+_OptionalComponentConfigurationOutputTypeDef = TypedDict(
+    "_OptionalComponentConfigurationOutputTypeDef",
+    {
+        "parameters": List[ComponentParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+class ComponentConfigurationOutputTypeDef(
+    _RequiredComponentConfigurationOutputTypeDef, _OptionalComponentConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredComponentConfigurationTypeDef = TypedDict(
     "_RequiredComponentConfigurationTypeDef",
     {
         "componentArn": str,
     },
 )
 _OptionalComponentConfigurationTypeDef = TypedDict(
@@ -1499,18 +1572,39 @@
 
 ListComponentsResponseTypeDef = TypedDict(
     "ListComponentsResponseTypeDef",
     {
         "requestId": str,
         "componentVersionList": List[ComponentVersionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredContainerDistributionConfigurationOutputTypeDef = TypedDict(
+    "_RequiredContainerDistributionConfigurationOutputTypeDef",
+    {
+        "targetRepository": TargetContainerRepositoryTypeDef,
+    },
+)
+_OptionalContainerDistributionConfigurationOutputTypeDef = TypedDict(
+    "_OptionalContainerDistributionConfigurationOutputTypeDef",
+    {
+        "description": str,
+        "containerTags": List[str],
     },
+    total=False,
 )
 
+class ContainerDistributionConfigurationOutputTypeDef(
+    _RequiredContainerDistributionConfigurationOutputTypeDef,
+    _OptionalContainerDistributionConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredContainerDistributionConfigurationTypeDef = TypedDict(
     "_RequiredContainerDistributionConfigurationTypeDef",
     {
         "targetRepository": TargetContainerRepositoryTypeDef,
     },
 )
 _OptionalContainerDistributionConfigurationTypeDef = TypedDict(
@@ -1530,15 +1624,15 @@
 
 ListContainerRecipesResponseTypeDef = TypedDict(
     "ListContainerRecipesResponseTypeDef",
     {
         "requestId": str,
         "containerRecipeSummaryList": List[ContainerRecipeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CvssScoreDetailsTypeDef = TypedDict(
     "CvssScoreDetailsTypeDef",
     {
         "scoreSource": str,
@@ -1553,29 +1647,38 @@
 
 ListDistributionConfigurationsResponseTypeDef = TypedDict(
     "ListDistributionConfigurationsResponseTypeDef",
     {
         "requestId": str,
         "distributionConfigurationSummaryList": List[DistributionConfigurationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceBlockDeviceMappingTypeDef = TypedDict(
     "InstanceBlockDeviceMappingTypeDef",
     {
         "deviceName": str,
         "ebs": EbsInstanceBlockDeviceSpecificationTypeDef,
         "virtualName": str,
         "noDevice": str,
     },
     total=False,
 )
 
+ImageScanningConfigurationOutputTypeDef = TypedDict(
+    "ImageScanningConfigurationOutputTypeDef",
+    {
+        "imageScanningEnabled": bool,
+        "ecrConfiguration": EcrConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 ImageScanningConfigurationTypeDef = TypedDict(
     "ImageScanningConfigurationTypeDef",
     {
         "imageScanningEnabled": bool,
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
     total=False,
@@ -1735,25 +1838,25 @@
 
 ListImagePackagesResponseTypeDef = TypedDict(
     "ListImagePackagesResponseTypeDef",
     {
         "requestId": str,
         "imagePackageList": List[ImagePackageTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageRecipesResponseTypeDef = TypedDict(
     "ListImageRecipesResponseTypeDef",
     {
         "requestId": str,
         "imageRecipeSummaryList": List[ImageRecipeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageScanFindingsRequestRequestTypeDef = TypedDict(
     "ListImageScanFindingsRequestRequestTypeDef",
     {
         "filters": Sequence[ImageScanFindingsFilterTypeDef],
@@ -1765,51 +1868,51 @@
 
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
         "requestId": str,
         "imageVersionList": List[ImageVersionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInfrastructureConfigurationsResponseTypeDef = TypedDict(
     "ListInfrastructureConfigurationsResponseTypeDef",
     {
         "requestId": str,
         "infrastructureConfigurationSummaryList": List[InfrastructureConfigurationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowExecutionsResponseTypeDef = TypedDict(
     "ListWorkflowExecutionsResponseTypeDef",
     {
         "requestId": str,
         "workflowExecutions": List[WorkflowExecutionMetadataTypeDef],
         "imageBuildVersionArn": str,
         "message": str,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkflowStepExecutionsResponseTypeDef = TypedDict(
     "ListWorkflowStepExecutionsResponseTypeDef",
     {
         "requestId": str,
         "steps": List[WorkflowStepMetadataTypeDef],
         "workflowBuildVersionArn": str,
         "workflowExecutionId": str,
         "imageBuildVersionArn": str,
         "message": str,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "s3Logs": S3LogsTypeDef,
@@ -1868,98 +1971,108 @@
     {
         "amis": List[AmiTypeDef],
         "containers": List[ContainerTypeDef],
     },
     total=False,
 )
 
+ComponentConfigurationUnionTypeDef = Union[
+    ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef
+]
 ListComponentBuildVersionsResponseTypeDef = TypedDict(
     "ListComponentBuildVersionsResponseTypeDef",
     {
         "requestId": str,
         "componentSummaryList": List[ComponentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComponentResponseTypeDef = TypedDict(
     "GetComponentResponseTypeDef",
     {
         "requestId": str,
         "component": ComponentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InspectorScoreDetailsTypeDef = TypedDict(
     "InspectorScoreDetailsTypeDef",
     {
         "adjustedCvss": CvssScoreDetailsTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateImageRecipeRequestRequestTypeDef",
-    {
-        "name": str,
-        "semanticVersion": str,
-        "components": Sequence[ComponentConfigurationTypeDef],
-        "parentImage": str,
-        "clientToken": str,
-    },
-)
-_OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateImageRecipeRequestRequestTypeDef",
-    {
-        "description": str,
-        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
-        "tags": Mapping[str, str],
-        "workingDirectory": str,
-        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class CreateImageRecipeRequestRequestTypeDef(
-    _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
-):
-    pass
-
 ImageRecipeTypeDef = TypedDict(
     "ImageRecipeTypeDef",
     {
         "arn": str,
         "type": ImageTypeType,
         "name": str,
         "description": str,
         "platform": PlatformType,
         "owner": str,
         "version": str,
-        "components": List[ComponentConfigurationTypeDef],
+        "components": List[ComponentConfigurationOutputTypeDef],
         "parentImage": str,
         "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
         "dateCreated": str,
         "tags": Dict[str, str],
         "workingDirectory": str,
         "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
     },
     total=False,
 )
 
+InstanceConfigurationOutputTypeDef = TypedDict(
+    "InstanceConfigurationOutputTypeDef",
+    {
+        "image": str,
+        "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
+    },
+    total=False,
+)
+
 InstanceConfigurationTypeDef = TypedDict(
     "InstanceConfigurationTypeDef",
     {
         "image": str,
         "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
     },
     total=False,
 )
 
+ImagePipelineTypeDef = TypedDict(
+    "ImagePipelineTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "platform": PlatformType,
+        "enhancedImageMetadataEnabled": bool,
+        "imageRecipeArn": str,
+        "containerRecipeArn": str,
+        "infrastructureConfigurationArn": str,
+        "distributionConfigurationArn": str,
+        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
+        "schedule": ScheduleTypeDef,
+        "status": PipelineStatusType,
+        "dateCreated": str,
+        "dateUpdated": str,
+        "dateLastRun": str,
+        "dateNextRun": str,
+        "tags": Dict[str, str],
+        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImagePipelineRequestRequestTypeDef",
     {
         "name": str,
         "infrastructureConfigurationArn": str,
         "clientToken": str,
     },
@@ -2009,39 +2122,17 @@
 )
 
 class CreateImageRequestRequestTypeDef(
     _RequiredCreateImageRequestRequestTypeDef, _OptionalCreateImageRequestRequestTypeDef
 ):
     pass
 
-ImagePipelineTypeDef = TypedDict(
-    "ImagePipelineTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "platform": PlatformType,
-        "enhancedImageMetadataEnabled": bool,
-        "imageRecipeArn": str,
-        "containerRecipeArn": str,
-        "infrastructureConfigurationArn": str,
-        "distributionConfigurationArn": str,
-        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
-        "schedule": ScheduleTypeDef,
-        "status": PipelineStatusType,
-        "dateCreated": str,
-        "dateUpdated": str,
-        "dateLastRun": str,
-        "dateNextRun": str,
-        "tags": Dict[str, str],
-        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
-    },
-    total=False,
-)
-
+ImageScanningConfigurationUnionTypeDef = Union[
+    ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
+]
 _RequiredUpdateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImagePipelineRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
         "infrastructureConfigurationArn": str,
         "clientToken": str,
     },
@@ -2064,14 +2155,38 @@
 
 class UpdateImagePipelineRequestRequestTypeDef(
     _RequiredUpdateImagePipelineRequestRequestTypeDef,
     _OptionalUpdateImagePipelineRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDistributionOutputTypeDef = TypedDict(
+    "_RequiredDistributionOutputTypeDef",
+    {
+        "region": str,
+    },
+)
+_OptionalDistributionOutputTypeDef = TypedDict(
+    "_OptionalDistributionOutputTypeDef",
+    {
+        "amiDistributionConfiguration": AmiDistributionConfigurationOutputTypeDef,
+        "containerDistributionConfiguration": ContainerDistributionConfigurationOutputTypeDef,
+        "licenseConfigurationArns": List[str],
+        "launchTemplateConfigurations": List[LaunchTemplateConfigurationTypeDef],
+        "s3ExportConfiguration": S3ExportConfigurationTypeDef,
+        "fastLaunchConfigurations": List[FastLaunchConfigurationTypeDef],
+    },
+    total=False,
+)
+
+class DistributionOutputTypeDef(
+    _RequiredDistributionOutputTypeDef, _OptionalDistributionOutputTypeDef
+):
+    pass
+
 _RequiredDistributionTypeDef = TypedDict(
     "_RequiredDistributionTypeDef",
     {
         "region": str,
     },
 )
 _OptionalDistributionTypeDef = TypedDict(
@@ -2179,15 +2294,15 @@
 ListImageScanFindingAggregationsResponseTypeDef = TypedDict(
     "ListImageScanFindingAggregationsResponseTypeDef",
     {
         "requestId": str,
         "aggregationType": str,
         "responses": List[ImageScanFindingAggregationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageSummaryTypeDef = TypedDict(
     "ImageSummaryTypeDef",
     {
         "arn": str,
@@ -2203,14 +2318,41 @@
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
     },
     total=False,
 )
 
+_RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateImageRecipeRequestRequestTypeDef",
+    {
+        "name": str,
+        "semanticVersion": str,
+        "components": Sequence[ComponentConfigurationUnionTypeDef],
+        "parentImage": str,
+        "clientToken": str,
+    },
+)
+_OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateImageRecipeRequestRequestTypeDef",
+    {
+        "description": str,
+        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
+        "tags": Mapping[str, str],
+        "workingDirectory": str,
+        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class CreateImageRecipeRequestRequestTypeDef(
+    _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
+):
+    pass
+
 ImageScanFindingTypeDef = TypedDict(
     "ImageScanFindingTypeDef",
     {
         "awsAccountId": str,
         "imageBuildVersionArn": str,
         "imagePipelineArn": str,
         "type": str,
@@ -2229,30 +2371,30 @@
 )
 
 GetImageRecipeResponseTypeDef = TypedDict(
     "GetImageRecipeResponseTypeDef",
     {
         "requestId": str,
         "imageRecipe": ImageRecipeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ContainerRecipeTypeDef = TypedDict(
     "ContainerRecipeTypeDef",
     {
         "arn": str,
         "containerType": Literal["DOCKER"],
         "name": str,
         "description": str,
         "platform": PlatformType,
         "owner": str,
         "version": str,
-        "components": List[ComponentConfigurationTypeDef],
-        "instanceConfiguration": InstanceConfigurationTypeDef,
+        "components": List[ComponentConfigurationOutputTypeDef],
+        "instanceConfiguration": InstanceConfigurationOutputTypeDef,
         "dockerfileTemplateData": str,
         "kmsKeyId": str,
         "encrypted": bool,
         "parentImage": str,
         "dateCreated": str,
         "tags": Dict[str, str],
         "workingDirectory": str,
@@ -2263,15 +2405,15 @@
 
 _RequiredCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerRecipeRequestRequestTypeDef",
     {
         "containerType": Literal["DOCKER"],
         "name": str,
         "semanticVersion": str,
-        "components": Sequence[ComponentConfigurationTypeDef],
+        "components": Sequence[ComponentConfigurationUnionTypeDef],
         "parentImage": str,
         "targetRepository": TargetContainerRepositoryTypeDef,
         "clientToken": str,
     },
 )
 _OptionalCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerRecipeRequestRequestTypeDef",
@@ -2291,157 +2433,116 @@
 
 class CreateContainerRecipeRequestRequestTypeDef(
     _RequiredCreateContainerRecipeRequestRequestTypeDef,
     _OptionalCreateContainerRecipeRequestRequestTypeDef,
 ):
     pass
 
+InstanceConfigurationUnionTypeDef = Union[
+    InstanceConfigurationTypeDef, InstanceConfigurationOutputTypeDef
+]
 GetImagePipelineResponseTypeDef = TypedDict(
     "GetImagePipelineResponseTypeDef",
     {
         "requestId": str,
         "imagePipeline": ImagePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImagePipelinesResponseTypeDef = TypedDict(
     "ListImagePipelinesResponseTypeDef",
     {
         "requestId": str,
         "imagePipelineList": List[ImagePipelineTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "name": str,
-        "distributions": Sequence[DistributionTypeDef],
-        "clientToken": str,
-    },
-)
-_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
 _RequiredDistributionConfigurationTypeDef = TypedDict(
     "_RequiredDistributionConfigurationTypeDef",
     {
         "timeoutMinutes": int,
     },
 )
 _OptionalDistributionConfigurationTypeDef = TypedDict(
     "_OptionalDistributionConfigurationTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
-        "distributions": List[DistributionTypeDef],
+        "distributions": List[DistributionOutputTypeDef],
         "dateCreated": str,
         "dateUpdated": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class DistributionConfigurationTypeDef(
     _RequiredDistributionConfigurationTypeDef, _OptionalDistributionConfigurationTypeDef
 ):
     pass
 
-_RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "distributionConfigurationArn": str,
-        "distributions": Sequence[DistributionTypeDef],
-        "clientToken": str,
-    },
-)
-_OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-class UpdateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredUpdateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalUpdateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
+DistributionUnionTypeDef = Union[DistributionTypeDef, DistributionOutputTypeDef]
 GetInfrastructureConfigurationResponseTypeDef = TypedDict(
     "GetInfrastructureConfigurationResponseTypeDef",
     {
         "requestId": str,
         "infrastructureConfiguration": InfrastructureConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageBuildVersionsResponseTypeDef = TypedDict(
     "ListImageBuildVersionsResponseTypeDef",
     {
         "requestId": str,
         "imageSummaryList": List[ImageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImagePipelineImagesResponseTypeDef = TypedDict(
     "ListImagePipelineImagesResponseTypeDef",
     {
         "requestId": str,
         "imageSummaryList": List[ImageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListImageScanFindingsResponseTypeDef = TypedDict(
     "ListImageScanFindingsResponseTypeDef",
     {
         "requestId": str,
         "findings": List[ImageScanFindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContainerRecipeResponseTypeDef = TypedDict(
     "GetContainerRecipeResponseTypeDef",
     {
         "requestId": str,
         "containerRecipe": ContainerRecipeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDistributionConfigurationResponseTypeDef = TypedDict(
     "GetDistributionConfigurationResponseTypeDef",
     {
         "requestId": str,
         "distributionConfiguration": DistributionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageTypeDef = TypedDict(
     "ImageTypeDef",
     {
         "arn": str,
@@ -2461,20 +2562,65 @@
         "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
         "dateCreated": str,
         "outputResources": OutputResourcesTypeDef,
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
         "scanState": ImageScanStateTypeDef,
-        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
+        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "name": str,
+        "distributions": Sequence[DistributionUnionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+class CreateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "distributionConfigurationArn": str,
+        "distributions": Sequence[DistributionUnionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+class UpdateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredUpdateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalUpdateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
 GetImageResponseTypeDef = TypedDict(
     "GetImageResponseTypeDef",
     {
         "requestId": str,
         "image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder.egg-info/PKG-INFO` & `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-imagebuilder
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.imagebuilder 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.imagebuilder 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore imagebuilder type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore imagebuilder type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-imagebuilder"></a>
 
 # types-aiobotocore-imagebuilder
 
 [![PyPI - types-aiobotocore-imagebuilder](https://img.shields.io/pypi/v/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-imagebuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-imagebuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-imagebuilder?color=blue)](https://pypistats.org/packages/types-aiobotocore-imagebuilder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-imagebuilder)](https://pepy.tech/project/types-aiobotocore-imagebuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.imagebuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
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
 [types-aiobotocore-imagebuilder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/).
 
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
@@ -299,143 +298,150 @@
 )
 
 
 def check_value(value: BuildTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_imagebuilder.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_imagebuilder.type_defs import (
     SeverityCountsTypeDef,
     SystemsManagerAgentTypeDef,
+    LaunchPermissionConfigurationOutputTypeDef,
     LaunchPermissionConfigurationTypeDef,
     ImageStateTypeDef,
     CancelImageCreationRequestRequestTypeDef,
-    CancelImageCreationResponseTypeDef,
+    ResponseMetadataTypeDef,
+    ComponentParameterOutputTypeDef,
     ComponentParameterTypeDef,
     ComponentParameterDetailTypeDef,
     ComponentStateTypeDef,
     ComponentVersionTypeDef,
     TargetContainerRepositoryTypeDef,
     ContainerRecipeSummaryTypeDef,
     ContainerTypeDef,
     CreateComponentRequestRequestTypeDef,
-    CreateComponentResponseTypeDef,
-    CreateContainerRecipeResponseTypeDef,
-    CreateDistributionConfigurationResponseTypeDef,
     ImageTestsConfigurationTypeDef,
     ScheduleTypeDef,
-    CreateImagePipelineResponseTypeDef,
-    CreateImageRecipeResponseTypeDef,
-    CreateImageResponseTypeDef,
     InstanceMetadataOptionsTypeDef,
-    CreateInfrastructureConfigurationResponseTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteComponentRequestRequestTypeDef,
-    DeleteComponentResponseTypeDef,
     DeleteContainerRecipeRequestRequestTypeDef,
-    DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationRequestRequestTypeDef,
-    DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineRequestRequestTypeDef,
-    DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeRequestRequestTypeDef,
-    DeleteImageRecipeResponseTypeDef,
     DeleteImageRequestRequestTypeDef,
-    DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationRequestRequestTypeDef,
-    DeleteInfrastructureConfigurationResponseTypeDef,
     DistributionConfigurationSummaryTypeDef,
     LaunchTemplateConfigurationTypeDef,
     S3ExportConfigurationTypeDef,
     EbsInstanceBlockDeviceSpecificationTypeDef,
+    EcrConfigurationOutputTypeDef,
     EcrConfigurationTypeDef,
     FastLaunchLaunchTemplateSpecificationTypeDef,
     FastLaunchSnapshotConfigurationTypeDef,
     FilterTypeDef,
     GetComponentPolicyRequestRequestTypeDef,
-    GetComponentPolicyResponseTypeDef,
     GetComponentRequestRequestTypeDef,
     GetContainerRecipePolicyRequestRequestTypeDef,
-    GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeRequestRequestTypeDef,
     GetDistributionConfigurationRequestRequestTypeDef,
     GetImagePipelineRequestRequestTypeDef,
     GetImagePolicyRequestRequestTypeDef,
-    GetImagePolicyResponseTypeDef,
     GetImageRecipePolicyRequestRequestTypeDef,
-    GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeRequestRequestTypeDef,
     GetImageRequestRequestTypeDef,
     GetInfrastructureConfigurationRequestRequestTypeDef,
     GetWorkflowExecutionRequestRequestTypeDef,
-    GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionRequestRequestTypeDef,
-    GetWorkflowStepExecutionResponseTypeDef,
     ImagePackageTypeDef,
     ImageRecipeSummaryTypeDef,
     ImageScanFindingsFilterTypeDef,
     ImageScanStateTypeDef,
     ImageVersionTypeDef,
     ImportComponentRequestRequestTypeDef,
-    ImportComponentResponseTypeDef,
     ImportVmImageRequestRequestTypeDef,
-    ImportVmImageResponseTypeDef,
     InfrastructureConfigurationSummaryTypeDef,
     ListComponentBuildVersionsRequestRequestTypeDef,
     ListImagePackagesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkflowExecutionsRequestRequestTypeDef,
     WorkflowExecutionMetadataTypeDef,
     ListWorkflowStepExecutionsRequestRequestTypeDef,
     WorkflowStepMetadataTypeDef,
     S3LogsTypeDef,
     VulnerablePackageTypeDef,
     PutComponentPolicyRequestRequestTypeDef,
-    PutComponentPolicyResponseTypeDef,
     PutContainerRecipePolicyRequestRequestTypeDef,
-    PutContainerRecipePolicyResponseTypeDef,
     PutImagePolicyRequestRequestTypeDef,
-    PutImagePolicyResponseTypeDef,
     PutImageRecipePolicyRequestRequestTypeDef,
-    PutImageRecipePolicyResponseTypeDef,
     RemediationRecommendationTypeDef,
-    ResponseMetadataTypeDef,
     StartImagePipelineExecutionRequestRequestTypeDef,
-    StartImagePipelineExecutionResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateDistributionConfigurationResponseTypeDef,
-    UpdateImagePipelineResponseTypeDef,
-    UpdateInfrastructureConfigurationResponseTypeDef,
     AccountAggregationTypeDef,
     ImageAggregationTypeDef,
     ImagePipelineAggregationTypeDef,
     VulnerabilityIdAggregationTypeDef,
     AdditionalInstanceConfigurationTypeDef,
+    AmiDistributionConfigurationOutputTypeDef,
     AmiDistributionConfigurationTypeDef,
     AmiTypeDef,
+    CancelImageCreationResponseTypeDef,
+    CreateComponentResponseTypeDef,
+    CreateContainerRecipeResponseTypeDef,
+    CreateDistributionConfigurationResponseTypeDef,
+    CreateImagePipelineResponseTypeDef,
+    CreateImageRecipeResponseTypeDef,
+    CreateImageResponseTypeDef,
+    CreateInfrastructureConfigurationResponseTypeDef,
+    DeleteComponentResponseTypeDef,
+    DeleteContainerRecipeResponseTypeDef,
+    DeleteDistributionConfigurationResponseTypeDef,
+    DeleteImagePipelineResponseTypeDef,
+    DeleteImageRecipeResponseTypeDef,
+    DeleteImageResponseTypeDef,
+    DeleteInfrastructureConfigurationResponseTypeDef,
+    GetComponentPolicyResponseTypeDef,
+    GetContainerRecipePolicyResponseTypeDef,
+    GetImagePolicyResponseTypeDef,
+    GetImageRecipePolicyResponseTypeDef,
+    GetWorkflowExecutionResponseTypeDef,
+    GetWorkflowStepExecutionResponseTypeDef,
+    ImportComponentResponseTypeDef,
+    ImportVmImageResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutComponentPolicyResponseTypeDef,
+    PutContainerRecipePolicyResponseTypeDef,
+    PutImagePolicyResponseTypeDef,
+    PutImageRecipePolicyResponseTypeDef,
+    StartImagePipelineExecutionResponseTypeDef,
+    UpdateDistributionConfigurationResponseTypeDef,
+    UpdateImagePipelineResponseTypeDef,
+    UpdateInfrastructureConfigurationResponseTypeDef,
+    ComponentConfigurationOutputTypeDef,
     ComponentConfigurationTypeDef,
     ComponentSummaryTypeDef,
     ComponentTypeDef,
     ListComponentsResponseTypeDef,
+    ContainerDistributionConfigurationOutputTypeDef,
     ContainerDistributionConfigurationTypeDef,
     ListContainerRecipesResponseTypeDef,
     CvssScoreDetailsTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
     InstanceBlockDeviceMappingTypeDef,
+    ImageScanningConfigurationOutputTypeDef,
     ImageScanningConfigurationTypeDef,
     FastLaunchConfigurationTypeDef,
     ListComponentsRequestRequestTypeDef,
     ListContainerRecipesRequestRequestTypeDef,
     ListDistributionConfigurationsRequestRequestTypeDef,
     ListImageBuildVersionsRequestRequestTypeDef,
     ListImagePipelineImagesRequestRequestTypeDef,
@@ -452,51 +458,57 @@
     ListWorkflowExecutionsResponseTypeDef,
     ListWorkflowStepExecutionsResponseTypeDef,
     LoggingTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
     ImageScanFindingAggregationTypeDef,
     OutputResourcesTypeDef,
+    ComponentConfigurationUnionTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     GetComponentResponseTypeDef,
     InspectorScoreDetailsTypeDef,
-    CreateImageRecipeRequestRequestTypeDef,
     ImageRecipeTypeDef,
+    InstanceConfigurationOutputTypeDef,
     InstanceConfigurationTypeDef,
+    ImagePipelineTypeDef,
     CreateImagePipelineRequestRequestTypeDef,
     CreateImageRequestRequestTypeDef,
-    ImagePipelineTypeDef,
+    ImageScanningConfigurationUnionTypeDef,
     UpdateImagePipelineRequestRequestTypeDef,
+    DistributionOutputTypeDef,
     DistributionTypeDef,
     CreateInfrastructureConfigurationRequestRequestTypeDef,
     InfrastructureConfigurationTypeDef,
     UpdateInfrastructureConfigurationRequestRequestTypeDef,
     ListImageScanFindingAggregationsResponseTypeDef,
     ImageSummaryTypeDef,
+    CreateImageRecipeRequestRequestTypeDef,
     ImageScanFindingTypeDef,
     GetImageRecipeResponseTypeDef,
     ContainerRecipeTypeDef,
     CreateContainerRecipeRequestRequestTypeDef,
+    InstanceConfigurationUnionTypeDef,
     GetImagePipelineResponseTypeDef,
     ListImagePipelinesResponseTypeDef,
-    CreateDistributionConfigurationRequestRequestTypeDef,
     DistributionConfigurationTypeDef,
-    UpdateDistributionConfigurationRequestRequestTypeDef,
+    DistributionUnionTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePipelineImagesResponseTypeDef,
     ListImageScanFindingsResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
     ImageTypeDef,
+    CreateDistributionConfigurationRequestRequestTypeDef,
+    UpdateDistributionConfigurationRequestRequestTypeDef,
     GetImageResponseTypeDef,
 )
 
 
-def get_structure() -> SeverityCountsTypeDef:
+def get_value() -> SeverityCountsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt` & `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*


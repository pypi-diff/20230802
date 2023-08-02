# Comparing `tmp/types-aiobotocore-ecr-2.5.2.tar.gz` & `tmp/types-aiobotocore-ecr-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ecr-2.5.2.tar", last modified: Sat Jul  8 01:43:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-ecr-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
```

## Comparing `types-aiobotocore-ecr-2.5.2.tar` & `types-aiobotocore-ecr-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:34.346069 types-aiobotocore-ecr-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-07-08 01:43:34.346069 types-aiobotocore-ecr-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:34.346069 types-aiobotocore-ecr-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:34.346069 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35776 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35718 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51990 2023-07-08 01:30:05.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51917 2023-07-08 01:30:05.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-08 01:30:04.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:34.346069 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20511 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:34.000000 types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.305595 types-aiobotocore-ecr-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-08-02 14:52:14.305595 types-aiobotocore-ecr-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19158 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.305595 types-aiobotocore-ecr-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.297595 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35749 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35691 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-08-02 14:37:50.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-08-02 14:37:50.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53296 2023-08-02 14:37:52.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53221 2023-08-02 14:37:52.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-02 14:37:50.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-08-02 14:37:49.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.305595 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ecr-2.5.2/LICENSE` & `types-aiobotocore-ecr-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2/PKG-INFO` & `types-aiobotocore-ecr-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ECR 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ECR 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ecr type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ecr type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ecr"></a>
 
 # types-aiobotocore-ecr
 
 [![PyPI - types-aiobotocore-ecr](https://img.shields.io/pypi/v/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ecr?color=blue)](https://pypistats.org/packages/types-aiobotocore-ecr)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr)](https://pepy.tech/project/types-aiobotocore-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ECR 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [types-aiobotocore-ecr docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/).
 
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
@@ -376,159 +375,165 @@
 )
 
 
 def check_value(value: DescribeImageScanFindingsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ecr.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ecr.type_defs import (
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
+    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
-    CreatePullThroughCacheRuleResponseTypeDef,
     EncryptionConfigurationTypeDef,
     ImageScanningConfigurationTypeDef,
     TagTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
-    DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleRequestRequestTypeDef,
-    DeletePullThroughCacheRuleResponseTypeDef,
-    DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
     ImageReplicationStatusTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     ImageScanStatusTypeDef,
     DescribeImagesFilterTypeDef,
-    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
     DescribePullThroughCacheRulesRequestRequestTypeDef,
     PullThroughCacheRuleTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
     GetDownloadUrlForLayerRequestRequestTypeDef,
-    GetDownloadUrlForLayerResponseTypeDef,
     LifecyclePolicyPreviewFilterTypeDef,
     LifecyclePolicyPreviewSummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
-    GetLifecyclePolicyResponseTypeDef,
-    GetRegistryPolicyResponseTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
     ImageScanFindingsSummaryTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
-    InitiateLayerUploadResponseTypeDef,
     LifecyclePolicyRuleActionTypeDef,
     ListImagesFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     VulnerablePackageTypeDef,
-    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutImageTagMutabilityRequestRequestTypeDef,
-    PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyRequestRequestTypeDef,
-    PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyRequestRequestTypeDef,
-    PutRegistryPolicyResponseTypeDef,
     RecommendationTypeDef,
     ScanningRepositoryFilterTypeDef,
     ReplicationDestinationTypeDef,
     RepositoryFilterTypeDef,
-    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
-    StartLifecyclePolicyPreviewResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
-    UploadLayerPartResponseTypeDef,
     ImageScanFindingTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
+    CompleteLayerUploadResponseTypeDef,
+    CreatePullThroughCacheRuleResponseTypeDef,
+    DeleteLifecyclePolicyResponseTypeDef,
+    DeletePullThroughCacheRuleResponseTypeDef,
+    DeleteRegistryPolicyResponseTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    GetDownloadUrlForLayerResponseTypeDef,
+    GetLifecyclePolicyResponseTypeDef,
+    GetRegistryPolicyResponseTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
+    InitiateLayerUploadResponseTypeDef,
+    PutImageTagMutabilityResponseTypeDef,
+    PutLifecyclePolicyResponseTypeDef,
+    PutRegistryPolicyResponseTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
+    StartLifecyclePolicyPreviewResponseTypeDef,
+    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
-    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
     StartImageScanRequestRequestTypeDef,
+    UploadLayerPartRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
     DescribeImageReplicationStatusResponseTypeDef,
+    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     StartImageScanResponseTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     DescribePullThroughCacheRulesResponseTypeDef,
     GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     GetLifecyclePolicyPreviewRequestRequestTypeDef,
     ImageDetailTypeDef,
     LifecyclePolicyPreviewResultTypeDef,
     ListImagesRequestListImagesPaginateTypeDef,
     ListImagesRequestRequestTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
+    RegistryScanningRuleOutputTypeDef,
     RegistryScanningRuleTypeDef,
     RepositoryScanningConfigurationTypeDef,
+    ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     ResourceTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     PutImageResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
     ScoreDetailsTypeDef,
     DescribeImagesResponseTypeDef,
     GetLifecyclePolicyPreviewResponseTypeDef,
-    PutRegistryScanningConfigurationRequestRequestTypeDef,
     RegistryScanningConfigurationTypeDef,
+    RegistryScanningRuleUnionTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     EnhancedImageScanFindingTypeDef,
     GetRegistryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
+    PutRegistryScanningConfigurationRequestRequestTypeDef,
     DescribeRegistryResponseTypeDef,
-    PutReplicationConfigurationRequestRequestTypeDef,
     PutReplicationConfigurationResponseTypeDef,
+    PutReplicationConfigurationRequestRequestTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     ImageScanFindingsTypeDef,
     DescribeImageScanFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ecr-2.5.2/README.md` & `types-aiobotocore-ecr-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-ecr"></a>
 
 # types-aiobotocore-ecr
 
 [![PyPI - types-aiobotocore-ecr](https://img.shields.io/pypi/v/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ecr?color=blue)](https://pypistats.org/packages/types-aiobotocore-ecr)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr)](https://pepy.tech/project/types-aiobotocore-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ECR 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [types-aiobotocore-ecr docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/).
 
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
@@ -343,159 +343,165 @@
 )
 
 
 def check_value(value: DescribeImageScanFindingsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ecr.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ecr.type_defs import (
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
+    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
-    CreatePullThroughCacheRuleResponseTypeDef,
     EncryptionConfigurationTypeDef,
     ImageScanningConfigurationTypeDef,
     TagTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
-    DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleRequestRequestTypeDef,
-    DeletePullThroughCacheRuleResponseTypeDef,
-    DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
     ImageReplicationStatusTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     ImageScanStatusTypeDef,
     DescribeImagesFilterTypeDef,
-    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
     DescribePullThroughCacheRulesRequestRequestTypeDef,
     PullThroughCacheRuleTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
     GetDownloadUrlForLayerRequestRequestTypeDef,
-    GetDownloadUrlForLayerResponseTypeDef,
     LifecyclePolicyPreviewFilterTypeDef,
     LifecyclePolicyPreviewSummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
-    GetLifecyclePolicyResponseTypeDef,
-    GetRegistryPolicyResponseTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
     ImageScanFindingsSummaryTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
-    InitiateLayerUploadResponseTypeDef,
     LifecyclePolicyRuleActionTypeDef,
     ListImagesFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     VulnerablePackageTypeDef,
-    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutImageTagMutabilityRequestRequestTypeDef,
-    PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyRequestRequestTypeDef,
-    PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyRequestRequestTypeDef,
-    PutRegistryPolicyResponseTypeDef,
     RecommendationTypeDef,
     ScanningRepositoryFilterTypeDef,
     ReplicationDestinationTypeDef,
     RepositoryFilterTypeDef,
-    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
-    StartLifecyclePolicyPreviewResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
-    UploadLayerPartResponseTypeDef,
     ImageScanFindingTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
+    CompleteLayerUploadResponseTypeDef,
+    CreatePullThroughCacheRuleResponseTypeDef,
+    DeleteLifecyclePolicyResponseTypeDef,
+    DeletePullThroughCacheRuleResponseTypeDef,
+    DeleteRegistryPolicyResponseTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    GetDownloadUrlForLayerResponseTypeDef,
+    GetLifecyclePolicyResponseTypeDef,
+    GetRegistryPolicyResponseTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
+    InitiateLayerUploadResponseTypeDef,
+    PutImageTagMutabilityResponseTypeDef,
+    PutLifecyclePolicyResponseTypeDef,
+    PutRegistryPolicyResponseTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
+    StartLifecyclePolicyPreviewResponseTypeDef,
+    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
-    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
     StartImageScanRequestRequestTypeDef,
+    UploadLayerPartRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
     DescribeImageReplicationStatusResponseTypeDef,
+    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     StartImageScanResponseTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     DescribePullThroughCacheRulesResponseTypeDef,
     GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     GetLifecyclePolicyPreviewRequestRequestTypeDef,
     ImageDetailTypeDef,
     LifecyclePolicyPreviewResultTypeDef,
     ListImagesRequestListImagesPaginateTypeDef,
     ListImagesRequestRequestTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
+    RegistryScanningRuleOutputTypeDef,
     RegistryScanningRuleTypeDef,
     RepositoryScanningConfigurationTypeDef,
+    ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     ResourceTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     PutImageResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
     ScoreDetailsTypeDef,
     DescribeImagesResponseTypeDef,
     GetLifecyclePolicyPreviewResponseTypeDef,
-    PutRegistryScanningConfigurationRequestRequestTypeDef,
     RegistryScanningConfigurationTypeDef,
+    RegistryScanningRuleUnionTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     EnhancedImageScanFindingTypeDef,
     GetRegistryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
+    PutRegistryScanningConfigurationRequestRequestTypeDef,
     DescribeRegistryResponseTypeDef,
-    PutReplicationConfigurationRequestRequestTypeDef,
     PutReplicationConfigurationResponseTypeDef,
+    PutReplicationConfigurationRequestRequestTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     ImageScanFindingsTypeDef,
     DescribeImageScanFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ecr-2.5.2/setup.py` & `types-aiobotocore-ecr-2.5.2.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ecr",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_ecr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ECR 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore ecr type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore ecr type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ecr": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/__init__.py` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/__init__.pyi` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/__main__.py` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ECR 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ECR 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR\nOther"
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

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/client.py` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("ecr") as client:
         client: ECRClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import ImageTagMutabilityType, ScanTypeType
 from .paginator import (
     DescribeImageScanFindingsPaginator,
     DescribeImagesPaginator,
     DescribePullThroughCacheRulesPaginator,
@@ -31,14 +30,15 @@
     ListImagesPaginator,
 )
 from .type_defs import (
     BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleResponseTypeDef,
     DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyResponseTypeDef,
@@ -68,16 +68,16 @@
     PutImageResponseTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
-    RegistryScanningRuleTypeDef,
-    ReplicationConfigurationTypeDef,
+    RegistryScanningRuleUnionTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     StartImageScanResponseTypeDef,
     StartLifecyclePolicyPreviewResponseTypeDef,
     TagTypeDef,
     UploadLayerPartResponseTypeDef,
 )
 from .waiter import ImageScanCompleteWaiter, LifecyclePolicyPreviewCompleteWaiter
@@ -576,25 +576,28 @@
         Creates or updates the permissions policy for your registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_registry_policy)
         """
 
     async def put_registry_scanning_configuration(
-        self, *, scanType: ScanTypeType = ..., rules: Sequence[RegistryScanningRuleTypeDef] = ...
+        self,
+        *,
+        scanType: ScanTypeType = ...,
+        rules: Sequence[RegistryScanningRuleUnionTypeDef] = ...
     ) -> PutRegistryScanningConfigurationResponseTypeDef:
         """
         Creates or updates the scanning configuration for your private registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_scanning_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_registry_scanning_configuration)
         """
 
     async def put_replication_configuration(
-        self, *, replicationConfiguration: ReplicationConfigurationTypeDef
+        self, *, replicationConfiguration: ReplicationConfigurationUnionTypeDef
     ) -> PutReplicationConfigurationResponseTypeDef:
         """
         Creates or updates the replication configuration for a registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_replication_configuration)
         """
@@ -649,15 +652,15 @@
     async def upload_layer_part(
         self,
         *,
         repositoryName: str,
         uploadId: str,
         partFirstByte: int,
         partLastByte: int,
-        layerPartBlob: Union[str, bytes, IO[Any], StreamingBody],
+        layerPartBlob: BlobTypeDef,
         registryId: str = ...
     ) -> UploadLayerPartResponseTypeDef:
         """
         Uploads an image layer part to Amazon ECR.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.upload_layer_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#upload_layer_part)
```

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/client.pyi` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("ecr") as client:
         client: ECRClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import ImageTagMutabilityType, ScanTypeType
 from .paginator import (
     DescribeImageScanFindingsPaginator,
     DescribeImagesPaginator,
     DescribePullThroughCacheRulesPaginator,
@@ -31,14 +30,15 @@
     ListImagesPaginator,
 )
 from .type_defs import (
     BatchCheckLayerAvailabilityResponseTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleResponseTypeDef,
     DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyResponseTypeDef,
@@ -68,16 +68,16 @@
     PutImageResponseTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
     PutReplicationConfigurationResponseTypeDef,
-    RegistryScanningRuleTypeDef,
-    ReplicationConfigurationTypeDef,
+    RegistryScanningRuleUnionTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     SetRepositoryPolicyResponseTypeDef,
     StartImageScanResponseTypeDef,
     StartLifecyclePolicyPreviewResponseTypeDef,
     TagTypeDef,
     UploadLayerPartResponseTypeDef,
 )
 from .waiter import ImageScanCompleteWaiter, LifecyclePolicyPreviewCompleteWaiter
@@ -535,24 +535,27 @@
         """
         Creates or updates the permissions policy for your registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_registry_policy)
         """
     async def put_registry_scanning_configuration(
-        self, *, scanType: ScanTypeType = ..., rules: Sequence[RegistryScanningRuleTypeDef] = ...
+        self,
+        *,
+        scanType: ScanTypeType = ...,
+        rules: Sequence[RegistryScanningRuleUnionTypeDef] = ...
     ) -> PutRegistryScanningConfigurationResponseTypeDef:
         """
         Creates or updates the scanning configuration for your private registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_registry_scanning_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_registry_scanning_configuration)
         """
     async def put_replication_configuration(
-        self, *, replicationConfiguration: ReplicationConfigurationTypeDef
+        self, *, replicationConfiguration: ReplicationConfigurationUnionTypeDef
     ) -> PutReplicationConfigurationResponseTypeDef:
         """
         Creates or updates the replication configuration for a registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_replication_configuration)
         """
@@ -601,15 +604,15 @@
     async def upload_layer_part(
         self,
         *,
         repositoryName: str,
         uploadId: str,
         partFirstByte: int,
         partLastByte: int,
-        layerPartBlob: Union[str, bytes, IO[Any], StreamingBody],
+        layerPartBlob: BlobTypeDef,
         registryId: str = ...
     ) -> UploadLayerPartResponseTypeDef:
         """
         Uploads an image layer part to Amazon ECR.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.upload_layer_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#upload_layer_part)
```

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/literals.py` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/literals.pyi` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/paginator.py` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         imageId: ImageIdentifierTypeDef,
         registryId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeImageScanFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImageScanFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describeimagescanfindingspaginator)
         """
 
 
@@ -98,15 +98,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: DescribeImagesFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describeimagespaginator)
         """
 
 
@@ -117,15 +117,15 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         ecrRepositoryPrefixes: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribePullThroughCacheRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribePullThroughCacheRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describepullthroughcacherulespaginator)
         """
 
 
@@ -136,15 +136,15 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describerepositoriespaginator)
         """
 
 
@@ -157,15 +157,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: LifecyclePolicyPreviewFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetLifecyclePolicyPreviewResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.GetLifecyclePolicyPreview.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#getlifecyclepolicypreviewpaginator)
         """
 
 
@@ -177,13 +177,13 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         filter: ListImagesFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.ListImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#listimagespaginator)
         """
```

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/paginator.pyi` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         imageId: ImageIdentifierTypeDef,
         registryId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeImageScanFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImageScanFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describeimagescanfindingspaginator)
         """
 
 class DescribeImagesPaginator(AioPaginator):
@@ -94,15 +94,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: DescribeImagesFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describeimagespaginator)
         """
 
 class DescribePullThroughCacheRulesPaginator(AioPaginator):
@@ -112,15 +112,15 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         ecrRepositoryPrefixes: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribePullThroughCacheRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribePullThroughCacheRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describepullthroughcacherulespaginator)
         """
 
 class DescribeRepositoriesPaginator(AioPaginator):
@@ -130,15 +130,15 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describerepositoriespaginator)
         """
 
 class GetLifecyclePolicyPreviewPaginator(AioPaginator):
@@ -150,15 +150,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: LifecyclePolicyPreviewFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetLifecyclePolicyPreviewResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.GetLifecyclePolicyPreview.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#getlifecyclepolicypreviewpaginator)
         """
 
 class ListImagesPaginator(AioPaginator):
@@ -169,13 +169,13 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         filter: ListImagesFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.ListImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#listimagespaginator)
         """
```

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/type_defs.py` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ecr.type_defs import AttributeTypeDef
 
-    data: AttributeTypeDef = {...}
+    data: AttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -37,146 +37,151 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttributeTypeDef",
     "AuthorizationDataTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
+    "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
     "BatchGetRepositoryScanningConfigurationRequestRequestTypeDef",
     "RepositoryScanningConfigurationFailureTypeDef",
+    "BlobTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
-    "CompleteLayerUploadResponseTypeDef",
     "CreatePullThroughCacheRuleRequestRequestTypeDef",
-    "CreatePullThroughCacheRuleResponseTypeDef",
     "EncryptionConfigurationTypeDef",
     "ImageScanningConfigurationTypeDef",
     "TagTypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DeleteLifecyclePolicyRequestRequestTypeDef",
-    "DeleteLifecyclePolicyResponseTypeDef",
     "DeletePullThroughCacheRuleRequestRequestTypeDef",
-    "DeletePullThroughCacheRuleResponseTypeDef",
-    "DeleteRegistryPolicyResponseTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
-    "DeleteRepositoryPolicyResponseTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
     "ImageReplicationStatusTypeDef",
+    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "ImageScanStatusTypeDef",
     "DescribeImagesFilterTypeDef",
-    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     "PullThroughCacheRuleTypeDef",
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
     "GetDownloadUrlForLayerRequestRequestTypeDef",
-    "GetDownloadUrlForLayerResponseTypeDef",
     "LifecyclePolicyPreviewFilterTypeDef",
     "LifecyclePolicyPreviewSummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
-    "GetLifecyclePolicyResponseTypeDef",
-    "GetRegistryPolicyResponseTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
-    "GetRepositoryPolicyResponseTypeDef",
     "ImageScanFindingsSummaryTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
-    "InitiateLayerUploadResponseTypeDef",
     "LifecyclePolicyRuleActionTypeDef",
     "ListImagesFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "VulnerablePackageTypeDef",
-    "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutImageTagMutabilityRequestRequestTypeDef",
-    "PutImageTagMutabilityResponseTypeDef",
     "PutLifecyclePolicyRequestRequestTypeDef",
-    "PutLifecyclePolicyResponseTypeDef",
     "PutRegistryPolicyRequestRequestTypeDef",
-    "PutRegistryPolicyResponseTypeDef",
     "RecommendationTypeDef",
     "ScanningRepositoryFilterTypeDef",
     "ReplicationDestinationTypeDef",
     "RepositoryFilterTypeDef",
-    "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
-    "SetRepositoryPolicyResponseTypeDef",
     "StartLifecyclePolicyPreviewRequestRequestTypeDef",
-    "StartLifecyclePolicyPreviewResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UploadLayerPartRequestRequestTypeDef",
-    "UploadLayerPartResponseTypeDef",
     "ImageScanFindingTypeDef",
-    "GetAuthorizationTokenResponseTypeDef",
     "ResourceDetailsTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
+    "CompleteLayerUploadResponseTypeDef",
+    "CreatePullThroughCacheRuleResponseTypeDef",
+    "DeleteLifecyclePolicyResponseTypeDef",
+    "DeletePullThroughCacheRuleResponseTypeDef",
+    "DeleteRegistryPolicyResponseTypeDef",
+    "DeleteRepositoryPolicyResponseTypeDef",
+    "GetAuthorizationTokenResponseTypeDef",
+    "GetDownloadUrlForLayerResponseTypeDef",
+    "GetLifecyclePolicyResponseTypeDef",
+    "GetRegistryPolicyResponseTypeDef",
+    "GetRepositoryPolicyResponseTypeDef",
+    "InitiateLayerUploadResponseTypeDef",
+    "PutImageTagMutabilityResponseTypeDef",
+    "PutLifecyclePolicyResponseTypeDef",
+    "PutRegistryPolicyResponseTypeDef",
+    "SetRepositoryPolicyResponseTypeDef",
+    "StartLifecyclePolicyPreviewResponseTypeDef",
+    "UploadLayerPartResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
     "BatchGetImageRequestRequestTypeDef",
     "DescribeImageReplicationStatusRequestRequestTypeDef",
-    "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
     "DescribeImageScanFindingsRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "ListImagesResponseTypeDef",
     "StartImageScanRequestRequestTypeDef",
+    "UploadLayerPartRequestRequestTypeDef",
     "PutImageScanningConfigurationRequestRequestTypeDef",
     "PutImageScanningConfigurationResponseTypeDef",
     "RepositoryTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CvssScoreDetailsTypeDef",
     "DescribeImageReplicationStatusResponseTypeDef",
+    "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     "StartImageScanResponseTypeDef",
     "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "DescribePullThroughCacheRulesResponseTypeDef",
     "GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     "GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
     "GetLifecyclePolicyPreviewRequestRequestTypeDef",
     "ImageDetailTypeDef",
     "LifecyclePolicyPreviewResultTypeDef",
     "ListImagesRequestListImagesPaginateTypeDef",
     "ListImagesRequestRequestTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
+    "RegistryScanningRuleOutputTypeDef",
     "RegistryScanningRuleTypeDef",
     "RepositoryScanningConfigurationTypeDef",
+    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "ResourceTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "BatchGetImageResponseTypeDef",
     "PutImageResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
     "ScoreDetailsTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetLifecyclePolicyPreviewResponseTypeDef",
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
     "RegistryScanningConfigurationTypeDef",
+    "RegistryScanningRuleUnionTypeDef",
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
+    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "EnhancedImageScanFindingTypeDef",
     "GetRegistryScanningConfigurationResponseTypeDef",
     "PutRegistryScanningConfigurationResponseTypeDef",
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
     "DescribeRegistryResponseTypeDef",
-    "PutReplicationConfigurationRequestRequestTypeDef",
     "PutReplicationConfigurationResponseTypeDef",
+    "PutReplicationConfigurationRequestRequestTypeDef",
+    "ReplicationConfigurationUnionTypeDef",
     "ImageScanFindingsTypeDef",
     "DescribeImageScanFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
@@ -187,19 +192,17 @@
     "_OptionalAttributeTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
-
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
-
 AuthorizationDataTypeDef = TypedDict(
     "AuthorizationDataTypeDef",
     {
         "authorizationToken": str,
         "expiresAt": datetime,
         "proxyEndpoint": str,
     },
@@ -232,22 +235,20 @@
     "_OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class BatchCheckLayerAvailabilityRequestRequestTypeDef(
     _RequiredBatchCheckLayerAvailabilityRequestRequestTypeDef,
     _OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef,
 ):
     pass
 
-
 LayerFailureTypeDef = TypedDict(
     "LayerFailureTypeDef",
     {
         "layerDigest": str,
         "failureCode": LayerFailureCodeType,
         "failureReason": str,
     },
@@ -261,14 +262,25 @@
         "layerAvailability": LayerAvailabilityType,
         "layerSize": int,
         "mediaType": str,
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
 ImageIdentifierTypeDef = TypedDict(
     "ImageIdentifierTypeDef",
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
@@ -287,14 +299,15 @@
         "repositoryName": str,
         "failureCode": Literal["REPOSITORY_NOT_FOUND"],
         "failureReason": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCompleteLayerUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCompleteLayerUploadRequestRequestTypeDef",
     {
         "repositoryName": str,
         "uploadId": str,
         "layerDigests": Sequence[str],
     },
@@ -303,33 +316,20 @@
     "_OptionalCompleteLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-
-CompleteLayerUploadResponseTypeDef = TypedDict(
-    "CompleteLayerUploadResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "layerDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePullThroughCacheRuleRequestRequestTypeDef",
     {
         "ecrRepositoryPrefix": str,
         "upstreamRegistryUrl": str,
     },
 )
@@ -337,54 +337,39 @@
     "_OptionalCreatePullThroughCacheRuleRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class CreatePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalCreatePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
-
-CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
-    "CreatePullThroughCacheRuleResponseTypeDef",
-    {
-        "ecrRepositoryPrefix": str,
-        "upstreamRegistryUrl": str,
-        "createdAt": datetime,
-        "registryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEncryptionConfigurationTypeDef = TypedDict(
     "_RequiredEncryptionConfigurationTypeDef",
     {
         "encryptionType": EncryptionTypeType,
     },
 )
 _OptionalEncryptionConfigurationTypeDef = TypedDict(
     "_OptionalEncryptionConfigurationTypeDef",
     {
         "kmsKey": str,
     },
     total=False,
 )
 
-
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
-
 ImageScanningConfigurationTypeDef = TypedDict(
     "ImageScanningConfigurationTypeDef",
     {
         "scanOnPush": bool,
     },
     total=False,
 )
@@ -428,107 +413,60 @@
     "_OptionalDeleteLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DeleteLifecyclePolicyRequestRequestTypeDef(
     _RequiredDeleteLifecyclePolicyRequestRequestTypeDef,
     _OptionalDeleteLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-
-DeleteLifecyclePolicyResponseTypeDef = TypedDict(
-    "DeleteLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "lastEvaluatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePullThroughCacheRuleRequestRequestTypeDef",
     {
         "ecrRepositoryPrefix": str,
     },
 )
 _OptionalDeletePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_OptionalDeletePullThroughCacheRuleRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DeletePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalDeletePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
-
-DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
-    "DeletePullThroughCacheRuleResponseTypeDef",
-    {
-        "ecrRepositoryPrefix": str,
-        "upstreamRegistryUrl": str,
-        "createdAt": datetime,
-        "registryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteRegistryPolicyResponseTypeDef = TypedDict(
-    "DeleteRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-DeleteRepositoryPolicyResponseTypeDef = TypedDict(
-    "DeleteRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDeleteRepositoryRequestRequestTypeDef = TypedDict(
@@ -536,32 +474,40 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
-
 ImageReplicationStatusTypeDef = TypedDict(
     "ImageReplicationStatusTypeDef",
     {
         "region": str,
         "registryId": str,
         "status": ReplicationStatusType,
         "failureCode": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -580,24 +526,14 @@
     "DescribeImagesFilterTypeDef",
     {
         "tagStatus": TagStatusType,
     },
     total=False,
 )
 
-DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = TypedDict(
-    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
-    {
-        "registryId": str,
-        "ecrRepositoryPrefixes": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribePullThroughCacheRulesRequestRequestTypeDef = TypedDict(
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     {
         "registryId": str,
         "ecrRepositoryPrefixes": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -612,24 +548,14 @@
         "upstreamRegistryUrl": str,
         "createdAt": datetime,
         "registryId": str,
     },
     total=False,
 )
 
-DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
-    {
-        "registryId": str,
-        "repositoryNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRepositoriesRequestRequestTypeDef = TypedDict(
     "DescribeRepositoriesRequestRequestTypeDef",
     {
         "registryId": str,
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -656,31 +582,20 @@
     "_OptionalGetDownloadUrlForLayerRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetDownloadUrlForLayerRequestRequestTypeDef(
     _RequiredGetDownloadUrlForLayerRequestRequestTypeDef,
     _OptionalGetDownloadUrlForLayerRequestRequestTypeDef,
 ):
     pass
 
-
-GetDownloadUrlForLayerResponseTypeDef = TypedDict(
-    "GetDownloadUrlForLayerResponseTypeDef",
-    {
-        "downloadUrl": str,
-        "layerDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifecyclePolicyPreviewFilterTypeDef = TypedDict(
     "LifecyclePolicyPreviewFilterTypeDef",
     {
         "tagStatus": TagStatusType,
     },
     total=False,
 )
@@ -703,74 +618,40 @@
     "_OptionalGetLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetLifecyclePolicyRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-
-GetLifecyclePolicyResponseTypeDef = TypedDict(
-    "GetLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "lastEvaluatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetRegistryPolicyResponseTypeDef = TypedDict(
-    "GetRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalGetRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-GetRepositoryPolicyResponseTypeDef = TypedDict(
-    "GetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImageScanFindingsSummaryTypeDef = TypedDict(
     "ImageScanFindingsSummaryTypeDef",
     {
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
     },
@@ -787,31 +668,20 @@
     "_OptionalInitiateLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-
-InitiateLayerUploadResponseTypeDef = TypedDict(
-    "InitiateLayerUploadResponseTypeDef",
-    {
-        "uploadId": str,
-        "partSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifecyclePolicyRuleActionTypeDef = TypedDict(
     "LifecyclePolicyRuleActionTypeDef",
     {
         "type": Literal["EXPIRE"],
     },
     total=False,
 )
@@ -842,24 +712,14 @@
         "release": str,
         "sourceLayerHash": str,
         "version": str,
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
 _RequiredPutImageRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageManifest": str,
     },
 )
@@ -870,21 +730,19 @@
         "imageManifestMediaType": str,
         "imageTag": str,
         "imageDigest": str,
     },
     total=False,
 )
 
-
 class PutImageRequestRequestTypeDef(
     _RequiredPutImageRequestRequestTypeDef, _OptionalPutImageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutImageTagMutabilityRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageTagMutabilityRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageTagMutability": ImageTagMutabilityType,
     },
 )
@@ -892,32 +750,20 @@
     "_OptionalPutImageTagMutabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class PutImageTagMutabilityRequestRequestTypeDef(
     _RequiredPutImageTagMutabilityRequestRequestTypeDef,
     _OptionalPutImageTagMutabilityRequestRequestTypeDef,
 ):
     pass
 
-
-PutImageTagMutabilityResponseTypeDef = TypedDict(
-    "PutImageTagMutabilityResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "imageTagMutability": ImageTagMutabilityType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutLifecyclePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutLifecyclePolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "lifecyclePolicyText": str,
     },
 )
@@ -925,48 +771,27 @@
     "_OptionalPutLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class PutLifecyclePolicyRequestRequestTypeDef(
     _RequiredPutLifecyclePolicyRequestRequestTypeDef,
     _OptionalPutLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-
-PutLifecyclePolicyResponseTypeDef = TypedDict(
-    "PutLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutRegistryPolicyRequestRequestTypeDef = TypedDict(
     "PutRegistryPolicyRequestRequestTypeDef",
     {
         "policyText": str,
     },
 )
 
-PutRegistryPolicyResponseTypeDef = TypedDict(
-    "PutRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "url": str,
         "text": str,
     },
     total=False,
@@ -992,25 +817,14 @@
     "RepositoryFilterTypeDef",
     {
         "filter": str,
         "filterType": Literal["PREFIX_MATCH"],
     },
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
 _RequiredSetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "policyText": str,
     },
 )
@@ -1019,32 +833,20 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
-
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-
-SetRepositoryPolicyResponseTypeDef = TypedDict(
-    "SetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalStartLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
@@ -1052,111 +854,234 @@
     {
         "registryId": str,
         "lifecyclePolicyText": str,
     },
     total=False,
 )
 
-
 class StartLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalStartLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
 
-StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
-    "StartLifecyclePolicyPreviewResponseTypeDef",
+ImageScanFindingTypeDef = TypedDict(
+    "ImageScanFindingTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "uri": str,
+        "severity": FindingSeverityType,
+        "attributes": List[AttributeTypeDef],
+    },
+    total=False,
+)
+
+ResourceDetailsTypeDef = TypedDict(
+    "ResourceDetailsTypeDef",
+    {
+        "awsEcrContainerImage": AwsEcrContainerImageDetailsTypeDef,
+    },
+    total=False,
+)
+
+BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
+    "BatchCheckLayerAvailabilityResponseTypeDef",
+    {
+        "layers": List[LayerTypeDef],
+        "failures": List[LayerFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CompleteLayerUploadResponseTypeDef = TypedDict(
+    "CompleteLayerUploadResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "status": LifecyclePolicyPreviewStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "uploadId": str,
+        "layerDigest": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
+    "CreatePullThroughCacheRuleResponseTypeDef",
     {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "ecrRepositoryPrefix": str,
+        "upstreamRegistryUrl": str,
+        "createdAt": datetime,
+        "registryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
-    "_RequiredUploadLayerPartRequestRequestTypeDef",
+DeleteLifecyclePolicyResponseTypeDef = TypedDict(
+    "DeleteLifecyclePolicyResponseTypeDef",
     {
+        "registryId": str,
         "repositoryName": str,
-        "uploadId": str,
-        "partFirstByte": int,
-        "partLastByte": int,
-        "layerPartBlob": Union[str, bytes, IO[Any], StreamingBody],
+        "lifecyclePolicyText": str,
+        "lastEvaluatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
-    "_OptionalUploadLayerPartRequestRequestTypeDef",
+
+DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
+    "DeletePullThroughCacheRuleResponseTypeDef",
     {
+        "ecrRepositoryPrefix": str,
+        "upstreamRegistryUrl": str,
+        "createdAt": datetime,
         "registryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+DeleteRegistryPolicyResponseTypeDef = TypedDict(
+    "DeleteRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UploadLayerPartRequestRequestTypeDef(
-    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
-):
-    pass
+DeleteRepositoryPolicyResponseTypeDef = TypedDict(
+    "DeleteRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetAuthorizationTokenResponseTypeDef = TypedDict(
+    "GetAuthorizationTokenResponseTypeDef",
+    {
+        "authorizationData": List[AuthorizationDataTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UploadLayerPartResponseTypeDef = TypedDict(
-    "UploadLayerPartResponseTypeDef",
+GetDownloadUrlForLayerResponseTypeDef = TypedDict(
+    "GetDownloadUrlForLayerResponseTypeDef",
+    {
+        "downloadUrl": str,
+        "layerDigest": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLifecyclePolicyResponseTypeDef = TypedDict(
+    "GetLifecyclePolicyResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "lastEvaluatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRegistryPolicyResponseTypeDef = TypedDict(
+    "GetRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRepositoryPolicyResponseTypeDef = TypedDict(
+    "GetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateLayerUploadResponseTypeDef = TypedDict(
+    "InitiateLayerUploadResponseTypeDef",
+    {
         "uploadId": str,
-        "lastByteReceived": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "partSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImageScanFindingTypeDef = TypedDict(
-    "ImageScanFindingTypeDef",
+PutImageTagMutabilityResponseTypeDef = TypedDict(
+    "PutImageTagMutabilityResponseTypeDef",
     {
-        "name": str,
-        "description": str,
-        "uri": str,
-        "severity": FindingSeverityType,
-        "attributes": List[AttributeTypeDef],
+        "registryId": str,
+        "repositoryName": str,
+        "imageTagMutability": ImageTagMutabilityType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-GetAuthorizationTokenResponseTypeDef = TypedDict(
-    "GetAuthorizationTokenResponseTypeDef",
+PutLifecyclePolicyResponseTypeDef = TypedDict(
+    "PutLifecyclePolicyResponseTypeDef",
     {
-        "authorizationData": List[AuthorizationDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResourceDetailsTypeDef = TypedDict(
-    "ResourceDetailsTypeDef",
+PutRegistryPolicyResponseTypeDef = TypedDict(
+    "PutRegistryPolicyResponseTypeDef",
     {
-        "awsEcrContainerImage": AwsEcrContainerImageDetailsTypeDef,
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
-    "BatchCheckLayerAvailabilityResponseTypeDef",
+SetRepositoryPolicyResponseTypeDef = TypedDict(
+    "SetRepositoryPolicyResponseTypeDef",
     {
-        "layers": List[LayerTypeDef],
-        "failures": List[LayerFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
+    "StartLifecyclePolicyPreviewResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "status": LifecyclePolicyPreviewStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadLayerPartResponseTypeDef = TypedDict(
+    "UploadLayerPartResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "lastByteReceived": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteImageRequestRequestTypeDef",
     {
         "repositoryName": str,
@@ -1167,21 +1092,19 @@
     "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class BatchDeleteImageRequestRequestTypeDef(
     _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredBatchGetImageRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
@@ -1190,21 +1113,19 @@
     {
         "registryId": str,
         "acceptedMediaTypes": Sequence[str],
     },
     total=False,
 )
 
-
 class BatchGetImageRequestRequestTypeDef(
     _RequiredBatchGetImageRequestRequestTypeDef, _OptionalBatchGetImageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeImageReplicationStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageReplicationStatusRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1212,46 +1133,20 @@
     "_OptionalDescribeImageReplicationStatusRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class DescribeImageReplicationStatusRequestRequestTypeDef(
     _RequiredDescribeImageReplicationStatusRequestRequestTypeDef,
     _OptionalDescribeImageReplicationStatusRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
-    },
-)
-_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    {
-        "registryId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
-    _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-    _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeImageScanFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1261,22 +1156,20 @@
         "registryId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class DescribeImageScanFindingsRequestRequestTypeDef(
     _RequiredDescribeImageScanFindingsRequestRequestTypeDef,
     _OptionalDescribeImageScanFindingsRequestRequestTypeDef,
 ):
     pass
 
-
 ImageFailureTypeDef = TypedDict(
     "ImageFailureTypeDef",
     {
         "imageId": ImageIdentifierTypeDef,
         "failureCode": ImageFailureCodeType,
         "failureReason": str,
     },
@@ -1296,15 +1189,15 @@
 )
 
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
         "imageIds": List[ImageIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartImageScanRequestRequestTypeDef = TypedDict(
     "_RequiredStartImageScanRequestRequestTypeDef",
     {
         "repositoryName": str,
@@ -1315,20 +1208,41 @@
     "_OptionalStartImageScanRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class StartImageScanRequestRequestTypeDef(
     _RequiredStartImageScanRequestRequestTypeDef, _OptionalStartImageScanRequestRequestTypeDef
 ):
     pass
 
+_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_RequiredUploadLayerPartRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+        "uploadId": str,
+        "partFirstByte": int,
+        "partLastByte": int,
+        "layerPartBlob": BlobTypeDef,
+    },
+)
+_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_OptionalUploadLayerPartRequestRequestTypeDef",
+    {
+        "registryId": str,
+    },
+    total=False,
+)
+
+class UploadLayerPartRequestRequestTypeDef(
+    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
+):
+    pass
 
 _RequiredPutImageScanningConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
     },
@@ -1337,29 +1251,27 @@
     "_OptionalPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
-
 class PutImageScanningConfigurationRequestRequestTypeDef(
     _RequiredPutImageScanningConfigurationRequestRequestTypeDef,
     _OptionalPutImageScanningConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 PutImageScanningConfigurationResponseTypeDef = TypedDict(
     "PutImageScanningConfigurationResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RepositoryTypeDef = TypedDict(
     "RepositoryTypeDef",
     {
         "repositoryArn": str,
@@ -1388,26 +1300,24 @@
         "imageTagMutability": ImageTagMutabilityType,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
         "encryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1429,16 +1339,58 @@
 
 DescribeImageReplicationStatusResponseTypeDef = TypedDict(
     "DescribeImageReplicationStatusResponseTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
         "replicationStatuses": List[ImageReplicationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "imageId": ImageIdentifierTypeDef,
+    },
+)
+_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    {
+        "registryId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
+    _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+    _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+):
+    pass
+
+DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = TypedDict(
+    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
+    {
+        "registryId": str,
+        "ecrRepositoryPrefixes": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
+    {
+        "registryId": str,
+        "repositoryNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
@@ -1451,30 +1403,28 @@
         "nextToken": str,
         "maxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef(
     _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     _OptionalDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
 ):
     pass
 
-
 StartImageScanResponseTypeDef = TypedDict(
     "StartImageScanResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "repositoryName": str,
@@ -1482,27 +1432,25 @@
 )
 _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": DescribeImagesFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeImagesRequestDescribeImagesPaginateTypeDef(
     _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
     _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImagesRequestRequestTypeDef = TypedDict(
@@ -1513,27 +1461,25 @@
         "nextToken": str,
         "maxResults": int,
         "filter": DescribeImagesFilterTypeDef,
     },
     total=False,
 )
 
-
 class DescribeImagesRequestRequestTypeDef(
     _RequiredDescribeImagesRequestRequestTypeDef, _OptionalDescribeImagesRequestRequestTypeDef
 ):
     pass
 
-
 DescribePullThroughCacheRulesResponseTypeDef = TypedDict(
     "DescribePullThroughCacheRulesResponseTypeDef",
     {
         "pullThroughCacheRules": List[PullThroughCacheRuleTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     {
         "repositoryName": str,
@@ -1541,27 +1487,25 @@
 )
 _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = TypedDict(
     "_OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     {
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": LifecyclePolicyPreviewFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef = TypedDict(
@@ -1573,22 +1517,20 @@
         "maxResults": int,
         "filter": LifecyclePolicyPreviewFilterTypeDef,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
@@ -1599,22 +1541,20 @@
         "nextToken": str,
         "maxResults": int,
         "filter": LifecyclePolicyPreviewFilterTypeDef,
     },
     total=False,
 )
 
-
 class GetLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
-
 ImageDetailTypeDef = TypedDict(
     "ImageDetailTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageDigest": str,
         "imageTags": List[str],
@@ -1648,27 +1588,25 @@
     },
 )
 _OptionalListImagesRequestListImagesPaginateTypeDef = TypedDict(
     "_OptionalListImagesRequestListImagesPaginateTypeDef",
     {
         "registryId": str,
         "filter": ListImagesFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListImagesRequestListImagesPaginateTypeDef(
     _RequiredListImagesRequestListImagesPaginateTypeDef,
     _OptionalListImagesRequestListImagesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListImagesRequestRequestTypeDef = TypedDict(
     "_RequiredListImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListImagesRequestRequestTypeDef = TypedDict(
@@ -1678,21 +1616,19 @@
         "nextToken": str,
         "maxResults": int,
         "filter": ListImagesFilterTypeDef,
     },
     total=False,
 )
 
-
 class ListImagesRequestRequestTypeDef(
     _RequiredListImagesRequestRequestTypeDef, _OptionalListImagesRequestRequestTypeDef
 ):
     pass
 
-
 PackageVulnerabilityDetailsTypeDef = TypedDict(
     "PackageVulnerabilityDetailsTypeDef",
     {
         "cvss": List[CvssScoreTypeDef],
         "referenceUrls": List[str],
         "relatedVulnerabilities": List[str],
         "source": str,
@@ -1710,19 +1646,27 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
+RegistryScanningRuleOutputTypeDef = TypedDict(
+    "RegistryScanningRuleOutputTypeDef",
+    {
+        "scanFrequency": ScanFrequencyType,
+        "repositoryFilters": List[ScanningRepositoryFilterTypeDef],
+    },
+)
+
 RegistryScanningRuleTypeDef = TypedDict(
     "RegistryScanningRuleTypeDef",
     {
         "scanFrequency": ScanFrequencyType,
-        "repositoryFilters": List[ScanningRepositoryFilterTypeDef],
+        "repositoryFilters": Sequence[ScanningRepositoryFilterTypeDef],
     },
 )
 
 RepositoryScanningConfigurationTypeDef = TypedDict(
     "RepositoryScanningConfigurationTypeDef",
     {
         "repositoryArn": str,
@@ -1730,33 +1674,50 @@
         "scanOnPush": bool,
         "scanFrequency": ScanFrequencyType,
         "appliedScanFilters": List[ScanningRepositoryFilterTypeDef],
     },
     total=False,
 )
 
+_RequiredReplicationRuleOutputTypeDef = TypedDict(
+    "_RequiredReplicationRuleOutputTypeDef",
+    {
+        "destinations": List[ReplicationDestinationTypeDef],
+    },
+)
+_OptionalReplicationRuleOutputTypeDef = TypedDict(
+    "_OptionalReplicationRuleOutputTypeDef",
+    {
+        "repositoryFilters": List[RepositoryFilterTypeDef],
+    },
+    total=False,
+)
+
+class ReplicationRuleOutputTypeDef(
+    _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
+):
+    pass
+
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
-        "destinations": List[ReplicationDestinationTypeDef],
+        "destinations": Sequence[ReplicationDestinationTypeDef],
     },
 )
 _OptionalReplicationRuleTypeDef = TypedDict(
     "_OptionalReplicationRuleTypeDef",
     {
-        "repositoryFilters": List[RepositoryFilterTypeDef],
+        "repositoryFilters": Sequence[RepositoryFilterTypeDef],
     },
     total=False,
 )
 
-
 class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
     pass
 
-
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "details": ResourceDetailsTypeDef,
         "id": str,
         "tags": Dict[str, str],
         "type": str,
@@ -1765,57 +1726,57 @@
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
         "imageIds": List[ImageIdentifierTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetImageResponseTypeDef = TypedDict(
     "BatchGetImageResponseTypeDef",
     {
         "images": List[ImageTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryResponseTypeDef = TypedDict(
     "DeleteRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoriesResponseTypeDef = TypedDict(
     "DescribeRepositoriesResponseTypeDef",
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScoreDetailsTypeDef = TypedDict(
     "ScoreDetailsTypeDef",
     {
         "cvss": CvssScoreDetailsTypeDef,
@@ -1824,63 +1785,64 @@
 )
 
 DescribeImagesResponseTypeDef = TypedDict(
     "DescribeImagesResponseTypeDef",
     {
         "imageDetails": List[ImageDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLifecyclePolicyPreviewResponseTypeDef = TypedDict(
     "GetLifecyclePolicyPreviewResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "status": LifecyclePolicyPreviewStatusType,
         "nextToken": str,
         "previewResults": List[LifecyclePolicyPreviewResultTypeDef],
         "summary": LifecyclePolicyPreviewSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
-    {
-        "scanType": ScanTypeType,
-        "rules": Sequence[RegistryScanningRuleTypeDef],
-    },
-    total=False,
-)
-
 RegistryScanningConfigurationTypeDef = TypedDict(
     "RegistryScanningConfigurationTypeDef",
     {
         "scanType": ScanTypeType,
-        "rules": List[RegistryScanningRuleTypeDef],
+        "rules": List[RegistryScanningRuleOutputTypeDef],
     },
     total=False,
 )
 
+RegistryScanningRuleUnionTypeDef = Union[
+    RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef
+]
 BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     {
         "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
         "failures": List[RepositoryScanningConfigurationFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReplicationConfigurationOutputTypeDef = TypedDict(
+    "ReplicationConfigurationOutputTypeDef",
+    {
+        "rules": List[ReplicationRuleOutputTypeDef],
     },
 )
 
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
-        "rules": List[ReplicationRuleTypeDef],
+        "rules": Sequence[ReplicationRuleTypeDef],
     },
 )
 
 EnhancedImageScanFindingTypeDef = TypedDict(
     "EnhancedImageScanFindingTypeDef",
     {
         "awsAccountId": str,
@@ -1903,50 +1865,62 @@
 )
 
 GetRegistryScanningConfigurationResponseTypeDef = TypedDict(
     "GetRegistryScanningConfigurationResponseTypeDef",
     {
         "registryId": str,
         "scanningConfiguration": RegistryScanningConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRegistryScanningConfigurationResponseTypeDef = TypedDict(
     "PutRegistryScanningConfigurationResponseTypeDef",
     {
         "registryScanningConfiguration": RegistryScanningConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    {
+        "scanType": ScanTypeType,
+        "rules": Sequence[RegistryScanningRuleUnionTypeDef],
     },
+    total=False,
 )
 
 DescribeRegistryResponseTypeDef = TypedDict(
     "DescribeRegistryResponseTypeDef",
     {
         "registryId": str,
-        "replicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutReplicationConfigurationRequestRequestTypeDef",
+PutReplicationConfigurationResponseTypeDef = TypedDict(
+    "PutReplicationConfigurationResponseTypeDef",
     {
-        "replicationConfiguration": ReplicationConfigurationTypeDef,
+        "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutReplicationConfigurationResponseTypeDef = TypedDict(
-    "PutReplicationConfigurationResponseTypeDef",
+PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutReplicationConfigurationRequestRequestTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ReplicationConfigurationUnionTypeDef = Union[
+    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
+]
 ImageScanFindingsTypeDef = TypedDict(
     "ImageScanFindingsTypeDef",
     {
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
         "findings": List[ImageScanFindingTypeDef],
@@ -1960,10 +1934,10 @@
     {
         "registryId": str,
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
         "imageScanFindings": ImageScanFindingsTypeDef,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/type_defs.pyi` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/type_defs.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ecr.type_defs import AttributeTypeDef
 
-    data: AttributeTypeDef = {...}
+    data: AttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -37,145 +37,152 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AttributeTypeDef",
     "AuthorizationDataTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
+    "ResponseMetadataTypeDef",
     "ImageIdentifierTypeDef",
     "BatchGetRepositoryScanningConfigurationRequestRequestTypeDef",
     "RepositoryScanningConfigurationFailureTypeDef",
+    "BlobTypeDef",
     "CompleteLayerUploadRequestRequestTypeDef",
-    "CompleteLayerUploadResponseTypeDef",
     "CreatePullThroughCacheRuleRequestRequestTypeDef",
-    "CreatePullThroughCacheRuleResponseTypeDef",
     "EncryptionConfigurationTypeDef",
     "ImageScanningConfigurationTypeDef",
     "TagTypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
     "DeleteLifecyclePolicyRequestRequestTypeDef",
-    "DeleteLifecyclePolicyResponseTypeDef",
     "DeletePullThroughCacheRuleRequestRequestTypeDef",
-    "DeletePullThroughCacheRuleResponseTypeDef",
-    "DeleteRegistryPolicyResponseTypeDef",
     "DeleteRepositoryPolicyRequestRequestTypeDef",
-    "DeleteRepositoryPolicyResponseTypeDef",
     "DeleteRepositoryRequestRequestTypeDef",
     "ImageReplicationStatusTypeDef",
+    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
     "ImageScanStatusTypeDef",
     "DescribeImagesFilterTypeDef",
-    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     "PullThroughCacheRuleTypeDef",
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeRepositoriesRequestRequestTypeDef",
     "GetAuthorizationTokenRequestRequestTypeDef",
     "GetDownloadUrlForLayerRequestRequestTypeDef",
-    "GetDownloadUrlForLayerResponseTypeDef",
     "LifecyclePolicyPreviewFilterTypeDef",
     "LifecyclePolicyPreviewSummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
-    "GetLifecyclePolicyResponseTypeDef",
-    "GetRegistryPolicyResponseTypeDef",
     "GetRepositoryPolicyRequestRequestTypeDef",
-    "GetRepositoryPolicyResponseTypeDef",
     "ImageScanFindingsSummaryTypeDef",
     "InitiateLayerUploadRequestRequestTypeDef",
-    "InitiateLayerUploadResponseTypeDef",
     "LifecyclePolicyRuleActionTypeDef",
     "ListImagesFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "VulnerablePackageTypeDef",
-    "PaginatorConfigTypeDef",
     "PutImageRequestRequestTypeDef",
     "PutImageTagMutabilityRequestRequestTypeDef",
-    "PutImageTagMutabilityResponseTypeDef",
     "PutLifecyclePolicyRequestRequestTypeDef",
-    "PutLifecyclePolicyResponseTypeDef",
     "PutRegistryPolicyRequestRequestTypeDef",
-    "PutRegistryPolicyResponseTypeDef",
     "RecommendationTypeDef",
     "ScanningRepositoryFilterTypeDef",
     "ReplicationDestinationTypeDef",
     "RepositoryFilterTypeDef",
-    "ResponseMetadataTypeDef",
     "SetRepositoryPolicyRequestRequestTypeDef",
-    "SetRepositoryPolicyResponseTypeDef",
     "StartLifecyclePolicyPreviewRequestRequestTypeDef",
-    "StartLifecyclePolicyPreviewResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UploadLayerPartRequestRequestTypeDef",
-    "UploadLayerPartResponseTypeDef",
     "ImageScanFindingTypeDef",
-    "GetAuthorizationTokenResponseTypeDef",
     "ResourceDetailsTypeDef",
     "BatchCheckLayerAvailabilityResponseTypeDef",
+    "CompleteLayerUploadResponseTypeDef",
+    "CreatePullThroughCacheRuleResponseTypeDef",
+    "DeleteLifecyclePolicyResponseTypeDef",
+    "DeletePullThroughCacheRuleResponseTypeDef",
+    "DeleteRegistryPolicyResponseTypeDef",
+    "DeleteRepositoryPolicyResponseTypeDef",
+    "GetAuthorizationTokenResponseTypeDef",
+    "GetDownloadUrlForLayerResponseTypeDef",
+    "GetLifecyclePolicyResponseTypeDef",
+    "GetRegistryPolicyResponseTypeDef",
+    "GetRepositoryPolicyResponseTypeDef",
+    "InitiateLayerUploadResponseTypeDef",
+    "PutImageTagMutabilityResponseTypeDef",
+    "PutLifecyclePolicyResponseTypeDef",
+    "PutRegistryPolicyResponseTypeDef",
+    "SetRepositoryPolicyResponseTypeDef",
+    "StartLifecyclePolicyPreviewResponseTypeDef",
+    "UploadLayerPartResponseTypeDef",
     "BatchDeleteImageRequestRequestTypeDef",
     "BatchGetImageRequestRequestTypeDef",
     "DescribeImageReplicationStatusRequestRequestTypeDef",
-    "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
     "DescribeImageScanFindingsRequestRequestTypeDef",
     "ImageFailureTypeDef",
     "ImageTypeDef",
     "ListImagesResponseTypeDef",
     "StartImageScanRequestRequestTypeDef",
+    "UploadLayerPartRequestRequestTypeDef",
     "PutImageScanningConfigurationRequestRequestTypeDef",
     "PutImageScanningConfigurationResponseTypeDef",
     "RepositoryTypeDef",
     "CreateRepositoryRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CvssScoreDetailsTypeDef",
     "DescribeImageReplicationStatusResponseTypeDef",
+    "DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
     "DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     "StartImageScanResponseTypeDef",
     "DescribeImagesRequestDescribeImagesPaginateTypeDef",
     "DescribeImagesRequestRequestTypeDef",
     "DescribePullThroughCacheRulesResponseTypeDef",
     "GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     "GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
     "GetLifecyclePolicyPreviewRequestRequestTypeDef",
     "ImageDetailTypeDef",
     "LifecyclePolicyPreviewResultTypeDef",
     "ListImagesRequestListImagesPaginateTypeDef",
     "ListImagesRequestRequestTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
+    "RegistryScanningRuleOutputTypeDef",
     "RegistryScanningRuleTypeDef",
     "RepositoryScanningConfigurationTypeDef",
+    "ReplicationRuleOutputTypeDef",
     "ReplicationRuleTypeDef",
     "ResourceTypeDef",
     "BatchDeleteImageResponseTypeDef",
     "BatchGetImageResponseTypeDef",
     "PutImageResponseTypeDef",
     "CreateRepositoryResponseTypeDef",
     "DeleteRepositoryResponseTypeDef",
     "DescribeRepositoriesResponseTypeDef",
     "ScoreDetailsTypeDef",
     "DescribeImagesResponseTypeDef",
     "GetLifecyclePolicyPreviewResponseTypeDef",
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
     "RegistryScanningConfigurationTypeDef",
+    "RegistryScanningRuleUnionTypeDef",
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
+    "ReplicationConfigurationOutputTypeDef",
     "ReplicationConfigurationTypeDef",
     "EnhancedImageScanFindingTypeDef",
     "GetRegistryScanningConfigurationResponseTypeDef",
     "PutRegistryScanningConfigurationResponseTypeDef",
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
     "DescribeRegistryResponseTypeDef",
-    "PutReplicationConfigurationRequestRequestTypeDef",
     "PutReplicationConfigurationResponseTypeDef",
+    "PutReplicationConfigurationRequestRequestTypeDef",
+    "ReplicationConfigurationUnionTypeDef",
     "ImageScanFindingsTypeDef",
     "DescribeImageScanFindingsResponseTypeDef",
 )
 
 _RequiredAttributeTypeDef = TypedDict(
     "_RequiredAttributeTypeDef",
     {
@@ -186,17 +193,19 @@
     "_OptionalAttributeTypeDef",
     {
         "value": str,
     },
     total=False,
 )
 
+
 class AttributeTypeDef(_RequiredAttributeTypeDef, _OptionalAttributeTypeDef):
     pass
 
+
 AuthorizationDataTypeDef = TypedDict(
     "AuthorizationDataTypeDef",
     {
         "authorizationToken": str,
         "expiresAt": datetime,
         "proxyEndpoint": str,
     },
@@ -229,20 +238,22 @@
     "_OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class BatchCheckLayerAvailabilityRequestRequestTypeDef(
     _RequiredBatchCheckLayerAvailabilityRequestRequestTypeDef,
     _OptionalBatchCheckLayerAvailabilityRequestRequestTypeDef,
 ):
     pass
 
+
 LayerFailureTypeDef = TypedDict(
     "LayerFailureTypeDef",
     {
         "layerDigest": str,
         "failureCode": LayerFailureCodeType,
         "failureReason": str,
     },
@@ -256,14 +267,25 @@
         "layerAvailability": LayerAvailabilityType,
         "layerSize": int,
         "mediaType": str,
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
 ImageIdentifierTypeDef = TypedDict(
     "ImageIdentifierTypeDef",
     {
         "imageDigest": str,
         "imageTag": str,
     },
     total=False,
@@ -282,14 +304,15 @@
         "repositoryName": str,
         "failureCode": Literal["REPOSITORY_NOT_FOUND"],
         "failureReason": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 _RequiredCompleteLayerUploadRequestRequestTypeDef = TypedDict(
     "_RequiredCompleteLayerUploadRequestRequestTypeDef",
     {
         "repositoryName": str,
         "uploadId": str,
         "layerDigests": Sequence[str],
     },
@@ -298,30 +321,21 @@
     "_OptionalCompleteLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class CompleteLayerUploadRequestRequestTypeDef(
     _RequiredCompleteLayerUploadRequestRequestTypeDef,
     _OptionalCompleteLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-CompleteLayerUploadResponseTypeDef = TypedDict(
-    "CompleteLayerUploadResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "uploadId": str,
-        "layerDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePullThroughCacheRuleRequestRequestTypeDef",
     {
         "ecrRepositoryPrefix": str,
         "upstreamRegistryUrl": str,
     },
@@ -330,30 +344,21 @@
     "_OptionalCreatePullThroughCacheRuleRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class CreatePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredCreatePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalCreatePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
-CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
-    "CreatePullThroughCacheRuleResponseTypeDef",
-    {
-        "ecrRepositoryPrefix": str,
-        "upstreamRegistryUrl": str,
-        "createdAt": datetime,
-        "registryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredEncryptionConfigurationTypeDef = TypedDict(
     "_RequiredEncryptionConfigurationTypeDef",
     {
         "encryptionType": EncryptionTypeType,
     },
 )
@@ -361,19 +366,21 @@
     "_OptionalEncryptionConfigurationTypeDef",
     {
         "kmsKey": str,
     },
     total=False,
 )
 
+
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
+
 ImageScanningConfigurationTypeDef = TypedDict(
     "ImageScanningConfigurationTypeDef",
     {
         "scanOnPush": bool,
     },
     total=False,
 )
@@ -417,30 +424,21 @@
     "_OptionalDeleteLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DeleteLifecyclePolicyRequestRequestTypeDef(
     _RequiredDeleteLifecyclePolicyRequestRequestTypeDef,
     _OptionalDeleteLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-DeleteLifecyclePolicyResponseTypeDef = TypedDict(
-    "DeleteLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "lastEvaluatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePullThroughCacheRuleRequestRequestTypeDef",
     {
         "ecrRepositoryPrefix": str,
     },
 )
@@ -448,39 +446,21 @@
     "_OptionalDeletePullThroughCacheRuleRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DeletePullThroughCacheRuleRequestRequestTypeDef(
     _RequiredDeletePullThroughCacheRuleRequestRequestTypeDef,
     _OptionalDeletePullThroughCacheRuleRequestRequestTypeDef,
 ):
     pass
 
-DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
-    "DeletePullThroughCacheRuleResponseTypeDef",
-    {
-        "ecrRepositoryPrefix": str,
-        "upstreamRegistryUrl": str,
-        "createdAt": datetime,
-        "registryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteRegistryPolicyResponseTypeDef = TypedDict(
-    "DeleteRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeleteRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
@@ -488,29 +468,21 @@
     "_OptionalDeleteRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DeleteRepositoryPolicyRequestRequestTypeDef(
     _RequiredDeleteRepositoryPolicyRequestRequestTypeDef,
     _OptionalDeleteRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-DeleteRepositoryPolicyResponseTypeDef = TypedDict(
-    "DeleteRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredDeleteRepositoryRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteRepositoryRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
@@ -519,30 +491,42 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class DeleteRepositoryRequestRequestTypeDef(
     _RequiredDeleteRepositoryRequestRequestTypeDef, _OptionalDeleteRepositoryRequestRequestTypeDef
 ):
     pass
 
+
 ImageReplicationStatusTypeDef = TypedDict(
     "ImageReplicationStatusTypeDef",
     {
         "region": str,
         "registryId": str,
         "status": ReplicationStatusType,
         "failureCode": str,
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -561,24 +545,14 @@
     "DescribeImagesFilterTypeDef",
     {
         "tagStatus": TagStatusType,
     },
     total=False,
 )
 
-DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = TypedDict(
-    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
-    {
-        "registryId": str,
-        "ecrRepositoryPrefixes": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribePullThroughCacheRulesRequestRequestTypeDef = TypedDict(
     "DescribePullThroughCacheRulesRequestRequestTypeDef",
     {
         "registryId": str,
         "ecrRepositoryPrefixes": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -593,24 +567,14 @@
         "upstreamRegistryUrl": str,
         "createdAt": datetime,
         "registryId": str,
     },
     total=False,
 )
 
-DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
-    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
-    {
-        "registryId": str,
-        "repositoryNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRepositoriesRequestRequestTypeDef = TypedDict(
     "DescribeRepositoriesRequestRequestTypeDef",
     {
         "registryId": str,
         "repositoryNames": Sequence[str],
         "nextToken": str,
         "maxResults": int,
@@ -637,28 +601,21 @@
     "_OptionalGetDownloadUrlForLayerRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetDownloadUrlForLayerRequestRequestTypeDef(
     _RequiredGetDownloadUrlForLayerRequestRequestTypeDef,
     _OptionalGetDownloadUrlForLayerRequestRequestTypeDef,
 ):
     pass
 
-GetDownloadUrlForLayerResponseTypeDef = TypedDict(
-    "GetDownloadUrlForLayerResponseTypeDef",
-    {
-        "downloadUrl": str,
-        "layerDigest": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 LifecyclePolicyPreviewFilterTypeDef = TypedDict(
     "LifecyclePolicyPreviewFilterTypeDef",
     {
         "tagStatus": TagStatusType,
     },
     total=False,
@@ -682,39 +639,21 @@
     "_OptionalGetLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetLifecyclePolicyRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-GetLifecyclePolicyResponseTypeDef = TypedDict(
-    "GetLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "lastEvaluatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetRegistryPolicyResponseTypeDef = TypedDict(
-    "GetRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
@@ -722,29 +661,21 @@
     "_OptionalGetRepositoryPolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class GetRepositoryPolicyRequestRequestTypeDef(
     _RequiredGetRepositoryPolicyRequestRequestTypeDef,
     _OptionalGetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-GetRepositoryPolicyResponseTypeDef = TypedDict(
-    "GetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ImageScanFindingsSummaryTypeDef = TypedDict(
     "ImageScanFindingsSummaryTypeDef",
     {
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
@@ -762,28 +693,21 @@
     "_OptionalInitiateLayerUploadRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class InitiateLayerUploadRequestRequestTypeDef(
     _RequiredInitiateLayerUploadRequestRequestTypeDef,
     _OptionalInitiateLayerUploadRequestRequestTypeDef,
 ):
     pass
 
-InitiateLayerUploadResponseTypeDef = TypedDict(
-    "InitiateLayerUploadResponseTypeDef",
-    {
-        "uploadId": str,
-        "partSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 LifecyclePolicyRuleActionTypeDef = TypedDict(
     "LifecyclePolicyRuleActionTypeDef",
     {
         "type": Literal["EXPIRE"],
     },
     total=False,
@@ -815,24 +739,14 @@
         "release": str,
         "sourceLayerHash": str,
         "version": str,
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
 _RequiredPutImageRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageManifest": str,
     },
 )
@@ -843,19 +757,21 @@
         "imageManifestMediaType": str,
         "imageTag": str,
         "imageDigest": str,
     },
     total=False,
 )
 
+
 class PutImageRequestRequestTypeDef(
     _RequiredPutImageRequestRequestTypeDef, _OptionalPutImageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutImageTagMutabilityRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageTagMutabilityRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageTagMutability": ImageTagMutabilityType,
     },
 )
@@ -863,29 +779,21 @@
     "_OptionalPutImageTagMutabilityRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class PutImageTagMutabilityRequestRequestTypeDef(
     _RequiredPutImageTagMutabilityRequestRequestTypeDef,
     _OptionalPutImageTagMutabilityRequestRequestTypeDef,
 ):
     pass
 
-PutImageTagMutabilityResponseTypeDef = TypedDict(
-    "PutImageTagMutabilityResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "imageTagMutability": ImageTagMutabilityType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredPutLifecyclePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutLifecyclePolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "lifecyclePolicyText": str,
     },
@@ -894,46 +802,29 @@
     "_OptionalPutLifecyclePolicyRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class PutLifecyclePolicyRequestRequestTypeDef(
     _RequiredPutLifecyclePolicyRequestRequestTypeDef,
     _OptionalPutLifecyclePolicyRequestRequestTypeDef,
 ):
     pass
 
-PutLifecyclePolicyResponseTypeDef = TypedDict(
-    "PutLifecyclePolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 PutRegistryPolicyRequestRequestTypeDef = TypedDict(
     "PutRegistryPolicyRequestRequestTypeDef",
     {
         "policyText": str,
     },
 )
 
-PutRegistryPolicyResponseTypeDef = TypedDict(
-    "PutRegistryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "url": str,
         "text": str,
     },
     total=False,
@@ -959,25 +850,14 @@
     "RepositoryFilterTypeDef",
     {
         "filter": str,
         "filterType": Literal["PREFIX_MATCH"],
     },
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
 _RequiredSetRepositoryPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredSetRepositoryPolicyRequestRequestTypeDef",
     {
         "repositoryName": str,
         "policyText": str,
     },
 )
@@ -986,29 +866,21 @@
     {
         "registryId": str,
         "force": bool,
     },
     total=False,
 )
 
+
 class SetRepositoryPolicyRequestRequestTypeDef(
     _RequiredSetRepositoryPolicyRequestRequestTypeDef,
     _OptionalSetRepositoryPolicyRequestRequestTypeDef,
 ):
     pass
 
-SetRepositoryPolicyResponseTypeDef = TypedDict(
-    "SetRepositoryPolicyResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "policyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
@@ -1017,107 +889,236 @@
     {
         "registryId": str,
         "lifecyclePolicyText": str,
     },
     total=False,
 )
 
+
 class StartLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredStartLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalStartLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
-StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
-    "StartLifecyclePolicyPreviewResponseTypeDef",
-    {
-        "registryId": str,
-        "repositoryName": str,
-        "lifecyclePolicyText": str,
-        "status": LifecyclePolicyPreviewStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
-    "_RequiredUploadLayerPartRequestRequestTypeDef",
+ImageScanFindingTypeDef = TypedDict(
+    "ImageScanFindingTypeDef",
     {
-        "repositoryName": str,
-        "uploadId": str,
-        "partFirstByte": int,
-        "partLastByte": int,
-        "layerPartBlob": Union[str, bytes, IO[Any], StreamingBody],
+        "name": str,
+        "description": str,
+        "uri": str,
+        "severity": FindingSeverityType,
+        "attributes": List[AttributeTypeDef],
     },
+    total=False,
 )
-_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
-    "_OptionalUploadLayerPartRequestRequestTypeDef",
+
+ResourceDetailsTypeDef = TypedDict(
+    "ResourceDetailsTypeDef",
     {
-        "registryId": str,
+        "awsEcrContainerImage": AwsEcrContainerImageDetailsTypeDef,
     },
     total=False,
 )
 
-class UploadLayerPartRequestRequestTypeDef(
-    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
-):
-    pass
+BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
+    "BatchCheckLayerAvailabilityResponseTypeDef",
+    {
+        "layers": List[LayerTypeDef],
+        "failures": List[LayerFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UploadLayerPartResponseTypeDef = TypedDict(
-    "UploadLayerPartResponseTypeDef",
+CompleteLayerUploadResponseTypeDef = TypedDict(
+    "CompleteLayerUploadResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "uploadId": str,
-        "lastByteReceived": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "layerDigest": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ImageScanFindingTypeDef = TypedDict(
-    "ImageScanFindingTypeDef",
+CreatePullThroughCacheRuleResponseTypeDef = TypedDict(
+    "CreatePullThroughCacheRuleResponseTypeDef",
     {
-        "name": str,
-        "description": str,
-        "uri": str,
-        "severity": FindingSeverityType,
-        "attributes": List[AttributeTypeDef],
+        "ecrRepositoryPrefix": str,
+        "upstreamRegistryUrl": str,
+        "createdAt": datetime,
+        "registryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteLifecyclePolicyResponseTypeDef = TypedDict(
+    "DeleteLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "lastEvaluatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePullThroughCacheRuleResponseTypeDef = TypedDict(
+    "DeletePullThroughCacheRuleResponseTypeDef",
+    {
+        "ecrRepositoryPrefix": str,
+        "upstreamRegistryUrl": str,
+        "createdAt": datetime,
+        "registryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRegistryPolicyResponseTypeDef = TypedDict(
+    "DeleteRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRepositoryPolicyResponseTypeDef = TypedDict(
+    "DeleteRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetAuthorizationTokenResponseTypeDef = TypedDict(
     "GetAuthorizationTokenResponseTypeDef",
     {
         "authorizationData": List[AuthorizationDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResourceDetailsTypeDef = TypedDict(
-    "ResourceDetailsTypeDef",
+GetDownloadUrlForLayerResponseTypeDef = TypedDict(
+    "GetDownloadUrlForLayerResponseTypeDef",
     {
-        "awsEcrContainerImage": AwsEcrContainerImageDetailsTypeDef,
+        "downloadUrl": str,
+        "layerDigest": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-BatchCheckLayerAvailabilityResponseTypeDef = TypedDict(
-    "BatchCheckLayerAvailabilityResponseTypeDef",
+GetLifecyclePolicyResponseTypeDef = TypedDict(
+    "GetLifecyclePolicyResponseTypeDef",
     {
-        "layers": List[LayerTypeDef],
-        "failures": List[LayerFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "lastEvaluatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRegistryPolicyResponseTypeDef = TypedDict(
+    "GetRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRepositoryPolicyResponseTypeDef = TypedDict(
+    "GetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateLayerUploadResponseTypeDef = TypedDict(
+    "InitiateLayerUploadResponseTypeDef",
+    {
+        "uploadId": str,
+        "partSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutImageTagMutabilityResponseTypeDef = TypedDict(
+    "PutImageTagMutabilityResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "imageTagMutability": ImageTagMutabilityType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutLifecyclePolicyResponseTypeDef = TypedDict(
+    "PutLifecyclePolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRegistryPolicyResponseTypeDef = TypedDict(
+    "PutRegistryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetRepositoryPolicyResponseTypeDef = TypedDict(
+    "SetRepositoryPolicyResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "policyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartLifecyclePolicyPreviewResponseTypeDef = TypedDict(
+    "StartLifecyclePolicyPreviewResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "lifecyclePolicyText": str,
+        "status": LifecyclePolicyPreviewStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadLayerPartResponseTypeDef = TypedDict(
+    "UploadLayerPartResponseTypeDef",
+    {
+        "registryId": str,
+        "repositoryName": str,
+        "uploadId": str,
+        "lastByteReceived": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchDeleteImageRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteImageRequestRequestTypeDef",
     {
         "repositoryName": str,
@@ -1128,19 +1129,21 @@
     "_OptionalBatchDeleteImageRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class BatchDeleteImageRequestRequestTypeDef(
     _RequiredBatchDeleteImageRequestRequestTypeDef, _OptionalBatchDeleteImageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredBatchGetImageRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetImageRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
     },
 )
@@ -1149,19 +1152,21 @@
     {
         "registryId": str,
         "acceptedMediaTypes": Sequence[str],
     },
     total=False,
 )
 
+
 class BatchGetImageRequestRequestTypeDef(
     _RequiredBatchGetImageRequestRequestTypeDef, _OptionalBatchGetImageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeImageReplicationStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageReplicationStatusRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
 )
@@ -1169,41 +1174,21 @@
     "_OptionalDescribeImageReplicationStatusRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class DescribeImageReplicationStatusRequestRequestTypeDef(
     _RequiredDescribeImageReplicationStatusRequestRequestTypeDef,
     _OptionalDescribeImageReplicationStatusRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    {
-        "repositoryName": str,
-        "imageId": ImageIdentifierTypeDef,
-    },
-)
-_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
-    {
-        "registryId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
-    _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-    _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
-):
-    pass
 
 _RequiredDescribeImageScanFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
     },
@@ -1214,20 +1199,22 @@
         "registryId": str,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class DescribeImageScanFindingsRequestRequestTypeDef(
     _RequiredDescribeImageScanFindingsRequestRequestTypeDef,
     _OptionalDescribeImageScanFindingsRequestRequestTypeDef,
 ):
     pass
 
+
 ImageFailureTypeDef = TypedDict(
     "ImageFailureTypeDef",
     {
         "imageId": ImageIdentifierTypeDef,
         "failureCode": ImageFailureCodeType,
         "failureReason": str,
     },
@@ -1247,15 +1234,15 @@
 )
 
 ListImagesResponseTypeDef = TypedDict(
     "ListImagesResponseTypeDef",
     {
         "imageIds": List[ImageIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartImageScanRequestRequestTypeDef = TypedDict(
     "_RequiredStartImageScanRequestRequestTypeDef",
     {
         "repositoryName": str,
@@ -1266,19 +1253,46 @@
     "_OptionalStartImageScanRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class StartImageScanRequestRequestTypeDef(
     _RequiredStartImageScanRequestRequestTypeDef, _OptionalStartImageScanRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_RequiredUploadLayerPartRequestRequestTypeDef",
+    {
+        "repositoryName": str,
+        "uploadId": str,
+        "partFirstByte": int,
+        "partLastByte": int,
+        "layerPartBlob": BlobTypeDef,
+    },
+)
+_OptionalUploadLayerPartRequestRequestTypeDef = TypedDict(
+    "_OptionalUploadLayerPartRequestRequestTypeDef",
+    {
+        "registryId": str,
+    },
+    total=False,
+)
+
+
+class UploadLayerPartRequestRequestTypeDef(
+    _RequiredUploadLayerPartRequestRequestTypeDef, _OptionalUploadLayerPartRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredPutImageScanningConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "repositoryName": str,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
     },
 )
@@ -1286,27 +1300,29 @@
     "_OptionalPutImageScanningConfigurationRequestRequestTypeDef",
     {
         "registryId": str,
     },
     total=False,
 )
 
+
 class PutImageScanningConfigurationRequestRequestTypeDef(
     _RequiredPutImageScanningConfigurationRequestRequestTypeDef,
     _OptionalPutImageScanningConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 PutImageScanningConfigurationResponseTypeDef = TypedDict(
     "PutImageScanningConfigurationResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RepositoryTypeDef = TypedDict(
     "RepositoryTypeDef",
     {
         "repositoryArn": str,
@@ -1335,24 +1351,26 @@
         "imageTagMutability": ImageTagMutabilityType,
         "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
         "encryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateRepositoryRequestRequestTypeDef(
     _RequiredCreateRepositoryRequestRequestTypeDef, _OptionalCreateRepositoryRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -1374,16 +1392,60 @@
 
 DescribeImageReplicationStatusResponseTypeDef = TypedDict(
     "DescribeImageReplicationStatusResponseTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
         "replicationStatuses": List[ImageReplicationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    {
+        "repositoryName": str,
+        "imageId": ImageIdentifierTypeDef,
+    },
+)
+_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef",
+    {
+        "registryId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef(
+    _RequiredDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+    _OptionalDescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+):
+    pass
+
+
+DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef = TypedDict(
+    "DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef",
+    {
+        "registryId": str,
+        "ecrRepositoryPrefixes": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef = TypedDict(
+    "DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef",
+    {
+        "registryId": str,
+        "repositoryNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef = TypedDict(
     "_RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef",
     {
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
@@ -1396,28 +1458,30 @@
         "nextToken": str,
         "maxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef(
     _RequiredDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     _OptionalDescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
 ):
     pass
 
+
 StartImageScanResponseTypeDef = TypedDict(
     "StartImageScanResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "repositoryName": str,
@@ -1425,25 +1489,27 @@
 )
 _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef = TypedDict(
     "_OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef",
     {
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": DescribeImagesFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeImagesRequestDescribeImagesPaginateTypeDef(
     _RequiredDescribeImagesRequestDescribeImagesPaginateTypeDef,
     _OptionalDescribeImagesRequestDescribeImagesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeImagesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalDescribeImagesRequestRequestTypeDef = TypedDict(
@@ -1454,25 +1520,27 @@
         "nextToken": str,
         "maxResults": int,
         "filter": DescribeImagesFilterTypeDef,
     },
     total=False,
 )
 
+
 class DescribeImagesRequestRequestTypeDef(
     _RequiredDescribeImagesRequestRequestTypeDef, _OptionalDescribeImagesRequestRequestTypeDef
 ):
     pass
 
+
 DescribePullThroughCacheRulesResponseTypeDef = TypedDict(
     "DescribePullThroughCacheRulesResponseTypeDef",
     {
         "pullThroughCacheRules": List[PullThroughCacheRuleTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     {
         "repositoryName": str,
@@ -1480,25 +1548,27 @@
 )
 _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef = TypedDict(
     "_OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef",
     {
         "registryId": str,
         "imageIds": Sequence[ImageIdentifierTypeDef],
         "filter": LifecyclePolicyPreviewFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef = TypedDict(
@@ -1510,20 +1580,22 @@
         "maxResults": int,
         "filter": LifecyclePolicyPreviewFilterTypeDef,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalGetLifecyclePolicyPreviewRequestRequestTypeDef = TypedDict(
@@ -1534,20 +1606,22 @@
         "nextToken": str,
         "maxResults": int,
         "filter": LifecyclePolicyPreviewFilterTypeDef,
     },
     total=False,
 )
 
+
 class GetLifecyclePolicyPreviewRequestRequestTypeDef(
     _RequiredGetLifecyclePolicyPreviewRequestRequestTypeDef,
     _OptionalGetLifecyclePolicyPreviewRequestRequestTypeDef,
 ):
     pass
 
+
 ImageDetailTypeDef = TypedDict(
     "ImageDetailTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "imageDigest": str,
         "imageTags": List[str],
@@ -1581,25 +1655,27 @@
     },
 )
 _OptionalListImagesRequestListImagesPaginateTypeDef = TypedDict(
     "_OptionalListImagesRequestListImagesPaginateTypeDef",
     {
         "registryId": str,
         "filter": ListImagesFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListImagesRequestListImagesPaginateTypeDef(
     _RequiredListImagesRequestListImagesPaginateTypeDef,
     _OptionalListImagesRequestListImagesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListImagesRequestRequestTypeDef = TypedDict(
     "_RequiredListImagesRequestRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 _OptionalListImagesRequestRequestTypeDef = TypedDict(
@@ -1609,19 +1685,21 @@
         "nextToken": str,
         "maxResults": int,
         "filter": ListImagesFilterTypeDef,
     },
     total=False,
 )
 
+
 class ListImagesRequestRequestTypeDef(
     _RequiredListImagesRequestRequestTypeDef, _OptionalListImagesRequestRequestTypeDef
 ):
     pass
 
+
 PackageVulnerabilityDetailsTypeDef = TypedDict(
     "PackageVulnerabilityDetailsTypeDef",
     {
         "cvss": List[CvssScoreTypeDef],
         "referenceUrls": List[str],
         "relatedVulnerabilities": List[str],
         "source": str,
@@ -1639,19 +1717,27 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
+RegistryScanningRuleOutputTypeDef = TypedDict(
+    "RegistryScanningRuleOutputTypeDef",
+    {
+        "scanFrequency": ScanFrequencyType,
+        "repositoryFilters": List[ScanningRepositoryFilterTypeDef],
+    },
+)
+
 RegistryScanningRuleTypeDef = TypedDict(
     "RegistryScanningRuleTypeDef",
     {
         "scanFrequency": ScanFrequencyType,
-        "repositoryFilters": List[ScanningRepositoryFilterTypeDef],
+        "repositoryFilters": Sequence[ScanningRepositoryFilterTypeDef],
     },
 )
 
 RepositoryScanningConfigurationTypeDef = TypedDict(
     "RepositoryScanningConfigurationTypeDef",
     {
         "repositoryArn": str,
@@ -1659,31 +1745,54 @@
         "scanOnPush": bool,
         "scanFrequency": ScanFrequencyType,
         "appliedScanFilters": List[ScanningRepositoryFilterTypeDef],
     },
     total=False,
 )
 
+_RequiredReplicationRuleOutputTypeDef = TypedDict(
+    "_RequiredReplicationRuleOutputTypeDef",
+    {
+        "destinations": List[ReplicationDestinationTypeDef],
+    },
+)
+_OptionalReplicationRuleOutputTypeDef = TypedDict(
+    "_OptionalReplicationRuleOutputTypeDef",
+    {
+        "repositoryFilters": List[RepositoryFilterTypeDef],
+    },
+    total=False,
+)
+
+
+class ReplicationRuleOutputTypeDef(
+    _RequiredReplicationRuleOutputTypeDef, _OptionalReplicationRuleOutputTypeDef
+):
+    pass
+
+
 _RequiredReplicationRuleTypeDef = TypedDict(
     "_RequiredReplicationRuleTypeDef",
     {
-        "destinations": List[ReplicationDestinationTypeDef],
+        "destinations": Sequence[ReplicationDestinationTypeDef],
     },
 )
 _OptionalReplicationRuleTypeDef = TypedDict(
     "_OptionalReplicationRuleTypeDef",
     {
-        "repositoryFilters": List[RepositoryFilterTypeDef],
+        "repositoryFilters": Sequence[RepositoryFilterTypeDef],
     },
     total=False,
 )
 
+
 class ReplicationRuleTypeDef(_RequiredReplicationRuleTypeDef, _OptionalReplicationRuleTypeDef):
     pass
 
+
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "details": ResourceDetailsTypeDef,
         "id": str,
         "tags": Dict[str, str],
         "type": str,
@@ -1692,57 +1801,57 @@
 )
 
 BatchDeleteImageResponseTypeDef = TypedDict(
     "BatchDeleteImageResponseTypeDef",
     {
         "imageIds": List[ImageIdentifierTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetImageResponseTypeDef = TypedDict(
     "BatchGetImageResponseTypeDef",
     {
         "images": List[ImageTypeDef],
         "failures": List[ImageFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutImageResponseTypeDef = TypedDict(
     "PutImageResponseTypeDef",
     {
         "image": ImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRepositoryResponseTypeDef = TypedDict(
     "CreateRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRepositoryResponseTypeDef = TypedDict(
     "DeleteRepositoryResponseTypeDef",
     {
         "repository": RepositoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRepositoriesResponseTypeDef = TypedDict(
     "DescribeRepositoriesResponseTypeDef",
     {
         "repositories": List[RepositoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ScoreDetailsTypeDef = TypedDict(
     "ScoreDetailsTypeDef",
     {
         "cvss": CvssScoreDetailsTypeDef,
@@ -1751,63 +1860,64 @@
 )
 
 DescribeImagesResponseTypeDef = TypedDict(
     "DescribeImagesResponseTypeDef",
     {
         "imageDetails": List[ImageDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLifecyclePolicyPreviewResponseTypeDef = TypedDict(
     "GetLifecyclePolicyPreviewResponseTypeDef",
     {
         "registryId": str,
         "repositoryName": str,
         "lifecyclePolicyText": str,
         "status": LifecyclePolicyPreviewStatusType,
         "nextToken": str,
         "previewResults": List[LifecyclePolicyPreviewResultTypeDef],
         "summary": LifecyclePolicyPreviewSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
-    "PutRegistryScanningConfigurationRequestRequestTypeDef",
-    {
-        "scanType": ScanTypeType,
-        "rules": Sequence[RegistryScanningRuleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 RegistryScanningConfigurationTypeDef = TypedDict(
     "RegistryScanningConfigurationTypeDef",
     {
         "scanType": ScanTypeType,
-        "rules": List[RegistryScanningRuleTypeDef],
+        "rules": List[RegistryScanningRuleOutputTypeDef],
     },
     total=False,
 )
 
+RegistryScanningRuleUnionTypeDef = Union[
+    RegistryScanningRuleTypeDef, RegistryScanningRuleOutputTypeDef
+]
 BatchGetRepositoryScanningConfigurationResponseTypeDef = TypedDict(
     "BatchGetRepositoryScanningConfigurationResponseTypeDef",
     {
         "scanningConfigurations": List[RepositoryScanningConfigurationTypeDef],
         "failures": List[RepositoryScanningConfigurationFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReplicationConfigurationOutputTypeDef = TypedDict(
+    "ReplicationConfigurationOutputTypeDef",
+    {
+        "rules": List[ReplicationRuleOutputTypeDef],
     },
 )
 
 ReplicationConfigurationTypeDef = TypedDict(
     "ReplicationConfigurationTypeDef",
     {
-        "rules": List[ReplicationRuleTypeDef],
+        "rules": Sequence[ReplicationRuleTypeDef],
     },
 )
 
 EnhancedImageScanFindingTypeDef = TypedDict(
     "EnhancedImageScanFindingTypeDef",
     {
         "awsAccountId": str,
@@ -1830,50 +1940,62 @@
 )
 
 GetRegistryScanningConfigurationResponseTypeDef = TypedDict(
     "GetRegistryScanningConfigurationResponseTypeDef",
     {
         "registryId": str,
         "scanningConfiguration": RegistryScanningConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRegistryScanningConfigurationResponseTypeDef = TypedDict(
     "PutRegistryScanningConfigurationResponseTypeDef",
     {
         "registryScanningConfiguration": RegistryScanningConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRegistryScanningConfigurationRequestRequestTypeDef = TypedDict(
+    "PutRegistryScanningConfigurationRequestRequestTypeDef",
+    {
+        "scanType": ScanTypeType,
+        "rules": Sequence[RegistryScanningRuleUnionTypeDef],
     },
+    total=False,
 )
 
 DescribeRegistryResponseTypeDef = TypedDict(
     "DescribeRegistryResponseTypeDef",
     {
         "registryId": str,
-        "replicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
-    "PutReplicationConfigurationRequestRequestTypeDef",
+PutReplicationConfigurationResponseTypeDef = TypedDict(
+    "PutReplicationConfigurationResponseTypeDef",
     {
-        "replicationConfiguration": ReplicationConfigurationTypeDef,
+        "replicationConfiguration": ReplicationConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutReplicationConfigurationResponseTypeDef = TypedDict(
-    "PutReplicationConfigurationResponseTypeDef",
+PutReplicationConfigurationRequestRequestTypeDef = TypedDict(
+    "PutReplicationConfigurationRequestRequestTypeDef",
     {
         "replicationConfiguration": ReplicationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+ReplicationConfigurationUnionTypeDef = Union[
+    ReplicationConfigurationTypeDef, ReplicationConfigurationOutputTypeDef
+]
 ImageScanFindingsTypeDef = TypedDict(
     "ImageScanFindingsTypeDef",
     {
         "imageScanCompletedAt": datetime,
         "vulnerabilitySourceUpdatedAt": datetime,
         "findingSeverityCounts": Dict[FindingSeverityType, int],
         "findings": List[ImageScanFindingTypeDef],
@@ -1887,10 +2009,10 @@
     {
         "registryId": str,
         "repositoryName": str,
         "imageId": ImageIdentifierTypeDef,
         "imageScanStatus": ImageScanStatusTypeDef,
         "imageScanFindings": ImageScanFindingsTypeDef,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/waiter.py` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr/waiter.pyi` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr.egg-info/PKG-INFO` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ECR 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ECR 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ecr type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ecr type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ecr"></a>
 
 # types-aiobotocore-ecr
 
 [![PyPI - types-aiobotocore-ecr](https://img.shields.io/pypi/v/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ecr?color=blue)](https://pypistats.org/packages/types-aiobotocore-ecr)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr)](https://pepy.tech/project/types-aiobotocore-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ECR 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [types-aiobotocore-ecr docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/).
 
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
@@ -376,159 +375,165 @@
 )
 
 
 def check_value(value: DescribeImageScanFindingsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ecr.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ecr.type_defs import (
     AttributeTypeDef,
     AuthorizationDataTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     BatchCheckLayerAvailabilityRequestRequestTypeDef,
     LayerFailureTypeDef,
     LayerTypeDef,
+    ResponseMetadataTypeDef,
     ImageIdentifierTypeDef,
     BatchGetRepositoryScanningConfigurationRequestRequestTypeDef,
     RepositoryScanningConfigurationFailureTypeDef,
+    BlobTypeDef,
     CompleteLayerUploadRequestRequestTypeDef,
-    CompleteLayerUploadResponseTypeDef,
     CreatePullThroughCacheRuleRequestRequestTypeDef,
-    CreatePullThroughCacheRuleResponseTypeDef,
     EncryptionConfigurationTypeDef,
     ImageScanningConfigurationTypeDef,
     TagTypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
-    DeleteLifecyclePolicyResponseTypeDef,
     DeletePullThroughCacheRuleRequestRequestTypeDef,
-    DeletePullThroughCacheRuleResponseTypeDef,
-    DeleteRegistryPolicyResponseTypeDef,
     DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
     DeleteRepositoryRequestRequestTypeDef,
     ImageReplicationStatusTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
     ImageScanStatusTypeDef,
     DescribeImagesFilterTypeDef,
-    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
     DescribePullThroughCacheRulesRequestRequestTypeDef,
     PullThroughCacheRuleTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeRepositoriesRequestRequestTypeDef,
     GetAuthorizationTokenRequestRequestTypeDef,
     GetDownloadUrlForLayerRequestRequestTypeDef,
-    GetDownloadUrlForLayerResponseTypeDef,
     LifecyclePolicyPreviewFilterTypeDef,
     LifecyclePolicyPreviewSummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
-    GetLifecyclePolicyResponseTypeDef,
-    GetRegistryPolicyResponseTypeDef,
     GetRepositoryPolicyRequestRequestTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
     ImageScanFindingsSummaryTypeDef,
     InitiateLayerUploadRequestRequestTypeDef,
-    InitiateLayerUploadResponseTypeDef,
     LifecyclePolicyRuleActionTypeDef,
     ListImagesFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     VulnerablePackageTypeDef,
-    PaginatorConfigTypeDef,
     PutImageRequestRequestTypeDef,
     PutImageTagMutabilityRequestRequestTypeDef,
-    PutImageTagMutabilityResponseTypeDef,
     PutLifecyclePolicyRequestRequestTypeDef,
-    PutLifecyclePolicyResponseTypeDef,
     PutRegistryPolicyRequestRequestTypeDef,
-    PutRegistryPolicyResponseTypeDef,
     RecommendationTypeDef,
     ScanningRepositoryFilterTypeDef,
     ReplicationDestinationTypeDef,
     RepositoryFilterTypeDef,
-    ResponseMetadataTypeDef,
     SetRepositoryPolicyRequestRequestTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
     StartLifecyclePolicyPreviewRequestRequestTypeDef,
-    StartLifecyclePolicyPreviewResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
-    UploadLayerPartResponseTypeDef,
     ImageScanFindingTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchCheckLayerAvailabilityResponseTypeDef,
+    CompleteLayerUploadResponseTypeDef,
+    CreatePullThroughCacheRuleResponseTypeDef,
+    DeleteLifecyclePolicyResponseTypeDef,
+    DeletePullThroughCacheRuleResponseTypeDef,
+    DeleteRegistryPolicyResponseTypeDef,
+    DeleteRepositoryPolicyResponseTypeDef,
+    GetAuthorizationTokenResponseTypeDef,
+    GetDownloadUrlForLayerResponseTypeDef,
+    GetLifecyclePolicyResponseTypeDef,
+    GetRegistryPolicyResponseTypeDef,
+    GetRepositoryPolicyResponseTypeDef,
+    InitiateLayerUploadResponseTypeDef,
+    PutImageTagMutabilityResponseTypeDef,
+    PutLifecyclePolicyResponseTypeDef,
+    PutRegistryPolicyResponseTypeDef,
+    SetRepositoryPolicyResponseTypeDef,
+    StartLifecyclePolicyPreviewResponseTypeDef,
+    UploadLayerPartResponseTypeDef,
     BatchDeleteImageRequestRequestTypeDef,
     BatchGetImageRequestRequestTypeDef,
     DescribeImageReplicationStatusRequestRequestTypeDef,
-    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
     DescribeImageScanFindingsRequestRequestTypeDef,
     ImageFailureTypeDef,
     ImageTypeDef,
     ListImagesResponseTypeDef,
     StartImageScanRequestRequestTypeDef,
+    UploadLayerPartRequestRequestTypeDef,
     PutImageScanningConfigurationRequestRequestTypeDef,
     PutImageScanningConfigurationResponseTypeDef,
     RepositoryTypeDef,
     CreateRepositoryRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CvssScoreDetailsTypeDef,
     DescribeImageReplicationStatusResponseTypeDef,
+    DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef,
+    DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef,
+    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
     DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef,
     StartImageScanResponseTypeDef,
     DescribeImagesRequestDescribeImagesPaginateTypeDef,
     DescribeImagesRequestRequestTypeDef,
     DescribePullThroughCacheRulesResponseTypeDef,
     GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef,
     GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef,
     GetLifecyclePolicyPreviewRequestRequestTypeDef,
     ImageDetailTypeDef,
     LifecyclePolicyPreviewResultTypeDef,
     ListImagesRequestListImagesPaginateTypeDef,
     ListImagesRequestRequestTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
+    RegistryScanningRuleOutputTypeDef,
     RegistryScanningRuleTypeDef,
     RepositoryScanningConfigurationTypeDef,
+    ReplicationRuleOutputTypeDef,
     ReplicationRuleTypeDef,
     ResourceTypeDef,
     BatchDeleteImageResponseTypeDef,
     BatchGetImageResponseTypeDef,
     PutImageResponseTypeDef,
     CreateRepositoryResponseTypeDef,
     DeleteRepositoryResponseTypeDef,
     DescribeRepositoriesResponseTypeDef,
     ScoreDetailsTypeDef,
     DescribeImagesResponseTypeDef,
     GetLifecyclePolicyPreviewResponseTypeDef,
-    PutRegistryScanningConfigurationRequestRequestTypeDef,
     RegistryScanningConfigurationTypeDef,
+    RegistryScanningRuleUnionTypeDef,
     BatchGetRepositoryScanningConfigurationResponseTypeDef,
+    ReplicationConfigurationOutputTypeDef,
     ReplicationConfigurationTypeDef,
     EnhancedImageScanFindingTypeDef,
     GetRegistryScanningConfigurationResponseTypeDef,
     PutRegistryScanningConfigurationResponseTypeDef,
+    PutRegistryScanningConfigurationRequestRequestTypeDef,
     DescribeRegistryResponseTypeDef,
-    PutReplicationConfigurationRequestRequestTypeDef,
     PutReplicationConfigurationResponseTypeDef,
+    PutReplicationConfigurationRequestRequestTypeDef,
+    ReplicationConfigurationUnionTypeDef,
     ImageScanFindingsTypeDef,
     DescribeImageScanFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ecr-2.5.2/types_aiobotocore_ecr.egg-info/SOURCES.txt` & `types-aiobotocore-ecr-2.5.2.post1/types_aiobotocore_ecr.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-batch-2.5.2.tar.gz` & `tmp/types-aiobotocore-batch-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-batch-2.5.2.tar", last modified: Sat Jul  8 01:43:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-batch-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
```

## Comparing `types-aiobotocore-batch-2.5.2.tar` & `types-aiobotocore-batch-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.969739 types-aiobotocore-batch-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:20.000000 types-aiobotocore-batch-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-07-08 01:43:16.965739 types-aiobotocore-batch-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16651 2023-07-08 01:26:20.000000 types-aiobotocore-batch-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:16.969739 types-aiobotocore-batch-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-08 01:26:20.000000 types-aiobotocore-batch-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.961739 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-08 01:26:20.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-08 01:26:20.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-08 01:26:20.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22153 2023-07-08 01:26:20.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22115 2023-07-08 01:26:20.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-07-08 01:26:21.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-07-08 01:26:21.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-07-08 01:26:21.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-08 01:26:20.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:20.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44081 2023-07-08 01:26:22.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44024 2023-07-08 01:26:21.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:20.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.965739 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18208 2023-07-08 01:43:16.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-08 01:43:16.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:16.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 01:43:16.000000 types-aiobotocore-batch-2.5.2/types_aiobotocore_batch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.385648 types-aiobotocore-batch-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18845 2023-08-02 14:51:55.385648 types-aiobotocore-batch-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17335 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.385648 types-aiobotocore-batch-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.385648 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22223 2023-08-02 14:33:48.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22185 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-08-02 14:33:48.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-08-02 14:33:48.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-08-02 14:33:48.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-08-02 14:33:48.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    51766 2023-08-02 14:33:50.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51697 2023-08-02 14:33:49.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.385648 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18845 2023-08-02 14:51:55.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 14:51:55.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:55.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:51:55.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-batch-2.5.2/LICENSE` & `types-aiobotocore-batch-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2/PKG-INFO` & `types-aiobotocore-batch-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-batch
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Batch 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Batch 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore batch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore batch type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-batch"></a>
 
 # types-aiobotocore-batch
 
 [![PyPI - types-aiobotocore-batch](https://img.shields.io/pypi/v/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-batch?color=blue)](https://pypistats.org/packages/types-aiobotocore-batch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-batch)](https://pepy.tech/project/types-aiobotocore-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Batch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [types-aiobotocore-batch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/).
 
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
@@ -345,20 +344,20 @@
 )
 
 
 def check_value(value: ArrayJobDependencyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_batch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_batch.type_defs import (
     ArrayPropertiesDetailTypeDef,
     ArrayPropertiesSummaryTypeDef,
     ArrayPropertiesTypeDef,
     NetworkInterfaceTypeDef,
@@ -373,118 +372,139 @@
     KeyValuePairTypeDef,
     MountPointTypeDef,
     NetworkConfigurationTypeDef,
     ResourceRequirementTypeDef,
     SecretTypeDef,
     UlimitTypeDef,
     ContainerSummaryTypeDef,
-    CreateComputeEnvironmentResponseTypeDef,
-    CreateJobQueueResponseTypeDef,
-    CreateSchedulingPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteComputeEnvironmentRequestRequestTypeDef,
     DeleteJobQueueRequestRequestTypeDef,
     DeleteSchedulingPolicyRequestRequestTypeDef,
     DeregisterJobDefinitionRequestRequestTypeDef,
-    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeComputeEnvironmentsRequestRequestTypeDef,
-    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
     DescribeJobDefinitionsRequestRequestTypeDef,
-    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
     DescribeJobQueuesRequestRequestTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeSchedulingPoliciesRequestRequestTypeDef,
+    DeviceOutputTypeDef,
     DeviceTypeDef,
     EFSAuthorizationConfigTypeDef,
     EksAttemptContainerDetailTypeDef,
     EksContainerEnvironmentVariableTypeDef,
-    EksContainerResourceRequirementsTypeDef,
+    EksContainerResourceRequirementsOutputTypeDef,
     EksContainerSecurityContextTypeDef,
     EksContainerVolumeMountTypeDef,
+    EksContainerResourceRequirementsTypeDef,
     EksEmptyDirTypeDef,
     EksHostPathTypeDef,
+    EksMetadataOutputTypeDef,
     EksMetadataTypeDef,
     EksSecretTypeDef,
     EvaluateOnExitTypeDef,
     ShareAttributesTypeDef,
     HostTypeDef,
     JobTimeoutTypeDef,
     JobDependencyTypeDef,
     NodeDetailsTypeDef,
     NodePropertiesSummaryTypeDef,
     KeyValuesPairTypeDef,
+    TmpfsOutputTypeDef,
     TmpfsTypeDef,
-    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     ListSchedulingPoliciesRequestRequestTypeDef,
     SchedulingPolicyListingDetailTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterJobDefinitionResponseTypeDef,
-    ResponseMetadataTypeDef,
-    SubmitJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateComputeEnvironmentResponseTypeDef,
-    UpdateJobQueueResponseTypeDef,
     AttemptContainerDetailTypeDef,
     CreateJobQueueRequestRequestTypeDef,
     JobQueueDetailTypeDef,
     UpdateJobQueueRequestRequestTypeDef,
+    ComputeResourceOutputTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
+    CreateComputeEnvironmentResponseTypeDef,
+    CreateJobQueueResponseTypeDef,
+    CreateSchedulingPolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterJobDefinitionResponseTypeDef,
+    SubmitJobResponseTypeDef,
+    UpdateComputeEnvironmentResponseTypeDef,
+    UpdateJobQueueResponseTypeDef,
+    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
+    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
+    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
+    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     EFSVolumeConfigurationTypeDef,
     EksAttemptDetailTypeDef,
-    EksContainerOverrideTypeDef,
     EksContainerDetailTypeDef,
+    EksContainerOutputTypeDef,
+    EksContainerOverrideTypeDef,
     EksContainerTypeDef,
     EksVolumeTypeDef,
+    RetryStrategyOutputTypeDef,
     RetryStrategyTypeDef,
+    FairsharePolicyOutputTypeDef,
     FairsharePolicyTypeDef,
     JobSummaryTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     AttemptDetailTypeDef,
     DescribeJobQueuesResponseTypeDef,
     ComputeEnvironmentDetailTypeDef,
+    ComputeResourceUnionTypeDef,
     CreateComputeEnvironmentRequestRequestTypeDef,
     UpdateComputeEnvironmentRequestRequestTypeDef,
     NodePropertyOverrideTypeDef,
     VolumeTypeDef,
     EksPodPropertiesOverrideTypeDef,
     EksPodPropertiesDetailTypeDef,
+    EksPodPropertiesOutputTypeDef,
     EksPodPropertiesTypeDef,
-    CreateSchedulingPolicyRequestRequestTypeDef,
+    RetryStrategyUnionTypeDef,
     SchedulingPolicyDetailTypeDef,
+    CreateSchedulingPolicyRequestRequestTypeDef,
+    FairsharePolicyUnionTypeDef,
     UpdateSchedulingPolicyRequestRequestTypeDef,
     ListJobsResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     NodeOverridesTypeDef,
     ContainerDetailTypeDef,
+    ContainerPropertiesOutputTypeDef,
     ContainerPropertiesTypeDef,
     EksPropertiesOverrideTypeDef,
     EksPropertiesDetailTypeDef,
+    EksPropertiesOutputTypeDef,
     EksPropertiesTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
+    NodeRangePropertyOutputTypeDef,
+    ContainerPropertiesUnionTypeDef,
     NodeRangePropertyTypeDef,
     SubmitJobRequestRequestTypeDef,
+    EksPropertiesUnionTypeDef,
+    NodePropertiesOutputTypeDef,
     NodePropertiesTypeDef,
     JobDefinitionTypeDef,
     JobDetailTypeDef,
+    NodePropertiesUnionTypeDef,
     RegisterJobDefinitionRequestRequestTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobsResponseTypeDef,
 )
 
 
-def get_structure() -> ArrayPropertiesDetailTypeDef:
+def get_value() -> ArrayPropertiesDetailTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-batch-2.5.2/README.md` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-batch
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Batch 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore batch type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-batch"></a>
 
 # types-aiobotocore-batch
 
 [![PyPI - types-aiobotocore-batch](https://img.shields.io/pypi/v/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-batch?color=blue)](https://pypistats.org/packages/types-aiobotocore-batch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-batch)](https://pepy.tech/project/types-aiobotocore-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Batch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [types-aiobotocore-batch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +73,15 @@
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
@@ -312,20 +344,20 @@
 )
 
 
 def check_value(value: ArrayJobDependencyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_batch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_batch.type_defs import (
     ArrayPropertiesDetailTypeDef,
     ArrayPropertiesSummaryTypeDef,
     ArrayPropertiesTypeDef,
     NetworkInterfaceTypeDef,
@@ -340,118 +372,139 @@
     KeyValuePairTypeDef,
     MountPointTypeDef,
     NetworkConfigurationTypeDef,
     ResourceRequirementTypeDef,
     SecretTypeDef,
     UlimitTypeDef,
     ContainerSummaryTypeDef,
-    CreateComputeEnvironmentResponseTypeDef,
-    CreateJobQueueResponseTypeDef,
-    CreateSchedulingPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteComputeEnvironmentRequestRequestTypeDef,
     DeleteJobQueueRequestRequestTypeDef,
     DeleteSchedulingPolicyRequestRequestTypeDef,
     DeregisterJobDefinitionRequestRequestTypeDef,
-    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeComputeEnvironmentsRequestRequestTypeDef,
-    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
     DescribeJobDefinitionsRequestRequestTypeDef,
-    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
     DescribeJobQueuesRequestRequestTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeSchedulingPoliciesRequestRequestTypeDef,
+    DeviceOutputTypeDef,
     DeviceTypeDef,
     EFSAuthorizationConfigTypeDef,
     EksAttemptContainerDetailTypeDef,
     EksContainerEnvironmentVariableTypeDef,
-    EksContainerResourceRequirementsTypeDef,
+    EksContainerResourceRequirementsOutputTypeDef,
     EksContainerSecurityContextTypeDef,
     EksContainerVolumeMountTypeDef,
+    EksContainerResourceRequirementsTypeDef,
     EksEmptyDirTypeDef,
     EksHostPathTypeDef,
+    EksMetadataOutputTypeDef,
     EksMetadataTypeDef,
     EksSecretTypeDef,
     EvaluateOnExitTypeDef,
     ShareAttributesTypeDef,
     HostTypeDef,
     JobTimeoutTypeDef,
     JobDependencyTypeDef,
     NodeDetailsTypeDef,
     NodePropertiesSummaryTypeDef,
     KeyValuesPairTypeDef,
+    TmpfsOutputTypeDef,
     TmpfsTypeDef,
-    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     ListSchedulingPoliciesRequestRequestTypeDef,
     SchedulingPolicyListingDetailTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterJobDefinitionResponseTypeDef,
-    ResponseMetadataTypeDef,
-    SubmitJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateComputeEnvironmentResponseTypeDef,
-    UpdateJobQueueResponseTypeDef,
     AttemptContainerDetailTypeDef,
     CreateJobQueueRequestRequestTypeDef,
     JobQueueDetailTypeDef,
     UpdateJobQueueRequestRequestTypeDef,
+    ComputeResourceOutputTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
+    CreateComputeEnvironmentResponseTypeDef,
+    CreateJobQueueResponseTypeDef,
+    CreateSchedulingPolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterJobDefinitionResponseTypeDef,
+    SubmitJobResponseTypeDef,
+    UpdateComputeEnvironmentResponseTypeDef,
+    UpdateJobQueueResponseTypeDef,
+    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
+    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
+    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
+    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     EFSVolumeConfigurationTypeDef,
     EksAttemptDetailTypeDef,
-    EksContainerOverrideTypeDef,
     EksContainerDetailTypeDef,
+    EksContainerOutputTypeDef,
+    EksContainerOverrideTypeDef,
     EksContainerTypeDef,
     EksVolumeTypeDef,
+    RetryStrategyOutputTypeDef,
     RetryStrategyTypeDef,
+    FairsharePolicyOutputTypeDef,
     FairsharePolicyTypeDef,
     JobSummaryTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     AttemptDetailTypeDef,
     DescribeJobQueuesResponseTypeDef,
     ComputeEnvironmentDetailTypeDef,
+    ComputeResourceUnionTypeDef,
     CreateComputeEnvironmentRequestRequestTypeDef,
     UpdateComputeEnvironmentRequestRequestTypeDef,
     NodePropertyOverrideTypeDef,
     VolumeTypeDef,
     EksPodPropertiesOverrideTypeDef,
     EksPodPropertiesDetailTypeDef,
+    EksPodPropertiesOutputTypeDef,
     EksPodPropertiesTypeDef,
-    CreateSchedulingPolicyRequestRequestTypeDef,
+    RetryStrategyUnionTypeDef,
     SchedulingPolicyDetailTypeDef,
+    CreateSchedulingPolicyRequestRequestTypeDef,
+    FairsharePolicyUnionTypeDef,
     UpdateSchedulingPolicyRequestRequestTypeDef,
     ListJobsResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     NodeOverridesTypeDef,
     ContainerDetailTypeDef,
+    ContainerPropertiesOutputTypeDef,
     ContainerPropertiesTypeDef,
     EksPropertiesOverrideTypeDef,
     EksPropertiesDetailTypeDef,
+    EksPropertiesOutputTypeDef,
     EksPropertiesTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
+    NodeRangePropertyOutputTypeDef,
+    ContainerPropertiesUnionTypeDef,
     NodeRangePropertyTypeDef,
     SubmitJobRequestRequestTypeDef,
+    EksPropertiesUnionTypeDef,
+    NodePropertiesOutputTypeDef,
     NodePropertiesTypeDef,
     JobDefinitionTypeDef,
     JobDetailTypeDef,
+    NodePropertiesUnionTypeDef,
     RegisterJobDefinitionRequestRequestTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobsResponseTypeDef,
 )
 
 
-def get_structure() -> ArrayPropertiesDetailTypeDef:
+def get_value() -> ArrayPropertiesDetailTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-batch-2.5.2/setup.py` & `types-aiobotocore-batch-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-batch",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_batch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Batch 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore batch type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore batch type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_batch": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/"
```

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/__init__.py` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/__init__.pyi` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/__main__.py` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Batch 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Batch 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch\nOther"
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

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/client.py` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,40 +34,40 @@
     DescribeJobQueuesPaginator,
     ListJobsPaginator,
     ListSchedulingPoliciesPaginator,
 )
 from .type_defs import (
     ArrayPropertiesTypeDef,
     ComputeEnvironmentOrderTypeDef,
-    ComputeResourceTypeDef,
+    ComputeResourceUnionTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
-    ContainerPropertiesTypeDef,
+    ContainerPropertiesUnionTypeDef,
     CreateComputeEnvironmentResponseTypeDef,
     CreateJobQueueResponseTypeDef,
     CreateSchedulingPolicyResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobQueuesResponseTypeDef,
     DescribeJobsResponseTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
     EksConfigurationTypeDef,
     EksPropertiesOverrideTypeDef,
-    EksPropertiesTypeDef,
-    FairsharePolicyTypeDef,
+    EksPropertiesUnionTypeDef,
+    FairsharePolicyUnionTypeDef,
     JobDependencyTypeDef,
     JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
     ListJobsResponseTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NodeOverridesTypeDef,
-    NodePropertiesTypeDef,
+    NodePropertiesUnionTypeDef,
     RegisterJobDefinitionResponseTypeDef,
-    RetryStrategyTypeDef,
+    RetryStrategyUnionTypeDef,
     SubmitJobResponseTypeDef,
     UpdateComputeEnvironmentResponseTypeDef,
     UpdateJobQueueResponseTypeDef,
     UpdatePolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -137,15 +137,15 @@
     async def create_compute_environment(
         self,
         *,
         computeEnvironmentName: str,
         type: CETypeType,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
-        computeResources: ComputeResourceTypeDef = ...,
+        computeResources: ComputeResourceUnionTypeDef = ...,
         serviceRole: str = ...,
         tags: Mapping[str, str] = ...,
         eksConfiguration: EksConfigurationTypeDef = ...
     ) -> CreateComputeEnvironmentResponseTypeDef:
         """
         Creates an Batch compute environment.
 
@@ -170,15 +170,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_job_queue)
         """
 
     async def create_scheduling_policy(
         self,
         *,
         name: str,
-        fairsharePolicy: FairsharePolicyTypeDef = ...,
+        fairsharePolicy: FairsharePolicyUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSchedulingPolicyResponseTypeDef:
         """
         Creates an Batch scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_scheduling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_scheduling_policy)
@@ -329,22 +329,22 @@
     async def register_job_definition(
         self,
         *,
         jobDefinitionName: str,
         type: JobDefinitionTypeType,
         parameters: Mapping[str, str] = ...,
         schedulingPriority: int = ...,
-        containerProperties: ContainerPropertiesTypeDef = ...,
-        nodeProperties: NodePropertiesTypeDef = ...,
-        retryStrategy: RetryStrategyTypeDef = ...,
+        containerProperties: ContainerPropertiesUnionTypeDef = ...,
+        nodeProperties: NodePropertiesUnionTypeDef = ...,
+        retryStrategy: RetryStrategyUnionTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         platformCapabilities: Sequence[PlatformCapabilityType] = ...,
-        eksProperties: EksPropertiesTypeDef = ...
+        eksProperties: EksPropertiesUnionTypeDef = ...
     ) -> RegisterJobDefinitionResponseTypeDef:
         """
         Registers an Batch job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.register_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#register_job_definition)
         """
@@ -358,15 +358,15 @@
         shareIdentifier: str = ...,
         schedulingPriorityOverride: int = ...,
         arrayProperties: ArrayPropertiesTypeDef = ...,
         dependsOn: Sequence[JobDependencyTypeDef] = ...,
         parameters: Mapping[str, str] = ...,
         containerOverrides: ContainerOverridesTypeDef = ...,
         nodeOverrides: NodeOverridesTypeDef = ...,
-        retryStrategy: RetryStrategyTypeDef = ...,
+        retryStrategy: RetryStrategyUnionTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...
     ) -> SubmitJobResponseTypeDef:
         """
         Submits an Batch job from a job definition.
@@ -429,15 +429,15 @@
         Updates a job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_job_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#update_job_queue)
         """
 
     async def update_scheduling_policy(
-        self, *, arn: str, fairsharePolicy: FairsharePolicyTypeDef = ...
+        self, *, arn: str, fairsharePolicy: FairsharePolicyUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_scheduling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#update_scheduling_policy)
         """
```

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/client.pyi` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -34,40 +34,40 @@
     DescribeJobQueuesPaginator,
     ListJobsPaginator,
     ListSchedulingPoliciesPaginator,
 )
 from .type_defs import (
     ArrayPropertiesTypeDef,
     ComputeEnvironmentOrderTypeDef,
-    ComputeResourceTypeDef,
+    ComputeResourceUnionTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
-    ContainerPropertiesTypeDef,
+    ContainerPropertiesUnionTypeDef,
     CreateComputeEnvironmentResponseTypeDef,
     CreateJobQueueResponseTypeDef,
     CreateSchedulingPolicyResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobQueuesResponseTypeDef,
     DescribeJobsResponseTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
     EksConfigurationTypeDef,
     EksPropertiesOverrideTypeDef,
-    EksPropertiesTypeDef,
-    FairsharePolicyTypeDef,
+    EksPropertiesUnionTypeDef,
+    FairsharePolicyUnionTypeDef,
     JobDependencyTypeDef,
     JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
     ListJobsResponseTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NodeOverridesTypeDef,
-    NodePropertiesTypeDef,
+    NodePropertiesUnionTypeDef,
     RegisterJobDefinitionResponseTypeDef,
-    RetryStrategyTypeDef,
+    RetryStrategyUnionTypeDef,
     SubmitJobResponseTypeDef,
     UpdateComputeEnvironmentResponseTypeDef,
     UpdateJobQueueResponseTypeDef,
     UpdatePolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -129,15 +129,15 @@
     async def create_compute_environment(
         self,
         *,
         computeEnvironmentName: str,
         type: CETypeType,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
-        computeResources: ComputeResourceTypeDef = ...,
+        computeResources: ComputeResourceUnionTypeDef = ...,
         serviceRole: str = ...,
         tags: Mapping[str, str] = ...,
         eksConfiguration: EksConfigurationTypeDef = ...
     ) -> CreateComputeEnvironmentResponseTypeDef:
         """
         Creates an Batch compute environment.
 
@@ -160,15 +160,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_job_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_job_queue)
         """
     async def create_scheduling_policy(
         self,
         *,
         name: str,
-        fairsharePolicy: FairsharePolicyTypeDef = ...,
+        fairsharePolicy: FairsharePolicyUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSchedulingPolicyResponseTypeDef:
         """
         Creates an Batch scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_scheduling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_scheduling_policy)
@@ -305,22 +305,22 @@
     async def register_job_definition(
         self,
         *,
         jobDefinitionName: str,
         type: JobDefinitionTypeType,
         parameters: Mapping[str, str] = ...,
         schedulingPriority: int = ...,
-        containerProperties: ContainerPropertiesTypeDef = ...,
-        nodeProperties: NodePropertiesTypeDef = ...,
-        retryStrategy: RetryStrategyTypeDef = ...,
+        containerProperties: ContainerPropertiesUnionTypeDef = ...,
+        nodeProperties: NodePropertiesUnionTypeDef = ...,
+        retryStrategy: RetryStrategyUnionTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         platformCapabilities: Sequence[PlatformCapabilityType] = ...,
-        eksProperties: EksPropertiesTypeDef = ...
+        eksProperties: EksPropertiesUnionTypeDef = ...
     ) -> RegisterJobDefinitionResponseTypeDef:
         """
         Registers an Batch job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.register_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#register_job_definition)
         """
@@ -333,15 +333,15 @@
         shareIdentifier: str = ...,
         schedulingPriorityOverride: int = ...,
         arrayProperties: ArrayPropertiesTypeDef = ...,
         dependsOn: Sequence[JobDependencyTypeDef] = ...,
         parameters: Mapping[str, str] = ...,
         containerOverrides: ContainerOverridesTypeDef = ...,
         nodeOverrides: NodeOverridesTypeDef = ...,
-        retryStrategy: RetryStrategyTypeDef = ...,
+        retryStrategy: RetryStrategyUnionTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...
     ) -> SubmitJobResponseTypeDef:
         """
         Submits an Batch job from a job definition.
@@ -398,15 +398,15 @@
         """
         Updates a job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_job_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#update_job_queue)
         """
     async def update_scheduling_policy(
-        self, *, arn: str, fairsharePolicy: FairsharePolicyTypeDef = ...
+        self, *, arn: str, fairsharePolicy: FairsharePolicyUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_scheduling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#update_scheduling_policy)
         """
```

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/literals.py` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/literals.pyi` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/paginator.py` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describecomputeenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         computeEnvironments: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeComputeEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeComputeEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describecomputeenvironmentspaginator)
         """
 
 
@@ -89,30 +89,30 @@
 
     def paginate(
         self,
         *,
         jobDefinitions: Sequence[str] = ...,
         jobDefinitionName: str = ...,
         status: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describejobdefinitionspaginator)
         """
 
 
 class DescribeJobQueuesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describejobqueuespaginator)
     """
 
     def paginate(
-        self, *, jobQueues: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobQueues: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeJobQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describejobqueuespaginator)
         """
 
 
@@ -126,28 +126,28 @@
         self,
         *,
         jobQueue: str = ...,
         arrayJobId: str = ...,
         multiNodeJobId: str = ...,
         jobStatus: JobStatusType = ...,
         filters: Sequence[KeyValuesPairTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#listjobspaginator)
         """
 
 
 class ListSchedulingPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#listschedulingpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSchedulingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#listschedulingpoliciespaginator)
         """
```

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/paginator.pyi` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describecomputeenvironmentspaginator)
     """
 
     def paginate(
         self,
         *,
         computeEnvironments: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeComputeEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeComputeEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describecomputeenvironmentspaginator)
         """
 
 class DescribeJobDefinitionsPaginator(AioPaginator):
@@ -85,29 +85,29 @@
 
     def paginate(
         self,
         *,
         jobDefinitions: Sequence[str] = ...,
         jobDefinitionName: str = ...,
         status: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describejobdefinitionspaginator)
         """
 
 class DescribeJobQueuesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describejobqueuespaginator)
     """
 
     def paginate(
-        self, *, jobQueues: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, jobQueues: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeJobQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#describejobqueuespaginator)
         """
 
 class ListJobsPaginator(AioPaginator):
@@ -120,27 +120,27 @@
         self,
         *,
         jobQueue: str = ...,
         arrayJobId: str = ...,
         multiNodeJobId: str = ...,
         jobStatus: JobStatusType = ...,
         filters: Sequence[KeyValuesPairTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#listjobspaginator)
         """
 
 class ListSchedulingPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#listschedulingpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSchedulingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/paginators/#listschedulingpoliciespaginator)
         """
```

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/type_defs.py` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_batch.type_defs import ArrayPropertiesDetailTypeDef
 
-    data: ArrayPropertiesDetailTypeDef = {...}
+    data: ArrayPropertiesDetailTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ArrayJobDependencyType,
     AssignPublicIpType,
     CEStateType,
     CEStatusType,
     CETypeType,
@@ -59,111 +59,132 @@
     "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "NetworkConfigurationTypeDef",
     "ResourceRequirementTypeDef",
     "SecretTypeDef",
     "UlimitTypeDef",
     "ContainerSummaryTypeDef",
-    "CreateComputeEnvironmentResponseTypeDef",
-    "CreateJobQueueResponseTypeDef",
-    "CreateSchedulingPolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     "DeleteJobQueueRequestRequestTypeDef",
     "DeleteSchedulingPolicyRequestRequestTypeDef",
     "DeregisterJobDefinitionRequestRequestTypeDef",
-    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
-    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
     "DescribeJobDefinitionsRequestRequestTypeDef",
-    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
     "DescribeJobQueuesRequestRequestTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
+    "DeviceOutputTypeDef",
     "DeviceTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EksAttemptContainerDetailTypeDef",
     "EksContainerEnvironmentVariableTypeDef",
-    "EksContainerResourceRequirementsTypeDef",
+    "EksContainerResourceRequirementsOutputTypeDef",
     "EksContainerSecurityContextTypeDef",
     "EksContainerVolumeMountTypeDef",
+    "EksContainerResourceRequirementsTypeDef",
     "EksEmptyDirTypeDef",
     "EksHostPathTypeDef",
+    "EksMetadataOutputTypeDef",
     "EksMetadataTypeDef",
     "EksSecretTypeDef",
     "EvaluateOnExitTypeDef",
     "ShareAttributesTypeDef",
     "HostTypeDef",
     "JobTimeoutTypeDef",
     "JobDependencyTypeDef",
     "NodeDetailsTypeDef",
     "NodePropertiesSummaryTypeDef",
     "KeyValuesPairTypeDef",
+    "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
-    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "ListSchedulingPoliciesRequestRequestTypeDef",
     "SchedulingPolicyListingDetailTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "RegisterJobDefinitionResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "SubmitJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateComputeEnvironmentResponseTypeDef",
-    "UpdateJobQueueResponseTypeDef",
     "AttemptContainerDetailTypeDef",
     "CreateJobQueueRequestRequestTypeDef",
     "JobQueueDetailTypeDef",
     "UpdateJobQueueRequestRequestTypeDef",
+    "ComputeResourceOutputTypeDef",
     "ComputeResourceTypeDef",
     "ComputeResourceUpdateTypeDef",
     "ContainerOverridesTypeDef",
+    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
+    "CreateComputeEnvironmentResponseTypeDef",
+    "CreateJobQueueResponseTypeDef",
+    "CreateSchedulingPolicyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterJobDefinitionResponseTypeDef",
+    "SubmitJobResponseTypeDef",
+    "UpdateComputeEnvironmentResponseTypeDef",
+    "UpdateJobQueueResponseTypeDef",
+    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
+    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
+    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "EksAttemptDetailTypeDef",
-    "EksContainerOverrideTypeDef",
     "EksContainerDetailTypeDef",
+    "EksContainerOutputTypeDef",
+    "EksContainerOverrideTypeDef",
     "EksContainerTypeDef",
     "EksVolumeTypeDef",
+    "RetryStrategyOutputTypeDef",
     "RetryStrategyTypeDef",
+    "FairsharePolicyOutputTypeDef",
     "FairsharePolicyTypeDef",
     "JobSummaryTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
     "ListSchedulingPoliciesResponseTypeDef",
     "AttemptDetailTypeDef",
     "DescribeJobQueuesResponseTypeDef",
     "ComputeEnvironmentDetailTypeDef",
+    "ComputeResourceUnionTypeDef",
     "CreateComputeEnvironmentRequestRequestTypeDef",
     "UpdateComputeEnvironmentRequestRequestTypeDef",
     "NodePropertyOverrideTypeDef",
     "VolumeTypeDef",
     "EksPodPropertiesOverrideTypeDef",
     "EksPodPropertiesDetailTypeDef",
+    "EksPodPropertiesOutputTypeDef",
     "EksPodPropertiesTypeDef",
-    "CreateSchedulingPolicyRequestRequestTypeDef",
+    "RetryStrategyUnionTypeDef",
     "SchedulingPolicyDetailTypeDef",
+    "CreateSchedulingPolicyRequestRequestTypeDef",
+    "FairsharePolicyUnionTypeDef",
     "UpdateSchedulingPolicyRequestRequestTypeDef",
     "ListJobsResponseTypeDef",
     "DescribeComputeEnvironmentsResponseTypeDef",
     "NodeOverridesTypeDef",
     "ContainerDetailTypeDef",
+    "ContainerPropertiesOutputTypeDef",
     "ContainerPropertiesTypeDef",
     "EksPropertiesOverrideTypeDef",
     "EksPropertiesDetailTypeDef",
+    "EksPropertiesOutputTypeDef",
     "EksPropertiesTypeDef",
     "DescribeSchedulingPoliciesResponseTypeDef",
+    "NodeRangePropertyOutputTypeDef",
+    "ContainerPropertiesUnionTypeDef",
     "NodeRangePropertyTypeDef",
     "SubmitJobRequestRequestTypeDef",
+    "EksPropertiesUnionTypeDef",
+    "NodePropertiesOutputTypeDef",
     "NodePropertiesTypeDef",
     "JobDefinitionTypeDef",
     "JobDetailTypeDef",
+    "NodePropertiesUnionTypeDef",
     "RegisterJobDefinitionRequestRequestTypeDef",
     "DescribeJobDefinitionsResponseTypeDef",
     "DescribeJobsResponseTypeDef",
 )
 
 ArrayPropertiesDetailTypeDef = TypedDict(
     "ArrayPropertiesDetailTypeDef",
@@ -337,38 +358,22 @@
     {
         "exitCode": int,
         "reason": str,
     },
     total=False,
 )
 
-CreateComputeEnvironmentResponseTypeDef = TypedDict(
-    "CreateComputeEnvironmentResponseTypeDef",
-    {
-        "computeEnvironmentName": str,
-        "computeEnvironmentArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateJobQueueResponseTypeDef = TypedDict(
-    "CreateJobQueueResponseTypeDef",
-    {
-        "jobQueueName": str,
-        "jobQueueArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSchedulingPolicyResponseTypeDef = TypedDict(
-    "CreateSchedulingPolicyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteComputeEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     {
         "computeEnvironment": str,
@@ -392,65 +397,46 @@
 DeregisterJobDefinitionRequestRequestTypeDef = TypedDict(
     "DeregisterJobDefinitionRequestRequestTypeDef",
     {
         "jobDefinition": str,
     },
 )
 
-DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = TypedDict(
-    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "computeEnvironments": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeComputeEnvironmentsRequestRequestTypeDef = TypedDict(
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
     {
         "computeEnvironments": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = TypedDict(
-    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
-    {
-        "jobDefinitions": Sequence[str],
-        "jobDefinitionName": str,
-        "status": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeJobDefinitionsRequestRequestTypeDef = TypedDict(
     "DescribeJobDefinitionsRequestRequestTypeDef",
     {
         "jobDefinitions": Sequence[str],
         "maxResults": int,
         "jobDefinitionName": str,
         "status": str,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = TypedDict(
-    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
-    {
-        "jobQueues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeJobQueuesRequestRequestTypeDef = TypedDict(
     "DescribeJobQueuesRequestRequestTypeDef",
     {
         "jobQueues": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -467,25 +453,45 @@
 DescribeSchedulingPoliciesRequestRequestTypeDef = TypedDict(
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
 )
 
+_RequiredDeviceOutputTypeDef = TypedDict(
+    "_RequiredDeviceOutputTypeDef",
+    {
+        "hostPath": str,
+    },
+)
+_OptionalDeviceOutputTypeDef = TypedDict(
+    "_OptionalDeviceOutputTypeDef",
+    {
+        "containerPath": str,
+        "permissions": List[DeviceCgroupPermissionType],
+    },
+    total=False,
+)
+
+
+class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
+    pass
+
+
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceTypeDef = TypedDict(
     "_OptionalDeviceTypeDef",
     {
         "containerPath": str,
-        "permissions": List[DeviceCgroupPermissionType],
+        "permissions": Sequence[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
 
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
@@ -526,16 +532,16 @@
 
 class EksContainerEnvironmentVariableTypeDef(
     _RequiredEksContainerEnvironmentVariableTypeDef, _OptionalEksContainerEnvironmentVariableTypeDef
 ):
     pass
 
 
-EksContainerResourceRequirementsTypeDef = TypedDict(
-    "EksContainerResourceRequirementsTypeDef",
+EksContainerResourceRequirementsOutputTypeDef = TypedDict(
+    "EksContainerResourceRequirementsOutputTypeDef",
     {
         "limits": Dict[str, str],
         "requests": Dict[str, str],
     },
     total=False,
 )
 
@@ -557,14 +563,23 @@
         "name": str,
         "mountPath": str,
         "readOnly": bool,
     },
     total=False,
 )
 
+EksContainerResourceRequirementsTypeDef = TypedDict(
+    "EksContainerResourceRequirementsTypeDef",
+    {
+        "limits": Mapping[str, str],
+        "requests": Mapping[str, str],
+    },
+    total=False,
+)
+
 EksEmptyDirTypeDef = TypedDict(
     "EksEmptyDirTypeDef",
     {
         "medium": str,
         "sizeLimit": str,
     },
     total=False,
@@ -574,18 +589,26 @@
     "EksHostPathTypeDef",
     {
         "path": str,
     },
     total=False,
 )
 
+EksMetadataOutputTypeDef = TypedDict(
+    "EksMetadataOutputTypeDef",
+    {
+        "labels": Dict[str, str],
+    },
+    total=False,
+)
+
 EksMetadataTypeDef = TypedDict(
     "EksMetadataTypeDef",
     {
-        "labels": Dict[str, str],
+        "labels": Mapping[str, str],
     },
     total=False,
 )
 
 _RequiredEksSecretTypeDef = TypedDict(
     "_RequiredEksSecretTypeDef",
     {
@@ -694,42 +717,54 @@
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
 )
 
-_RequiredTmpfsTypeDef = TypedDict(
-    "_RequiredTmpfsTypeDef",
+_RequiredTmpfsOutputTypeDef = TypedDict(
+    "_RequiredTmpfsOutputTypeDef",
     {
         "containerPath": str,
         "size": int,
     },
 )
-_OptionalTmpfsTypeDef = TypedDict(
-    "_OptionalTmpfsTypeDef",
+_OptionalTmpfsOutputTypeDef = TypedDict(
+    "_OptionalTmpfsOutputTypeDef",
     {
         "mountOptions": List[str],
     },
     total=False,
 )
 
 
-class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
+class TmpfsOutputTypeDef(_RequiredTmpfsOutputTypeDef, _OptionalTmpfsOutputTypeDef):
     pass
 
 
-ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = TypedDict(
-    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
+_RequiredTmpfsTypeDef = TypedDict(
+    "_RequiredTmpfsTypeDef",
+    {
+        "containerPath": str,
+        "size": int,
+    },
+)
+_OptionalTmpfsTypeDef = TypedDict(
+    "_OptionalTmpfsTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "mountOptions": Sequence[str],
     },
     total=False,
 )
 
+
+class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
+    pass
+
+
 ListSchedulingPoliciesRequestRequestTypeDef = TypedDict(
     "ListSchedulingPoliciesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -745,63 +780,14 @@
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
-RegisterJobDefinitionResponseTypeDef = TypedDict(
-    "RegisterJobDefinitionResponseTypeDef",
-    {
-        "jobDefinitionName": str,
-        "jobDefinitionArn": str,
-        "revision": int,
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
-SubmitJobResponseTypeDef = TypedDict(
-    "SubmitJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobName": str,
-        "jobId": str,
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
@@ -818,32 +804,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateComputeEnvironmentResponseTypeDef = TypedDict(
-    "UpdateComputeEnvironmentResponseTypeDef",
-    {
-        "computeEnvironmentName": str,
-        "computeEnvironmentArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateJobQueueResponseTypeDef = TypedDict(
-    "UpdateJobQueueResponseTypeDef",
-    {
-        "jobQueueName": str,
-        "jobQueueArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttemptContainerDetailTypeDef = TypedDict(
     "AttemptContainerDetailTypeDef",
     {
         "containerInstanceArn": str,
         "taskArn": str,
         "exitCode": int,
         "reason": str,
@@ -924,14 +892,50 @@
 
 class UpdateJobQueueRequestRequestTypeDef(
     _RequiredUpdateJobQueueRequestRequestTypeDef, _OptionalUpdateJobQueueRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredComputeResourceOutputTypeDef = TypedDict(
+    "_RequiredComputeResourceOutputTypeDef",
+    {
+        "type": CRTypeType,
+        "maxvCpus": int,
+        "subnets": List[str],
+    },
+)
+_OptionalComputeResourceOutputTypeDef = TypedDict(
+    "_OptionalComputeResourceOutputTypeDef",
+    {
+        "allocationStrategy": CRAllocationStrategyType,
+        "minvCpus": int,
+        "desiredvCpus": int,
+        "instanceTypes": List[str],
+        "imageId": str,
+        "securityGroupIds": List[str],
+        "ec2KeyPair": str,
+        "instanceRole": str,
+        "tags": Dict[str, str],
+        "placementGroup": str,
+        "bidPercentage": int,
+        "spotIamFleetRole": str,
+        "launchTemplate": LaunchTemplateSpecificationTypeDef,
+        "ec2Configuration": List[Ec2ConfigurationTypeDef],
+    },
+    total=False,
+)
+
+
+class ComputeResourceOutputTypeDef(
+    _RequiredComputeResourceOutputTypeDef, _OptionalComputeResourceOutputTypeDef
+):
+    pass
+
+
 _RequiredComputeResourceTypeDef = TypedDict(
     "_RequiredComputeResourceTypeDef",
     {
         "type": CRTypeType,
         "maxvCpus": int,
         "subnets": Sequence[str],
     },
@@ -995,34 +999,166 @@
         "instanceType": str,
         "environment": Sequence[KeyValuePairTypeDef],
         "resourceRequirements": Sequence[ResourceRequirementTypeDef],
     },
     total=False,
 )
 
+_RequiredLogConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLogConfigurationOutputTypeDef",
+    {
+        "logDriver": LogDriverType,
+    },
+)
+_OptionalLogConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLogConfigurationOutputTypeDef",
+    {
+        "options": Dict[str, str],
+        "secretOptions": List[SecretTypeDef],
+    },
+    total=False,
+)
+
+
+class LogConfigurationOutputTypeDef(
+    _RequiredLogConfigurationOutputTypeDef, _OptionalLogConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredLogConfigurationTypeDef = TypedDict(
     "_RequiredLogConfigurationTypeDef",
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
     "_OptionalLogConfigurationTypeDef",
     {
-        "options": Dict[str, str],
-        "secretOptions": List[SecretTypeDef],
+        "options": Mapping[str, str],
+        "secretOptions": Sequence[SecretTypeDef],
     },
     total=False,
 )
 
 
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
 
+CreateComputeEnvironmentResponseTypeDef = TypedDict(
+    "CreateComputeEnvironmentResponseTypeDef",
+    {
+        "computeEnvironmentName": str,
+        "computeEnvironmentArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobQueueResponseTypeDef = TypedDict(
+    "CreateJobQueueResponseTypeDef",
+    {
+        "jobQueueName": str,
+        "jobQueueArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSchedulingPolicyResponseTypeDef = TypedDict(
+    "CreateSchedulingPolicyResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
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
+RegisterJobDefinitionResponseTypeDef = TypedDict(
+    "RegisterJobDefinitionResponseTypeDef",
+    {
+        "jobDefinitionName": str,
+        "jobDefinitionArn": str,
+        "revision": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitJobResponseTypeDef = TypedDict(
+    "SubmitJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobName": str,
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateComputeEnvironmentResponseTypeDef = TypedDict(
+    "UpdateComputeEnvironmentResponseTypeDef",
+    {
+        "computeEnvironmentName": str,
+        "computeEnvironmentArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateJobQueueResponseTypeDef = TypedDict(
+    "UpdateJobQueueResponseTypeDef",
+    {
+        "jobQueueName": str,
+        "jobQueueArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = TypedDict(
+    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+    {
+        "computeEnvironments": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = TypedDict(
+    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
+    {
+        "jobDefinitions": Sequence[str],
+        "jobDefinitionName": str,
+        "status": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = TypedDict(
+    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
+    {
+        "jobQueues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = TypedDict(
+    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -1052,60 +1188,88 @@
         "startedAt": int,
         "stoppedAt": int,
         "statusReason": str,
     },
     total=False,
 )
 
-EksContainerOverrideTypeDef = TypedDict(
-    "EksContainerOverrideTypeDef",
+EksContainerDetailTypeDef = TypedDict(
+    "EksContainerDetailTypeDef",
     {
+        "name": str,
         "image": str,
-        "command": Sequence[str],
-        "args": Sequence[str],
-        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
-        "resources": EksContainerResourceRequirementsTypeDef,
+        "imagePullPolicy": str,
+        "command": List[str],
+        "args": List[str],
+        "env": List[EksContainerEnvironmentVariableTypeDef],
+        "resources": EksContainerResourceRequirementsOutputTypeDef,
+        "exitCode": int,
+        "reason": str,
+        "volumeMounts": List[EksContainerVolumeMountTypeDef],
+        "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
-EksContainerDetailTypeDef = TypedDict(
-    "EksContainerDetailTypeDef",
+_RequiredEksContainerOutputTypeDef = TypedDict(
+    "_RequiredEksContainerOutputTypeDef",
     {
-        "name": str,
         "image": str,
+    },
+)
+_OptionalEksContainerOutputTypeDef = TypedDict(
+    "_OptionalEksContainerOutputTypeDef",
+    {
+        "name": str,
         "imagePullPolicy": str,
         "command": List[str],
         "args": List[str],
         "env": List[EksContainerEnvironmentVariableTypeDef],
-        "resources": EksContainerResourceRequirementsTypeDef,
-        "exitCode": int,
-        "reason": str,
+        "resources": EksContainerResourceRequirementsOutputTypeDef,
         "volumeMounts": List[EksContainerVolumeMountTypeDef],
         "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
+
+class EksContainerOutputTypeDef(
+    _RequiredEksContainerOutputTypeDef, _OptionalEksContainerOutputTypeDef
+):
+    pass
+
+
+EksContainerOverrideTypeDef = TypedDict(
+    "EksContainerOverrideTypeDef",
+    {
+        "image": str,
+        "command": Sequence[str],
+        "args": Sequence[str],
+        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
+        "resources": EksContainerResourceRequirementsTypeDef,
+    },
+    total=False,
+)
+
 _RequiredEksContainerTypeDef = TypedDict(
     "_RequiredEksContainerTypeDef",
     {
         "image": str,
     },
 )
 _OptionalEksContainerTypeDef = TypedDict(
     "_OptionalEksContainerTypeDef",
     {
         "name": str,
         "imagePullPolicy": str,
-        "command": List[str],
-        "args": List[str],
-        "env": List[EksContainerEnvironmentVariableTypeDef],
+        "command": Sequence[str],
+        "args": Sequence[str],
+        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
         "resources": EksContainerResourceRequirementsTypeDef,
-        "volumeMounts": List[EksContainerVolumeMountTypeDef],
+        "volumeMounts": Sequence[EksContainerVolumeMountTypeDef],
         "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
 
 class EksContainerTypeDef(_RequiredEksContainerTypeDef, _OptionalEksContainerTypeDef):
@@ -1129,19 +1293,38 @@
 )
 
 
 class EksVolumeTypeDef(_RequiredEksVolumeTypeDef, _OptionalEksVolumeTypeDef):
     pass
 
 
+RetryStrategyOutputTypeDef = TypedDict(
+    "RetryStrategyOutputTypeDef",
+    {
+        "attempts": int,
+        "evaluateOnExit": List[EvaluateOnExitTypeDef],
+    },
+    total=False,
+)
+
 RetryStrategyTypeDef = TypedDict(
     "RetryStrategyTypeDef",
     {
         "attempts": int,
-        "evaluateOnExit": List[EvaluateOnExitTypeDef],
+        "evaluateOnExit": Sequence[EvaluateOnExitTypeDef],
+    },
+    total=False,
+)
+
+FairsharePolicyOutputTypeDef = TypedDict(
+    "FairsharePolicyOutputTypeDef",
+    {
+        "shareDecaySeconds": int,
+        "computeReservation": int,
+        "shareDistribution": List[ShareAttributesTypeDef],
     },
     total=False,
 )
 
 FairsharePolicyTypeDef = TypedDict(
     "FairsharePolicyTypeDef",
     {
@@ -1185,15 +1368,15 @@
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "jobQueue": str,
         "arrayJobId": str,
         "multiNodeJobId": str,
         "jobStatus": JobStatusType,
         "filters": Sequence[KeyValuesPairTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
@@ -1204,33 +1387,46 @@
         "maxResults": int,
         "nextToken": str,
         "filters": Sequence[KeyValuesPairTypeDef],
     },
     total=False,
 )
 
+LinuxParametersOutputTypeDef = TypedDict(
+    "LinuxParametersOutputTypeDef",
+    {
+        "devices": List[DeviceOutputTypeDef],
+        "initProcessEnabled": bool,
+        "sharedMemorySize": int,
+        "tmpfs": List[TmpfsOutputTypeDef],
+        "maxSwap": int,
+        "swappiness": int,
+    },
+    total=False,
+)
+
 LinuxParametersTypeDef = TypedDict(
     "LinuxParametersTypeDef",
     {
-        "devices": List[DeviceTypeDef],
+        "devices": Sequence[DeviceTypeDef],
         "initProcessEnabled": bool,
         "sharedMemorySize": int,
-        "tmpfs": List[TmpfsTypeDef],
+        "tmpfs": Sequence[TmpfsTypeDef],
         "maxSwap": int,
         "swappiness": int,
     },
     total=False,
 )
 
 ListSchedulingPoliciesResponseTypeDef = TypedDict(
     "ListSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyListingDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttemptDetailTypeDef = TypedDict(
     "AttemptDetailTypeDef",
     {
         "container": AttemptContainerDetailTypeDef,
@@ -1242,15 +1438,15 @@
 )
 
 DescribeJobQueuesResponseTypeDef = TypedDict(
     "DescribeJobQueuesResponseTypeDef",
     {
         "jobQueues": List[JobQueueDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredComputeEnvironmentDetailTypeDef = TypedDict(
     "_RequiredComputeEnvironmentDetailTypeDef",
     {
         "computeEnvironmentName": str,
@@ -1263,15 +1459,15 @@
         "unmanagedvCpus": int,
         "ecsClusterArn": str,
         "tags": Dict[str, str],
         "type": CETypeType,
         "state": CEStateType,
         "status": CEStatusType,
         "statusReason": str,
-        "computeResources": ComputeResourceTypeDef,
+        "computeResources": ComputeResourceOutputTypeDef,
         "serviceRole": str,
         "updatePolicy": UpdatePolicyTypeDef,
         "eksConfiguration": EksConfigurationTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
         "uuid": str,
     },
     total=False,
@@ -1280,14 +1476,15 @@
 
 class ComputeEnvironmentDetailTypeDef(
     _RequiredComputeEnvironmentDetailTypeDef, _OptionalComputeEnvironmentDetailTypeDef
 ):
     pass
 
 
+ComputeResourceUnionTypeDef = Union[ComputeResourceTypeDef, ComputeResourceOutputTypeDef]
 _RequiredCreateComputeEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComputeEnvironmentRequestRequestTypeDef",
     {
         "computeEnvironmentName": str,
         "type": CETypeType,
     },
 )
@@ -1384,78 +1581,93 @@
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
         "containers": List[EksContainerDetailTypeDef],
         "volumes": List[EksVolumeTypeDef],
         "podName": str,
         "nodeName": str,
-        "metadata": EksMetadataTypeDef,
+        "metadata": EksMetadataOutputTypeDef,
+    },
+    total=False,
+)
+
+EksPodPropertiesOutputTypeDef = TypedDict(
+    "EksPodPropertiesOutputTypeDef",
+    {
+        "serviceAccountName": str,
+        "hostNetwork": bool,
+        "dnsPolicy": str,
+        "containers": List[EksContainerOutputTypeDef],
+        "volumes": List[EksVolumeTypeDef],
+        "metadata": EksMetadataOutputTypeDef,
     },
     total=False,
 )
 
 EksPodPropertiesTypeDef = TypedDict(
     "EksPodPropertiesTypeDef",
     {
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
-        "containers": List[EksContainerTypeDef],
-        "volumes": List[EksVolumeTypeDef],
+        "containers": Sequence[EksContainerTypeDef],
+        "volumes": Sequence[EksVolumeTypeDef],
         "metadata": EksMetadataTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSchedulingPolicyRequestRequestTypeDef",
+RetryStrategyUnionTypeDef = Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef]
+_RequiredSchedulingPolicyDetailTypeDef = TypedDict(
+    "_RequiredSchedulingPolicyDetailTypeDef",
     {
         "name": str,
+        "arn": str,
     },
 )
-_OptionalCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSchedulingPolicyRequestRequestTypeDef",
+_OptionalSchedulingPolicyDetailTypeDef = TypedDict(
+    "_OptionalSchedulingPolicyDetailTypeDef",
     {
-        "fairsharePolicy": FairsharePolicyTypeDef,
-        "tags": Mapping[str, str],
+        "fairsharePolicy": FairsharePolicyOutputTypeDef,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class CreateSchedulingPolicyRequestRequestTypeDef(
-    _RequiredCreateSchedulingPolicyRequestRequestTypeDef,
-    _OptionalCreateSchedulingPolicyRequestRequestTypeDef,
+class SchedulingPolicyDetailTypeDef(
+    _RequiredSchedulingPolicyDetailTypeDef, _OptionalSchedulingPolicyDetailTypeDef
 ):
     pass
 
 
-_RequiredSchedulingPolicyDetailTypeDef = TypedDict(
-    "_RequiredSchedulingPolicyDetailTypeDef",
+_RequiredCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSchedulingPolicyRequestRequestTypeDef",
     {
         "name": str,
-        "arn": str,
     },
 )
-_OptionalSchedulingPolicyDetailTypeDef = TypedDict(
-    "_OptionalSchedulingPolicyDetailTypeDef",
+_OptionalCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSchedulingPolicyRequestRequestTypeDef",
     {
         "fairsharePolicy": FairsharePolicyTypeDef,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class SchedulingPolicyDetailTypeDef(
-    _RequiredSchedulingPolicyDetailTypeDef, _OptionalSchedulingPolicyDetailTypeDef
+class CreateSchedulingPolicyRequestRequestTypeDef(
+    _RequiredCreateSchedulingPolicyRequestRequestTypeDef,
+    _OptionalCreateSchedulingPolicyRequestRequestTypeDef,
 ):
     pass
 
 
+FairsharePolicyUnionTypeDef = Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef]
 _RequiredUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchedulingPolicyRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
@@ -1475,24 +1687,24 @@
 
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "jobSummaryList": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComputeEnvironmentsResponseTypeDef = TypedDict(
     "DescribeComputeEnvironmentsResponseTypeDef",
     {
         "computeEnvironments": List[ComputeEnvironmentDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NodeOverridesTypeDef = TypedDict(
     "NodeOverridesTypeDef",
     {
         "numNodes": int,
@@ -1521,26 +1733,26 @@
         "reason": str,
         "containerInstanceArn": str,
         "taskArn": str,
         "logStreamName": str,
         "instanceType": str,
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "resourceRequirements": List[ResourceRequirementTypeDef],
-        "linuxParameters": LinuxParametersTypeDef,
-        "logConfiguration": LogConfigurationTypeDef,
+        "linuxParameters": LinuxParametersOutputTypeDef,
+        "logConfiguration": LogConfigurationOutputTypeDef,
         "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
-ContainerPropertiesTypeDef = TypedDict(
-    "ContainerPropertiesTypeDef",
+ContainerPropertiesOutputTypeDef = TypedDict(
+    "ContainerPropertiesOutputTypeDef",
     {
         "image": str,
         "vcpus": int,
         "memory": int,
         "command": List[str],
         "jobRoleArn": str,
         "executionRoleArn": str,
@@ -1549,17 +1761,45 @@
         "mountPoints": List[MountPointTypeDef],
         "readonlyRootFilesystem": bool,
         "privileged": bool,
         "ulimits": List[UlimitTypeDef],
         "user": str,
         "instanceType": str,
         "resourceRequirements": List[ResourceRequirementTypeDef],
+        "linuxParameters": LinuxParametersOutputTypeDef,
+        "logConfiguration": LogConfigurationOutputTypeDef,
+        "secrets": List[SecretTypeDef],
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
+        "ephemeralStorage": EphemeralStorageTypeDef,
+    },
+    total=False,
+)
+
+ContainerPropertiesTypeDef = TypedDict(
+    "ContainerPropertiesTypeDef",
+    {
+        "image": str,
+        "vcpus": int,
+        "memory": int,
+        "command": Sequence[str],
+        "jobRoleArn": str,
+        "executionRoleArn": str,
+        "volumes": Sequence[VolumeTypeDef],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "mountPoints": Sequence[MountPointTypeDef],
+        "readonlyRootFilesystem": bool,
+        "privileged": bool,
+        "ulimits": Sequence[UlimitTypeDef],
+        "user": str,
+        "instanceType": str,
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
-        "secrets": List[SecretTypeDef],
+        "secrets": Sequence[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
@@ -1575,30 +1815,62 @@
     "EksPropertiesDetailTypeDef",
     {
         "podProperties": EksPodPropertiesDetailTypeDef,
     },
     total=False,
 )
 
+EksPropertiesOutputTypeDef = TypedDict(
+    "EksPropertiesOutputTypeDef",
+    {
+        "podProperties": EksPodPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 EksPropertiesTypeDef = TypedDict(
     "EksPropertiesTypeDef",
     {
         "podProperties": EksPodPropertiesTypeDef,
     },
     total=False,
 )
 
 DescribeSchedulingPoliciesResponseTypeDef = TypedDict(
     "DescribeSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredNodeRangePropertyOutputTypeDef = TypedDict(
+    "_RequiredNodeRangePropertyOutputTypeDef",
+    {
+        "targetNodes": str,
+    },
+)
+_OptionalNodeRangePropertyOutputTypeDef = TypedDict(
+    "_OptionalNodeRangePropertyOutputTypeDef",
+    {
+        "container": ContainerPropertiesOutputTypeDef,
     },
+    total=False,
 )
 
+
+class NodeRangePropertyOutputTypeDef(
+    _RequiredNodeRangePropertyOutputTypeDef, _OptionalNodeRangePropertyOutputTypeDef
+):
+    pass
+
+
+ContainerPropertiesUnionTypeDef = Union[
+    ContainerPropertiesTypeDef, ContainerPropertiesOutputTypeDef
+]
 _RequiredNodeRangePropertyTypeDef = TypedDict(
     "_RequiredNodeRangePropertyTypeDef",
     {
         "targetNodes": str,
     },
 )
 _OptionalNodeRangePropertyTypeDef = TypedDict(
@@ -1646,20 +1918,30 @@
 
 class SubmitJobRequestRequestTypeDef(
     _RequiredSubmitJobRequestRequestTypeDef, _OptionalSubmitJobRequestRequestTypeDef
 ):
     pass
 
 
+EksPropertiesUnionTypeDef = Union[EksPropertiesTypeDef, EksPropertiesOutputTypeDef]
+NodePropertiesOutputTypeDef = TypedDict(
+    "NodePropertiesOutputTypeDef",
+    {
+        "numNodes": int,
+        "mainNode": int,
+        "nodeRangeProperties": List[NodeRangePropertyOutputTypeDef],
+    },
+)
+
 NodePropertiesTypeDef = TypedDict(
     "NodePropertiesTypeDef",
     {
         "numNodes": int,
         "mainNode": int,
-        "nodeRangeProperties": List[NodeRangePropertyTypeDef],
+        "nodeRangeProperties": Sequence[NodeRangePropertyTypeDef],
     },
 )
 
 _RequiredJobDefinitionTypeDef = TypedDict(
     "_RequiredJobDefinitionTypeDef",
     {
         "jobDefinitionName": str,
@@ -1670,22 +1952,22 @@
 )
 _OptionalJobDefinitionTypeDef = TypedDict(
     "_OptionalJobDefinitionTypeDef",
     {
         "status": str,
         "schedulingPriority": int,
         "parameters": Dict[str, str],
-        "retryStrategy": RetryStrategyTypeDef,
-        "containerProperties": ContainerPropertiesTypeDef,
+        "retryStrategy": RetryStrategyOutputTypeDef,
+        "containerProperties": ContainerPropertiesOutputTypeDef,
         "timeout": JobTimeoutTypeDef,
-        "nodeProperties": NodePropertiesTypeDef,
+        "nodeProperties": NodePropertiesOutputTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
-        "eksProperties": EksPropertiesTypeDef,
+        "eksProperties": EksPropertiesOutputTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
     },
     total=False,
 )
 
 
 class JobDefinitionTypeDef(_RequiredJobDefinitionTypeDef, _OptionalJobDefinitionTypeDef):
@@ -1708,21 +1990,21 @@
     {
         "jobArn": str,
         "shareIdentifier": str,
         "schedulingPriority": int,
         "attempts": List[AttemptDetailTypeDef],
         "statusReason": str,
         "createdAt": int,
-        "retryStrategy": RetryStrategyTypeDef,
+        "retryStrategy": RetryStrategyOutputTypeDef,
         "stoppedAt": int,
         "dependsOn": List[JobDependencyTypeDef],
         "parameters": Dict[str, str],
         "container": ContainerDetailTypeDef,
         "nodeDetails": NodeDetailsTypeDef,
-        "nodeProperties": NodePropertiesTypeDef,
+        "nodeProperties": NodePropertiesOutputTypeDef,
         "arrayProperties": ArrayPropertiesDetailTypeDef,
         "timeout": JobTimeoutTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
         "eksProperties": EksPropertiesDetailTypeDef,
         "eksAttempts": List[EksAttemptDetailTypeDef],
@@ -1733,14 +2015,15 @@
 )
 
 
 class JobDetailTypeDef(_RequiredJobDetailTypeDef, _OptionalJobDetailTypeDef):
     pass
 
 
+NodePropertiesUnionTypeDef = Union[NodePropertiesTypeDef, NodePropertiesOutputTypeDef]
 _RequiredRegisterJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterJobDefinitionRequestRequestTypeDef",
     {
         "jobDefinitionName": str,
         "type": JobDefinitionTypeType,
     },
 )
@@ -1770,18 +2053,18 @@
 
 
 DescribeJobDefinitionsResponseTypeDef = TypedDict(
     "DescribeJobDefinitionsResponseTypeDef",
     {
         "jobDefinitions": List[JobDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "jobs": List[JobDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch/type_defs.pyi` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_batch.type_defs import ArrayPropertiesDetailTypeDef
 
-    data: ArrayPropertiesDetailTypeDef = {...}
+    data: ArrayPropertiesDetailTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ArrayJobDependencyType,
     AssignPublicIpType,
     CEStateType,
     CEStatusType,
     CETypeType,
@@ -58,111 +58,132 @@
     "KeyValuePairTypeDef",
     "MountPointTypeDef",
     "NetworkConfigurationTypeDef",
     "ResourceRequirementTypeDef",
     "SecretTypeDef",
     "UlimitTypeDef",
     "ContainerSummaryTypeDef",
-    "CreateComputeEnvironmentResponseTypeDef",
-    "CreateJobQueueResponseTypeDef",
-    "CreateSchedulingPolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     "DeleteJobQueueRequestRequestTypeDef",
     "DeleteSchedulingPolicyRequestRequestTypeDef",
     "DeregisterJobDefinitionRequestRequestTypeDef",
-    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
-    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
     "DescribeJobDefinitionsRequestRequestTypeDef",
-    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
     "DescribeJobQueuesRequestRequestTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
+    "DeviceOutputTypeDef",
     "DeviceTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EksAttemptContainerDetailTypeDef",
     "EksContainerEnvironmentVariableTypeDef",
-    "EksContainerResourceRequirementsTypeDef",
+    "EksContainerResourceRequirementsOutputTypeDef",
     "EksContainerSecurityContextTypeDef",
     "EksContainerVolumeMountTypeDef",
+    "EksContainerResourceRequirementsTypeDef",
     "EksEmptyDirTypeDef",
     "EksHostPathTypeDef",
+    "EksMetadataOutputTypeDef",
     "EksMetadataTypeDef",
     "EksSecretTypeDef",
     "EvaluateOnExitTypeDef",
     "ShareAttributesTypeDef",
     "HostTypeDef",
     "JobTimeoutTypeDef",
     "JobDependencyTypeDef",
     "NodeDetailsTypeDef",
     "NodePropertiesSummaryTypeDef",
     "KeyValuesPairTypeDef",
+    "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
-    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "ListSchedulingPoliciesRequestRequestTypeDef",
     "SchedulingPolicyListingDetailTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "RegisterJobDefinitionResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "SubmitJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateComputeEnvironmentResponseTypeDef",
-    "UpdateJobQueueResponseTypeDef",
     "AttemptContainerDetailTypeDef",
     "CreateJobQueueRequestRequestTypeDef",
     "JobQueueDetailTypeDef",
     "UpdateJobQueueRequestRequestTypeDef",
+    "ComputeResourceOutputTypeDef",
     "ComputeResourceTypeDef",
     "ComputeResourceUpdateTypeDef",
     "ContainerOverridesTypeDef",
+    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
+    "CreateComputeEnvironmentResponseTypeDef",
+    "CreateJobQueueResponseTypeDef",
+    "CreateSchedulingPolicyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RegisterJobDefinitionResponseTypeDef",
+    "SubmitJobResponseTypeDef",
+    "UpdateComputeEnvironmentResponseTypeDef",
+    "UpdateJobQueueResponseTypeDef",
+    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
+    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
+    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "EksAttemptDetailTypeDef",
-    "EksContainerOverrideTypeDef",
     "EksContainerDetailTypeDef",
+    "EksContainerOutputTypeDef",
+    "EksContainerOverrideTypeDef",
     "EksContainerTypeDef",
     "EksVolumeTypeDef",
+    "RetryStrategyOutputTypeDef",
     "RetryStrategyTypeDef",
+    "FairsharePolicyOutputTypeDef",
     "FairsharePolicyTypeDef",
     "JobSummaryTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
+    "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
     "ListSchedulingPoliciesResponseTypeDef",
     "AttemptDetailTypeDef",
     "DescribeJobQueuesResponseTypeDef",
     "ComputeEnvironmentDetailTypeDef",
+    "ComputeResourceUnionTypeDef",
     "CreateComputeEnvironmentRequestRequestTypeDef",
     "UpdateComputeEnvironmentRequestRequestTypeDef",
     "NodePropertyOverrideTypeDef",
     "VolumeTypeDef",
     "EksPodPropertiesOverrideTypeDef",
     "EksPodPropertiesDetailTypeDef",
+    "EksPodPropertiesOutputTypeDef",
     "EksPodPropertiesTypeDef",
-    "CreateSchedulingPolicyRequestRequestTypeDef",
+    "RetryStrategyUnionTypeDef",
     "SchedulingPolicyDetailTypeDef",
+    "CreateSchedulingPolicyRequestRequestTypeDef",
+    "FairsharePolicyUnionTypeDef",
     "UpdateSchedulingPolicyRequestRequestTypeDef",
     "ListJobsResponseTypeDef",
     "DescribeComputeEnvironmentsResponseTypeDef",
     "NodeOverridesTypeDef",
     "ContainerDetailTypeDef",
+    "ContainerPropertiesOutputTypeDef",
     "ContainerPropertiesTypeDef",
     "EksPropertiesOverrideTypeDef",
     "EksPropertiesDetailTypeDef",
+    "EksPropertiesOutputTypeDef",
     "EksPropertiesTypeDef",
     "DescribeSchedulingPoliciesResponseTypeDef",
+    "NodeRangePropertyOutputTypeDef",
+    "ContainerPropertiesUnionTypeDef",
     "NodeRangePropertyTypeDef",
     "SubmitJobRequestRequestTypeDef",
+    "EksPropertiesUnionTypeDef",
+    "NodePropertiesOutputTypeDef",
     "NodePropertiesTypeDef",
     "JobDefinitionTypeDef",
     "JobDetailTypeDef",
+    "NodePropertiesUnionTypeDef",
     "RegisterJobDefinitionRequestRequestTypeDef",
     "DescribeJobDefinitionsResponseTypeDef",
     "DescribeJobsResponseTypeDef",
 )
 
 ArrayPropertiesDetailTypeDef = TypedDict(
     "ArrayPropertiesDetailTypeDef",
@@ -334,38 +355,22 @@
     {
         "exitCode": int,
         "reason": str,
     },
     total=False,
 )
 
-CreateComputeEnvironmentResponseTypeDef = TypedDict(
-    "CreateComputeEnvironmentResponseTypeDef",
-    {
-        "computeEnvironmentName": str,
-        "computeEnvironmentArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateJobQueueResponseTypeDef = TypedDict(
-    "CreateJobQueueResponseTypeDef",
-    {
-        "jobQueueName": str,
-        "jobQueueArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSchedulingPolicyResponseTypeDef = TypedDict(
-    "CreateSchedulingPolicyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DeleteComputeEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteComputeEnvironmentRequestRequestTypeDef",
     {
         "computeEnvironment": str,
@@ -389,65 +394,46 @@
 DeregisterJobDefinitionRequestRequestTypeDef = TypedDict(
     "DeregisterJobDefinitionRequestRequestTypeDef",
     {
         "jobDefinition": str,
     },
 )
 
-DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = TypedDict(
-    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "computeEnvironments": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeComputeEnvironmentsRequestRequestTypeDef = TypedDict(
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
     {
         "computeEnvironments": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = TypedDict(
-    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
-    {
-        "jobDefinitions": Sequence[str],
-        "jobDefinitionName": str,
-        "status": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeJobDefinitionsRequestRequestTypeDef = TypedDict(
     "DescribeJobDefinitionsRequestRequestTypeDef",
     {
         "jobDefinitions": Sequence[str],
         "maxResults": int,
         "jobDefinitionName": str,
         "status": str,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = TypedDict(
-    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
-    {
-        "jobQueues": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeJobQueuesRequestRequestTypeDef = TypedDict(
     "DescribeJobQueuesRequestRequestTypeDef",
     {
         "jobQueues": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -464,25 +450,43 @@
 DescribeSchedulingPoliciesRequestRequestTypeDef = TypedDict(
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
 )
 
+_RequiredDeviceOutputTypeDef = TypedDict(
+    "_RequiredDeviceOutputTypeDef",
+    {
+        "hostPath": str,
+    },
+)
+_OptionalDeviceOutputTypeDef = TypedDict(
+    "_OptionalDeviceOutputTypeDef",
+    {
+        "containerPath": str,
+        "permissions": List[DeviceCgroupPermissionType],
+    },
+    total=False,
+)
+
+class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
+    pass
+
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceTypeDef = TypedDict(
     "_OptionalDeviceTypeDef",
     {
         "containerPath": str,
-        "permissions": List[DeviceCgroupPermissionType],
+        "permissions": Sequence[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
@@ -519,16 +523,16 @@
 )
 
 class EksContainerEnvironmentVariableTypeDef(
     _RequiredEksContainerEnvironmentVariableTypeDef, _OptionalEksContainerEnvironmentVariableTypeDef
 ):
     pass
 
-EksContainerResourceRequirementsTypeDef = TypedDict(
-    "EksContainerResourceRequirementsTypeDef",
+EksContainerResourceRequirementsOutputTypeDef = TypedDict(
+    "EksContainerResourceRequirementsOutputTypeDef",
     {
         "limits": Dict[str, str],
         "requests": Dict[str, str],
     },
     total=False,
 )
 
@@ -550,14 +554,23 @@
         "name": str,
         "mountPath": str,
         "readOnly": bool,
     },
     total=False,
 )
 
+EksContainerResourceRequirementsTypeDef = TypedDict(
+    "EksContainerResourceRequirementsTypeDef",
+    {
+        "limits": Mapping[str, str],
+        "requests": Mapping[str, str],
+    },
+    total=False,
+)
+
 EksEmptyDirTypeDef = TypedDict(
     "EksEmptyDirTypeDef",
     {
         "medium": str,
         "sizeLimit": str,
     },
     total=False,
@@ -567,18 +580,26 @@
     "EksHostPathTypeDef",
     {
         "path": str,
     },
     total=False,
 )
 
+EksMetadataOutputTypeDef = TypedDict(
+    "EksMetadataOutputTypeDef",
+    {
+        "labels": Dict[str, str],
+    },
+    total=False,
+)
+
 EksMetadataTypeDef = TypedDict(
     "EksMetadataTypeDef",
     {
-        "labels": Dict[str, str],
+        "labels": Mapping[str, str],
     },
     total=False,
 )
 
 _RequiredEksSecretTypeDef = TypedDict(
     "_RequiredEksSecretTypeDef",
     {
@@ -681,40 +702,50 @@
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
 )
 
-_RequiredTmpfsTypeDef = TypedDict(
-    "_RequiredTmpfsTypeDef",
+_RequiredTmpfsOutputTypeDef = TypedDict(
+    "_RequiredTmpfsOutputTypeDef",
     {
         "containerPath": str,
         "size": int,
     },
 )
-_OptionalTmpfsTypeDef = TypedDict(
-    "_OptionalTmpfsTypeDef",
+_OptionalTmpfsOutputTypeDef = TypedDict(
+    "_OptionalTmpfsOutputTypeDef",
     {
         "mountOptions": List[str],
     },
     total=False,
 )
 
-class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
+class TmpfsOutputTypeDef(_RequiredTmpfsOutputTypeDef, _OptionalTmpfsOutputTypeDef):
     pass
 
-ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = TypedDict(
-    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
+_RequiredTmpfsTypeDef = TypedDict(
+    "_RequiredTmpfsTypeDef",
+    {
+        "containerPath": str,
+        "size": int,
+    },
+)
+_OptionalTmpfsTypeDef = TypedDict(
+    "_OptionalTmpfsTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "mountOptions": Sequence[str],
     },
     total=False,
 )
 
+class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
+    pass
+
 ListSchedulingPoliciesRequestRequestTypeDef = TypedDict(
     "ListSchedulingPoliciesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -730,63 +761,14 @@
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
-RegisterJobDefinitionResponseTypeDef = TypedDict(
-    "RegisterJobDefinitionResponseTypeDef",
-    {
-        "jobDefinitionName": str,
-        "jobDefinitionArn": str,
-        "revision": int,
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
-SubmitJobResponseTypeDef = TypedDict(
-    "SubmitJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobName": str,
-        "jobId": str,
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
@@ -803,32 +785,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateComputeEnvironmentResponseTypeDef = TypedDict(
-    "UpdateComputeEnvironmentResponseTypeDef",
-    {
-        "computeEnvironmentName": str,
-        "computeEnvironmentArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateJobQueueResponseTypeDef = TypedDict(
-    "UpdateJobQueueResponseTypeDef",
-    {
-        "jobQueueName": str,
-        "jobQueueArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttemptContainerDetailTypeDef = TypedDict(
     "AttemptContainerDetailTypeDef",
     {
         "containerInstanceArn": str,
         "taskArn": str,
         "exitCode": int,
         "reason": str,
@@ -903,14 +867,48 @@
 )
 
 class UpdateJobQueueRequestRequestTypeDef(
     _RequiredUpdateJobQueueRequestRequestTypeDef, _OptionalUpdateJobQueueRequestRequestTypeDef
 ):
     pass
 
+_RequiredComputeResourceOutputTypeDef = TypedDict(
+    "_RequiredComputeResourceOutputTypeDef",
+    {
+        "type": CRTypeType,
+        "maxvCpus": int,
+        "subnets": List[str],
+    },
+)
+_OptionalComputeResourceOutputTypeDef = TypedDict(
+    "_OptionalComputeResourceOutputTypeDef",
+    {
+        "allocationStrategy": CRAllocationStrategyType,
+        "minvCpus": int,
+        "desiredvCpus": int,
+        "instanceTypes": List[str],
+        "imageId": str,
+        "securityGroupIds": List[str],
+        "ec2KeyPair": str,
+        "instanceRole": str,
+        "tags": Dict[str, str],
+        "placementGroup": str,
+        "bidPercentage": int,
+        "spotIamFleetRole": str,
+        "launchTemplate": LaunchTemplateSpecificationTypeDef,
+        "ec2Configuration": List[Ec2ConfigurationTypeDef],
+    },
+    total=False,
+)
+
+class ComputeResourceOutputTypeDef(
+    _RequiredComputeResourceOutputTypeDef, _OptionalComputeResourceOutputTypeDef
+):
+    pass
+
 _RequiredComputeResourceTypeDef = TypedDict(
     "_RequiredComputeResourceTypeDef",
     {
         "type": CRTypeType,
         "maxvCpus": int,
         "subnets": Sequence[str],
     },
@@ -972,32 +970,162 @@
         "instanceType": str,
         "environment": Sequence[KeyValuePairTypeDef],
         "resourceRequirements": Sequence[ResourceRequirementTypeDef],
     },
     total=False,
 )
 
+_RequiredLogConfigurationOutputTypeDef = TypedDict(
+    "_RequiredLogConfigurationOutputTypeDef",
+    {
+        "logDriver": LogDriverType,
+    },
+)
+_OptionalLogConfigurationOutputTypeDef = TypedDict(
+    "_OptionalLogConfigurationOutputTypeDef",
+    {
+        "options": Dict[str, str],
+        "secretOptions": List[SecretTypeDef],
+    },
+    total=False,
+)
+
+class LogConfigurationOutputTypeDef(
+    _RequiredLogConfigurationOutputTypeDef, _OptionalLogConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredLogConfigurationTypeDef = TypedDict(
     "_RequiredLogConfigurationTypeDef",
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
     "_OptionalLogConfigurationTypeDef",
     {
-        "options": Dict[str, str],
-        "secretOptions": List[SecretTypeDef],
+        "options": Mapping[str, str],
+        "secretOptions": Sequence[SecretTypeDef],
     },
     total=False,
 )
 
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
+CreateComputeEnvironmentResponseTypeDef = TypedDict(
+    "CreateComputeEnvironmentResponseTypeDef",
+    {
+        "computeEnvironmentName": str,
+        "computeEnvironmentArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobQueueResponseTypeDef = TypedDict(
+    "CreateJobQueueResponseTypeDef",
+    {
+        "jobQueueName": str,
+        "jobQueueArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSchedulingPolicyResponseTypeDef = TypedDict(
+    "CreateSchedulingPolicyResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
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
+RegisterJobDefinitionResponseTypeDef = TypedDict(
+    "RegisterJobDefinitionResponseTypeDef",
+    {
+        "jobDefinitionName": str,
+        "jobDefinitionArn": str,
+        "revision": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SubmitJobResponseTypeDef = TypedDict(
+    "SubmitJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobName": str,
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateComputeEnvironmentResponseTypeDef = TypedDict(
+    "UpdateComputeEnvironmentResponseTypeDef",
+    {
+        "computeEnvironmentName": str,
+        "computeEnvironmentArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateJobQueueResponseTypeDef = TypedDict(
+    "UpdateJobQueueResponseTypeDef",
+    {
+        "jobQueueName": str,
+        "jobQueueArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef = TypedDict(
+    "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
+    {
+        "computeEnvironments": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef = TypedDict(
+    "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
+    {
+        "jobDefinitions": Sequence[str],
+        "jobDefinitionName": str,
+        "status": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef = TypedDict(
+    "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
+    {
+        "jobQueues": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef = TypedDict(
+    "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredEFSVolumeConfigurationTypeDef = TypedDict(
     "_RequiredEFSVolumeConfigurationTypeDef",
     {
         "fileSystemId": str,
     },
 )
 _OptionalEFSVolumeConfigurationTypeDef = TypedDict(
@@ -1025,60 +1153,86 @@
         "startedAt": int,
         "stoppedAt": int,
         "statusReason": str,
     },
     total=False,
 )
 
-EksContainerOverrideTypeDef = TypedDict(
-    "EksContainerOverrideTypeDef",
+EksContainerDetailTypeDef = TypedDict(
+    "EksContainerDetailTypeDef",
     {
+        "name": str,
         "image": str,
-        "command": Sequence[str],
-        "args": Sequence[str],
-        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
-        "resources": EksContainerResourceRequirementsTypeDef,
+        "imagePullPolicy": str,
+        "command": List[str],
+        "args": List[str],
+        "env": List[EksContainerEnvironmentVariableTypeDef],
+        "resources": EksContainerResourceRequirementsOutputTypeDef,
+        "exitCode": int,
+        "reason": str,
+        "volumeMounts": List[EksContainerVolumeMountTypeDef],
+        "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
-EksContainerDetailTypeDef = TypedDict(
-    "EksContainerDetailTypeDef",
+_RequiredEksContainerOutputTypeDef = TypedDict(
+    "_RequiredEksContainerOutputTypeDef",
     {
-        "name": str,
         "image": str,
+    },
+)
+_OptionalEksContainerOutputTypeDef = TypedDict(
+    "_OptionalEksContainerOutputTypeDef",
+    {
+        "name": str,
         "imagePullPolicy": str,
         "command": List[str],
         "args": List[str],
         "env": List[EksContainerEnvironmentVariableTypeDef],
-        "resources": EksContainerResourceRequirementsTypeDef,
-        "exitCode": int,
-        "reason": str,
+        "resources": EksContainerResourceRequirementsOutputTypeDef,
         "volumeMounts": List[EksContainerVolumeMountTypeDef],
         "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
+class EksContainerOutputTypeDef(
+    _RequiredEksContainerOutputTypeDef, _OptionalEksContainerOutputTypeDef
+):
+    pass
+
+EksContainerOverrideTypeDef = TypedDict(
+    "EksContainerOverrideTypeDef",
+    {
+        "image": str,
+        "command": Sequence[str],
+        "args": Sequence[str],
+        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
+        "resources": EksContainerResourceRequirementsTypeDef,
+    },
+    total=False,
+)
+
 _RequiredEksContainerTypeDef = TypedDict(
     "_RequiredEksContainerTypeDef",
     {
         "image": str,
     },
 )
 _OptionalEksContainerTypeDef = TypedDict(
     "_OptionalEksContainerTypeDef",
     {
         "name": str,
         "imagePullPolicy": str,
-        "command": List[str],
-        "args": List[str],
-        "env": List[EksContainerEnvironmentVariableTypeDef],
+        "command": Sequence[str],
+        "args": Sequence[str],
+        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
         "resources": EksContainerResourceRequirementsTypeDef,
-        "volumeMounts": List[EksContainerVolumeMountTypeDef],
+        "volumeMounts": Sequence[EksContainerVolumeMountTypeDef],
         "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
 class EksContainerTypeDef(_RequiredEksContainerTypeDef, _OptionalEksContainerTypeDef):
     pass
@@ -1098,19 +1252,38 @@
     },
     total=False,
 )
 
 class EksVolumeTypeDef(_RequiredEksVolumeTypeDef, _OptionalEksVolumeTypeDef):
     pass
 
+RetryStrategyOutputTypeDef = TypedDict(
+    "RetryStrategyOutputTypeDef",
+    {
+        "attempts": int,
+        "evaluateOnExit": List[EvaluateOnExitTypeDef],
+    },
+    total=False,
+)
+
 RetryStrategyTypeDef = TypedDict(
     "RetryStrategyTypeDef",
     {
         "attempts": int,
-        "evaluateOnExit": List[EvaluateOnExitTypeDef],
+        "evaluateOnExit": Sequence[EvaluateOnExitTypeDef],
+    },
+    total=False,
+)
+
+FairsharePolicyOutputTypeDef = TypedDict(
+    "FairsharePolicyOutputTypeDef",
+    {
+        "shareDecaySeconds": int,
+        "computeReservation": int,
+        "shareDistribution": List[ShareAttributesTypeDef],
     },
     total=False,
 )
 
 FairsharePolicyTypeDef = TypedDict(
     "FairsharePolicyTypeDef",
     {
@@ -1152,15 +1325,15 @@
     "ListJobsRequestListJobsPaginateTypeDef",
     {
         "jobQueue": str,
         "arrayJobId": str,
         "multiNodeJobId": str,
         "jobStatus": JobStatusType,
         "filters": Sequence[KeyValuesPairTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
@@ -1171,33 +1344,46 @@
         "maxResults": int,
         "nextToken": str,
         "filters": Sequence[KeyValuesPairTypeDef],
     },
     total=False,
 )
 
+LinuxParametersOutputTypeDef = TypedDict(
+    "LinuxParametersOutputTypeDef",
+    {
+        "devices": List[DeviceOutputTypeDef],
+        "initProcessEnabled": bool,
+        "sharedMemorySize": int,
+        "tmpfs": List[TmpfsOutputTypeDef],
+        "maxSwap": int,
+        "swappiness": int,
+    },
+    total=False,
+)
+
 LinuxParametersTypeDef = TypedDict(
     "LinuxParametersTypeDef",
     {
-        "devices": List[DeviceTypeDef],
+        "devices": Sequence[DeviceTypeDef],
         "initProcessEnabled": bool,
         "sharedMemorySize": int,
-        "tmpfs": List[TmpfsTypeDef],
+        "tmpfs": Sequence[TmpfsTypeDef],
         "maxSwap": int,
         "swappiness": int,
     },
     total=False,
 )
 
 ListSchedulingPoliciesResponseTypeDef = TypedDict(
     "ListSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyListingDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttemptDetailTypeDef = TypedDict(
     "AttemptDetailTypeDef",
     {
         "container": AttemptContainerDetailTypeDef,
@@ -1209,15 +1395,15 @@
 )
 
 DescribeJobQueuesResponseTypeDef = TypedDict(
     "DescribeJobQueuesResponseTypeDef",
     {
         "jobQueues": List[JobQueueDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredComputeEnvironmentDetailTypeDef = TypedDict(
     "_RequiredComputeEnvironmentDetailTypeDef",
     {
         "computeEnvironmentName": str,
@@ -1230,29 +1416,30 @@
         "unmanagedvCpus": int,
         "ecsClusterArn": str,
         "tags": Dict[str, str],
         "type": CETypeType,
         "state": CEStateType,
         "status": CEStatusType,
         "statusReason": str,
-        "computeResources": ComputeResourceTypeDef,
+        "computeResources": ComputeResourceOutputTypeDef,
         "serviceRole": str,
         "updatePolicy": UpdatePolicyTypeDef,
         "eksConfiguration": EksConfigurationTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
         "uuid": str,
     },
     total=False,
 )
 
 class ComputeEnvironmentDetailTypeDef(
     _RequiredComputeEnvironmentDetailTypeDef, _OptionalComputeEnvironmentDetailTypeDef
 ):
     pass
 
+ComputeResourceUnionTypeDef = Union[ComputeResourceTypeDef, ComputeResourceOutputTypeDef]
 _RequiredCreateComputeEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComputeEnvironmentRequestRequestTypeDef",
     {
         "computeEnvironmentName": str,
         "type": CETypeType,
     },
 )
@@ -1343,74 +1530,89 @@
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
         "containers": List[EksContainerDetailTypeDef],
         "volumes": List[EksVolumeTypeDef],
         "podName": str,
         "nodeName": str,
-        "metadata": EksMetadataTypeDef,
+        "metadata": EksMetadataOutputTypeDef,
+    },
+    total=False,
+)
+
+EksPodPropertiesOutputTypeDef = TypedDict(
+    "EksPodPropertiesOutputTypeDef",
+    {
+        "serviceAccountName": str,
+        "hostNetwork": bool,
+        "dnsPolicy": str,
+        "containers": List[EksContainerOutputTypeDef],
+        "volumes": List[EksVolumeTypeDef],
+        "metadata": EksMetadataOutputTypeDef,
     },
     total=False,
 )
 
 EksPodPropertiesTypeDef = TypedDict(
     "EksPodPropertiesTypeDef",
     {
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
-        "containers": List[EksContainerTypeDef],
-        "volumes": List[EksVolumeTypeDef],
+        "containers": Sequence[EksContainerTypeDef],
+        "volumes": Sequence[EksVolumeTypeDef],
         "metadata": EksMetadataTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSchedulingPolicyRequestRequestTypeDef",
+RetryStrategyUnionTypeDef = Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef]
+_RequiredSchedulingPolicyDetailTypeDef = TypedDict(
+    "_RequiredSchedulingPolicyDetailTypeDef",
     {
         "name": str,
+        "arn": str,
     },
 )
-_OptionalCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSchedulingPolicyRequestRequestTypeDef",
+_OptionalSchedulingPolicyDetailTypeDef = TypedDict(
+    "_OptionalSchedulingPolicyDetailTypeDef",
     {
-        "fairsharePolicy": FairsharePolicyTypeDef,
-        "tags": Mapping[str, str],
+        "fairsharePolicy": FairsharePolicyOutputTypeDef,
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
-class CreateSchedulingPolicyRequestRequestTypeDef(
-    _RequiredCreateSchedulingPolicyRequestRequestTypeDef,
-    _OptionalCreateSchedulingPolicyRequestRequestTypeDef,
+class SchedulingPolicyDetailTypeDef(
+    _RequiredSchedulingPolicyDetailTypeDef, _OptionalSchedulingPolicyDetailTypeDef
 ):
     pass
 
-_RequiredSchedulingPolicyDetailTypeDef = TypedDict(
-    "_RequiredSchedulingPolicyDetailTypeDef",
+_RequiredCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSchedulingPolicyRequestRequestTypeDef",
     {
         "name": str,
-        "arn": str,
     },
 )
-_OptionalSchedulingPolicyDetailTypeDef = TypedDict(
-    "_OptionalSchedulingPolicyDetailTypeDef",
+_OptionalCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSchedulingPolicyRequestRequestTypeDef",
     {
         "fairsharePolicy": FairsharePolicyTypeDef,
-        "tags": Dict[str, str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class SchedulingPolicyDetailTypeDef(
-    _RequiredSchedulingPolicyDetailTypeDef, _OptionalSchedulingPolicyDetailTypeDef
+class CreateSchedulingPolicyRequestRequestTypeDef(
+    _RequiredCreateSchedulingPolicyRequestRequestTypeDef,
+    _OptionalCreateSchedulingPolicyRequestRequestTypeDef,
 ):
     pass
 
+FairsharePolicyUnionTypeDef = Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef]
 _RequiredUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchedulingPolicyRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
@@ -1428,24 +1630,24 @@
     pass
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "jobSummaryList": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComputeEnvironmentsResponseTypeDef = TypedDict(
     "DescribeComputeEnvironmentsResponseTypeDef",
     {
         "computeEnvironments": List[ComputeEnvironmentDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NodeOverridesTypeDef = TypedDict(
     "NodeOverridesTypeDef",
     {
         "numNodes": int,
@@ -1474,26 +1676,26 @@
         "reason": str,
         "containerInstanceArn": str,
         "taskArn": str,
         "logStreamName": str,
         "instanceType": str,
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "resourceRequirements": List[ResourceRequirementTypeDef],
-        "linuxParameters": LinuxParametersTypeDef,
-        "logConfiguration": LogConfigurationTypeDef,
+        "linuxParameters": LinuxParametersOutputTypeDef,
+        "logConfiguration": LogConfigurationOutputTypeDef,
         "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
-ContainerPropertiesTypeDef = TypedDict(
-    "ContainerPropertiesTypeDef",
+ContainerPropertiesOutputTypeDef = TypedDict(
+    "ContainerPropertiesOutputTypeDef",
     {
         "image": str,
         "vcpus": int,
         "memory": int,
         "command": List[str],
         "jobRoleArn": str,
         "executionRoleArn": str,
@@ -1502,17 +1704,45 @@
         "mountPoints": List[MountPointTypeDef],
         "readonlyRootFilesystem": bool,
         "privileged": bool,
         "ulimits": List[UlimitTypeDef],
         "user": str,
         "instanceType": str,
         "resourceRequirements": List[ResourceRequirementTypeDef],
+        "linuxParameters": LinuxParametersOutputTypeDef,
+        "logConfiguration": LogConfigurationOutputTypeDef,
+        "secrets": List[SecretTypeDef],
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
+        "ephemeralStorage": EphemeralStorageTypeDef,
+    },
+    total=False,
+)
+
+ContainerPropertiesTypeDef = TypedDict(
+    "ContainerPropertiesTypeDef",
+    {
+        "image": str,
+        "vcpus": int,
+        "memory": int,
+        "command": Sequence[str],
+        "jobRoleArn": str,
+        "executionRoleArn": str,
+        "volumes": Sequence[VolumeTypeDef],
+        "environment": Sequence[KeyValuePairTypeDef],
+        "mountPoints": Sequence[MountPointTypeDef],
+        "readonlyRootFilesystem": bool,
+        "privileged": bool,
+        "ulimits": Sequence[UlimitTypeDef],
+        "user": str,
+        "instanceType": str,
+        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
-        "secrets": List[SecretTypeDef],
+        "secrets": Sequence[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
@@ -1528,30 +1758,60 @@
     "EksPropertiesDetailTypeDef",
     {
         "podProperties": EksPodPropertiesDetailTypeDef,
     },
     total=False,
 )
 
+EksPropertiesOutputTypeDef = TypedDict(
+    "EksPropertiesOutputTypeDef",
+    {
+        "podProperties": EksPodPropertiesOutputTypeDef,
+    },
+    total=False,
+)
+
 EksPropertiesTypeDef = TypedDict(
     "EksPropertiesTypeDef",
     {
         "podProperties": EksPodPropertiesTypeDef,
     },
     total=False,
 )
 
 DescribeSchedulingPoliciesResponseTypeDef = TypedDict(
     "DescribeSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredNodeRangePropertyOutputTypeDef = TypedDict(
+    "_RequiredNodeRangePropertyOutputTypeDef",
+    {
+        "targetNodes": str,
     },
 )
+_OptionalNodeRangePropertyOutputTypeDef = TypedDict(
+    "_OptionalNodeRangePropertyOutputTypeDef",
+    {
+        "container": ContainerPropertiesOutputTypeDef,
+    },
+    total=False,
+)
 
+class NodeRangePropertyOutputTypeDef(
+    _RequiredNodeRangePropertyOutputTypeDef, _OptionalNodeRangePropertyOutputTypeDef
+):
+    pass
+
+ContainerPropertiesUnionTypeDef = Union[
+    ContainerPropertiesTypeDef, ContainerPropertiesOutputTypeDef
+]
 _RequiredNodeRangePropertyTypeDef = TypedDict(
     "_RequiredNodeRangePropertyTypeDef",
     {
         "targetNodes": str,
     },
 )
 _OptionalNodeRangePropertyTypeDef = TypedDict(
@@ -1595,20 +1855,30 @@
 )
 
 class SubmitJobRequestRequestTypeDef(
     _RequiredSubmitJobRequestRequestTypeDef, _OptionalSubmitJobRequestRequestTypeDef
 ):
     pass
 
+EksPropertiesUnionTypeDef = Union[EksPropertiesTypeDef, EksPropertiesOutputTypeDef]
+NodePropertiesOutputTypeDef = TypedDict(
+    "NodePropertiesOutputTypeDef",
+    {
+        "numNodes": int,
+        "mainNode": int,
+        "nodeRangeProperties": List[NodeRangePropertyOutputTypeDef],
+    },
+)
+
 NodePropertiesTypeDef = TypedDict(
     "NodePropertiesTypeDef",
     {
         "numNodes": int,
         "mainNode": int,
-        "nodeRangeProperties": List[NodeRangePropertyTypeDef],
+        "nodeRangeProperties": Sequence[NodeRangePropertyTypeDef],
     },
 )
 
 _RequiredJobDefinitionTypeDef = TypedDict(
     "_RequiredJobDefinitionTypeDef",
     {
         "jobDefinitionName": str,
@@ -1619,22 +1889,22 @@
 )
 _OptionalJobDefinitionTypeDef = TypedDict(
     "_OptionalJobDefinitionTypeDef",
     {
         "status": str,
         "schedulingPriority": int,
         "parameters": Dict[str, str],
-        "retryStrategy": RetryStrategyTypeDef,
-        "containerProperties": ContainerPropertiesTypeDef,
+        "retryStrategy": RetryStrategyOutputTypeDef,
+        "containerProperties": ContainerPropertiesOutputTypeDef,
         "timeout": JobTimeoutTypeDef,
-        "nodeProperties": NodePropertiesTypeDef,
+        "nodeProperties": NodePropertiesOutputTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
-        "eksProperties": EksPropertiesTypeDef,
+        "eksProperties": EksPropertiesOutputTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
     },
     total=False,
 )
 
 class JobDefinitionTypeDef(_RequiredJobDefinitionTypeDef, _OptionalJobDefinitionTypeDef):
     pass
@@ -1655,21 +1925,21 @@
     {
         "jobArn": str,
         "shareIdentifier": str,
         "schedulingPriority": int,
         "attempts": List[AttemptDetailTypeDef],
         "statusReason": str,
         "createdAt": int,
-        "retryStrategy": RetryStrategyTypeDef,
+        "retryStrategy": RetryStrategyOutputTypeDef,
         "stoppedAt": int,
         "dependsOn": List[JobDependencyTypeDef],
         "parameters": Dict[str, str],
         "container": ContainerDetailTypeDef,
         "nodeDetails": NodeDetailsTypeDef,
-        "nodeProperties": NodePropertiesTypeDef,
+        "nodeProperties": NodePropertiesOutputTypeDef,
         "arrayProperties": ArrayPropertiesDetailTypeDef,
         "timeout": JobTimeoutTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
         "eksProperties": EksPropertiesDetailTypeDef,
         "eksAttempts": List[EksAttemptDetailTypeDef],
@@ -1678,14 +1948,15 @@
     },
     total=False,
 )
 
 class JobDetailTypeDef(_RequiredJobDetailTypeDef, _OptionalJobDetailTypeDef):
     pass
 
+NodePropertiesUnionTypeDef = Union[NodePropertiesTypeDef, NodePropertiesOutputTypeDef]
 _RequiredRegisterJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterJobDefinitionRequestRequestTypeDef",
     {
         "jobDefinitionName": str,
         "type": JobDefinitionTypeType,
     },
 )
@@ -1713,18 +1984,18 @@
     pass
 
 DescribeJobDefinitionsResponseTypeDef = TypedDict(
     "DescribeJobDefinitionsResponseTypeDef",
     {
         "jobDefinitions": List[JobDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeJobsResponseTypeDef = TypedDict(
     "DescribeJobsResponseTypeDef",
     {
         "jobs": List[JobDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch.egg-info/PKG-INFO` & `types-aiobotocore-batch-2.5.2.post1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-batch
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Batch 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore batch type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-batch"></a>
 
 # types-aiobotocore-batch
 
 [![PyPI - types-aiobotocore-batch](https://img.shields.io/pypi/v/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-batch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-batch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-batch?color=blue)](https://pypistats.org/packages/types-aiobotocore-batch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-batch)](https://pepy.tech/project/types-aiobotocore-batch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Batch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
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
 [types-aiobotocore-batch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +41,15 @@
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
@@ -345,20 +312,20 @@
 )
 
 
 def check_value(value: ArrayJobDependencyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_batch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_batch.type_defs import (
     ArrayPropertiesDetailTypeDef,
     ArrayPropertiesSummaryTypeDef,
     ArrayPropertiesTypeDef,
     NetworkInterfaceTypeDef,
@@ -373,118 +340,139 @@
     KeyValuePairTypeDef,
     MountPointTypeDef,
     NetworkConfigurationTypeDef,
     ResourceRequirementTypeDef,
     SecretTypeDef,
     UlimitTypeDef,
     ContainerSummaryTypeDef,
-    CreateComputeEnvironmentResponseTypeDef,
-    CreateJobQueueResponseTypeDef,
-    CreateSchedulingPolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteComputeEnvironmentRequestRequestTypeDef,
     DeleteJobQueueRequestRequestTypeDef,
     DeleteSchedulingPolicyRequestRequestTypeDef,
     DeregisterJobDefinitionRequestRequestTypeDef,
-    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeComputeEnvironmentsRequestRequestTypeDef,
-    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
     DescribeJobDefinitionsRequestRequestTypeDef,
-    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
     DescribeJobQueuesRequestRequestTypeDef,
     DescribeJobsRequestRequestTypeDef,
     DescribeSchedulingPoliciesRequestRequestTypeDef,
+    DeviceOutputTypeDef,
     DeviceTypeDef,
     EFSAuthorizationConfigTypeDef,
     EksAttemptContainerDetailTypeDef,
     EksContainerEnvironmentVariableTypeDef,
-    EksContainerResourceRequirementsTypeDef,
+    EksContainerResourceRequirementsOutputTypeDef,
     EksContainerSecurityContextTypeDef,
     EksContainerVolumeMountTypeDef,
+    EksContainerResourceRequirementsTypeDef,
     EksEmptyDirTypeDef,
     EksHostPathTypeDef,
+    EksMetadataOutputTypeDef,
     EksMetadataTypeDef,
     EksSecretTypeDef,
     EvaluateOnExitTypeDef,
     ShareAttributesTypeDef,
     HostTypeDef,
     JobTimeoutTypeDef,
     JobDependencyTypeDef,
     NodeDetailsTypeDef,
     NodePropertiesSummaryTypeDef,
     KeyValuesPairTypeDef,
+    TmpfsOutputTypeDef,
     TmpfsTypeDef,
-    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     ListSchedulingPoliciesRequestRequestTypeDef,
     SchedulingPolicyListingDetailTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    RegisterJobDefinitionResponseTypeDef,
-    ResponseMetadataTypeDef,
-    SubmitJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TerminateJobRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateComputeEnvironmentResponseTypeDef,
-    UpdateJobQueueResponseTypeDef,
     AttemptContainerDetailTypeDef,
     CreateJobQueueRequestRequestTypeDef,
     JobQueueDetailTypeDef,
     UpdateJobQueueRequestRequestTypeDef,
+    ComputeResourceOutputTypeDef,
     ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
+    LogConfigurationOutputTypeDef,
     LogConfigurationTypeDef,
+    CreateComputeEnvironmentResponseTypeDef,
+    CreateJobQueueResponseTypeDef,
+    CreateSchedulingPolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RegisterJobDefinitionResponseTypeDef,
+    SubmitJobResponseTypeDef,
+    UpdateComputeEnvironmentResponseTypeDef,
+    UpdateJobQueueResponseTypeDef,
+    DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef,
+    DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef,
+    DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef,
+    ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef,
     EFSVolumeConfigurationTypeDef,
     EksAttemptDetailTypeDef,
-    EksContainerOverrideTypeDef,
     EksContainerDetailTypeDef,
+    EksContainerOutputTypeDef,
+    EksContainerOverrideTypeDef,
     EksContainerTypeDef,
     EksVolumeTypeDef,
+    RetryStrategyOutputTypeDef,
     RetryStrategyTypeDef,
+    FairsharePolicyOutputTypeDef,
     FairsharePolicyTypeDef,
     JobSummaryTypeDef,
     ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
+    LinuxParametersOutputTypeDef,
     LinuxParametersTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     AttemptDetailTypeDef,
     DescribeJobQueuesResponseTypeDef,
     ComputeEnvironmentDetailTypeDef,
+    ComputeResourceUnionTypeDef,
     CreateComputeEnvironmentRequestRequestTypeDef,
     UpdateComputeEnvironmentRequestRequestTypeDef,
     NodePropertyOverrideTypeDef,
     VolumeTypeDef,
     EksPodPropertiesOverrideTypeDef,
     EksPodPropertiesDetailTypeDef,
+    EksPodPropertiesOutputTypeDef,
     EksPodPropertiesTypeDef,
-    CreateSchedulingPolicyRequestRequestTypeDef,
+    RetryStrategyUnionTypeDef,
     SchedulingPolicyDetailTypeDef,
+    CreateSchedulingPolicyRequestRequestTypeDef,
+    FairsharePolicyUnionTypeDef,
     UpdateSchedulingPolicyRequestRequestTypeDef,
     ListJobsResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     NodeOverridesTypeDef,
     ContainerDetailTypeDef,
+    ContainerPropertiesOutputTypeDef,
     ContainerPropertiesTypeDef,
     EksPropertiesOverrideTypeDef,
     EksPropertiesDetailTypeDef,
+    EksPropertiesOutputTypeDef,
     EksPropertiesTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
+    NodeRangePropertyOutputTypeDef,
+    ContainerPropertiesUnionTypeDef,
     NodeRangePropertyTypeDef,
     SubmitJobRequestRequestTypeDef,
+    EksPropertiesUnionTypeDef,
+    NodePropertiesOutputTypeDef,
     NodePropertiesTypeDef,
     JobDefinitionTypeDef,
     JobDetailTypeDef,
+    NodePropertiesUnionTypeDef,
     RegisterJobDefinitionRequestRequestTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobsResponseTypeDef,
 )
 
 
-def get_structure() -> ArrayPropertiesDetailTypeDef:
+def get_value() -> ArrayPropertiesDetailTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-batch-2.5.2/types_aiobotocore_batch.egg-info/SOURCES.txt` & `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*


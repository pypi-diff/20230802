# Comparing `tmp/types-aiobotocore-elasticbeanstalk-2.5.2.tar.gz` & `tmp/types-aiobotocore-elasticbeanstalk-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elasticbeanstalk-2.5.2.tar", last modified: Sat Jul  8 01:43:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-elasticbeanstalk-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
```

## Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.tar` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.378089 types-aiobotocore-elasticbeanstalk-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-07-08 01:43:35.378089 types-aiobotocore-elasticbeanstalk-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20318 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:35.378089 types-aiobotocore-elasticbeanstalk-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.374089 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45094 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45030 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52878 2023-07-08 01:30:26.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52839 2023-07-08 01:30:26.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-07-08 01:30:25.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.378089 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-07-08 01:43:35.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-08 01:43:35.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:35.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 01:43:35.000000 types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.817593 types-aiobotocore-elasticbeanstalk-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:12.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21861 2023-08-02 14:52:14.817593 types-aiobotocore-elasticbeanstalk-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20307 2023-08-02 14:38:12.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.817593 types-aiobotocore-elasticbeanstalk-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:38:12.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.805593 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45011 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44947 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52786 2023-08-02 14:38:16.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52747 2023-08-02 14:38:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:12.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.817593 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21861 2023-08-02 14:52:14.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-02 14:52:14.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:14.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/LICENSE` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/PKG-INFO` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elasticbeanstalk
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElasticBeanstalk 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElasticBeanstalk 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore elasticbeanstalk type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore elasticbeanstalk type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elasticbeanstalk"></a>
 
 # types-aiobotocore-elasticbeanstalk
 
 [![PyPI - types-aiobotocore-elasticbeanstalk](https://img.shields.io/pypi/v/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elasticbeanstalk?color=blue)](https://pypistats.org/packages/types-aiobotocore-elasticbeanstalk)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticbeanstalk)](https://pepy.tech/project/types-aiobotocore-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticBeanstalk 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [types-aiobotocore-elasticbeanstalk docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/).
 
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
@@ -381,77 +380,70 @@
 )
 
 
 def check_value(value: ActionHistoryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elasticbeanstalk.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
     S3LocationTypeDef,
     SourceBuildInformationTypeDef,
     MaxAgeRuleTypeDef,
     MaxCountRuleTypeDef,
     ApplyEnvironmentManagedActionRequestRequestTypeDef,
-    ApplyEnvironmentManagedActionResultTypeDef,
     AssociateEnvironmentOperationsRoleMessageRequestTypeDef,
     AutoScalingGroupTypeDef,
     BuildConfigurationTypeDef,
     BuilderTypeDef,
     CPUUtilizationTypeDef,
     CheckDNSAvailabilityMessageRequestTypeDef,
-    CheckDNSAvailabilityResultMessageTypeDef,
     ComposeEnvironmentsMessageRequestTypeDef,
     OptionRestrictionRegexTypeDef,
     ConfigurationOptionSettingTypeDef,
     ValidationMessageTypeDef,
     TagTypeDef,
     SourceConfigurationTypeDef,
     EnvironmentTierTypeDef,
     OptionSpecificationTypeDef,
     PlatformSummaryTypeDef,
-    CreateStorageLocationResultMessageTypeDef,
     CustomAmiTypeDef,
     DeleteApplicationMessageRequestTypeDef,
     DeleteApplicationVersionMessageRequestTypeDef,
     DeleteConfigurationTemplateMessageRequestTypeDef,
     DeleteEnvironmentConfigurationMessageRequestTypeDef,
     DeletePlatformVersionRequestRequestTypeDef,
     DeploymentTypeDef,
-    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeApplicationVersionsMessageRequestTypeDef,
     DescribeApplicationsMessageRequestTypeDef,
     DescribeConfigurationSettingsMessageRequestTypeDef,
     DescribeEnvironmentHealthRequestRequestTypeDef,
     InstanceHealthSummaryTypeDef,
-    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef,
     ManagedActionHistoryItemTypeDef,
     DescribeEnvironmentManagedActionsRequestRequestTypeDef,
     ManagedActionTypeDef,
     DescribeEnvironmentResourcesMessageRequestTypeDef,
-    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
+    TimestampTypeDef,
     WaiterConfigTypeDef,
-    DescribeEnvironmentsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnvironmentLinkTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateTypeDef,
     LoadBalancerTypeDef,
     QueueTypeDef,
@@ -459,33 +451,35 @@
     EventDescriptionTypeDef,
     SolutionStackDescriptionTypeDef,
     SearchFilterTypeDef,
     PlatformBranchSummaryTypeDef,
     PlatformFilterTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ListenerTypeDef,
-    PaginatorConfigTypeDef,
     PlatformFrameworkTypeDef,
     PlatformProgrammingLanguageTypeDef,
     RebuildEnvironmentMessageRequestTypeDef,
     RequestEnvironmentInfoMessageRequestTypeDef,
     ResourceQuotaTypeDef,
-    ResponseMetadataTypeDef,
     RestartAppServerMessageRequestTypeDef,
     RetrieveEnvironmentInfoMessageRequestTypeDef,
     SwapEnvironmentCNAMEsMessageRequestTypeDef,
     TerminateEnvironmentMessageRequestTypeDef,
     UpdateApplicationMessageRequestTypeDef,
     UpdateApplicationVersionMessageRequestTypeDef,
+    ApplyEnvironmentManagedActionResultTypeDef,
+    CheckDNSAvailabilityResultMessageTypeDef,
+    CreateStorageLocationResultMessageTypeDef,
+    EmptyResponseMetadataTypeDef,
     ApplicationMetricsTypeDef,
     ApplicationVersionDescriptionTypeDef,
     ApplicationVersionLifecycleConfigTypeDef,
     SystemStatusTypeDef,
     ConfigurationOptionDescriptionTypeDef,
-    ConfigurationSettingsDescriptionResponseMetadataTypeDef,
+    ConfigurationSettingsDescriptionResponseTypeDef,
     ConfigurationSettingsDescriptionTypeDef,
     ValidateConfigurationSettingsMessageRequestTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
     CreateApplicationVersionMessageRequestTypeDef,
     CreatePlatformVersionRequestRequestTypeDef,
     ResourceTagsDescriptionMessageTypeDef,
     UpdateTagsForResourceMessageRequestTypeDef,
@@ -493,16 +487,22 @@
     CreateEnvironmentMessageRequestTypeDef,
     DescribeConfigurationOptionsMessageRequestTypeDef,
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
     ListPlatformVersionsResultTypeDef,
+    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
+    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
+    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
+    DescribeEnvironmentsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
     DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     EnvironmentResourceDescriptionTypeDef,
     EventDescriptionsMessageTypeDef,
     ListAvailableSolutionStacksResultMessageTypeDef,
@@ -525,23 +525,23 @@
     DescribePlatformVersionResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     ApplicationDescriptionTypeDef,
     ApplicationResourceLifecycleDescriptionMessageTypeDef,
     CreateApplicationMessageRequestTypeDef,
     UpdateApplicationResourceLifecycleMessageRequestTypeDef,
     DescribeInstancesHealthResultTypeDef,
-    EnvironmentDescriptionResponseMetadataTypeDef,
+    EnvironmentDescriptionResponseTypeDef,
     EnvironmentDescriptionTypeDef,
     ApplicationDescriptionMessageTypeDef,
     ApplicationDescriptionsMessageTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
 )
 
 
-def get_structure() -> AbortEnvironmentUpdateMessageRequestTypeDef:
+def get_value() -> AbortEnvironmentUpdateMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/README.md` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-elasticbeanstalk"></a>
 
 # types-aiobotocore-elasticbeanstalk
 
 [![PyPI - types-aiobotocore-elasticbeanstalk](https://img.shields.io/pypi/v/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elasticbeanstalk?color=blue)](https://pypistats.org/packages/types-aiobotocore-elasticbeanstalk)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticbeanstalk)](https://pepy.tech/project/types-aiobotocore-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticBeanstalk 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [types-aiobotocore-elasticbeanstalk docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/).
 
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
@@ -348,77 +348,70 @@
 )
 
 
 def check_value(value: ActionHistoryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elasticbeanstalk.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
     S3LocationTypeDef,
     SourceBuildInformationTypeDef,
     MaxAgeRuleTypeDef,
     MaxCountRuleTypeDef,
     ApplyEnvironmentManagedActionRequestRequestTypeDef,
-    ApplyEnvironmentManagedActionResultTypeDef,
     AssociateEnvironmentOperationsRoleMessageRequestTypeDef,
     AutoScalingGroupTypeDef,
     BuildConfigurationTypeDef,
     BuilderTypeDef,
     CPUUtilizationTypeDef,
     CheckDNSAvailabilityMessageRequestTypeDef,
-    CheckDNSAvailabilityResultMessageTypeDef,
     ComposeEnvironmentsMessageRequestTypeDef,
     OptionRestrictionRegexTypeDef,
     ConfigurationOptionSettingTypeDef,
     ValidationMessageTypeDef,
     TagTypeDef,
     SourceConfigurationTypeDef,
     EnvironmentTierTypeDef,
     OptionSpecificationTypeDef,
     PlatformSummaryTypeDef,
-    CreateStorageLocationResultMessageTypeDef,
     CustomAmiTypeDef,
     DeleteApplicationMessageRequestTypeDef,
     DeleteApplicationVersionMessageRequestTypeDef,
     DeleteConfigurationTemplateMessageRequestTypeDef,
     DeleteEnvironmentConfigurationMessageRequestTypeDef,
     DeletePlatformVersionRequestRequestTypeDef,
     DeploymentTypeDef,
-    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeApplicationVersionsMessageRequestTypeDef,
     DescribeApplicationsMessageRequestTypeDef,
     DescribeConfigurationSettingsMessageRequestTypeDef,
     DescribeEnvironmentHealthRequestRequestTypeDef,
     InstanceHealthSummaryTypeDef,
-    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef,
     ManagedActionHistoryItemTypeDef,
     DescribeEnvironmentManagedActionsRequestRequestTypeDef,
     ManagedActionTypeDef,
     DescribeEnvironmentResourcesMessageRequestTypeDef,
-    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
+    TimestampTypeDef,
     WaiterConfigTypeDef,
-    DescribeEnvironmentsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnvironmentLinkTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateTypeDef,
     LoadBalancerTypeDef,
     QueueTypeDef,
@@ -426,33 +419,35 @@
     EventDescriptionTypeDef,
     SolutionStackDescriptionTypeDef,
     SearchFilterTypeDef,
     PlatformBranchSummaryTypeDef,
     PlatformFilterTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ListenerTypeDef,
-    PaginatorConfigTypeDef,
     PlatformFrameworkTypeDef,
     PlatformProgrammingLanguageTypeDef,
     RebuildEnvironmentMessageRequestTypeDef,
     RequestEnvironmentInfoMessageRequestTypeDef,
     ResourceQuotaTypeDef,
-    ResponseMetadataTypeDef,
     RestartAppServerMessageRequestTypeDef,
     RetrieveEnvironmentInfoMessageRequestTypeDef,
     SwapEnvironmentCNAMEsMessageRequestTypeDef,
     TerminateEnvironmentMessageRequestTypeDef,
     UpdateApplicationMessageRequestTypeDef,
     UpdateApplicationVersionMessageRequestTypeDef,
+    ApplyEnvironmentManagedActionResultTypeDef,
+    CheckDNSAvailabilityResultMessageTypeDef,
+    CreateStorageLocationResultMessageTypeDef,
+    EmptyResponseMetadataTypeDef,
     ApplicationMetricsTypeDef,
     ApplicationVersionDescriptionTypeDef,
     ApplicationVersionLifecycleConfigTypeDef,
     SystemStatusTypeDef,
     ConfigurationOptionDescriptionTypeDef,
-    ConfigurationSettingsDescriptionResponseMetadataTypeDef,
+    ConfigurationSettingsDescriptionResponseTypeDef,
     ConfigurationSettingsDescriptionTypeDef,
     ValidateConfigurationSettingsMessageRequestTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
     CreateApplicationVersionMessageRequestTypeDef,
     CreatePlatformVersionRequestRequestTypeDef,
     ResourceTagsDescriptionMessageTypeDef,
     UpdateTagsForResourceMessageRequestTypeDef,
@@ -460,16 +455,22 @@
     CreateEnvironmentMessageRequestTypeDef,
     DescribeConfigurationOptionsMessageRequestTypeDef,
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
     ListPlatformVersionsResultTypeDef,
+    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
+    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
+    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
+    DescribeEnvironmentsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
     DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     EnvironmentResourceDescriptionTypeDef,
     EventDescriptionsMessageTypeDef,
     ListAvailableSolutionStacksResultMessageTypeDef,
@@ -492,23 +493,23 @@
     DescribePlatformVersionResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     ApplicationDescriptionTypeDef,
     ApplicationResourceLifecycleDescriptionMessageTypeDef,
     CreateApplicationMessageRequestTypeDef,
     UpdateApplicationResourceLifecycleMessageRequestTypeDef,
     DescribeInstancesHealthResultTypeDef,
-    EnvironmentDescriptionResponseMetadataTypeDef,
+    EnvironmentDescriptionResponseTypeDef,
     EnvironmentDescriptionTypeDef,
     ApplicationDescriptionMessageTypeDef,
     ApplicationDescriptionsMessageTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
 )
 
 
-def get_structure() -> AbortEnvironmentUpdateMessageRequestTypeDef:
+def get_value() -> AbortEnvironmentUpdateMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/setup.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elasticbeanstalk",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_elasticbeanstalk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElasticBeanstalk 2.5.2 service generated with"
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
-    keywords="aiobotocore elasticbeanstalk type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore elasticbeanstalk type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_elasticbeanstalk": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/"
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/__init__.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/__init__.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/__main__.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticBeanstalk 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ElasticBeanstalk 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk\nOther"
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

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/client.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("elasticbeanstalk") as client:
         client: ElasticBeanstalkClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     ActionStatusType,
     EnvironmentHealthAttributeType,
@@ -43,28 +42,28 @@
     ApplicationVersionDescriptionMessageTypeDef,
     ApplicationVersionDescriptionsMessageTypeDef,
     ApplyEnvironmentManagedActionResultTypeDef,
     BuildConfigurationTypeDef,
     CheckDNSAvailabilityResultMessageTypeDef,
     ConfigurationOptionsDescriptionTypeDef,
     ConfigurationOptionSettingTypeDef,
-    ConfigurationSettingsDescriptionResponseMetadataTypeDef,
+    ConfigurationSettingsDescriptionResponseTypeDef,
     ConfigurationSettingsDescriptionsTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
     CreatePlatformVersionResultTypeDef,
     CreateStorageLocationResultMessageTypeDef,
     DeletePlatformVersionResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     DescribeEnvironmentHealthResultTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
     DescribeInstancesHealthResultTypeDef,
     DescribePlatformVersionResultTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnvironmentDescriptionResponseMetadataTypeDef,
+    EnvironmentDescriptionResponseTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
     EnvironmentResourceDescriptionsMessageTypeDef,
     EnvironmentTierTypeDef,
     EventDescriptionsMessageTypeDef,
     ListAvailableSolutionStacksResultMessageTypeDef,
     ListPlatformBranchesResultTypeDef,
     ListPlatformVersionsResultTypeDef,
@@ -73,14 +72,15 @@
     ResourceTagsDescriptionMessageTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     S3LocationTypeDef,
     SearchFilterTypeDef,
     SourceBuildInformationTypeDef,
     SourceConfigurationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import EnvironmentExistsWaiter, EnvironmentTerminatedWaiter, EnvironmentUpdatedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -253,15 +253,15 @@
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         SourceConfiguration: SourceConfigurationTypeDef = ...,
         EnvironmentId: str = ...,
         Description: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> ConfigurationSettingsDescriptionResponseMetadataTypeDef:
+    ) -> ConfigurationSettingsDescriptionResponseTypeDef:
         """
         Creates an AWS Elastic Beanstalk configuration template, associated with a
         specific Elastic Beanstalk application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#create_configuration_template)
         """
@@ -279,15 +279,15 @@
         VersionLabel: str = ...,
         TemplateName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...,
         OperationsRole: str = ...
-    ) -> EnvironmentDescriptionResponseMetadataTypeDef:
+    ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Launches an AWS Elastic Beanstalk environment for the specified application
         using the specified configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#create_environment)
         """
@@ -490,15 +490,15 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...
     ) -> EnvironmentDescriptionsMessageTypeDef:
         """
         Returns descriptions for existing environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_environments)
@@ -512,16 +512,16 @@
         VersionLabel: str = ...,
         TemplateName: str = ...,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...
     ) -> EventDescriptionsMessageTypeDef:
         """
         Returns list of event descriptions matching criteria up to the last 6 weeks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_events)
@@ -696,15 +696,15 @@
     async def terminate_environment(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         TerminateResources: bool = ...,
         ForceTerminate: bool = ...
-    ) -> EnvironmentDescriptionResponseMetadataTypeDef:
+    ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Terminates the specified environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.terminate_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#terminate_environment)
         """
 
@@ -745,15 +745,15 @@
         self,
         *,
         ApplicationName: str,
         TemplateName: str,
         Description: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...
-    ) -> ConfigurationSettingsDescriptionResponseMetadataTypeDef:
+    ) -> ConfigurationSettingsDescriptionResponseTypeDef:
         """
         Updates the specified configuration template to have the specified properties or
         configuration option values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#update_configuration_template)
         """
@@ -769,15 +769,15 @@
         Tier: EnvironmentTierTypeDef = ...,
         VersionLabel: str = ...,
         TemplateName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...
-    ) -> EnvironmentDescriptionResponseMetadataTypeDef:
+    ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Updates the environment description, deploys a new application version, updates
         the configuration settings to an entirely new configuration template, or updates
         select configuration option values in the running environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#update_environment)
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/client.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("elasticbeanstalk") as client:
         client: ElasticBeanstalkClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     ActionStatusType,
     EnvironmentHealthAttributeType,
@@ -43,28 +42,28 @@
     ApplicationVersionDescriptionMessageTypeDef,
     ApplicationVersionDescriptionsMessageTypeDef,
     ApplyEnvironmentManagedActionResultTypeDef,
     BuildConfigurationTypeDef,
     CheckDNSAvailabilityResultMessageTypeDef,
     ConfigurationOptionsDescriptionTypeDef,
     ConfigurationOptionSettingTypeDef,
-    ConfigurationSettingsDescriptionResponseMetadataTypeDef,
+    ConfigurationSettingsDescriptionResponseTypeDef,
     ConfigurationSettingsDescriptionsTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
     CreatePlatformVersionResultTypeDef,
     CreateStorageLocationResultMessageTypeDef,
     DeletePlatformVersionResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     DescribeEnvironmentHealthResultTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
     DescribeInstancesHealthResultTypeDef,
     DescribePlatformVersionResultTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnvironmentDescriptionResponseMetadataTypeDef,
+    EnvironmentDescriptionResponseTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
     EnvironmentResourceDescriptionsMessageTypeDef,
     EnvironmentTierTypeDef,
     EventDescriptionsMessageTypeDef,
     ListAvailableSolutionStacksResultMessageTypeDef,
     ListPlatformBranchesResultTypeDef,
     ListPlatformVersionsResultTypeDef,
@@ -73,14 +72,15 @@
     ResourceTagsDescriptionMessageTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     S3LocationTypeDef,
     SearchFilterTypeDef,
     SourceBuildInformationTypeDef,
     SourceConfigurationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import EnvironmentExistsWaiter, EnvironmentTerminatedWaiter, EnvironmentUpdatedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -239,15 +239,15 @@
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         SourceConfiguration: SourceConfigurationTypeDef = ...,
         EnvironmentId: str = ...,
         Description: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> ConfigurationSettingsDescriptionResponseMetadataTypeDef:
+    ) -> ConfigurationSettingsDescriptionResponseTypeDef:
         """
         Creates an AWS Elastic Beanstalk configuration template, associated with a
         specific Elastic Beanstalk application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#create_configuration_template)
         """
@@ -264,15 +264,15 @@
         VersionLabel: str = ...,
         TemplateName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...,
         OperationsRole: str = ...
-    ) -> EnvironmentDescriptionResponseMetadataTypeDef:
+    ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Launches an AWS Elastic Beanstalk environment for the specified application
         using the specified configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#create_environment)
         """
@@ -458,15 +458,15 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...
     ) -> EnvironmentDescriptionsMessageTypeDef:
         """
         Returns descriptions for existing environments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_environments)
@@ -479,16 +479,16 @@
         VersionLabel: str = ...,
         TemplateName: str = ...,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...
     ) -> EventDescriptionsMessageTypeDef:
         """
         Returns list of event descriptions matching criteria up to the last 6 weeks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.describe_events)
@@ -649,15 +649,15 @@
     async def terminate_environment(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         TerminateResources: bool = ...,
         ForceTerminate: bool = ...
-    ) -> EnvironmentDescriptionResponseMetadataTypeDef:
+    ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Terminates the specified environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.terminate_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#terminate_environment)
         """
     async def update_application(
@@ -694,15 +694,15 @@
         self,
         *,
         ApplicationName: str,
         TemplateName: str,
         Description: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...
-    ) -> ConfigurationSettingsDescriptionResponseMetadataTypeDef:
+    ) -> ConfigurationSettingsDescriptionResponseTypeDef:
         """
         Updates the specified configuration template to have the specified properties or
         configuration option values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_configuration_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#update_configuration_template)
         """
@@ -717,15 +717,15 @@
         Tier: EnvironmentTierTypeDef = ...,
         VersionLabel: str = ...,
         TemplateName: str = ...,
         SolutionStackName: str = ...,
         PlatformArn: str = ...,
         OptionSettings: Sequence[ConfigurationOptionSettingTypeDef] = ...,
         OptionsToRemove: Sequence[OptionSpecificationTypeDef] = ...
-    ) -> EnvironmentDescriptionResponseMetadataTypeDef:
+    ) -> EnvironmentDescriptionResponseTypeDef:
         """
         Updates the environment description, deploys a new application version, updates
         the configuration settings to an entirely new configuration template, or updates
         select configuration option values in the running environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/client/#update_environment)
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/literals.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/literals.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/paginator.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,29 +24,29 @@
         describe_application_versions_paginator: DescribeApplicationVersionsPaginator = client.get_paginator("describe_application_versions")
         describe_environment_managed_action_history_paginator: DescribeEnvironmentManagedActionHistoryPaginator = client.get_paginator("describe_environment_managed_action_history")
         describe_environments_paginator: DescribeEnvironmentsPaginator = client.get_paginator("describe_environments")
         describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
         list_platform_versions_paginator: ListPlatformVersionsPaginator = client.get_paginator("list_platform_versions")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import EventSeverityType
 from .type_defs import (
     ApplicationVersionDescriptionsMessageTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
     EventDescriptionsMessageTypeDef,
     ListPlatformVersionsResultTypeDef,
     PaginatorConfigTypeDef,
     PlatformFilterTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeApplicationVersionsPaginator",
     "DescribeEnvironmentManagedActionHistoryPaginator",
     "DescribeEnvironmentsPaginator",
     "DescribeEventsPaginator",
@@ -71,15 +71,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabels: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ApplicationVersionDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeApplicationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeapplicationversionspaginator)
         """
 
 
@@ -90,15 +90,15 @@
     """
 
     def paginate(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEnvironmentManagedActionHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironmentManagedActionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeenvironmentmanagedactionhistorypaginator)
         """
 
 
@@ -112,16 +112,16 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EnvironmentDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeenvironmentspaginator)
         """
 
 
@@ -138,17 +138,17 @@
         VersionLabel: str = ...,
         TemplateName: str = ...,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EventDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeeventspaginator)
         """
 
 
@@ -158,13 +158,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#listplatformversionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PlatformFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPlatformVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.ListPlatformVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#listplatformversionspaginator)
         """
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/paginator.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,29 +24,29 @@
         describe_application_versions_paginator: DescribeApplicationVersionsPaginator = client.get_paginator("describe_application_versions")
         describe_environment_managed_action_history_paginator: DescribeEnvironmentManagedActionHistoryPaginator = client.get_paginator("describe_environment_managed_action_history")
         describe_environments_paginator: DescribeEnvironmentsPaginator = client.get_paginator("describe_environments")
         describe_events_paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
         list_platform_versions_paginator: ListPlatformVersionsPaginator = client.get_paginator("list_platform_versions")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import EventSeverityType
 from .type_defs import (
     ApplicationVersionDescriptionsMessageTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
     EventDescriptionsMessageTypeDef,
     ListPlatformVersionsResultTypeDef,
     PaginatorConfigTypeDef,
     PlatformFilterTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeApplicationVersionsPaginator",
     "DescribeEnvironmentManagedActionHistoryPaginator",
     "DescribeEnvironmentsPaginator",
     "DescribeEventsPaginator",
@@ -68,15 +68,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabels: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ApplicationVersionDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeApplicationVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeapplicationversionspaginator)
         """
 
 class DescribeEnvironmentManagedActionHistoryPaginator(AioPaginator):
@@ -86,15 +86,15 @@
     """
 
     def paginate(
         self,
         *,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEnvironmentManagedActionHistoryResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironmentManagedActionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeenvironmentmanagedactionhistorypaginator)
         """
 
 class DescribeEnvironmentsPaginator(AioPaginator):
@@ -107,16 +107,16 @@
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EnvironmentDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeenvironmentspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -132,17 +132,17 @@
         VersionLabel: str = ...,
         TemplateName: str = ...,
         EnvironmentId: str = ...,
         EnvironmentName: str = ...,
         PlatformArn: str = ...,
         RequestId: str = ...,
         Severity: EventSeverityType = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[EventDescriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#describeeventspaginator)
         """
 
 class ListPlatformVersionsPaginator(AioPaginator):
@@ -151,13 +151,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#listplatformversionspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[PlatformFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPlatformVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.ListPlatformVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/paginators/#listplatformversionspaginator)
         """
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/type_defs.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_elasticbeanstalk.type_defs import AbortEnvironmentUpdateMessageRequestTypeDef
 
-    data: AbortEnvironmentUpdateMessageRequestTypeDef = {...}
+    data: AbortEnvironmentUpdateMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -38,70 +38,62 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbortEnvironmentUpdateMessageRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "LatencyTypeDef",
     "StatusCodesTypeDef",
     "S3LocationTypeDef",
     "SourceBuildInformationTypeDef",
     "MaxAgeRuleTypeDef",
     "MaxCountRuleTypeDef",
     "ApplyEnvironmentManagedActionRequestRequestTypeDef",
-    "ApplyEnvironmentManagedActionResultTypeDef",
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "BuildConfigurationTypeDef",
     "BuilderTypeDef",
     "CPUUtilizationTypeDef",
     "CheckDNSAvailabilityMessageRequestTypeDef",
-    "CheckDNSAvailabilityResultMessageTypeDef",
     "ComposeEnvironmentsMessageRequestTypeDef",
     "OptionRestrictionRegexTypeDef",
     "ConfigurationOptionSettingTypeDef",
     "ValidationMessageTypeDef",
     "TagTypeDef",
     "SourceConfigurationTypeDef",
     "EnvironmentTierTypeDef",
     "OptionSpecificationTypeDef",
     "PlatformSummaryTypeDef",
-    "CreateStorageLocationResultMessageTypeDef",
     "CustomAmiTypeDef",
     "DeleteApplicationMessageRequestTypeDef",
     "DeleteApplicationVersionMessageRequestTypeDef",
     "DeleteConfigurationTemplateMessageRequestTypeDef",
     "DeleteEnvironmentConfigurationMessageRequestTypeDef",
     "DeletePlatformVersionRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeApplicationVersionsMessageRequestTypeDef",
     "DescribeApplicationsMessageRequestTypeDef",
     "DescribeConfigurationSettingsMessageRequestTypeDef",
     "DescribeEnvironmentHealthRequestRequestTypeDef",
     "InstanceHealthSummaryTypeDef",
-    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     "ManagedActionHistoryItemTypeDef",
     "DescribeEnvironmentManagedActionsRequestRequestTypeDef",
     "ManagedActionTypeDef",
     "DescribeEnvironmentResourcesMessageRequestTypeDef",
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    "TimestampTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeEnvironmentsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
     "DescribeInstancesHealthRequestRequestTypeDef",
     "DescribePlatformVersionRequestRequestTypeDef",
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnvironmentLinkTypeDef",
     "EnvironmentInfoDescriptionTypeDef",
     "InstanceTypeDef",
     "LaunchConfigurationTypeDef",
     "LaunchTemplateTypeDef",
     "LoadBalancerTypeDef",
     "QueueTypeDef",
@@ -109,33 +101,35 @@
     "EventDescriptionTypeDef",
     "SolutionStackDescriptionTypeDef",
     "SearchFilterTypeDef",
     "PlatformBranchSummaryTypeDef",
     "PlatformFilterTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ListenerTypeDef",
-    "PaginatorConfigTypeDef",
     "PlatformFrameworkTypeDef",
     "PlatformProgrammingLanguageTypeDef",
     "RebuildEnvironmentMessageRequestTypeDef",
     "RequestEnvironmentInfoMessageRequestTypeDef",
     "ResourceQuotaTypeDef",
-    "ResponseMetadataTypeDef",
     "RestartAppServerMessageRequestTypeDef",
     "RetrieveEnvironmentInfoMessageRequestTypeDef",
     "SwapEnvironmentCNAMEsMessageRequestTypeDef",
     "TerminateEnvironmentMessageRequestTypeDef",
     "UpdateApplicationMessageRequestTypeDef",
     "UpdateApplicationVersionMessageRequestTypeDef",
+    "ApplyEnvironmentManagedActionResultTypeDef",
+    "CheckDNSAvailabilityResultMessageTypeDef",
+    "CreateStorageLocationResultMessageTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ApplicationMetricsTypeDef",
     "ApplicationVersionDescriptionTypeDef",
     "ApplicationVersionLifecycleConfigTypeDef",
     "SystemStatusTypeDef",
     "ConfigurationOptionDescriptionTypeDef",
-    "ConfigurationSettingsDescriptionResponseMetadataTypeDef",
+    "ConfigurationSettingsDescriptionResponseTypeDef",
     "ConfigurationSettingsDescriptionTypeDef",
     "ValidateConfigurationSettingsMessageRequestTypeDef",
     "ConfigurationSettingsValidationMessagesTypeDef",
     "CreateApplicationVersionMessageRequestTypeDef",
     "CreatePlatformVersionRequestRequestTypeDef",
     "ResourceTagsDescriptionMessageTypeDef",
     "UpdateTagsForResourceMessageRequestTypeDef",
@@ -143,16 +137,22 @@
     "CreateEnvironmentMessageRequestTypeDef",
     "DescribeConfigurationOptionsMessageRequestTypeDef",
     "UpdateConfigurationTemplateMessageRequestTypeDef",
     "UpdateEnvironmentMessageRequestTypeDef",
     "CreatePlatformVersionResultTypeDef",
     "DeletePlatformVersionResultTypeDef",
     "ListPlatformVersionsResultTypeDef",
+    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     "DescribeEnvironmentManagedActionsResultTypeDef",
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    "DescribeEnvironmentsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef",
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     "EnvironmentResourceDescriptionTypeDef",
     "EventDescriptionsMessageTypeDef",
     "ListAvailableSolutionStacksResultMessageTypeDef",
@@ -175,15 +175,15 @@
     "DescribePlatformVersionResultTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "ApplicationDescriptionTypeDef",
     "ApplicationResourceLifecycleDescriptionMessageTypeDef",
     "CreateApplicationMessageRequestTypeDef",
     "UpdateApplicationResourceLifecycleMessageRequestTypeDef",
     "DescribeInstancesHealthResultTypeDef",
-    "EnvironmentDescriptionResponseMetadataTypeDef",
+    "EnvironmentDescriptionResponseTypeDef",
     "EnvironmentDescriptionTypeDef",
     "ApplicationDescriptionMessageTypeDef",
     "ApplicationDescriptionsMessageTypeDef",
     "EnvironmentDescriptionsMessageTypeDef",
 )
 
 AbortEnvironmentUpdateMessageRequestTypeDef = TypedDict(
@@ -191,14 +191,25 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
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
 LatencyTypeDef = TypedDict(
     "LatencyTypeDef",
     {
         "P999": float,
         "P99": float,
         "P95": float,
         "P90": float,
@@ -250,19 +261,17 @@
     {
         "MaxAgeInDays": int,
         "DeleteSourceFromS3": bool,
     },
     total=False,
 )
 
-
 class MaxAgeRuleTypeDef(_RequiredMaxAgeRuleTypeDef, _OptionalMaxAgeRuleTypeDef):
     pass
 
-
 _RequiredMaxCountRuleTypeDef = TypedDict(
     "_RequiredMaxCountRuleTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalMaxCountRuleTypeDef = TypedDict(
@@ -270,19 +279,17 @@
     {
         "MaxCount": int,
         "DeleteSourceFromS3": bool,
     },
     total=False,
 )
 
-
 class MaxCountRuleTypeDef(_RequiredMaxCountRuleTypeDef, _OptionalMaxCountRuleTypeDef):
     pass
 
-
 _RequiredApplyEnvironmentManagedActionRequestRequestTypeDef = TypedDict(
     "_RequiredApplyEnvironmentManagedActionRequestRequestTypeDef",
     {
         "ActionId": str,
     },
 )
 _OptionalApplyEnvironmentManagedActionRequestRequestTypeDef = TypedDict(
@@ -290,33 +297,20 @@
     {
         "EnvironmentName": str,
         "EnvironmentId": str,
     },
     total=False,
 )
 
-
 class ApplyEnvironmentManagedActionRequestRequestTypeDef(
     _RequiredApplyEnvironmentManagedActionRequestRequestTypeDef,
     _OptionalApplyEnvironmentManagedActionRequestRequestTypeDef,
 ):
     pass
 
-
-ApplyEnvironmentManagedActionResultTypeDef = TypedDict(
-    "ApplyEnvironmentManagedActionResultTypeDef",
-    {
-        "ActionId": str,
-        "ActionDescription": str,
-        "ActionType": ActionTypeType,
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateEnvironmentOperationsRoleMessageRequestTypeDef = TypedDict(
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     {
         "EnvironmentName": str,
         "OperationsRole": str,
     },
 )
@@ -342,21 +336,19 @@
         "ArtifactName": str,
         "ComputeType": ComputeTypeType,
         "TimeoutInMinutes": int,
     },
     total=False,
 )
 
-
 class BuildConfigurationTypeDef(
     _RequiredBuildConfigurationTypeDef, _OptionalBuildConfigurationTypeDef
 ):
     pass
 
-
 BuilderTypeDef = TypedDict(
     "BuilderTypeDef",
     {
         "ARN": str,
     },
     total=False,
 )
@@ -379,23 +371,14 @@
 CheckDNSAvailabilityMessageRequestTypeDef = TypedDict(
     "CheckDNSAvailabilityMessageRequestTypeDef",
     {
         "CNAMEPrefix": str,
     },
 )
 
-CheckDNSAvailabilityResultMessageTypeDef = TypedDict(
-    "CheckDNSAvailabilityResultMessageTypeDef",
-    {
-        "Available": bool,
-        "FullyQualifiedCNAME": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ComposeEnvironmentsMessageRequestTypeDef = TypedDict(
     "ComposeEnvironmentsMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "GroupName": str,
         "VersionLabels": Sequence[str],
     },
@@ -486,22 +469,14 @@
         "PlatformVersion": str,
         "PlatformBranchName": str,
         "PlatformBranchLifecycleState": str,
     },
     total=False,
 )
 
-CreateStorageLocationResultMessageTypeDef = TypedDict(
-    "CreateStorageLocationResultMessageTypeDef",
-    {
-        "S3Bucket": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomAmiTypeDef = TypedDict(
     "CustomAmiTypeDef",
     {
         "VirtualizationType": str,
         "ImageId": str,
     },
     total=False,
@@ -517,21 +492,19 @@
     "_OptionalDeleteApplicationMessageRequestTypeDef",
     {
         "TerminateEnvByForce": bool,
     },
     total=False,
 )
 
-
 class DeleteApplicationMessageRequestTypeDef(
     _RequiredDeleteApplicationMessageRequestTypeDef, _OptionalDeleteApplicationMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteApplicationVersionMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteApplicationVersionMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
     },
 )
@@ -539,22 +512,20 @@
     "_OptionalDeleteApplicationVersionMessageRequestTypeDef",
     {
         "DeleteSourceBundle": bool,
     },
     total=False,
 )
 
-
 class DeleteApplicationVersionMessageRequestTypeDef(
     _RequiredDeleteApplicationVersionMessageRequestTypeDef,
     _OptionalDeleteApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
-
 DeleteConfigurationTemplateMessageRequestTypeDef = TypedDict(
     "DeleteConfigurationTemplateMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "TemplateName": str,
     },
 )
@@ -582,20 +553,20 @@
         "DeploymentId": int,
         "Status": str,
         "DeploymentTime": datetime,
     },
     total=False,
 )
 
-DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = TypedDict(
-    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ApplicationName": str,
-        "VersionLabels": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeApplicationVersionsMessageRequestTypeDef = TypedDict(
     "DescribeApplicationVersionsMessageRequestTypeDef",
     {
@@ -626,22 +597,20 @@
     {
         "TemplateName": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
-
 class DescribeConfigurationSettingsMessageRequestTypeDef(
     _RequiredDescribeConfigurationSettingsMessageRequestTypeDef,
     _OptionalDescribeConfigurationSettingsMessageRequestTypeDef,
 ):
     pass
 
-
 DescribeEnvironmentHealthRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentHealthRequestRequestTypeDef",
     {
         "EnvironmentName": str,
         "EnvironmentId": str,
         "AttributeNames": Sequence[EnvironmentHealthAttributeType],
     },
@@ -659,24 +628,14 @@
         "Warning": int,
         "Degraded": int,
         "Severe": int,
     },
     total=False,
 )
 
-DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
-    {
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
         "NextToken": str,
         "MaxItems": int,
@@ -726,89 +685,24 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
-DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "EnvironmentIds": Sequence[str],
-        "EnvironmentNames": Sequence[str],
-        "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeEnvironmentsMessageRequestTypeDef = TypedDict(
-    "DescribeEnvironmentsMessageRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "EnvironmentIds": Sequence[str],
-        "EnvironmentNames": Sequence[str],
-        "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "TemplateName": str,
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PlatformArn": str,
-        "RequestId": str,
-        "Severity": EventSeverityType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "TemplateName": str,
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PlatformArn": str,
-        "RequestId": str,
-        "Severity": EventSeverityType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 DescribeInstancesHealthRequestRequestTypeDef = TypedDict(
     "DescribeInstancesHealthRequestRequestTypeDef",
     {
         "EnvironmentName": str,
         "EnvironmentId": str,
         "AttributeNames": Sequence[InstancesHealthAttributeType],
         "NextToken": str,
@@ -827,21 +721,14 @@
 DisassociateEnvironmentOperationsRoleMessageRequestTypeDef = TypedDict(
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
     {
         "EnvironmentName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentLinkTypeDef = TypedDict(
     "EnvironmentLinkTypeDef",
     {
         "LinkName": str,
         "EnvironmentName": str,
     },
     total=False,
@@ -976,24 +863,14 @@
     {
         "Protocol": str,
         "Port": int,
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
 PlatformFrameworkTypeDef = TypedDict(
     "PlatformFrameworkTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
@@ -1028,41 +905,28 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
-
 class RequestEnvironmentInfoMessageRequestTypeDef(
     _RequiredRequestEnvironmentInfoMessageRequestTypeDef,
     _OptionalRequestEnvironmentInfoMessageRequestTypeDef,
 ):
     pass
 
-
 ResourceQuotaTypeDef = TypedDict(
     "ResourceQuotaTypeDef",
     {
         "Maximum": int,
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
 RestartAppServerMessageRequestTypeDef = TypedDict(
     "RestartAppServerMessageRequestTypeDef",
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
@@ -1079,22 +943,20 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
-
 class RetrieveEnvironmentInfoMessageRequestTypeDef(
     _RequiredRetrieveEnvironmentInfoMessageRequestTypeDef,
     _OptionalRetrieveEnvironmentInfoMessageRequestTypeDef,
 ):
     pass
 
-
 SwapEnvironmentCNAMEsMessageRequestTypeDef = TypedDict(
     "SwapEnvironmentCNAMEsMessageRequestTypeDef",
     {
         "SourceEnvironmentId": str,
         "SourceEnvironmentName": str,
         "DestinationEnvironmentId": str,
         "DestinationEnvironmentName": str,
@@ -1123,21 +985,19 @@
     "_OptionalUpdateApplicationMessageRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateApplicationMessageRequestTypeDef(
     _RequiredUpdateApplicationMessageRequestTypeDef, _OptionalUpdateApplicationMessageRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateApplicationVersionMessageRequestTypeDef = TypedDict(
     "_RequiredUpdateApplicationVersionMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
     },
 )
@@ -1145,21 +1005,54 @@
     "_OptionalUpdateApplicationVersionMessageRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateApplicationVersionMessageRequestTypeDef(
     _RequiredUpdateApplicationVersionMessageRequestTypeDef,
     _OptionalUpdateApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
+ApplyEnvironmentManagedActionResultTypeDef = TypedDict(
+    "ApplyEnvironmentManagedActionResultTypeDef",
+    {
+        "ActionId": str,
+        "ActionDescription": str,
+        "ActionType": ActionTypeType,
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CheckDNSAvailabilityResultMessageTypeDef = TypedDict(
+    "CheckDNSAvailabilityResultMessageTypeDef",
+    {
+        "Available": bool,
+        "FullyQualifiedCNAME": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStorageLocationResultMessageTypeDef = TypedDict(
+    "CreateStorageLocationResultMessageTypeDef",
+    {
+        "S3Bucket": str,
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
 
 ApplicationMetricsTypeDef = TypedDict(
     "ApplicationMetricsTypeDef",
     {
         "Duration": int,
         "RequestCount": int,
         "StatusCodes": StatusCodesTypeDef,
@@ -1217,28 +1110,28 @@
         "MaxValue": int,
         "MaxLength": int,
         "Regex": OptionRestrictionRegexTypeDef,
     },
     total=False,
 )
 
-ConfigurationSettingsDescriptionResponseMetadataTypeDef = TypedDict(
-    "ConfigurationSettingsDescriptionResponseMetadataTypeDef",
+ConfigurationSettingsDescriptionResponseTypeDef = TypedDict(
+    "ConfigurationSettingsDescriptionResponseTypeDef",
     {
         "SolutionStackName": str,
         "PlatformArn": str,
         "ApplicationName": str,
         "TemplateName": str,
         "Description": str,
         "EnvironmentName": str,
         "DeploymentStatus": ConfigurationDeploymentStatusType,
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "OptionSettings": List[ConfigurationOptionSettingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationSettingsDescriptionTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionTypeDef",
     {
         "SolutionStackName": str,
@@ -1267,27 +1160,25 @@
     {
         "TemplateName": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
-
 class ValidateConfigurationSettingsMessageRequestTypeDef(
     _RequiredValidateConfigurationSettingsMessageRequestTypeDef,
     _OptionalValidateConfigurationSettingsMessageRequestTypeDef,
 ):
     pass
 
-
 ConfigurationSettingsValidationMessagesTypeDef = TypedDict(
     "ConfigurationSettingsValidationMessagesTypeDef",
     {
         "Messages": List[ValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateApplicationVersionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationVersionMessageRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1304,22 +1195,20 @@
         "AutoCreateApplication": bool,
         "Process": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateApplicationVersionMessageRequestTypeDef(
     _RequiredCreateApplicationVersionMessageRequestTypeDef,
     _OptionalCreateApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreatePlatformVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlatformVersionRequestRequestTypeDef",
     {
         "PlatformName": str,
         "PlatformVersion": str,
         "PlatformDefinitionBundle": S3LocationTypeDef,
     },
@@ -1330,28 +1219,26 @@
         "EnvironmentName": str,
         "OptionSettings": Sequence[ConfigurationOptionSettingTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePlatformVersionRequestRequestTypeDef(
     _RequiredCreatePlatformVersionRequestRequestTypeDef,
     _OptionalCreatePlatformVersionRequestRequestTypeDef,
 ):
     pass
 
-
 ResourceTagsDescriptionMessageTypeDef = TypedDict(
     "ResourceTagsDescriptionMessageTypeDef",
     {
         "ResourceArn": str,
         "ResourceTags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
     "_RequiredUpdateTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1362,22 +1249,20 @@
     {
         "TagsToAdd": Sequence[TagTypeDef],
         "TagsToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateTagsForResourceMessageRequestTypeDef(
     _RequiredUpdateTagsForResourceMessageRequestTypeDef,
     _OptionalUpdateTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateConfigurationTemplateMessageRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationTemplateMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "TemplateName": str,
     },
 )
@@ -1391,22 +1276,20 @@
         "Description": str,
         "OptionSettings": Sequence[ConfigurationOptionSettingTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateConfigurationTemplateMessageRequestTypeDef(
     _RequiredCreateConfigurationTemplateMessageRequestTypeDef,
     _OptionalCreateConfigurationTemplateMessageRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateEnvironmentMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentMessageRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 _OptionalCreateEnvironmentMessageRequestTypeDef = TypedDict(
@@ -1425,21 +1308,19 @@
         "OptionSettings": Sequence[ConfigurationOptionSettingTypeDef],
         "OptionsToRemove": Sequence[OptionSpecificationTypeDef],
         "OperationsRole": str,
     },
     total=False,
 )
 
-
 class CreateEnvironmentMessageRequestTypeDef(
     _RequiredCreateEnvironmentMessageRequestTypeDef, _OptionalCreateEnvironmentMessageRequestTypeDef
 ):
     pass
 
-
 DescribeConfigurationOptionsMessageRequestTypeDef = TypedDict(
     "DescribeConfigurationOptionsMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "TemplateName": str,
         "EnvironmentName": str,
         "SolutionStackName": str,
@@ -1462,22 +1343,20 @@
         "Description": str,
         "OptionSettings": Sequence[ConfigurationOptionSettingTypeDef],
         "OptionsToRemove": Sequence[OptionSpecificationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateConfigurationTemplateMessageRequestTypeDef(
     _RequiredUpdateConfigurationTemplateMessageRequestTypeDef,
     _OptionalUpdateConfigurationTemplateMessageRequestTypeDef,
 ):
     pass
 
-
 UpdateEnvironmentMessageRequestTypeDef = TypedDict(
     "UpdateEnvironmentMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "EnvironmentId": str,
         "EnvironmentName": str,
         "GroupName": str,
@@ -1494,61 +1373,147 @@
 )
 
 CreatePlatformVersionResultTypeDef = TypedDict(
     "CreatePlatformVersionResultTypeDef",
     {
         "PlatformSummary": PlatformSummaryTypeDef,
         "Builder": BuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePlatformVersionResultTypeDef = TypedDict(
     "DeletePlatformVersionResultTypeDef",
     {
         "PlatformSummary": PlatformSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformVersionsResultTypeDef = TypedDict(
     "ListPlatformVersionsResultTypeDef",
     {
         "PlatformSummaryList": List[PlatformSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = TypedDict(
+    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabels": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
+    {
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeEnvironmentManagedActionHistoryResultTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     {
         "ManagedActionHistoryItems": List[ManagedActionHistoryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEnvironmentManagedActionsResultTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionsResultTypeDef",
     {
         "ManagedActions": List[ManagedActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "EnvironmentIds": Sequence[str],
+        "EnvironmentNames": Sequence[str],
+        "IncludeDeleted": bool,
+        "IncludedDeletedBackTo": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEnvironmentsMessageRequestTypeDef = TypedDict(
+    "DescribeEnvironmentsMessageRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "EnvironmentIds": Sequence[str],
+        "EnvironmentNames": Sequence[str],
+        "IncludeDeleted": bool,
+        "IncludedDeletedBackTo": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "TemplateName": str,
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PlatformArn": str,
+        "RequestId": str,
+        "Severity": EventSeverityType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "TemplateName": str,
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PlatformArn": str,
+        "RequestId": str,
+        "Severity": EventSeverityType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
     },
+    total=False,
 )
 
 DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef = TypedDict(
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "MaxRecords": int,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
@@ -1556,15 +1521,15 @@
     "DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "MaxRecords": int,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
@@ -1572,27 +1537,27 @@
     "DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "MaxRecords": int,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 RetrieveEnvironmentInfoResultMessageTypeDef = TypedDict(
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     {
         "EnvironmentInfo": List[EnvironmentInfoDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentResourceDescriptionTypeDef = TypedDict(
     "EnvironmentResourceDescriptionTypeDef",
     {
         "EnvironmentName": str,
@@ -1608,24 +1573,24 @@
 )
 
 EventDescriptionsMessageTypeDef = TypedDict(
     "EventDescriptionsMessageTypeDef",
     {
         "Events": List[EventDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAvailableSolutionStacksResultMessageTypeDef = TypedDict(
     "ListAvailableSolutionStacksResultMessageTypeDef",
     {
         "SolutionStacks": List[str],
         "SolutionStackDetails": List[SolutionStackDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformBranchesRequestRequestTypeDef = TypedDict(
     "ListPlatformBranchesRequestRequestTypeDef",
     {
         "Filters": Sequence[SearchFilterTypeDef],
@@ -1636,23 +1601,23 @@
 )
 
 ListPlatformBranchesResultTypeDef = TypedDict(
     "ListPlatformBranchesResultTypeDef",
     {
         "PlatformBranchSummaryList": List[PlatformBranchSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef = TypedDict(
     "ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef",
     {
         "Filters": Sequence[PlatformFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPlatformVersionsRequestRequestTypeDef = TypedDict(
     "ListPlatformVersionsRequestRequestTypeDef",
     {
@@ -1720,32 +1685,32 @@
         "HealthStatus": str,
         "Status": EnvironmentHealthType,
         "Color": str,
         "Causes": List[str],
         "ApplicationMetrics": ApplicationMetricsTypeDef,
         "InstancesHealth": InstanceHealthSummaryTypeDef,
         "RefreshedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationVersionDescriptionMessageTypeDef = TypedDict(
     "ApplicationVersionDescriptionMessageTypeDef",
     {
         "ApplicationVersion": ApplicationVersionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationVersionDescriptionsMessageTypeDef = TypedDict(
     "ApplicationVersionDescriptionsMessageTypeDef",
     {
         "ApplicationVersions": List[ApplicationVersionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationResourceLifecycleConfigTypeDef = TypedDict(
     "ApplicationResourceLifecycleConfigTypeDef",
     {
         "ServiceRole": str,
@@ -1773,31 +1738,31 @@
 
 ConfigurationOptionsDescriptionTypeDef = TypedDict(
     "ConfigurationOptionsDescriptionTypeDef",
     {
         "SolutionStackName": str,
         "PlatformArn": str,
         "Options": List[ConfigurationOptionDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationSettingsDescriptionsTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionsTypeDef",
     {
         "ConfigurationSettings": List[ConfigurationSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentResourceDescriptionsMessageTypeDef = TypedDict(
     "EnvironmentResourceDescriptionsMessageTypeDef",
     {
         "EnvironmentResources": EnvironmentResourceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentResourcesDescriptionTypeDef = TypedDict(
     "EnvironmentResourcesDescriptionTypeDef",
     {
         "LoadBalancer": LoadBalancerDescriptionTypeDef,
@@ -1805,23 +1770,23 @@
     total=False,
 )
 
 DescribePlatformVersionResultTypeDef = TypedDict(
     "DescribePlatformVersionResultTypeDef",
     {
         "PlatformDescription": PlatformDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "ResourceQuotas": ResourceQuotasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationDescriptionTypeDef = TypedDict(
     "ApplicationDescriptionTypeDef",
     {
         "ApplicationArn": str,
@@ -1837,15 +1802,15 @@
 )
 
 ApplicationResourceLifecycleDescriptionMessageTypeDef = TypedDict(
     "ApplicationResourceLifecycleDescriptionMessageTypeDef",
     {
         "ApplicationName": str,
         "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateApplicationMessageRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationMessageRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1857,41 +1822,39 @@
         "Description": str,
         "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateApplicationMessageRequestTypeDef(
     _RequiredCreateApplicationMessageRequestTypeDef, _OptionalCreateApplicationMessageRequestTypeDef
 ):
     pass
 
-
 UpdateApplicationResourceLifecycleMessageRequestTypeDef = TypedDict(
     "UpdateApplicationResourceLifecycleMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
     },
 )
 
 DescribeInstancesHealthResultTypeDef = TypedDict(
     "DescribeInstancesHealthResultTypeDef",
     {
         "InstanceHealthList": List[SingleInstanceHealthTypeDef],
         "RefreshedAt": datetime,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EnvironmentDescriptionResponseMetadataTypeDef = TypedDict(
-    "EnvironmentDescriptionResponseMetadataTypeDef",
+EnvironmentDescriptionResponseTypeDef = TypedDict(
+    "EnvironmentDescriptionResponseTypeDef",
     {
         "EnvironmentName": str,
         "EnvironmentId": str,
         "ApplicationName": str,
         "VersionLabel": str,
         "SolutionStackName": str,
         "PlatformArn": str,
@@ -1906,15 +1869,15 @@
         "Health": EnvironmentHealthType,
         "HealthStatus": EnvironmentHealthStatusType,
         "Resources": EnvironmentResourcesDescriptionTypeDef,
         "Tier": EnvironmentTierTypeDef,
         "EnvironmentLinks": List[EnvironmentLinkTypeDef],
         "EnvironmentArn": str,
         "OperationsRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentDescriptionTypeDef = TypedDict(
     "EnvironmentDescriptionTypeDef",
     {
         "EnvironmentName": str,
@@ -1942,27 +1905,27 @@
     total=False,
 )
 
 ApplicationDescriptionMessageTypeDef = TypedDict(
     "ApplicationDescriptionMessageTypeDef",
     {
         "Application": ApplicationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationDescriptionsMessageTypeDef = TypedDict(
     "ApplicationDescriptionsMessageTypeDef",
     {
         "Applications": List[ApplicationDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentDescriptionsMessageTypeDef = TypedDict(
     "EnvironmentDescriptionsMessageTypeDef",
     {
         "Environments": List[EnvironmentDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/type_defs.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_elasticbeanstalk.type_defs import AbortEnvironmentUpdateMessageRequestTypeDef
 
-    data: AbortEnvironmentUpdateMessageRequestTypeDef = {...}
+    data: AbortEnvironmentUpdateMessageRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -38,69 +38,63 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AbortEnvironmentUpdateMessageRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "LatencyTypeDef",
     "StatusCodesTypeDef",
     "S3LocationTypeDef",
     "SourceBuildInformationTypeDef",
     "MaxAgeRuleTypeDef",
     "MaxCountRuleTypeDef",
     "ApplyEnvironmentManagedActionRequestRequestTypeDef",
-    "ApplyEnvironmentManagedActionResultTypeDef",
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     "AutoScalingGroupTypeDef",
     "BuildConfigurationTypeDef",
     "BuilderTypeDef",
     "CPUUtilizationTypeDef",
     "CheckDNSAvailabilityMessageRequestTypeDef",
-    "CheckDNSAvailabilityResultMessageTypeDef",
     "ComposeEnvironmentsMessageRequestTypeDef",
     "OptionRestrictionRegexTypeDef",
     "ConfigurationOptionSettingTypeDef",
     "ValidationMessageTypeDef",
     "TagTypeDef",
     "SourceConfigurationTypeDef",
     "EnvironmentTierTypeDef",
     "OptionSpecificationTypeDef",
     "PlatformSummaryTypeDef",
-    "CreateStorageLocationResultMessageTypeDef",
     "CustomAmiTypeDef",
     "DeleteApplicationMessageRequestTypeDef",
     "DeleteApplicationVersionMessageRequestTypeDef",
     "DeleteConfigurationTemplateMessageRequestTypeDef",
     "DeleteEnvironmentConfigurationMessageRequestTypeDef",
     "DeletePlatformVersionRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeApplicationVersionsMessageRequestTypeDef",
     "DescribeApplicationsMessageRequestTypeDef",
     "DescribeConfigurationSettingsMessageRequestTypeDef",
     "DescribeEnvironmentHealthRequestRequestTypeDef",
     "InstanceHealthSummaryTypeDef",
-    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     "ManagedActionHistoryItemTypeDef",
     "DescribeEnvironmentManagedActionsRequestRequestTypeDef",
     "ManagedActionTypeDef",
     "DescribeEnvironmentResourcesMessageRequestTypeDef",
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    "TimestampTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeEnvironmentsMessageRequestTypeDef",
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    "DescribeEventsMessageRequestTypeDef",
     "DescribeInstancesHealthRequestRequestTypeDef",
     "DescribePlatformVersionRequestRequestTypeDef",
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnvironmentLinkTypeDef",
     "EnvironmentInfoDescriptionTypeDef",
     "InstanceTypeDef",
     "LaunchConfigurationTypeDef",
     "LaunchTemplateTypeDef",
     "LoadBalancerTypeDef",
     "QueueTypeDef",
@@ -108,33 +102,35 @@
     "EventDescriptionTypeDef",
     "SolutionStackDescriptionTypeDef",
     "SearchFilterTypeDef",
     "PlatformBranchSummaryTypeDef",
     "PlatformFilterTypeDef",
     "ListTagsForResourceMessageRequestTypeDef",
     "ListenerTypeDef",
-    "PaginatorConfigTypeDef",
     "PlatformFrameworkTypeDef",
     "PlatformProgrammingLanguageTypeDef",
     "RebuildEnvironmentMessageRequestTypeDef",
     "RequestEnvironmentInfoMessageRequestTypeDef",
     "ResourceQuotaTypeDef",
-    "ResponseMetadataTypeDef",
     "RestartAppServerMessageRequestTypeDef",
     "RetrieveEnvironmentInfoMessageRequestTypeDef",
     "SwapEnvironmentCNAMEsMessageRequestTypeDef",
     "TerminateEnvironmentMessageRequestTypeDef",
     "UpdateApplicationMessageRequestTypeDef",
     "UpdateApplicationVersionMessageRequestTypeDef",
+    "ApplyEnvironmentManagedActionResultTypeDef",
+    "CheckDNSAvailabilityResultMessageTypeDef",
+    "CreateStorageLocationResultMessageTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ApplicationMetricsTypeDef",
     "ApplicationVersionDescriptionTypeDef",
     "ApplicationVersionLifecycleConfigTypeDef",
     "SystemStatusTypeDef",
     "ConfigurationOptionDescriptionTypeDef",
-    "ConfigurationSettingsDescriptionResponseMetadataTypeDef",
+    "ConfigurationSettingsDescriptionResponseTypeDef",
     "ConfigurationSettingsDescriptionTypeDef",
     "ValidateConfigurationSettingsMessageRequestTypeDef",
     "ConfigurationSettingsValidationMessagesTypeDef",
     "CreateApplicationVersionMessageRequestTypeDef",
     "CreatePlatformVersionRequestRequestTypeDef",
     "ResourceTagsDescriptionMessageTypeDef",
     "UpdateTagsForResourceMessageRequestTypeDef",
@@ -142,16 +138,22 @@
     "CreateEnvironmentMessageRequestTypeDef",
     "DescribeConfigurationOptionsMessageRequestTypeDef",
     "UpdateConfigurationTemplateMessageRequestTypeDef",
     "UpdateEnvironmentMessageRequestTypeDef",
     "CreatePlatformVersionResultTypeDef",
     "DeletePlatformVersionResultTypeDef",
     "ListPlatformVersionsResultTypeDef",
+    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     "DescribeEnvironmentManagedActionsResultTypeDef",
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    "DescribeEnvironmentsMessageRequestTypeDef",
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    "DescribeEventsMessageRequestTypeDef",
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef",
     "DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef",
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     "EnvironmentResourceDescriptionTypeDef",
     "EventDescriptionsMessageTypeDef",
     "ListAvailableSolutionStacksResultMessageTypeDef",
@@ -174,15 +176,15 @@
     "DescribePlatformVersionResultTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "ApplicationDescriptionTypeDef",
     "ApplicationResourceLifecycleDescriptionMessageTypeDef",
     "CreateApplicationMessageRequestTypeDef",
     "UpdateApplicationResourceLifecycleMessageRequestTypeDef",
     "DescribeInstancesHealthResultTypeDef",
-    "EnvironmentDescriptionResponseMetadataTypeDef",
+    "EnvironmentDescriptionResponseTypeDef",
     "EnvironmentDescriptionTypeDef",
     "ApplicationDescriptionMessageTypeDef",
     "ApplicationDescriptionsMessageTypeDef",
     "EnvironmentDescriptionsMessageTypeDef",
 )
 
 AbortEnvironmentUpdateMessageRequestTypeDef = TypedDict(
@@ -190,14 +192,25 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
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
 LatencyTypeDef = TypedDict(
     "LatencyTypeDef",
     {
         "P999": float,
         "P99": float,
         "P95": float,
         "P90": float,
@@ -249,17 +262,19 @@
     {
         "MaxAgeInDays": int,
         "DeleteSourceFromS3": bool,
     },
     total=False,
 )
 
+
 class MaxAgeRuleTypeDef(_RequiredMaxAgeRuleTypeDef, _OptionalMaxAgeRuleTypeDef):
     pass
 
+
 _RequiredMaxCountRuleTypeDef = TypedDict(
     "_RequiredMaxCountRuleTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalMaxCountRuleTypeDef = TypedDict(
@@ -267,17 +282,19 @@
     {
         "MaxCount": int,
         "DeleteSourceFromS3": bool,
     },
     total=False,
 )
 
+
 class MaxCountRuleTypeDef(_RequiredMaxCountRuleTypeDef, _OptionalMaxCountRuleTypeDef):
     pass
 
+
 _RequiredApplyEnvironmentManagedActionRequestRequestTypeDef = TypedDict(
     "_RequiredApplyEnvironmentManagedActionRequestRequestTypeDef",
     {
         "ActionId": str,
     },
 )
 _OptionalApplyEnvironmentManagedActionRequestRequestTypeDef = TypedDict(
@@ -285,30 +302,21 @@
     {
         "EnvironmentName": str,
         "EnvironmentId": str,
     },
     total=False,
 )
 
+
 class ApplyEnvironmentManagedActionRequestRequestTypeDef(
     _RequiredApplyEnvironmentManagedActionRequestRequestTypeDef,
     _OptionalApplyEnvironmentManagedActionRequestRequestTypeDef,
 ):
     pass
 
-ApplyEnvironmentManagedActionResultTypeDef = TypedDict(
-    "ApplyEnvironmentManagedActionResultTypeDef",
-    {
-        "ActionId": str,
-        "ActionDescription": str,
-        "ActionType": ActionTypeType,
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 AssociateEnvironmentOperationsRoleMessageRequestTypeDef = TypedDict(
     "AssociateEnvironmentOperationsRoleMessageRequestTypeDef",
     {
         "EnvironmentName": str,
         "OperationsRole": str,
     },
@@ -335,19 +343,21 @@
         "ArtifactName": str,
         "ComputeType": ComputeTypeType,
         "TimeoutInMinutes": int,
     },
     total=False,
 )
 
+
 class BuildConfigurationTypeDef(
     _RequiredBuildConfigurationTypeDef, _OptionalBuildConfigurationTypeDef
 ):
     pass
 
+
 BuilderTypeDef = TypedDict(
     "BuilderTypeDef",
     {
         "ARN": str,
     },
     total=False,
 )
@@ -370,23 +380,14 @@
 CheckDNSAvailabilityMessageRequestTypeDef = TypedDict(
     "CheckDNSAvailabilityMessageRequestTypeDef",
     {
         "CNAMEPrefix": str,
     },
 )
 
-CheckDNSAvailabilityResultMessageTypeDef = TypedDict(
-    "CheckDNSAvailabilityResultMessageTypeDef",
-    {
-        "Available": bool,
-        "FullyQualifiedCNAME": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ComposeEnvironmentsMessageRequestTypeDef = TypedDict(
     "ComposeEnvironmentsMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "GroupName": str,
         "VersionLabels": Sequence[str],
     },
@@ -477,22 +478,14 @@
         "PlatformVersion": str,
         "PlatformBranchName": str,
         "PlatformBranchLifecycleState": str,
     },
     total=False,
 )
 
-CreateStorageLocationResultMessageTypeDef = TypedDict(
-    "CreateStorageLocationResultMessageTypeDef",
-    {
-        "S3Bucket": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomAmiTypeDef = TypedDict(
     "CustomAmiTypeDef",
     {
         "VirtualizationType": str,
         "ImageId": str,
     },
     total=False,
@@ -508,19 +501,21 @@
     "_OptionalDeleteApplicationMessageRequestTypeDef",
     {
         "TerminateEnvByForce": bool,
     },
     total=False,
 )
 
+
 class DeleteApplicationMessageRequestTypeDef(
     _RequiredDeleteApplicationMessageRequestTypeDef, _OptionalDeleteApplicationMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteApplicationVersionMessageRequestTypeDef = TypedDict(
     "_RequiredDeleteApplicationVersionMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
     },
 )
@@ -528,20 +523,22 @@
     "_OptionalDeleteApplicationVersionMessageRequestTypeDef",
     {
         "DeleteSourceBundle": bool,
     },
     total=False,
 )
 
+
 class DeleteApplicationVersionMessageRequestTypeDef(
     _RequiredDeleteApplicationVersionMessageRequestTypeDef,
     _OptionalDeleteApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
+
 DeleteConfigurationTemplateMessageRequestTypeDef = TypedDict(
     "DeleteConfigurationTemplateMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "TemplateName": str,
     },
 )
@@ -569,20 +566,20 @@
         "DeploymentId": int,
         "Status": str,
         "DeploymentTime": datetime,
     },
     total=False,
 )
 
-DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = TypedDict(
-    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ApplicationName": str,
-        "VersionLabels": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeApplicationVersionsMessageRequestTypeDef = TypedDict(
     "DescribeApplicationVersionsMessageRequestTypeDef",
     {
@@ -613,20 +610,22 @@
     {
         "TemplateName": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
+
 class DescribeConfigurationSettingsMessageRequestTypeDef(
     _RequiredDescribeConfigurationSettingsMessageRequestTypeDef,
     _OptionalDescribeConfigurationSettingsMessageRequestTypeDef,
 ):
     pass
 
+
 DescribeEnvironmentHealthRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentHealthRequestRequestTypeDef",
     {
         "EnvironmentName": str,
         "EnvironmentId": str,
         "AttributeNames": Sequence[EnvironmentHealthAttributeType],
     },
@@ -644,24 +643,14 @@
         "Warning": int,
         "Degraded": int,
         "Severe": int,
     },
     total=False,
 )
 
-DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
-    {
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef",
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
         "NextToken": str,
         "MaxItems": int,
@@ -711,89 +700,24 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
-DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "EnvironmentIds": Sequence[str],
-        "EnvironmentNames": Sequence[str],
-        "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeEnvironmentsMessageRequestTypeDef = TypedDict(
-    "DescribeEnvironmentsMessageRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "EnvironmentIds": Sequence[str],
-        "EnvironmentNames": Sequence[str],
-        "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "TemplateName": str,
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PlatformArn": str,
-        "RequestId": str,
-        "Severity": EventSeverityType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-DescribeEventsMessageRequestTypeDef = TypedDict(
-    "DescribeEventsMessageRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "VersionLabel": str,
-        "TemplateName": str,
-        "EnvironmentId": str,
-        "EnvironmentName": str,
-        "PlatformArn": str,
-        "RequestId": str,
-        "Severity": EventSeverityType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
 DescribeInstancesHealthRequestRequestTypeDef = TypedDict(
     "DescribeInstancesHealthRequestRequestTypeDef",
     {
         "EnvironmentName": str,
         "EnvironmentId": str,
         "AttributeNames": Sequence[InstancesHealthAttributeType],
         "NextToken": str,
@@ -812,21 +736,14 @@
 DisassociateEnvironmentOperationsRoleMessageRequestTypeDef = TypedDict(
     "DisassociateEnvironmentOperationsRoleMessageRequestTypeDef",
     {
         "EnvironmentName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentLinkTypeDef = TypedDict(
     "EnvironmentLinkTypeDef",
     {
         "LinkName": str,
         "EnvironmentName": str,
     },
     total=False,
@@ -961,24 +878,14 @@
     {
         "Protocol": str,
         "Port": int,
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
 PlatformFrameworkTypeDef = TypedDict(
     "PlatformFrameworkTypeDef",
     {
         "Name": str,
         "Version": str,
     },
     total=False,
@@ -1013,39 +920,30 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
+
 class RequestEnvironmentInfoMessageRequestTypeDef(
     _RequiredRequestEnvironmentInfoMessageRequestTypeDef,
     _OptionalRequestEnvironmentInfoMessageRequestTypeDef,
 ):
     pass
 
+
 ResourceQuotaTypeDef = TypedDict(
     "ResourceQuotaTypeDef",
     {
         "Maximum": int,
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
 RestartAppServerMessageRequestTypeDef = TypedDict(
     "RestartAppServerMessageRequestTypeDef",
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
@@ -1062,20 +960,22 @@
     {
         "EnvironmentId": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
+
 class RetrieveEnvironmentInfoMessageRequestTypeDef(
     _RequiredRetrieveEnvironmentInfoMessageRequestTypeDef,
     _OptionalRetrieveEnvironmentInfoMessageRequestTypeDef,
 ):
     pass
 
+
 SwapEnvironmentCNAMEsMessageRequestTypeDef = TypedDict(
     "SwapEnvironmentCNAMEsMessageRequestTypeDef",
     {
         "SourceEnvironmentId": str,
         "SourceEnvironmentName": str,
         "DestinationEnvironmentId": str,
         "DestinationEnvironmentName": str,
@@ -1104,19 +1004,21 @@
     "_OptionalUpdateApplicationMessageRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateApplicationMessageRequestTypeDef(
     _RequiredUpdateApplicationMessageRequestTypeDef, _OptionalUpdateApplicationMessageRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateApplicationVersionMessageRequestTypeDef = TypedDict(
     "_RequiredUpdateApplicationVersionMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
     },
 )
@@ -1124,20 +1026,57 @@
     "_OptionalUpdateApplicationVersionMessageRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateApplicationVersionMessageRequestTypeDef(
     _RequiredUpdateApplicationVersionMessageRequestTypeDef,
     _OptionalUpdateApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
+
+ApplyEnvironmentManagedActionResultTypeDef = TypedDict(
+    "ApplyEnvironmentManagedActionResultTypeDef",
+    {
+        "ActionId": str,
+        "ActionDescription": str,
+        "ActionType": ActionTypeType,
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CheckDNSAvailabilityResultMessageTypeDef = TypedDict(
+    "CheckDNSAvailabilityResultMessageTypeDef",
+    {
+        "Available": bool,
+        "FullyQualifiedCNAME": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStorageLocationResultMessageTypeDef = TypedDict(
+    "CreateStorageLocationResultMessageTypeDef",
+    {
+        "S3Bucket": str,
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
 ApplicationMetricsTypeDef = TypedDict(
     "ApplicationMetricsTypeDef",
     {
         "Duration": int,
         "RequestCount": int,
         "StatusCodes": StatusCodesTypeDef,
         "Latency": LatencyTypeDef,
@@ -1194,28 +1133,28 @@
         "MaxValue": int,
         "MaxLength": int,
         "Regex": OptionRestrictionRegexTypeDef,
     },
     total=False,
 )
 
-ConfigurationSettingsDescriptionResponseMetadataTypeDef = TypedDict(
-    "ConfigurationSettingsDescriptionResponseMetadataTypeDef",
+ConfigurationSettingsDescriptionResponseTypeDef = TypedDict(
+    "ConfigurationSettingsDescriptionResponseTypeDef",
     {
         "SolutionStackName": str,
         "PlatformArn": str,
         "ApplicationName": str,
         "TemplateName": str,
         "Description": str,
         "EnvironmentName": str,
         "DeploymentStatus": ConfigurationDeploymentStatusType,
         "DateCreated": datetime,
         "DateUpdated": datetime,
         "OptionSettings": List[ConfigurationOptionSettingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationSettingsDescriptionTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionTypeDef",
     {
         "SolutionStackName": str,
@@ -1244,25 +1183,27 @@
     {
         "TemplateName": str,
         "EnvironmentName": str,
     },
     total=False,
 )
 
+
 class ValidateConfigurationSettingsMessageRequestTypeDef(
     _RequiredValidateConfigurationSettingsMessageRequestTypeDef,
     _OptionalValidateConfigurationSettingsMessageRequestTypeDef,
 ):
     pass
 
+
 ConfigurationSettingsValidationMessagesTypeDef = TypedDict(
     "ConfigurationSettingsValidationMessagesTypeDef",
     {
         "Messages": List[ValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateApplicationVersionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationVersionMessageRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1279,20 +1220,22 @@
         "AutoCreateApplication": bool,
         "Process": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateApplicationVersionMessageRequestTypeDef(
     _RequiredCreateApplicationVersionMessageRequestTypeDef,
     _OptionalCreateApplicationVersionMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreatePlatformVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePlatformVersionRequestRequestTypeDef",
     {
         "PlatformName": str,
         "PlatformVersion": str,
         "PlatformDefinitionBundle": S3LocationTypeDef,
     },
@@ -1303,26 +1246,28 @@
         "EnvironmentName": str,
         "OptionSettings": Sequence[ConfigurationOptionSettingTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePlatformVersionRequestRequestTypeDef(
     _RequiredCreatePlatformVersionRequestRequestTypeDef,
     _OptionalCreatePlatformVersionRequestRequestTypeDef,
 ):
     pass
 
+
 ResourceTagsDescriptionMessageTypeDef = TypedDict(
     "ResourceTagsDescriptionMessageTypeDef",
     {
         "ResourceArn": str,
         "ResourceTags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTagsForResourceMessageRequestTypeDef = TypedDict(
     "_RequiredUpdateTagsForResourceMessageRequestTypeDef",
     {
         "ResourceArn": str,
@@ -1333,20 +1278,22 @@
     {
         "TagsToAdd": Sequence[TagTypeDef],
         "TagsToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateTagsForResourceMessageRequestTypeDef(
     _RequiredUpdateTagsForResourceMessageRequestTypeDef,
     _OptionalUpdateTagsForResourceMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateConfigurationTemplateMessageRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationTemplateMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "TemplateName": str,
     },
 )
@@ -1360,20 +1307,22 @@
         "Description": str,
         "OptionSettings": Sequence[ConfigurationOptionSettingTypeDef],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateConfigurationTemplateMessageRequestTypeDef(
     _RequiredCreateConfigurationTemplateMessageRequestTypeDef,
     _OptionalCreateConfigurationTemplateMessageRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateEnvironmentMessageRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentMessageRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 _OptionalCreateEnvironmentMessageRequestTypeDef = TypedDict(
@@ -1392,19 +1341,21 @@
         "OptionSettings": Sequence[ConfigurationOptionSettingTypeDef],
         "OptionsToRemove": Sequence[OptionSpecificationTypeDef],
         "OperationsRole": str,
     },
     total=False,
 )
 
+
 class CreateEnvironmentMessageRequestTypeDef(
     _RequiredCreateEnvironmentMessageRequestTypeDef, _OptionalCreateEnvironmentMessageRequestTypeDef
 ):
     pass
 
+
 DescribeConfigurationOptionsMessageRequestTypeDef = TypedDict(
     "DescribeConfigurationOptionsMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "TemplateName": str,
         "EnvironmentName": str,
         "SolutionStackName": str,
@@ -1427,20 +1378,22 @@
         "Description": str,
         "OptionSettings": Sequence[ConfigurationOptionSettingTypeDef],
         "OptionsToRemove": Sequence[OptionSpecificationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateConfigurationTemplateMessageRequestTypeDef(
     _RequiredUpdateConfigurationTemplateMessageRequestTypeDef,
     _OptionalUpdateConfigurationTemplateMessageRequestTypeDef,
 ):
     pass
 
+
 UpdateEnvironmentMessageRequestTypeDef = TypedDict(
     "UpdateEnvironmentMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "EnvironmentId": str,
         "EnvironmentName": str,
         "GroupName": str,
@@ -1457,61 +1410,147 @@
 )
 
 CreatePlatformVersionResultTypeDef = TypedDict(
     "CreatePlatformVersionResultTypeDef",
     {
         "PlatformSummary": PlatformSummaryTypeDef,
         "Builder": BuilderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePlatformVersionResultTypeDef = TypedDict(
     "DeletePlatformVersionResultTypeDef",
     {
         "PlatformSummary": PlatformSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformVersionsResultTypeDef = TypedDict(
     "ListPlatformVersionsResultTypeDef",
     {
         "PlatformSummaryList": List[PlatformSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = TypedDict(
+    "DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabels": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef",
+    {
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeEnvironmentManagedActionHistoryResultTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionHistoryResultTypeDef",
     {
         "ManagedActionHistoryItems": List[ManagedActionHistoryItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEnvironmentManagedActionsResultTypeDef = TypedDict(
     "DescribeEnvironmentManagedActionsResultTypeDef",
     {
         "ManagedActions": List[ManagedActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "EnvironmentIds": Sequence[str],
+        "EnvironmentNames": Sequence[str],
+        "IncludeDeleted": bool,
+        "IncludedDeletedBackTo": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEnvironmentsMessageRequestTypeDef = TypedDict(
+    "DescribeEnvironmentsMessageRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "EnvironmentIds": Sequence[str],
+        "EnvironmentNames": Sequence[str],
+        "IncludeDeleted": bool,
+        "IncludedDeletedBackTo": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+DescribeEventsMessageDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsMessageDescribeEventsPaginateTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "TemplateName": str,
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PlatformArn": str,
+        "RequestId": str,
+        "Severity": EventSeverityType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsMessageRequestTypeDef = TypedDict(
+    "DescribeEventsMessageRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "VersionLabel": str,
+        "TemplateName": str,
+        "EnvironmentId": str,
+        "EnvironmentName": str,
+        "PlatformArn": str,
+        "RequestId": str,
+        "Severity": EventSeverityType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
     },
+    total=False,
 )
 
 DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef = TypedDict(
     "DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "MaxRecords": int,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
@@ -1519,15 +1558,15 @@
     "DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "MaxRecords": int,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
@@ -1535,27 +1574,27 @@
     "DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef",
     {
         "ApplicationName": str,
         "VersionLabel": str,
         "EnvironmentIds": Sequence[str],
         "EnvironmentNames": Sequence[str],
         "IncludeDeleted": bool,
-        "IncludedDeletedBackTo": Union[datetime, str],
+        "IncludedDeletedBackTo": TimestampTypeDef,
         "MaxRecords": int,
         "NextToken": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
 RetrieveEnvironmentInfoResultMessageTypeDef = TypedDict(
     "RetrieveEnvironmentInfoResultMessageTypeDef",
     {
         "EnvironmentInfo": List[EnvironmentInfoDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentResourceDescriptionTypeDef = TypedDict(
     "EnvironmentResourceDescriptionTypeDef",
     {
         "EnvironmentName": str,
@@ -1571,24 +1610,24 @@
 )
 
 EventDescriptionsMessageTypeDef = TypedDict(
     "EventDescriptionsMessageTypeDef",
     {
         "Events": List[EventDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAvailableSolutionStacksResultMessageTypeDef = TypedDict(
     "ListAvailableSolutionStacksResultMessageTypeDef",
     {
         "SolutionStacks": List[str],
         "SolutionStackDetails": List[SolutionStackDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformBranchesRequestRequestTypeDef = TypedDict(
     "ListPlatformBranchesRequestRequestTypeDef",
     {
         "Filters": Sequence[SearchFilterTypeDef],
@@ -1599,23 +1638,23 @@
 )
 
 ListPlatformBranchesResultTypeDef = TypedDict(
     "ListPlatformBranchesResultTypeDef",
     {
         "PlatformBranchSummaryList": List[PlatformBranchSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef = TypedDict(
     "ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef",
     {
         "Filters": Sequence[PlatformFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListPlatformVersionsRequestRequestTypeDef = TypedDict(
     "ListPlatformVersionsRequestRequestTypeDef",
     {
@@ -1683,32 +1722,32 @@
         "HealthStatus": str,
         "Status": EnvironmentHealthType,
         "Color": str,
         "Causes": List[str],
         "ApplicationMetrics": ApplicationMetricsTypeDef,
         "InstancesHealth": InstanceHealthSummaryTypeDef,
         "RefreshedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationVersionDescriptionMessageTypeDef = TypedDict(
     "ApplicationVersionDescriptionMessageTypeDef",
     {
         "ApplicationVersion": ApplicationVersionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationVersionDescriptionsMessageTypeDef = TypedDict(
     "ApplicationVersionDescriptionsMessageTypeDef",
     {
         "ApplicationVersions": List[ApplicationVersionDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationResourceLifecycleConfigTypeDef = TypedDict(
     "ApplicationResourceLifecycleConfigTypeDef",
     {
         "ServiceRole": str,
@@ -1736,31 +1775,31 @@
 
 ConfigurationOptionsDescriptionTypeDef = TypedDict(
     "ConfigurationOptionsDescriptionTypeDef",
     {
         "SolutionStackName": str,
         "PlatformArn": str,
         "Options": List[ConfigurationOptionDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConfigurationSettingsDescriptionsTypeDef = TypedDict(
     "ConfigurationSettingsDescriptionsTypeDef",
     {
         "ConfigurationSettings": List[ConfigurationSettingsDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentResourceDescriptionsMessageTypeDef = TypedDict(
     "EnvironmentResourceDescriptionsMessageTypeDef",
     {
         "EnvironmentResources": EnvironmentResourceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentResourcesDescriptionTypeDef = TypedDict(
     "EnvironmentResourcesDescriptionTypeDef",
     {
         "LoadBalancer": LoadBalancerDescriptionTypeDef,
@@ -1768,23 +1807,23 @@
     total=False,
 )
 
 DescribePlatformVersionResultTypeDef = TypedDict(
     "DescribePlatformVersionResultTypeDef",
     {
         "PlatformDescription": PlatformDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "ResourceQuotas": ResourceQuotasTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationDescriptionTypeDef = TypedDict(
     "ApplicationDescriptionTypeDef",
     {
         "ApplicationArn": str,
@@ -1800,15 +1839,15 @@
 )
 
 ApplicationResourceLifecycleDescriptionMessageTypeDef = TypedDict(
     "ApplicationResourceLifecycleDescriptionMessageTypeDef",
     {
         "ApplicationName": str,
         "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateApplicationMessageRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationMessageRequestTypeDef",
     {
         "ApplicationName": str,
@@ -1820,39 +1859,41 @@
         "Description": str,
         "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateApplicationMessageRequestTypeDef(
     _RequiredCreateApplicationMessageRequestTypeDef, _OptionalCreateApplicationMessageRequestTypeDef
 ):
     pass
 
+
 UpdateApplicationResourceLifecycleMessageRequestTypeDef = TypedDict(
     "UpdateApplicationResourceLifecycleMessageRequestTypeDef",
     {
         "ApplicationName": str,
         "ResourceLifecycleConfig": ApplicationResourceLifecycleConfigTypeDef,
     },
 )
 
 DescribeInstancesHealthResultTypeDef = TypedDict(
     "DescribeInstancesHealthResultTypeDef",
     {
         "InstanceHealthList": List[SingleInstanceHealthTypeDef],
         "RefreshedAt": datetime,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EnvironmentDescriptionResponseMetadataTypeDef = TypedDict(
-    "EnvironmentDescriptionResponseMetadataTypeDef",
+EnvironmentDescriptionResponseTypeDef = TypedDict(
+    "EnvironmentDescriptionResponseTypeDef",
     {
         "EnvironmentName": str,
         "EnvironmentId": str,
         "ApplicationName": str,
         "VersionLabel": str,
         "SolutionStackName": str,
         "PlatformArn": str,
@@ -1867,15 +1908,15 @@
         "Health": EnvironmentHealthType,
         "HealthStatus": EnvironmentHealthStatusType,
         "Resources": EnvironmentResourcesDescriptionTypeDef,
         "Tier": EnvironmentTierTypeDef,
         "EnvironmentLinks": List[EnvironmentLinkTypeDef],
         "EnvironmentArn": str,
         "OperationsRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentDescriptionTypeDef = TypedDict(
     "EnvironmentDescriptionTypeDef",
     {
         "EnvironmentName": str,
@@ -1903,27 +1944,27 @@
     total=False,
 )
 
 ApplicationDescriptionMessageTypeDef = TypedDict(
     "ApplicationDescriptionMessageTypeDef",
     {
         "Application": ApplicationDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ApplicationDescriptionsMessageTypeDef = TypedDict(
     "ApplicationDescriptionsMessageTypeDef",
     {
         "Applications": List[ApplicationDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentDescriptionsMessageTypeDef = TypedDict(
     "EnvironmentDescriptionsMessageTypeDef",
     {
         "Environments": List[EnvironmentDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/waiter.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/waiter.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,89 +20,85 @@
         client: ElasticBeanstalkClient
 
         environment_exists_waiter: EnvironmentExistsWaiter = client.get_waiter("environment_exists")
         environment_terminated_waiter: EnvironmentTerminatedWaiter = client.get_waiter("environment_terminated")
         environment_updated_waiter: EnvironmentUpdatedWaiter = client.get_waiter("environment_updated")
     ```
 """
-from datetime import datetime
-from typing import Sequence, Union
+from typing import Sequence
 
 from aiobotocore.waiter import AIOWaiter
 
-from .type_defs import WaiterConfigTypeDef
+from .type_defs import TimestampTypeDef, WaiterConfigTypeDef
 
 __all__ = ("EnvironmentExistsWaiter", "EnvironmentTerminatedWaiter", "EnvironmentUpdatedWaiter")
 
-
 class EnvironmentExistsWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentExists)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentexistswaiter)
     """
 
     async def wait(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentexistswaiter)
         """
 
-
 class EnvironmentTerminatedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentTerminated)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentterminatedwaiter)
     """
 
     async def wait(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentTerminated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentterminatedwaiter)
         """
 
-
 class EnvironmentUpdatedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentUpdated)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentupdatedwaiter)
     """
 
     async def wait(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentUpdated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentupdatedwaiter)
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk/waiter.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/waiter.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,86 +20,88 @@
         client: ElasticBeanstalkClient
 
         environment_exists_waiter: EnvironmentExistsWaiter = client.get_waiter("environment_exists")
         environment_terminated_waiter: EnvironmentTerminatedWaiter = client.get_waiter("environment_terminated")
         environment_updated_waiter: EnvironmentUpdatedWaiter = client.get_waiter("environment_updated")
     ```
 """
-from datetime import datetime
-from typing import Sequence, Union
+from typing import Sequence
 
 from aiobotocore.waiter import AIOWaiter
 
-from .type_defs import WaiterConfigTypeDef
+from .type_defs import TimestampTypeDef, WaiterConfigTypeDef
 
 __all__ = ("EnvironmentExistsWaiter", "EnvironmentTerminatedWaiter", "EnvironmentUpdatedWaiter")
 
+
 class EnvironmentExistsWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentExists)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentexistswaiter)
     """
 
     async def wait(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentexistswaiter)
         """
 
+
 class EnvironmentTerminatedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentTerminated)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentterminatedwaiter)
     """
 
     async def wait(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentTerminated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentterminatedwaiter)
         """
 
+
 class EnvironmentUpdatedWaiter(AIOWaiter):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentUpdated)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentupdatedwaiter)
     """
 
     async def wait(
         self,
         *,
         ApplicationName: str = ...,
         VersionLabel: str = ...,
         EnvironmentIds: Sequence[str] = ...,
         EnvironmentNames: Sequence[str] = ...,
         IncludeDeleted: bool = ...,
-        IncludedDeletedBackTo: Union[datetime, str] = ...,
+        IncludedDeletedBackTo: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         WaiterConfig: WaiterConfigTypeDef = ...
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Waiter.EnvironmentUpdated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/waiters/#environmentupdatedwaiter)
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elasticbeanstalk
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElasticBeanstalk 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElasticBeanstalk 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore elasticbeanstalk type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore elasticbeanstalk type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elasticbeanstalk"></a>
 
 # types-aiobotocore-elasticbeanstalk
 
 [![PyPI - types-aiobotocore-elasticbeanstalk](https://img.shields.io/pypi/v/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elasticbeanstalk.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elasticbeanstalk)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elasticbeanstalk?color=blue)](https://pypistats.org/packages/types-aiobotocore-elasticbeanstalk)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elasticbeanstalk)](https://pepy.tech/project/types-aiobotocore-elasticbeanstalk)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticBeanstalk 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
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
 [types-aiobotocore-elasticbeanstalk docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk/).
 
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
@@ -381,77 +380,70 @@
 )
 
 
 def check_value(value: ActionHistoryStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elasticbeanstalk.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elasticbeanstalk.type_defs import (
     AbortEnvironmentUpdateMessageRequestTypeDef,
+    ResponseMetadataTypeDef,
     LatencyTypeDef,
     StatusCodesTypeDef,
     S3LocationTypeDef,
     SourceBuildInformationTypeDef,
     MaxAgeRuleTypeDef,
     MaxCountRuleTypeDef,
     ApplyEnvironmentManagedActionRequestRequestTypeDef,
-    ApplyEnvironmentManagedActionResultTypeDef,
     AssociateEnvironmentOperationsRoleMessageRequestTypeDef,
     AutoScalingGroupTypeDef,
     BuildConfigurationTypeDef,
     BuilderTypeDef,
     CPUUtilizationTypeDef,
     CheckDNSAvailabilityMessageRequestTypeDef,
-    CheckDNSAvailabilityResultMessageTypeDef,
     ComposeEnvironmentsMessageRequestTypeDef,
     OptionRestrictionRegexTypeDef,
     ConfigurationOptionSettingTypeDef,
     ValidationMessageTypeDef,
     TagTypeDef,
     SourceConfigurationTypeDef,
     EnvironmentTierTypeDef,
     OptionSpecificationTypeDef,
     PlatformSummaryTypeDef,
-    CreateStorageLocationResultMessageTypeDef,
     CustomAmiTypeDef,
     DeleteApplicationMessageRequestTypeDef,
     DeleteApplicationVersionMessageRequestTypeDef,
     DeleteConfigurationTemplateMessageRequestTypeDef,
     DeleteEnvironmentConfigurationMessageRequestTypeDef,
     DeletePlatformVersionRequestRequestTypeDef,
     DeploymentTypeDef,
-    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeApplicationVersionsMessageRequestTypeDef,
     DescribeApplicationsMessageRequestTypeDef,
     DescribeConfigurationSettingsMessageRequestTypeDef,
     DescribeEnvironmentHealthRequestRequestTypeDef,
     InstanceHealthSummaryTypeDef,
-    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef,
     ManagedActionHistoryItemTypeDef,
     DescribeEnvironmentManagedActionsRequestRequestTypeDef,
     ManagedActionTypeDef,
     DescribeEnvironmentResourcesMessageRequestTypeDef,
-    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
+    TimestampTypeDef,
     WaiterConfigTypeDef,
-    DescribeEnvironmentsMessageRequestTypeDef,
-    DescribeEventsMessageDescribeEventsPaginateTypeDef,
-    DescribeEventsMessageRequestTypeDef,
     DescribeInstancesHealthRequestRequestTypeDef,
     DescribePlatformVersionRequestRequestTypeDef,
     DisassociateEnvironmentOperationsRoleMessageRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnvironmentLinkTypeDef,
     EnvironmentInfoDescriptionTypeDef,
     InstanceTypeDef,
     LaunchConfigurationTypeDef,
     LaunchTemplateTypeDef,
     LoadBalancerTypeDef,
     QueueTypeDef,
@@ -459,33 +451,35 @@
     EventDescriptionTypeDef,
     SolutionStackDescriptionTypeDef,
     SearchFilterTypeDef,
     PlatformBranchSummaryTypeDef,
     PlatformFilterTypeDef,
     ListTagsForResourceMessageRequestTypeDef,
     ListenerTypeDef,
-    PaginatorConfigTypeDef,
     PlatformFrameworkTypeDef,
     PlatformProgrammingLanguageTypeDef,
     RebuildEnvironmentMessageRequestTypeDef,
     RequestEnvironmentInfoMessageRequestTypeDef,
     ResourceQuotaTypeDef,
-    ResponseMetadataTypeDef,
     RestartAppServerMessageRequestTypeDef,
     RetrieveEnvironmentInfoMessageRequestTypeDef,
     SwapEnvironmentCNAMEsMessageRequestTypeDef,
     TerminateEnvironmentMessageRequestTypeDef,
     UpdateApplicationMessageRequestTypeDef,
     UpdateApplicationVersionMessageRequestTypeDef,
+    ApplyEnvironmentManagedActionResultTypeDef,
+    CheckDNSAvailabilityResultMessageTypeDef,
+    CreateStorageLocationResultMessageTypeDef,
+    EmptyResponseMetadataTypeDef,
     ApplicationMetricsTypeDef,
     ApplicationVersionDescriptionTypeDef,
     ApplicationVersionLifecycleConfigTypeDef,
     SystemStatusTypeDef,
     ConfigurationOptionDescriptionTypeDef,
-    ConfigurationSettingsDescriptionResponseMetadataTypeDef,
+    ConfigurationSettingsDescriptionResponseTypeDef,
     ConfigurationSettingsDescriptionTypeDef,
     ValidateConfigurationSettingsMessageRequestTypeDef,
     ConfigurationSettingsValidationMessagesTypeDef,
     CreateApplicationVersionMessageRequestTypeDef,
     CreatePlatformVersionRequestRequestTypeDef,
     ResourceTagsDescriptionMessageTypeDef,
     UpdateTagsForResourceMessageRequestTypeDef,
@@ -493,16 +487,22 @@
     CreateEnvironmentMessageRequestTypeDef,
     DescribeConfigurationOptionsMessageRequestTypeDef,
     UpdateConfigurationTemplateMessageRequestTypeDef,
     UpdateEnvironmentMessageRequestTypeDef,
     CreatePlatformVersionResultTypeDef,
     DeletePlatformVersionResultTypeDef,
     ListPlatformVersionsResultTypeDef,
+    DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef,
+    DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef,
     DescribeEnvironmentManagedActionHistoryResultTypeDef,
     DescribeEnvironmentManagedActionsResultTypeDef,
+    DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef,
+    DescribeEnvironmentsMessageRequestTypeDef,
+    DescribeEventsMessageDescribeEventsPaginateTypeDef,
+    DescribeEventsMessageRequestTypeDef,
     DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef,
     DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef,
     RetrieveEnvironmentInfoResultMessageTypeDef,
     EnvironmentResourceDescriptionTypeDef,
     EventDescriptionsMessageTypeDef,
     ListAvailableSolutionStacksResultMessageTypeDef,
@@ -525,23 +525,23 @@
     DescribePlatformVersionResultTypeDef,
     DescribeAccountAttributesResultTypeDef,
     ApplicationDescriptionTypeDef,
     ApplicationResourceLifecycleDescriptionMessageTypeDef,
     CreateApplicationMessageRequestTypeDef,
     UpdateApplicationResourceLifecycleMessageRequestTypeDef,
     DescribeInstancesHealthResultTypeDef,
-    EnvironmentDescriptionResponseMetadataTypeDef,
+    EnvironmentDescriptionResponseTypeDef,
     EnvironmentDescriptionTypeDef,
     ApplicationDescriptionMessageTypeDef,
     ApplicationDescriptionsMessageTypeDef,
     EnvironmentDescriptionsMessageTypeDef,
 )
 
 
-def get_structure() -> AbortEnvironmentUpdateMessageRequestTypeDef:
+def get_value() -> AbortEnvironmentUpdateMessageRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt` & `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*


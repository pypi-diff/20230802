# Comparing `tmp/types-aiobotocore-autoscaling-2.5.2.tar.gz` & `tmp/types-aiobotocore-autoscaling-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-autoscaling-2.5.2.tar", last modified: Sat Jul  8 01:43:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-autoscaling-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
```

## Comparing `types-aiobotocore-autoscaling-2.5.2.tar` & `types-aiobotocore-autoscaling-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.773735 types-aiobotocore-autoscaling-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-07-08 01:43:16.769735 types-aiobotocore-autoscaling-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21569 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:16.773735 types-aiobotocore-autoscaling-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.761735 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55230 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    55146 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-07-08 01:26:11.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75427 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75310 2023-07-08 01:26:12.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:10.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.769735 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23150 2023-07-08 01:43:16.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-08 01:43:16.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:16.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:43:16.000000 types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.141648 types-aiobotocore-autoscaling-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-08-02 14:51:55.141648 types-aiobotocore-autoscaling-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.141648 types-aiobotocore-autoscaling-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.137648 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55242 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55158 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-08-02 14:33:38.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    86393 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86258 2023-08-02 14:33:38.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.141648 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-08-02 14:51:54.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:51:54.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:54.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:54.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:54.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:51:54.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-autoscaling-2.5.2/LICENSE` & `types-aiobotocore-autoscaling-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2/PKG-INFO` & `types-aiobotocore-autoscaling-2.5.2.post1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-autoscaling
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AutoScaling 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AutoScaling 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore autoscaling type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore autoscaling type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-autoscaling"></a>
 
 # types-aiobotocore-autoscaling
 
 [![PyPI - types-aiobotocore-autoscaling](https://img.shields.io/pypi/v/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-autoscaling?color=blue)](https://pypistats.org/packages/types-aiobotocore-autoscaling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling)](https://pepy.tech/project/types-aiobotocore-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AutoScaling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [types-aiobotocore-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/).
 
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
@@ -378,203 +377,227 @@
 )
 
 
 def check_value(value: AcceleratorManufacturerType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_autoscaling.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_autoscaling.type_defs import (
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
+    ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     EnabledMetricTypeDef,
     LaunchTemplateSpecificationTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
-    ScheduledUpdateGroupActionRequestTypeDef,
     EbsTypeDef,
-    CancelInstanceRefreshAnswerTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
-    DescribeAccountLimitsAnswerTypeDef,
-    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
     DescribeAutoScalingInstancesTypeRequestTypeDef,
-    DescribeAutoScalingNotificationTypesAnswerTypeDef,
     DescribeInstanceRefreshesTypeRequestTypeDef,
-    DescribeLifecycleHookTypesAnswerTypeDef,
     LifecycleHookTypeDef,
     DescribeLifecycleHooksTypeRequestTypeDef,
-    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     DescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
     LoadBalancerTargetGroupStateTypeDef,
-    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     DescribeLoadBalancersRequestRequestTypeDef,
     LoadBalancerStateTypeDef,
     MetricCollectionTypeTypeDef,
     MetricGranularityTypeTypeDef,
     NotificationConfigurationTypeDef,
-    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
     DescribeNotificationConfigurationsTypeRequestTypeDef,
-    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
     DescribePoliciesTypeRequestTypeDef,
-    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingActivitiesTypeRequestTypeDef,
-    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
-    DescribeScheduledActionsTypeRequestTypeDef,
-    DescribeTerminationPolicyTypesAnswerTypeDef,
+    TimestampTypeDef,
     DescribeTrafficSourcesRequestRequestTypeDef,
     TrafficSourceStateTypeDef,
     DescribeWarmPoolTypeRequestTypeDef,
     DetachInstancesQueryRequestTypeDef,
     DetachLoadBalancerTargetGroupsTypeRequestTypeDef,
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
-    GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
-    RefreshPreferencesTypeDef,
+    RefreshPreferencesOutputTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
     InstanceReusePolicyTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
-    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
-    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
-    PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RollbackInstanceRefreshAnswerTypeDef,
+    RefreshPreferencesTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
-    StartInstanceRefreshAnswerTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
+    CancelInstanceRefreshAnswerTypeDef,
+    DescribeAccountLimitsAnswerTypeDef,
+    DescribeAutoScalingNotificationTypesAnswerTypeDef,
+    DescribeLifecycleHookTypesAnswerTypeDef,
+    DescribeTerminationPolicyTypesAnswerTypeDef,
     DetachInstancesAnswerTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
+    RollbackInstanceRefreshAnswerTypeDef,
+    StartInstanceRefreshAnswerTypeDef,
     DescribeAdjustmentTypesAnswerTypeDef,
     PolicyARNTypeTypeDef,
     AttachTrafficSourcesTypeRequestTypeDef,
     DetachTrafficSourcesTypeRequestTypeDef,
-    AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
     AutoScalingGroupNamesTypeRequestTypeDef,
-    DescribeTagsTypeDescribeTagsPaginateTypeDef,
     DescribeTagsTypeRequestTypeDef,
+    AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
+    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
+    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
+    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
+    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
+    DescribeTagsTypeDescribeTagsPaginateTypeDef,
+    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
-    BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
+    DescribeScheduledActionsTypeRequestTypeDef,
+    GetPredictiveScalingForecastTypeRequestTypeDef,
+    PutScheduledUpdateGroupActionTypeRequestTypeDef,
+    ScheduledUpdateGroupActionRequestTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
+    InstanceRequirementsOutputTypeDef,
     InstanceRequirementsTypeDef,
     PutWarmPoolTypeRequestTypeDef,
     WarmPoolConfigurationTypeDef,
     ProcessesTypeTypeDef,
+    RefreshPreferencesUnionTypeDef,
     ScheduledActionsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     CreateLaunchConfigurationTypeRequestTypeDef,
     LaunchConfigurationTypeDef,
+    MetricStatOutputTypeDef,
+    TargetTrackingMetricStatOutputTypeDef,
     MetricStatTypeDef,
     TargetTrackingMetricStatTypeDef,
+    BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     RollbackDetailsTypeDef,
+    LaunchTemplateOverridesOutputTypeDef,
     LaunchTemplateOverridesTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     LaunchConfigurationsTypeTypeDef,
+    MetricDataQueryOutputTypeDef,
+    TargetTrackingMetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TargetTrackingMetricDataQueryTypeDef,
+    LaunchTemplateOutputTypeDef,
     LaunchTemplateTypeDef,
+    PredictiveScalingCustomizedCapacityMetricOutputTypeDef,
+    PredictiveScalingCustomizedLoadMetricOutputTypeDef,
+    PredictiveScalingCustomizedScalingMetricOutputTypeDef,
+    CustomizedMetricSpecificationOutputTypeDef,
     PredictiveScalingCustomizedCapacityMetricTypeDef,
     PredictiveScalingCustomizedLoadMetricTypeDef,
     PredictiveScalingCustomizedScalingMetricTypeDef,
     CustomizedMetricSpecificationTypeDef,
+    MixedInstancesPolicyOutputTypeDef,
     MixedInstancesPolicyTypeDef,
+    PredictiveScalingMetricSpecificationOutputTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
     PredictiveScalingMetricSpecificationTypeDef,
     TargetTrackingConfigurationTypeDef,
     AutoScalingGroupTypeDef,
+    DesiredConfigurationOutputTypeDef,
     CreateAutoScalingGroupTypeRequestTypeDef,
     DesiredConfigurationTypeDef,
+    MixedInstancesPolicyUnionTypeDef,
     UpdateAutoScalingGroupTypeRequestTypeDef,
     LoadForecastTypeDef,
+    PredictiveScalingConfigurationOutputTypeDef,
     PredictiveScalingConfigurationTypeDef,
+    TargetTrackingConfigurationUnionTypeDef,
     AutoScalingGroupsTypeTypeDef,
     InstanceRefreshTypeDef,
+    DesiredConfigurationUnionTypeDef,
     StartInstanceRefreshTypeRequestTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
-    PutScalingPolicyTypeRequestTypeDef,
     ScalingPolicyTypeDef,
+    PredictiveScalingConfigurationUnionTypeDef,
+    PutScalingPolicyTypeRequestTypeDef,
     DescribeInstanceRefreshesAnswerTypeDef,
     PoliciesTypeTypeDef,
 )
 
 
-def get_structure() -> AcceleratorCountRequestTypeDef:
+def get_value() -> AcceleratorCountRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-autoscaling-2.5.2/README.md` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-autoscaling
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AutoScaling 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore autoscaling type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-autoscaling"></a>
 
 # types-aiobotocore-autoscaling
 
 [![PyPI - types-aiobotocore-autoscaling](https://img.shields.io/pypi/v/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-autoscaling?color=blue)](https://pypistats.org/packages/types-aiobotocore-autoscaling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling)](https://pepy.tech/project/types-aiobotocore-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AutoScaling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [types-aiobotocore-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/).
 
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
@@ -345,203 +377,227 @@
 )
 
 
 def check_value(value: AcceleratorManufacturerType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_autoscaling.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_autoscaling.type_defs import (
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
+    ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     EnabledMetricTypeDef,
     LaunchTemplateSpecificationTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
-    ScheduledUpdateGroupActionRequestTypeDef,
     EbsTypeDef,
-    CancelInstanceRefreshAnswerTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
-    DescribeAccountLimitsAnswerTypeDef,
-    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
     DescribeAutoScalingInstancesTypeRequestTypeDef,
-    DescribeAutoScalingNotificationTypesAnswerTypeDef,
     DescribeInstanceRefreshesTypeRequestTypeDef,
-    DescribeLifecycleHookTypesAnswerTypeDef,
     LifecycleHookTypeDef,
     DescribeLifecycleHooksTypeRequestTypeDef,
-    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     DescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
     LoadBalancerTargetGroupStateTypeDef,
-    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     DescribeLoadBalancersRequestRequestTypeDef,
     LoadBalancerStateTypeDef,
     MetricCollectionTypeTypeDef,
     MetricGranularityTypeTypeDef,
     NotificationConfigurationTypeDef,
-    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
     DescribeNotificationConfigurationsTypeRequestTypeDef,
-    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
     DescribePoliciesTypeRequestTypeDef,
-    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingActivitiesTypeRequestTypeDef,
-    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
-    DescribeScheduledActionsTypeRequestTypeDef,
-    DescribeTerminationPolicyTypesAnswerTypeDef,
+    TimestampTypeDef,
     DescribeTrafficSourcesRequestRequestTypeDef,
     TrafficSourceStateTypeDef,
     DescribeWarmPoolTypeRequestTypeDef,
     DetachInstancesQueryRequestTypeDef,
     DetachLoadBalancerTargetGroupsTypeRequestTypeDef,
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
-    GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
-    RefreshPreferencesTypeDef,
+    RefreshPreferencesOutputTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
     InstanceReusePolicyTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
-    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
-    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
-    PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RollbackInstanceRefreshAnswerTypeDef,
+    RefreshPreferencesTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
-    StartInstanceRefreshAnswerTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
+    CancelInstanceRefreshAnswerTypeDef,
+    DescribeAccountLimitsAnswerTypeDef,
+    DescribeAutoScalingNotificationTypesAnswerTypeDef,
+    DescribeLifecycleHookTypesAnswerTypeDef,
+    DescribeTerminationPolicyTypesAnswerTypeDef,
     DetachInstancesAnswerTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
+    RollbackInstanceRefreshAnswerTypeDef,
+    StartInstanceRefreshAnswerTypeDef,
     DescribeAdjustmentTypesAnswerTypeDef,
     PolicyARNTypeTypeDef,
     AttachTrafficSourcesTypeRequestTypeDef,
     DetachTrafficSourcesTypeRequestTypeDef,
-    AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
     AutoScalingGroupNamesTypeRequestTypeDef,
-    DescribeTagsTypeDescribeTagsPaginateTypeDef,
     DescribeTagsTypeRequestTypeDef,
+    AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
+    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
+    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
+    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
+    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
+    DescribeTagsTypeDescribeTagsPaginateTypeDef,
+    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
-    BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
+    DescribeScheduledActionsTypeRequestTypeDef,
+    GetPredictiveScalingForecastTypeRequestTypeDef,
+    PutScheduledUpdateGroupActionTypeRequestTypeDef,
+    ScheduledUpdateGroupActionRequestTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
+    InstanceRequirementsOutputTypeDef,
     InstanceRequirementsTypeDef,
     PutWarmPoolTypeRequestTypeDef,
     WarmPoolConfigurationTypeDef,
     ProcessesTypeTypeDef,
+    RefreshPreferencesUnionTypeDef,
     ScheduledActionsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     CreateLaunchConfigurationTypeRequestTypeDef,
     LaunchConfigurationTypeDef,
+    MetricStatOutputTypeDef,
+    TargetTrackingMetricStatOutputTypeDef,
     MetricStatTypeDef,
     TargetTrackingMetricStatTypeDef,
+    BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     RollbackDetailsTypeDef,
+    LaunchTemplateOverridesOutputTypeDef,
     LaunchTemplateOverridesTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     LaunchConfigurationsTypeTypeDef,
+    MetricDataQueryOutputTypeDef,
+    TargetTrackingMetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TargetTrackingMetricDataQueryTypeDef,
+    LaunchTemplateOutputTypeDef,
     LaunchTemplateTypeDef,
+    PredictiveScalingCustomizedCapacityMetricOutputTypeDef,
+    PredictiveScalingCustomizedLoadMetricOutputTypeDef,
+    PredictiveScalingCustomizedScalingMetricOutputTypeDef,
+    CustomizedMetricSpecificationOutputTypeDef,
     PredictiveScalingCustomizedCapacityMetricTypeDef,
     PredictiveScalingCustomizedLoadMetricTypeDef,
     PredictiveScalingCustomizedScalingMetricTypeDef,
     CustomizedMetricSpecificationTypeDef,
+    MixedInstancesPolicyOutputTypeDef,
     MixedInstancesPolicyTypeDef,
+    PredictiveScalingMetricSpecificationOutputTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
     PredictiveScalingMetricSpecificationTypeDef,
     TargetTrackingConfigurationTypeDef,
     AutoScalingGroupTypeDef,
+    DesiredConfigurationOutputTypeDef,
     CreateAutoScalingGroupTypeRequestTypeDef,
     DesiredConfigurationTypeDef,
+    MixedInstancesPolicyUnionTypeDef,
     UpdateAutoScalingGroupTypeRequestTypeDef,
     LoadForecastTypeDef,
+    PredictiveScalingConfigurationOutputTypeDef,
     PredictiveScalingConfigurationTypeDef,
+    TargetTrackingConfigurationUnionTypeDef,
     AutoScalingGroupsTypeTypeDef,
     InstanceRefreshTypeDef,
+    DesiredConfigurationUnionTypeDef,
     StartInstanceRefreshTypeRequestTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
-    PutScalingPolicyTypeRequestTypeDef,
     ScalingPolicyTypeDef,
+    PredictiveScalingConfigurationUnionTypeDef,
+    PutScalingPolicyTypeRequestTypeDef,
     DescribeInstanceRefreshesAnswerTypeDef,
     PoliciesTypeTypeDef,
 )
 
 
-def get_structure() -> AcceleratorCountRequestTypeDef:
+def get_value() -> AcceleratorCountRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-autoscaling-2.5.2/setup.py` & `types-aiobotocore-autoscaling-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-autoscaling",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AutoScaling 2.5.2 service generated with"
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
-    keywords="aiobotocore autoscaling type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore autoscaling type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_autoscaling": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/"
```

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/__init__.py` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/__init__.pyi` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/__main__.py` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AutoScaling 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.AutoScaling 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling\nOther"
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

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/client.py` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("autoscaling") as client:
         client: AutoScalingClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import WarmPoolStateType
 from .paginator import (
     DescribeAutoScalingGroupsPaginator,
@@ -52,41 +51,42 @@
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTerminationPolicyTypesAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     DescribeWarmPoolAnswerTypeDef,
-    DesiredConfigurationTypeDef,
+    DesiredConfigurationUnionTypeDef,
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     FilterTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     InstanceReusePolicyTypeDef,
     LaunchConfigurationsTypeTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
-    MixedInstancesPolicyTypeDef,
+    MixedInstancesPolicyUnionTypeDef,
     PoliciesTypeTypeDef,
     PolicyARNTypeTypeDef,
-    PredictiveScalingConfigurationTypeDef,
+    PredictiveScalingConfigurationUnionTypeDef,
     ProcessesTypeTypeDef,
-    RefreshPreferencesTypeDef,
+    RefreshPreferencesUnionTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     ScheduledActionsTypeTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     StepAdjustmentTypeDef,
     TagsTypeTypeDef,
     TagTypeDef,
-    TargetTrackingConfigurationTypeDef,
+    TargetTrackingConfigurationUnionTypeDef,
+    TimestampTypeDef,
     TrafficSourceIdentifierTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -245,15 +245,15 @@
         self,
         *,
         AutoScalingGroupName: str,
         MinSize: int,
         MaxSize: int,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: MixedInstancesPolicyTypeDef = ...,
+        MixedInstancesPolicy: MixedInstancesPolicyUnionTypeDef = ...,
         InstanceId: str = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         LoadBalancerNames: Sequence[str] = ...,
         TargetGroupARNs: Sequence[str] = ...,
         HealthCheckType: str = ...,
@@ -584,16 +584,16 @@
         """
 
     async def describe_scheduled_actions(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxRecords: int = ...
     ) -> ScheduledActionsTypeTypeDef:
         """
         Gets information about the scheduled actions that haven't run or that have not
         reached their end time.
 
@@ -765,16 +765,16 @@
         """
 
     async def get_predictive_scaling_forecast(
         self,
         *,
         AutoScalingGroupName: str,
         PolicyName: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str]
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef
     ) -> GetPredictiveScalingForecastAnswerTypeDef:
         """
         Retrieves the forecast data for a predictive scaling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_predictive_scaling_forecast)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#get_predictive_scaling_forecast)
         """
@@ -819,33 +819,33 @@
         MinAdjustmentStep: int = ...,
         MinAdjustmentMagnitude: int = ...,
         ScalingAdjustment: int = ...,
         Cooldown: int = ...,
         MetricAggregationType: str = ...,
         StepAdjustments: Sequence[StepAdjustmentTypeDef] = ...,
         EstimatedInstanceWarmup: int = ...,
-        TargetTrackingConfiguration: TargetTrackingConfigurationTypeDef = ...,
+        TargetTrackingConfiguration: TargetTrackingConfigurationUnionTypeDef = ...,
         Enabled: bool = ...,
-        PredictiveScalingConfiguration: PredictiveScalingConfigurationTypeDef = ...
+        PredictiveScalingConfiguration: PredictiveScalingConfigurationUnionTypeDef = ...
     ) -> PolicyARNTypeTypeDef:
         """
         Creates or updates a scaling policy for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#put_scaling_policy)
         """
 
     async def put_scheduled_update_group_action(
         self,
         *,
         AutoScalingGroupName: str,
         ScheduledActionName: str,
-        Time: Union[datetime, str] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        Time: TimestampTypeDef = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Recurrence: str = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
         TimeZone: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
@@ -940,16 +940,16 @@
         """
 
     async def start_instance_refresh(
         self,
         *,
         AutoScalingGroupName: str,
         Strategy: Literal["Rolling"] = ...,
-        DesiredConfiguration: DesiredConfigurationTypeDef = ...,
-        Preferences: RefreshPreferencesTypeDef = ...
+        DesiredConfiguration: DesiredConfigurationUnionTypeDef = ...,
+        Preferences: RefreshPreferencesUnionTypeDef = ...
     ) -> StartInstanceRefreshAnswerTypeDef:
         """
         Starts an instance refresh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.start_instance_refresh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#start_instance_refresh)
         """
@@ -977,15 +977,15 @@
 
     async def update_auto_scaling_group(
         self,
         *,
         AutoScalingGroupName: str,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: MixedInstancesPolicyTypeDef = ...,
+        MixedInstancesPolicy: MixedInstancesPolicyUnionTypeDef = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         HealthCheckType: str = ...,
         HealthCheckGracePeriod: int = ...,
```

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/client.pyi` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("autoscaling") as client:
         client: AutoScalingClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import WarmPoolStateType
 from .paginator import (
     DescribeAutoScalingGroupsPaginator,
@@ -52,41 +51,42 @@
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTerminationPolicyTypesAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     DescribeWarmPoolAnswerTypeDef,
-    DesiredConfigurationTypeDef,
+    DesiredConfigurationUnionTypeDef,
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     FilterTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     InstanceReusePolicyTypeDef,
     LaunchConfigurationsTypeTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
-    MixedInstancesPolicyTypeDef,
+    MixedInstancesPolicyUnionTypeDef,
     PoliciesTypeTypeDef,
     PolicyARNTypeTypeDef,
-    PredictiveScalingConfigurationTypeDef,
+    PredictiveScalingConfigurationUnionTypeDef,
     ProcessesTypeTypeDef,
-    RefreshPreferencesTypeDef,
+    RefreshPreferencesUnionTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     ScheduledActionsTypeTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     StepAdjustmentTypeDef,
     TagsTypeTypeDef,
     TagTypeDef,
-    TargetTrackingConfigurationTypeDef,
+    TargetTrackingConfigurationUnionTypeDef,
+    TimestampTypeDef,
     TrafficSourceIdentifierTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -230,15 +230,15 @@
         self,
         *,
         AutoScalingGroupName: str,
         MinSize: int,
         MaxSize: int,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: MixedInstancesPolicyTypeDef = ...,
+        MixedInstancesPolicy: MixedInstancesPolicyUnionTypeDef = ...,
         InstanceId: str = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         LoadBalancerNames: Sequence[str] = ...,
         TargetGroupARNs: Sequence[str] = ...,
         HealthCheckType: str = ...,
@@ -542,16 +542,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#describe_scaling_process_types)
         """
     async def describe_scheduled_actions(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxRecords: int = ...
     ) -> ScheduledActionsTypeTypeDef:
         """
         Gets information about the scheduled actions that haven't run or that have not
         reached their end time.
 
@@ -708,16 +708,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#generate_presigned_url)
         """
     async def get_predictive_scaling_forecast(
         self,
         *,
         AutoScalingGroupName: str,
         PolicyName: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str]
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef
     ) -> GetPredictiveScalingForecastAnswerTypeDef:
         """
         Retrieves the forecast data for a predictive scaling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.get_predictive_scaling_forecast)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#get_predictive_scaling_forecast)
         """
@@ -759,32 +759,32 @@
         MinAdjustmentStep: int = ...,
         MinAdjustmentMagnitude: int = ...,
         ScalingAdjustment: int = ...,
         Cooldown: int = ...,
         MetricAggregationType: str = ...,
         StepAdjustments: Sequence[StepAdjustmentTypeDef] = ...,
         EstimatedInstanceWarmup: int = ...,
-        TargetTrackingConfiguration: TargetTrackingConfigurationTypeDef = ...,
+        TargetTrackingConfiguration: TargetTrackingConfigurationUnionTypeDef = ...,
         Enabled: bool = ...,
-        PredictiveScalingConfiguration: PredictiveScalingConfigurationTypeDef = ...
+        PredictiveScalingConfiguration: PredictiveScalingConfigurationUnionTypeDef = ...
     ) -> PolicyARNTypeTypeDef:
         """
         Creates or updates a scaling policy for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#put_scaling_policy)
         """
     async def put_scheduled_update_group_action(
         self,
         *,
         AutoScalingGroupName: str,
         ScheduledActionName: str,
-        Time: Union[datetime, str] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        Time: TimestampTypeDef = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         Recurrence: str = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
         TimeZone: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
@@ -871,16 +871,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#set_instance_protection)
         """
     async def start_instance_refresh(
         self,
         *,
         AutoScalingGroupName: str,
         Strategy: Literal["Rolling"] = ...,
-        DesiredConfiguration: DesiredConfigurationTypeDef = ...,
-        Preferences: RefreshPreferencesTypeDef = ...
+        DesiredConfiguration: DesiredConfigurationUnionTypeDef = ...,
+        Preferences: RefreshPreferencesUnionTypeDef = ...
     ) -> StartInstanceRefreshAnswerTypeDef:
         """
         Starts an instance refresh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.start_instance_refresh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#start_instance_refresh)
         """
@@ -905,15 +905,15 @@
         """
     async def update_auto_scaling_group(
         self,
         *,
         AutoScalingGroupName: str,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: MixedInstancesPolicyTypeDef = ...,
+        MixedInstancesPolicy: MixedInstancesPolicyUnionTypeDef = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         HealthCheckType: str = ...,
         HealthCheckGracePeriod: int = ...,
```

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/literals.py` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/literals.pyi` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/paginator.py` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         describe_notification_configurations_paginator: DescribeNotificationConfigurationsPaginator = client.get_paginator("describe_notification_configurations")
         describe_policies_paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
         describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
         describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
         describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ActivitiesTypeTypeDef,
     AutoScalingGroupsTypeTypeDef,
@@ -53,14 +52,15 @@
     DescribeNotificationConfigurationsAnswerTypeDef,
     FilterTypeDef,
     LaunchConfigurationsTypeTypeDef,
     PaginatorConfigTypeDef,
     PoliciesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     TagsTypeTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeAutoScalingGroupsPaginator",
     "DescribeAutoScalingInstancesPaginator",
     "DescribeLaunchConfigurationsPaginator",
     "DescribeLoadBalancerTargetGroupsPaginator",
@@ -90,30 +90,30 @@
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[AutoScalingGroupsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeautoscalinggroupspaginator)
         """
 
 
 class DescribeAutoScalingInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeautoscalinginstancespaginator)
     """
 
     def paginate(
-        self, *, InstanceIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[AutoScalingInstancesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeautoscalinginstancespaginator)
         """
 
 
@@ -123,45 +123,45 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describelaunchconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         LaunchConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[LaunchConfigurationsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLaunchConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describelaunchconfigurationspaginator)
         """
 
 
 class DescribeLoadBalancerTargetGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeloadbalancertargetgroupspaginator)
     """
 
     def paginate(
-        self, *, AutoScalingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeLoadBalancerTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeloadbalancertargetgroupspaginator)
         """
 
 
 class DescribeLoadBalancersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
-        self, *, AutoScalingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeLoadBalancersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeloadbalancerspaginator)
         """
 
 
@@ -171,15 +171,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describenotificationconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeNotificationConfigurationsAnswerTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeNotificationConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describenotificationconfigurationspaginator)
         """
 
 
@@ -191,15 +191,15 @@
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         PolicyNames: Sequence[str] = ...,
         PolicyTypes: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[PoliciesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describepoliciespaginator)
         """
 
 
@@ -211,15 +211,15 @@
 
     def paginate(
         self,
         *,
         ActivityIds: Sequence[str] = ...,
         AutoScalingGroupName: str = ...,
         IncludeDeletedGroups: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ActivitiesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
 
@@ -230,17 +230,17 @@
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ScheduledActionsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describescheduledactionspaginator)
         """
 
 
@@ -250,13 +250,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[TagsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describetagspaginator)
         """
```

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/paginator.pyi` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         describe_notification_configurations_paginator: DescribeNotificationConfigurationsPaginator = client.get_paginator("describe_notification_configurations")
         describe_policies_paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
         describe_scaling_activities_paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
         describe_scheduled_actions_paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
         describe_tags_paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     ActivitiesTypeTypeDef,
     AutoScalingGroupsTypeTypeDef,
@@ -53,14 +52,15 @@
     DescribeNotificationConfigurationsAnswerTypeDef,
     FilterTypeDef,
     LaunchConfigurationsTypeTypeDef,
     PaginatorConfigTypeDef,
     PoliciesTypeTypeDef,
     ScheduledActionsTypeTypeDef,
     TagsTypeTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeAutoScalingGroupsPaginator",
     "DescribeAutoScalingInstancesPaginator",
     "DescribeLaunchConfigurationsPaginator",
     "DescribeLoadBalancerTargetGroupsPaginator",
@@ -87,29 +87,29 @@
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[AutoScalingGroupsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeautoscalinggroupspaginator)
         """
 
 class DescribeAutoScalingInstancesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeautoscalinginstancespaginator)
     """
 
     def paginate(
-        self, *, InstanceIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InstanceIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[AutoScalingInstancesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeautoscalinginstancespaginator)
         """
 
 class DescribeLaunchConfigurationsPaginator(AioPaginator):
@@ -118,43 +118,43 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describelaunchconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         LaunchConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[LaunchConfigurationsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLaunchConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describelaunchconfigurationspaginator)
         """
 
 class DescribeLoadBalancerTargetGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeloadbalancertargetgroupspaginator)
     """
 
     def paginate(
-        self, *, AutoScalingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeLoadBalancerTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeloadbalancertargetgroupspaginator)
         """
 
 class DescribeLoadBalancersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeloadbalancerspaginator)
     """
 
     def paginate(
-        self, *, AutoScalingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AutoScalingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeLoadBalancersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describeloadbalancerspaginator)
         """
 
 class DescribeNotificationConfigurationsPaginator(AioPaginator):
@@ -163,15 +163,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describenotificationconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeNotificationConfigurationsAnswerTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeNotificationConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describenotificationconfigurationspaginator)
         """
 
 class DescribePoliciesPaginator(AioPaginator):
@@ -182,15 +182,15 @@
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         PolicyNames: Sequence[str] = ...,
         PolicyTypes: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[PoliciesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describepoliciespaginator)
         """
 
 class DescribeScalingActivitiesPaginator(AioPaginator):
@@ -201,15 +201,15 @@
 
     def paginate(
         self,
         *,
         ActivityIds: Sequence[str] = ...,
         AutoScalingGroupName: str = ...,
         IncludeDeletedGroups: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ActivitiesTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
 class DescribeScheduledActionsPaginator(AioPaginator):
@@ -219,17 +219,17 @@
     """
 
     def paginate(
         self,
         *,
         AutoScalingGroupName: str = ...,
         ScheduledActionNames: Sequence[str] = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ScheduledActionsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describescheduledactionspaginator)
         """
 
 class DescribeTagsPaginator(AioPaginator):
@@ -238,13 +238,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[TagsTypeTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/paginators/#describetagspaginator)
         """
```

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/type_defs.py` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_autoscaling.type_defs import AcceleratorCountRequestTypeDef
 
-    data: AcceleratorCountRequestTypeDef = {...}
+    data: AcceleratorCountRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -52,185 +52,209 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
+    "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
     "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "EnabledMetricTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "SuspendedProcessTypeDef",
     "TagDescriptionTypeDef",
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     "FailedScheduledUpdateGroupActionRequestTypeDef",
     "BatchDeleteScheduledActionTypeRequestTypeDef",
-    "ScheduledUpdateGroupActionRequestTypeDef",
     "EbsTypeDef",
-    "CancelInstanceRefreshAnswerTypeDef",
     "CancelInstanceRefreshTypeRequestTypeDef",
     "CapacityForecastTypeDef",
     "CompleteLifecycleActionTypeRequestTypeDef",
     "LifecycleHookSpecificationTypeDef",
     "TagTypeDef",
     "InstanceMetadataOptionsTypeDef",
     "InstanceMonitoringTypeDef",
     "MetricDimensionTypeDef",
     "DeleteAutoScalingGroupTypeRequestTypeDef",
     "DeleteLifecycleHookTypeRequestTypeDef",
     "DeleteNotificationConfigurationTypeRequestTypeDef",
     "DeletePolicyTypeRequestTypeDef",
     "DeleteScheduledActionTypeRequestTypeDef",
     "DeleteWarmPoolTypeRequestTypeDef",
-    "DescribeAccountLimitsAnswerTypeDef",
-    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
-    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
     "DescribeInstanceRefreshesTypeRequestTypeDef",
-    "DescribeLifecycleHookTypesAnswerTypeDef",
     "LifecycleHookTypeDef",
     "DescribeLifecycleHooksTypeRequestTypeDef",
-    "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
     "DescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     "LoadBalancerTargetGroupStateTypeDef",
-    "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     "DescribeLoadBalancersRequestRequestTypeDef",
     "LoadBalancerStateTypeDef",
     "MetricCollectionTypeTypeDef",
     "MetricGranularityTypeTypeDef",
     "NotificationConfigurationTypeDef",
-    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
-    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
     "DescribePoliciesTypeRequestTypeDef",
-    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
     "DescribeScalingActivitiesTypeRequestTypeDef",
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
-    "DescribeScheduledActionsTypeRequestTypeDef",
-    "DescribeTerminationPolicyTypesAnswerTypeDef",
+    "TimestampTypeDef",
     "DescribeTrafficSourcesRequestRequestTypeDef",
     "TrafficSourceStateTypeDef",
     "DescribeWarmPoolTypeRequestTypeDef",
     "DetachInstancesQueryRequestTypeDef",
     "DetachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "DetachLoadBalancersTypeRequestTypeDef",
     "DisableMetricsCollectionQueryRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
-    "GetPredictiveScalingForecastTypeRequestTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
-    "RefreshPreferencesTypeDef",
+    "RefreshPreferencesOutputTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
     "InstanceReusePolicyTypeDef",
     "InstancesDistributionTypeDef",
     "LaunchConfigurationNameTypeRequestTypeDef",
-    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "LaunchConfigurationNamesTypeRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "PredictiveScalingPredefinedLoadMetricTypeDef",
     "PredictiveScalingPredefinedMetricPairTypeDef",
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
-    "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "RollbackInstanceRefreshAnswerTypeDef",
+    "RefreshPreferencesTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
-    "StartInstanceRefreshAnswerTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     "ActivitiesTypeTypeDef",
     "ActivityTypeTypeDef",
+    "CancelInstanceRefreshAnswerTypeDef",
+    "DescribeAccountLimitsAnswerTypeDef",
+    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
+    "DescribeLifecycleHookTypesAnswerTypeDef",
+    "DescribeTerminationPolicyTypesAnswerTypeDef",
     "DetachInstancesAnswerTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnterStandbyAnswerTypeDef",
     "ExitStandbyAnswerTypeDef",
+    "RollbackInstanceRefreshAnswerTypeDef",
+    "StartInstanceRefreshAnswerTypeDef",
     "DescribeAdjustmentTypesAnswerTypeDef",
     "PolicyARNTypeTypeDef",
     "AttachTrafficSourcesTypeRequestTypeDef",
     "DetachTrafficSourcesTypeRequestTypeDef",
-    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
     "AutoScalingGroupNamesTypeRequestTypeDef",
-    "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     "DescribeTagsTypeRequestTypeDef",
+    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
+    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
+    "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
+    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
+    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
+    "DescribeTagsTypeDescribeTagsPaginateTypeDef",
+    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
-    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "BlockDeviceMappingTypeDef",
     "CreateOrUpdateTagsTypeRequestTypeDef",
     "DeleteTagsTypeRequestTypeDef",
+    "MetricOutputTypeDef",
     "MetricTypeDef",
     "DescribeLifecycleHooksAnswerTypeDef",
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     "DescribeLoadBalancersResponseTypeDef",
     "DescribeMetricCollectionTypesAnswerTypeDef",
     "DescribeNotificationConfigurationsAnswerTypeDef",
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    "DescribeScheduledActionsTypeRequestTypeDef",
+    "GetPredictiveScalingForecastTypeRequestTypeDef",
+    "PutScheduledUpdateGroupActionTypeRequestTypeDef",
+    "ScheduledUpdateGroupActionRequestTypeDef",
     "DescribeTrafficSourcesResponseTypeDef",
     "InstanceRefreshProgressDetailsTypeDef",
+    "InstanceRequirementsOutputTypeDef",
     "InstanceRequirementsTypeDef",
     "PutWarmPoolTypeRequestTypeDef",
     "WarmPoolConfigurationTypeDef",
     "ProcessesTypeTypeDef",
+    "RefreshPreferencesUnionTypeDef",
     "ScheduledActionsTypeTypeDef",
     "AutoScalingInstancesTypeTypeDef",
     "CreateLaunchConfigurationTypeRequestTypeDef",
     "LaunchConfigurationTypeDef",
+    "MetricStatOutputTypeDef",
+    "TargetTrackingMetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "TargetTrackingMetricStatTypeDef",
+    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RollbackDetailsTypeDef",
+    "LaunchTemplateOverridesOutputTypeDef",
     "LaunchTemplateOverridesTypeDef",
     "DescribeWarmPoolAnswerTypeDef",
     "LaunchConfigurationsTypeTypeDef",
+    "MetricDataQueryOutputTypeDef",
+    "TargetTrackingMetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
     "TargetTrackingMetricDataQueryTypeDef",
+    "LaunchTemplateOutputTypeDef",
     "LaunchTemplateTypeDef",
+    "PredictiveScalingCustomizedCapacityMetricOutputTypeDef",
+    "PredictiveScalingCustomizedLoadMetricOutputTypeDef",
+    "PredictiveScalingCustomizedScalingMetricOutputTypeDef",
+    "CustomizedMetricSpecificationOutputTypeDef",
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     "CustomizedMetricSpecificationTypeDef",
+    "MixedInstancesPolicyOutputTypeDef",
     "MixedInstancesPolicyTypeDef",
+    "PredictiveScalingMetricSpecificationOutputTypeDef",
+    "TargetTrackingConfigurationOutputTypeDef",
     "PredictiveScalingMetricSpecificationTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
+    "DesiredConfigurationOutputTypeDef",
     "CreateAutoScalingGroupTypeRequestTypeDef",
     "DesiredConfigurationTypeDef",
+    "MixedInstancesPolicyUnionTypeDef",
     "UpdateAutoScalingGroupTypeRequestTypeDef",
     "LoadForecastTypeDef",
+    "PredictiveScalingConfigurationOutputTypeDef",
     "PredictiveScalingConfigurationTypeDef",
+    "TargetTrackingConfigurationUnionTypeDef",
     "AutoScalingGroupsTypeTypeDef",
     "InstanceRefreshTypeDef",
+    "DesiredConfigurationUnionTypeDef",
     "StartInstanceRefreshTypeRequestTypeDef",
     "GetPredictiveScalingForecastAnswerTypeDef",
-    "PutScalingPolicyTypeRequestTypeDef",
     "ScalingPolicyTypeDef",
+    "PredictiveScalingConfigurationUnionTypeDef",
+    "PutScalingPolicyTypeRequestTypeDef",
     "DescribeInstanceRefreshesAnswerTypeDef",
     "PoliciesTypeTypeDef",
 )
 
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
     {
@@ -274,14 +298,25 @@
 )
 
 
 class ActivityTypeDef(_RequiredActivityTypeDef, _OptionalActivityTypeDef):
     pass
 
 
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
 AdjustmentTypeTypeDef = TypedDict(
     "AdjustmentTypeTypeDef",
     {
         "AdjustmentType": str,
     },
     total=False,
 )
@@ -358,14 +393,24 @@
     {
         "Name": str,
         "Values": Sequence[str],
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
 EnabledMetricTypeDef = TypedDict(
     "EnabledMetricTypeDef",
     {
         "Metric": str,
         "Granularity": str,
     },
     total=False,
@@ -438,64 +483,28 @@
     "BatchDeleteScheduledActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledActionNames": Sequence[str],
     },
 )
 
-_RequiredScheduledUpdateGroupActionRequestTypeDef = TypedDict(
-    "_RequiredScheduledUpdateGroupActionRequestTypeDef",
-    {
-        "ScheduledActionName": str,
-    },
-)
-_OptionalScheduledUpdateGroupActionRequestTypeDef = TypedDict(
-    "_OptionalScheduledUpdateGroupActionRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Recurrence": str,
-        "MinSize": int,
-        "MaxSize": int,
-        "DesiredCapacity": int,
-        "TimeZone": str,
-    },
-    total=False,
-)
-
-
-class ScheduledUpdateGroupActionRequestTypeDef(
-    _RequiredScheduledUpdateGroupActionRequestTypeDef,
-    _OptionalScheduledUpdateGroupActionRequestTypeDef,
-):
-    pass
-
-
 EbsTypeDef = TypedDict(
     "EbsTypeDef",
     {
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": str,
         "DeleteOnTermination": bool,
         "Iops": int,
         "Encrypted": bool,
         "Throughput": int,
     },
     total=False,
 )
 
-CancelInstanceRefreshAnswerTypeDef = TypedDict(
-    "CancelInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CancelInstanceRefreshTypeRequestTypeDef = TypedDict(
     "CancelInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 
@@ -690,52 +699,24 @@
 
 class DeleteWarmPoolTypeRequestTypeDef(
     _RequiredDeleteWarmPoolTypeRequestTypeDef, _OptionalDeleteWarmPoolTypeRequestTypeDef
 ):
     pass
 
 
-DescribeAccountLimitsAnswerTypeDef = TypedDict(
-    "DescribeAccountLimitsAnswerTypeDef",
-    {
-        "MaxNumberOfAutoScalingGroups": int,
-        "MaxNumberOfLaunchConfigurations": int,
-        "NumberOfAutoScalingGroups": int,
-        "NumberOfLaunchConfigurations": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef = TypedDict(
-    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAutoScalingInstancesTypeRequestTypeDef = TypedDict(
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeAutoScalingNotificationTypesAnswerTypeDef = TypedDict(
-    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
-    {
-        "AutoScalingNotificationTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeInstanceRefreshesTypeRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceRefreshesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeInstanceRefreshesTypeRequestTypeDef = TypedDict(
@@ -752,22 +733,14 @@
 class DescribeInstanceRefreshesTypeRequestTypeDef(
     _RequiredDescribeInstanceRefreshesTypeRequestTypeDef,
     _OptionalDescribeInstanceRefreshesTypeRequestTypeDef,
 ):
     pass
 
 
-DescribeLifecycleHookTypesAnswerTypeDef = TypedDict(
-    "DescribeLifecycleHookTypesAnswerTypeDef",
-    {
-        "LifecycleHookTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifecycleHookTypeDef = TypedDict(
     "LifecycleHookTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
         "LifecycleTransition": str,
         "NotificationTargetARN": str,
@@ -798,36 +771,14 @@
 class DescribeLifecycleHooksTypeRequestTypeDef(
     _RequiredDescribeLifecycleHooksTypeRequestTypeDef,
     _OptionalDescribeLifecycleHooksTypeRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-    },
-)
-_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
-    _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-    _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
@@ -852,36 +803,14 @@
     {
         "LoadBalancerTargetGroupARN": str,
         "State": str,
     },
     total=False,
 )
 
-_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-    },
-)
-_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
-    _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-    _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeLoadBalancersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancersRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancersRequestRequestTypeDef = TypedDict(
@@ -932,112 +861,49 @@
         "AutoScalingGroupName": str,
         "TopicARN": str,
         "NotificationType": str,
     },
     total=False,
 )
 
-DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
-    {
-        "AutoScalingGroupNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeNotificationConfigurationsTypeRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribePoliciesTypeDescribePoliciesPaginateTypeDef = TypedDict(
-    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "PolicyNames": Sequence[str],
-        "PolicyTypes": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribePoliciesTypeRequestTypeDef = TypedDict(
     "DescribePoliciesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyNames": Sequence[str],
         "PolicyTypes": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ActivityIds": Sequence[str],
-        "AutoScalingGroupName": str,
-        "IncludeDeletedGroups": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeScalingActivitiesTypeRequestTypeDef = TypedDict(
     "DescribeScalingActivitiesTypeRequestTypeDef",
     {
         "ActivityIds": Sequence[str],
         "AutoScalingGroupName": str,
         "IncludeDeletedGroups": bool,
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionNames": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-DescribeScheduledActionsTypeRequestTypeDef = TypedDict(
-    "DescribeScheduledActionsTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionNames": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxRecords": int,
-    },
-    total=False,
-)
-
-DescribeTerminationPolicyTypesAnswerTypeDef = TypedDict(
-    "DescribeTerminationPolicyTypesAnswerTypeDef",
-    {
-        "TerminationPolicyTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTrafficSourcesRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
@@ -1147,21 +1013,14 @@
 class DisableMetricsCollectionQueryRequestTypeDef(
     _RequiredDisableMetricsCollectionQueryRequestTypeDef,
     _OptionalDisableMetricsCollectionQueryRequestTypeDef,
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableMetricsCollectionQueryRequestTypeDef = TypedDict(
     "_RequiredEnableMetricsCollectionQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "Granularity": str,
     },
 )
@@ -1244,24 +1103,14 @@
 
 class ExitStandbyQueryRequestTypeDef(
     _RequiredExitStandbyQueryRequestTypeDef, _OptionalExitStandbyQueryRequestTypeDef
 ):
     pass
 
 
-GetPredictiveScalingForecastTypeRequestTypeDef = TypedDict(
-    "GetPredictiveScalingForecastTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "PolicyName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-
 InstanceRefreshLivePoolProgressTypeDef = TypedDict(
     "InstanceRefreshLivePoolProgressTypeDef",
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
@@ -1272,16 +1121,16 @@
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
 )
 
-RefreshPreferencesTypeDef = TypedDict(
-    "RefreshPreferencesTypeDef",
+RefreshPreferencesOutputTypeDef = TypedDict(
+    "RefreshPreferencesOutputTypeDef",
     {
         "MinHealthyPercentage": int,
         "InstanceWarmup": int,
         "CheckpointPercentages": List[int],
         "CheckpointDelay": int,
         "SkipMatching": bool,
         "AutoRollback": bool,
@@ -1389,43 +1238,24 @@
 LaunchConfigurationNameTypeRequestTypeDef = TypedDict(
     "LaunchConfigurationNameTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
     },
 )
 
-LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
-    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
-    {
-        "LaunchConfigurationNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 LaunchConfigurationNamesTypeRequestTypeDef = TypedDict(
     "LaunchConfigurationNamesTypeRequestTypeDef",
     {
         "LaunchConfigurationNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
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
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
@@ -1568,44 +1398,14 @@
 )
 
 
 class StepAdjustmentTypeDef(_RequiredStepAdjustmentTypeDef, _OptionalStepAdjustmentTypeDef):
     pass
 
 
-_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
-    "_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionName": str,
-    },
-)
-_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
-    "_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    {
-        "Time": Union[datetime, str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Recurrence": str,
-        "MinSize": int,
-        "MaxSize": int,
-        "DesiredCapacity": int,
-        "TimeZone": str,
-    },
-    total=False,
-)
-
-
-class PutScheduledUpdateGroupActionTypeRequestTypeDef(
-    _RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef,
-    _OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef,
-):
-    pass
-
-
 _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef = TypedDict(
     "_RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
     },
 )
@@ -1622,31 +1422,27 @@
 class RecordLifecycleActionHeartbeatTypeRequestTypeDef(
     _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef,
     _OptionalRecordLifecycleActionHeartbeatTypeRequestTypeDef,
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
-
-RollbackInstanceRefreshAnswerTypeDef = TypedDict(
-    "RollbackInstanceRefreshAnswerTypeDef",
+RefreshPreferencesTypeDef = TypedDict(
+    "RefreshPreferencesTypeDef",
     {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MinHealthyPercentage": int,
+        "InstanceWarmup": int,
+        "CheckpointPercentages": Sequence[int],
+        "CheckpointDelay": int,
+        "SkipMatching": bool,
+        "AutoRollback": bool,
+        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
+        "StandbyInstances": StandbyInstancesType,
     },
+    total=False,
 )
 
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
@@ -1741,85 +1537,143 @@
     {
         "InstanceIds": Sequence[str],
         "AutoScalingGroupName": str,
         "ProtectedFromScaleIn": bool,
     },
 )
 
-StartInstanceRefreshAnswerTypeDef = TypedDict(
-    "StartInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TerminateInstanceInAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     {
         "InstanceId": str,
         "ShouldDecrementDesiredCapacity": bool,
     },
 )
 
 ActivitiesTypeTypeDef = TypedDict(
     "ActivitiesTypeTypeDef",
     {
         "Activities": List[ActivityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActivityTypeTypeDef = TypedDict(
     "ActivityTypeTypeDef",
     {
         "Activity": ActivityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelInstanceRefreshAnswerTypeDef = TypedDict(
+    "CancelInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountLimitsAnswerTypeDef = TypedDict(
+    "DescribeAccountLimitsAnswerTypeDef",
+    {
+        "MaxNumberOfAutoScalingGroups": int,
+        "MaxNumberOfLaunchConfigurations": int,
+        "NumberOfAutoScalingGroups": int,
+        "NumberOfLaunchConfigurations": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAutoScalingNotificationTypesAnswerTypeDef = TypedDict(
+    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
+    {
+        "AutoScalingNotificationTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLifecycleHookTypesAnswerTypeDef = TypedDict(
+    "DescribeLifecycleHookTypesAnswerTypeDef",
+    {
+        "LifecycleHookTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTerminationPolicyTypesAnswerTypeDef = TypedDict(
+    "DescribeTerminationPolicyTypesAnswerTypeDef",
+    {
+        "TerminationPolicyTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetachInstancesAnswerTypeDef = TypedDict(
     "DetachInstancesAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnterStandbyAnswerTypeDef = TypedDict(
     "EnterStandbyAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExitStandbyAnswerTypeDef = TypedDict(
     "ExitStandbyAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackInstanceRefreshAnswerTypeDef = TypedDict(
+    "RollbackInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartInstanceRefreshAnswerTypeDef = TypedDict(
+    "StartInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAdjustmentTypesAnswerTypeDef = TypedDict(
     "DescribeAdjustmentTypesAnswerTypeDef",
     {
         "AdjustmentTypes": List[AdjustmentTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyARNTypeTypeDef = TypedDict(
     "PolicyARNTypeTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachTrafficSourcesTypeRequestTypeDef = TypedDict(
     "AttachTrafficSourcesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
@@ -1831,50 +1685,143 @@
     "DetachTrafficSourcesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "TrafficSources": Sequence[TrafficSourceIdentifierTypeDef],
     },
 )
 
-AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef = TypedDict(
-    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
+AutoScalingGroupNamesTypeRequestTypeDef = TypedDict(
+    "AutoScalingGroupNamesTypeRequestTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
+        "NextToken": str,
+        "MaxRecords": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-AutoScalingGroupNamesTypeRequestTypeDef = TypedDict(
-    "AutoScalingGroupNamesTypeRequestTypeDef",
+DescribeTagsTypeRequestTypeDef = TypedDict(
+    "DescribeTagsTypeRequestTypeDef",
     {
-        "AutoScalingGroupNames": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxRecords": int,
+    },
+    total=False,
+)
+
+AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef = TypedDict(
+    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
+    {
+        "AutoScalingGroupNames": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef = TypedDict(
+    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
+    _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+    _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
+    _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+    _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+):
+    pass
+
+
+DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
+    {
+        "AutoScalingGroupNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribePoliciesTypeDescribePoliciesPaginateTypeDef = TypedDict(
+    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "PolicyNames": Sequence[str],
+        "PolicyTypes": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
+    {
+        "ActivityIds": Sequence[str],
+        "AutoScalingGroupName": str,
+        "IncludeDeletedGroups": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeTagsTypeDescribeTagsPaginateTypeDef = TypedDict(
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeTagsTypeRequestTypeDef = TypedDict(
-    "DescribeTagsTypeRequestTypeDef",
+LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
+    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "NextToken": str,
-        "MaxRecords": int,
+        "LaunchConfigurationNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredAutoScalingInstanceDetailsTypeDef = TypedDict(
     "_RequiredAutoScalingInstanceDetailsTypeDef",
     {
@@ -1931,39 +1878,31 @@
 
 
 TagsTypeTypeDef = TypedDict(
     "TagsTypeTypeDef",
     {
         "Tags": List[TagDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteScheduledActionAnswerTypeDef = TypedDict(
     "BatchDeleteScheduledActionAnswerTypeDef",
     {
         "FailedScheduledActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutScheduledUpdateGroupActionAnswerTypeDef = TypedDict(
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     {
         "FailedScheduledUpdateGroupActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
-    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledUpdateGroupActions": Sequence[ScheduledUpdateGroupActionRequestTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBlockDeviceMappingTypeDef = TypedDict(
     "_RequiredBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
@@ -1996,96 +1935,251 @@
 DeleteTagsTypeRequestTypeDef = TypedDict(
     "DeleteTagsTypeRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredMetricOutputTypeDef = TypedDict(
+    "_RequiredMetricOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+    },
+)
+_OptionalMetricOutputTypeDef = TypedDict(
+    "_OptionalMetricOutputTypeDef",
+    {
+        "Dimensions": List[MetricDimensionTypeDef],
+    },
+    total=False,
+)
+
+
+class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
+    pass
+
+
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
 _OptionalMetricTypeDef = TypedDict(
     "_OptionalMetricTypeDef",
     {
-        "Dimensions": List[MetricDimensionTypeDef],
+        "Dimensions": Sequence[MetricDimensionTypeDef],
     },
     total=False,
 )
 
 
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
 
 DescribeLifecycleHooksAnswerTypeDef = TypedDict(
     "DescribeLifecycleHooksAnswerTypeDef",
     {
         "LifecycleHooks": List[LifecycleHookTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerTargetGroupsResponseTypeDef = TypedDict(
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     {
         "LoadBalancerTargetGroups": List[LoadBalancerTargetGroupStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancersResponseTypeDef = TypedDict(
     "DescribeLoadBalancersResponseTypeDef",
     {
         "LoadBalancers": List[LoadBalancerStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMetricCollectionTypesAnswerTypeDef = TypedDict(
     "DescribeMetricCollectionTypesAnswerTypeDef",
     {
         "Metrics": List[MetricCollectionTypeTypeDef],
         "Granularities": List[MetricGranularityTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotificationConfigurationsAnswerTypeDef = TypedDict(
     "DescribeNotificationConfigurationsAnswerTypeDef",
     {
         "NotificationConfigurations": List[NotificationConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionNames": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScheduledActionsTypeRequestTypeDef = TypedDict(
+    "DescribeScheduledActionsTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionNames": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxRecords": int,
     },
+    total=False,
 )
 
+GetPredictiveScalingForecastTypeRequestTypeDef = TypedDict(
+    "GetPredictiveScalingForecastTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "PolicyName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
+_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
+    "_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionName": str,
+    },
+)
+_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
+    "_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    {
+        "Time": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Recurrence": str,
+        "MinSize": int,
+        "MaxSize": int,
+        "DesiredCapacity": int,
+        "TimeZone": str,
+    },
+    total=False,
+)
+
+
+class PutScheduledUpdateGroupActionTypeRequestTypeDef(
+    _RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef,
+    _OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef,
+):
+    pass
+
+
+_RequiredScheduledUpdateGroupActionRequestTypeDef = TypedDict(
+    "_RequiredScheduledUpdateGroupActionRequestTypeDef",
+    {
+        "ScheduledActionName": str,
+    },
+)
+_OptionalScheduledUpdateGroupActionRequestTypeDef = TypedDict(
+    "_OptionalScheduledUpdateGroupActionRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Recurrence": str,
+        "MinSize": int,
+        "MaxSize": int,
+        "DesiredCapacity": int,
+        "TimeZone": str,
+    },
+    total=False,
+)
+
+
+class ScheduledUpdateGroupActionRequestTypeDef(
+    _RequiredScheduledUpdateGroupActionRequestTypeDef,
+    _OptionalScheduledUpdateGroupActionRequestTypeDef,
+):
+    pass
+
+
 DescribeTrafficSourcesResponseTypeDef = TypedDict(
     "DescribeTrafficSourcesResponseTypeDef",
     {
         "TrafficSources": List[TrafficSourceStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceRefreshProgressDetailsTypeDef = TypedDict(
     "InstanceRefreshProgressDetailsTypeDef",
     {
         "LivePoolProgress": InstanceRefreshLivePoolProgressTypeDef,
         "WarmPoolProgress": InstanceRefreshWarmPoolProgressTypeDef,
     },
     total=False,
 )
 
+_RequiredInstanceRequirementsOutputTypeDef = TypedDict(
+    "_RequiredInstanceRequirementsOutputTypeDef",
+    {
+        "VCpuCount": VCpuCountRequestTypeDef,
+        "MemoryMiB": MemoryMiBRequestTypeDef,
+    },
+)
+_OptionalInstanceRequirementsOutputTypeDef = TypedDict(
+    "_OptionalInstanceRequirementsOutputTypeDef",
+    {
+        "CpuManufacturers": List[CpuManufacturerType],
+        "MemoryGiBPerVCpu": MemoryGiBPerVCpuRequestTypeDef,
+        "ExcludedInstanceTypes": List[str],
+        "InstanceGenerations": List[InstanceGenerationType],
+        "SpotMaxPricePercentageOverLowestPrice": int,
+        "OnDemandMaxPricePercentageOverLowestPrice": int,
+        "BareMetal": BareMetalType,
+        "BurstablePerformance": BurstablePerformanceType,
+        "RequireHibernateSupport": bool,
+        "NetworkInterfaceCount": NetworkInterfaceCountRequestTypeDef,
+        "LocalStorage": LocalStorageType,
+        "LocalStorageTypes": List[LocalStorageTypeType],
+        "TotalLocalStorageGB": TotalLocalStorageGBRequestTypeDef,
+        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsRequestTypeDef,
+        "AcceleratorTypes": List[AcceleratorTypeType],
+        "AcceleratorCount": AcceleratorCountRequestTypeDef,
+        "AcceleratorManufacturers": List[AcceleratorManufacturerType],
+        "AcceleratorNames": List[AcceleratorNameType],
+        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestTypeDef,
+        "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestTypeDef,
+        "AllowedInstanceTypes": List[str],
+    },
+    total=False,
+)
+
+
+class InstanceRequirementsOutputTypeDef(
+    _RequiredInstanceRequirementsOutputTypeDef, _OptionalInstanceRequirementsOutputTypeDef
+):
+    pass
+
+
 _RequiredInstanceRequirementsTypeDef = TypedDict(
     "_RequiredInstanceRequirementsTypeDef",
     {
         "VCpuCount": VCpuCountRequestTypeDef,
         "MemoryMiB": MemoryMiBRequestTypeDef,
     },
 )
@@ -2160,33 +2254,34 @@
     total=False,
 )
 
 ProcessesTypeTypeDef = TypedDict(
     "ProcessesTypeTypeDef",
     {
         "Processes": List[ProcessTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RefreshPreferencesUnionTypeDef = Union[RefreshPreferencesTypeDef, RefreshPreferencesOutputTypeDef]
 ScheduledActionsTypeTypeDef = TypedDict(
     "ScheduledActionsTypeTypeDef",
     {
         "ScheduledUpdateGroupActions": List[ScheduledUpdateGroupActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoScalingInstancesTypeTypeDef = TypedDict(
     "AutoScalingInstancesTypeTypeDef",
     {
         "AutoScalingInstances": List[AutoScalingInstanceDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchConfigurationTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
@@ -2260,14 +2355,56 @@
 
 class LaunchConfigurationTypeDef(
     _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
 ):
     pass
 
 
+_RequiredMetricStatOutputTypeDef = TypedDict(
+    "_RequiredMetricStatOutputTypeDef",
+    {
+        "Metric": MetricOutputTypeDef,
+        "Stat": str,
+    },
+)
+_OptionalMetricStatOutputTypeDef = TypedDict(
+    "_OptionalMetricStatOutputTypeDef",
+    {
+        "Unit": str,
+    },
+    total=False,
+)
+
+
+class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
+    pass
+
+
+_RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricStatOutputTypeDef",
+    {
+        "Metric": MetricOutputTypeDef,
+        "Stat": str,
+    },
+)
+_OptionalTargetTrackingMetricStatOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingMetricStatOutputTypeDef",
+    {
+        "Unit": str,
+    },
+    total=False,
+)
+
+
+class TargetTrackingMetricStatOutputTypeDef(
+    _RequiredTargetTrackingMetricStatOutputTypeDef, _OptionalTargetTrackingMetricStatOutputTypeDef
+):
+    pass
+
+
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Stat": str,
     },
 )
@@ -2302,26 +2439,45 @@
 
 class TargetTrackingMetricStatTypeDef(
     _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
 ):
     pass
 
 
+BatchPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
+    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledUpdateGroupActions": Sequence[ScheduledUpdateGroupActionRequestTypeDef],
+    },
+)
+
 RollbackDetailsTypeDef = TypedDict(
     "RollbackDetailsTypeDef",
     {
         "RollbackReason": str,
         "RollbackStartTime": datetime,
         "PercentageCompleteOnRollback": int,
         "InstancesToUpdateOnRollback": int,
         "ProgressDetailsOnRollback": InstanceRefreshProgressDetailsTypeDef,
     },
     total=False,
 )
 
+LaunchTemplateOverridesOutputTypeDef = TypedDict(
+    "LaunchTemplateOverridesOutputTypeDef",
+    {
+        "InstanceType": str,
+        "WeightedCapacity": str,
+        "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
+        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
+    },
+    total=False,
+)
+
 LaunchTemplateOverridesTypeDef = TypedDict(
     "LaunchTemplateOverridesTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": str,
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "InstanceRequirements": InstanceRequirementsTypeDef,
@@ -2331,27 +2487,76 @@
 
 DescribeWarmPoolAnswerTypeDef = TypedDict(
     "DescribeWarmPoolAnswerTypeDef",
     {
         "WarmPoolConfiguration": WarmPoolConfigurationTypeDef,
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LaunchConfigurationsTypeTypeDef = TypedDict(
     "LaunchConfigurationsTypeTypeDef",
     {
         "LaunchConfigurations": List[LaunchConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredMetricDataQueryOutputTypeDef = TypedDict(
+    "_RequiredMetricDataQueryOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalMetricDataQueryOutputTypeDef = TypedDict(
+    "_OptionalMetricDataQueryOutputTypeDef",
+    {
+        "Expression": str,
+        "MetricStat": MetricStatOutputTypeDef,
+        "Label": str,
+        "ReturnData": bool,
+    },
+    total=False,
+)
+
+
+class MetricDataQueryOutputTypeDef(
+    _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
+):
+    pass
+
+
+_RequiredTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricDataQueryOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingMetricDataQueryOutputTypeDef",
+    {
+        "Expression": str,
+        "MetricStat": TargetTrackingMetricStatOutputTypeDef,
+        "Label": str,
+        "ReturnData": bool,
+    },
+    total=False,
+)
+
+
+class TargetTrackingMetricDataQueryOutputTypeDef(
+    _RequiredTargetTrackingMetricDataQueryOutputTypeDef,
+    _OptionalTargetTrackingMetricDataQueryOutputTypeDef,
+):
+    pass
+
+
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryTypeDef = TypedDict(
@@ -2390,66 +2595,173 @@
 
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
 
+LaunchTemplateOutputTypeDef = TypedDict(
+    "LaunchTemplateOutputTypeDef",
+    {
+        "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
+        "Overrides": List[LaunchTemplateOverridesOutputTypeDef],
+    },
+    total=False,
+)
+
 LaunchTemplateTypeDef = TypedDict(
     "LaunchTemplateTypeDef",
     {
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[LaunchTemplateOverridesTypeDef],
     },
     total=False,
 )
 
+PredictiveScalingCustomizedCapacityMetricOutputTypeDef = TypedDict(
+    "PredictiveScalingCustomizedCapacityMetricOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+)
+
+PredictiveScalingCustomizedLoadMetricOutputTypeDef = TypedDict(
+    "PredictiveScalingCustomizedLoadMetricOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+)
+
+PredictiveScalingCustomizedScalingMetricOutputTypeDef = TypedDict(
+    "PredictiveScalingCustomizedScalingMetricOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+)
+
+CustomizedMetricSpecificationOutputTypeDef = TypedDict(
+    "CustomizedMetricSpecificationOutputTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Dimensions": List[MetricDimensionTypeDef],
+        "Statistic": MetricStatisticType,
+        "Unit": str,
+        "Metrics": List[TargetTrackingMetricDataQueryOutputTypeDef],
+    },
+    total=False,
+)
+
 PredictiveScalingCustomizedCapacityMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryTypeDef],
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
 )
 
 PredictiveScalingCustomizedLoadMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryTypeDef],
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
 )
 
 PredictiveScalingCustomizedScalingMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryTypeDef],
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
 )
 
 CustomizedMetricSpecificationTypeDef = TypedDict(
     "CustomizedMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
-        "Dimensions": List[MetricDimensionTypeDef],
+        "Dimensions": Sequence[MetricDimensionTypeDef],
         "Statistic": MetricStatisticType,
         "Unit": str,
-        "Metrics": List[TargetTrackingMetricDataQueryTypeDef],
+        "Metrics": Sequence[TargetTrackingMetricDataQueryTypeDef],
+    },
+    total=False,
+)
+
+MixedInstancesPolicyOutputTypeDef = TypedDict(
+    "MixedInstancesPolicyOutputTypeDef",
+    {
+        "LaunchTemplate": LaunchTemplateOutputTypeDef,
+        "InstancesDistribution": InstancesDistributionTypeDef,
     },
     total=False,
 )
 
 MixedInstancesPolicyTypeDef = TypedDict(
     "MixedInstancesPolicyTypeDef",
     {
         "LaunchTemplate": LaunchTemplateTypeDef,
         "InstancesDistribution": InstancesDistributionTypeDef,
     },
     total=False,
 )
 
+_RequiredPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingMetricSpecificationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingMetricSpecificationOutputTypeDef",
+    {
+        "PredefinedMetricPairSpecification": PredictiveScalingPredefinedMetricPairTypeDef,
+        "PredefinedScalingMetricSpecification": PredictiveScalingPredefinedScalingMetricTypeDef,
+        "PredefinedLoadMetricSpecification": PredictiveScalingPredefinedLoadMetricTypeDef,
+        "CustomizedScalingMetricSpecification": (
+            PredictiveScalingCustomizedScalingMetricOutputTypeDef
+        ),
+        "CustomizedLoadMetricSpecification": PredictiveScalingCustomizedLoadMetricOutputTypeDef,
+        "CustomizedCapacityMetricSpecification": (
+            PredictiveScalingCustomizedCapacityMetricOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
+
+class PredictiveScalingMetricSpecificationOutputTypeDef(
+    _RequiredPredictiveScalingMetricSpecificationOutputTypeDef,
+    _OptionalPredictiveScalingMetricSpecificationOutputTypeDef,
+):
+    pass
+
+
+_RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingConfigurationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingConfigurationOutputTypeDef",
+    {
+        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
+        "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
+        "DisableScaleIn": bool,
+    },
+    total=False,
+)
+
+
+class TargetTrackingConfigurationOutputTypeDef(
+    _RequiredTargetTrackingConfigurationOutputTypeDef,
+    _OptionalTargetTrackingConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredPredictiveScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredictiveScalingMetricSpecificationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalPredictiveScalingMetricSpecificationTypeDef = TypedDict(
@@ -2511,15 +2823,15 @@
 )
 _OptionalAutoScalingGroupTypeDef = TypedDict(
     "_OptionalAutoScalingGroupTypeDef",
     {
         "AutoScalingGroupARN": str,
         "LaunchConfigurationName": str,
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "MixedInstancesPolicy": MixedInstancesPolicyTypeDef,
+        "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
         "PredictedCapacity": int,
         "LoadBalancerNames": List[str],
         "TargetGroupARNs": List[str],
         "HealthCheckGracePeriod": int,
         "Instances": List[InstanceTypeDef],
         "SuspendedProcesses": List[SuspendedProcessTypeDef],
         "PlacementGroup": str,
@@ -2543,14 +2855,23 @@
 )
 
 
 class AutoScalingGroupTypeDef(_RequiredAutoScalingGroupTypeDef, _OptionalAutoScalingGroupTypeDef):
     pass
 
 
+DesiredConfigurationOutputTypeDef = TypedDict(
+    "DesiredConfigurationOutputTypeDef",
+    {
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
+        "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredCreateAutoScalingGroupTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "MinSize": int,
         "MaxSize": int,
     },
@@ -2599,14 +2920,17 @@
     {
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "MixedInstancesPolicy": MixedInstancesPolicyTypeDef,
     },
     total=False,
 )
 
+MixedInstancesPolicyUnionTypeDef = Union[
+    MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
+]
 _RequiredUpdateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredUpdateAutoScalingGroupTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalUpdateAutoScalingGroupTypeRequestTypeDef = TypedDict(
@@ -2645,22 +2969,47 @@
 
 
 LoadForecastTypeDef = TypedDict(
     "LoadForecastTypeDef",
     {
         "Timestamps": List[datetime],
         "Values": List[float],
-        "MetricSpecification": PredictiveScalingMetricSpecificationTypeDef,
+        "MetricSpecification": PredictiveScalingMetricSpecificationOutputTypeDef,
     },
 )
 
+_RequiredPredictiveScalingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingConfigurationOutputTypeDef",
+    {
+        "MetricSpecifications": List[PredictiveScalingMetricSpecificationOutputTypeDef],
+    },
+)
+_OptionalPredictiveScalingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingConfigurationOutputTypeDef",
+    {
+        "Mode": PredictiveScalingModeType,
+        "SchedulingBufferTime": int,
+        "MaxCapacityBreachBehavior": PredictiveScalingMaxCapacityBreachBehaviorType,
+        "MaxCapacityBuffer": int,
+    },
+    total=False,
+)
+
+
+class PredictiveScalingConfigurationOutputTypeDef(
+    _RequiredPredictiveScalingConfigurationOutputTypeDef,
+    _OptionalPredictiveScalingConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredPredictiveScalingConfigurationTypeDef = TypedDict(
     "_RequiredPredictiveScalingConfigurationTypeDef",
     {
-        "MetricSpecifications": List[PredictiveScalingMetricSpecificationTypeDef],
+        "MetricSpecifications": Sequence[PredictiveScalingMetricSpecificationTypeDef],
     },
 )
 _OptionalPredictiveScalingConfigurationTypeDef = TypedDict(
     "_OptionalPredictiveScalingConfigurationTypeDef",
     {
         "Mode": PredictiveScalingModeType,
         "SchedulingBufferTime": int,
@@ -2673,20 +3022,23 @@
 
 class PredictiveScalingConfigurationTypeDef(
     _RequiredPredictiveScalingConfigurationTypeDef, _OptionalPredictiveScalingConfigurationTypeDef
 ):
     pass
 
 
+TargetTrackingConfigurationUnionTypeDef = Union[
+    TargetTrackingConfigurationTypeDef, TargetTrackingConfigurationOutputTypeDef
+]
 AutoScalingGroupsTypeTypeDef = TypedDict(
     "AutoScalingGroupsTypeTypeDef",
     {
         "AutoScalingGroups": List[AutoScalingGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceRefreshTypeDef = TypedDict(
     "InstanceRefreshTypeDef",
     {
         "InstanceRefreshId": str,
@@ -2694,21 +3046,24 @@
         "Status": InstanceRefreshStatusType,
         "StatusReason": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "PercentageComplete": int,
         "InstancesToUpdate": int,
         "ProgressDetails": InstanceRefreshProgressDetailsTypeDef,
-        "Preferences": RefreshPreferencesTypeDef,
-        "DesiredConfiguration": DesiredConfigurationTypeDef,
+        "Preferences": RefreshPreferencesOutputTypeDef,
+        "DesiredConfiguration": DesiredConfigurationOutputTypeDef,
         "RollbackDetails": RollbackDetailsTypeDef,
     },
     total=False,
 )
 
+DesiredConfigurationUnionTypeDef = Union[
+    DesiredConfigurationTypeDef, DesiredConfigurationOutputTypeDef
+]
 _RequiredStartInstanceRefreshTypeRequestTypeDef = TypedDict(
     "_RequiredStartInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalStartInstanceRefreshTypeRequestTypeDef = TypedDict(
@@ -2730,84 +3085,87 @@
 
 GetPredictiveScalingForecastAnswerTypeDef = TypedDict(
     "GetPredictiveScalingForecastAnswerTypeDef",
     {
         "LoadForecast": List[LoadForecastTypeDef],
         "CapacityForecast": CapacityForecastTypeDef,
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
-    "_RequiredPutScalingPolicyTypeRequestTypeDef",
+ScalingPolicyTypeDef = TypedDict(
+    "ScalingPolicyTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
-    },
-)
-_OptionalPutScalingPolicyTypeRequestTypeDef = TypedDict(
-    "_OptionalPutScalingPolicyTypeRequestTypeDef",
-    {
+        "PolicyARN": str,
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
+        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MetricAggregationType": str,
-        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "EstimatedInstanceWarmup": int,
-        "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
+        "Alarms": List[AlarmTypeDef],
+        "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
         "Enabled": bool,
-        "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
+        "PredictiveScalingConfiguration": PredictiveScalingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-
-class PutScalingPolicyTypeRequestTypeDef(
-    _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
-):
-    pass
-
-
-ScalingPolicyTypeDef = TypedDict(
-    "ScalingPolicyTypeDef",
+PredictiveScalingConfigurationUnionTypeDef = Union[
+    PredictiveScalingConfigurationTypeDef, PredictiveScalingConfigurationOutputTypeDef
+]
+_RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
+    "_RequiredPutScalingPolicyTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
-        "PolicyARN": str,
+    },
+)
+_OptionalPutScalingPolicyTypeRequestTypeDef = TypedDict(
+    "_OptionalPutScalingPolicyTypeRequestTypeDef",
+    {
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
-        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MetricAggregationType": str,
+        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "EstimatedInstanceWarmup": int,
-        "Alarms": List[AlarmTypeDef],
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
         "Enabled": bool,
         "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
     },
     total=False,
 )
 
+
+class PutScalingPolicyTypeRequestTypeDef(
+    _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
+):
+    pass
+
+
 DescribeInstanceRefreshesAnswerTypeDef = TypedDict(
     "DescribeInstanceRefreshesAnswerTypeDef",
     {
         "InstanceRefreshes": List[InstanceRefreshTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PoliciesTypeTypeDef = TypedDict(
     "PoliciesTypeTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling/type_defs.pyi` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_autoscaling.type_defs import AcceleratorCountRequestTypeDef
 
-    data: AcceleratorCountRequestTypeDef = {...}
+    data: AcceleratorCountRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -51,185 +51,209 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceleratorCountRequestTypeDef",
     "AcceleratorTotalMemoryMiBRequestTypeDef",
     "ActivityTypeDef",
+    "ResponseMetadataTypeDef",
     "AdjustmentTypeTypeDef",
     "AlarmTypeDef",
     "AttachInstancesQueryRequestTypeDef",
     "AttachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "AttachLoadBalancersTypeRequestTypeDef",
     "TrafficSourceIdentifierTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "EnabledMetricTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "SuspendedProcessTypeDef",
     "TagDescriptionTypeDef",
     "BaselineEbsBandwidthMbpsRequestTypeDef",
     "FailedScheduledUpdateGroupActionRequestTypeDef",
     "BatchDeleteScheduledActionTypeRequestTypeDef",
-    "ScheduledUpdateGroupActionRequestTypeDef",
     "EbsTypeDef",
-    "CancelInstanceRefreshAnswerTypeDef",
     "CancelInstanceRefreshTypeRequestTypeDef",
     "CapacityForecastTypeDef",
     "CompleteLifecycleActionTypeRequestTypeDef",
     "LifecycleHookSpecificationTypeDef",
     "TagTypeDef",
     "InstanceMetadataOptionsTypeDef",
     "InstanceMonitoringTypeDef",
     "MetricDimensionTypeDef",
     "DeleteAutoScalingGroupTypeRequestTypeDef",
     "DeleteLifecycleHookTypeRequestTypeDef",
     "DeleteNotificationConfigurationTypeRequestTypeDef",
     "DeletePolicyTypeRequestTypeDef",
     "DeleteScheduledActionTypeRequestTypeDef",
     "DeleteWarmPoolTypeRequestTypeDef",
-    "DescribeAccountLimitsAnswerTypeDef",
-    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
-    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
     "DescribeInstanceRefreshesTypeRequestTypeDef",
-    "DescribeLifecycleHookTypesAnswerTypeDef",
     "LifecycleHookTypeDef",
     "DescribeLifecycleHooksTypeRequestTypeDef",
-    "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
     "DescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     "LoadBalancerTargetGroupStateTypeDef",
-    "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
     "DescribeLoadBalancersRequestRequestTypeDef",
     "LoadBalancerStateTypeDef",
     "MetricCollectionTypeTypeDef",
     "MetricGranularityTypeTypeDef",
     "NotificationConfigurationTypeDef",
-    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
-    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
     "DescribePoliciesTypeRequestTypeDef",
-    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
     "DescribeScalingActivitiesTypeRequestTypeDef",
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
-    "DescribeScheduledActionsTypeRequestTypeDef",
-    "DescribeTerminationPolicyTypesAnswerTypeDef",
+    "TimestampTypeDef",
     "DescribeTrafficSourcesRequestRequestTypeDef",
     "TrafficSourceStateTypeDef",
     "DescribeWarmPoolTypeRequestTypeDef",
     "DetachInstancesQueryRequestTypeDef",
     "DetachLoadBalancerTargetGroupsTypeRequestTypeDef",
     "DetachLoadBalancersTypeRequestTypeDef",
     "DisableMetricsCollectionQueryRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
-    "GetPredictiveScalingForecastTypeRequestTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
-    "RefreshPreferencesTypeDef",
+    "RefreshPreferencesOutputTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
     "InstanceReusePolicyTypeDef",
     "InstancesDistributionTypeDef",
     "LaunchConfigurationNameTypeRequestTypeDef",
-    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "LaunchConfigurationNamesTypeRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "PredictiveScalingPredefinedLoadMetricTypeDef",
     "PredictiveScalingPredefinedMetricPairTypeDef",
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
-    "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "RollbackInstanceRefreshAnswerTypeDef",
+    "RefreshPreferencesTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
-    "StartInstanceRefreshAnswerTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     "ActivitiesTypeTypeDef",
     "ActivityTypeTypeDef",
+    "CancelInstanceRefreshAnswerTypeDef",
+    "DescribeAccountLimitsAnswerTypeDef",
+    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
+    "DescribeLifecycleHookTypesAnswerTypeDef",
+    "DescribeTerminationPolicyTypesAnswerTypeDef",
     "DetachInstancesAnswerTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnterStandbyAnswerTypeDef",
     "ExitStandbyAnswerTypeDef",
+    "RollbackInstanceRefreshAnswerTypeDef",
+    "StartInstanceRefreshAnswerTypeDef",
     "DescribeAdjustmentTypesAnswerTypeDef",
     "PolicyARNTypeTypeDef",
     "AttachTrafficSourcesTypeRequestTypeDef",
     "DetachTrafficSourcesTypeRequestTypeDef",
-    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
     "AutoScalingGroupNamesTypeRequestTypeDef",
-    "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     "DescribeTagsTypeRequestTypeDef",
+    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
+    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
+    "DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    "DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
+    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
+    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
+    "DescribeTagsTypeDescribeTagsPaginateTypeDef",
+    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     "AutoScalingInstanceDetailsTypeDef",
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
-    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "BlockDeviceMappingTypeDef",
     "CreateOrUpdateTagsTypeRequestTypeDef",
     "DeleteTagsTypeRequestTypeDef",
+    "MetricOutputTypeDef",
     "MetricTypeDef",
     "DescribeLifecycleHooksAnswerTypeDef",
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     "DescribeLoadBalancersResponseTypeDef",
     "DescribeMetricCollectionTypesAnswerTypeDef",
     "DescribeNotificationConfigurationsAnswerTypeDef",
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    "DescribeScheduledActionsTypeRequestTypeDef",
+    "GetPredictiveScalingForecastTypeRequestTypeDef",
+    "PutScheduledUpdateGroupActionTypeRequestTypeDef",
+    "ScheduledUpdateGroupActionRequestTypeDef",
     "DescribeTrafficSourcesResponseTypeDef",
     "InstanceRefreshProgressDetailsTypeDef",
+    "InstanceRequirementsOutputTypeDef",
     "InstanceRequirementsTypeDef",
     "PutWarmPoolTypeRequestTypeDef",
     "WarmPoolConfigurationTypeDef",
     "ProcessesTypeTypeDef",
+    "RefreshPreferencesUnionTypeDef",
     "ScheduledActionsTypeTypeDef",
     "AutoScalingInstancesTypeTypeDef",
     "CreateLaunchConfigurationTypeRequestTypeDef",
     "LaunchConfigurationTypeDef",
+    "MetricStatOutputTypeDef",
+    "TargetTrackingMetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "TargetTrackingMetricStatTypeDef",
+    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RollbackDetailsTypeDef",
+    "LaunchTemplateOverridesOutputTypeDef",
     "LaunchTemplateOverridesTypeDef",
     "DescribeWarmPoolAnswerTypeDef",
     "LaunchConfigurationsTypeTypeDef",
+    "MetricDataQueryOutputTypeDef",
+    "TargetTrackingMetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
     "TargetTrackingMetricDataQueryTypeDef",
+    "LaunchTemplateOutputTypeDef",
     "LaunchTemplateTypeDef",
+    "PredictiveScalingCustomizedCapacityMetricOutputTypeDef",
+    "PredictiveScalingCustomizedLoadMetricOutputTypeDef",
+    "PredictiveScalingCustomizedScalingMetricOutputTypeDef",
+    "CustomizedMetricSpecificationOutputTypeDef",
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     "CustomizedMetricSpecificationTypeDef",
+    "MixedInstancesPolicyOutputTypeDef",
     "MixedInstancesPolicyTypeDef",
+    "PredictiveScalingMetricSpecificationOutputTypeDef",
+    "TargetTrackingConfigurationOutputTypeDef",
     "PredictiveScalingMetricSpecificationTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
+    "DesiredConfigurationOutputTypeDef",
     "CreateAutoScalingGroupTypeRequestTypeDef",
     "DesiredConfigurationTypeDef",
+    "MixedInstancesPolicyUnionTypeDef",
     "UpdateAutoScalingGroupTypeRequestTypeDef",
     "LoadForecastTypeDef",
+    "PredictiveScalingConfigurationOutputTypeDef",
     "PredictiveScalingConfigurationTypeDef",
+    "TargetTrackingConfigurationUnionTypeDef",
     "AutoScalingGroupsTypeTypeDef",
     "InstanceRefreshTypeDef",
+    "DesiredConfigurationUnionTypeDef",
     "StartInstanceRefreshTypeRequestTypeDef",
     "GetPredictiveScalingForecastAnswerTypeDef",
-    "PutScalingPolicyTypeRequestTypeDef",
     "ScalingPolicyTypeDef",
+    "PredictiveScalingConfigurationUnionTypeDef",
+    "PutScalingPolicyTypeRequestTypeDef",
     "DescribeInstanceRefreshesAnswerTypeDef",
     "PoliciesTypeTypeDef",
 )
 
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
     {
@@ -271,14 +295,25 @@
     },
     total=False,
 )
 
 class ActivityTypeDef(_RequiredActivityTypeDef, _OptionalActivityTypeDef):
     pass
 
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
 AdjustmentTypeTypeDef = TypedDict(
     "AdjustmentTypeTypeDef",
     {
         "AdjustmentType": str,
     },
     total=False,
 )
@@ -351,14 +386,24 @@
     {
         "Name": str,
         "Values": Sequence[str],
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
 EnabledMetricTypeDef = TypedDict(
     "EnabledMetricTypeDef",
     {
         "Metric": str,
         "Granularity": str,
     },
     total=False,
@@ -429,62 +474,28 @@
     "BatchDeleteScheduledActionTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "ScheduledActionNames": Sequence[str],
     },
 )
 
-_RequiredScheduledUpdateGroupActionRequestTypeDef = TypedDict(
-    "_RequiredScheduledUpdateGroupActionRequestTypeDef",
-    {
-        "ScheduledActionName": str,
-    },
-)
-_OptionalScheduledUpdateGroupActionRequestTypeDef = TypedDict(
-    "_OptionalScheduledUpdateGroupActionRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Recurrence": str,
-        "MinSize": int,
-        "MaxSize": int,
-        "DesiredCapacity": int,
-        "TimeZone": str,
-    },
-    total=False,
-)
-
-class ScheduledUpdateGroupActionRequestTypeDef(
-    _RequiredScheduledUpdateGroupActionRequestTypeDef,
-    _OptionalScheduledUpdateGroupActionRequestTypeDef,
-):
-    pass
-
 EbsTypeDef = TypedDict(
     "EbsTypeDef",
     {
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": str,
         "DeleteOnTermination": bool,
         "Iops": int,
         "Encrypted": bool,
         "Throughput": int,
     },
     total=False,
 )
 
-CancelInstanceRefreshAnswerTypeDef = TypedDict(
-    "CancelInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CancelInstanceRefreshTypeRequestTypeDef = TypedDict(
     "CancelInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 
@@ -667,52 +678,24 @@
 )
 
 class DeleteWarmPoolTypeRequestTypeDef(
     _RequiredDeleteWarmPoolTypeRequestTypeDef, _OptionalDeleteWarmPoolTypeRequestTypeDef
 ):
     pass
 
-DescribeAccountLimitsAnswerTypeDef = TypedDict(
-    "DescribeAccountLimitsAnswerTypeDef",
-    {
-        "MaxNumberOfAutoScalingGroups": int,
-        "MaxNumberOfLaunchConfigurations": int,
-        "NumberOfAutoScalingGroups": int,
-        "NumberOfLaunchConfigurations": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef = TypedDict(
-    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
-    {
-        "InstanceIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAutoScalingInstancesTypeRequestTypeDef = TypedDict(
     "DescribeAutoScalingInstancesTypeRequestTypeDef",
     {
         "InstanceIds": Sequence[str],
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeAutoScalingNotificationTypesAnswerTypeDef = TypedDict(
-    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
-    {
-        "AutoScalingNotificationTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeInstanceRefreshesTypeRequestTypeDef = TypedDict(
     "_RequiredDescribeInstanceRefreshesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeInstanceRefreshesTypeRequestTypeDef = TypedDict(
@@ -727,22 +710,14 @@
 
 class DescribeInstanceRefreshesTypeRequestTypeDef(
     _RequiredDescribeInstanceRefreshesTypeRequestTypeDef,
     _OptionalDescribeInstanceRefreshesTypeRequestTypeDef,
 ):
     pass
 
-DescribeLifecycleHookTypesAnswerTypeDef = TypedDict(
-    "DescribeLifecycleHookTypesAnswerTypeDef",
-    {
-        "LifecycleHookTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifecycleHookTypeDef = TypedDict(
     "LifecycleHookTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
         "LifecycleTransition": str,
         "NotificationTargetARN": str,
@@ -771,34 +746,14 @@
 
 class DescribeLifecycleHooksTypeRequestTypeDef(
     _RequiredDescribeLifecycleHooksTypeRequestTypeDef,
     _OptionalDescribeLifecycleHooksTypeRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-    },
-)
-_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
-    _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-    _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancerTargetGroupsRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancerTargetGroupsRequestRequestTypeDef = TypedDict(
@@ -821,34 +776,14 @@
     {
         "LoadBalancerTargetGroupARN": str,
         "State": str,
     },
     total=False,
 )
 
-_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-    },
-)
-_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
-    _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-    _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeLoadBalancersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeLoadBalancersRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeLoadBalancersRequestRequestTypeDef = TypedDict(
@@ -897,112 +832,49 @@
         "AutoScalingGroupName": str,
         "TopicARN": str,
         "NotificationType": str,
     },
     total=False,
 )
 
-DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
-    {
-        "AutoScalingGroupNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeNotificationConfigurationsTypeRequestTypeDef = TypedDict(
     "DescribeNotificationConfigurationsTypeRequestTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribePoliciesTypeDescribePoliciesPaginateTypeDef = TypedDict(
-    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "PolicyNames": Sequence[str],
-        "PolicyTypes": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribePoliciesTypeRequestTypeDef = TypedDict(
     "DescribePoliciesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyNames": Sequence[str],
         "PolicyTypes": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
     },
     total=False,
 )
 
-DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ActivityIds": Sequence[str],
-        "AutoScalingGroupName": str,
-        "IncludeDeletedGroups": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeScalingActivitiesTypeRequestTypeDef = TypedDict(
     "DescribeScalingActivitiesTypeRequestTypeDef",
     {
         "ActivityIds": Sequence[str],
         "AutoScalingGroupName": str,
         "IncludeDeletedGroups": bool,
         "MaxRecords": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionNames": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-DescribeScheduledActionsTypeRequestTypeDef = TypedDict(
-    "DescribeScheduledActionsTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionNames": Sequence[str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxRecords": int,
-    },
-    total=False,
-)
-
-DescribeTerminationPolicyTypesAnswerTypeDef = TypedDict(
-    "DescribeTerminationPolicyTypesAnswerTypeDef",
-    {
-        "TerminationPolicyTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTrafficSourcesRequestRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalDescribeTrafficSourcesRequestRequestTypeDef = TypedDict(
@@ -1104,21 +976,14 @@
 
 class DisableMetricsCollectionQueryRequestTypeDef(
     _RequiredDisableMetricsCollectionQueryRequestTypeDef,
     _OptionalDisableMetricsCollectionQueryRequestTypeDef,
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableMetricsCollectionQueryRequestTypeDef = TypedDict(
     "_RequiredEnableMetricsCollectionQueryRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "Granularity": str,
     },
 )
@@ -1193,24 +1058,14 @@
 )
 
 class ExitStandbyQueryRequestTypeDef(
     _RequiredExitStandbyQueryRequestTypeDef, _OptionalExitStandbyQueryRequestTypeDef
 ):
     pass
 
-GetPredictiveScalingForecastTypeRequestTypeDef = TypedDict(
-    "GetPredictiveScalingForecastTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "PolicyName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-
 InstanceRefreshLivePoolProgressTypeDef = TypedDict(
     "InstanceRefreshLivePoolProgressTypeDef",
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
@@ -1221,16 +1076,16 @@
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
 )
 
-RefreshPreferencesTypeDef = TypedDict(
-    "RefreshPreferencesTypeDef",
+RefreshPreferencesOutputTypeDef = TypedDict(
+    "RefreshPreferencesOutputTypeDef",
     {
         "MinHealthyPercentage": int,
         "InstanceWarmup": int,
         "CheckpointPercentages": List[int],
         "CheckpointDelay": int,
         "SkipMatching": bool,
         "AutoRollback": bool,
@@ -1334,43 +1189,24 @@
 LaunchConfigurationNameTypeRequestTypeDef = TypedDict(
     "LaunchConfigurationNameTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
     },
 )
 
-LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
-    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
-    {
-        "LaunchConfigurationNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 LaunchConfigurationNamesTypeRequestTypeDef = TypedDict(
     "LaunchConfigurationNamesTypeRequestTypeDef",
     {
         "LaunchConfigurationNames": Sequence[str],
         "NextToken": str,
         "MaxRecords": int,
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
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
@@ -1501,42 +1337,14 @@
     },
     total=False,
 )
 
 class StepAdjustmentTypeDef(_RequiredStepAdjustmentTypeDef, _OptionalStepAdjustmentTypeDef):
     pass
 
-_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
-    "_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledActionName": str,
-    },
-)
-_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
-    "_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    {
-        "Time": Union[datetime, str],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Recurrence": str,
-        "MinSize": int,
-        "MaxSize": int,
-        "DesiredCapacity": int,
-        "TimeZone": str,
-    },
-    total=False,
-)
-
-class PutScheduledUpdateGroupActionTypeRequestTypeDef(
-    _RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef,
-    _OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef,
-):
-    pass
-
 _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef = TypedDict(
     "_RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef",
     {
         "LifecycleHookName": str,
         "AutoScalingGroupName": str,
     },
 )
@@ -1551,31 +1359,27 @@
 
 class RecordLifecycleActionHeartbeatTypeRequestTypeDef(
     _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef,
     _OptionalRecordLifecycleActionHeartbeatTypeRequestTypeDef,
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
-
-RollbackInstanceRefreshAnswerTypeDef = TypedDict(
-    "RollbackInstanceRefreshAnswerTypeDef",
+RefreshPreferencesTypeDef = TypedDict(
+    "RefreshPreferencesTypeDef",
     {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MinHealthyPercentage": int,
+        "InstanceWarmup": int,
+        "CheckpointPercentages": Sequence[int],
+        "CheckpointDelay": int,
+        "SkipMatching": bool,
+        "AutoRollback": bool,
+        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
+        "StandbyInstances": StandbyInstancesType,
     },
+    total=False,
 )
 
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
@@ -1664,85 +1468,143 @@
     {
         "InstanceIds": Sequence[str],
         "AutoScalingGroupName": str,
         "ProtectedFromScaleIn": bool,
     },
 )
 
-StartInstanceRefreshAnswerTypeDef = TypedDict(
-    "StartInstanceRefreshAnswerTypeDef",
-    {
-        "InstanceRefreshId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TerminateInstanceInAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
     {
         "InstanceId": str,
         "ShouldDecrementDesiredCapacity": bool,
     },
 )
 
 ActivitiesTypeTypeDef = TypedDict(
     "ActivitiesTypeTypeDef",
     {
         "Activities": List[ActivityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActivityTypeTypeDef = TypedDict(
     "ActivityTypeTypeDef",
     {
         "Activity": ActivityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelInstanceRefreshAnswerTypeDef = TypedDict(
+    "CancelInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountLimitsAnswerTypeDef = TypedDict(
+    "DescribeAccountLimitsAnswerTypeDef",
+    {
+        "MaxNumberOfAutoScalingGroups": int,
+        "MaxNumberOfLaunchConfigurations": int,
+        "NumberOfAutoScalingGroups": int,
+        "NumberOfLaunchConfigurations": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAutoScalingNotificationTypesAnswerTypeDef = TypedDict(
+    "DescribeAutoScalingNotificationTypesAnswerTypeDef",
+    {
+        "AutoScalingNotificationTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLifecycleHookTypesAnswerTypeDef = TypedDict(
+    "DescribeLifecycleHookTypesAnswerTypeDef",
+    {
+        "LifecycleHookTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeTerminationPolicyTypesAnswerTypeDef = TypedDict(
+    "DescribeTerminationPolicyTypesAnswerTypeDef",
+    {
+        "TerminationPolicyTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetachInstancesAnswerTypeDef = TypedDict(
     "DetachInstancesAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnterStandbyAnswerTypeDef = TypedDict(
     "EnterStandbyAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExitStandbyAnswerTypeDef = TypedDict(
     "ExitStandbyAnswerTypeDef",
     {
         "Activities": List[ActivityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackInstanceRefreshAnswerTypeDef = TypedDict(
+    "RollbackInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartInstanceRefreshAnswerTypeDef = TypedDict(
+    "StartInstanceRefreshAnswerTypeDef",
+    {
+        "InstanceRefreshId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAdjustmentTypesAnswerTypeDef = TypedDict(
     "DescribeAdjustmentTypesAnswerTypeDef",
     {
         "AdjustmentTypes": List[AdjustmentTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyARNTypeTypeDef = TypedDict(
     "PolicyARNTypeTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachTrafficSourcesTypeRequestTypeDef = TypedDict(
     "AttachTrafficSourcesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
@@ -1754,50 +1616,139 @@
     "DetachTrafficSourcesTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "TrafficSources": Sequence[TrafficSourceIdentifierTypeDef],
     },
 )
 
-AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef = TypedDict(
-    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
+AutoScalingGroupNamesTypeRequestTypeDef = TypedDict(
+    "AutoScalingGroupNamesTypeRequestTypeDef",
     {
         "AutoScalingGroupNames": Sequence[str],
+        "NextToken": str,
+        "MaxRecords": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-AutoScalingGroupNamesTypeRequestTypeDef = TypedDict(
-    "AutoScalingGroupNamesTypeRequestTypeDef",
+DescribeTagsTypeRequestTypeDef = TypedDict(
+    "DescribeTagsTypeRequestTypeDef",
     {
-        "AutoScalingGroupNames": Sequence[str],
+        "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxRecords": int,
+    },
+    total=False,
+)
+
+AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef = TypedDict(
+    "AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef",
+    {
+        "AutoScalingGroupNames": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef = TypedDict(
+    "DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef",
+    {
+        "InstanceIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef(
+    _RequiredDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+    _OptionalDescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+    },
+)
+_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef(
+    _RequiredDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+    _OptionalDescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+):
+    pass
+
+DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef",
+    {
+        "AutoScalingGroupNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribePoliciesTypeDescribePoliciesPaginateTypeDef = TypedDict(
+    "DescribePoliciesTypeDescribePoliciesPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "PolicyNames": Sequence[str],
+        "PolicyTypes": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef",
+    {
+        "ActivityIds": Sequence[str],
+        "AutoScalingGroupName": str,
+        "IncludeDeletedGroups": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeTagsTypeDescribeTagsPaginateTypeDef = TypedDict(
     "DescribeTagsTypeDescribeTagsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeTagsTypeRequestTypeDef = TypedDict(
-    "DescribeTagsTypeRequestTypeDef",
+LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef = TypedDict(
+    "LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "NextToken": str,
-        "MaxRecords": int,
+        "LaunchConfigurationNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredAutoScalingInstanceDetailsTypeDef = TypedDict(
     "_RequiredAutoScalingInstanceDetailsTypeDef",
     {
@@ -1850,39 +1801,31 @@
     pass
 
 TagsTypeTypeDef = TypedDict(
     "TagsTypeTypeDef",
     {
         "Tags": List[TagDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteScheduledActionAnswerTypeDef = TypedDict(
     "BatchDeleteScheduledActionAnswerTypeDef",
     {
         "FailedScheduledActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutScheduledUpdateGroupActionAnswerTypeDef = TypedDict(
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     {
         "FailedScheduledUpdateGroupActions": List[FailedScheduledUpdateGroupActionRequestTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-BatchPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
-    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
-    {
-        "AutoScalingGroupName": str,
-        "ScheduledUpdateGroupActions": Sequence[ScheduledUpdateGroupActionRequestTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBlockDeviceMappingTypeDef = TypedDict(
     "_RequiredBlockDeviceMappingTypeDef",
     {
         "DeviceName": str,
@@ -1913,94 +1856,241 @@
 DeleteTagsTypeRequestTypeDef = TypedDict(
     "DeleteTagsTypeRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredMetricOutputTypeDef = TypedDict(
+    "_RequiredMetricOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+    },
+)
+_OptionalMetricOutputTypeDef = TypedDict(
+    "_OptionalMetricOutputTypeDef",
+    {
+        "Dimensions": List[MetricDimensionTypeDef],
+    },
+    total=False,
+)
+
+class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
+    pass
+
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
 _OptionalMetricTypeDef = TypedDict(
     "_OptionalMetricTypeDef",
     {
-        "Dimensions": List[MetricDimensionTypeDef],
+        "Dimensions": Sequence[MetricDimensionTypeDef],
     },
     total=False,
 )
 
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
 DescribeLifecycleHooksAnswerTypeDef = TypedDict(
     "DescribeLifecycleHooksAnswerTypeDef",
     {
         "LifecycleHooks": List[LifecycleHookTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancerTargetGroupsResponseTypeDef = TypedDict(
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     {
         "LoadBalancerTargetGroups": List[LoadBalancerTargetGroupStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLoadBalancersResponseTypeDef = TypedDict(
     "DescribeLoadBalancersResponseTypeDef",
     {
         "LoadBalancers": List[LoadBalancerStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMetricCollectionTypesAnswerTypeDef = TypedDict(
     "DescribeMetricCollectionTypesAnswerTypeDef",
     {
         "Metrics": List[MetricCollectionTypeTypeDef],
         "Granularities": List[MetricGranularityTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotificationConfigurationsAnswerTypeDef = TypedDict(
     "DescribeNotificationConfigurationsAnswerTypeDef",
     {
         "NotificationConfigurations": List[NotificationConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionNames": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScheduledActionsTypeRequestTypeDef = TypedDict(
+    "DescribeScheduledActionsTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionNames": Sequence[str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxRecords": int,
+    },
+    total=False,
+)
+
+GetPredictiveScalingForecastTypeRequestTypeDef = TypedDict(
+    "GetPredictiveScalingForecastTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "PolicyName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
+_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
+    "_RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledActionName": str,
+    },
+)
+_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
+    "_OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    {
+        "Time": TimestampTypeDef,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Recurrence": str,
+        "MinSize": int,
+        "MaxSize": int,
+        "DesiredCapacity": int,
+        "TimeZone": str,
+    },
+    total=False,
+)
+
+class PutScheduledUpdateGroupActionTypeRequestTypeDef(
+    _RequiredPutScheduledUpdateGroupActionTypeRequestTypeDef,
+    _OptionalPutScheduledUpdateGroupActionTypeRequestTypeDef,
+):
+    pass
+
+_RequiredScheduledUpdateGroupActionRequestTypeDef = TypedDict(
+    "_RequiredScheduledUpdateGroupActionRequestTypeDef",
+    {
+        "ScheduledActionName": str,
+    },
+)
+_OptionalScheduledUpdateGroupActionRequestTypeDef = TypedDict(
+    "_OptionalScheduledUpdateGroupActionRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Recurrence": str,
+        "MinSize": int,
+        "MaxSize": int,
+        "DesiredCapacity": int,
+        "TimeZone": str,
+    },
+    total=False,
+)
+
+class ScheduledUpdateGroupActionRequestTypeDef(
+    _RequiredScheduledUpdateGroupActionRequestTypeDef,
+    _OptionalScheduledUpdateGroupActionRequestTypeDef,
+):
+    pass
+
 DescribeTrafficSourcesResponseTypeDef = TypedDict(
     "DescribeTrafficSourcesResponseTypeDef",
     {
         "TrafficSources": List[TrafficSourceStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceRefreshProgressDetailsTypeDef = TypedDict(
     "InstanceRefreshProgressDetailsTypeDef",
     {
         "LivePoolProgress": InstanceRefreshLivePoolProgressTypeDef,
         "WarmPoolProgress": InstanceRefreshWarmPoolProgressTypeDef,
     },
     total=False,
 )
 
+_RequiredInstanceRequirementsOutputTypeDef = TypedDict(
+    "_RequiredInstanceRequirementsOutputTypeDef",
+    {
+        "VCpuCount": VCpuCountRequestTypeDef,
+        "MemoryMiB": MemoryMiBRequestTypeDef,
+    },
+)
+_OptionalInstanceRequirementsOutputTypeDef = TypedDict(
+    "_OptionalInstanceRequirementsOutputTypeDef",
+    {
+        "CpuManufacturers": List[CpuManufacturerType],
+        "MemoryGiBPerVCpu": MemoryGiBPerVCpuRequestTypeDef,
+        "ExcludedInstanceTypes": List[str],
+        "InstanceGenerations": List[InstanceGenerationType],
+        "SpotMaxPricePercentageOverLowestPrice": int,
+        "OnDemandMaxPricePercentageOverLowestPrice": int,
+        "BareMetal": BareMetalType,
+        "BurstablePerformance": BurstablePerformanceType,
+        "RequireHibernateSupport": bool,
+        "NetworkInterfaceCount": NetworkInterfaceCountRequestTypeDef,
+        "LocalStorage": LocalStorageType,
+        "LocalStorageTypes": List[LocalStorageTypeType],
+        "TotalLocalStorageGB": TotalLocalStorageGBRequestTypeDef,
+        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsRequestTypeDef,
+        "AcceleratorTypes": List[AcceleratorTypeType],
+        "AcceleratorCount": AcceleratorCountRequestTypeDef,
+        "AcceleratorManufacturers": List[AcceleratorManufacturerType],
+        "AcceleratorNames": List[AcceleratorNameType],
+        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestTypeDef,
+        "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestTypeDef,
+        "AllowedInstanceTypes": List[str],
+    },
+    total=False,
+)
+
+class InstanceRequirementsOutputTypeDef(
+    _RequiredInstanceRequirementsOutputTypeDef, _OptionalInstanceRequirementsOutputTypeDef
+):
+    pass
+
 _RequiredInstanceRequirementsTypeDef = TypedDict(
     "_RequiredInstanceRequirementsTypeDef",
     {
         "VCpuCount": VCpuCountRequestTypeDef,
         "MemoryMiB": MemoryMiBRequestTypeDef,
     },
 )
@@ -2071,33 +2161,34 @@
     total=False,
 )
 
 ProcessesTypeTypeDef = TypedDict(
     "ProcessesTypeTypeDef",
     {
         "Processes": List[ProcessTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RefreshPreferencesUnionTypeDef = Union[RefreshPreferencesTypeDef, RefreshPreferencesOutputTypeDef]
 ScheduledActionsTypeTypeDef = TypedDict(
     "ScheduledActionsTypeTypeDef",
     {
         "ScheduledUpdateGroupActions": List[ScheduledUpdateGroupActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoScalingInstancesTypeTypeDef = TypedDict(
     "AutoScalingInstancesTypeTypeDef",
     {
         "AutoScalingInstances": List[AutoScalingInstanceDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateLaunchConfigurationTypeRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchConfigurationTypeRequestTypeDef",
     {
         "LaunchConfigurationName": str,
@@ -2167,14 +2258,52 @@
 )
 
 class LaunchConfigurationTypeDef(
     _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
 ):
     pass
 
+_RequiredMetricStatOutputTypeDef = TypedDict(
+    "_RequiredMetricStatOutputTypeDef",
+    {
+        "Metric": MetricOutputTypeDef,
+        "Stat": str,
+    },
+)
+_OptionalMetricStatOutputTypeDef = TypedDict(
+    "_OptionalMetricStatOutputTypeDef",
+    {
+        "Unit": str,
+    },
+    total=False,
+)
+
+class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
+    pass
+
+_RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricStatOutputTypeDef",
+    {
+        "Metric": MetricOutputTypeDef,
+        "Stat": str,
+    },
+)
+_OptionalTargetTrackingMetricStatOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingMetricStatOutputTypeDef",
+    {
+        "Unit": str,
+    },
+    total=False,
+)
+
+class TargetTrackingMetricStatOutputTypeDef(
+    _RequiredTargetTrackingMetricStatOutputTypeDef, _OptionalTargetTrackingMetricStatOutputTypeDef
+):
+    pass
+
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Stat": str,
     },
 )
@@ -2205,26 +2334,45 @@
 )
 
 class TargetTrackingMetricStatTypeDef(
     _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
 ):
     pass
 
+BatchPutScheduledUpdateGroupActionTypeRequestTypeDef = TypedDict(
+    "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
+    {
+        "AutoScalingGroupName": str,
+        "ScheduledUpdateGroupActions": Sequence[ScheduledUpdateGroupActionRequestTypeDef],
+    },
+)
+
 RollbackDetailsTypeDef = TypedDict(
     "RollbackDetailsTypeDef",
     {
         "RollbackReason": str,
         "RollbackStartTime": datetime,
         "PercentageCompleteOnRollback": int,
         "InstancesToUpdateOnRollback": int,
         "ProgressDetailsOnRollback": InstanceRefreshProgressDetailsTypeDef,
     },
     total=False,
 )
 
+LaunchTemplateOverridesOutputTypeDef = TypedDict(
+    "LaunchTemplateOverridesOutputTypeDef",
+    {
+        "InstanceType": str,
+        "WeightedCapacity": str,
+        "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
+        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
+    },
+    total=False,
+)
+
 LaunchTemplateOverridesTypeDef = TypedDict(
     "LaunchTemplateOverridesTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": str,
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "InstanceRequirements": InstanceRequirementsTypeDef,
@@ -2234,27 +2382,72 @@
 
 DescribeWarmPoolAnswerTypeDef = TypedDict(
     "DescribeWarmPoolAnswerTypeDef",
     {
         "WarmPoolConfiguration": WarmPoolConfigurationTypeDef,
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LaunchConfigurationsTypeTypeDef = TypedDict(
     "LaunchConfigurationsTypeTypeDef",
     {
         "LaunchConfigurations": List[LaunchConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredMetricDataQueryOutputTypeDef = TypedDict(
+    "_RequiredMetricDataQueryOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalMetricDataQueryOutputTypeDef = TypedDict(
+    "_OptionalMetricDataQueryOutputTypeDef",
+    {
+        "Expression": str,
+        "MetricStat": MetricStatOutputTypeDef,
+        "Label": str,
+        "ReturnData": bool,
     },
+    total=False,
 )
 
+class MetricDataQueryOutputTypeDef(
+    _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
+):
+    pass
+
+_RequiredTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricDataQueryOutputTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingMetricDataQueryOutputTypeDef",
+    {
+        "Expression": str,
+        "MetricStat": TargetTrackingMetricStatOutputTypeDef,
+        "Label": str,
+        "ReturnData": bool,
+    },
+    total=False,
+)
+
+class TargetTrackingMetricDataQueryOutputTypeDef(
+    _RequiredTargetTrackingMetricDataQueryOutputTypeDef,
+    _OptionalTargetTrackingMetricDataQueryOutputTypeDef,
+):
+    pass
+
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryTypeDef = TypedDict(
@@ -2289,66 +2482,169 @@
 )
 
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
+LaunchTemplateOutputTypeDef = TypedDict(
+    "LaunchTemplateOutputTypeDef",
+    {
+        "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
+        "Overrides": List[LaunchTemplateOverridesOutputTypeDef],
+    },
+    total=False,
+)
+
 LaunchTemplateTypeDef = TypedDict(
     "LaunchTemplateTypeDef",
     {
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[LaunchTemplateOverridesTypeDef],
     },
     total=False,
 )
 
+PredictiveScalingCustomizedCapacityMetricOutputTypeDef = TypedDict(
+    "PredictiveScalingCustomizedCapacityMetricOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+)
+
+PredictiveScalingCustomizedLoadMetricOutputTypeDef = TypedDict(
+    "PredictiveScalingCustomizedLoadMetricOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+)
+
+PredictiveScalingCustomizedScalingMetricOutputTypeDef = TypedDict(
+    "PredictiveScalingCustomizedScalingMetricOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+)
+
+CustomizedMetricSpecificationOutputTypeDef = TypedDict(
+    "CustomizedMetricSpecificationOutputTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Dimensions": List[MetricDimensionTypeDef],
+        "Statistic": MetricStatisticType,
+        "Unit": str,
+        "Metrics": List[TargetTrackingMetricDataQueryOutputTypeDef],
+    },
+    total=False,
+)
+
 PredictiveScalingCustomizedCapacityMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryTypeDef],
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
 )
 
 PredictiveScalingCustomizedLoadMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryTypeDef],
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
 )
 
 PredictiveScalingCustomizedScalingMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     {
-        "MetricDataQueries": List[MetricDataQueryTypeDef],
+        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
 )
 
 CustomizedMetricSpecificationTypeDef = TypedDict(
     "CustomizedMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
-        "Dimensions": List[MetricDimensionTypeDef],
+        "Dimensions": Sequence[MetricDimensionTypeDef],
         "Statistic": MetricStatisticType,
         "Unit": str,
-        "Metrics": List[TargetTrackingMetricDataQueryTypeDef],
+        "Metrics": Sequence[TargetTrackingMetricDataQueryTypeDef],
+    },
+    total=False,
+)
+
+MixedInstancesPolicyOutputTypeDef = TypedDict(
+    "MixedInstancesPolicyOutputTypeDef",
+    {
+        "LaunchTemplate": LaunchTemplateOutputTypeDef,
+        "InstancesDistribution": InstancesDistributionTypeDef,
     },
     total=False,
 )
 
 MixedInstancesPolicyTypeDef = TypedDict(
     "MixedInstancesPolicyTypeDef",
     {
         "LaunchTemplate": LaunchTemplateTypeDef,
         "InstancesDistribution": InstancesDistributionTypeDef,
     },
     total=False,
 )
 
+_RequiredPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingMetricSpecificationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingMetricSpecificationOutputTypeDef",
+    {
+        "PredefinedMetricPairSpecification": PredictiveScalingPredefinedMetricPairTypeDef,
+        "PredefinedScalingMetricSpecification": PredictiveScalingPredefinedScalingMetricTypeDef,
+        "PredefinedLoadMetricSpecification": PredictiveScalingPredefinedLoadMetricTypeDef,
+        "CustomizedScalingMetricSpecification": (
+            PredictiveScalingCustomizedScalingMetricOutputTypeDef
+        ),
+        "CustomizedLoadMetricSpecification": PredictiveScalingCustomizedLoadMetricOutputTypeDef,
+        "CustomizedCapacityMetricSpecification": (
+            PredictiveScalingCustomizedCapacityMetricOutputTypeDef
+        ),
+    },
+    total=False,
+)
+
+class PredictiveScalingMetricSpecificationOutputTypeDef(
+    _RequiredPredictiveScalingMetricSpecificationOutputTypeDef,
+    _OptionalPredictiveScalingMetricSpecificationOutputTypeDef,
+):
+    pass
+
+_RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingConfigurationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingConfigurationOutputTypeDef",
+    {
+        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
+        "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
+        "DisableScaleIn": bool,
+    },
+    total=False,
+)
+
+class TargetTrackingConfigurationOutputTypeDef(
+    _RequiredTargetTrackingConfigurationOutputTypeDef,
+    _OptionalTargetTrackingConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredPredictiveScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredictiveScalingMetricSpecificationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalPredictiveScalingMetricSpecificationTypeDef = TypedDict(
@@ -2406,15 +2702,15 @@
 )
 _OptionalAutoScalingGroupTypeDef = TypedDict(
     "_OptionalAutoScalingGroupTypeDef",
     {
         "AutoScalingGroupARN": str,
         "LaunchConfigurationName": str,
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "MixedInstancesPolicy": MixedInstancesPolicyTypeDef,
+        "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
         "PredictedCapacity": int,
         "LoadBalancerNames": List[str],
         "TargetGroupARNs": List[str],
         "HealthCheckGracePeriod": int,
         "Instances": List[InstanceTypeDef],
         "SuspendedProcesses": List[SuspendedProcessTypeDef],
         "PlacementGroup": str,
@@ -2436,14 +2732,23 @@
     },
     total=False,
 )
 
 class AutoScalingGroupTypeDef(_RequiredAutoScalingGroupTypeDef, _OptionalAutoScalingGroupTypeDef):
     pass
 
+DesiredConfigurationOutputTypeDef = TypedDict(
+    "DesiredConfigurationOutputTypeDef",
+    {
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
+        "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredCreateAutoScalingGroupTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "MinSize": int,
         "MaxSize": int,
     },
@@ -2490,14 +2795,17 @@
     {
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "MixedInstancesPolicy": MixedInstancesPolicyTypeDef,
     },
     total=False,
 )
 
+MixedInstancesPolicyUnionTypeDef = Union[
+    MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
+]
 _RequiredUpdateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredUpdateAutoScalingGroupTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalUpdateAutoScalingGroupTypeRequestTypeDef = TypedDict(
@@ -2534,22 +2842,45 @@
     pass
 
 LoadForecastTypeDef = TypedDict(
     "LoadForecastTypeDef",
     {
         "Timestamps": List[datetime],
         "Values": List[float],
-        "MetricSpecification": PredictiveScalingMetricSpecificationTypeDef,
+        "MetricSpecification": PredictiveScalingMetricSpecificationOutputTypeDef,
+    },
+)
+
+_RequiredPredictiveScalingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredPredictiveScalingConfigurationOutputTypeDef",
+    {
+        "MetricSpecifications": List[PredictiveScalingMetricSpecificationOutputTypeDef],
+    },
+)
+_OptionalPredictiveScalingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalPredictiveScalingConfigurationOutputTypeDef",
+    {
+        "Mode": PredictiveScalingModeType,
+        "SchedulingBufferTime": int,
+        "MaxCapacityBreachBehavior": PredictiveScalingMaxCapacityBreachBehaviorType,
+        "MaxCapacityBuffer": int,
     },
+    total=False,
 )
 
+class PredictiveScalingConfigurationOutputTypeDef(
+    _RequiredPredictiveScalingConfigurationOutputTypeDef,
+    _OptionalPredictiveScalingConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredPredictiveScalingConfigurationTypeDef = TypedDict(
     "_RequiredPredictiveScalingConfigurationTypeDef",
     {
-        "MetricSpecifications": List[PredictiveScalingMetricSpecificationTypeDef],
+        "MetricSpecifications": Sequence[PredictiveScalingMetricSpecificationTypeDef],
     },
 )
 _OptionalPredictiveScalingConfigurationTypeDef = TypedDict(
     "_OptionalPredictiveScalingConfigurationTypeDef",
     {
         "Mode": PredictiveScalingModeType,
         "SchedulingBufferTime": int,
@@ -2560,20 +2891,23 @@
 )
 
 class PredictiveScalingConfigurationTypeDef(
     _RequiredPredictiveScalingConfigurationTypeDef, _OptionalPredictiveScalingConfigurationTypeDef
 ):
     pass
 
+TargetTrackingConfigurationUnionTypeDef = Union[
+    TargetTrackingConfigurationTypeDef, TargetTrackingConfigurationOutputTypeDef
+]
 AutoScalingGroupsTypeTypeDef = TypedDict(
     "AutoScalingGroupsTypeTypeDef",
     {
         "AutoScalingGroups": List[AutoScalingGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceRefreshTypeDef = TypedDict(
     "InstanceRefreshTypeDef",
     {
         "InstanceRefreshId": str,
@@ -2581,21 +2915,24 @@
         "Status": InstanceRefreshStatusType,
         "StatusReason": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "PercentageComplete": int,
         "InstancesToUpdate": int,
         "ProgressDetails": InstanceRefreshProgressDetailsTypeDef,
-        "Preferences": RefreshPreferencesTypeDef,
-        "DesiredConfiguration": DesiredConfigurationTypeDef,
+        "Preferences": RefreshPreferencesOutputTypeDef,
+        "DesiredConfiguration": DesiredConfigurationOutputTypeDef,
         "RollbackDetails": RollbackDetailsTypeDef,
     },
     total=False,
 )
 
+DesiredConfigurationUnionTypeDef = Union[
+    DesiredConfigurationTypeDef, DesiredConfigurationOutputTypeDef
+]
 _RequiredStartInstanceRefreshTypeRequestTypeDef = TypedDict(
     "_RequiredStartInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalStartInstanceRefreshTypeRequestTypeDef = TypedDict(
@@ -2615,82 +2952,85 @@
 
 GetPredictiveScalingForecastAnswerTypeDef = TypedDict(
     "GetPredictiveScalingForecastAnswerTypeDef",
     {
         "LoadForecast": List[LoadForecastTypeDef],
         "CapacityForecast": CapacityForecastTypeDef,
         "UpdateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
-    "_RequiredPutScalingPolicyTypeRequestTypeDef",
+ScalingPolicyTypeDef = TypedDict(
+    "ScalingPolicyTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
-    },
-)
-_OptionalPutScalingPolicyTypeRequestTypeDef = TypedDict(
-    "_OptionalPutScalingPolicyTypeRequestTypeDef",
-    {
+        "PolicyARN": str,
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
+        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MetricAggregationType": str,
-        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "EstimatedInstanceWarmup": int,
-        "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
+        "Alarms": List[AlarmTypeDef],
+        "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
         "Enabled": bool,
-        "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
+        "PredictiveScalingConfiguration": PredictiveScalingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
-class PutScalingPolicyTypeRequestTypeDef(
-    _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
-):
-    pass
-
-ScalingPolicyTypeDef = TypedDict(
-    "ScalingPolicyTypeDef",
+PredictiveScalingConfigurationUnionTypeDef = Union[
+    PredictiveScalingConfigurationTypeDef, PredictiveScalingConfigurationOutputTypeDef
+]
+_RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
+    "_RequiredPutScalingPolicyTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
-        "PolicyARN": str,
+    },
+)
+_OptionalPutScalingPolicyTypeRequestTypeDef = TypedDict(
+    "_OptionalPutScalingPolicyTypeRequestTypeDef",
+    {
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
-        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MetricAggregationType": str,
+        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "EstimatedInstanceWarmup": int,
-        "Alarms": List[AlarmTypeDef],
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
         "Enabled": bool,
         "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
     },
     total=False,
 )
 
+class PutScalingPolicyTypeRequestTypeDef(
+    _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
+):
+    pass
+
 DescribeInstanceRefreshesAnswerTypeDef = TypedDict(
     "DescribeInstanceRefreshesAnswerTypeDef",
     {
         "InstanceRefreshes": List[InstanceRefreshTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PoliciesTypeTypeDef = TypedDict(
     "PoliciesTypeTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling.egg-info/PKG-INFO` & `types-aiobotocore-autoscaling-2.5.2.post1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-autoscaling
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AutoScaling 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore autoscaling type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-autoscaling"></a>
 
 # types-aiobotocore-autoscaling
 
 [![PyPI - types-aiobotocore-autoscaling](https://img.shields.io/pypi/v/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-autoscaling?color=blue)](https://pypistats.org/packages/types-aiobotocore-autoscaling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling)](https://pepy.tech/project/types-aiobotocore-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AutoScaling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
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
 [types-aiobotocore-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/).
 
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
@@ -378,203 +345,227 @@
 )
 
 
 def check_value(value: AcceleratorManufacturerType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_autoscaling.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_autoscaling.type_defs import (
     AcceleratorCountRequestTypeDef,
     AcceleratorTotalMemoryMiBRequestTypeDef,
     ActivityTypeDef,
+    ResponseMetadataTypeDef,
     AdjustmentTypeTypeDef,
     AlarmTypeDef,
     AttachInstancesQueryRequestTypeDef,
     AttachLoadBalancerTargetGroupsTypeRequestTypeDef,
     AttachLoadBalancersTypeRequestTypeDef,
     TrafficSourceIdentifierTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     EnabledMetricTypeDef,
     LaunchTemplateSpecificationTypeDef,
     SuspendedProcessTypeDef,
     TagDescriptionTypeDef,
     BaselineEbsBandwidthMbpsRequestTypeDef,
     FailedScheduledUpdateGroupActionRequestTypeDef,
     BatchDeleteScheduledActionTypeRequestTypeDef,
-    ScheduledUpdateGroupActionRequestTypeDef,
     EbsTypeDef,
-    CancelInstanceRefreshAnswerTypeDef,
     CancelInstanceRefreshTypeRequestTypeDef,
     CapacityForecastTypeDef,
     CompleteLifecycleActionTypeRequestTypeDef,
     LifecycleHookSpecificationTypeDef,
     TagTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     MetricDimensionTypeDef,
     DeleteAutoScalingGroupTypeRequestTypeDef,
     DeleteLifecycleHookTypeRequestTypeDef,
     DeleteNotificationConfigurationTypeRequestTypeDef,
     DeletePolicyTypeRequestTypeDef,
     DeleteScheduledActionTypeRequestTypeDef,
     DeleteWarmPoolTypeRequestTypeDef,
-    DescribeAccountLimitsAnswerTypeDef,
-    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
     DescribeAutoScalingInstancesTypeRequestTypeDef,
-    DescribeAutoScalingNotificationTypesAnswerTypeDef,
     DescribeInstanceRefreshesTypeRequestTypeDef,
-    DescribeLifecycleHookTypesAnswerTypeDef,
     LifecycleHookTypeDef,
     DescribeLifecycleHooksTypeRequestTypeDef,
-    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
     DescribeLoadBalancerTargetGroupsRequestRequestTypeDef,
     LoadBalancerTargetGroupStateTypeDef,
-    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
     DescribeLoadBalancersRequestRequestTypeDef,
     LoadBalancerStateTypeDef,
     MetricCollectionTypeTypeDef,
     MetricGranularityTypeTypeDef,
     NotificationConfigurationTypeDef,
-    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
     DescribeNotificationConfigurationsTypeRequestTypeDef,
-    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
     DescribePoliciesTypeRequestTypeDef,
-    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
     DescribeScalingActivitiesTypeRequestTypeDef,
-    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
-    DescribeScheduledActionsTypeRequestTypeDef,
-    DescribeTerminationPolicyTypesAnswerTypeDef,
+    TimestampTypeDef,
     DescribeTrafficSourcesRequestRequestTypeDef,
     TrafficSourceStateTypeDef,
     DescribeWarmPoolTypeRequestTypeDef,
     DetachInstancesQueryRequestTypeDef,
     DetachLoadBalancerTargetGroupsTypeRequestTypeDef,
     DetachLoadBalancersTypeRequestTypeDef,
     DisableMetricsCollectionQueryRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableMetricsCollectionQueryRequestTypeDef,
     EnterStandbyQueryRequestTypeDef,
     ExecutePolicyTypeRequestTypeDef,
     ExitStandbyQueryRequestTypeDef,
-    GetPredictiveScalingForecastTypeRequestTypeDef,
     InstanceRefreshLivePoolProgressTypeDef,
     InstanceRefreshWarmPoolProgressTypeDef,
-    RefreshPreferencesTypeDef,
+    RefreshPreferencesOutputTypeDef,
     MemoryGiBPerVCpuRequestTypeDef,
     MemoryMiBRequestTypeDef,
     NetworkBandwidthGbpsRequestTypeDef,
     NetworkInterfaceCountRequestTypeDef,
     TotalLocalStorageGBRequestTypeDef,
     VCpuCountRequestTypeDef,
     InstanceReusePolicyTypeDef,
     InstancesDistributionTypeDef,
     LaunchConfigurationNameTypeRequestTypeDef,
-    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     LaunchConfigurationNamesTypeRequestTypeDef,
-    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationTypeDef,
     PredictiveScalingPredefinedLoadMetricTypeDef,
     PredictiveScalingPredefinedMetricPairTypeDef,
     PredictiveScalingPredefinedScalingMetricTypeDef,
     ProcessTypeTypeDef,
     PutLifecycleHookTypeRequestTypeDef,
     PutNotificationConfigurationTypeRequestTypeDef,
     StepAdjustmentTypeDef,
-    PutScheduledUpdateGroupActionTypeRequestTypeDef,
     RecordLifecycleActionHeartbeatTypeRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RollbackInstanceRefreshAnswerTypeDef,
+    RefreshPreferencesTypeDef,
     RollbackInstanceRefreshTypeRequestTypeDef,
     ScalingProcessQueryRequestTypeDef,
     ScheduledUpdateGroupActionTypeDef,
     SetDesiredCapacityTypeRequestTypeDef,
     SetInstanceHealthQueryRequestTypeDef,
     SetInstanceProtectionQueryRequestTypeDef,
-    StartInstanceRefreshAnswerTypeDef,
     TerminateInstanceInAutoScalingGroupTypeRequestTypeDef,
     ActivitiesTypeTypeDef,
     ActivityTypeTypeDef,
+    CancelInstanceRefreshAnswerTypeDef,
+    DescribeAccountLimitsAnswerTypeDef,
+    DescribeAutoScalingNotificationTypesAnswerTypeDef,
+    DescribeLifecycleHookTypesAnswerTypeDef,
+    DescribeTerminationPolicyTypesAnswerTypeDef,
     DetachInstancesAnswerTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
+    RollbackInstanceRefreshAnswerTypeDef,
+    StartInstanceRefreshAnswerTypeDef,
     DescribeAdjustmentTypesAnswerTypeDef,
     PolicyARNTypeTypeDef,
     AttachTrafficSourcesTypeRequestTypeDef,
     DetachTrafficSourcesTypeRequestTypeDef,
-    AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
     AutoScalingGroupNamesTypeRequestTypeDef,
-    DescribeTagsTypeDescribeTagsPaginateTypeDef,
     DescribeTagsTypeRequestTypeDef,
+    AutoScalingGroupNamesTypeDescribeAutoScalingGroupsPaginateTypeDef,
+    DescribeAutoScalingInstancesTypeDescribeAutoScalingInstancesPaginateTypeDef,
+    DescribeLoadBalancerTargetGroupsRequestDescribeLoadBalancerTargetGroupsPaginateTypeDef,
+    DescribeLoadBalancersRequestDescribeLoadBalancersPaginateTypeDef,
+    DescribeNotificationConfigurationsTypeDescribeNotificationConfigurationsPaginateTypeDef,
+    DescribePoliciesTypeDescribePoliciesPaginateTypeDef,
+    DescribeScalingActivitiesTypeDescribeScalingActivitiesPaginateTypeDef,
+    DescribeTagsTypeDescribeTagsPaginateTypeDef,
+    LaunchConfigurationNamesTypeDescribeLaunchConfigurationsPaginateTypeDef,
     AutoScalingInstanceDetailsTypeDef,
     InstanceTypeDef,
     TagsTypeTypeDef,
     BatchDeleteScheduledActionAnswerTypeDef,
     BatchPutScheduledUpdateGroupActionAnswerTypeDef,
-    BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     BlockDeviceMappingTypeDef,
     CreateOrUpdateTagsTypeRequestTypeDef,
     DeleteTagsTypeRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
     DescribeLifecycleHooksAnswerTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeLoadBalancersResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
+    DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef,
+    DescribeScheduledActionsTypeRequestTypeDef,
+    GetPredictiveScalingForecastTypeRequestTypeDef,
+    PutScheduledUpdateGroupActionTypeRequestTypeDef,
+    ScheduledUpdateGroupActionRequestTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     InstanceRefreshProgressDetailsTypeDef,
+    InstanceRequirementsOutputTypeDef,
     InstanceRequirementsTypeDef,
     PutWarmPoolTypeRequestTypeDef,
     WarmPoolConfigurationTypeDef,
     ProcessesTypeTypeDef,
+    RefreshPreferencesUnionTypeDef,
     ScheduledActionsTypeTypeDef,
     AutoScalingInstancesTypeTypeDef,
     CreateLaunchConfigurationTypeRequestTypeDef,
     LaunchConfigurationTypeDef,
+    MetricStatOutputTypeDef,
+    TargetTrackingMetricStatOutputTypeDef,
     MetricStatTypeDef,
     TargetTrackingMetricStatTypeDef,
+    BatchPutScheduledUpdateGroupActionTypeRequestTypeDef,
     RollbackDetailsTypeDef,
+    LaunchTemplateOverridesOutputTypeDef,
     LaunchTemplateOverridesTypeDef,
     DescribeWarmPoolAnswerTypeDef,
     LaunchConfigurationsTypeTypeDef,
+    MetricDataQueryOutputTypeDef,
+    TargetTrackingMetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TargetTrackingMetricDataQueryTypeDef,
+    LaunchTemplateOutputTypeDef,
     LaunchTemplateTypeDef,
+    PredictiveScalingCustomizedCapacityMetricOutputTypeDef,
+    PredictiveScalingCustomizedLoadMetricOutputTypeDef,
+    PredictiveScalingCustomizedScalingMetricOutputTypeDef,
+    CustomizedMetricSpecificationOutputTypeDef,
     PredictiveScalingCustomizedCapacityMetricTypeDef,
     PredictiveScalingCustomizedLoadMetricTypeDef,
     PredictiveScalingCustomizedScalingMetricTypeDef,
     CustomizedMetricSpecificationTypeDef,
+    MixedInstancesPolicyOutputTypeDef,
     MixedInstancesPolicyTypeDef,
+    PredictiveScalingMetricSpecificationOutputTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
     PredictiveScalingMetricSpecificationTypeDef,
     TargetTrackingConfigurationTypeDef,
     AutoScalingGroupTypeDef,
+    DesiredConfigurationOutputTypeDef,
     CreateAutoScalingGroupTypeRequestTypeDef,
     DesiredConfigurationTypeDef,
+    MixedInstancesPolicyUnionTypeDef,
     UpdateAutoScalingGroupTypeRequestTypeDef,
     LoadForecastTypeDef,
+    PredictiveScalingConfigurationOutputTypeDef,
     PredictiveScalingConfigurationTypeDef,
+    TargetTrackingConfigurationUnionTypeDef,
     AutoScalingGroupsTypeTypeDef,
     InstanceRefreshTypeDef,
+    DesiredConfigurationUnionTypeDef,
     StartInstanceRefreshTypeRequestTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
-    PutScalingPolicyTypeRequestTypeDef,
     ScalingPolicyTypeDef,
+    PredictiveScalingConfigurationUnionTypeDef,
+    PutScalingPolicyTypeRequestTypeDef,
     DescribeInstanceRefreshesAnswerTypeDef,
     PoliciesTypeTypeDef,
 )
 
 
-def get_structure() -> AcceleratorCountRequestTypeDef:
+def get_value() -> AcceleratorCountRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-autoscaling-2.5.2/types_aiobotocore_autoscaling.egg-info/SOURCES.txt` & `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*


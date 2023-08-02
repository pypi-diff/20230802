# Comparing `tmp/types-aiobotocore-application-autoscaling-2.5.2.tar.gz` & `tmp/types-aiobotocore-application-autoscaling-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-application-autoscaling-2.5.2.tar", last modified: Sat Jul  8 01:43:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-application-autoscaling-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:52 2023, max compression
```

## Comparing `types-aiobotocore-application-autoscaling-2.5.2.tar` & `types-aiobotocore-application-autoscaling-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.441691 types-aiobotocore-application-autoscaling-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:46.000000 types-aiobotocore-application-autoscaling-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-07-08 01:43:14.437691 types-aiobotocore-application-autoscaling-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-07-08 01:25:46.000000 types-aiobotocore-application-autoscaling-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:14.441691 types-aiobotocore-application-autoscaling-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-08 01:25:46.000000 types-aiobotocore-application-autoscaling-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.437691 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-08 01:25:47.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-08 01:25:46.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-08 01:25:47.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-07-08 01:25:47.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-07-08 01:25:47.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-08 01:25:47.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-08 01:25:47.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-07-08 01:25:47.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-08 01:25:47.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:47.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22761 2023-07-08 01:25:47.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22718 2023-07-08 01:25:47.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:46.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.437691 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-07-08 01:43:14.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-08 01:43:14.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:14.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-08 01:43:14.000000 types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.729654 types-aiobotocore-application-autoscaling-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-08-02 14:51:52.729654 types-aiobotocore-application-autoscaling-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:52.729654 types-aiobotocore-application-autoscaling-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.729654 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17842 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26509 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.729654 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-08-02 14:51:52.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 14:51:52.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:52.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 14:51:52.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/LICENSE` & `types-aiobotocore-application-autoscaling-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/PKG-INFO` & `types-aiobotocore-application-autoscaling-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-application-autoscaling
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore application-autoscaling type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore application-autoscaling type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-application-autoscaling"></a>
 
 # types-aiobotocore-application-autoscaling
 
 [![PyPI - types-aiobotocore-application-autoscaling](https://img.shields.io/pypi/v/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-application-autoscaling?color=blue)](https://pypistats.org/packages/types-aiobotocore-application-autoscaling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-autoscaling)](https://pepy.tech/project/types-aiobotocore-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApplicationAutoScaling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [types-aiobotocore-application-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/).
 
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
@@ -332,72 +331,81 @@
 )
 
 
 def check_value(value: AdjustmentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_application_autoscaling.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_application_autoscaling.type_defs import (
     AlarmTypeDef,
     MetricDimensionTypeDef,
     DeleteScalingPolicyRequestRequestTypeDef,
     DeleteScheduledActionRequestRequestTypeDef,
     DeregisterScalableTargetRequestRequestTypeDef,
-    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeScalableTargetsRequestRequestTypeDef,
-    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    ResponseMetadataTypeDef,
     DescribeScalingActivitiesRequestRequestTypeDef,
-    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
-    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NotScaledReasonTypeDef,
-    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
+    TimestampTypeDef,
     SuspendedStateTypeDef,
-    RegisterScalableTargetResponseTypeDef,
-    ResponseMetadataTypeDef,
     StepAdjustmentTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetTrackingMetricDimensionTypeDef,
     UntagResourceRequestRequestTypeDef,
+    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
+    RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
-    PutScheduledActionRequestRequestTypeDef,
     ScheduledActionTypeDef,
+    PutScheduledActionRequestRequestTypeDef,
     RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
+    StepScalingPolicyConfigurationOutputTypeDef,
     StepScalingPolicyConfigurationTypeDef,
+    TargetTrackingMetricOutputTypeDef,
     TargetTrackingMetricTypeDef,
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     DescribeScalableTargetsResponseTypeDef,
+    StepScalingPolicyConfigurationUnionTypeDef,
+    TargetTrackingMetricStatOutputTypeDef,
     TargetTrackingMetricStatTypeDef,
+    TargetTrackingMetricDataQueryOutputTypeDef,
     TargetTrackingMetricDataQueryTypeDef,
+    CustomizedMetricSpecificationOutputTypeDef,
     CustomizedMetricSpecificationTypeDef,
+    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
     TargetTrackingScalingPolicyConfigurationTypeDef,
-    PutScalingPolicyRequestRequestTypeDef,
     ScalingPolicyTypeDef,
+    PutScalingPolicyRequestRequestTypeDef,
+    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
 )
 
 
-def get_structure() -> AlarmTypeDef:
+def get_value() -> AlarmTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/README.md` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-application-autoscaling
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore application-autoscaling type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-application-autoscaling"></a>
 
 # types-aiobotocore-application-autoscaling
 
 [![PyPI - types-aiobotocore-application-autoscaling](https://img.shields.io/pypi/v/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-application-autoscaling?color=blue)](https://pypistats.org/packages/types-aiobotocore-application-autoscaling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-autoscaling)](https://pepy.tech/project/types-aiobotocore-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApplicationAutoScaling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [types-aiobotocore-application-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/).
 
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
@@ -299,72 +331,81 @@
 )
 
 
 def check_value(value: AdjustmentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_application_autoscaling.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_application_autoscaling.type_defs import (
     AlarmTypeDef,
     MetricDimensionTypeDef,
     DeleteScalingPolicyRequestRequestTypeDef,
     DeleteScheduledActionRequestRequestTypeDef,
     DeregisterScalableTargetRequestRequestTypeDef,
-    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeScalableTargetsRequestRequestTypeDef,
-    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    ResponseMetadataTypeDef,
     DescribeScalingActivitiesRequestRequestTypeDef,
-    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
-    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NotScaledReasonTypeDef,
-    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
+    TimestampTypeDef,
     SuspendedStateTypeDef,
-    RegisterScalableTargetResponseTypeDef,
-    ResponseMetadataTypeDef,
     StepAdjustmentTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetTrackingMetricDimensionTypeDef,
     UntagResourceRequestRequestTypeDef,
+    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
+    RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
-    PutScheduledActionRequestRequestTypeDef,
     ScheduledActionTypeDef,
+    PutScheduledActionRequestRequestTypeDef,
     RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
+    StepScalingPolicyConfigurationOutputTypeDef,
     StepScalingPolicyConfigurationTypeDef,
+    TargetTrackingMetricOutputTypeDef,
     TargetTrackingMetricTypeDef,
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     DescribeScalableTargetsResponseTypeDef,
+    StepScalingPolicyConfigurationUnionTypeDef,
+    TargetTrackingMetricStatOutputTypeDef,
     TargetTrackingMetricStatTypeDef,
+    TargetTrackingMetricDataQueryOutputTypeDef,
     TargetTrackingMetricDataQueryTypeDef,
+    CustomizedMetricSpecificationOutputTypeDef,
     CustomizedMetricSpecificationTypeDef,
+    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
     TargetTrackingScalingPolicyConfigurationTypeDef,
-    PutScalingPolicyRequestRequestTypeDef,
     ScalingPolicyTypeDef,
+    PutScalingPolicyRequestRequestTypeDef,
+    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
 )
 
 
-def get_structure() -> AlarmTypeDef:
+def get_value() -> AlarmTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/setup.py` & `types-aiobotocore-application-autoscaling-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,46 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-application-autoscaling",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_application_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2 service generated with"
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
     keywords=(
-        "aiobotocore application-autoscaling type-annotations boto3-stubs mypy typeshed"
-        " autocomplete"
+        "aiobotocore application-autoscaling type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_application_autoscaling": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/",
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/__init__.py` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/__init__.pyi` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/__main__.py` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling\nOther"
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

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/client.py` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("application-autoscaling") as client:
         client: ApplicationAutoScalingClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import PolicyTypeType, ScalableDimensionType, ServiceNamespaceType
 from .paginator import (
     DescribeScalableTargetsPaginator,
@@ -33,17 +32,18 @@
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
     RegisterScalableTargetResponseTypeDef,
     ScalableTargetActionTypeDef,
-    StepScalingPolicyConfigurationTypeDef,
+    StepScalingPolicyConfigurationUnionTypeDef,
     SuspendedStateTypeDef,
-    TargetTrackingScalingPolicyConfigurationTypeDef,
+    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -250,16 +250,16 @@
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         PolicyType: PolicyTypeType = ...,
-        StepScalingPolicyConfiguration: StepScalingPolicyConfigurationTypeDef = ...,
-        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationTypeDef = ...
+        StepScalingPolicyConfiguration: StepScalingPolicyConfigurationUnionTypeDef = ...,
+        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationUnionTypeDef = ...
     ) -> PutScalingPolicyResponseTypeDef:
         """
         Creates or updates a scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#put_scaling_policy)
@@ -270,16 +270,16 @@
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionName: str,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         Schedule: str = ...,
         Timezone: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         ScalableTargetAction: ScalableTargetActionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scheduled_action)
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/client.pyi` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("application-autoscaling") as client:
         client: ApplicationAutoScalingClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import PolicyTypeType, ScalableDimensionType, ServiceNamespaceType
 from .paginator import (
     DescribeScalableTargetsPaginator,
@@ -33,17 +32,18 @@
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
     RegisterScalableTargetResponseTypeDef,
     ScalableTargetActionTypeDef,
-    StepScalingPolicyConfigurationTypeDef,
+    StepScalingPolicyConfigurationUnionTypeDef,
     SuspendedStateTypeDef,
-    TargetTrackingScalingPolicyConfigurationTypeDef,
+    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -234,16 +234,16 @@
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         PolicyType: PolicyTypeType = ...,
-        StepScalingPolicyConfiguration: StepScalingPolicyConfigurationTypeDef = ...,
-        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationTypeDef = ...
+        StepScalingPolicyConfiguration: StepScalingPolicyConfigurationUnionTypeDef = ...,
+        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationUnionTypeDef = ...
     ) -> PutScalingPolicyResponseTypeDef:
         """
         Creates or updates a scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#put_scaling_policy)
@@ -253,16 +253,16 @@
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionName: str,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         Schedule: str = ...,
         Timezone: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         ScalableTargetAction: ScalableTargetActionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates or updates a scheduled action for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scheduled_action)
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/literals.py` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/literals.pyi` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/paginator.py` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,99 +43,93 @@
 __all__ = (
     "DescribeScalableTargetsPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScalingPoliciesPaginator",
     "DescribeScheduledActionsPaginator",
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
 class DescribeScalableTargetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalabletargetspaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScalableTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalabletargetspaginator)
         """
 
-
 class DescribeScalingActivitiesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalingactivitiespaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         IncludeNotScaledActivities: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScalingActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
-
 class DescribeScalingPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalingpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScalingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalingpoliciespaginator)
         """
 
-
 class DescribeScheduledActionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescheduledactionspaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScheduledActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescheduledactionspaginator)
         """
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/paginator.pyi` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,93 +43,99 @@
 __all__ = (
     "DescribeScalableTargetsPaginator",
     "DescribeScalingActivitiesPaginator",
     "DescribeScalingPoliciesPaginator",
     "DescribeScheduledActionsPaginator",
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
 class DescribeScalableTargetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalabletargetspaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceIds: Sequence[str] = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScalableTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalabletargetspaginator)
         """
 
+
 class DescribeScalingActivitiesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalingactivitiespaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
         IncludeNotScaledActivities: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScalingActivitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalingactivitiespaginator)
         """
 
+
 class DescribeScalingPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalingpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         PolicyNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScalingPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescalingpoliciespaginator)
         """
 
+
 class DescribeScheduledActionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescheduledactionspaginator)
     """
 
     def paginate(
         self,
         *,
         ServiceNamespace: ServiceNamespaceType,
         ScheduledActionNames: Sequence[str] = ...,
         ResourceId: str = ...,
         ScalableDimension: ScalableDimensionType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScheduledActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/paginators/#describescheduledactionspaginator)
         """
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/type_defs.py` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/type_defs.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_application_autoscaling.type_defs import AlarmTypeDef
 
-    data: AlarmTypeDef = {...}
+    data: AlarmTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -34,52 +34,61 @@
 
 __all__ = (
     "AlarmTypeDef",
     "MetricDimensionTypeDef",
     "DeleteScalingPolicyRequestRequestTypeDef",
     "DeleteScheduledActionRequestRequestTypeDef",
     "DeregisterScalableTargetRequestRequestTypeDef",
-    "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeScalableTargetsRequestRequestTypeDef",
-    "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeScalingActivitiesRequestRequestTypeDef",
-    "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     "DescribeScalingPoliciesRequestRequestTypeDef",
-    "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NotScaledReasonTypeDef",
-    "PaginatorConfigTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "ScalableTargetActionTypeDef",
+    "TimestampTypeDef",
     "SuspendedStateTypeDef",
-    "RegisterScalableTargetResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StepAdjustmentTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TargetTrackingMetricDimensionTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
+    "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutScalingPolicyResponseTypeDef",
+    "RegisterScalableTargetResponseTypeDef",
     "ScalingActivityTypeDef",
-    "PutScheduledActionRequestRequestTypeDef",
     "ScheduledActionTypeDef",
+    "PutScheduledActionRequestRequestTypeDef",
     "RegisterScalableTargetRequestRequestTypeDef",
     "ScalableTargetTypeDef",
+    "StepScalingPolicyConfigurationOutputTypeDef",
     "StepScalingPolicyConfigurationTypeDef",
+    "TargetTrackingMetricOutputTypeDef",
     "TargetTrackingMetricTypeDef",
     "DescribeScalingActivitiesResponseTypeDef",
     "DescribeScheduledActionsResponseTypeDef",
     "DescribeScalableTargetsResponseTypeDef",
+    "StepScalingPolicyConfigurationUnionTypeDef",
+    "TargetTrackingMetricStatOutputTypeDef",
     "TargetTrackingMetricStatTypeDef",
+    "TargetTrackingMetricDataQueryOutputTypeDef",
     "TargetTrackingMetricDataQueryTypeDef",
+    "CustomizedMetricSpecificationOutputTypeDef",
     "CustomizedMetricSpecificationTypeDef",
+    "TargetTrackingScalingPolicyConfigurationOutputTypeDef",
     "TargetTrackingScalingPolicyConfigurationTypeDef",
-    "PutScalingPolicyRequestRequestTypeDef",
     "ScalingPolicyTypeDef",
+    "PutScalingPolicyRequestRequestTypeDef",
+    "TargetTrackingScalingPolicyConfigurationUnionTypeDef",
     "DescribeScalingPoliciesResponseTypeDef",
 )
 
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "AlarmName": str,
@@ -120,38 +129,24 @@
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
     },
 )
 
-_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ResourceIds": Sequence[str],
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
-    _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-    _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeScalableTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalableTargetsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalableTargetsRequestRequestTypeDef = TypedDict(
@@ -169,39 +164,25 @@
 class DescribeScalableTargetsRequestRequestTypeDef(
     _RequiredDescribeScalableTargetsRequestRequestTypeDef,
     _OptionalDescribeScalableTargetsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "IncludeNotScaledActivities": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
-    _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-    _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeScalingActivitiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingActivitiesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingActivitiesRequestRequestTypeDef = TypedDict(
@@ -220,39 +201,14 @@
 class DescribeScalingActivitiesRequestRequestTypeDef(
     _RequiredDescribeScalingActivitiesRequestRequestTypeDef,
     _OptionalDescribeScalingActivitiesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    {
-        "PolicyNames": Sequence[str],
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
-    _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-    _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
@@ -271,39 +227,14 @@
 class DescribeScalingPoliciesRequestRequestTypeDef(
     _RequiredDescribeScalingPoliciesRequestRequestTypeDef,
     _OptionalDescribeScalingPoliciesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    {
-        "ScheduledActionNames": Sequence[str],
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
-    _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-    _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
@@ -329,22 +260,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredNotScaledReasonTypeDef = TypedDict(
     "_RequiredNotScaledReasonTypeDef",
     {
         "Code": str,
     },
 )
 _OptionalNotScaledReasonTypeDef = TypedDict(
@@ -358,24 +281,14 @@
 )
 
 
 class NotScaledReasonTypeDef(_RequiredNotScaledReasonTypeDef, _OptionalNotScaledReasonTypeDef):
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
-
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
@@ -398,43 +311,25 @@
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 SuspendedStateTypeDef = TypedDict(
     "SuspendedStateTypeDef",
     {
         "DynamicScalingInSuspended": bool,
         "DynamicScalingOutSuspended": bool,
         "ScheduledScalingSuspended": bool,
     },
     total=False,
 )
 
-RegisterScalableTargetResponseTypeDef = TypedDict(
-    "RegisterScalableTargetResponseTypeDef",
-    {
-        "ScalableTargetARN": str,
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
 _RequiredStepAdjustmentTypeDef = TypedDict(
     "_RequiredStepAdjustmentTypeDef",
     {
         "ScalingAdjustment": int,
     },
 )
 _OptionalStepAdjustmentTypeDef = TypedDict(
@@ -471,20 +366,135 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    {
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    {
+        "ResourceIds": Sequence[str],
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
+    _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    {
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    {
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "IncludeNotScaledActivities": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
+    _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
+    {
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
+    {
+        "PolicyNames": Sequence[str],
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
+    _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+    _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    {
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    {
+        "ScheduledActionNames": Sequence[str],
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
+    _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+):
+    pass
+
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutScalingPolicyResponseTypeDef = TypedDict(
     "PutScalingPolicyResponseTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterScalableTargetResponseTypeDef = TypedDict(
+    "RegisterScalableTargetResponseTypeDef",
+    {
+        "ScalableTargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredScalingActivityTypeDef = TypedDict(
     "_RequiredScalingActivityTypeDef",
     {
         "ActivityId": str,
@@ -509,68 +519,68 @@
 )
 
 
 class ScalingActivityTypeDef(_RequiredScalingActivityTypeDef, _OptionalScalingActivityTypeDef):
     pass
 
 
-_RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutScheduledActionRequestRequestTypeDef",
+_RequiredScheduledActionTypeDef = TypedDict(
+    "_RequiredScheduledActionTypeDef",
     {
-        "ServiceNamespace": ServiceNamespaceType,
         "ScheduledActionName": str,
+        "ScheduledActionARN": str,
+        "ServiceNamespace": ServiceNamespaceType,
+        "Schedule": str,
         "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
+        "CreationTime": datetime,
     },
 )
-_OptionalPutScheduledActionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutScheduledActionRequestRequestTypeDef",
+_OptionalScheduledActionTypeDef = TypedDict(
+    "_OptionalScheduledActionTypeDef",
     {
-        "Schedule": str,
         "Timezone": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "ScalableDimension": ScalableDimensionType,
+        "StartTime": datetime,
+        "EndTime": datetime,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
 
-class PutScheduledActionRequestRequestTypeDef(
-    _RequiredPutScheduledActionRequestRequestTypeDef,
-    _OptionalPutScheduledActionRequestRequestTypeDef,
-):
+class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
     pass
 
 
-_RequiredScheduledActionTypeDef = TypedDict(
-    "_RequiredScheduledActionTypeDef",
+_RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutScheduledActionRequestRequestTypeDef",
     {
-        "ScheduledActionName": str,
-        "ScheduledActionARN": str,
         "ServiceNamespace": ServiceNamespaceType,
-        "Schedule": str,
+        "ScheduledActionName": str,
         "ResourceId": str,
-        "CreationTime": datetime,
+        "ScalableDimension": ScalableDimensionType,
     },
 )
-_OptionalScheduledActionTypeDef = TypedDict(
-    "_OptionalScheduledActionTypeDef",
+_OptionalPutScheduledActionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutScheduledActionRequestRequestTypeDef",
     {
+        "Schedule": str,
         "Timezone": str,
-        "ScalableDimension": ScalableDimensionType,
-        "StartTime": datetime,
-        "EndTime": datetime,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
 
-class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
+class PutScheduledActionRequestRequestTypeDef(
+    _RequiredPutScheduledActionRequestRequestTypeDef,
+    _OptionalPutScheduledActionRequestRequestTypeDef,
+):
     pass
 
 
 _RequiredRegisterScalableTargetRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterScalableTargetRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
@@ -620,63 +630,110 @@
 )
 
 
 class ScalableTargetTypeDef(_RequiredScalableTargetTypeDef, _OptionalScalableTargetTypeDef):
     pass
 
 
+StepScalingPolicyConfigurationOutputTypeDef = TypedDict(
+    "StepScalingPolicyConfigurationOutputTypeDef",
+    {
+        "AdjustmentType": AdjustmentTypeType,
+        "StepAdjustments": List[StepAdjustmentTypeDef],
+        "MinAdjustmentMagnitude": int,
+        "Cooldown": int,
+        "MetricAggregationType": MetricAggregationTypeType,
+    },
+    total=False,
+)
+
 StepScalingPolicyConfigurationTypeDef = TypedDict(
     "StepScalingPolicyConfigurationTypeDef",
     {
         "AdjustmentType": AdjustmentTypeType,
-        "StepAdjustments": List[StepAdjustmentTypeDef],
+        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "MinAdjustmentMagnitude": int,
         "Cooldown": int,
         "MetricAggregationType": MetricAggregationTypeType,
     },
     total=False,
 )
 
+TargetTrackingMetricOutputTypeDef = TypedDict(
+    "TargetTrackingMetricOutputTypeDef",
+    {
+        "Dimensions": List[TargetTrackingMetricDimensionTypeDef],
+        "MetricName": str,
+        "Namespace": str,
+    },
+    total=False,
+)
+
 TargetTrackingMetricTypeDef = TypedDict(
     "TargetTrackingMetricTypeDef",
     {
-        "Dimensions": List[TargetTrackingMetricDimensionTypeDef],
+        "Dimensions": Sequence[TargetTrackingMetricDimensionTypeDef],
         "MetricName": str,
         "Namespace": str,
     },
     total=False,
 )
 
 DescribeScalingActivitiesResponseTypeDef = TypedDict(
     "DescribeScalingActivitiesResponseTypeDef",
     {
         "ScalingActivities": List[ScalingActivityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScheduledActionsResponseTypeDef = TypedDict(
     "DescribeScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScalableTargetsResponseTypeDef = TypedDict(
     "DescribeScalableTargetsResponseTypeDef",
     {
         "ScalableTargets": List[ScalableTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StepScalingPolicyConfigurationUnionTypeDef = Union[
+    StepScalingPolicyConfigurationTypeDef, StepScalingPolicyConfigurationOutputTypeDef
+]
+_RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricStatOutputTypeDef",
+    {
+        "Metric": TargetTrackingMetricOutputTypeDef,
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
 _RequiredTargetTrackingMetricStatTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatTypeDef",
     {
         "Metric": TargetTrackingMetricTypeDef,
         "Stat": str,
     },
 )
@@ -691,14 +748,39 @@
 
 class TargetTrackingMetricStatTypeDef(
     _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
 ):
     pass
 
 
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
+        "Label": str,
+        "MetricStat": TargetTrackingMetricStatOutputTypeDef,
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
 _RequiredTargetTrackingMetricDataQueryTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryTypeDef = TypedDict(
@@ -715,27 +797,66 @@
 
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
 
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
+_RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef",
+    {
+        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
+        "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
+        "ScaleOutCooldown": int,
+        "ScaleInCooldown": int,
+        "DisableScaleIn": bool,
     },
     total=False,
 )
 
+
+class TargetTrackingScalingPolicyConfigurationOutputTypeDef(
+    _RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef,
+    _OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredTargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingScalingPolicyConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
@@ -754,68 +875,74 @@
 class TargetTrackingScalingPolicyConfigurationTypeDef(
     _RequiredTargetTrackingScalingPolicyConfigurationTypeDef,
     _OptionalTargetTrackingScalingPolicyConfigurationTypeDef,
 ):
     pass
 
 
-_RequiredPutScalingPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredPutScalingPolicyRequestRequestTypeDef",
+_RequiredScalingPolicyTypeDef = TypedDict(
+    "_RequiredScalingPolicyTypeDef",
     {
+        "PolicyARN": str,
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
+        "PolicyType": PolicyTypeType,
+        "CreationTime": datetime,
     },
 )
-_OptionalPutScalingPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalPutScalingPolicyRequestRequestTypeDef",
+_OptionalScalingPolicyTypeDef = TypedDict(
+    "_OptionalScalingPolicyTypeDef",
     {
-        "PolicyType": PolicyTypeType,
-        "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
-        "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
+        "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationOutputTypeDef,
+        "TargetTrackingScalingPolicyConfiguration": (
+            TargetTrackingScalingPolicyConfigurationOutputTypeDef
+        ),
+        "Alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
 
-class PutScalingPolicyRequestRequestTypeDef(
-    _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
-):
+class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
 
-_RequiredScalingPolicyTypeDef = TypedDict(
-    "_RequiredScalingPolicyTypeDef",
+_RequiredPutScalingPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPutScalingPolicyRequestRequestTypeDef",
     {
-        "PolicyARN": str,
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
-        "PolicyType": PolicyTypeType,
-        "CreationTime": datetime,
     },
 )
-_OptionalScalingPolicyTypeDef = TypedDict(
-    "_OptionalScalingPolicyTypeDef",
+_OptionalPutScalingPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPutScalingPolicyRequestRequestTypeDef",
     {
+        "PolicyType": PolicyTypeType,
         "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
         "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
-        "Alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
 
-class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
+class PutScalingPolicyRequestRequestTypeDef(
+    _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
+):
     pass
 
 
+TargetTrackingScalingPolicyConfigurationUnionTypeDef = Union[
+    TargetTrackingScalingPolicyConfigurationTypeDef,
+    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
+]
 DescribeScalingPoliciesResponseTypeDef = TypedDict(
     "DescribeScalingPoliciesResponseTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling/type_defs.pyi` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/type_defs.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_application_autoscaling.type_defs import AlarmTypeDef
 
-    data: AlarmTypeDef = {...}
+    data: AlarmTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -33,52 +33,61 @@
 
 __all__ = (
     "AlarmTypeDef",
     "MetricDimensionTypeDef",
     "DeleteScalingPolicyRequestRequestTypeDef",
     "DeleteScheduledActionRequestRequestTypeDef",
     "DeregisterScalableTargetRequestRequestTypeDef",
-    "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeScalableTargetsRequestRequestTypeDef",
-    "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeScalingActivitiesRequestRequestTypeDef",
-    "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     "DescribeScalingPoliciesRequestRequestTypeDef",
-    "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "NotScaledReasonTypeDef",
-    "PaginatorConfigTypeDef",
     "PredefinedMetricSpecificationTypeDef",
     "ScalableTargetActionTypeDef",
+    "TimestampTypeDef",
     "SuspendedStateTypeDef",
-    "RegisterScalableTargetResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "StepAdjustmentTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TargetTrackingMetricDimensionTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    "DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    "DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
+    "DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "PutScalingPolicyResponseTypeDef",
+    "RegisterScalableTargetResponseTypeDef",
     "ScalingActivityTypeDef",
-    "PutScheduledActionRequestRequestTypeDef",
     "ScheduledActionTypeDef",
+    "PutScheduledActionRequestRequestTypeDef",
     "RegisterScalableTargetRequestRequestTypeDef",
     "ScalableTargetTypeDef",
+    "StepScalingPolicyConfigurationOutputTypeDef",
     "StepScalingPolicyConfigurationTypeDef",
+    "TargetTrackingMetricOutputTypeDef",
     "TargetTrackingMetricTypeDef",
     "DescribeScalingActivitiesResponseTypeDef",
     "DescribeScheduledActionsResponseTypeDef",
     "DescribeScalableTargetsResponseTypeDef",
+    "StepScalingPolicyConfigurationUnionTypeDef",
+    "TargetTrackingMetricStatOutputTypeDef",
     "TargetTrackingMetricStatTypeDef",
+    "TargetTrackingMetricDataQueryOutputTypeDef",
     "TargetTrackingMetricDataQueryTypeDef",
+    "CustomizedMetricSpecificationOutputTypeDef",
     "CustomizedMetricSpecificationTypeDef",
+    "TargetTrackingScalingPolicyConfigurationOutputTypeDef",
     "TargetTrackingScalingPolicyConfigurationTypeDef",
-    "PutScalingPolicyRequestRequestTypeDef",
     "ScalingPolicyTypeDef",
+    "PutScalingPolicyRequestRequestTypeDef",
+    "TargetTrackingScalingPolicyConfigurationUnionTypeDef",
     "DescribeScalingPoliciesResponseTypeDef",
 )
 
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "AlarmName": str,
@@ -119,36 +128,24 @@
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
     },
 )
 
-_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ResourceIds": Sequence[str],
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
-    _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-    _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeScalableTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalableTargetsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalableTargetsRequestRequestTypeDef = TypedDict(
@@ -164,37 +161,25 @@
 
 class DescribeScalableTargetsRequestRequestTypeDef(
     _RequiredDescribeScalableTargetsRequestRequestTypeDef,
     _OptionalDescribeScalableTargetsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "IncludeNotScaledActivities": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
-    _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-    _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeScalingActivitiesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingActivitiesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingActivitiesRequestRequestTypeDef = TypedDict(
@@ -211,37 +196,14 @@
 
 class DescribeScalingActivitiesRequestRequestTypeDef(
     _RequiredDescribeScalingActivitiesRequestRequestTypeDef,
     _OptionalDescribeScalingActivitiesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
-    {
-        "PolicyNames": Sequence[str],
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
-    _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-    _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
@@ -258,37 +220,14 @@
 
 class DescribeScalingPoliciesRequestRequestTypeDef(
     _RequiredDescribeScalingPoliciesRequestRequestTypeDef,
     _OptionalDescribeScalingPoliciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-    },
-)
-_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
-    {
-        "ScheduledActionNames": Sequence[str],
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
-    _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-    _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
@@ -312,22 +251,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredNotScaledReasonTypeDef = TypedDict(
     "_RequiredNotScaledReasonTypeDef",
     {
         "Code": str,
     },
 )
 _OptionalNotScaledReasonTypeDef = TypedDict(
@@ -339,24 +270,14 @@
     },
     total=False,
 )
 
 class NotScaledReasonTypeDef(_RequiredNotScaledReasonTypeDef, _OptionalNotScaledReasonTypeDef):
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
-
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
@@ -377,43 +298,25 @@
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 SuspendedStateTypeDef = TypedDict(
     "SuspendedStateTypeDef",
     {
         "DynamicScalingInSuspended": bool,
         "DynamicScalingOutSuspended": bool,
         "ScheduledScalingSuspended": bool,
     },
     total=False,
 )
 
-RegisterScalableTargetResponseTypeDef = TypedDict(
-    "RegisterScalableTargetResponseTypeDef",
-    {
-        "ScalableTargetARN": str,
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
 _RequiredStepAdjustmentTypeDef = TypedDict(
     "_RequiredStepAdjustmentTypeDef",
     {
         "ScalingAdjustment": int,
     },
 )
 _OptionalStepAdjustmentTypeDef = TypedDict(
@@ -448,20 +351,127 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    {
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef",
+    {
+        "ResourceIds": Sequence[str],
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
+    _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    {
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
+    {
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "IncludeNotScaledActivities": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
+    _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
+    {
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
+    {
+        "PolicyNames": Sequence[str],
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
+    _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+    _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    {
+        "ServiceNamespace": ServiceNamespaceType,
+    },
+)
+_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
+    {
+        "ScheduledActionNames": Sequence[str],
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
+    _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+):
+    pass
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PutScalingPolicyResponseTypeDef = TypedDict(
     "PutScalingPolicyResponseTypeDef",
     {
         "PolicyARN": str,
         "Alarms": List[AlarmTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterScalableTargetResponseTypeDef = TypedDict(
+    "RegisterScalableTargetResponseTypeDef",
+    {
+        "ScalableTargetARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredScalingActivityTypeDef = TypedDict(
     "_RequiredScalingActivityTypeDef",
     {
         "ActivityId": str,
@@ -484,65 +494,65 @@
     },
     total=False,
 )
 
 class ScalingActivityTypeDef(_RequiredScalingActivityTypeDef, _OptionalScalingActivityTypeDef):
     pass
 
-_RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutScheduledActionRequestRequestTypeDef",
+_RequiredScheduledActionTypeDef = TypedDict(
+    "_RequiredScheduledActionTypeDef",
     {
-        "ServiceNamespace": ServiceNamespaceType,
         "ScheduledActionName": str,
+        "ScheduledActionARN": str,
+        "ServiceNamespace": ServiceNamespaceType,
+        "Schedule": str,
         "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
+        "CreationTime": datetime,
     },
 )
-_OptionalPutScheduledActionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutScheduledActionRequestRequestTypeDef",
+_OptionalScheduledActionTypeDef = TypedDict(
+    "_OptionalScheduledActionTypeDef",
     {
-        "Schedule": str,
         "Timezone": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "ScalableDimension": ScalableDimensionType,
+        "StartTime": datetime,
+        "EndTime": datetime,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
-class PutScheduledActionRequestRequestTypeDef(
-    _RequiredPutScheduledActionRequestRequestTypeDef,
-    _OptionalPutScheduledActionRequestRequestTypeDef,
-):
+class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
     pass
 
-_RequiredScheduledActionTypeDef = TypedDict(
-    "_RequiredScheduledActionTypeDef",
+_RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutScheduledActionRequestRequestTypeDef",
     {
-        "ScheduledActionName": str,
-        "ScheduledActionARN": str,
         "ServiceNamespace": ServiceNamespaceType,
-        "Schedule": str,
+        "ScheduledActionName": str,
         "ResourceId": str,
-        "CreationTime": datetime,
+        "ScalableDimension": ScalableDimensionType,
     },
 )
-_OptionalScheduledActionTypeDef = TypedDict(
-    "_OptionalScheduledActionTypeDef",
+_OptionalPutScheduledActionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutScheduledActionRequestRequestTypeDef",
     {
+        "Schedule": str,
         "Timezone": str,
-        "ScalableDimension": ScalableDimensionType,
-        "StartTime": datetime,
-        "EndTime": datetime,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
-class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
+class PutScheduledActionRequestRequestTypeDef(
+    _RequiredPutScheduledActionRequestRequestTypeDef,
+    _OptionalPutScheduledActionRequestRequestTypeDef,
+):
     pass
 
 _RequiredRegisterScalableTargetRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterScalableTargetRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
@@ -587,63 +597,108 @@
     },
     total=False,
 )
 
 class ScalableTargetTypeDef(_RequiredScalableTargetTypeDef, _OptionalScalableTargetTypeDef):
     pass
 
+StepScalingPolicyConfigurationOutputTypeDef = TypedDict(
+    "StepScalingPolicyConfigurationOutputTypeDef",
+    {
+        "AdjustmentType": AdjustmentTypeType,
+        "StepAdjustments": List[StepAdjustmentTypeDef],
+        "MinAdjustmentMagnitude": int,
+        "Cooldown": int,
+        "MetricAggregationType": MetricAggregationTypeType,
+    },
+    total=False,
+)
+
 StepScalingPolicyConfigurationTypeDef = TypedDict(
     "StepScalingPolicyConfigurationTypeDef",
     {
         "AdjustmentType": AdjustmentTypeType,
-        "StepAdjustments": List[StepAdjustmentTypeDef],
+        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "MinAdjustmentMagnitude": int,
         "Cooldown": int,
         "MetricAggregationType": MetricAggregationTypeType,
     },
     total=False,
 )
 
+TargetTrackingMetricOutputTypeDef = TypedDict(
+    "TargetTrackingMetricOutputTypeDef",
+    {
+        "Dimensions": List[TargetTrackingMetricDimensionTypeDef],
+        "MetricName": str,
+        "Namespace": str,
+    },
+    total=False,
+)
+
 TargetTrackingMetricTypeDef = TypedDict(
     "TargetTrackingMetricTypeDef",
     {
-        "Dimensions": List[TargetTrackingMetricDimensionTypeDef],
+        "Dimensions": Sequence[TargetTrackingMetricDimensionTypeDef],
         "MetricName": str,
         "Namespace": str,
     },
     total=False,
 )
 
 DescribeScalingActivitiesResponseTypeDef = TypedDict(
     "DescribeScalingActivitiesResponseTypeDef",
     {
         "ScalingActivities": List[ScalingActivityTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScheduledActionsResponseTypeDef = TypedDict(
     "DescribeScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScalableTargetsResponseTypeDef = TypedDict(
     "DescribeScalableTargetsResponseTypeDef",
     {
         "ScalableTargets": List[ScalableTargetTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StepScalingPolicyConfigurationUnionTypeDef = Union[
+    StepScalingPolicyConfigurationTypeDef, StepScalingPolicyConfigurationOutputTypeDef
+]
+_RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingMetricStatOutputTypeDef",
+    {
+        "Metric": TargetTrackingMetricOutputTypeDef,
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
 _RequiredTargetTrackingMetricStatTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatTypeDef",
     {
         "Metric": TargetTrackingMetricTypeDef,
         "Stat": str,
     },
 )
@@ -656,14 +711,37 @@
 )
 
 class TargetTrackingMetricStatTypeDef(
     _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
 ):
     pass
 
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
+        "Label": str,
+        "MetricStat": TargetTrackingMetricStatOutputTypeDef,
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
 _RequiredTargetTrackingMetricDataQueryTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryTypeDef = TypedDict(
@@ -678,27 +756,64 @@
 )
 
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
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
+_RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef",
+    {
+        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
+        "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
+        "ScaleOutCooldown": int,
+        "ScaleInCooldown": int,
+        "DisableScaleIn": bool,
     },
     total=False,
 )
 
+class TargetTrackingScalingPolicyConfigurationOutputTypeDef(
+    _RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef,
+    _OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredTargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingScalingPolicyConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
@@ -715,64 +830,70 @@
 
 class TargetTrackingScalingPolicyConfigurationTypeDef(
     _RequiredTargetTrackingScalingPolicyConfigurationTypeDef,
     _OptionalTargetTrackingScalingPolicyConfigurationTypeDef,
 ):
     pass
 
-_RequiredPutScalingPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredPutScalingPolicyRequestRequestTypeDef",
+_RequiredScalingPolicyTypeDef = TypedDict(
+    "_RequiredScalingPolicyTypeDef",
     {
+        "PolicyARN": str,
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
+        "PolicyType": PolicyTypeType,
+        "CreationTime": datetime,
     },
 )
-_OptionalPutScalingPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalPutScalingPolicyRequestRequestTypeDef",
+_OptionalScalingPolicyTypeDef = TypedDict(
+    "_OptionalScalingPolicyTypeDef",
     {
-        "PolicyType": PolicyTypeType,
-        "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
-        "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
+        "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationOutputTypeDef,
+        "TargetTrackingScalingPolicyConfiguration": (
+            TargetTrackingScalingPolicyConfigurationOutputTypeDef
+        ),
+        "Alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
-class PutScalingPolicyRequestRequestTypeDef(
-    _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
-):
+class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
-_RequiredScalingPolicyTypeDef = TypedDict(
-    "_RequiredScalingPolicyTypeDef",
+_RequiredPutScalingPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPutScalingPolicyRequestRequestTypeDef",
     {
-        "PolicyARN": str,
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
-        "PolicyType": PolicyTypeType,
-        "CreationTime": datetime,
     },
 )
-_OptionalScalingPolicyTypeDef = TypedDict(
-    "_OptionalScalingPolicyTypeDef",
+_OptionalPutScalingPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPutScalingPolicyRequestRequestTypeDef",
     {
+        "PolicyType": PolicyTypeType,
         "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
         "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
-        "Alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
-class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
+class PutScalingPolicyRequestRequestTypeDef(
+    _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
+):
     pass
 
+TargetTrackingScalingPolicyConfigurationUnionTypeDef = Union[
+    TargetTrackingScalingPolicyConfigurationTypeDef,
+    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
+]
 DescribeScalingPoliciesResponseTypeDef = TypedDict(
     "DescribeScalingPoliciesResponseTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO` & `types-aiobotocore-application-autoscaling-2.5.2.post1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-application-autoscaling
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore application-autoscaling type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-application-autoscaling"></a>
 
 # types-aiobotocore-application-autoscaling
 
 [![PyPI - types-aiobotocore-application-autoscaling](https://img.shields.io/pypi/v/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-application-autoscaling?color=blue)](https://pypistats.org/packages/types-aiobotocore-application-autoscaling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-autoscaling)](https://pepy.tech/project/types-aiobotocore-application-autoscaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApplicationAutoScaling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
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
 [types-aiobotocore-application-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/).
 
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
@@ -332,72 +299,81 @@
 )
 
 
 def check_value(value: AdjustmentTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_application_autoscaling.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_application_autoscaling.type_defs import (
     AlarmTypeDef,
     MetricDimensionTypeDef,
     DeleteScalingPolicyRequestRequestTypeDef,
     DeleteScheduledActionRequestRequestTypeDef,
     DeregisterScalableTargetRequestRequestTypeDef,
-    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeScalableTargetsRequestRequestTypeDef,
-    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    ResponseMetadataTypeDef,
     DescribeScalingActivitiesRequestRequestTypeDef,
-    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     DescribeScalingPoliciesRequestRequestTypeDef,
-    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     NotScaledReasonTypeDef,
-    PaginatorConfigTypeDef,
     PredefinedMetricSpecificationTypeDef,
     ScalableTargetActionTypeDef,
+    TimestampTypeDef,
     SuspendedStateTypeDef,
-    RegisterScalableTargetResponseTypeDef,
-    ResponseMetadataTypeDef,
     StepAdjustmentTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetTrackingMetricDimensionTypeDef,
     UntagResourceRequestRequestTypeDef,
+    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
+    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
+    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
+    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
+    ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
+    RegisterScalableTargetResponseTypeDef,
     ScalingActivityTypeDef,
-    PutScheduledActionRequestRequestTypeDef,
     ScheduledActionTypeDef,
+    PutScheduledActionRequestRequestTypeDef,
     RegisterScalableTargetRequestRequestTypeDef,
     ScalableTargetTypeDef,
+    StepScalingPolicyConfigurationOutputTypeDef,
     StepScalingPolicyConfigurationTypeDef,
+    TargetTrackingMetricOutputTypeDef,
     TargetTrackingMetricTypeDef,
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     DescribeScalableTargetsResponseTypeDef,
+    StepScalingPolicyConfigurationUnionTypeDef,
+    TargetTrackingMetricStatOutputTypeDef,
     TargetTrackingMetricStatTypeDef,
+    TargetTrackingMetricDataQueryOutputTypeDef,
     TargetTrackingMetricDataQueryTypeDef,
+    CustomizedMetricSpecificationOutputTypeDef,
     CustomizedMetricSpecificationTypeDef,
+    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
     TargetTrackingScalingPolicyConfigurationTypeDef,
-    PutScalingPolicyRequestRequestTypeDef,
     ScalingPolicyTypeDef,
+    PutScalingPolicyRequestRequestTypeDef,
+    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
 )
 
 
-def get_structure() -> AlarmTypeDef:
+def get_value() -> AlarmTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt` & `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*


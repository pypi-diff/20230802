# Comparing `tmp/types-aiobotocore-autoscaling-plans-2.5.2.tar.gz` & `tmp/types-aiobotocore-autoscaling-plans-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-autoscaling-plans-2.5.2.tar", last modified: Sat Jul  8 01:43:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-autoscaling-plans-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
```

## Comparing `types-aiobotocore-autoscaling-plans-2.5.2.tar` & `types-aiobotocore-autoscaling-plans-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.933738 types-aiobotocore-autoscaling-plans-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-07-08 01:43:16.933738 types-aiobotocore-autoscaling-plans-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:16.933738 types-aiobotocore-autoscaling-plans-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.925738 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10272 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10255 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-07-08 01:26:14.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14019 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:13.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.933738 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-07-08 01:43:16.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-08 01:43:16.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:16.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:16.000000 types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.185648 types-aiobotocore-autoscaling-plans-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15417 2023-08-02 14:51:55.185648 types-aiobotocore-autoscaling-plans-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.185648 types-aiobotocore-autoscaling-plans-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.185648 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-08-02 14:33:41.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-08-02 14:33:41.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.185648 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15417 2023-08-02 14:51:55.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:51:55.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:55.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:51:55.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/LICENSE` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/PKG-INFO` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-autoscaling-plans
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore autoscaling-plans type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore autoscaling-plans type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-autoscaling-plans"></a>
 
 # types-aiobotocore-autoscaling-plans
 
 [![PyPI - types-aiobotocore-autoscaling-plans](https://img.shields.io/pypi/v/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-autoscaling-plans?color=blue)](https://pypistats.org/packages/types-aiobotocore-autoscaling-plans)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling-plans)](https://pepy.tech/project/types-aiobotocore-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AutoScalingPlans 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [types-aiobotocore-autoscaling-plans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/).
 
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
@@ -326,54 +325,63 @@
 )
 
 
 def check_value(value: DescribeScalingPlanResourcesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_autoscaling_plans.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_autoscaling_plans.type_defs import (
+    TagFilterOutputTypeDef,
     TagFilterTypeDef,
-    CreateScalingPlanResponseTypeDef,
+    ResponseMetadataTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
-    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    DescribeScalingPlanResourcesRequestRequestTypeDef,
-    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    DescribeScalingPlanResourcesRequestRequestTypeDef,
+    TimestampTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
-    ResponseMetadataTypeDef,
+    ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
+    CreateScalingPlanResponseTypeDef,
+    CustomizedLoadMetricSpecificationOutputTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
+    CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
+    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
+    ApplicationSourceUnionTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
+    TargetTrackingConfigurationTypeDef,
     DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
     DescribeScalingPlansRequestRequestTypeDef,
-    TargetTrackingConfigurationTypeDef,
-    ScalingInstructionTypeDef,
+    ScalingInstructionOutputTypeDef,
     ScalingPolicyTypeDef,
-    CreateScalingPlanRequestRequestTypeDef,
+    ScalingInstructionTypeDef,
     ScalingPlanTypeDef,
-    UpdateScalingPlanRequestRequestTypeDef,
     ScalingPlanResourceTypeDef,
+    ScalingInstructionUnionTypeDef,
     DescribeScalingPlansResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
+    CreateScalingPlanRequestRequestTypeDef,
+    UpdateScalingPlanRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagFilterTypeDef:
+def get_value() -> TagFilterOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/README.md` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-autoscaling-plans"></a>
 
 # types-aiobotocore-autoscaling-plans
 
 [![PyPI - types-aiobotocore-autoscaling-plans](https://img.shields.io/pypi/v/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-autoscaling-plans?color=blue)](https://pypistats.org/packages/types-aiobotocore-autoscaling-plans)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling-plans)](https://pepy.tech/project/types-aiobotocore-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AutoScalingPlans 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [types-aiobotocore-autoscaling-plans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/).
 
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
@@ -293,54 +293,63 @@
 )
 
 
 def check_value(value: DescribeScalingPlanResourcesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_autoscaling_plans.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_autoscaling_plans.type_defs import (
+    TagFilterOutputTypeDef,
     TagFilterTypeDef,
-    CreateScalingPlanResponseTypeDef,
+    ResponseMetadataTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
-    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    DescribeScalingPlanResourcesRequestRequestTypeDef,
-    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    DescribeScalingPlanResourcesRequestRequestTypeDef,
+    TimestampTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
-    ResponseMetadataTypeDef,
+    ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
+    CreateScalingPlanResponseTypeDef,
+    CustomizedLoadMetricSpecificationOutputTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
+    CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
+    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
+    ApplicationSourceUnionTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
+    TargetTrackingConfigurationTypeDef,
     DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
     DescribeScalingPlansRequestRequestTypeDef,
-    TargetTrackingConfigurationTypeDef,
-    ScalingInstructionTypeDef,
+    ScalingInstructionOutputTypeDef,
     ScalingPolicyTypeDef,
-    CreateScalingPlanRequestRequestTypeDef,
+    ScalingInstructionTypeDef,
     ScalingPlanTypeDef,
-    UpdateScalingPlanRequestRequestTypeDef,
     ScalingPlanResourceTypeDef,
+    ScalingInstructionUnionTypeDef,
     DescribeScalingPlansResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
+    CreateScalingPlanRequestRequestTypeDef,
+    UpdateScalingPlanRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagFilterTypeDef:
+def get_value() -> TagFilterOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/setup.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-autoscaling-plans",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_autoscaling_plans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with"
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
-    keywords=(
-        "aiobotocore autoscaling-plans type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore autoscaling-plans type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_autoscaling_plans": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/"
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/__init__.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/__init__.pyi` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/__main__.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AutoScalingPlans 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.AutoScalingPlans 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans\nOther"
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

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/client.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 
     session = get_session()
     async with session.create_client("autoscaling-plans") as client:
         client: AutoScalingPlansClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ForecastDataTypeType, ScalableDimensionType, ServiceNamespaceType
 from .paginator import DescribeScalingPlanResourcesPaginator, DescribeScalingPlansPaginator
 from .type_defs import (
-    ApplicationSourceTypeDef,
+    ApplicationSourceUnionTypeDef,
     CreateScalingPlanResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
-    ScalingInstructionTypeDef,
+    ScalingInstructionUnionTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -92,16 +92,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#close)
         """
 
     async def create_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
-        ApplicationSource: ApplicationSourceTypeDef,
-        ScalingInstructions: Sequence[ScalingInstructionTypeDef]
+        ApplicationSource: ApplicationSourceUnionTypeDef,
+        ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef]
     ) -> CreateScalingPlanResponseTypeDef:
         """
         Creates a scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.create_scaling_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#create_scaling_plan)
         """
@@ -132,15 +132,15 @@
         """
 
     async def describe_scaling_plans(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
+        ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeScalingPlansResponseTypeDef:
         """
         Describes one or more of your scaling plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plans)
@@ -166,31 +166,31 @@
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         ForecastDataType: ForecastDataTypeType,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str]
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef
     ) -> GetScalingPlanResourceForecastDataResponseTypeDef:
         """
         Retrieves the forecast data for a scalable resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.get_scaling_plan_resource_forecast_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#get_scaling_plan_resource_forecast_data)
         """
 
     async def update_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        ApplicationSource: ApplicationSourceTypeDef = ...,
-        ScalingInstructions: Sequence[ScalingInstructionTypeDef] = ...
+        ApplicationSource: ApplicationSourceUnionTypeDef = ...,
+        ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.update_scaling_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#update_scaling_plan)
         """
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/client.pyi` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 
     session = get_session()
     async with session.create_client("autoscaling-plans") as client:
         client: AutoScalingPlansClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ForecastDataTypeType, ScalableDimensionType, ServiceNamespaceType
 from .paginator import DescribeScalingPlanResourcesPaginator, DescribeScalingPlansPaginator
 from .type_defs import (
-    ApplicationSourceTypeDef,
+    ApplicationSourceUnionTypeDef,
     CreateScalingPlanResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
-    ScalingInstructionTypeDef,
+    ScalingInstructionUnionTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -85,16 +85,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#close)
         """
     async def create_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
-        ApplicationSource: ApplicationSourceTypeDef,
-        ScalingInstructions: Sequence[ScalingInstructionTypeDef]
+        ApplicationSource: ApplicationSourceUnionTypeDef,
+        ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef]
     ) -> CreateScalingPlanResponseTypeDef:
         """
         Creates a scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.create_scaling_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#create_scaling_plan)
         """
@@ -122,15 +122,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#describe_scaling_plan_resources)
         """
     async def describe_scaling_plans(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
+        ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeScalingPlansResponseTypeDef:
         """
         Describes one or more of your scaling plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plans)
@@ -154,30 +154,30 @@
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         ForecastDataType: ForecastDataTypeType,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str]
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef
     ) -> GetScalingPlanResourceForecastDataResponseTypeDef:
         """
         Retrieves the forecast data for a scalable resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.get_scaling_plan_resource_forecast_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#get_scaling_plan_resource_forecast_data)
         """
     async def update_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        ApplicationSource: ApplicationSourceTypeDef = ...,
-        ScalingInstructions: Sequence[ScalingInstructionTypeDef] = ...
+        ApplicationSource: ApplicationSourceUnionTypeDef = ...,
+        ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.update_scaling_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#update_scaling_plan)
         """
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/literals.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/literals.pyi` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/paginator.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 """
 from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
-    ApplicationSourceTypeDef,
+    ApplicationSourceUnionTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeScalingPlanResourcesPaginator", "DescribeScalingPlansPaginator")
 
@@ -54,15 +54,15 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScalingPlanResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlanResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/paginators/#describescalingplanresourcespaginator)
         """
 
 
@@ -73,14 +73,14 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScalingPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/paginator.pyi` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 """
 from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
-    ApplicationSourceTypeDef,
+    ApplicationSourceUnionTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeScalingPlanResourcesPaginator", "DescribeScalingPlansPaginator")
 
@@ -51,15 +51,15 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScalingPlanResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlanResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/paginators/#describescalingplanresourcespaginator)
         """
 
 class DescribeScalingPlansPaginator(AioPaginator):
@@ -69,14 +69,14 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScalingPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/type_defs.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/type_defs.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for autoscaling-plans service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_autoscaling_plans.type_defs import TagFilterTypeDef
+    from types_aiobotocore_autoscaling_plans.type_defs import TagFilterOutputTypeDef
 
-    data: TagFilterTypeDef = {...}
+    data: TagFilterOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -36,57 +36,78 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "TagFilterOutputTypeDef",
     "TagFilterTypeDef",
-    "CreateScalingPlanResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
-    "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
-    "DescribeScalingPlanResourcesRequestRequestTypeDef",
-    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "DescribeScalingPlanResourcesRequestRequestTypeDef",
+    "TimestampTypeDef",
     "PredefinedLoadMetricSpecificationTypeDef",
     "PredefinedScalingMetricSpecificationTypeDef",
-    "ResponseMetadataTypeDef",
+    "ApplicationSourceOutputTypeDef",
     "ApplicationSourceTypeDef",
+    "CreateScalingPlanResponseTypeDef",
+    "CustomizedLoadMetricSpecificationOutputTypeDef",
     "CustomizedLoadMetricSpecificationTypeDef",
+    "CustomizedScalingMetricSpecificationOutputTypeDef",
     "CustomizedScalingMetricSpecificationTypeDef",
     "GetScalingPlanResourceForecastDataResponseTypeDef",
+    "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
+    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
+    "ApplicationSourceUnionTypeDef",
+    "TargetTrackingConfigurationOutputTypeDef",
+    "TargetTrackingConfigurationTypeDef",
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     "DescribeScalingPlansRequestRequestTypeDef",
-    "TargetTrackingConfigurationTypeDef",
-    "ScalingInstructionTypeDef",
+    "ScalingInstructionOutputTypeDef",
     "ScalingPolicyTypeDef",
-    "CreateScalingPlanRequestRequestTypeDef",
+    "ScalingInstructionTypeDef",
     "ScalingPlanTypeDef",
-    "UpdateScalingPlanRequestRequestTypeDef",
     "ScalingPlanResourceTypeDef",
+    "ScalingInstructionUnionTypeDef",
     "DescribeScalingPlansResponseTypeDef",
     "DescribeScalingPlanResourcesResponseTypeDef",
+    "CreateScalingPlanRequestRequestTypeDef",
+    "UpdateScalingPlanRequestRequestTypeDef",
+)
+
+TagFilterOutputTypeDef = TypedDict(
+    "TagFilterOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+    },
+    total=False,
 )
 
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-CreateScalingPlanResponseTypeDef = TypedDict(
-    "CreateScalingPlanResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ScalingPlanVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Name": str,
@@ -107,37 +128,24 @@
     "DeleteScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
 
-_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-    },
-)
-_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
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
 
-
-class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
-    _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPlanResourcesRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
@@ -154,38 +162,15 @@
 class DescribeScalingPlanResourcesRequestRequestTypeDef(
     _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef,
     _OptionalDescribeScalingPlanResourcesRequestRequestTypeDef,
 ):
     pass
 
 
-GetScalingPlanResourceForecastDataRequestRequestTypeDef = TypedDict(
-    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-        "ServiceNamespace": ServiceNamespaceType,
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "ForecastDataType": ForecastDataTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
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
+TimestampTypeDef = Union[datetime, str]
 _RequiredPredefinedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedLoadMetricSpecificationTypeDef",
     {
         "PredefinedLoadMetricType": LoadMetricTypeType,
     },
 )
 _OptionalPredefinedLoadMetricSpecificationTypeDef = TypedDict(
@@ -222,34 +207,65 @@
 class PredefinedScalingMetricSpecificationTypeDef(
     _RequiredPredefinedScalingMetricSpecificationTypeDef,
     _OptionalPredefinedScalingMetricSpecificationTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ApplicationSourceOutputTypeDef = TypedDict(
+    "ApplicationSourceOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "CloudFormationStackARN": str,
+        "TagFilters": List[TagFilterOutputTypeDef],
     },
+    total=False,
 )
 
 ApplicationSourceTypeDef = TypedDict(
     "ApplicationSourceTypeDef",
     {
         "CloudFormationStackARN": str,
         "TagFilters": Sequence[TagFilterTypeDef],
     },
     total=False,
 )
 
+CreateScalingPlanResponseTypeDef = TypedDict(
+    "CreateScalingPlanResponseTypeDef",
+    {
+        "ScalingPlanVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredCustomizedLoadMetricSpecificationOutputTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": MetricStatisticType,
+    },
+)
+_OptionalCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalCustomizedLoadMetricSpecificationOutputTypeDef",
+    {
+        "Dimensions": List[MetricDimensionTypeDef],
+        "Unit": str,
+    },
+    total=False,
+)
+
+
+class CustomizedLoadMetricSpecificationOutputTypeDef(
+    _RequiredCustomizedLoadMetricSpecificationOutputTypeDef,
+    _OptionalCustomizedLoadMetricSpecificationOutputTypeDef,
+):
+    pass
+
+
 _RequiredCustomizedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedLoadMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -267,14 +283,39 @@
 class CustomizedLoadMetricSpecificationTypeDef(
     _RequiredCustomizedLoadMetricSpecificationTypeDef,
     _OptionalCustomizedLoadMetricSpecificationTypeDef,
 ):
     pass
 
 
+_RequiredCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredCustomizedScalingMetricSpecificationOutputTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": MetricStatisticType,
+    },
+)
+_OptionalCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalCustomizedScalingMetricSpecificationOutputTypeDef",
+    {
+        "Dimensions": List[MetricDimensionTypeDef],
+        "Unit": str,
+    },
+    total=False,
+)
+
+
+class CustomizedScalingMetricSpecificationOutputTypeDef(
+    _RequiredCustomizedScalingMetricSpecificationOutputTypeDef,
+    _OptionalCustomizedScalingMetricSpecificationOutputTypeDef,
+):
+    pass
+
+
 _RequiredCustomizedScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedScalingMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -296,41 +337,83 @@
     pass
 
 
 GetScalingPlanResourceForecastDataResponseTypeDef = TypedDict(
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     {
         "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
-    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
+_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     {
-        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[ApplicationSourceTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+)
+_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeScalingPlansRequestRequestTypeDef = TypedDict(
-    "DescribeScalingPlansRequestRequestTypeDef",
+
+class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
+    _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+    _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+):
+    pass
+
+
+GetScalingPlanResourceForecastDataRequestRequestTypeDef = TypedDict(
+    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
     {
-        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[ApplicationSourceTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
+        "ServiceNamespace": ServiceNamespaceType,
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "ForecastDataType": ForecastDataTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
+ApplicationSourceUnionTypeDef = Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
+_RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingConfigurationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingConfigurationOutputTypeDef",
+    {
+        "PredefinedScalingMetricSpecification": PredefinedScalingMetricSpecificationTypeDef,
+        "CustomizedScalingMetricSpecification": CustomizedScalingMetricSpecificationOutputTypeDef,
+        "DisableScaleIn": bool,
+        "ScaleOutCooldown": int,
+        "ScaleInCooldown": int,
+        "EstimatedInstanceWarmup": int,
     },
     total=False,
 )
 
+
+class TargetTrackingConfigurationOutputTypeDef(
+    _RequiredTargetTrackingConfigurationOutputTypeDef,
+    _OptionalTargetTrackingConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredTargetTrackingConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationTypeDef = TypedDict(
@@ -349,83 +432,130 @@
 
 class TargetTrackingConfigurationTypeDef(
     _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
 ):
     pass
 
 
-_RequiredScalingInstructionTypeDef = TypedDict(
-    "_RequiredScalingInstructionTypeDef",
+DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
+    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
+    {
+        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanVersion": int,
+        "ApplicationSources": Sequence[ApplicationSourceUnionTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScalingPlansRequestRequestTypeDef = TypedDict(
+    "DescribeScalingPlansRequestRequestTypeDef",
+    {
+        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanVersion": int,
+        "ApplicationSources": Sequence[ApplicationSourceUnionTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredScalingInstructionOutputTypeDef = TypedDict(
+    "_RequiredScalingInstructionOutputTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
         "MaxCapacity": int,
-        "TargetTrackingConfigurations": Sequence[TargetTrackingConfigurationTypeDef],
+        "TargetTrackingConfigurations": List[TargetTrackingConfigurationOutputTypeDef],
     },
 )
-_OptionalScalingInstructionTypeDef = TypedDict(
-    "_OptionalScalingInstructionTypeDef",
+_OptionalScalingInstructionOutputTypeDef = TypedDict(
+    "_OptionalScalingInstructionOutputTypeDef",
     {
         "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
-        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationTypeDef,
+        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationOutputTypeDef,
         "ScheduledActionBufferTime": int,
         "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
         "PredictiveScalingMaxCapacityBuffer": int,
         "PredictiveScalingMode": PredictiveScalingModeType,
         "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
         "DisableDynamicScaling": bool,
     },
     total=False,
 )
 
 
-class ScalingInstructionTypeDef(
-    _RequiredScalingInstructionTypeDef, _OptionalScalingInstructionTypeDef
+class ScalingInstructionOutputTypeDef(
+    _RequiredScalingInstructionOutputTypeDef, _OptionalScalingInstructionOutputTypeDef
 ):
     pass
 
 
 _RequiredScalingPolicyTypeDef = TypedDict(
     "_RequiredScalingPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyType": Literal["TargetTrackingScaling"],
     },
 )
 _OptionalScalingPolicyTypeDef = TypedDict(
     "_OptionalScalingPolicyTypeDef",
     {
-        "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
+        "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 
 class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
 
-CreateScalingPlanRequestRequestTypeDef = TypedDict(
-    "CreateScalingPlanRequestRequestTypeDef",
+_RequiredScalingInstructionTypeDef = TypedDict(
+    "_RequiredScalingInstructionTypeDef",
     {
-        "ScalingPlanName": str,
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+        "ServiceNamespace": ServiceNamespaceType,
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "MinCapacity": int,
+        "MaxCapacity": int,
+        "TargetTrackingConfigurations": Sequence[TargetTrackingConfigurationTypeDef],
     },
 )
+_OptionalScalingInstructionTypeDef = TypedDict(
+    "_OptionalScalingInstructionTypeDef",
+    {
+        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
+        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationTypeDef,
+        "ScheduledActionBufferTime": int,
+        "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
+        "PredictiveScalingMaxCapacityBuffer": int,
+        "PredictiveScalingMode": PredictiveScalingModeType,
+        "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
+        "DisableDynamicScaling": bool,
+    },
+    total=False,
+)
+
+
+class ScalingInstructionTypeDef(
+    _RequiredScalingInstructionTypeDef, _OptionalScalingInstructionTypeDef
+):
+    pass
+
 
 _RequiredScalingPlanTypeDef = TypedDict(
     "_RequiredScalingPlanTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": List[ScalingInstructionTypeDef],
+        "ApplicationSource": ApplicationSourceOutputTypeDef,
+        "ScalingInstructions": List[ScalingInstructionOutputTypeDef],
         "StatusCode": ScalingPlanStatusCodeType,
     },
 )
 _OptionalScalingPlanTypeDef = TypedDict(
     "_OptionalScalingPlanTypeDef",
     {
         "StatusMessage": str,
@@ -436,37 +566,14 @@
 )
 
 
 class ScalingPlanTypeDef(_RequiredScalingPlanTypeDef, _OptionalScalingPlanTypeDef):
     pass
 
 
-_RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateScalingPlanRequestRequestTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-    },
-)
-_OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateScalingPlanRequestRequestTypeDef",
-    {
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateScalingPlanRequestRequestTypeDef(
-    _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredScalingPlanResourceTypeDef = TypedDict(
     "_RequiredScalingPlanResourceTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
@@ -486,24 +593,56 @@
 
 class ScalingPlanResourceTypeDef(
     _RequiredScalingPlanResourceTypeDef, _OptionalScalingPlanResourceTypeDef
 ):
     pass
 
 
+ScalingInstructionUnionTypeDef = Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
 DescribeScalingPlansResponseTypeDef = TypedDict(
     "DescribeScalingPlansResponseTypeDef",
     {
         "ScalingPlans": List[ScalingPlanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScalingPlanResourcesResponseTypeDef = TypedDict(
     "DescribeScalingPlanResourcesResponseTypeDef",
     {
         "ScalingPlanResources": List[ScalingPlanResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScalingPlanRequestRequestTypeDef = TypedDict(
+    "CreateScalingPlanRequestRequestTypeDef",
+    {
+        "ScalingPlanName": str,
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": Sequence[ScalingInstructionUnionTypeDef],
+    },
+)
+
+_RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateScalingPlanRequestRequestTypeDef",
+    {
+        "ScalingPlanName": str,
+        "ScalingPlanVersion": int,
+    },
+)
+_OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateScalingPlanRequestRequestTypeDef",
+    {
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": Sequence[ScalingInstructionUnionTypeDef],
     },
+    total=False,
 )
+
+
+class UpdateScalingPlanRequestRequestTypeDef(
+    _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans/type_defs.pyi` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for autoscaling-plans service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_autoscaling_plans.type_defs import TagFilterTypeDef
+    from types_aiobotocore_autoscaling_plans.type_defs import TagFilterOutputTypeDef
 
-    data: TagFilterTypeDef = {...}
+    data: TagFilterOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -35,57 +35,78 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "TagFilterOutputTypeDef",
     "TagFilterTypeDef",
-    "CreateScalingPlanResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
-    "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
-    "DescribeScalingPlanResourcesRequestRequestTypeDef",
-    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "DescribeScalingPlanResourcesRequestRequestTypeDef",
+    "TimestampTypeDef",
     "PredefinedLoadMetricSpecificationTypeDef",
     "PredefinedScalingMetricSpecificationTypeDef",
-    "ResponseMetadataTypeDef",
+    "ApplicationSourceOutputTypeDef",
     "ApplicationSourceTypeDef",
+    "CreateScalingPlanResponseTypeDef",
+    "CustomizedLoadMetricSpecificationOutputTypeDef",
     "CustomizedLoadMetricSpecificationTypeDef",
+    "CustomizedScalingMetricSpecificationOutputTypeDef",
     "CustomizedScalingMetricSpecificationTypeDef",
     "GetScalingPlanResourceForecastDataResponseTypeDef",
+    "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
+    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
+    "ApplicationSourceUnionTypeDef",
+    "TargetTrackingConfigurationOutputTypeDef",
+    "TargetTrackingConfigurationTypeDef",
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     "DescribeScalingPlansRequestRequestTypeDef",
-    "TargetTrackingConfigurationTypeDef",
-    "ScalingInstructionTypeDef",
+    "ScalingInstructionOutputTypeDef",
     "ScalingPolicyTypeDef",
-    "CreateScalingPlanRequestRequestTypeDef",
+    "ScalingInstructionTypeDef",
     "ScalingPlanTypeDef",
-    "UpdateScalingPlanRequestRequestTypeDef",
     "ScalingPlanResourceTypeDef",
+    "ScalingInstructionUnionTypeDef",
     "DescribeScalingPlansResponseTypeDef",
     "DescribeScalingPlanResourcesResponseTypeDef",
+    "CreateScalingPlanRequestRequestTypeDef",
+    "UpdateScalingPlanRequestRequestTypeDef",
+)
+
+TagFilterOutputTypeDef = TypedDict(
+    "TagFilterOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+    },
+    total=False,
 )
 
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-CreateScalingPlanResponseTypeDef = TypedDict(
-    "CreateScalingPlanResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ScalingPlanVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Name": str,
@@ -106,35 +127,24 @@
     "DeleteScalingPlanRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
 
-_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-    },
-)
-_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
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
 
-class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
-    _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPlanResourcesRequestRequestTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
     },
 )
@@ -149,38 +159,15 @@
 
 class DescribeScalingPlanResourcesRequestRequestTypeDef(
     _RequiredDescribeScalingPlanResourcesRequestRequestTypeDef,
     _OptionalDescribeScalingPlanResourcesRequestRequestTypeDef,
 ):
     pass
 
-GetScalingPlanResourceForecastDataRequestRequestTypeDef = TypedDict(
-    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-        "ServiceNamespace": ServiceNamespaceType,
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "ForecastDataType": ForecastDataTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
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
+TimestampTypeDef = Union[datetime, str]
 _RequiredPredefinedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedLoadMetricSpecificationTypeDef",
     {
         "PredefinedLoadMetricType": LoadMetricTypeType,
     },
 )
 _OptionalPredefinedLoadMetricSpecificationTypeDef = TypedDict(
@@ -213,34 +200,63 @@
 
 class PredefinedScalingMetricSpecificationTypeDef(
     _RequiredPredefinedScalingMetricSpecificationTypeDef,
     _OptionalPredefinedScalingMetricSpecificationTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ApplicationSourceOutputTypeDef = TypedDict(
+    "ApplicationSourceOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "CloudFormationStackARN": str,
+        "TagFilters": List[TagFilterOutputTypeDef],
     },
+    total=False,
 )
 
 ApplicationSourceTypeDef = TypedDict(
     "ApplicationSourceTypeDef",
     {
         "CloudFormationStackARN": str,
         "TagFilters": Sequence[TagFilterTypeDef],
     },
     total=False,
 )
 
+CreateScalingPlanResponseTypeDef = TypedDict(
+    "CreateScalingPlanResponseTypeDef",
+    {
+        "ScalingPlanVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredCustomizedLoadMetricSpecificationOutputTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": MetricStatisticType,
+    },
+)
+_OptionalCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalCustomizedLoadMetricSpecificationOutputTypeDef",
+    {
+        "Dimensions": List[MetricDimensionTypeDef],
+        "Unit": str,
+    },
+    total=False,
+)
+
+class CustomizedLoadMetricSpecificationOutputTypeDef(
+    _RequiredCustomizedLoadMetricSpecificationOutputTypeDef,
+    _OptionalCustomizedLoadMetricSpecificationOutputTypeDef,
+):
+    pass
+
 _RequiredCustomizedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedLoadMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -256,14 +272,37 @@
 
 class CustomizedLoadMetricSpecificationTypeDef(
     _RequiredCustomizedLoadMetricSpecificationTypeDef,
     _OptionalCustomizedLoadMetricSpecificationTypeDef,
 ):
     pass
 
+_RequiredCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_RequiredCustomizedScalingMetricSpecificationOutputTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": MetricStatisticType,
+    },
+)
+_OptionalCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
+    "_OptionalCustomizedScalingMetricSpecificationOutputTypeDef",
+    {
+        "Dimensions": List[MetricDimensionTypeDef],
+        "Unit": str,
+    },
+    total=False,
+)
+
+class CustomizedScalingMetricSpecificationOutputTypeDef(
+    _RequiredCustomizedScalingMetricSpecificationOutputTypeDef,
+    _OptionalCustomizedScalingMetricSpecificationOutputTypeDef,
+):
+    pass
+
 _RequiredCustomizedScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedScalingMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -283,41 +322,79 @@
 ):
     pass
 
 GetScalingPlanResourceForecastDataResponseTypeDef = TypedDict(
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     {
         "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
-    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
+_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     {
-        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[ApplicationSourceTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+)
+_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeScalingPlansRequestRequestTypeDef = TypedDict(
-    "DescribeScalingPlansRequestRequestTypeDef",
+class DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef(
+    _RequiredDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+    _OptionalDescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+):
+    pass
+
+GetScalingPlanResourceForecastDataRequestRequestTypeDef = TypedDict(
+    "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
     {
-        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[ApplicationSourceTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
+        "ServiceNamespace": ServiceNamespaceType,
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "ForecastDataType": ForecastDataTypeType,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+
+ApplicationSourceUnionTypeDef = Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
+_RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTargetTrackingConfigurationOutputTypeDef",
+    {
+        "TargetValue": float,
+    },
+)
+_OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTargetTrackingConfigurationOutputTypeDef",
+    {
+        "PredefinedScalingMetricSpecification": PredefinedScalingMetricSpecificationTypeDef,
+        "CustomizedScalingMetricSpecification": CustomizedScalingMetricSpecificationOutputTypeDef,
+        "DisableScaleIn": bool,
+        "ScaleOutCooldown": int,
+        "ScaleInCooldown": int,
+        "EstimatedInstanceWarmup": int,
     },
     total=False,
 )
 
+class TargetTrackingConfigurationOutputTypeDef(
+    _RequiredTargetTrackingConfigurationOutputTypeDef,
+    _OptionalTargetTrackingConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredTargetTrackingConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationTypeDef = TypedDict(
@@ -334,79 +411,124 @@
 )
 
 class TargetTrackingConfigurationTypeDef(
     _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
 ):
     pass
 
-_RequiredScalingInstructionTypeDef = TypedDict(
-    "_RequiredScalingInstructionTypeDef",
+DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
+    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
+    {
+        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanVersion": int,
+        "ApplicationSources": Sequence[ApplicationSourceUnionTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeScalingPlansRequestRequestTypeDef = TypedDict(
+    "DescribeScalingPlansRequestRequestTypeDef",
+    {
+        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanVersion": int,
+        "ApplicationSources": Sequence[ApplicationSourceUnionTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+_RequiredScalingInstructionOutputTypeDef = TypedDict(
+    "_RequiredScalingInstructionOutputTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
         "MaxCapacity": int,
-        "TargetTrackingConfigurations": Sequence[TargetTrackingConfigurationTypeDef],
+        "TargetTrackingConfigurations": List[TargetTrackingConfigurationOutputTypeDef],
     },
 )
-_OptionalScalingInstructionTypeDef = TypedDict(
-    "_OptionalScalingInstructionTypeDef",
+_OptionalScalingInstructionOutputTypeDef = TypedDict(
+    "_OptionalScalingInstructionOutputTypeDef",
     {
         "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
-        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationTypeDef,
+        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationOutputTypeDef,
         "ScheduledActionBufferTime": int,
         "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
         "PredictiveScalingMaxCapacityBuffer": int,
         "PredictiveScalingMode": PredictiveScalingModeType,
         "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
         "DisableDynamicScaling": bool,
     },
     total=False,
 )
 
-class ScalingInstructionTypeDef(
-    _RequiredScalingInstructionTypeDef, _OptionalScalingInstructionTypeDef
+class ScalingInstructionOutputTypeDef(
+    _RequiredScalingInstructionOutputTypeDef, _OptionalScalingInstructionOutputTypeDef
 ):
     pass
 
 _RequiredScalingPolicyTypeDef = TypedDict(
     "_RequiredScalingPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyType": Literal["TargetTrackingScaling"],
     },
 )
 _OptionalScalingPolicyTypeDef = TypedDict(
     "_OptionalScalingPolicyTypeDef",
     {
-        "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
+        "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
     },
     total=False,
 )
 
 class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
-CreateScalingPlanRequestRequestTypeDef = TypedDict(
-    "CreateScalingPlanRequestRequestTypeDef",
+_RequiredScalingInstructionTypeDef = TypedDict(
+    "_RequiredScalingInstructionTypeDef",
     {
-        "ScalingPlanName": str,
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+        "ServiceNamespace": ServiceNamespaceType,
+        "ResourceId": str,
+        "ScalableDimension": ScalableDimensionType,
+        "MinCapacity": int,
+        "MaxCapacity": int,
+        "TargetTrackingConfigurations": Sequence[TargetTrackingConfigurationTypeDef],
     },
 )
+_OptionalScalingInstructionTypeDef = TypedDict(
+    "_OptionalScalingInstructionTypeDef",
+    {
+        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
+        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationTypeDef,
+        "ScheduledActionBufferTime": int,
+        "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
+        "PredictiveScalingMaxCapacityBuffer": int,
+        "PredictiveScalingMode": PredictiveScalingModeType,
+        "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
+        "DisableDynamicScaling": bool,
+    },
+    total=False,
+)
+
+class ScalingInstructionTypeDef(
+    _RequiredScalingInstructionTypeDef, _OptionalScalingInstructionTypeDef
+):
+    pass
 
 _RequiredScalingPlanTypeDef = TypedDict(
     "_RequiredScalingPlanTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": List[ScalingInstructionTypeDef],
+        "ApplicationSource": ApplicationSourceOutputTypeDef,
+        "ScalingInstructions": List[ScalingInstructionOutputTypeDef],
         "StatusCode": ScalingPlanStatusCodeType,
     },
 )
 _OptionalScalingPlanTypeDef = TypedDict(
     "_OptionalScalingPlanTypeDef",
     {
         "StatusMessage": str,
@@ -415,35 +537,14 @@
     },
     total=False,
 )
 
 class ScalingPlanTypeDef(_RequiredScalingPlanTypeDef, _OptionalScalingPlanTypeDef):
     pass
 
-_RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateScalingPlanRequestRequestTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-    },
-)
-_OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateScalingPlanRequestRequestTypeDef",
-    {
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
-    },
-    total=False,
-)
-
-class UpdateScalingPlanRequestRequestTypeDef(
-    _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
-):
-    pass
-
 _RequiredScalingPlanResourceTypeDef = TypedDict(
     "_RequiredScalingPlanResourceTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
@@ -461,24 +562,55 @@
 )
 
 class ScalingPlanResourceTypeDef(
     _RequiredScalingPlanResourceTypeDef, _OptionalScalingPlanResourceTypeDef
 ):
     pass
 
+ScalingInstructionUnionTypeDef = Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
 DescribeScalingPlansResponseTypeDef = TypedDict(
     "DescribeScalingPlansResponseTypeDef",
     {
         "ScalingPlans": List[ScalingPlanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeScalingPlanResourcesResponseTypeDef = TypedDict(
     "DescribeScalingPlanResourcesResponseTypeDef",
     {
         "ScalingPlanResources": List[ScalingPlanResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScalingPlanRequestRequestTypeDef = TypedDict(
+    "CreateScalingPlanRequestRequestTypeDef",
+    {
+        "ScalingPlanName": str,
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": Sequence[ScalingInstructionUnionTypeDef],
+    },
+)
+
+_RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateScalingPlanRequestRequestTypeDef",
+    {
+        "ScalingPlanName": str,
+        "ScalingPlanVersion": int,
     },
 )
+_OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateScalingPlanRequestRequestTypeDef",
+    {
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": Sequence[ScalingInstructionUnionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateScalingPlanRequestRequestTypeDef(
+    _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-autoscaling-plans
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore autoscaling-plans type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore autoscaling-plans type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-autoscaling-plans"></a>
 
 # types-aiobotocore-autoscaling-plans
 
 [![PyPI - types-aiobotocore-autoscaling-plans](https://img.shields.io/pypi/v/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-autoscaling-plans?color=blue)](https://pypistats.org/packages/types-aiobotocore-autoscaling-plans)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-autoscaling-plans)](https://pepy.tech/project/types-aiobotocore-autoscaling-plans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AutoScalingPlans 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
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
 [types-aiobotocore-autoscaling-plans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/).
 
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
@@ -326,54 +325,63 @@
 )
 
 
 def check_value(value: DescribeScalingPlanResourcesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_autoscaling_plans.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_autoscaling_plans.type_defs import (
+    TagFilterOutputTypeDef,
     TagFilterTypeDef,
-    CreateScalingPlanResponseTypeDef,
+    ResponseMetadataTypeDef,
     MetricDimensionTypeDef,
     DatapointTypeDef,
     DeleteScalingPlanRequestRequestTypeDef,
-    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    DescribeScalingPlanResourcesRequestRequestTypeDef,
-    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    DescribeScalingPlanResourcesRequestRequestTypeDef,
+    TimestampTypeDef,
     PredefinedLoadMetricSpecificationTypeDef,
     PredefinedScalingMetricSpecificationTypeDef,
-    ResponseMetadataTypeDef,
+    ApplicationSourceOutputTypeDef,
     ApplicationSourceTypeDef,
+    CreateScalingPlanResponseTypeDef,
+    CustomizedLoadMetricSpecificationOutputTypeDef,
     CustomizedLoadMetricSpecificationTypeDef,
+    CustomizedScalingMetricSpecificationOutputTypeDef,
     CustomizedScalingMetricSpecificationTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
+    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
+    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
+    ApplicationSourceUnionTypeDef,
+    TargetTrackingConfigurationOutputTypeDef,
+    TargetTrackingConfigurationTypeDef,
     DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
     DescribeScalingPlansRequestRequestTypeDef,
-    TargetTrackingConfigurationTypeDef,
-    ScalingInstructionTypeDef,
+    ScalingInstructionOutputTypeDef,
     ScalingPolicyTypeDef,
-    CreateScalingPlanRequestRequestTypeDef,
+    ScalingInstructionTypeDef,
     ScalingPlanTypeDef,
-    UpdateScalingPlanRequestRequestTypeDef,
     ScalingPlanResourceTypeDef,
+    ScalingInstructionUnionTypeDef,
     DescribeScalingPlansResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
+    CreateScalingPlanRequestRequestTypeDef,
+    UpdateScalingPlanRequestRequestTypeDef,
 )
 
 
-def get_structure() -> TagFilterTypeDef:
+def get_value() -> TagFilterOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt` & `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt`

 * *Files identical despite different names*


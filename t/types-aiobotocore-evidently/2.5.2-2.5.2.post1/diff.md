# Comparing `tmp/types-aiobotocore-evidently-2.5.2.tar.gz` & `tmp/types-aiobotocore-evidently-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-evidently-2.5.2.tar", last modified: Sat Jul  8 01:43:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-evidently-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:17 2023, max compression
```

## Comparing `types-aiobotocore-evidently-2.5.2.tar` & `types-aiobotocore-evidently-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.682133 types-aiobotocore-evidently-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18698 2023-07-08 01:43:37.678132 types-aiobotocore-evidently-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:37.682133 types-aiobotocore-evidently-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.674132 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32420 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45547 2023-07-08 01:30:50.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45462 2023-07-08 01:30:49.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:48.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:37.678132 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18698 2023-07-08 01:43:37.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-08 01:43:37.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:37.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:37.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:37.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:37.000000 types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:17.153588 types-aiobotocore-evidently-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-08-02 14:52:17.153588 types-aiobotocore-evidently-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:17.153588 types-aiobotocore-evidently-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:17.153588 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-08-02 14:38:40.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-08-02 14:38:40.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45742 2023-08-02 14:38:41.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45657 2023-08-02 14:38:40.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:17.153588 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-08-02 14:52:16.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:17.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:16.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-evidently-2.5.2/LICENSE` & `types-aiobotocore-evidently-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2/PKG-INFO` & `types-aiobotocore-evidently-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-evidently
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudWatchEvidently 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudWatchEvidently 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore evidently type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore evidently type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-evidently"></a>
 
 # types-aiobotocore-evidently
 
 [![PyPI - types-aiobotocore-evidently](https://img.shields.io/pypi/v/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-evidently?color=blue)](https://pypistats.org/packages/types-aiobotocore-evidently)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-evidently)](https://pepy.tech/project/types-aiobotocore-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudWatchEvidently 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [types-aiobotocore-evidently docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/).
 
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
@@ -341,24 +340,25 @@
 )
 
 
 def check_value(value: ChangeDirectionEnumType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_evidently.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_evidently.type_defs import (
     EvaluationRequestTypeDef,
+    ResponseMetadataTypeDef,
     CloudWatchLogsDestinationConfigTypeDef,
     CloudWatchLogsDestinationTypeDef,
     OnlineAbConfigTypeDef,
     TreatmentConfigTypeDef,
     LaunchGroupConfigTypeDef,
     ProjectAppConfigResourceConfigTypeDef,
     CreateSegmentRequestRequestTypeDef,
@@ -367,77 +367,77 @@
     DeleteFeatureRequestRequestTypeDef,
     DeleteLaunchRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteSegmentRequestRequestTypeDef,
     EvaluateFeatureRequestRequestTypeDef,
     VariableValueTypeDef,
     EvaluationRuleTypeDef,
-    EventTypeDef,
+    TimestampTypeDef,
     ExperimentExecutionTypeDef,
     ExperimentReportTypeDef,
     ExperimentResultsDataTypeDef,
     ExperimentScheduleTypeDef,
     OnlineAbDefinitionTypeDef,
     TreatmentTypeDef,
     GetExperimentRequestRequestTypeDef,
-    GetExperimentResultsRequestRequestTypeDef,
     GetFeatureRequestRequestTypeDef,
     GetLaunchRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     LaunchExecutionTypeDef,
     LaunchGroupTypeDef,
-    ListExperimentsRequestListExperimentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListExperimentsRequestRequestTypeDef,
-    ListFeaturesRequestListFeaturesPaginateTypeDef,
     ListFeaturesRequestRequestTypeDef,
-    ListLaunchesRequestListLaunchesPaginateTypeDef,
     ListLaunchesRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
     ListSegmentReferencesRequestRequestTypeDef,
     RefResourceTypeDef,
-    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListSegmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MetricDefinitionConfigTypeDef,
     MetricDefinitionTypeDef,
-    PaginatorConfigTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
-    ResponseMetadataTypeDef,
     SegmentOverrideTypeDef,
-    StartExperimentRequestRequestTypeDef,
-    StartExperimentResponseTypeDef,
+    SegmentOverrideOutputTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
-    StopExperimentResponseTypeDef,
     StopLaunchRequestRequestTypeDef,
-    StopLaunchResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
-    TestSegmentPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartExperimentResponseTypeDef,
+    StopExperimentResponseTypeDef,
+    StopLaunchResponseTypeDef,
+    TestSegmentPatternResponseTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
     VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
-    PutProjectEventsRequestRequestTypeDef,
+    EventTypeDef,
+    GetExperimentResultsRequestRequestTypeDef,
+    StartExperimentRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
+    ListExperimentsRequestListExperimentsPaginateTypeDef,
+    ListFeaturesRequestListFeaturesPaginateTypeDef,
+    ListLaunchesRequestListLaunchesPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListProjectsResponseTypeDef,
     ListSegmentReferencesResponseTypeDef,
     MetricGoalConfigTypeDef,
     MetricMonitorConfigTypeDef,
     MetricGoalTypeDef,
     MetricMonitorTypeDef,
     ProjectDataDeliveryConfigTypeDef,
@@ -447,14 +447,15 @@
     ScheduledSplitConfigTypeDef,
     ScheduledSplitTypeDef,
     BatchEvaluateFeatureResponseTypeDef,
     CreateFeatureRequestRequestTypeDef,
     UpdateFeatureRequestRequestTypeDef,
     FeatureTypeDef,
     ListFeaturesResponseTypeDef,
+    PutProjectEventsRequestRequestTypeDef,
     CreateExperimentRequestRequestTypeDef,
     UpdateExperimentRequestRequestTypeDef,
     ExperimentTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     ScheduledSplitsLaunchDefinitionTypeDef,
@@ -476,15 +477,15 @@
     GetLaunchResponseTypeDef,
     ListLaunchesResponseTypeDef,
     StartLaunchResponseTypeDef,
     UpdateLaunchResponseTypeDef,
 )
 
 
-def get_structure() -> EvaluationRequestTypeDef:
+def get_value() -> EvaluationRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-evidently-2.5.2/README.md` & `types-aiobotocore-evidently-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-evidently"></a>
 
 # types-aiobotocore-evidently
 
 [![PyPI - types-aiobotocore-evidently](https://img.shields.io/pypi/v/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-evidently?color=blue)](https://pypistats.org/packages/types-aiobotocore-evidently)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-evidently)](https://pepy.tech/project/types-aiobotocore-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudWatchEvidently 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [types-aiobotocore-evidently docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/).
 
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
@@ -308,24 +308,25 @@
 )
 
 
 def check_value(value: ChangeDirectionEnumType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_evidently.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_evidently.type_defs import (
     EvaluationRequestTypeDef,
+    ResponseMetadataTypeDef,
     CloudWatchLogsDestinationConfigTypeDef,
     CloudWatchLogsDestinationTypeDef,
     OnlineAbConfigTypeDef,
     TreatmentConfigTypeDef,
     LaunchGroupConfigTypeDef,
     ProjectAppConfigResourceConfigTypeDef,
     CreateSegmentRequestRequestTypeDef,
@@ -334,77 +335,77 @@
     DeleteFeatureRequestRequestTypeDef,
     DeleteLaunchRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteSegmentRequestRequestTypeDef,
     EvaluateFeatureRequestRequestTypeDef,
     VariableValueTypeDef,
     EvaluationRuleTypeDef,
-    EventTypeDef,
+    TimestampTypeDef,
     ExperimentExecutionTypeDef,
     ExperimentReportTypeDef,
     ExperimentResultsDataTypeDef,
     ExperimentScheduleTypeDef,
     OnlineAbDefinitionTypeDef,
     TreatmentTypeDef,
     GetExperimentRequestRequestTypeDef,
-    GetExperimentResultsRequestRequestTypeDef,
     GetFeatureRequestRequestTypeDef,
     GetLaunchRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     LaunchExecutionTypeDef,
     LaunchGroupTypeDef,
-    ListExperimentsRequestListExperimentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListExperimentsRequestRequestTypeDef,
-    ListFeaturesRequestListFeaturesPaginateTypeDef,
     ListFeaturesRequestRequestTypeDef,
-    ListLaunchesRequestListLaunchesPaginateTypeDef,
     ListLaunchesRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
     ListSegmentReferencesRequestRequestTypeDef,
     RefResourceTypeDef,
-    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListSegmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MetricDefinitionConfigTypeDef,
     MetricDefinitionTypeDef,
-    PaginatorConfigTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
-    ResponseMetadataTypeDef,
     SegmentOverrideTypeDef,
-    StartExperimentRequestRequestTypeDef,
-    StartExperimentResponseTypeDef,
+    SegmentOverrideOutputTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
-    StopExperimentResponseTypeDef,
     StopLaunchRequestRequestTypeDef,
-    StopLaunchResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
-    TestSegmentPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartExperimentResponseTypeDef,
+    StopExperimentResponseTypeDef,
+    StopLaunchResponseTypeDef,
+    TestSegmentPatternResponseTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
     VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
-    PutProjectEventsRequestRequestTypeDef,
+    EventTypeDef,
+    GetExperimentResultsRequestRequestTypeDef,
+    StartExperimentRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
+    ListExperimentsRequestListExperimentsPaginateTypeDef,
+    ListFeaturesRequestListFeaturesPaginateTypeDef,
+    ListLaunchesRequestListLaunchesPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListProjectsResponseTypeDef,
     ListSegmentReferencesResponseTypeDef,
     MetricGoalConfigTypeDef,
     MetricMonitorConfigTypeDef,
     MetricGoalTypeDef,
     MetricMonitorTypeDef,
     ProjectDataDeliveryConfigTypeDef,
@@ -414,14 +415,15 @@
     ScheduledSplitConfigTypeDef,
     ScheduledSplitTypeDef,
     BatchEvaluateFeatureResponseTypeDef,
     CreateFeatureRequestRequestTypeDef,
     UpdateFeatureRequestRequestTypeDef,
     FeatureTypeDef,
     ListFeaturesResponseTypeDef,
+    PutProjectEventsRequestRequestTypeDef,
     CreateExperimentRequestRequestTypeDef,
     UpdateExperimentRequestRequestTypeDef,
     ExperimentTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     ScheduledSplitsLaunchDefinitionTypeDef,
@@ -443,15 +445,15 @@
     GetLaunchResponseTypeDef,
     ListLaunchesResponseTypeDef,
     StartLaunchResponseTypeDef,
     UpdateLaunchResponseTypeDef,
 )
 
 
-def get_structure() -> EvaluationRequestTypeDef:
+def get_value() -> EvaluationRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-evidently-2.5.2/setup.py` & `types-aiobotocore-evidently-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-evidently",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_evidently"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudWatchEvidently 2.5.2 service generated with"
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
-    keywords="aiobotocore evidently type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore evidently type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_evidently": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/"
```

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/__init__.py` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/__init__.pyi` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/__main__.py` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CloudWatchEvidently 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently\nOther"
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

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/client.py` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("evidently") as client:
         client: CloudWatchEvidentlyClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     ExperimentResultRequestTypeType,
     ExperimentStatusType,
@@ -72,14 +71,15 @@
     S3DestinationConfigTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     StartExperimentResponseTypeDef,
     StartLaunchResponseTypeDef,
     StopExperimentResponseTypeDef,
     StopLaunchResponseTypeDef,
     TestSegmentPatternResponseTypeDef,
+    TimestampTypeDef,
     TreatmentConfigTypeDef,
     UpdateExperimentResponseTypeDef,
     UpdateFeatureResponseTypeDef,
     UpdateLaunchResponseTypeDef,
     UpdateProjectDataDeliveryResponseTypeDef,
     UpdateProjectResponseTypeDef,
     VariationConfigTypeDef,
@@ -321,19 +321,19 @@
         self,
         *,
         experiment: str,
         metricNames: Sequence[str],
         project: str,
         treatmentNames: Sequence[str],
         baseStat: Literal["Mean"] = ...,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         period: int = ...,
         reportNames: Sequence[Literal["BayesianInference"]] = ...,
         resultStats: Sequence[ExperimentResultRequestTypeType] = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> GetExperimentResultsResponseTypeDef:
         """
         Retrieves the results of a running or completed experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.get_experiment_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#get_experiment_results)
         """
@@ -466,15 +466,15 @@
         Sends performance events to Evidently.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.put_project_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#put_project_events)
         """
 
     async def start_experiment(
-        self, *, analysisCompleteTime: Union[datetime, str], experiment: str, project: str
+        self, *, analysisCompleteTime: TimestampTypeDef, experiment: str, project: str
     ) -> StartExperimentResponseTypeDef:
         """
         Starts an existing experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.start_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#start_experiment)
         """
```

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/client.pyi` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("evidently") as client:
         client: CloudWatchEvidentlyClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     ExperimentResultRequestTypeType,
     ExperimentStatusType,
@@ -72,14 +71,15 @@
     S3DestinationConfigTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     StartExperimentResponseTypeDef,
     StartLaunchResponseTypeDef,
     StopExperimentResponseTypeDef,
     StopLaunchResponseTypeDef,
     TestSegmentPatternResponseTypeDef,
+    TimestampTypeDef,
     TreatmentConfigTypeDef,
     UpdateExperimentResponseTypeDef,
     UpdateFeatureResponseTypeDef,
     UpdateLaunchResponseTypeDef,
     UpdateProjectDataDeliveryResponseTypeDef,
     UpdateProjectResponseTypeDef,
     VariationConfigTypeDef,
@@ -300,19 +300,19 @@
         self,
         *,
         experiment: str,
         metricNames: Sequence[str],
         project: str,
         treatmentNames: Sequence[str],
         baseStat: Literal["Mean"] = ...,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         period: int = ...,
         reportNames: Sequence[Literal["BayesianInference"]] = ...,
         resultStats: Sequence[ExperimentResultRequestTypeType] = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> GetExperimentResultsResponseTypeDef:
         """
         Retrieves the results of a running or completed experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.get_experiment_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#get_experiment_results)
         """
@@ -432,15 +432,15 @@
         """
         Sends performance events to Evidently.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.put_project_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#put_project_events)
         """
     async def start_experiment(
-        self, *, analysisCompleteTime: Union[datetime, str], experiment: str, project: str
+        self, *, analysisCompleteTime: TimestampTypeDef, experiment: str, project: str
     ) -> StartExperimentResponseTypeDef:
         """
         Starts an existing experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Client.start_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/client/#start_experiment)
         """
```

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/literals.py` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/literals.pyi` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/paginator.py` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,30 +73,30 @@
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: ExperimentStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExperimentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListExperiments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listexperimentspaginator)
         """
 
 
 class ListFeaturesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listfeaturespaginator)
     """
 
     def paginate(
-        self, *, project: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, project: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFeaturesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listfeaturespaginator)
         """
 
 
@@ -107,30 +107,30 @@
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: LaunchStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLaunchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListLaunches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listlaunchespaginator)
         """
 
 
 class ListProjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listprojectspaginator)
         """
 
 
@@ -141,28 +141,28 @@
     """
 
     def paginate(
         self,
         *,
         segment: str,
         type: SegmentReferenceResourceTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSegmentReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegmentReferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listsegmentreferencespaginator)
         """
 
 
 class ListSegmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listsegmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSegmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listsegmentspaginator)
         """
```

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/paginator.pyi` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -70,29 +70,29 @@
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: ExperimentStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExperimentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListExperiments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listexperimentspaginator)
         """
 
 class ListFeaturesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listfeaturespaginator)
     """
 
     def paginate(
-        self, *, project: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, project: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFeaturesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListFeatures.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listfeaturespaginator)
         """
 
 class ListLaunchesPaginator(AioPaginator):
@@ -102,29 +102,29 @@
     """
 
     def paginate(
         self,
         *,
         project: str,
         status: LaunchStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLaunchesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListLaunches.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listlaunchespaginator)
         """
 
 class ListProjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listprojectspaginator)
         """
 
 class ListSegmentReferencesPaginator(AioPaginator):
@@ -134,27 +134,27 @@
     """
 
     def paginate(
         self,
         *,
         segment: str,
         type: SegmentReferenceResourceTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSegmentReferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegmentReferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listsegmentreferencespaginator)
         """
 
 class ListSegmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listsegmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSegmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently.Paginator.ListSegments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/paginators/#listsegmentspaginator)
         """
```

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/type_defs.py` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_evidently.type_defs import EvaluationRequestTypeDef
 
-    data: EvaluationRequestTypeDef = {...}
+    data: EvaluationRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -39,14 +39,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "EvaluationRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CloudWatchLogsDestinationConfigTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "OnlineAbConfigTypeDef",
     "TreatmentConfigTypeDef",
     "LaunchGroupConfigTypeDef",
     "ProjectAppConfigResourceConfigTypeDef",
     "CreateSegmentRequestRequestTypeDef",
@@ -55,77 +56,77 @@
     "DeleteFeatureRequestRequestTypeDef",
     "DeleteLaunchRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteSegmentRequestRequestTypeDef",
     "EvaluateFeatureRequestRequestTypeDef",
     "VariableValueTypeDef",
     "EvaluationRuleTypeDef",
-    "EventTypeDef",
+    "TimestampTypeDef",
     "ExperimentExecutionTypeDef",
     "ExperimentReportTypeDef",
     "ExperimentResultsDataTypeDef",
     "ExperimentScheduleTypeDef",
     "OnlineAbDefinitionTypeDef",
     "TreatmentTypeDef",
     "GetExperimentRequestRequestTypeDef",
-    "GetExperimentResultsRequestRequestTypeDef",
     "GetFeatureRequestRequestTypeDef",
     "GetLaunchRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSegmentRequestRequestTypeDef",
     "LaunchExecutionTypeDef",
     "LaunchGroupTypeDef",
-    "ListExperimentsRequestListExperimentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListExperimentsRequestRequestTypeDef",
-    "ListFeaturesRequestListFeaturesPaginateTypeDef",
     "ListFeaturesRequestRequestTypeDef",
-    "ListLaunchesRequestListLaunchesPaginateTypeDef",
     "ListLaunchesRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
-    "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
     "ListSegmentReferencesRequestRequestTypeDef",
     "RefResourceTypeDef",
-    "ListSegmentsRequestListSegmentsPaginateTypeDef",
     "ListSegmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MetricDefinitionConfigTypeDef",
     "MetricDefinitionTypeDef",
-    "PaginatorConfigTypeDef",
     "ProjectAppConfigResourceTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "PutProjectEventsResultEntryTypeDef",
-    "ResponseMetadataTypeDef",
     "SegmentOverrideTypeDef",
-    "StartExperimentRequestRequestTypeDef",
-    "StartExperimentResponseTypeDef",
+    "SegmentOverrideOutputTypeDef",
     "StartLaunchRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
-    "StopExperimentResponseTypeDef",
     "StopLaunchRequestRequestTypeDef",
-    "StopLaunchResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSegmentPatternRequestRequestTypeDef",
-    "TestSegmentPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchEvaluateFeatureRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartExperimentResponseTypeDef",
+    "StopExperimentResponseTypeDef",
+    "StopLaunchResponseTypeDef",
+    "TestSegmentPatternResponseTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "CreateSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "ListSegmentsResponseTypeDef",
     "EvaluateFeatureResponseTypeDef",
     "EvaluationResultTypeDef",
     "VariationConfigTypeDef",
     "VariationTypeDef",
     "FeatureSummaryTypeDef",
-    "PutProjectEventsRequestRequestTypeDef",
+    "EventTypeDef",
+    "GetExperimentResultsRequestRequestTypeDef",
+    "StartExperimentRequestRequestTypeDef",
     "GetExperimentResultsResponseTypeDef",
+    "ListExperimentsRequestListExperimentsPaginateTypeDef",
+    "ListFeaturesRequestListFeaturesPaginateTypeDef",
+    "ListLaunchesRequestListLaunchesPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    "ListSegmentsRequestListSegmentsPaginateTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSegmentReferencesResponseTypeDef",
     "MetricGoalConfigTypeDef",
     "MetricMonitorConfigTypeDef",
     "MetricGoalTypeDef",
     "MetricMonitorTypeDef",
     "ProjectDataDeliveryConfigTypeDef",
@@ -135,14 +136,15 @@
     "ScheduledSplitConfigTypeDef",
     "ScheduledSplitTypeDef",
     "BatchEvaluateFeatureResponseTypeDef",
     "CreateFeatureRequestRequestTypeDef",
     "UpdateFeatureRequestRequestTypeDef",
     "FeatureTypeDef",
     "ListFeaturesResponseTypeDef",
+    "PutProjectEventsRequestRequestTypeDef",
     "CreateExperimentRequestRequestTypeDef",
     "UpdateExperimentRequestRequestTypeDef",
     "ExperimentTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectTypeDef",
     "ScheduledSplitsLaunchConfigTypeDef",
     "ScheduledSplitsLaunchDefinitionTypeDef",
@@ -185,14 +187,25 @@
 
 class EvaluationRequestTypeDef(
     _RequiredEvaluationRequestTypeDef, _OptionalEvaluationRequestTypeDef
 ):
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
 CloudWatchLogsDestinationConfigTypeDef = TypedDict(
     "CloudWatchLogsDestinationConfigTypeDef",
     {
         "logGroup": str,
     },
     total=False,
 )
@@ -403,23 +416,15 @@
 )
 
 
 class EvaluationRuleTypeDef(_RequiredEvaluationRuleTypeDef, _OptionalEvaluationRuleTypeDef):
     pass
 
 
-EventTypeDef = TypedDict(
-    "EventTypeDef",
-    {
-        "data": str,
-        "timestamp": Union[datetime, str],
-        "type": EventTypeType,
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ExperimentExecutionTypeDef = TypedDict(
     "ExperimentExecutionTypeDef",
     {
         "endedTime": datetime,
         "startedTime": datetime,
     },
     total=False,
@@ -488,44 +493,14 @@
     "GetExperimentRequestRequestTypeDef",
     {
         "experiment": str,
         "project": str,
     },
 )
 
-_RequiredGetExperimentResultsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetExperimentResultsRequestRequestTypeDef",
-    {
-        "experiment": str,
-        "metricNames": Sequence[str],
-        "project": str,
-        "treatmentNames": Sequence[str],
-    },
-)
-_OptionalGetExperimentResultsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetExperimentResultsRequestRequestTypeDef",
-    {
-        "baseStat": Literal["Mean"],
-        "endTime": Union[datetime, str],
-        "period": int,
-        "reportNames": Sequence[Literal["BayesianInference"]],
-        "resultStats": Sequence[ExperimentResultRequestTypeType],
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class GetExperimentResultsRequestRequestTypeDef(
-    _RequiredGetExperimentResultsRequestRequestTypeDef,
-    _OptionalGetExperimentResultsRequestRequestTypeDef,
-):
-    pass
-
-
 GetFeatureRequestRequestTypeDef = TypedDict(
     "GetFeatureRequestRequestTypeDef",
     {
         "feature": str,
         "project": str,
     },
 )
@@ -577,37 +552,24 @@
 )
 
 
 class LaunchGroupTypeDef(_RequiredLaunchGroupTypeDef, _OptionalLaunchGroupTypeDef):
     pass
 
 
-_RequiredListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
-    "_RequiredListExperimentsRequestListExperimentsPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
-    "_OptionalListExperimentsRequestListExperimentsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": ExperimentStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListExperimentsRequestListExperimentsPaginateTypeDef(
-    _RequiredListExperimentsRequestListExperimentsPaginateTypeDef,
-    _OptionalListExperimentsRequestListExperimentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListExperimentsRequestRequestTypeDef = TypedDict(
     "_RequiredListExperimentsRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListExperimentsRequestRequestTypeDef = TypedDict(
@@ -623,36 +585,14 @@
 
 class ListExperimentsRequestRequestTypeDef(
     _RequiredListExperimentsRequestRequestTypeDef, _OptionalListExperimentsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
-    "_RequiredListFeaturesRequestListFeaturesPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
-    "_OptionalListFeaturesRequestListFeaturesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFeaturesRequestListFeaturesPaginateTypeDef(
-    _RequiredListFeaturesRequestListFeaturesPaginateTypeDef,
-    _OptionalListFeaturesRequestListFeaturesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFeaturesRequestRequestTypeDef = TypedDict(
     "_RequiredListFeaturesRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListFeaturesRequestRequestTypeDef = TypedDict(
@@ -667,37 +607,14 @@
 
 class ListFeaturesRequestRequestTypeDef(
     _RequiredListFeaturesRequestRequestTypeDef, _OptionalListFeaturesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchesRequestListLaunchesPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchesRequestListLaunchesPaginateTypeDef",
-    {
-        "status": LaunchStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListLaunchesRequestListLaunchesPaginateTypeDef(
-    _RequiredListLaunchesRequestListLaunchesPaginateTypeDef,
-    _OptionalListLaunchesRequestListLaunchesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListLaunchesRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchesRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListLaunchesRequestRequestTypeDef = TypedDict(
@@ -713,22 +630,14 @@
 
 class ListLaunchesRequestRequestTypeDef(
     _RequiredListLaunchesRequestRequestTypeDef, _OptionalListLaunchesRequestRequestTypeDef
 ):
     pass
 
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -759,37 +668,14 @@
 )
 
 
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
 
-_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
-    "_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    {
-        "segment": str,
-        "type": SegmentReferenceResourceTypeType,
-    },
-)
-_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
-    "_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(
-    _RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-    _OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSegmentReferencesRequestRequestTypeDef = TypedDict(
     "_RequiredListSegmentReferencesRequestRequestTypeDef",
     {
         "segment": str,
         "type": SegmentReferenceResourceTypeType,
     },
 )
@@ -830,22 +716,14 @@
 )
 
 
 class RefResourceTypeDef(_RequiredRefResourceTypeDef, _OptionalRefResourceTypeDef):
     pass
 
 
-ListSegmentsRequestListSegmentsPaginateTypeDef = TypedDict(
-    "ListSegmentsRequestListSegmentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSegmentsRequestRequestTypeDef = TypedDict(
     "ListSegmentsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -854,22 +732,14 @@
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
 _RequiredMetricDefinitionConfigTypeDef = TypedDict(
     "_RequiredMetricDefinitionConfigTypeDef",
     {
         "entityIdKey": str,
         "name": str,
         "valueKey": str,
     },
@@ -898,24 +768,14 @@
         "name": str,
         "unitLabel": str,
         "valueKey": str,
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
 ProjectAppConfigResourceTypeDef = TypedDict(
     "ProjectAppConfigResourceTypeDef",
     {
         "applicationId": str,
         "configurationProfileId": str,
         "environmentId": str,
     },
@@ -945,48 +805,29 @@
         "errorCode": str,
         "errorMessage": str,
         "eventId": str,
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
 SegmentOverrideTypeDef = TypedDict(
     "SegmentOverrideTypeDef",
     {
         "evaluationOrder": int,
         "segment": str,
         "weights": Mapping[str, int],
     },
 )
 
-StartExperimentRequestRequestTypeDef = TypedDict(
-    "StartExperimentRequestRequestTypeDef",
-    {
-        "analysisCompleteTime": Union[datetime, str],
-        "experiment": str,
-        "project": str,
-    },
-)
-
-StartExperimentResponseTypeDef = TypedDict(
-    "StartExperimentResponseTypeDef",
+SegmentOverrideOutputTypeDef = TypedDict(
+    "SegmentOverrideOutputTypeDef",
     {
-        "startedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "evaluationOrder": int,
+        "segment": str,
+        "weights": Dict[str, int],
     },
 )
 
 StartLaunchRequestRequestTypeDef = TypedDict(
     "StartLaunchRequestRequestTypeDef",
     {
         "launch": str,
@@ -1013,22 +854,14 @@
 
 class StopExperimentRequestRequestTypeDef(
     _RequiredStopExperimentRequestRequestTypeDef, _OptionalStopExperimentRequestRequestTypeDef
 ):
     pass
 
 
-StopExperimentResponseTypeDef = TypedDict(
-    "StopExperimentResponseTypeDef",
-    {
-        "endedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopLaunchRequestRequestTypeDef = TypedDict(
     "_RequiredStopLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -1044,22 +877,14 @@
 
 class StopLaunchRequestRequestTypeDef(
     _RequiredStopLaunchRequestRequestTypeDef, _OptionalStopLaunchRequestRequestTypeDef
 ):
     pass
 
 
-StopLaunchResponseTypeDef = TypedDict(
-    "StopLaunchResponseTypeDef",
-    {
-        "endedTime": datetime,
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
@@ -1068,22 +893,14 @@
     "TestSegmentPatternRequestRequestTypeDef",
     {
         "pattern": str,
         "payload": str,
     },
 )
 
-TestSegmentPatternResponseTypeDef = TypedDict(
-    "TestSegmentPatternResponseTypeDef",
-    {
-        "match": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1092,14 +909,54 @@
     "BatchEvaluateFeatureRequestRequestTypeDef",
     {
         "project": str,
         "requests": Sequence[EvaluationRequestTypeDef],
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartExperimentResponseTypeDef = TypedDict(
+    "StartExperimentResponseTypeDef",
+    {
+        "startedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopExperimentResponseTypeDef = TypedDict(
+    "StopExperimentResponseTypeDef",
+    {
+        "endedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopLaunchResponseTypeDef = TypedDict(
+    "StopLaunchResponseTypeDef",
+    {
+        "endedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestSegmentPatternResponseTypeDef = TypedDict(
+    "TestSegmentPatternResponseTypeDef",
+    {
+        "match": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -1118,43 +975,43 @@
     pass
 
 
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "segment": SegmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "segment": SegmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSegmentsResponseTypeDef = TypedDict(
     "ListSegmentsResponseTypeDef",
     {
         "nextToken": str,
         "segments": List[SegmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EvaluateFeatureResponseTypeDef = TypedDict(
     "EvaluateFeatureResponseTypeDef",
     {
         "details": str,
         "reason": str,
         "value": VariableValueTypeDef,
         "variation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEvaluationResultTypeDef = TypedDict(
     "_RequiredEvaluationResultTypeDef",
     {
         "entityId": str,
@@ -1218,48 +1075,195 @@
 )
 
 
 class FeatureSummaryTypeDef(_RequiredFeatureSummaryTypeDef, _OptionalFeatureSummaryTypeDef):
     pass
 
 
-PutProjectEventsRequestRequestTypeDef = TypedDict(
-    "PutProjectEventsRequestRequestTypeDef",
+EventTypeDef = TypedDict(
+    "EventTypeDef",
     {
-        "events": Sequence[EventTypeDef],
+        "data": str,
+        "timestamp": TimestampTypeDef,
+        "type": EventTypeType,
+    },
+)
+
+_RequiredGetExperimentResultsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetExperimentResultsRequestRequestTypeDef",
+    {
+        "experiment": str,
+        "metricNames": Sequence[str],
+        "project": str,
+        "treatmentNames": Sequence[str],
+    },
+)
+_OptionalGetExperimentResultsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetExperimentResultsRequestRequestTypeDef",
+    {
+        "baseStat": Literal["Mean"],
+        "endTime": TimestampTypeDef,
+        "period": int,
+        "reportNames": Sequence[Literal["BayesianInference"]],
+        "resultStats": Sequence[ExperimentResultRequestTypeType],
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class GetExperimentResultsRequestRequestTypeDef(
+    _RequiredGetExperimentResultsRequestRequestTypeDef,
+    _OptionalGetExperimentResultsRequestRequestTypeDef,
+):
+    pass
+
+
+StartExperimentRequestRequestTypeDef = TypedDict(
+    "StartExperimentRequestRequestTypeDef",
+    {
+        "analysisCompleteTime": TimestampTypeDef,
+        "experiment": str,
         "project": str,
     },
 )
 
 GetExperimentResultsResponseTypeDef = TypedDict(
     "GetExperimentResultsResponseTypeDef",
     {
         "details": str,
         "reports": List[ExperimentReportTypeDef],
         "resultsData": List[ExperimentResultsDataTypeDef],
         "timestamps": List[datetime],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
+    "_RequiredListExperimentsRequestListExperimentsPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
+    "_OptionalListExperimentsRequestListExperimentsPaginateTypeDef",
+    {
+        "status": ExperimentStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListExperimentsRequestListExperimentsPaginateTypeDef(
+    _RequiredListExperimentsRequestListExperimentsPaginateTypeDef,
+    _OptionalListExperimentsRequestListExperimentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
+    "_RequiredListFeaturesRequestListFeaturesPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
+    "_OptionalListFeaturesRequestListFeaturesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFeaturesRequestListFeaturesPaginateTypeDef(
+    _RequiredListFeaturesRequestListFeaturesPaginateTypeDef,
+    _OptionalListFeaturesRequestListFeaturesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchesRequestListLaunchesPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchesRequestListLaunchesPaginateTypeDef",
+    {
+        "status": LaunchStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListLaunchesRequestListLaunchesPaginateTypeDef(
+    _RequiredListLaunchesRequestListLaunchesPaginateTypeDef,
+    _OptionalListLaunchesRequestListLaunchesPaginateTypeDef,
+):
+    pass
+
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
+    "_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    {
+        "segment": str,
+        "type": SegmentReferenceResourceTypeType,
+    },
+)
+_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
+    "_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(
+    _RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+    _OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+):
+    pass
+
+
+ListSegmentsRequestListSegmentsPaginateTypeDef = TypedDict(
+    "ListSegmentsRequestListSegmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "projects": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSegmentReferencesResponseTypeDef = TypedDict(
     "ListSegmentReferencesResponseTypeDef",
     {
         "nextToken": str,
         "referencedBy": List[RefResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMetricGoalConfigTypeDef = TypedDict(
     "_RequiredMetricGoalConfigTypeDef",
     {
         "metricDefinition": MetricDefinitionConfigTypeDef,
@@ -1353,23 +1357,23 @@
 )
 
 PutProjectEventsResponseTypeDef = TypedDict(
     "PutProjectEventsResponseTypeDef",
     {
         "eventResults": List[PutProjectEventsResultEntryTypeDef],
         "failedEventCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredScheduledSplitConfigTypeDef = TypedDict(
     "_RequiredScheduledSplitConfigTypeDef",
     {
         "groupWeights": Mapping[str, int],
-        "startTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
     },
 )
 _OptionalScheduledSplitConfigTypeDef = TypedDict(
     "_OptionalScheduledSplitConfigTypeDef",
     {
         "segmentOverrides": Sequence[SegmentOverrideTypeDef],
     },
@@ -1389,29 +1393,29 @@
         "startTime": datetime,
     },
 )
 _OptionalScheduledSplitTypeDef = TypedDict(
     "_OptionalScheduledSplitTypeDef",
     {
         "groupWeights": Dict[str, int],
-        "segmentOverrides": List[SegmentOverrideTypeDef],
+        "segmentOverrides": List[SegmentOverrideOutputTypeDef],
     },
     total=False,
 )
 
 
 class ScheduledSplitTypeDef(_RequiredScheduledSplitTypeDef, _OptionalScheduledSplitTypeDef):
     pass
 
 
 BatchEvaluateFeatureResponseTypeDef = TypedDict(
     "BatchEvaluateFeatureResponseTypeDef",
     {
         "results": List[EvaluationResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFeatureRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFeatureRequestRequestTypeDef",
     {
         "name": str,
@@ -1497,15 +1501,23 @@
 
 
 ListFeaturesResponseTypeDef = TypedDict(
     "ListFeaturesResponseTypeDef",
     {
         "features": List[FeatureSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutProjectEventsRequestRequestTypeDef = TypedDict(
+    "PutProjectEventsRequestRequestTypeDef",
+    {
+        "events": Sequence[EventTypeDef],
+        "project": str,
     },
 )
 
 _RequiredCreateExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperimentRequestRequestTypeDef",
     {
         "metricGoals": Sequence[MetricGoalConfigTypeDef],
@@ -1668,96 +1680,96 @@
     total=False,
 )
 
 CreateFeatureResponseTypeDef = TypedDict(
     "CreateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFeatureResponseTypeDef = TypedDict(
     "GetFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFeatureResponseTypeDef = TypedDict(
     "UpdateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExperimentResponseTypeDef = TypedDict(
     "CreateExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExperimentResponseTypeDef = TypedDict(
     "GetExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExperimentsResponseTypeDef = TypedDict(
     "ListExperimentsResponseTypeDef",
     {
         "experiments": List[ExperimentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateExperimentResponseTypeDef = TypedDict(
     "UpdateExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProjectResponseTypeDef = TypedDict(
     "CreateProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProjectResponseTypeDef = TypedDict(
     "GetProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectDataDeliveryResponseTypeDef = TypedDict(
     "UpdateProjectDataDeliveryResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectResponseTypeDef = TypedDict(
     "UpdateProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateLaunchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchRequestRequestTypeDef",
     {
         "groups": Sequence[LaunchGroupConfigTypeDef],
@@ -1842,43 +1854,43 @@
     pass
 
 
 CreateLaunchResponseTypeDef = TypedDict(
     "CreateLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLaunchResponseTypeDef = TypedDict(
     "GetLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLaunchesResponseTypeDef = TypedDict(
     "ListLaunchesResponseTypeDef",
     {
         "launches": List[LaunchTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartLaunchResponseTypeDef = TypedDict(
     "StartLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLaunchResponseTypeDef = TypedDict(
     "UpdateLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently/type_defs.pyi` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_evidently.type_defs import EvaluationRequestTypeDef
 
-    data: EvaluationRequestTypeDef = {...}
+    data: EvaluationRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -38,14 +38,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "EvaluationRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CloudWatchLogsDestinationConfigTypeDef",
     "CloudWatchLogsDestinationTypeDef",
     "OnlineAbConfigTypeDef",
     "TreatmentConfigTypeDef",
     "LaunchGroupConfigTypeDef",
     "ProjectAppConfigResourceConfigTypeDef",
     "CreateSegmentRequestRequestTypeDef",
@@ -54,77 +55,77 @@
     "DeleteFeatureRequestRequestTypeDef",
     "DeleteLaunchRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DeleteSegmentRequestRequestTypeDef",
     "EvaluateFeatureRequestRequestTypeDef",
     "VariableValueTypeDef",
     "EvaluationRuleTypeDef",
-    "EventTypeDef",
+    "TimestampTypeDef",
     "ExperimentExecutionTypeDef",
     "ExperimentReportTypeDef",
     "ExperimentResultsDataTypeDef",
     "ExperimentScheduleTypeDef",
     "OnlineAbDefinitionTypeDef",
     "TreatmentTypeDef",
     "GetExperimentRequestRequestTypeDef",
-    "GetExperimentResultsRequestRequestTypeDef",
     "GetFeatureRequestRequestTypeDef",
     "GetLaunchRequestRequestTypeDef",
     "GetProjectRequestRequestTypeDef",
     "GetSegmentRequestRequestTypeDef",
     "LaunchExecutionTypeDef",
     "LaunchGroupTypeDef",
-    "ListExperimentsRequestListExperimentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListExperimentsRequestRequestTypeDef",
-    "ListFeaturesRequestListFeaturesPaginateTypeDef",
     "ListFeaturesRequestRequestTypeDef",
-    "ListLaunchesRequestListLaunchesPaginateTypeDef",
     "ListLaunchesRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
-    "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
     "ListSegmentReferencesRequestRequestTypeDef",
     "RefResourceTypeDef",
-    "ListSegmentsRequestListSegmentsPaginateTypeDef",
     "ListSegmentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MetricDefinitionConfigTypeDef",
     "MetricDefinitionTypeDef",
-    "PaginatorConfigTypeDef",
     "ProjectAppConfigResourceTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "PutProjectEventsResultEntryTypeDef",
-    "ResponseMetadataTypeDef",
     "SegmentOverrideTypeDef",
-    "StartExperimentRequestRequestTypeDef",
-    "StartExperimentResponseTypeDef",
+    "SegmentOverrideOutputTypeDef",
     "StartLaunchRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
-    "StopExperimentResponseTypeDef",
     "StopLaunchRequestRequestTypeDef",
-    "StopLaunchResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSegmentPatternRequestRequestTypeDef",
-    "TestSegmentPatternResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchEvaluateFeatureRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartExperimentResponseTypeDef",
+    "StopExperimentResponseTypeDef",
+    "StopLaunchResponseTypeDef",
+    "TestSegmentPatternResponseTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "CreateSegmentResponseTypeDef",
     "GetSegmentResponseTypeDef",
     "ListSegmentsResponseTypeDef",
     "EvaluateFeatureResponseTypeDef",
     "EvaluationResultTypeDef",
     "VariationConfigTypeDef",
     "VariationTypeDef",
     "FeatureSummaryTypeDef",
-    "PutProjectEventsRequestRequestTypeDef",
+    "EventTypeDef",
+    "GetExperimentResultsRequestRequestTypeDef",
+    "StartExperimentRequestRequestTypeDef",
     "GetExperimentResultsResponseTypeDef",
+    "ListExperimentsRequestListExperimentsPaginateTypeDef",
+    "ListFeaturesRequestListFeaturesPaginateTypeDef",
+    "ListLaunchesRequestListLaunchesPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    "ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    "ListSegmentsRequestListSegmentsPaginateTypeDef",
     "ListProjectsResponseTypeDef",
     "ListSegmentReferencesResponseTypeDef",
     "MetricGoalConfigTypeDef",
     "MetricMonitorConfigTypeDef",
     "MetricGoalTypeDef",
     "MetricMonitorTypeDef",
     "ProjectDataDeliveryConfigTypeDef",
@@ -134,14 +135,15 @@
     "ScheduledSplitConfigTypeDef",
     "ScheduledSplitTypeDef",
     "BatchEvaluateFeatureResponseTypeDef",
     "CreateFeatureRequestRequestTypeDef",
     "UpdateFeatureRequestRequestTypeDef",
     "FeatureTypeDef",
     "ListFeaturesResponseTypeDef",
+    "PutProjectEventsRequestRequestTypeDef",
     "CreateExperimentRequestRequestTypeDef",
     "UpdateExperimentRequestRequestTypeDef",
     "ExperimentTypeDef",
     "CreateProjectRequestRequestTypeDef",
     "ProjectTypeDef",
     "ScheduledSplitsLaunchConfigTypeDef",
     "ScheduledSplitsLaunchDefinitionTypeDef",
@@ -182,14 +184,25 @@
 )
 
 class EvaluationRequestTypeDef(
     _RequiredEvaluationRequestTypeDef, _OptionalEvaluationRequestTypeDef
 ):
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
 CloudWatchLogsDestinationConfigTypeDef = TypedDict(
     "CloudWatchLogsDestinationConfigTypeDef",
     {
         "logGroup": str,
     },
     total=False,
 )
@@ -388,23 +401,15 @@
     },
     total=False,
 )
 
 class EvaluationRuleTypeDef(_RequiredEvaluationRuleTypeDef, _OptionalEvaluationRuleTypeDef):
     pass
 
-EventTypeDef = TypedDict(
-    "EventTypeDef",
-    {
-        "data": str,
-        "timestamp": Union[datetime, str],
-        "type": EventTypeType,
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ExperimentExecutionTypeDef = TypedDict(
     "ExperimentExecutionTypeDef",
     {
         "endedTime": datetime,
         "startedTime": datetime,
     },
     total=False,
@@ -471,42 +476,14 @@
     "GetExperimentRequestRequestTypeDef",
     {
         "experiment": str,
         "project": str,
     },
 )
 
-_RequiredGetExperimentResultsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetExperimentResultsRequestRequestTypeDef",
-    {
-        "experiment": str,
-        "metricNames": Sequence[str],
-        "project": str,
-        "treatmentNames": Sequence[str],
-    },
-)
-_OptionalGetExperimentResultsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetExperimentResultsRequestRequestTypeDef",
-    {
-        "baseStat": Literal["Mean"],
-        "endTime": Union[datetime, str],
-        "period": int,
-        "reportNames": Sequence[Literal["BayesianInference"]],
-        "resultStats": Sequence[ExperimentResultRequestTypeType],
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class GetExperimentResultsRequestRequestTypeDef(
-    _RequiredGetExperimentResultsRequestRequestTypeDef,
-    _OptionalGetExperimentResultsRequestRequestTypeDef,
-):
-    pass
-
 GetFeatureRequestRequestTypeDef = TypedDict(
     "GetFeatureRequestRequestTypeDef",
     {
         "feature": str,
         "project": str,
     },
 )
@@ -556,35 +533,24 @@
     },
     total=False,
 )
 
 class LaunchGroupTypeDef(_RequiredLaunchGroupTypeDef, _OptionalLaunchGroupTypeDef):
     pass
 
-_RequiredListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
-    "_RequiredListExperimentsRequestListExperimentsPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
-    "_OptionalListExperimentsRequestListExperimentsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "status": ExperimentStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListExperimentsRequestListExperimentsPaginateTypeDef(
-    _RequiredListExperimentsRequestListExperimentsPaginateTypeDef,
-    _OptionalListExperimentsRequestListExperimentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListExperimentsRequestRequestTypeDef = TypedDict(
     "_RequiredListExperimentsRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListExperimentsRequestRequestTypeDef = TypedDict(
@@ -598,34 +564,14 @@
 )
 
 class ListExperimentsRequestRequestTypeDef(
     _RequiredListExperimentsRequestRequestTypeDef, _OptionalListExperimentsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
-    "_RequiredListFeaturesRequestListFeaturesPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
-    "_OptionalListFeaturesRequestListFeaturesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFeaturesRequestListFeaturesPaginateTypeDef(
-    _RequiredListFeaturesRequestListFeaturesPaginateTypeDef,
-    _OptionalListFeaturesRequestListFeaturesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFeaturesRequestRequestTypeDef = TypedDict(
     "_RequiredListFeaturesRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListFeaturesRequestRequestTypeDef = TypedDict(
@@ -638,35 +584,14 @@
 )
 
 class ListFeaturesRequestRequestTypeDef(
     _RequiredListFeaturesRequestRequestTypeDef, _OptionalListFeaturesRequestRequestTypeDef
 ):
     pass
 
-_RequiredListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
-    "_RequiredListLaunchesRequestListLaunchesPaginateTypeDef",
-    {
-        "project": str,
-    },
-)
-_OptionalListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
-    "_OptionalListLaunchesRequestListLaunchesPaginateTypeDef",
-    {
-        "status": LaunchStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListLaunchesRequestListLaunchesPaginateTypeDef(
-    _RequiredListLaunchesRequestListLaunchesPaginateTypeDef,
-    _OptionalListLaunchesRequestListLaunchesPaginateTypeDef,
-):
-    pass
-
 _RequiredListLaunchesRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchesRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalListLaunchesRequestRequestTypeDef = TypedDict(
@@ -680,22 +605,14 @@
 )
 
 class ListLaunchesRequestRequestTypeDef(
     _RequiredListLaunchesRequestRequestTypeDef, _OptionalListLaunchesRequestRequestTypeDef
 ):
     pass
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -724,35 +641,14 @@
     },
     total=False,
 )
 
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
-_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
-    "_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    {
-        "segment": str,
-        "type": SegmentReferenceResourceTypeType,
-    },
-)
-_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
-    "_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(
-    _RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-    _OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
-):
-    pass
-
 _RequiredListSegmentReferencesRequestRequestTypeDef = TypedDict(
     "_RequiredListSegmentReferencesRequestRequestTypeDef",
     {
         "segment": str,
         "type": SegmentReferenceResourceTypeType,
     },
 )
@@ -789,22 +685,14 @@
     },
     total=False,
 )
 
 class RefResourceTypeDef(_RequiredRefResourceTypeDef, _OptionalRefResourceTypeDef):
     pass
 
-ListSegmentsRequestListSegmentsPaginateTypeDef = TypedDict(
-    "ListSegmentsRequestListSegmentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSegmentsRequestRequestTypeDef = TypedDict(
     "ListSegmentsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -813,22 +701,14 @@
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
 _RequiredMetricDefinitionConfigTypeDef = TypedDict(
     "_RequiredMetricDefinitionConfigTypeDef",
     {
         "entityIdKey": str,
         "name": str,
         "valueKey": str,
     },
@@ -855,24 +735,14 @@
         "name": str,
         "unitLabel": str,
         "valueKey": str,
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
 ProjectAppConfigResourceTypeDef = TypedDict(
     "ProjectAppConfigResourceTypeDef",
     {
         "applicationId": str,
         "configurationProfileId": str,
         "environmentId": str,
     },
@@ -902,48 +772,29 @@
         "errorCode": str,
         "errorMessage": str,
         "eventId": str,
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
 SegmentOverrideTypeDef = TypedDict(
     "SegmentOverrideTypeDef",
     {
         "evaluationOrder": int,
         "segment": str,
         "weights": Mapping[str, int],
     },
 )
 
-StartExperimentRequestRequestTypeDef = TypedDict(
-    "StartExperimentRequestRequestTypeDef",
-    {
-        "analysisCompleteTime": Union[datetime, str],
-        "experiment": str,
-        "project": str,
-    },
-)
-
-StartExperimentResponseTypeDef = TypedDict(
-    "StartExperimentResponseTypeDef",
+SegmentOverrideOutputTypeDef = TypedDict(
+    "SegmentOverrideOutputTypeDef",
     {
-        "startedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "evaluationOrder": int,
+        "segment": str,
+        "weights": Dict[str, int],
     },
 )
 
 StartLaunchRequestRequestTypeDef = TypedDict(
     "StartLaunchRequestRequestTypeDef",
     {
         "launch": str,
@@ -968,22 +819,14 @@
 )
 
 class StopExperimentRequestRequestTypeDef(
     _RequiredStopExperimentRequestRequestTypeDef, _OptionalStopExperimentRequestRequestTypeDef
 ):
     pass
 
-StopExperimentResponseTypeDef = TypedDict(
-    "StopExperimentResponseTypeDef",
-    {
-        "endedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStopLaunchRequestRequestTypeDef = TypedDict(
     "_RequiredStopLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -997,22 +840,14 @@
 )
 
 class StopLaunchRequestRequestTypeDef(
     _RequiredStopLaunchRequestRequestTypeDef, _OptionalStopLaunchRequestRequestTypeDef
 ):
     pass
 
-StopLaunchResponseTypeDef = TypedDict(
-    "StopLaunchResponseTypeDef",
-    {
-        "endedTime": datetime,
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
@@ -1021,22 +856,14 @@
     "TestSegmentPatternRequestRequestTypeDef",
     {
         "pattern": str,
         "payload": str,
     },
 )
 
-TestSegmentPatternResponseTypeDef = TypedDict(
-    "TestSegmentPatternResponseTypeDef",
-    {
-        "match": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1045,14 +872,54 @@
     "BatchEvaluateFeatureRequestRequestTypeDef",
     {
         "project": str,
         "requests": Sequence[EvaluationRequestTypeDef],
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartExperimentResponseTypeDef = TypedDict(
+    "StartExperimentResponseTypeDef",
+    {
+        "startedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopExperimentResponseTypeDef = TypedDict(
+    "StopExperimentResponseTypeDef",
+    {
+        "endedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopLaunchResponseTypeDef = TypedDict(
+    "StopLaunchResponseTypeDef",
+    {
+        "endedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestSegmentPatternResponseTypeDef = TypedDict(
+    "TestSegmentPatternResponseTypeDef",
+    {
+        "match": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "project": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
@@ -1069,43 +936,43 @@
 ):
     pass
 
 CreateSegmentResponseTypeDef = TypedDict(
     "CreateSegmentResponseTypeDef",
     {
         "segment": SegmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentResponseTypeDef = TypedDict(
     "GetSegmentResponseTypeDef",
     {
         "segment": SegmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSegmentsResponseTypeDef = TypedDict(
     "ListSegmentsResponseTypeDef",
     {
         "nextToken": str,
         "segments": List[SegmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EvaluateFeatureResponseTypeDef = TypedDict(
     "EvaluateFeatureResponseTypeDef",
     {
         "details": str,
         "reason": str,
         "value": VariableValueTypeDef,
         "variation": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEvaluationResultTypeDef = TypedDict(
     "_RequiredEvaluationResultTypeDef",
     {
         "entityId": str,
@@ -1165,48 +1032,185 @@
     },
     total=False,
 )
 
 class FeatureSummaryTypeDef(_RequiredFeatureSummaryTypeDef, _OptionalFeatureSummaryTypeDef):
     pass
 
-PutProjectEventsRequestRequestTypeDef = TypedDict(
-    "PutProjectEventsRequestRequestTypeDef",
+EventTypeDef = TypedDict(
+    "EventTypeDef",
     {
-        "events": Sequence[EventTypeDef],
+        "data": str,
+        "timestamp": TimestampTypeDef,
+        "type": EventTypeType,
+    },
+)
+
+_RequiredGetExperimentResultsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetExperimentResultsRequestRequestTypeDef",
+    {
+        "experiment": str,
+        "metricNames": Sequence[str],
+        "project": str,
+        "treatmentNames": Sequence[str],
+    },
+)
+_OptionalGetExperimentResultsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetExperimentResultsRequestRequestTypeDef",
+    {
+        "baseStat": Literal["Mean"],
+        "endTime": TimestampTypeDef,
+        "period": int,
+        "reportNames": Sequence[Literal["BayesianInference"]],
+        "resultStats": Sequence[ExperimentResultRequestTypeType],
+        "startTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class GetExperimentResultsRequestRequestTypeDef(
+    _RequiredGetExperimentResultsRequestRequestTypeDef,
+    _OptionalGetExperimentResultsRequestRequestTypeDef,
+):
+    pass
+
+StartExperimentRequestRequestTypeDef = TypedDict(
+    "StartExperimentRequestRequestTypeDef",
+    {
+        "analysisCompleteTime": TimestampTypeDef,
+        "experiment": str,
         "project": str,
     },
 )
 
 GetExperimentResultsResponseTypeDef = TypedDict(
     "GetExperimentResultsResponseTypeDef",
     {
         "details": str,
         "reports": List[ExperimentReportTypeDef],
         "resultsData": List[ExperimentResultsDataTypeDef],
         "timestamps": List[datetime],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
+    "_RequiredListExperimentsRequestListExperimentsPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListExperimentsRequestListExperimentsPaginateTypeDef = TypedDict(
+    "_OptionalListExperimentsRequestListExperimentsPaginateTypeDef",
+    {
+        "status": ExperimentStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListExperimentsRequestListExperimentsPaginateTypeDef(
+    _RequiredListExperimentsRequestListExperimentsPaginateTypeDef,
+    _OptionalListExperimentsRequestListExperimentsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
+    "_RequiredListFeaturesRequestListFeaturesPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListFeaturesRequestListFeaturesPaginateTypeDef = TypedDict(
+    "_OptionalListFeaturesRequestListFeaturesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFeaturesRequestListFeaturesPaginateTypeDef(
+    _RequiredListFeaturesRequestListFeaturesPaginateTypeDef,
+    _OptionalListFeaturesRequestListFeaturesPaginateTypeDef,
+):
+    pass
+
+_RequiredListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
+    "_RequiredListLaunchesRequestListLaunchesPaginateTypeDef",
+    {
+        "project": str,
+    },
+)
+_OptionalListLaunchesRequestListLaunchesPaginateTypeDef = TypedDict(
+    "_OptionalListLaunchesRequestListLaunchesPaginateTypeDef",
+    {
+        "status": LaunchStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListLaunchesRequestListLaunchesPaginateTypeDef(
+    _RequiredListLaunchesRequestListLaunchesPaginateTypeDef,
+    _OptionalListLaunchesRequestListLaunchesPaginateTypeDef,
+):
+    pass
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
+    "_RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    {
+        "segment": str,
+        "type": SegmentReferenceResourceTypeType,
+    },
+)
+_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef = TypedDict(
+    "_OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(
+    _RequiredListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+    _OptionalListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+):
+    pass
+
+ListSegmentsRequestListSegmentsPaginateTypeDef = TypedDict(
+    "ListSegmentsRequestListSegmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListProjectsResponseTypeDef = TypedDict(
     "ListProjectsResponseTypeDef",
     {
         "nextToken": str,
         "projects": List[ProjectSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSegmentReferencesResponseTypeDef = TypedDict(
     "ListSegmentReferencesResponseTypeDef",
     {
         "nextToken": str,
         "referencedBy": List[RefResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMetricGoalConfigTypeDef = TypedDict(
     "_RequiredMetricGoalConfigTypeDef",
     {
         "metricDefinition": MetricDefinitionConfigTypeDef,
@@ -1294,23 +1298,23 @@
 )
 
 PutProjectEventsResponseTypeDef = TypedDict(
     "PutProjectEventsResponseTypeDef",
     {
         "eventResults": List[PutProjectEventsResultEntryTypeDef],
         "failedEventCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredScheduledSplitConfigTypeDef = TypedDict(
     "_RequiredScheduledSplitConfigTypeDef",
     {
         "groupWeights": Mapping[str, int],
-        "startTime": Union[datetime, str],
+        "startTime": TimestampTypeDef,
     },
 )
 _OptionalScheduledSplitConfigTypeDef = TypedDict(
     "_OptionalScheduledSplitConfigTypeDef",
     {
         "segmentOverrides": Sequence[SegmentOverrideTypeDef],
     },
@@ -1328,27 +1332,27 @@
         "startTime": datetime,
     },
 )
 _OptionalScheduledSplitTypeDef = TypedDict(
     "_OptionalScheduledSplitTypeDef",
     {
         "groupWeights": Dict[str, int],
-        "segmentOverrides": List[SegmentOverrideTypeDef],
+        "segmentOverrides": List[SegmentOverrideOutputTypeDef],
     },
     total=False,
 )
 
 class ScheduledSplitTypeDef(_RequiredScheduledSplitTypeDef, _OptionalScheduledSplitTypeDef):
     pass
 
 BatchEvaluateFeatureResponseTypeDef = TypedDict(
     "BatchEvaluateFeatureResponseTypeDef",
     {
         "results": List[EvaluationResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFeatureRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFeatureRequestRequestTypeDef",
     {
         "name": str,
@@ -1428,15 +1432,23 @@
     pass
 
 ListFeaturesResponseTypeDef = TypedDict(
     "ListFeaturesResponseTypeDef",
     {
         "features": List[FeatureSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutProjectEventsRequestRequestTypeDef = TypedDict(
+    "PutProjectEventsRequestRequestTypeDef",
+    {
+        "events": Sequence[EventTypeDef],
+        "project": str,
     },
 )
 
 _RequiredCreateExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperimentRequestRequestTypeDef",
     {
         "metricGoals": Sequence[MetricGoalConfigTypeDef],
@@ -1589,96 +1601,96 @@
     total=False,
 )
 
 CreateFeatureResponseTypeDef = TypedDict(
     "CreateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFeatureResponseTypeDef = TypedDict(
     "GetFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFeatureResponseTypeDef = TypedDict(
     "UpdateFeatureResponseTypeDef",
     {
         "feature": FeatureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExperimentResponseTypeDef = TypedDict(
     "CreateExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExperimentResponseTypeDef = TypedDict(
     "GetExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExperimentsResponseTypeDef = TypedDict(
     "ListExperimentsResponseTypeDef",
     {
         "experiments": List[ExperimentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateExperimentResponseTypeDef = TypedDict(
     "UpdateExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProjectResponseTypeDef = TypedDict(
     "CreateProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProjectResponseTypeDef = TypedDict(
     "GetProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectDataDeliveryResponseTypeDef = TypedDict(
     "UpdateProjectDataDeliveryResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectResponseTypeDef = TypedDict(
     "UpdateProjectResponseTypeDef",
     {
         "project": ProjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateLaunchRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchRequestRequestTypeDef",
     {
         "groups": Sequence[LaunchGroupConfigTypeDef],
@@ -1757,43 +1769,43 @@
 class LaunchTypeDef(_RequiredLaunchTypeDef, _OptionalLaunchTypeDef):
     pass
 
 CreateLaunchResponseTypeDef = TypedDict(
     "CreateLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLaunchResponseTypeDef = TypedDict(
     "GetLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLaunchesResponseTypeDef = TypedDict(
     "ListLaunchesResponseTypeDef",
     {
         "launches": List[LaunchTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartLaunchResponseTypeDef = TypedDict(
     "StartLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLaunchResponseTypeDef = TypedDict(
     "UpdateLaunchResponseTypeDef",
     {
         "launch": LaunchTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently.egg-info/PKG-INFO` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-evidently
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudWatchEvidently 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudWatchEvidently 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore evidently type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore evidently type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-evidently"></a>
 
 # types-aiobotocore-evidently
 
 [![PyPI - types-aiobotocore-evidently](https://img.shields.io/pypi/v/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-evidently.svg?color=blue)](https://pypi.org/project/types-aiobotocore-evidently)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-evidently?color=blue)](https://pypistats.org/packages/types-aiobotocore-evidently)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-evidently)](https://pepy.tech/project/types-aiobotocore-evidently)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudWatchEvidently 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
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
 [types-aiobotocore-evidently docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently/).
 
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
@@ -341,24 +340,25 @@
 )
 
 
 def check_value(value: ChangeDirectionEnumType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_evidently.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_evidently.type_defs import (
     EvaluationRequestTypeDef,
+    ResponseMetadataTypeDef,
     CloudWatchLogsDestinationConfigTypeDef,
     CloudWatchLogsDestinationTypeDef,
     OnlineAbConfigTypeDef,
     TreatmentConfigTypeDef,
     LaunchGroupConfigTypeDef,
     ProjectAppConfigResourceConfigTypeDef,
     CreateSegmentRequestRequestTypeDef,
@@ -367,77 +367,77 @@
     DeleteFeatureRequestRequestTypeDef,
     DeleteLaunchRequestRequestTypeDef,
     DeleteProjectRequestRequestTypeDef,
     DeleteSegmentRequestRequestTypeDef,
     EvaluateFeatureRequestRequestTypeDef,
     VariableValueTypeDef,
     EvaluationRuleTypeDef,
-    EventTypeDef,
+    TimestampTypeDef,
     ExperimentExecutionTypeDef,
     ExperimentReportTypeDef,
     ExperimentResultsDataTypeDef,
     ExperimentScheduleTypeDef,
     OnlineAbDefinitionTypeDef,
     TreatmentTypeDef,
     GetExperimentRequestRequestTypeDef,
-    GetExperimentResultsRequestRequestTypeDef,
     GetFeatureRequestRequestTypeDef,
     GetLaunchRequestRequestTypeDef,
     GetProjectRequestRequestTypeDef,
     GetSegmentRequestRequestTypeDef,
     LaunchExecutionTypeDef,
     LaunchGroupTypeDef,
-    ListExperimentsRequestListExperimentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListExperimentsRequestRequestTypeDef,
-    ListFeaturesRequestListFeaturesPaginateTypeDef,
     ListFeaturesRequestRequestTypeDef,
-    ListLaunchesRequestListLaunchesPaginateTypeDef,
     ListLaunchesRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
     ListSegmentReferencesRequestRequestTypeDef,
     RefResourceTypeDef,
-    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListSegmentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MetricDefinitionConfigTypeDef,
     MetricDefinitionTypeDef,
-    PaginatorConfigTypeDef,
     ProjectAppConfigResourceTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     PutProjectEventsResultEntryTypeDef,
-    ResponseMetadataTypeDef,
     SegmentOverrideTypeDef,
-    StartExperimentRequestRequestTypeDef,
-    StartExperimentResponseTypeDef,
+    SegmentOverrideOutputTypeDef,
     StartLaunchRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
-    StopExperimentResponseTypeDef,
     StopLaunchRequestRequestTypeDef,
-    StopLaunchResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TestSegmentPatternRequestRequestTypeDef,
-    TestSegmentPatternResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchEvaluateFeatureRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartExperimentResponseTypeDef,
+    StopExperimentResponseTypeDef,
+    StopLaunchResponseTypeDef,
+    TestSegmentPatternResponseTypeDef,
     UpdateProjectRequestRequestTypeDef,
     CreateSegmentResponseTypeDef,
     GetSegmentResponseTypeDef,
     ListSegmentsResponseTypeDef,
     EvaluateFeatureResponseTypeDef,
     EvaluationResultTypeDef,
     VariationConfigTypeDef,
     VariationTypeDef,
     FeatureSummaryTypeDef,
-    PutProjectEventsRequestRequestTypeDef,
+    EventTypeDef,
+    GetExperimentResultsRequestRequestTypeDef,
+    StartExperimentRequestRequestTypeDef,
     GetExperimentResultsResponseTypeDef,
+    ListExperimentsRequestListExperimentsPaginateTypeDef,
+    ListFeaturesRequestListFeaturesPaginateTypeDef,
+    ListLaunchesRequestListLaunchesPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
+    ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef,
+    ListSegmentsRequestListSegmentsPaginateTypeDef,
     ListProjectsResponseTypeDef,
     ListSegmentReferencesResponseTypeDef,
     MetricGoalConfigTypeDef,
     MetricMonitorConfigTypeDef,
     MetricGoalTypeDef,
     MetricMonitorTypeDef,
     ProjectDataDeliveryConfigTypeDef,
@@ -447,14 +447,15 @@
     ScheduledSplitConfigTypeDef,
     ScheduledSplitTypeDef,
     BatchEvaluateFeatureResponseTypeDef,
     CreateFeatureRequestRequestTypeDef,
     UpdateFeatureRequestRequestTypeDef,
     FeatureTypeDef,
     ListFeaturesResponseTypeDef,
+    PutProjectEventsRequestRequestTypeDef,
     CreateExperimentRequestRequestTypeDef,
     UpdateExperimentRequestRequestTypeDef,
     ExperimentTypeDef,
     CreateProjectRequestRequestTypeDef,
     ProjectTypeDef,
     ScheduledSplitsLaunchConfigTypeDef,
     ScheduledSplitsLaunchDefinitionTypeDef,
@@ -476,15 +477,15 @@
     GetLaunchResponseTypeDef,
     ListLaunchesResponseTypeDef,
     StartLaunchResponseTypeDef,
     UpdateLaunchResponseTypeDef,
 )
 
 
-def get_structure() -> EvaluationRequestTypeDef:
+def get_value() -> EvaluationRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-evidently-2.5.2/types_aiobotocore_evidently.egg-info/SOURCES.txt` & `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/SOURCES.txt`

 * *Files identical despite different names*


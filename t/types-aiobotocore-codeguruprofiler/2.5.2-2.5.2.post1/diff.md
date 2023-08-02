# Comparing `tmp/types-aiobotocore-codeguruprofiler-2.5.2.tar.gz` & `tmp/types-aiobotocore-codeguruprofiler-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeguruprofiler-2.5.2.tar", last modified: Sat Jul  8 01:43:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeguruprofiler-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:04 2023, max compression
```

## Comparing `types-aiobotocore-codeguruprofiler-2.5.2.tar` & `types-aiobotocore-codeguruprofiler-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:24.993891 types-aiobotocore-codeguruprofiler-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:36.000000 types-aiobotocore-codeguruprofiler-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15894 2023-07-08 01:43:24.993891 types-aiobotocore-codeguruprofiler-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-07-08 01:27:36.000000 types-aiobotocore-codeguruprofiler-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:24.993891 types-aiobotocore-codeguruprofiler-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-08 01:27:36.000000 types-aiobotocore-codeguruprofiler-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:24.993891 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-08 01:27:36.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-08 01:27:36.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-08 01:27:36.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21466 2023-07-08 01:27:36.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21433 2023-07-08 01:27:36.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-07-08 01:27:37.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-08 01:27:37.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-08 01:27:36.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-08 01:27:36.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:36.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22319 2023-07-08 01:27:37.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22290 2023-07-08 01:27:37.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:36.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:24.993891 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15894 2023-07-08 01:43:24.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-08 01:43:24.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:24.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:24.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:24.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 01:43:24.000000 types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.505619 types-aiobotocore-codeguruprofiler-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-08-02 14:52:04.505619 types-aiobotocore-codeguruprofiler-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14434 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.505619 types-aiobotocore-codeguruprofiler-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.505619 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21367 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-08-02 14:35:11.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23256 2023-08-02 14:35:11.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23225 2023-08-02 14:35:11.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:10.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.505619 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-08-02 14:52:04.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:52:04.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:04.000000 types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/LICENSE` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/PKG-INFO` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguruprofiler
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeGuruProfiler 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeGuruProfiler 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codeguruprofiler type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore codeguruprofiler type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codeguruprofiler"></a>
 
 # types-aiobotocore-codeguruprofiler
 
 [![PyPI - types-aiobotocore-codeguruprofiler](https://img.shields.io/pypi/v/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeguruprofiler?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeguruprofiler)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguruprofiler)](https://pepy.tech/project/types-aiobotocore-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeGuruProfiler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [types-aiobotocore-codeguruprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/).
 
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
@@ -315,90 +314,96 @@
 )
 
 
 def check_value(value: ActionGroupType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codeguruprofiler.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codeguruprofiler.type_defs import (
-    ChannelTypeDef,
+    ResponseMetadataTypeDef,
     AgentConfigurationTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
-    FrameMetricTypeDef,
+    TimestampTypeDef,
     TimestampStructureTypeDef,
+    BlobTypeDef,
+    ChannelOutputTypeDef,
+    ChannelTypeDef,
     ConfigureAgentRequestRequestTypeDef,
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
+    FrameMetricOutputTypeDef,
+    FrameMetricTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
-    GetProfileRequestRequestTypeDef,
-    GetProfileResponseTypeDef,
-    GetRecommendationsRequestRequestTypeDef,
-    ListFindingsReportsRequestRequestTypeDef,
-    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
-    ListProfileTimesRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ProfileTimeTypeDef,
     ListProfilingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MatchTypeDef,
-    PaginatorConfigTypeDef,
     PatternTypeDef,
-    PostAgentProfileRequestRequestTypeDef,
     PutPermissionRequestRequestTypeDef,
-    PutPermissionResponseTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    RemovePermissionResponseTypeDef,
-    ResponseMetadataTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AddNotificationChannelsRequestRequestTypeDef,
-    NotificationConfigurationTypeDef,
+    GetPolicyResponseTypeDef,
+    GetProfileResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutPermissionResponseTypeDef,
+    RemovePermissionResponseTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
-    BatchGetFrameMetricDataRequestRequestTypeDef,
-    FrameMetricDatumTypeDef,
+    GetProfileRequestRequestTypeDef,
+    GetRecommendationsRequestRequestTypeDef,
+    ListFindingsReportsRequestRequestTypeDef,
+    ListProfileTimesRequestRequestTypeDef,
+    PostAgentProfileRequestRequestTypeDef,
+    NotificationConfigurationTypeDef,
+    ChannelUnionTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
+    FrameMetricDatumTypeDef,
+    FrameMetricUnionTypeDef,
+    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
+    ProfilingGroupDescriptionTypeDef,
+    AnomalyTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
-    ProfilingGroupDescriptionTypeDef,
-    AnomalyTypeDef,
+    AddNotificationChannelsRequestRequestTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
+    BatchGetFrameMetricDataRequestRequestTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     UpdateProfilingGroupResponseTypeDef,
     GetRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> ChannelTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/README.md` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-codeguruprofiler
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CodeGuruProfiler 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore codeguruprofiler type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codeguruprofiler"></a>
 
 # types-aiobotocore-codeguruprofiler
 
 [![PyPI - types-aiobotocore-codeguruprofiler](https://img.shields.io/pypi/v/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeguruprofiler?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeguruprofiler)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguruprofiler)](https://pepy.tech/project/types-aiobotocore-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeGuruProfiler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [types-aiobotocore-codeguruprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/).
 
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
@@ -282,90 +314,96 @@
 )
 
 
 def check_value(value: ActionGroupType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codeguruprofiler.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codeguruprofiler.type_defs import (
-    ChannelTypeDef,
+    ResponseMetadataTypeDef,
     AgentConfigurationTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
-    FrameMetricTypeDef,
+    TimestampTypeDef,
     TimestampStructureTypeDef,
+    BlobTypeDef,
+    ChannelOutputTypeDef,
+    ChannelTypeDef,
     ConfigureAgentRequestRequestTypeDef,
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
+    FrameMetricOutputTypeDef,
+    FrameMetricTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
-    GetProfileRequestRequestTypeDef,
-    GetProfileResponseTypeDef,
-    GetRecommendationsRequestRequestTypeDef,
-    ListFindingsReportsRequestRequestTypeDef,
-    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
-    ListProfileTimesRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ProfileTimeTypeDef,
     ListProfilingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MatchTypeDef,
-    PaginatorConfigTypeDef,
     PatternTypeDef,
-    PostAgentProfileRequestRequestTypeDef,
     PutPermissionRequestRequestTypeDef,
-    PutPermissionResponseTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    RemovePermissionResponseTypeDef,
-    ResponseMetadataTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AddNotificationChannelsRequestRequestTypeDef,
-    NotificationConfigurationTypeDef,
+    GetPolicyResponseTypeDef,
+    GetProfileResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutPermissionResponseTypeDef,
+    RemovePermissionResponseTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
-    BatchGetFrameMetricDataRequestRequestTypeDef,
-    FrameMetricDatumTypeDef,
+    GetProfileRequestRequestTypeDef,
+    GetRecommendationsRequestRequestTypeDef,
+    ListFindingsReportsRequestRequestTypeDef,
+    ListProfileTimesRequestRequestTypeDef,
+    PostAgentProfileRequestRequestTypeDef,
+    NotificationConfigurationTypeDef,
+    ChannelUnionTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
+    FrameMetricDatumTypeDef,
+    FrameMetricUnionTypeDef,
+    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
+    ProfilingGroupDescriptionTypeDef,
+    AnomalyTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
-    ProfilingGroupDescriptionTypeDef,
-    AnomalyTypeDef,
+    AddNotificationChannelsRequestRequestTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
+    BatchGetFrameMetricDataRequestRequestTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     UpdateProfilingGroupResponseTypeDef,
     GetRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> ChannelTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/setup.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeguruprofiler",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_codeguruprofiler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeGuruProfiler 2.5.2 service generated with"
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
-    keywords="aiobotocore codeguruprofiler type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore codeguruprofiler type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_codeguruprofiler": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/"
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/__init__.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/__init__.pyi` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/__main__.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeGuruProfiler 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CodeGuruProfiler 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler\nOther"
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

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/client.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,50 +11,50 @@
 
     session = get_session()
     async with session.create_client("codeguruprofiler") as client:
         client: CodeGuruProfilerClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     AggregationPeriodType,
     ComputePlatformType,
     FeedbackTypeType,
     MetadataFieldType,
     OrderByType,
 )
 from .paginator import ListProfileTimesPaginator
 from .type_defs import (
     AddNotificationChannelsResponseTypeDef,
     AgentOrchestrationConfigTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
-    ChannelTypeDef,
+    BlobTypeDef,
+    ChannelUnionTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
-    FrameMetricTypeDef,
+    FrameMetricUnionTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProfileResponseTypeDef,
     GetRecommendationsResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
     ListProfileTimesResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutPermissionResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
     RemovePermissionResponseTypeDef,
+    TimestampTypeDef,
     UpdateProfilingGroupResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -95,31 +95,31 @@
         CodeGuruProfilerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#exceptions)
         """
 
     async def add_notification_channels(
-        self, *, channels: Sequence[ChannelTypeDef], profilingGroupName: str
+        self, *, channels: Sequence[ChannelUnionTypeDef], profilingGroupName: str
     ) -> AddNotificationChannelsResponseTypeDef:
         """
         Add up to 2 anomaly notifications channels for a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.add_notification_channels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#add_notification_channels)
         """
 
     async def batch_get_frame_metric_data(
         self,
         *,
         profilingGroupName: str,
-        endTime: Union[datetime, str] = ...,
-        frameMetrics: Sequence[FrameMetricTypeDef] = ...,
+        endTime: TimestampTypeDef = ...,
+        frameMetrics: Sequence[FrameMetricUnionTypeDef] = ...,
         period: str = ...,
-        startTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
         targetResolution: AggregationPeriodType = ...
     ) -> BatchGetFrameMetricDataResponseTypeDef:
         """
         Returns the time series of values for a requested list of frame metrics from a
         time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.batch_get_frame_metric_data)
@@ -240,32 +240,32 @@
         """
 
     async def get_profile(
         self,
         *,
         profilingGroupName: str,
         accept: str = ...,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         maxDepth: int = ...,
         period: str = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> GetProfileResponseTypeDef:
         """
         Gets the aggregated profile of a profiling group for a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#get_profile)
         """
 
     async def get_recommendations(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         locale: str = ...
     ) -> GetRecommendationsResponseTypeDef:
         """
         Returns a list of
         [Recommendation](https://docs.aws.amazon.com/codeguru/latest/profiler-
         api/API_Recommendation.html)_ objects that contain recommendations for a
         profiling group for a given time period.
@@ -273,35 +273,35 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#get_recommendations)
         """
 
     async def list_findings_reports(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         dailyReportsOnly: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListFindingsReportsResponseTypeDef:
         """
         List the available reports for a given profiling group and time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_findings_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#list_findings_reports)
         """
 
     async def list_profile_times(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         period: AggregationPeriodType,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...,
         orderBy: OrderByType = ...
     ) -> ListProfileTimesResponseTypeDef:
         """
         Lists the start times of the available aggregated profiles of a profiling group
         for an aggregation period within the specified time range.
@@ -329,15 +329,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#list_tags_for_resource)
         """
 
     async def post_agent_profile(
         self,
         *,
-        agentProfile: Union[str, bytes, IO[Any], StreamingBody],
+        agentProfile: BlobTypeDef,
         contentType: str,
         profilingGroupName: str,
         profileToken: str = ...
     ) -> Dict[str, Any]:
         """
         Submits profiling data to an aggregated profile of a profiling group.
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/client.pyi` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,50 +11,50 @@
 
     session = get_session()
     async with session.create_client("codeguruprofiler") as client:
         client: CodeGuruProfilerClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     AggregationPeriodType,
     ComputePlatformType,
     FeedbackTypeType,
     MetadataFieldType,
     OrderByType,
 )
 from .paginator import ListProfileTimesPaginator
 from .type_defs import (
     AddNotificationChannelsResponseTypeDef,
     AgentOrchestrationConfigTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
-    ChannelTypeDef,
+    BlobTypeDef,
+    ChannelUnionTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
-    FrameMetricTypeDef,
+    FrameMetricUnionTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetProfileResponseTypeDef,
     GetRecommendationsResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
     ListProfileTimesResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutPermissionResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
     RemovePermissionResponseTypeDef,
+    TimestampTypeDef,
     UpdateProfilingGroupResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -90,30 +90,30 @@
         """
         CodeGuruProfilerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#exceptions)
         """
     async def add_notification_channels(
-        self, *, channels: Sequence[ChannelTypeDef], profilingGroupName: str
+        self, *, channels: Sequence[ChannelUnionTypeDef], profilingGroupName: str
     ) -> AddNotificationChannelsResponseTypeDef:
         """
         Add up to 2 anomaly notifications channels for a profiling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.add_notification_channels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#add_notification_channels)
         """
     async def batch_get_frame_metric_data(
         self,
         *,
         profilingGroupName: str,
-        endTime: Union[datetime, str] = ...,
-        frameMetrics: Sequence[FrameMetricTypeDef] = ...,
+        endTime: TimestampTypeDef = ...,
+        frameMetrics: Sequence[FrameMetricUnionTypeDef] = ...,
         period: str = ...,
-        startTime: Union[datetime, str] = ...,
+        startTime: TimestampTypeDef = ...,
         targetResolution: AggregationPeriodType = ...
     ) -> BatchGetFrameMetricDataResponseTypeDef:
         """
         Returns the time series of values for a requested list of frame metrics from a
         time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.batch_get_frame_metric_data)
@@ -223,65 +223,65 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#get_policy)
         """
     async def get_profile(
         self,
         *,
         profilingGroupName: str,
         accept: str = ...,
-        endTime: Union[datetime, str] = ...,
+        endTime: TimestampTypeDef = ...,
         maxDepth: int = ...,
         period: str = ...,
-        startTime: Union[datetime, str] = ...
+        startTime: TimestampTypeDef = ...
     ) -> GetProfileResponseTypeDef:
         """
         Gets the aggregated profile of a profiling group for a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#get_profile)
         """
     async def get_recommendations(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         locale: str = ...
     ) -> GetRecommendationsResponseTypeDef:
         """
         Returns a list of
         [Recommendation](https://docs.aws.amazon.com/codeguru/latest/profiler-
         api/API_Recommendation.html)_ objects that contain recommendations for a
         profiling group for a given time period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#get_recommendations)
         """
     async def list_findings_reports(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         dailyReportsOnly: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListFindingsReportsResponseTypeDef:
         """
         List the available reports for a given profiling group and time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_findings_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#list_findings_reports)
         """
     async def list_profile_times(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         period: AggregationPeriodType,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         maxResults: int = ...,
         nextToken: str = ...,
         orderBy: OrderByType = ...
     ) -> ListProfileTimesResponseTypeDef:
         """
         Lists the start times of the available aggregated profiles of a profiling group
         for an aggregation period within the specified time range.
@@ -306,15 +306,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/client/#list_tags_for_resource)
         """
     async def post_agent_profile(
         self,
         *,
-        agentProfile: Union[str, bytes, IO[Any], StreamingBody],
+        agentProfile: BlobTypeDef,
         contentType: str,
         profilingGroupName: str,
         profileToken: str = ...
     ) -> Dict[str, Any]:
         """
         Submits profiling data to an aggregated profile of a profiling group.
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/literals.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/literals.pyi` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/paginator.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -16,49 +16,45 @@
     session = get_session()
     with session.create_client("codeguruprofiler") as client:
         client: CodeGuruProfilerClient
 
         list_profile_times_paginator: ListProfileTimesPaginator = client.get_paginator("list_profile_times")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import AggregationPeriodType, OrderByType
-from .type_defs import ListProfileTimesResponseTypeDef, PaginatorConfigTypeDef
+from .type_defs import ListProfileTimesResponseTypeDef, PaginatorConfigTypeDef, TimestampTypeDef
 
 __all__ = ("ListProfileTimesPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListProfileTimesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/paginators/#listprofiletimespaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         period: AggregationPeriodType,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         orderBy: OrderByType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProfileTimesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/paginators/#listprofiletimespaginator)
         """
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/paginator.pyi` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,46 +16,48 @@
     session = get_session()
     with session.create_client("codeguruprofiler") as client:
         client: CodeGuruProfilerClient
 
         list_profile_times_paginator: ListProfileTimesPaginator = client.get_paginator("list_profile_times")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import AggregationPeriodType, OrderByType
-from .type_defs import ListProfileTimesResponseTypeDef, PaginatorConfigTypeDef
+from .type_defs import ListProfileTimesResponseTypeDef, PaginatorConfigTypeDef, TimestampTypeDef
 
 __all__ = ("ListProfileTimesPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListProfileTimesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/paginators/#listprofiletimespaginator)
     """
 
     def paginate(
         self,
         *,
-        endTime: Union[datetime, str],
+        endTime: TimestampTypeDef,
         period: AggregationPeriodType,
         profilingGroupName: str,
-        startTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
         orderBy: OrderByType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProfileTimesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Paginator.ListProfileTimes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/paginators/#listprofiletimespaginator)
         """
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/type_defs.py` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for codeguruprofiler service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_codeguruprofiler.type_defs import ChannelTypeDef
+    from types_aiobotocore_codeguruprofiler.type_defs import ResponseMetadataTypeDef
 
-    data: ChannelTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -33,99 +33,96 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ChannelTypeDef",
+    "ResponseMetadataTypeDef",
     "AgentConfigurationTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
     "MetricTypeDef",
-    "FrameMetricTypeDef",
+    "TimestampTypeDef",
     "TimestampStructureTypeDef",
+    "BlobTypeDef",
+    "ChannelOutputTypeDef",
+    "ChannelTypeDef",
     "ConfigureAgentRequestRequestTypeDef",
     "DeleteProfilingGroupRequestRequestTypeDef",
     "DescribeProfilingGroupRequestRequestTypeDef",
     "FindingsReportSummaryTypeDef",
+    "FrameMetricOutputTypeDef",
+    "FrameMetricTypeDef",
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     "GetNotificationConfigurationRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetPolicyResponseTypeDef",
-    "GetProfileRequestRequestTypeDef",
-    "GetProfileResponseTypeDef",
-    "GetRecommendationsRequestRequestTypeDef",
-    "ListFindingsReportsRequestRequestTypeDef",
-    "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
-    "ListProfileTimesRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ProfileTimeTypeDef",
     "ListProfilingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MatchTypeDef",
-    "PaginatorConfigTypeDef",
     "PatternTypeDef",
-    "PostAgentProfileRequestRequestTypeDef",
     "PutPermissionRequestRequestTypeDef",
-    "PutPermissionResponseTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
-    "RemovePermissionResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AddNotificationChannelsRequestRequestTypeDef",
-    "NotificationConfigurationTypeDef",
+    "GetPolicyResponseTypeDef",
+    "GetProfileResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutPermissionResponseTypeDef",
+    "RemovePermissionResponseTypeDef",
     "ConfigureAgentResponseTypeDef",
     "CreateProfilingGroupRequestRequestTypeDef",
     "UpdateProfilingGroupRequestRequestTypeDef",
     "ProfilingStatusTypeDef",
     "AnomalyInstanceTypeDef",
-    "BatchGetFrameMetricDataRequestRequestTypeDef",
-    "FrameMetricDatumTypeDef",
+    "GetProfileRequestRequestTypeDef",
+    "GetRecommendationsRequestRequestTypeDef",
+    "ListFindingsReportsRequestRequestTypeDef",
+    "ListProfileTimesRequestRequestTypeDef",
+    "PostAgentProfileRequestRequestTypeDef",
+    "NotificationConfigurationTypeDef",
+    "ChannelUnionTypeDef",
     "GetFindingsReportAccountSummaryResponseTypeDef",
     "ListFindingsReportsResponseTypeDef",
+    "FrameMetricDatumTypeDef",
+    "FrameMetricUnionTypeDef",
+    "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
     "ListProfileTimesResponseTypeDef",
     "RecommendationTypeDef",
+    "ProfilingGroupDescriptionTypeDef",
+    "AnomalyTypeDef",
     "AddNotificationChannelsResponseTypeDef",
     "GetNotificationConfigurationResponseTypeDef",
     "RemoveNotificationChannelResponseTypeDef",
-    "ProfilingGroupDescriptionTypeDef",
-    "AnomalyTypeDef",
+    "AddNotificationChannelsRequestRequestTypeDef",
     "BatchGetFrameMetricDataResponseTypeDef",
+    "BatchGetFrameMetricDataRequestRequestTypeDef",
     "CreateProfilingGroupResponseTypeDef",
     "DescribeProfilingGroupResponseTypeDef",
     "ListProfilingGroupsResponseTypeDef",
     "UpdateProfilingGroupResponseTypeDef",
     "GetRecommendationsResponseTypeDef",
 )
 
-_RequiredChannelTypeDef = TypedDict(
-    "_RequiredChannelTypeDef",
-    {
-        "eventPublishers": Sequence[Literal["AnomalyDetection"]],
-        "uri": str,
-    },
-)
-_OptionalChannelTypeDef = TypedDict(
-    "_OptionalChannelTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "id": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
-    pass
-
-
 _RequiredAgentConfigurationTypeDef = TypedDict(
     "_RequiredAgentConfigurationTypeDef",
     {
         "periodInSeconds": int,
         "shouldProfile": bool,
     },
 )
@@ -172,30 +169,63 @@
     {
         "frameName": str,
         "threadStates": List[str],
         "type": Literal["AggregatedRelativeTotalTime"],
     },
 )
 
-FrameMetricTypeDef = TypedDict(
-    "FrameMetricTypeDef",
+TimestampTypeDef = Union[datetime, str]
+TimestampStructureTypeDef = TypedDict(
+    "TimestampStructureTypeDef",
     {
-        "frameName": str,
-        "threadStates": Sequence[str],
-        "type": Literal["AggregatedRelativeTotalTime"],
+        "value": datetime,
     },
 )
 
-TimestampStructureTypeDef = TypedDict(
-    "TimestampStructureTypeDef",
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
+_RequiredChannelOutputTypeDef = TypedDict(
+    "_RequiredChannelOutputTypeDef",
     {
-        "value": datetime,
+        "eventPublishers": List[Literal["AnomalyDetection"]],
+        "uri": str,
+    },
+)
+_OptionalChannelOutputTypeDef = TypedDict(
+    "_OptionalChannelOutputTypeDef",
+    {
+        "id": str,
+    },
+    total=False,
+)
+
+
+class ChannelOutputTypeDef(_RequiredChannelOutputTypeDef, _OptionalChannelOutputTypeDef):
+    pass
+
+
+_RequiredChannelTypeDef = TypedDict(
+    "_RequiredChannelTypeDef",
+    {
+        "eventPublishers": Sequence[Literal["AnomalyDetection"]],
+        "uri": str,
+    },
+)
+_OptionalChannelTypeDef = TypedDict(
+    "_OptionalChannelTypeDef",
+    {
+        "id": str,
     },
+    total=False,
 )
 
+
+class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
+    pass
+
+
 _RequiredConfigureAgentRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAgentRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
 _OptionalConfigureAgentRequestRequestTypeDef = TypedDict(
@@ -236,184 +266,66 @@
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "totalNumberOfFindings": int,
     },
     total=False,
 )
 
-GetFindingsReportAccountSummaryRequestRequestTypeDef = TypedDict(
-    "GetFindingsReportAccountSummaryRequestRequestTypeDef",
-    {
-        "dailyReportsOnly": bool,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-GetNotificationConfigurationRequestRequestTypeDef = TypedDict(
-    "GetNotificationConfigurationRequestRequestTypeDef",
-    {
-        "profilingGroupName": str,
-    },
-)
-
-GetPolicyRequestRequestTypeDef = TypedDict(
-    "GetPolicyRequestRequestTypeDef",
-    {
-        "profilingGroupName": str,
-    },
-)
-
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredGetProfileRequestRequestTypeDef",
-    {
-        "profilingGroupName": str,
-    },
-)
-_OptionalGetProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalGetProfileRequestRequestTypeDef",
-    {
-        "accept": str,
-        "endTime": Union[datetime, str],
-        "maxDepth": int,
-        "period": str,
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class GetProfileRequestRequestTypeDef(
-    _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
-):
-    pass
-
-
-GetProfileResponseTypeDef = TypedDict(
-    "GetProfileResponseTypeDef",
+FrameMetricOutputTypeDef = TypedDict(
+    "FrameMetricOutputTypeDef",
     {
-        "contentEncoding": str,
-        "contentType": str,
-        "profile": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "frameName": str,
+        "threadStates": List[str],
+        "type": Literal["AggregatedRelativeTotalTime"],
     },
 )
 
-_RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetRecommendationsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalGetRecommendationsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetRecommendationsRequestRequestTypeDef",
+FrameMetricTypeDef = TypedDict(
+    "FrameMetricTypeDef",
     {
-        "locale": str,
+        "frameName": str,
+        "threadStates": Sequence[str],
+        "type": Literal["AggregatedRelativeTotalTime"],
     },
-    total=False,
 )
 
-
-class GetRecommendationsRequestRequestTypeDef(
-    _RequiredGetRecommendationsRequestRequestTypeDef,
-    _OptionalGetRecommendationsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredListFindingsReportsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFindingsReportsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListFindingsReportsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFindingsReportsRequestRequestTypeDef",
+GetFindingsReportAccountSummaryRequestRequestTypeDef = TypedDict(
+    "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     {
         "dailyReportsOnly": bool,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
-class ListFindingsReportsRequestRequestTypeDef(
-    _RequiredListFindingsReportsRequestRequestTypeDef,
-    _OptionalListFindingsReportsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
-    "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
+GetNotificationConfigurationRequestRequestTypeDef = TypedDict(
+    "GetNotificationConfigurationRequestRequestTypeDef",
     {
-        "endTime": Union[datetime, str],
-        "period": AggregationPeriodType,
         "profilingGroupName": str,
-        "startTime": Union[datetime, str],
     },
 )
-_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
-    "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
-    {
-        "orderBy": OrderByType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
-    _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
-    _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
-):
-    pass
 
-
-_RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
-    "_RequiredListProfileTimesRequestRequestTypeDef",
+GetPolicyRequestRequestTypeDef = TypedDict(
+    "GetPolicyRequestRequestTypeDef",
     {
-        "endTime": Union[datetime, str],
-        "period": AggregationPeriodType,
         "profilingGroupName": str,
-        "startTime": Union[datetime, str],
     },
 )
-_OptionalListProfileTimesRequestRequestTypeDef = TypedDict(
-    "_OptionalListProfileTimesRequestRequestTypeDef",
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "orderBy": OrderByType,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListProfileTimesRequestRequestTypeDef(
-    _RequiredListProfileTimesRequestRequestTypeDef, _OptionalListProfileTimesRequestRequestTypeDef
-):
-    pass
-
-
 ProfileTimeTypeDef = TypedDict(
     "ProfileTimeTypeDef",
     {
         "start": datetime,
     },
     total=False,
 )
@@ -431,79 +343,38 @@
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
 MatchTypeDef = TypedDict(
     "MatchTypeDef",
     {
         "frameAddress": str,
         "targetFramesIndex": int,
         "thresholdBreachValue": float,
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
 PatternTypeDef = TypedDict(
     "PatternTypeDef",
     {
         "countersToAggregate": List[str],
         "description": str,
         "id": str,
         "name": str,
         "resolutionSteps": str,
         "targetFrames": List[List[str]],
         "thresholdPercent": float,
     },
     total=False,
 )
 
-_RequiredPostAgentProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredPostAgentProfileRequestRequestTypeDef",
-    {
-        "agentProfile": Union[str, bytes, IO[Any], StreamingBody],
-        "contentType": str,
-        "profilingGroupName": str,
-    },
-)
-_OptionalPostAgentProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalPostAgentProfileRequestRequestTypeDef",
-    {
-        "profileToken": str,
-    },
-    total=False,
-)
-
-
-class PostAgentProfileRequestRequestTypeDef(
-    _RequiredPostAgentProfileRequestRequestTypeDef, _OptionalPostAgentProfileRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredPutPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredPutPermissionRequestRequestTypeDef",
     {
         "actionGroup": Literal["agentPermissions"],
         "principals": Sequence[str],
         "profilingGroupName": str,
     },
@@ -519,23 +390,14 @@
 
 class PutPermissionRequestRequestTypeDef(
     _RequiredPutPermissionRequestRequestTypeDef, _OptionalPutPermissionRequestRequestTypeDef
 ):
     pass
 
 
-PutPermissionResponseTypeDef = TypedDict(
-    "PutPermissionResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveNotificationChannelRequestRequestTypeDef = TypedDict(
     "RemoveNotificationChannelRequestRequestTypeDef",
     {
         "channelId": str,
         "profilingGroupName": str,
     },
 )
@@ -545,34 +407,14 @@
     {
         "actionGroup": Literal["agentPermissions"],
         "profilingGroupName": str,
         "revisionId": str,
     },
 )
 
-RemovePermissionResponseTypeDef = TypedDict(
-    "RemovePermissionResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
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
 _RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitFeedbackRequestRequestTypeDef",
     {
         "anomalyInstanceId": str,
         "profilingGroupName": str,
         "type": FeedbackTypeType,
     },
@@ -604,35 +446,64 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-AddNotificationChannelsRequestRequestTypeDef = TypedDict(
-    "AddNotificationChannelsRequestRequestTypeDef",
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
     {
-        "channels": Sequence[ChannelTypeDef],
-        "profilingGroupName": str,
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NotificationConfigurationTypeDef = TypedDict(
-    "NotificationConfigurationTypeDef",
+GetProfileResponseTypeDef = TypedDict(
+    "GetProfileResponseTypeDef",
     {
-        "channels": List[ChannelTypeDef],
+        "contentEncoding": str,
+        "contentType": str,
+        "profile": StreamingBody,
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
+PutPermissionResponseTypeDef = TypedDict(
+    "PutPermissionResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemovePermissionResponseTypeDef = TypedDict(
+    "RemovePermissionResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ConfigureAgentResponseTypeDef = TypedDict(
     "ConfigureAgentResponseTypeDef",
     {
         "configuration": AgentConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProfilingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfilingGroupRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -692,72 +563,206 @@
 )
 
 
 class AnomalyInstanceTypeDef(_RequiredAnomalyInstanceTypeDef, _OptionalAnomalyInstanceTypeDef):
     pass
 
 
-_RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
+_RequiredGetProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredGetProfileRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
-_OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetFrameMetricDataRequestRequestTypeDef",
+_OptionalGetProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalGetProfileRequestRequestTypeDef",
     {
-        "endTime": Union[datetime, str],
-        "frameMetrics": Sequence[FrameMetricTypeDef],
+        "accept": str,
+        "endTime": TimestampTypeDef,
+        "maxDepth": int,
         "period": str,
-        "startTime": Union[datetime, str],
-        "targetResolution": AggregationPeriodType,
+        "startTime": TimestampTypeDef,
     },
     total=False,
 )
 
 
-class BatchGetFrameMetricDataRequestRequestTypeDef(
-    _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
-    _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
+class GetProfileRequestRequestTypeDef(
+    _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
 ):
     pass
 
 
-FrameMetricDatumTypeDef = TypedDict(
-    "FrameMetricDatumTypeDef",
+_RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetRecommendationsRequestRequestTypeDef",
     {
-        "frameMetric": FrameMetricTypeDef,
-        "values": List[float],
+        "endTime": TimestampTypeDef,
+        "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalGetRecommendationsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetRecommendationsRequestRequestTypeDef",
+    {
+        "locale": str,
     },
+    total=False,
 )
 
+
+class GetRecommendationsRequestRequestTypeDef(
+    _RequiredGetRecommendationsRequestRequestTypeDef,
+    _OptionalGetRecommendationsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListFindingsReportsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFindingsReportsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalListFindingsReportsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFindingsReportsRequestRequestTypeDef",
+    {
+        "dailyReportsOnly": bool,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+
+class ListFindingsReportsRequestRequestTypeDef(
+    _RequiredListFindingsReportsRequestRequestTypeDef,
+    _OptionalListFindingsReportsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
+    "_RequiredListProfileTimesRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "period": AggregationPeriodType,
+        "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalListProfileTimesRequestRequestTypeDef = TypedDict(
+    "_OptionalListProfileTimesRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "orderBy": OrderByType,
+    },
+    total=False,
+)
+
+
+class ListProfileTimesRequestRequestTypeDef(
+    _RequiredListProfileTimesRequestRequestTypeDef, _OptionalListProfileTimesRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredPostAgentProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredPostAgentProfileRequestRequestTypeDef",
+    {
+        "agentProfile": BlobTypeDef,
+        "contentType": str,
+        "profilingGroupName": str,
+    },
+)
+_OptionalPostAgentProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalPostAgentProfileRequestRequestTypeDef",
+    {
+        "profileToken": str,
+    },
+    total=False,
+)
+
+
+class PostAgentProfileRequestRequestTypeDef(
+    _RequiredPostAgentProfileRequestRequestTypeDef, _OptionalPostAgentProfileRequestRequestTypeDef
+):
+    pass
+
+
+NotificationConfigurationTypeDef = TypedDict(
+    "NotificationConfigurationTypeDef",
+    {
+        "channels": List[ChannelOutputTypeDef],
+    },
+    total=False,
+)
+
+ChannelUnionTypeDef = Union[ChannelTypeDef, ChannelOutputTypeDef]
 GetFindingsReportAccountSummaryResponseTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryResponseTypeDef",
     {
         "nextToken": str,
         "reportSummaries": List[FindingsReportSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingsReportsResponseTypeDef = TypedDict(
     "ListFindingsReportsResponseTypeDef",
     {
         "findingsReportSummaries": List[FindingsReportSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FrameMetricDatumTypeDef = TypedDict(
+    "FrameMetricDatumTypeDef",
+    {
+        "frameMetric": FrameMetricOutputTypeDef,
+        "values": List[float],
     },
 )
 
+FrameMetricUnionTypeDef = Union[FrameMetricTypeDef, FrameMetricOutputTypeDef]
+_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
+    "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "period": AggregationPeriodType,
+        "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
+    "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
+    {
+        "orderBy": OrderByType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
+    _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
+    _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
+):
+    pass
+
+
 ListProfileTimesResponseTypeDef = TypedDict(
     "ListProfileTimesResponseTypeDef",
     {
         "nextToken": str,
         "profileTimes": List[ProfileTimeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "allMatchesCount": int,
@@ -765,113 +770,147 @@
         "endTime": datetime,
         "pattern": PatternTypeDef,
         "startTime": datetime,
         "topMatches": List[MatchTypeDef],
     },
 )
 
+ProfilingGroupDescriptionTypeDef = TypedDict(
+    "ProfilingGroupDescriptionTypeDef",
+    {
+        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
+        "arn": str,
+        "computePlatform": ComputePlatformType,
+        "createdAt": datetime,
+        "name": str,
+        "profilingStatus": ProfilingStatusTypeDef,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+    },
+    total=False,
+)
+
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
+    {
+        "instances": List[AnomalyInstanceTypeDef],
+        "metric": MetricTypeDef,
+        "reason": str,
+    },
+)
+
 AddNotificationChannelsResponseTypeDef = TypedDict(
     "AddNotificationChannelsResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNotificationConfigurationResponseTypeDef = TypedDict(
     "GetNotificationConfigurationResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveNotificationChannelResponseTypeDef = TypedDict(
     "RemoveNotificationChannelResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProfilingGroupDescriptionTypeDef = TypedDict(
-    "ProfilingGroupDescriptionTypeDef",
-    {
-        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
-        "arn": str,
-        "computePlatform": ComputePlatformType,
-        "createdAt": datetime,
-        "name": str,
-        "profilingStatus": ProfilingStatusTypeDef,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
+AddNotificationChannelsRequestRequestTypeDef = TypedDict(
+    "AddNotificationChannelsRequestRequestTypeDef",
     {
-        "instances": List[AnomalyInstanceTypeDef],
-        "metric": MetricTypeDef,
-        "reason": str,
+        "channels": Sequence[ChannelUnionTypeDef],
+        "profilingGroupName": str,
     },
 )
 
 BatchGetFrameMetricDataResponseTypeDef = TypedDict(
     "BatchGetFrameMetricDataResponseTypeDef",
     {
         "endTime": datetime,
         "endTimes": List[TimestampStructureTypeDef],
         "frameMetricData": List[FrameMetricDatumTypeDef],
         "resolution": AggregationPeriodType,
         "startTime": datetime,
         "unprocessedEndTimes": Dict[str, List[TimestampStructureTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
+    {
+        "profilingGroupName": str,
+    },
+)
+_OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetFrameMetricDataRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "frameMetrics": Sequence[FrameMetricUnionTypeDef],
+        "period": str,
+        "startTime": TimestampTypeDef,
+        "targetResolution": AggregationPeriodType,
+    },
+    total=False,
+)
+
+
+class BatchGetFrameMetricDataRequestRequestTypeDef(
+    _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
+    _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
+):
+    pass
+
+
 CreateProfilingGroupResponseTypeDef = TypedDict(
     "CreateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProfilingGroupResponseTypeDef = TypedDict(
     "DescribeProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfilingGroupsResponseTypeDef = TypedDict(
     "ListProfilingGroupsResponseTypeDef",
     {
         "nextToken": str,
         "profilingGroupNames": List[str],
         "profilingGroups": List[ProfilingGroupDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProfilingGroupResponseTypeDef = TypedDict(
     "UpdateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "anomalies": List[AnomalyTypeDef],
         "profileEndTime": datetime,
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler/type_defs.pyi` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for codeguruprofiler service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_codeguruprofiler.type_defs import ChannelTypeDef
+    from types_aiobotocore_codeguruprofiler.type_defs import ResponseMetadataTypeDef
 
-    data: ChannelTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -32,97 +32,96 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ChannelTypeDef",
+    "ResponseMetadataTypeDef",
     "AgentConfigurationTypeDef",
     "AgentOrchestrationConfigTypeDef",
     "AggregatedProfileTimeTypeDef",
     "UserFeedbackTypeDef",
     "MetricTypeDef",
-    "FrameMetricTypeDef",
+    "TimestampTypeDef",
     "TimestampStructureTypeDef",
+    "BlobTypeDef",
+    "ChannelOutputTypeDef",
+    "ChannelTypeDef",
     "ConfigureAgentRequestRequestTypeDef",
     "DeleteProfilingGroupRequestRequestTypeDef",
     "DescribeProfilingGroupRequestRequestTypeDef",
     "FindingsReportSummaryTypeDef",
+    "FrameMetricOutputTypeDef",
+    "FrameMetricTypeDef",
     "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     "GetNotificationConfigurationRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetPolicyResponseTypeDef",
-    "GetProfileRequestRequestTypeDef",
-    "GetProfileResponseTypeDef",
-    "GetRecommendationsRequestRequestTypeDef",
-    "ListFindingsReportsRequestRequestTypeDef",
-    "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
-    "ListProfileTimesRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "ProfileTimeTypeDef",
     "ListProfilingGroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MatchTypeDef",
-    "PaginatorConfigTypeDef",
     "PatternTypeDef",
-    "PostAgentProfileRequestRequestTypeDef",
     "PutPermissionRequestRequestTypeDef",
-    "PutPermissionResponseTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
-    "RemovePermissionResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SubmitFeedbackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AddNotificationChannelsRequestRequestTypeDef",
-    "NotificationConfigurationTypeDef",
+    "GetPolicyResponseTypeDef",
+    "GetProfileResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutPermissionResponseTypeDef",
+    "RemovePermissionResponseTypeDef",
     "ConfigureAgentResponseTypeDef",
     "CreateProfilingGroupRequestRequestTypeDef",
     "UpdateProfilingGroupRequestRequestTypeDef",
     "ProfilingStatusTypeDef",
     "AnomalyInstanceTypeDef",
-    "BatchGetFrameMetricDataRequestRequestTypeDef",
-    "FrameMetricDatumTypeDef",
+    "GetProfileRequestRequestTypeDef",
+    "GetRecommendationsRequestRequestTypeDef",
+    "ListFindingsReportsRequestRequestTypeDef",
+    "ListProfileTimesRequestRequestTypeDef",
+    "PostAgentProfileRequestRequestTypeDef",
+    "NotificationConfigurationTypeDef",
+    "ChannelUnionTypeDef",
     "GetFindingsReportAccountSummaryResponseTypeDef",
     "ListFindingsReportsResponseTypeDef",
+    "FrameMetricDatumTypeDef",
+    "FrameMetricUnionTypeDef",
+    "ListProfileTimesRequestListProfileTimesPaginateTypeDef",
     "ListProfileTimesResponseTypeDef",
     "RecommendationTypeDef",
+    "ProfilingGroupDescriptionTypeDef",
+    "AnomalyTypeDef",
     "AddNotificationChannelsResponseTypeDef",
     "GetNotificationConfigurationResponseTypeDef",
     "RemoveNotificationChannelResponseTypeDef",
-    "ProfilingGroupDescriptionTypeDef",
-    "AnomalyTypeDef",
+    "AddNotificationChannelsRequestRequestTypeDef",
     "BatchGetFrameMetricDataResponseTypeDef",
+    "BatchGetFrameMetricDataRequestRequestTypeDef",
     "CreateProfilingGroupResponseTypeDef",
     "DescribeProfilingGroupResponseTypeDef",
     "ListProfilingGroupsResponseTypeDef",
     "UpdateProfilingGroupResponseTypeDef",
     "GetRecommendationsResponseTypeDef",
 )
 
-_RequiredChannelTypeDef = TypedDict(
-    "_RequiredChannelTypeDef",
-    {
-        "eventPublishers": Sequence[Literal["AnomalyDetection"]],
-        "uri": str,
-    },
-)
-_OptionalChannelTypeDef = TypedDict(
-    "_OptionalChannelTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "id": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
-    pass
-
 _RequiredAgentConfigurationTypeDef = TypedDict(
     "_RequiredAgentConfigurationTypeDef",
     {
         "periodInSeconds": int,
         "shouldProfile": bool,
     },
 )
@@ -167,29 +166,58 @@
     {
         "frameName": str,
         "threadStates": List[str],
         "type": Literal["AggregatedRelativeTotalTime"],
     },
 )
 
-FrameMetricTypeDef = TypedDict(
-    "FrameMetricTypeDef",
+TimestampTypeDef = Union[datetime, str]
+TimestampStructureTypeDef = TypedDict(
+    "TimestampStructureTypeDef",
     {
-        "frameName": str,
-        "threadStates": Sequence[str],
-        "type": Literal["AggregatedRelativeTotalTime"],
+        "value": datetime,
     },
 )
 
-TimestampStructureTypeDef = TypedDict(
-    "TimestampStructureTypeDef",
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
+_RequiredChannelOutputTypeDef = TypedDict(
+    "_RequiredChannelOutputTypeDef",
     {
-        "value": datetime,
+        "eventPublishers": List[Literal["AnomalyDetection"]],
+        "uri": str,
+    },
+)
+_OptionalChannelOutputTypeDef = TypedDict(
+    "_OptionalChannelOutputTypeDef",
+    {
+        "id": str,
+    },
+    total=False,
+)
+
+class ChannelOutputTypeDef(_RequiredChannelOutputTypeDef, _OptionalChannelOutputTypeDef):
+    pass
+
+_RequiredChannelTypeDef = TypedDict(
+    "_RequiredChannelTypeDef",
+    {
+        "eventPublishers": Sequence[Literal["AnomalyDetection"]],
+        "uri": str,
     },
 )
+_OptionalChannelTypeDef = TypedDict(
+    "_OptionalChannelTypeDef",
+    {
+        "id": str,
+    },
+    total=False,
+)
+
+class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
+    pass
 
 _RequiredConfigureAgentRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAgentRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
@@ -229,174 +257,66 @@
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "totalNumberOfFindings": int,
     },
     total=False,
 )
 
-GetFindingsReportAccountSummaryRequestRequestTypeDef = TypedDict(
-    "GetFindingsReportAccountSummaryRequestRequestTypeDef",
-    {
-        "dailyReportsOnly": bool,
-        "maxResults": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-GetNotificationConfigurationRequestRequestTypeDef = TypedDict(
-    "GetNotificationConfigurationRequestRequestTypeDef",
-    {
-        "profilingGroupName": str,
-    },
-)
-
-GetPolicyRequestRequestTypeDef = TypedDict(
-    "GetPolicyRequestRequestTypeDef",
-    {
-        "profilingGroupName": str,
-    },
-)
-
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
+FrameMetricOutputTypeDef = TypedDict(
+    "FrameMetricOutputTypeDef",
     {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredGetProfileRequestRequestTypeDef",
-    {
-        "profilingGroupName": str,
-    },
-)
-_OptionalGetProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalGetProfileRequestRequestTypeDef",
-    {
-        "accept": str,
-        "endTime": Union[datetime, str],
-        "maxDepth": int,
-        "period": str,
-        "startTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class GetProfileRequestRequestTypeDef(
-    _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
-):
-    pass
-
-GetProfileResponseTypeDef = TypedDict(
-    "GetProfileResponseTypeDef",
-    {
-        "contentEncoding": str,
-        "contentType": str,
-        "profile": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "frameName": str,
+        "threadStates": List[str],
+        "type": Literal["AggregatedRelativeTotalTime"],
     },
 )
 
-_RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetRecommendationsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalGetRecommendationsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetRecommendationsRequestRequestTypeDef",
+FrameMetricTypeDef = TypedDict(
+    "FrameMetricTypeDef",
     {
-        "locale": str,
+        "frameName": str,
+        "threadStates": Sequence[str],
+        "type": Literal["AggregatedRelativeTotalTime"],
     },
-    total=False,
 )
 
-class GetRecommendationsRequestRequestTypeDef(
-    _RequiredGetRecommendationsRequestRequestTypeDef,
-    _OptionalGetRecommendationsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredListFindingsReportsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFindingsReportsRequestRequestTypeDef",
-    {
-        "endTime": Union[datetime, str],
-        "profilingGroupName": str,
-        "startTime": Union[datetime, str],
-    },
-)
-_OptionalListFindingsReportsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFindingsReportsRequestRequestTypeDef",
+GetFindingsReportAccountSummaryRequestRequestTypeDef = TypedDict(
+    "GetFindingsReportAccountSummaryRequestRequestTypeDef",
     {
         "dailyReportsOnly": bool,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-class ListFindingsReportsRequestRequestTypeDef(
-    _RequiredListFindingsReportsRequestRequestTypeDef,
-    _OptionalListFindingsReportsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
-    "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
+GetNotificationConfigurationRequestRequestTypeDef = TypedDict(
+    "GetNotificationConfigurationRequestRequestTypeDef",
     {
-        "endTime": Union[datetime, str],
-        "period": AggregationPeriodType,
         "profilingGroupName": str,
-        "startTime": Union[datetime, str],
     },
 )
-_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
-    "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
-    {
-        "orderBy": OrderByType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
-class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
-    _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
-    _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
-):
-    pass
-
-_RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
-    "_RequiredListProfileTimesRequestRequestTypeDef",
+GetPolicyRequestRequestTypeDef = TypedDict(
+    "GetPolicyRequestRequestTypeDef",
     {
-        "endTime": Union[datetime, str],
-        "period": AggregationPeriodType,
         "profilingGroupName": str,
-        "startTime": Union[datetime, str],
     },
 )
-_OptionalListProfileTimesRequestRequestTypeDef = TypedDict(
-    "_OptionalListProfileTimesRequestRequestTypeDef",
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "maxResults": int,
-        "nextToken": str,
-        "orderBy": OrderByType,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListProfileTimesRequestRequestTypeDef(
-    _RequiredListProfileTimesRequestRequestTypeDef, _OptionalListProfileTimesRequestRequestTypeDef
-):
-    pass
-
 ProfileTimeTypeDef = TypedDict(
     "ProfileTimeTypeDef",
     {
         "start": datetime,
     },
     total=False,
 )
@@ -414,77 +334,38 @@
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
 MatchTypeDef = TypedDict(
     "MatchTypeDef",
     {
         "frameAddress": str,
         "targetFramesIndex": int,
         "thresholdBreachValue": float,
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
 PatternTypeDef = TypedDict(
     "PatternTypeDef",
     {
         "countersToAggregate": List[str],
         "description": str,
         "id": str,
         "name": str,
         "resolutionSteps": str,
         "targetFrames": List[List[str]],
         "thresholdPercent": float,
     },
     total=False,
 )
 
-_RequiredPostAgentProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredPostAgentProfileRequestRequestTypeDef",
-    {
-        "agentProfile": Union[str, bytes, IO[Any], StreamingBody],
-        "contentType": str,
-        "profilingGroupName": str,
-    },
-)
-_OptionalPostAgentProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalPostAgentProfileRequestRequestTypeDef",
-    {
-        "profileToken": str,
-    },
-    total=False,
-)
-
-class PostAgentProfileRequestRequestTypeDef(
-    _RequiredPostAgentProfileRequestRequestTypeDef, _OptionalPostAgentProfileRequestRequestTypeDef
-):
-    pass
-
 _RequiredPutPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredPutPermissionRequestRequestTypeDef",
     {
         "actionGroup": Literal["agentPermissions"],
         "principals": Sequence[str],
         "profilingGroupName": str,
     },
@@ -498,23 +379,14 @@
 )
 
 class PutPermissionRequestRequestTypeDef(
     _RequiredPutPermissionRequestRequestTypeDef, _OptionalPutPermissionRequestRequestTypeDef
 ):
     pass
 
-PutPermissionResponseTypeDef = TypedDict(
-    "PutPermissionResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveNotificationChannelRequestRequestTypeDef = TypedDict(
     "RemoveNotificationChannelRequestRequestTypeDef",
     {
         "channelId": str,
         "profilingGroupName": str,
     },
 )
@@ -524,34 +396,14 @@
     {
         "actionGroup": Literal["agentPermissions"],
         "profilingGroupName": str,
         "revisionId": str,
     },
 )
 
-RemovePermissionResponseTypeDef = TypedDict(
-    "RemovePermissionResponseTypeDef",
-    {
-        "policy": str,
-        "revisionId": str,
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
 _RequiredSubmitFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredSubmitFeedbackRequestRequestTypeDef",
     {
         "anomalyInstanceId": str,
         "profilingGroupName": str,
         "type": FeedbackTypeType,
     },
@@ -581,35 +433,64 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-AddNotificationChannelsRequestRequestTypeDef = TypedDict(
-    "AddNotificationChannelsRequestRequestTypeDef",
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
     {
-        "channels": Sequence[ChannelTypeDef],
-        "profilingGroupName": str,
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NotificationConfigurationTypeDef = TypedDict(
-    "NotificationConfigurationTypeDef",
+GetProfileResponseTypeDef = TypedDict(
+    "GetProfileResponseTypeDef",
     {
-        "channels": List[ChannelTypeDef],
+        "contentEncoding": str,
+        "contentType": str,
+        "profile": StreamingBody,
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
+PutPermissionResponseTypeDef = TypedDict(
+    "PutPermissionResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemovePermissionResponseTypeDef = TypedDict(
+    "RemovePermissionResponseTypeDef",
+    {
+        "policy": str,
+        "revisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ConfigureAgentResponseTypeDef = TypedDict(
     "ConfigureAgentResponseTypeDef",
     {
         "configuration": AgentConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProfilingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfilingGroupRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -665,70 +546,194 @@
     },
     total=False,
 )
 
 class AnomalyInstanceTypeDef(_RequiredAnomalyInstanceTypeDef, _OptionalAnomalyInstanceTypeDef):
     pass
 
-_RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
-    "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
+_RequiredGetProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredGetProfileRequestRequestTypeDef",
     {
         "profilingGroupName": str,
     },
 )
-_OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
-    "_OptionalBatchGetFrameMetricDataRequestRequestTypeDef",
+_OptionalGetProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalGetProfileRequestRequestTypeDef",
     {
-        "endTime": Union[datetime, str],
-        "frameMetrics": Sequence[FrameMetricTypeDef],
+        "accept": str,
+        "endTime": TimestampTypeDef,
+        "maxDepth": int,
         "period": str,
-        "startTime": Union[datetime, str],
-        "targetResolution": AggregationPeriodType,
+        "startTime": TimestampTypeDef,
     },
     total=False,
 )
 
-class BatchGetFrameMetricDataRequestRequestTypeDef(
-    _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
-    _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
+class GetProfileRequestRequestTypeDef(
+    _RequiredGetProfileRequestRequestTypeDef, _OptionalGetProfileRequestRequestTypeDef
 ):
     pass
 
-FrameMetricDatumTypeDef = TypedDict(
-    "FrameMetricDatumTypeDef",
+_RequiredGetRecommendationsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetRecommendationsRequestRequestTypeDef",
     {
-        "frameMetric": FrameMetricTypeDef,
-        "values": List[float],
+        "endTime": TimestampTypeDef,
+        "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalGetRecommendationsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetRecommendationsRequestRequestTypeDef",
+    {
+        "locale": str,
+    },
+    total=False,
+)
+
+class GetRecommendationsRequestRequestTypeDef(
+    _RequiredGetRecommendationsRequestRequestTypeDef,
+    _OptionalGetRecommendationsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListFindingsReportsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFindingsReportsRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalListFindingsReportsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFindingsReportsRequestRequestTypeDef",
+    {
+        "dailyReportsOnly": bool,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+class ListFindingsReportsRequestRequestTypeDef(
+    _RequiredListFindingsReportsRequestRequestTypeDef,
+    _OptionalListFindingsReportsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredListProfileTimesRequestRequestTypeDef = TypedDict(
+    "_RequiredListProfileTimesRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "period": AggregationPeriodType,
+        "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
+    },
+)
+_OptionalListProfileTimesRequestRequestTypeDef = TypedDict(
+    "_OptionalListProfileTimesRequestRequestTypeDef",
+    {
+        "maxResults": int,
+        "nextToken": str,
+        "orderBy": OrderByType,
+    },
+    total=False,
+)
+
+class ListProfileTimesRequestRequestTypeDef(
+    _RequiredListProfileTimesRequestRequestTypeDef, _OptionalListProfileTimesRequestRequestTypeDef
+):
+    pass
+
+_RequiredPostAgentProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredPostAgentProfileRequestRequestTypeDef",
+    {
+        "agentProfile": BlobTypeDef,
+        "contentType": str,
+        "profilingGroupName": str,
+    },
+)
+_OptionalPostAgentProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalPostAgentProfileRequestRequestTypeDef",
+    {
+        "profileToken": str,
+    },
+    total=False,
+)
+
+class PostAgentProfileRequestRequestTypeDef(
+    _RequiredPostAgentProfileRequestRequestTypeDef, _OptionalPostAgentProfileRequestRequestTypeDef
+):
+    pass
+
+NotificationConfigurationTypeDef = TypedDict(
+    "NotificationConfigurationTypeDef",
+    {
+        "channels": List[ChannelOutputTypeDef],
     },
+    total=False,
 )
 
+ChannelUnionTypeDef = Union[ChannelTypeDef, ChannelOutputTypeDef]
 GetFindingsReportAccountSummaryResponseTypeDef = TypedDict(
     "GetFindingsReportAccountSummaryResponseTypeDef",
     {
         "nextToken": str,
         "reportSummaries": List[FindingsReportSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingsReportsResponseTypeDef = TypedDict(
     "ListFindingsReportsResponseTypeDef",
     {
         "findingsReportSummaries": List[FindingsReportSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FrameMetricDatumTypeDef = TypedDict(
+    "FrameMetricDatumTypeDef",
+    {
+        "frameMetric": FrameMetricOutputTypeDef,
+        "values": List[float],
+    },
+)
+
+FrameMetricUnionTypeDef = Union[FrameMetricTypeDef, FrameMetricOutputTypeDef]
+_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
+    "_RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "period": AggregationPeriodType,
+        "profilingGroupName": str,
+        "startTime": TimestampTypeDef,
     },
 )
+_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef = TypedDict(
+    "_OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef",
+    {
+        "orderBy": OrderByType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListProfileTimesRequestListProfileTimesPaginateTypeDef(
+    _RequiredListProfileTimesRequestListProfileTimesPaginateTypeDef,
+    _OptionalListProfileTimesRequestListProfileTimesPaginateTypeDef,
+):
+    pass
 
 ListProfileTimesResponseTypeDef = TypedDict(
     "ListProfileTimesResponseTypeDef",
     {
         "nextToken": str,
         "profileTimes": List[ProfileTimeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "allMatchesCount": int,
@@ -736,113 +741,145 @@
         "endTime": datetime,
         "pattern": PatternTypeDef,
         "startTime": datetime,
         "topMatches": List[MatchTypeDef],
     },
 )
 
+ProfilingGroupDescriptionTypeDef = TypedDict(
+    "ProfilingGroupDescriptionTypeDef",
+    {
+        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
+        "arn": str,
+        "computePlatform": ComputePlatformType,
+        "createdAt": datetime,
+        "name": str,
+        "profilingStatus": ProfilingStatusTypeDef,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+    },
+    total=False,
+)
+
+AnomalyTypeDef = TypedDict(
+    "AnomalyTypeDef",
+    {
+        "instances": List[AnomalyInstanceTypeDef],
+        "metric": MetricTypeDef,
+        "reason": str,
+    },
+)
+
 AddNotificationChannelsResponseTypeDef = TypedDict(
     "AddNotificationChannelsResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNotificationConfigurationResponseTypeDef = TypedDict(
     "GetNotificationConfigurationResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveNotificationChannelResponseTypeDef = TypedDict(
     "RemoveNotificationChannelResponseTypeDef",
     {
         "notificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProfilingGroupDescriptionTypeDef = TypedDict(
-    "ProfilingGroupDescriptionTypeDef",
-    {
-        "agentOrchestrationConfig": AgentOrchestrationConfigTypeDef,
-        "arn": str,
-        "computePlatform": ComputePlatformType,
-        "createdAt": datetime,
-        "name": str,
-        "profilingStatus": ProfilingStatusTypeDef,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-    },
-    total=False,
-)
-
-AnomalyTypeDef = TypedDict(
-    "AnomalyTypeDef",
+AddNotificationChannelsRequestRequestTypeDef = TypedDict(
+    "AddNotificationChannelsRequestRequestTypeDef",
     {
-        "instances": List[AnomalyInstanceTypeDef],
-        "metric": MetricTypeDef,
-        "reason": str,
+        "channels": Sequence[ChannelUnionTypeDef],
+        "profilingGroupName": str,
     },
 )
 
 BatchGetFrameMetricDataResponseTypeDef = TypedDict(
     "BatchGetFrameMetricDataResponseTypeDef",
     {
         "endTime": datetime,
         "endTimes": List[TimestampStructureTypeDef],
         "frameMetricData": List[FrameMetricDatumTypeDef],
         "resolution": AggregationPeriodType,
         "startTime": datetime,
         "unprocessedEndTimes": Dict[str, List[TimestampStructureTypeDef]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
+    "_RequiredBatchGetFrameMetricDataRequestRequestTypeDef",
+    {
+        "profilingGroupName": str,
+    },
+)
+_OptionalBatchGetFrameMetricDataRequestRequestTypeDef = TypedDict(
+    "_OptionalBatchGetFrameMetricDataRequestRequestTypeDef",
+    {
+        "endTime": TimestampTypeDef,
+        "frameMetrics": Sequence[FrameMetricUnionTypeDef],
+        "period": str,
+        "startTime": TimestampTypeDef,
+        "targetResolution": AggregationPeriodType,
+    },
+    total=False,
+)
+
+class BatchGetFrameMetricDataRequestRequestTypeDef(
+    _RequiredBatchGetFrameMetricDataRequestRequestTypeDef,
+    _OptionalBatchGetFrameMetricDataRequestRequestTypeDef,
+):
+    pass
+
 CreateProfilingGroupResponseTypeDef = TypedDict(
     "CreateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProfilingGroupResponseTypeDef = TypedDict(
     "DescribeProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProfilingGroupsResponseTypeDef = TypedDict(
     "ListProfilingGroupsResponseTypeDef",
     {
         "nextToken": str,
         "profilingGroupNames": List[str],
         "profilingGroups": List[ProfilingGroupDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProfilingGroupResponseTypeDef = TypedDict(
     "UpdateProfilingGroupResponseTypeDef",
     {
         "profilingGroup": ProfilingGroupDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationsResponseTypeDef = TypedDict(
     "GetRecommendationsResponseTypeDef",
     {
         "anomalies": List[AnomalyTypeDef],
         "profileEndTime": datetime,
         "profileStartTime": datetime,
         "profilingGroupName": str,
         "recommendations": List[RecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler.egg-info/PKG-INFO` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-codeguruprofiler
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CodeGuruProfiler 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codeguruprofiler type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codeguruprofiler"></a>
 
 # types-aiobotocore-codeguruprofiler
 
 [![PyPI - types-aiobotocore-codeguruprofiler](https://img.shields.io/pypi/v/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguruprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguruprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-codeguruprofiler?color=blue)](https://pypistats.org/packages/types-aiobotocore-codeguruprofiler)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-codeguruprofiler)](https://pepy.tech/project/types-aiobotocore-codeguruprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CodeGuruProfiler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
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
 [types-aiobotocore-codeguruprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguruprofiler/).
 
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
@@ -315,90 +282,96 @@
 )
 
 
 def check_value(value: ActionGroupType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_codeguruprofiler.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_codeguruprofiler.type_defs import (
-    ChannelTypeDef,
+    ResponseMetadataTypeDef,
     AgentConfigurationTypeDef,
     AgentOrchestrationConfigTypeDef,
     AggregatedProfileTimeTypeDef,
     UserFeedbackTypeDef,
     MetricTypeDef,
-    FrameMetricTypeDef,
+    TimestampTypeDef,
     TimestampStructureTypeDef,
+    BlobTypeDef,
+    ChannelOutputTypeDef,
+    ChannelTypeDef,
     ConfigureAgentRequestRequestTypeDef,
     DeleteProfilingGroupRequestRequestTypeDef,
     DescribeProfilingGroupRequestRequestTypeDef,
     FindingsReportSummaryTypeDef,
+    FrameMetricOutputTypeDef,
+    FrameMetricTypeDef,
     GetFindingsReportAccountSummaryRequestRequestTypeDef,
     GetNotificationConfigurationRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
-    GetProfileRequestRequestTypeDef,
-    GetProfileResponseTypeDef,
-    GetRecommendationsRequestRequestTypeDef,
-    ListFindingsReportsRequestRequestTypeDef,
-    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
-    ListProfileTimesRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     ProfileTimeTypeDef,
     ListProfilingGroupsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MatchTypeDef,
-    PaginatorConfigTypeDef,
     PatternTypeDef,
-    PostAgentProfileRequestRequestTypeDef,
     PutPermissionRequestRequestTypeDef,
-    PutPermissionResponseTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    RemovePermissionResponseTypeDef,
-    ResponseMetadataTypeDef,
     SubmitFeedbackRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AddNotificationChannelsRequestRequestTypeDef,
-    NotificationConfigurationTypeDef,
+    GetPolicyResponseTypeDef,
+    GetProfileResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutPermissionResponseTypeDef,
+    RemovePermissionResponseTypeDef,
     ConfigureAgentResponseTypeDef,
     CreateProfilingGroupRequestRequestTypeDef,
     UpdateProfilingGroupRequestRequestTypeDef,
     ProfilingStatusTypeDef,
     AnomalyInstanceTypeDef,
-    BatchGetFrameMetricDataRequestRequestTypeDef,
-    FrameMetricDatumTypeDef,
+    GetProfileRequestRequestTypeDef,
+    GetRecommendationsRequestRequestTypeDef,
+    ListFindingsReportsRequestRequestTypeDef,
+    ListProfileTimesRequestRequestTypeDef,
+    PostAgentProfileRequestRequestTypeDef,
+    NotificationConfigurationTypeDef,
+    ChannelUnionTypeDef,
     GetFindingsReportAccountSummaryResponseTypeDef,
     ListFindingsReportsResponseTypeDef,
+    FrameMetricDatumTypeDef,
+    FrameMetricUnionTypeDef,
+    ListProfileTimesRequestListProfileTimesPaginateTypeDef,
     ListProfileTimesResponseTypeDef,
     RecommendationTypeDef,
+    ProfilingGroupDescriptionTypeDef,
+    AnomalyTypeDef,
     AddNotificationChannelsResponseTypeDef,
     GetNotificationConfigurationResponseTypeDef,
     RemoveNotificationChannelResponseTypeDef,
-    ProfilingGroupDescriptionTypeDef,
-    AnomalyTypeDef,
+    AddNotificationChannelsRequestRequestTypeDef,
     BatchGetFrameMetricDataResponseTypeDef,
+    BatchGetFrameMetricDataRequestRequestTypeDef,
     CreateProfilingGroupResponseTypeDef,
     DescribeProfilingGroupResponseTypeDef,
     ListProfilingGroupsResponseTypeDef,
     UpdateProfilingGroupResponseTypeDef,
     GetRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> ChannelTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-codeguruprofiler-2.5.2/types_aiobotocore_codeguruprofiler.egg-info/SOURCES.txt` & `types-aiobotocore-codeguruprofiler-2.5.2.post1/types_aiobotocore_codeguruprofiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*


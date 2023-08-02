# Comparing `tmp/types-aiobotocore-stepfunctions-2.5.2.tar.gz` & `tmp/types-aiobotocore-stepfunctions-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-stepfunctions-2.5.2.tar", last modified: Sat Jul  8 01:44:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-stepfunctions-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:05 2023, max compression
```

## Comparing `types-aiobotocore-stepfunctions-2.5.2.tar` & `types-aiobotocore-stepfunctions-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:23.670964 types-aiobotocore-stepfunctions-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:41.000000 types-aiobotocore-stepfunctions-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-07-08 01:44:23.670964 types-aiobotocore-stepfunctions-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-07-08 01:41:41.000000 types-aiobotocore-stepfunctions-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:23.670964 types-aiobotocore-stepfunctions-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-08 01:41:41.000000 types-aiobotocore-stepfunctions-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:23.666964 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-08 01:41:41.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-08 01:41:41.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:41:41.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30282 2023-07-08 01:41:42.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30234 2023-07-08 01:41:41.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-08 01:41:42.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-07-08 01:41:42.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-08 01:41:42.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-08 01:41:42.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:41.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43965 2023-07-08 01:41:43.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43900 2023-07-08 01:41:42.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:41.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:23.670964 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18500 2023-07-08 01:44:23.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-08 01:44:23.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:23.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:23.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:23.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:44:23.000000 types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.521444 types-aiobotocore-stepfunctions-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-08-02 14:53:05.521444 types-aiobotocore-stepfunctions-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:05.521444 types-aiobotocore-stepfunctions-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.513444 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30297 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30249 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-08-02 14:50:20.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-08-02 14:50:20.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-08-02 14:50:20.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-08-02 14:50:20.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44359 2023-08-02 14:50:21.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44294 2023-08-02 14:50:20.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.521444 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-08-02 14:53:05.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:53:05.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:05.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:05.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:05.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:53:05.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2/LICENSE` & `types-aiobotocore-stepfunctions-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2/PKG-INFO` & `types-aiobotocore-stepfunctions-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-stepfunctions
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SFN 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SFN 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore stepfunctions type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore stepfunctions type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-stepfunctions"></a>
 
 # types-aiobotocore-stepfunctions
 
 [![PyPI - types-aiobotocore-stepfunctions](https://img.shields.io/pypi/v/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-stepfunctions?color=blue)](https://pypistats.org/packages/types-aiobotocore-stepfunctions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-stepfunctions)](https://pepy.tech/project/types-aiobotocore-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SFN 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [types-aiobotocore-stepfunctions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/).
 
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
@@ -329,58 +328,54 @@
 )
 
 
 def check_value(value: ExecutionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_stepfunctions.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_stepfunctions.type_defs import (
     ActivityFailedEventDetailsTypeDef,
     ActivityListItemTypeDef,
     ActivityScheduleFailedEventDetailsTypeDef,
     HistoryEventExecutionDataDetailsTypeDef,
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
-    CreateActivityOutputTypeDef,
+    ResponseMetadataTypeDef,
     RoutingConfigurationListItemTypeDef,
-    CreateStateMachineAliasOutputTypeDef,
     TracingConfigurationTypeDef,
-    CreateStateMachineOutputTypeDef,
     DeleteActivityInputRequestTypeDef,
     DeleteStateMachineAliasInputRequestTypeDef,
     DeleteStateMachineInputRequestTypeDef,
     DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
-    DescribeActivityOutputTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
     DescribeStateMachineAliasInputRequestTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
-    GetActivityTaskOutputTypeDef,
-    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetExecutionHistoryInputRequestTypeDef,
     LambdaFunctionFailedEventDetailsTypeDef,
     LambdaFunctionScheduleFailedEventDetailsTypeDef,
     LambdaFunctionStartFailedEventDetailsTypeDef,
     LambdaFunctionTimedOutEventDetailsTypeDef,
     MapIterationEventDetailsTypeDef,
     MapRunFailedEventDetailsTypeDef,
@@ -388,83 +383,89 @@
     MapStateStartedEventDetailsTypeDef,
     TaskFailedEventDetailsTypeDef,
     TaskStartFailedEventDetailsTypeDef,
     TaskStartedEventDetailsTypeDef,
     TaskSubmitFailedEventDetailsTypeDef,
     TaskTimedOutEventDetailsTypeDef,
     TaskCredentialsTypeDef,
-    ListActivitiesInputListActivitiesPaginateTypeDef,
     ListActivitiesInputRequestTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
-    ListMapRunsInputListMapRunsPaginateTypeDef,
     ListMapRunsInputRequestTypeDef,
     MapRunListItemTypeDef,
     ListStateMachineAliasesInputRequestTypeDef,
     StateMachineAliasListItemTypeDef,
     ListStateMachineVersionsInputRequestTypeDef,
     StateMachineVersionListItemTypeDef,
-    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PublishStateMachineVersionInputRequestTypeDef,
-    PublishStateMachineVersionOutputTypeDef,
-    ResponseMetadataTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
-    StartExecutionOutputTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
-    StopExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateMapRunInputRequestTypeDef,
-    UpdateStateMachineAliasOutputTypeDef,
-    UpdateStateMachineOutputTypeDef,
-    ListActivitiesOutputTypeDef,
     ActivityScheduledEventDetailsTypeDef,
     ActivitySucceededEventDetailsTypeDef,
     ExecutionStartedEventDetailsTypeDef,
     ExecutionSucceededEventDetailsTypeDef,
     LambdaFunctionSucceededEventDetailsTypeDef,
     StateEnteredEventDetailsTypeDef,
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
-    DescribeExecutionOutputTypeDef,
-    StartSyncExecutionOutputTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateActivityOutputTypeDef,
+    CreateStateMachineAliasOutputTypeDef,
+    CreateStateMachineOutputTypeDef,
+    DescribeActivityOutputTypeDef,
+    DescribeExecutionOutputTypeDef,
+    GetActivityTaskOutputTypeDef,
+    ListActivitiesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PublishStateMachineVersionOutputTypeDef,
+    StartExecutionOutputTypeDef,
+    StartSyncExecutionOutputTypeDef,
+    StopExecutionOutputTypeDef,
+    UpdateStateMachineAliasOutputTypeDef,
+    UpdateStateMachineOutputTypeDef,
     CreateStateMachineAliasInputRequestTypeDef,
     DescribeStateMachineAliasOutputTypeDef,
     UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
     ListExecutionsOutputTypeDef,
+    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    ListActivitiesInputListActivitiesPaginateTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
+    ListMapRunsInputListMapRunsPaginateTypeDef,
+    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
-    CreateStateMachineInputRequestTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
+    CreateStateMachineInputRequestTypeDef,
+    LoggingConfigurationUnionTypeDef,
     UpdateStateMachineInputRequestTypeDef,
     GetExecutionHistoryOutputTypeDef,
 )
 
 
-def get_structure() -> ActivityFailedEventDetailsTypeDef:
+def get_value() -> ActivityFailedEventDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2/README.md` & `types-aiobotocore-stepfunctions-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-stepfunctions"></a>
 
 # types-aiobotocore-stepfunctions
 
 [![PyPI - types-aiobotocore-stepfunctions](https://img.shields.io/pypi/v/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-stepfunctions?color=blue)](https://pypistats.org/packages/types-aiobotocore-stepfunctions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-stepfunctions)](https://pepy.tech/project/types-aiobotocore-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SFN 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [types-aiobotocore-stepfunctions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/).
 
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
@@ -296,58 +296,54 @@
 )
 
 
 def check_value(value: ExecutionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_stepfunctions.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_stepfunctions.type_defs import (
     ActivityFailedEventDetailsTypeDef,
     ActivityListItemTypeDef,
     ActivityScheduleFailedEventDetailsTypeDef,
     HistoryEventExecutionDataDetailsTypeDef,
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
-    CreateActivityOutputTypeDef,
+    ResponseMetadataTypeDef,
     RoutingConfigurationListItemTypeDef,
-    CreateStateMachineAliasOutputTypeDef,
     TracingConfigurationTypeDef,
-    CreateStateMachineOutputTypeDef,
     DeleteActivityInputRequestTypeDef,
     DeleteStateMachineAliasInputRequestTypeDef,
     DeleteStateMachineInputRequestTypeDef,
     DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
-    DescribeActivityOutputTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
     DescribeStateMachineAliasInputRequestTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
-    GetActivityTaskOutputTypeDef,
-    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetExecutionHistoryInputRequestTypeDef,
     LambdaFunctionFailedEventDetailsTypeDef,
     LambdaFunctionScheduleFailedEventDetailsTypeDef,
     LambdaFunctionStartFailedEventDetailsTypeDef,
     LambdaFunctionTimedOutEventDetailsTypeDef,
     MapIterationEventDetailsTypeDef,
     MapRunFailedEventDetailsTypeDef,
@@ -355,83 +351,89 @@
     MapStateStartedEventDetailsTypeDef,
     TaskFailedEventDetailsTypeDef,
     TaskStartFailedEventDetailsTypeDef,
     TaskStartedEventDetailsTypeDef,
     TaskSubmitFailedEventDetailsTypeDef,
     TaskTimedOutEventDetailsTypeDef,
     TaskCredentialsTypeDef,
-    ListActivitiesInputListActivitiesPaginateTypeDef,
     ListActivitiesInputRequestTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
-    ListMapRunsInputListMapRunsPaginateTypeDef,
     ListMapRunsInputRequestTypeDef,
     MapRunListItemTypeDef,
     ListStateMachineAliasesInputRequestTypeDef,
     StateMachineAliasListItemTypeDef,
     ListStateMachineVersionsInputRequestTypeDef,
     StateMachineVersionListItemTypeDef,
-    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PublishStateMachineVersionInputRequestTypeDef,
-    PublishStateMachineVersionOutputTypeDef,
-    ResponseMetadataTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
-    StartExecutionOutputTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
-    StopExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateMapRunInputRequestTypeDef,
-    UpdateStateMachineAliasOutputTypeDef,
-    UpdateStateMachineOutputTypeDef,
-    ListActivitiesOutputTypeDef,
     ActivityScheduledEventDetailsTypeDef,
     ActivitySucceededEventDetailsTypeDef,
     ExecutionStartedEventDetailsTypeDef,
     ExecutionSucceededEventDetailsTypeDef,
     LambdaFunctionSucceededEventDetailsTypeDef,
     StateEnteredEventDetailsTypeDef,
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
-    DescribeExecutionOutputTypeDef,
-    StartSyncExecutionOutputTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateActivityOutputTypeDef,
+    CreateStateMachineAliasOutputTypeDef,
+    CreateStateMachineOutputTypeDef,
+    DescribeActivityOutputTypeDef,
+    DescribeExecutionOutputTypeDef,
+    GetActivityTaskOutputTypeDef,
+    ListActivitiesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PublishStateMachineVersionOutputTypeDef,
+    StartExecutionOutputTypeDef,
+    StartSyncExecutionOutputTypeDef,
+    StopExecutionOutputTypeDef,
+    UpdateStateMachineAliasOutputTypeDef,
+    UpdateStateMachineOutputTypeDef,
     CreateStateMachineAliasInputRequestTypeDef,
     DescribeStateMachineAliasOutputTypeDef,
     UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
     ListExecutionsOutputTypeDef,
+    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    ListActivitiesInputListActivitiesPaginateTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
+    ListMapRunsInputListMapRunsPaginateTypeDef,
+    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
-    CreateStateMachineInputRequestTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
+    CreateStateMachineInputRequestTypeDef,
+    LoggingConfigurationUnionTypeDef,
     UpdateStateMachineInputRequestTypeDef,
     GetExecutionHistoryOutputTypeDef,
 )
 
 
-def get_structure() -> ActivityFailedEventDetailsTypeDef:
+def get_value() -> ActivityFailedEventDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2/setup.py` & `types-aiobotocore-stepfunctions-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-stepfunctions",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_stepfunctions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SFN 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore stepfunctions type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore stepfunctions type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_stepfunctions": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/"
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/__init__.py` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/__init__.pyi` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/__main__.py` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SFN 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SFN 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN\nOther"
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

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/client.py` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
     TracingConfigurationTypeDef,
@@ -153,15 +153,15 @@
     async def create_state_machine(
         self,
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
-        loggingConfiguration: LoggingConfigurationTypeDef = ...,
+        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
@@ -511,15 +511,15 @@
 
     async def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
-        loggingConfiguration: LoggingConfigurationTypeDef = ...,
+        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> UpdateStateMachineOutputTypeDef:
         """
         Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/client.pyi` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoggingConfigurationTypeDef,
+    LoggingConfigurationUnionTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
     TracingConfigurationTypeDef,
@@ -145,15 +145,15 @@
     async def create_state_machine(
         self,
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
-        loggingConfiguration: LoggingConfigurationTypeDef = ...,
+        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
@@ -471,15 +471,15 @@
         """
     async def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
-        loggingConfiguration: LoggingConfigurationTypeDef = ...,
+        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> UpdateStateMachineOutputTypeDef:
         """
         Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/literals.py` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/literals.pyi` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/paginator.py` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -47,101 +47,94 @@
     "GetExecutionHistoryPaginator",
     "ListActivitiesPaginator",
     "ListExecutionsPaginator",
     "ListMapRunsPaginator",
     "ListStateMachinesPaginator",
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
 class GetExecutionHistoryPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#getexecutionhistorypaginator)
     """
 
     def paginate(
         self,
         *,
         executionArn: str,
         reverseOrder: bool = ...,
         includeExecutionData: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetExecutionHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#getexecutionhistorypaginator)
         """
 
-
 class ListActivitiesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listactivitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListActivitiesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listactivitiespaginator)
         """
 
-
 class ListExecutionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         mapRunArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listexecutionspaginator)
         """
 
-
 class ListMapRunsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listmaprunspaginator)
     """
 
     def paginate(
-        self, *, executionArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, executionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMapRunsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listmaprunspaginator)
         """
 
-
 class ListStateMachinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#liststatemachinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStateMachinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#liststatemachinespaginator)
         """
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/paginator.pyi` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,94 +47,101 @@
     "GetExecutionHistoryPaginator",
     "ListActivitiesPaginator",
     "ListExecutionsPaginator",
     "ListMapRunsPaginator",
     "ListStateMachinesPaginator",
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
 class GetExecutionHistoryPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#getexecutionhistorypaginator)
     """
 
     def paginate(
         self,
         *,
         executionArn: str,
         reverseOrder: bool = ...,
         includeExecutionData: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetExecutionHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#getexecutionhistorypaginator)
         """
 
+
 class ListActivitiesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listactivitiespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListActivitiesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listactivitiespaginator)
         """
 
+
 class ListExecutionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listexecutionspaginator)
     """
 
     def paginate(
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         mapRunArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listexecutionspaginator)
         """
 
+
 class ListMapRunsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listmaprunspaginator)
     """
 
     def paginate(
-        self, *, executionArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, executionArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMapRunsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listmaprunspaginator)
         """
 
+
 class ListStateMachinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#liststatemachinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStateMachinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#liststatemachinespaginator)
         """
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/type_defs.py` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_stepfunctions.type_defs import ActivityFailedEventDetailsTypeDef
 
-    data: ActivityFailedEventDetailsTypeDef = {...}
+    data: ActivityFailedEventDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ExecutionStatusType,
     HistoryEventTypeType,
     LogLevelType,
     MapRunStatusType,
     StateMachineStatusType,
@@ -38,39 +38,35 @@
     "HistoryEventExecutionDataDetailsTypeDef",
     "ActivityStartedEventDetailsTypeDef",
     "ActivityTimedOutEventDetailsTypeDef",
     "BillingDetailsTypeDef",
     "CloudWatchEventsExecutionDataDetailsTypeDef",
     "CloudWatchLogsLogGroupTypeDef",
     "TagTypeDef",
-    "CreateActivityOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "RoutingConfigurationListItemTypeDef",
-    "CreateStateMachineAliasOutputTypeDef",
     "TracingConfigurationTypeDef",
-    "CreateStateMachineOutputTypeDef",
     "DeleteActivityInputRequestTypeDef",
     "DeleteStateMachineAliasInputRequestTypeDef",
     "DeleteStateMachineInputRequestTypeDef",
     "DeleteStateMachineVersionInputRequestTypeDef",
     "DescribeActivityInputRequestTypeDef",
-    "DescribeActivityOutputTypeDef",
     "DescribeExecutionInputRequestTypeDef",
     "DescribeMapRunInputRequestTypeDef",
     "MapRunExecutionCountsTypeDef",
     "MapRunItemCountsTypeDef",
     "DescribeStateMachineAliasInputRequestTypeDef",
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     "DescribeStateMachineInputRequestTypeDef",
     "ExecutionAbortedEventDetailsTypeDef",
     "ExecutionFailedEventDetailsTypeDef",
     "ExecutionListItemTypeDef",
     "ExecutionTimedOutEventDetailsTypeDef",
     "GetActivityTaskInputRequestTypeDef",
-    "GetActivityTaskOutputTypeDef",
-    "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetExecutionHistoryInputRequestTypeDef",
     "LambdaFunctionFailedEventDetailsTypeDef",
     "LambdaFunctionScheduleFailedEventDetailsTypeDef",
     "LambdaFunctionStartFailedEventDetailsTypeDef",
     "LambdaFunctionTimedOutEventDetailsTypeDef",
     "MapIterationEventDetailsTypeDef",
     "MapRunFailedEventDetailsTypeDef",
@@ -78,77 +74,83 @@
     "MapStateStartedEventDetailsTypeDef",
     "TaskFailedEventDetailsTypeDef",
     "TaskStartFailedEventDetailsTypeDef",
     "TaskStartedEventDetailsTypeDef",
     "TaskSubmitFailedEventDetailsTypeDef",
     "TaskTimedOutEventDetailsTypeDef",
     "TaskCredentialsTypeDef",
-    "ListActivitiesInputListActivitiesPaginateTypeDef",
     "ListActivitiesInputRequestTypeDef",
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListExecutionsInputRequestTypeDef",
-    "ListMapRunsInputListMapRunsPaginateTypeDef",
     "ListMapRunsInputRequestTypeDef",
     "MapRunListItemTypeDef",
     "ListStateMachineAliasesInputRequestTypeDef",
     "StateMachineAliasListItemTypeDef",
     "ListStateMachineVersionsInputRequestTypeDef",
     "StateMachineVersionListItemTypeDef",
-    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "ListStateMachinesInputRequestTypeDef",
     "StateMachineListItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PublishStateMachineVersionInputRequestTypeDef",
-    "PublishStateMachineVersionOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SendTaskFailureInputRequestTypeDef",
     "SendTaskHeartbeatInputRequestTypeDef",
     "SendTaskSuccessInputRequestTypeDef",
     "StartExecutionInputRequestTypeDef",
-    "StartExecutionOutputTypeDef",
     "StartSyncExecutionInputRequestTypeDef",
     "StopExecutionInputRequestTypeDef",
-    "StopExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateMapRunInputRequestTypeDef",
-    "UpdateStateMachineAliasOutputTypeDef",
-    "UpdateStateMachineOutputTypeDef",
-    "ListActivitiesOutputTypeDef",
     "ActivityScheduledEventDetailsTypeDef",
     "ActivitySucceededEventDetailsTypeDef",
     "ExecutionStartedEventDetailsTypeDef",
     "ExecutionSucceededEventDetailsTypeDef",
     "LambdaFunctionSucceededEventDetailsTypeDef",
     "StateEnteredEventDetailsTypeDef",
     "StateExitedEventDetailsTypeDef",
     "TaskSubmittedEventDetailsTypeDef",
     "TaskSucceededEventDetailsTypeDef",
-    "DescribeExecutionOutputTypeDef",
-    "StartSyncExecutionOutputTypeDef",
     "LogDestinationTypeDef",
     "CreateActivityInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "CreateActivityOutputTypeDef",
+    "CreateStateMachineAliasOutputTypeDef",
+    "CreateStateMachineOutputTypeDef",
+    "DescribeActivityOutputTypeDef",
+    "DescribeExecutionOutputTypeDef",
+    "GetActivityTaskOutputTypeDef",
+    "ListActivitiesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PublishStateMachineVersionOutputTypeDef",
+    "StartExecutionOutputTypeDef",
+    "StartSyncExecutionOutputTypeDef",
+    "StopExecutionOutputTypeDef",
+    "UpdateStateMachineAliasOutputTypeDef",
+    "UpdateStateMachineOutputTypeDef",
     "CreateStateMachineAliasInputRequestTypeDef",
     "DescribeStateMachineAliasOutputTypeDef",
     "UpdateStateMachineAliasInputRequestTypeDef",
     "DescribeMapRunOutputTypeDef",
     "ListExecutionsOutputTypeDef",
+    "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    "ListActivitiesInputListActivitiesPaginateTypeDef",
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
+    "ListMapRunsInputListMapRunsPaginateTypeDef",
+    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
     "ListStateMachineAliasesOutputTypeDef",
     "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
-    "CreateStateMachineInputRequestTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
+    "CreateStateMachineInputRequestTypeDef",
+    "LoggingConfigurationUnionTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
     "GetExecutionHistoryOutputTypeDef",
 )
 
 ActivityFailedEventDetailsTypeDef = TypedDict(
     "ActivityFailedEventDetailsTypeDef",
     {
@@ -231,58 +233,41 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-CreateActivityOutputTypeDef = TypedDict(
-    "CreateActivityOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "activityArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 RoutingConfigurationListItemTypeDef = TypedDict(
     "RoutingConfigurationListItemTypeDef",
     {
         "stateMachineVersionArn": str,
         "weight": int,
     },
 )
 
-CreateStateMachineAliasOutputTypeDef = TypedDict(
-    "CreateStateMachineAliasOutputTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TracingConfigurationTypeDef = TypedDict(
     "TracingConfigurationTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
 
-CreateStateMachineOutputTypeDef = TypedDict(
-    "CreateStateMachineOutputTypeDef",
-    {
-        "stateMachineArn": str,
-        "creationDate": datetime,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteActivityInputRequestTypeDef = TypedDict(
     "DeleteActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
@@ -310,24 +295,14 @@
 DescribeActivityInputRequestTypeDef = TypedDict(
     "DescribeActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
-DescribeActivityOutputTypeDef = TypedDict(
-    "DescribeActivityOutputTypeDef",
-    {
-        "activityArn": str,
-        "name": str,
-        "creationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeExecutionInputRequestTypeDef = TypedDict(
     "DescribeExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
@@ -460,47 +435,24 @@
 
 class GetActivityTaskInputRequestTypeDef(
     _RequiredGetActivityTaskInputRequestTypeDef, _OptionalGetActivityTaskInputRequestTypeDef
 ):
     pass
 
 
-GetActivityTaskOutputTypeDef = TypedDict(
-    "GetActivityTaskOutputTypeDef",
-    {
-        "taskToken": str,
-        "input": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
-    {
-        "executionArn": str,
-    },
-)
-_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "reverseOrder": bool,
-        "includeExecutionData": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
-    _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-    _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetExecutionHistoryInputRequestTypeDef = TypedDict(
     "_RequiredGetExecutionHistoryInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalGetExecutionHistoryInputRequestTypeDef = TypedDict(
@@ -695,76 +647,35 @@
     "TaskCredentialsTypeDef",
     {
         "roleArn": str,
     },
     total=False,
 )
 
-ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
-    "ListActivitiesInputListActivitiesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListActivitiesInputRequestTypeDef = TypedDict(
     "ListActivitiesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "stateMachineArn": str,
-        "statusFilter": ExecutionStatusType,
-        "mapRunArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExecutionsInputRequestTypeDef = TypedDict(
     "ListExecutionsInputRequestTypeDef",
     {
         "stateMachineArn": str,
         "statusFilter": ExecutionStatusType,
         "maxResults": int,
         "nextToken": str,
         "mapRunArn": str,
     },
     total=False,
 )
 
-_RequiredListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
-    "_RequiredListMapRunsInputListMapRunsPaginateTypeDef",
-    {
-        "executionArn": str,
-    },
-)
-_OptionalListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
-    "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMapRunsInputListMapRunsPaginateTypeDef(
-    _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
-    _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMapRunsInputRequestTypeDef = TypedDict(
     "_RequiredListMapRunsInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalListMapRunsInputRequestTypeDef = TypedDict(
@@ -863,22 +774,14 @@
     "StateMachineVersionListItemTypeDef",
     {
         "stateMachineVersionArn": str,
         "creationDate": datetime,
     },
 )
 
-ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
-    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStateMachinesInputRequestTypeDef = TypedDict(
     "ListStateMachinesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -897,24 +800,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
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
 _RequiredPublishStateMachineVersionInputRequestTypeDef = TypedDict(
     "_RequiredPublishStateMachineVersionInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalPublishStateMachineVersionInputRequestTypeDef = TypedDict(
@@ -930,34 +823,14 @@
 class PublishStateMachineVersionInputRequestTypeDef(
     _RequiredPublishStateMachineVersionInputRequestTypeDef,
     _OptionalPublishStateMachineVersionInputRequestTypeDef,
 ):
     pass
 
 
-PublishStateMachineVersionOutputTypeDef = TypedDict(
-    "PublishStateMachineVersionOutputTypeDef",
-    {
-        "creationDate": datetime,
-        "stateMachineVersionArn": str,
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
 _RequiredSendTaskFailureInputRequestTypeDef = TypedDict(
     "_RequiredSendTaskFailureInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalSendTaskFailureInputRequestTypeDef = TypedDict(
@@ -1010,23 +883,14 @@
 
 class StartExecutionInputRequestTypeDef(
     _RequiredStartExecutionInputRequestTypeDef, _OptionalStartExecutionInputRequestTypeDef
 ):
     pass
 
 
-StartExecutionOutputTypeDef = TypedDict(
-    "StartExecutionOutputTypeDef",
-    {
-        "executionArn": str,
-        "startDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartSyncExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStartSyncExecutionInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalStartSyncExecutionInputRequestTypeDef = TypedDict(
@@ -1064,22 +928,14 @@
 
 class StopExecutionInputRequestTypeDef(
     _RequiredStopExecutionInputRequestTypeDef, _OptionalStopExecutionInputRequestTypeDef
 ):
     pass
 
 
-StopExecutionOutputTypeDef = TypedDict(
-    "StopExecutionOutputTypeDef",
-    {
-        "stopDate": datetime,
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
@@ -1103,41 +959,14 @@
 
 class UpdateMapRunInputRequestTypeDef(
     _RequiredUpdateMapRunInputRequestTypeDef, _OptionalUpdateMapRunInputRequestTypeDef
 ):
     pass
 
 
-UpdateStateMachineAliasOutputTypeDef = TypedDict(
-    "UpdateStateMachineAliasOutputTypeDef",
-    {
-        "updateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStateMachineOutputTypeDef = TypedDict(
-    "UpdateStateMachineOutputTypeDef",
-    {
-        "updateDate": datetime,
-        "revisionId": str,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListActivitiesOutputTypeDef = TypedDict(
-    "ListActivitiesOutputTypeDef",
-    {
-        "activities": List[ActivityListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredActivityScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredActivityScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
 )
 _OptionalActivityScheduledEventDetailsTypeDef = TypedDict(
@@ -1283,14 +1112,89 @@
 
 class TaskSucceededEventDetailsTypeDef(
     _RequiredTaskSucceededEventDetailsTypeDef, _OptionalTaskSucceededEventDetailsTypeDef
 ):
     pass
 
 
+LogDestinationTypeDef = TypedDict(
+    "LogDestinationTypeDef",
+    {
+        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateActivityInputRequestTypeDef = TypedDict(
+    "_RequiredCreateActivityInputRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateActivityInputRequestTypeDef = TypedDict(
+    "_OptionalCreateActivityInputRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateActivityInputRequestTypeDef(
+    _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
+):
+    pass
+
+
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateActivityOutputTypeDef = TypedDict(
+    "CreateActivityOutputTypeDef",
+    {
+        "activityArn": str,
+        "creationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStateMachineAliasOutputTypeDef = TypedDict(
+    "CreateStateMachineAliasOutputTypeDef",
+    {
+        "stateMachineAliasArn": str,
+        "creationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStateMachineOutputTypeDef = TypedDict(
+    "CreateStateMachineOutputTypeDef",
+    {
+        "stateMachineArn": str,
+        "creationDate": datetime,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeActivityOutputTypeDef = TypedDict(
+    "DescribeActivityOutputTypeDef",
+    {
+        "activityArn": str,
+        "name": str,
+        "creationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeExecutionOutputTypeDef = TypedDict(
     "DescribeExecutionOutputTypeDef",
     {
         "executionArn": str,
         "stateMachineArn": str,
         "name": str,
         "status": ExecutionStatusType,
@@ -1302,15 +1206,59 @@
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "mapRunArn": str,
         "error": str,
         "cause": str,
         "stateMachineVersionArn": str,
         "stateMachineAliasArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetActivityTaskOutputTypeDef = TypedDict(
+    "GetActivityTaskOutputTypeDef",
+    {
+        "taskToken": str,
+        "input": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListActivitiesOutputTypeDef = TypedDict(
+    "ListActivitiesOutputTypeDef",
+    {
+        "activities": List[ActivityListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishStateMachineVersionOutputTypeDef = TypedDict(
+    "PublishStateMachineVersionOutputTypeDef",
+    {
+        "creationDate": datetime,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartExecutionOutputTypeDef = TypedDict(
+    "StartExecutionOutputTypeDef",
+    {
+        "executionArn": str,
+        "startDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSyncExecutionOutputTypeDef = TypedDict(
     "StartSyncExecutionOutputTypeDef",
     {
         "executionArn": str,
@@ -1323,60 +1271,41 @@
         "cause": str,
         "input": str,
         "inputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "output": str,
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "billingDetails": BillingDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LogDestinationTypeDef = TypedDict(
-    "LogDestinationTypeDef",
-    {
-        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredCreateActivityInputRequestTypeDef = TypedDict(
-    "_RequiredCreateActivityInputRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateActivityInputRequestTypeDef = TypedDict(
-    "_OptionalCreateActivityInputRequestTypeDef",
+StopExecutionOutputTypeDef = TypedDict(
+    "StopExecutionOutputTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "stopDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateActivityInputRequestTypeDef(
-    _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
-):
-    pass
-
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+UpdateStateMachineAliasOutputTypeDef = TypedDict(
+    "UpdateStateMachineAliasOutputTypeDef",
     {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "updateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+UpdateStateMachineOutputTypeDef = TypedDict(
+    "UpdateStateMachineOutputTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
+        "updateDate": datetime,
+        "revisionId": str,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateStateMachineAliasInputRequestTypeDef = TypedDict(
     "_RequiredCreateStateMachineAliasInputRequestTypeDef",
     {
         "name": str,
@@ -1404,15 +1333,15 @@
     {
         "stateMachineAliasArn": str,
         "name": str,
         "description": str,
         "routingConfiguration": List[RoutingConfigurationListItemTypeDef],
         "creationDate": datetime,
         "updateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineAliasInputRequestTypeDef",
     {
         "stateMachineAliasArn": str,
@@ -1444,27 +1373,100 @@
         "startDate": datetime,
         "stopDate": datetime,
         "maxConcurrency": int,
         "toleratedFailurePercentage": float,
         "toleratedFailureCount": int,
         "itemCounts": MapRunItemCountsTypeDef,
         "executionCounts": MapRunExecutionCountsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExecutionsOutputTypeDef = TypedDict(
     "ListExecutionsOutputTypeDef",
     {
         "executions": List[ExecutionListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    {
+        "executionArn": str,
+    },
+)
+_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "includeExecutionData": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
+    _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+):
+    pass
+
+
+ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
+    "ListActivitiesInputListActivitiesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "stateMachineArn": str,
+        "statusFilter": ExecutionStatusType,
+        "mapRunArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
+    "_RequiredListMapRunsInputListMapRunsPaginateTypeDef",
+    {
+        "executionArn": str,
+    },
+)
+_OptionalListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
+    "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMapRunsInputListMapRunsPaginateTypeDef(
+    _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
+    _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
+):
+    pass
+
+
+ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
+    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredLambdaFunctionScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredLambdaFunctionScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
 )
 _OptionalLambdaFunctionScheduledEventDetailsTypeDef = TypedDict(
@@ -1513,45 +1515,55 @@
 
 
 ListMapRunsOutputTypeDef = TypedDict(
     "ListMapRunsOutputTypeDef",
     {
         "mapRuns": List[MapRunListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStateMachineAliasesOutputTypeDef = TypedDict(
     "ListStateMachineAliasesOutputTypeDef",
     {
         "stateMachineAliases": List[StateMachineAliasListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStateMachineVersionsOutputTypeDef = TypedDict(
     "ListStateMachineVersionsOutputTypeDef",
     {
         "stateMachineVersions": List[StateMachineVersionListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStateMachinesOutputTypeDef = TypedDict(
     "ListStateMachinesOutputTypeDef",
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingConfigurationOutputTypeDef = TypedDict(
+    "LoggingConfigurationOutputTypeDef",
+    {
+        "level": LogLevelType,
+        "includeExecutionData": bool,
+        "destinations": List[LogDestinationTypeDef],
+    },
+    total=False,
+)
+
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "level": LogLevelType,
         "includeExecutionData": bool,
         "destinations": Sequence[LogDestinationTypeDef],
     },
@@ -1609,78 +1621,81 @@
 )
 
 
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
 
-_RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
-    "_RequiredCreateStateMachineInputRequestTypeDef",
-    {
-        "name": str,
-        "definition": str,
-        "roleArn": str,
-    },
-)
-_OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
-    "_OptionalCreateStateMachineInputRequestTypeDef",
-    {
-        "type": StateMachineTypeType,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
-        "tags": Sequence[TagTypeDef],
-        "tracingConfiguration": TracingConfigurationTypeDef,
-        "publish": bool,
-        "versionDescription": str,
-    },
-    total=False,
-)
-
-
-class CreateStateMachineInputRequestTypeDef(
-    _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
-):
-    pass
-
-
 DescribeStateMachineForExecutionOutputTypeDef = TypedDict(
     "DescribeStateMachineForExecutionOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "mapRunArn": str,
         "label": str,
         "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStateMachineOutputTypeDef = TypedDict(
     "DescribeStateMachineOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "status": StateMachineStatusType,
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "label": str,
         "revisionId": str,
         "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
+    "_RequiredCreateStateMachineInputRequestTypeDef",
+    {
+        "name": str,
+        "definition": str,
+        "roleArn": str,
     },
 )
+_OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
+    "_OptionalCreateStateMachineInputRequestTypeDef",
+    {
+        "type": StateMachineTypeType,
+        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "tracingConfiguration": TracingConfigurationTypeDef,
+        "publish": bool,
+        "versionDescription": str,
+    },
+    total=False,
+)
+
+
+class CreateStateMachineInputRequestTypeDef(
+    _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
+):
+    pass
+
 
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 _RequiredUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalUpdateStateMachineInputRequestTypeDef = TypedDict(
@@ -1704,10 +1719,10 @@
 
 
 GetExecutionHistoryOutputTypeDef = TypedDict(
     "GetExecutionHistoryOutputTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions/type_defs.pyi` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_stepfunctions.type_defs import ActivityFailedEventDetailsTypeDef
 
-    data: ActivityFailedEventDetailsTypeDef = {...}
+    data: ActivityFailedEventDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ExecutionStatusType,
     HistoryEventTypeType,
     LogLevelType,
     MapRunStatusType,
     StateMachineStatusType,
@@ -37,39 +37,35 @@
     "HistoryEventExecutionDataDetailsTypeDef",
     "ActivityStartedEventDetailsTypeDef",
     "ActivityTimedOutEventDetailsTypeDef",
     "BillingDetailsTypeDef",
     "CloudWatchEventsExecutionDataDetailsTypeDef",
     "CloudWatchLogsLogGroupTypeDef",
     "TagTypeDef",
-    "CreateActivityOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "RoutingConfigurationListItemTypeDef",
-    "CreateStateMachineAliasOutputTypeDef",
     "TracingConfigurationTypeDef",
-    "CreateStateMachineOutputTypeDef",
     "DeleteActivityInputRequestTypeDef",
     "DeleteStateMachineAliasInputRequestTypeDef",
     "DeleteStateMachineInputRequestTypeDef",
     "DeleteStateMachineVersionInputRequestTypeDef",
     "DescribeActivityInputRequestTypeDef",
-    "DescribeActivityOutputTypeDef",
     "DescribeExecutionInputRequestTypeDef",
     "DescribeMapRunInputRequestTypeDef",
     "MapRunExecutionCountsTypeDef",
     "MapRunItemCountsTypeDef",
     "DescribeStateMachineAliasInputRequestTypeDef",
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     "DescribeStateMachineInputRequestTypeDef",
     "ExecutionAbortedEventDetailsTypeDef",
     "ExecutionFailedEventDetailsTypeDef",
     "ExecutionListItemTypeDef",
     "ExecutionTimedOutEventDetailsTypeDef",
     "GetActivityTaskInputRequestTypeDef",
-    "GetActivityTaskOutputTypeDef",
-    "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetExecutionHistoryInputRequestTypeDef",
     "LambdaFunctionFailedEventDetailsTypeDef",
     "LambdaFunctionScheduleFailedEventDetailsTypeDef",
     "LambdaFunctionStartFailedEventDetailsTypeDef",
     "LambdaFunctionTimedOutEventDetailsTypeDef",
     "MapIterationEventDetailsTypeDef",
     "MapRunFailedEventDetailsTypeDef",
@@ -77,77 +73,83 @@
     "MapStateStartedEventDetailsTypeDef",
     "TaskFailedEventDetailsTypeDef",
     "TaskStartFailedEventDetailsTypeDef",
     "TaskStartedEventDetailsTypeDef",
     "TaskSubmitFailedEventDetailsTypeDef",
     "TaskTimedOutEventDetailsTypeDef",
     "TaskCredentialsTypeDef",
-    "ListActivitiesInputListActivitiesPaginateTypeDef",
     "ListActivitiesInputRequestTypeDef",
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListExecutionsInputRequestTypeDef",
-    "ListMapRunsInputListMapRunsPaginateTypeDef",
     "ListMapRunsInputRequestTypeDef",
     "MapRunListItemTypeDef",
     "ListStateMachineAliasesInputRequestTypeDef",
     "StateMachineAliasListItemTypeDef",
     "ListStateMachineVersionsInputRequestTypeDef",
     "StateMachineVersionListItemTypeDef",
-    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "ListStateMachinesInputRequestTypeDef",
     "StateMachineListItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PublishStateMachineVersionInputRequestTypeDef",
-    "PublishStateMachineVersionOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SendTaskFailureInputRequestTypeDef",
     "SendTaskHeartbeatInputRequestTypeDef",
     "SendTaskSuccessInputRequestTypeDef",
     "StartExecutionInputRequestTypeDef",
-    "StartExecutionOutputTypeDef",
     "StartSyncExecutionInputRequestTypeDef",
     "StopExecutionInputRequestTypeDef",
-    "StopExecutionOutputTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateMapRunInputRequestTypeDef",
-    "UpdateStateMachineAliasOutputTypeDef",
-    "UpdateStateMachineOutputTypeDef",
-    "ListActivitiesOutputTypeDef",
     "ActivityScheduledEventDetailsTypeDef",
     "ActivitySucceededEventDetailsTypeDef",
     "ExecutionStartedEventDetailsTypeDef",
     "ExecutionSucceededEventDetailsTypeDef",
     "LambdaFunctionSucceededEventDetailsTypeDef",
     "StateEnteredEventDetailsTypeDef",
     "StateExitedEventDetailsTypeDef",
     "TaskSubmittedEventDetailsTypeDef",
     "TaskSucceededEventDetailsTypeDef",
-    "DescribeExecutionOutputTypeDef",
-    "StartSyncExecutionOutputTypeDef",
     "LogDestinationTypeDef",
     "CreateActivityInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "CreateActivityOutputTypeDef",
+    "CreateStateMachineAliasOutputTypeDef",
+    "CreateStateMachineOutputTypeDef",
+    "DescribeActivityOutputTypeDef",
+    "DescribeExecutionOutputTypeDef",
+    "GetActivityTaskOutputTypeDef",
+    "ListActivitiesOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PublishStateMachineVersionOutputTypeDef",
+    "StartExecutionOutputTypeDef",
+    "StartSyncExecutionOutputTypeDef",
+    "StopExecutionOutputTypeDef",
+    "UpdateStateMachineAliasOutputTypeDef",
+    "UpdateStateMachineOutputTypeDef",
     "CreateStateMachineAliasInputRequestTypeDef",
     "DescribeStateMachineAliasOutputTypeDef",
     "UpdateStateMachineAliasInputRequestTypeDef",
     "DescribeMapRunOutputTypeDef",
     "ListExecutionsOutputTypeDef",
+    "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    "ListActivitiesInputListActivitiesPaginateTypeDef",
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
+    "ListMapRunsInputListMapRunsPaginateTypeDef",
+    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
     "ListStateMachineAliasesOutputTypeDef",
     "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
+    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
-    "CreateStateMachineInputRequestTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
+    "CreateStateMachineInputRequestTypeDef",
+    "LoggingConfigurationUnionTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
     "GetExecutionHistoryOutputTypeDef",
 )
 
 ActivityFailedEventDetailsTypeDef = TypedDict(
     "ActivityFailedEventDetailsTypeDef",
     {
@@ -230,58 +232,41 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-CreateActivityOutputTypeDef = TypedDict(
-    "CreateActivityOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "activityArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 RoutingConfigurationListItemTypeDef = TypedDict(
     "RoutingConfigurationListItemTypeDef",
     {
         "stateMachineVersionArn": str,
         "weight": int,
     },
 )
 
-CreateStateMachineAliasOutputTypeDef = TypedDict(
-    "CreateStateMachineAliasOutputTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TracingConfigurationTypeDef = TypedDict(
     "TracingConfigurationTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
 
-CreateStateMachineOutputTypeDef = TypedDict(
-    "CreateStateMachineOutputTypeDef",
-    {
-        "stateMachineArn": str,
-        "creationDate": datetime,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteActivityInputRequestTypeDef = TypedDict(
     "DeleteActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
@@ -309,24 +294,14 @@
 DescribeActivityInputRequestTypeDef = TypedDict(
     "DescribeActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
-DescribeActivityOutputTypeDef = TypedDict(
-    "DescribeActivityOutputTypeDef",
-    {
-        "activityArn": str,
-        "name": str,
-        "creationDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeExecutionInputRequestTypeDef = TypedDict(
     "DescribeExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
@@ -455,45 +430,24 @@
 )
 
 class GetActivityTaskInputRequestTypeDef(
     _RequiredGetActivityTaskInputRequestTypeDef, _OptionalGetActivityTaskInputRequestTypeDef
 ):
     pass
 
-GetActivityTaskOutputTypeDef = TypedDict(
-    "GetActivityTaskOutputTypeDef",
-    {
-        "taskToken": str,
-        "input": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
-    {
-        "executionArn": str,
-    },
-)
-_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "reverseOrder": bool,
-        "includeExecutionData": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
-    _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-    _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
-):
-    pass
-
 _RequiredGetExecutionHistoryInputRequestTypeDef = TypedDict(
     "_RequiredGetExecutionHistoryInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalGetExecutionHistoryInputRequestTypeDef = TypedDict(
@@ -678,74 +632,35 @@
     "TaskCredentialsTypeDef",
     {
         "roleArn": str,
     },
     total=False,
 )
 
-ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
-    "ListActivitiesInputListActivitiesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListActivitiesInputRequestTypeDef = TypedDict(
     "ListActivitiesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
-    "ListExecutionsInputListExecutionsPaginateTypeDef",
-    {
-        "stateMachineArn": str,
-        "statusFilter": ExecutionStatusType,
-        "mapRunArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExecutionsInputRequestTypeDef = TypedDict(
     "ListExecutionsInputRequestTypeDef",
     {
         "stateMachineArn": str,
         "statusFilter": ExecutionStatusType,
         "maxResults": int,
         "nextToken": str,
         "mapRunArn": str,
     },
     total=False,
 )
 
-_RequiredListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
-    "_RequiredListMapRunsInputListMapRunsPaginateTypeDef",
-    {
-        "executionArn": str,
-    },
-)
-_OptionalListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
-    "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMapRunsInputListMapRunsPaginateTypeDef(
-    _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
-    _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
-):
-    pass
-
 _RequiredListMapRunsInputRequestTypeDef = TypedDict(
     "_RequiredListMapRunsInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalListMapRunsInputRequestTypeDef = TypedDict(
@@ -836,22 +751,14 @@
     "StateMachineVersionListItemTypeDef",
     {
         "stateMachineVersionArn": str,
         "creationDate": datetime,
     },
 )
 
-ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
-    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStateMachinesInputRequestTypeDef = TypedDict(
     "ListStateMachinesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -870,24 +777,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
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
 _RequiredPublishStateMachineVersionInputRequestTypeDef = TypedDict(
     "_RequiredPublishStateMachineVersionInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalPublishStateMachineVersionInputRequestTypeDef = TypedDict(
@@ -901,34 +798,14 @@
 
 class PublishStateMachineVersionInputRequestTypeDef(
     _RequiredPublishStateMachineVersionInputRequestTypeDef,
     _OptionalPublishStateMachineVersionInputRequestTypeDef,
 ):
     pass
 
-PublishStateMachineVersionOutputTypeDef = TypedDict(
-    "PublishStateMachineVersionOutputTypeDef",
-    {
-        "creationDate": datetime,
-        "stateMachineVersionArn": str,
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
 _RequiredSendTaskFailureInputRequestTypeDef = TypedDict(
     "_RequiredSendTaskFailureInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalSendTaskFailureInputRequestTypeDef = TypedDict(
@@ -977,23 +854,14 @@
 )
 
 class StartExecutionInputRequestTypeDef(
     _RequiredStartExecutionInputRequestTypeDef, _OptionalStartExecutionInputRequestTypeDef
 ):
     pass
 
-StartExecutionOutputTypeDef = TypedDict(
-    "StartExecutionOutputTypeDef",
-    {
-        "executionArn": str,
-        "startDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartSyncExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStartSyncExecutionInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalStartSyncExecutionInputRequestTypeDef = TypedDict(
@@ -1027,22 +895,14 @@
 )
 
 class StopExecutionInputRequestTypeDef(
     _RequiredStopExecutionInputRequestTypeDef, _OptionalStopExecutionInputRequestTypeDef
 ):
     pass
 
-StopExecutionOutputTypeDef = TypedDict(
-    "StopExecutionOutputTypeDef",
-    {
-        "stopDate": datetime,
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
@@ -1064,41 +924,14 @@
 )
 
 class UpdateMapRunInputRequestTypeDef(
     _RequiredUpdateMapRunInputRequestTypeDef, _OptionalUpdateMapRunInputRequestTypeDef
 ):
     pass
 
-UpdateStateMachineAliasOutputTypeDef = TypedDict(
-    "UpdateStateMachineAliasOutputTypeDef",
-    {
-        "updateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStateMachineOutputTypeDef = TypedDict(
-    "UpdateStateMachineOutputTypeDef",
-    {
-        "updateDate": datetime,
-        "revisionId": str,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListActivitiesOutputTypeDef = TypedDict(
-    "ListActivitiesOutputTypeDef",
-    {
-        "activities": List[ActivityListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredActivityScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredActivityScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
 )
 _OptionalActivityScheduledEventDetailsTypeDef = TypedDict(
@@ -1234,14 +1067,87 @@
 )
 
 class TaskSucceededEventDetailsTypeDef(
     _RequiredTaskSucceededEventDetailsTypeDef, _OptionalTaskSucceededEventDetailsTypeDef
 ):
     pass
 
+LogDestinationTypeDef = TypedDict(
+    "LogDestinationTypeDef",
+    {
+        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCreateActivityInputRequestTypeDef = TypedDict(
+    "_RequiredCreateActivityInputRequestTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalCreateActivityInputRequestTypeDef = TypedDict(
+    "_OptionalCreateActivityInputRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateActivityInputRequestTypeDef(
+    _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
+):
+    pass
+
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateActivityOutputTypeDef = TypedDict(
+    "CreateActivityOutputTypeDef",
+    {
+        "activityArn": str,
+        "creationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStateMachineAliasOutputTypeDef = TypedDict(
+    "CreateStateMachineAliasOutputTypeDef",
+    {
+        "stateMachineAliasArn": str,
+        "creationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStateMachineOutputTypeDef = TypedDict(
+    "CreateStateMachineOutputTypeDef",
+    {
+        "stateMachineArn": str,
+        "creationDate": datetime,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeActivityOutputTypeDef = TypedDict(
+    "DescribeActivityOutputTypeDef",
+    {
+        "activityArn": str,
+        "name": str,
+        "creationDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeExecutionOutputTypeDef = TypedDict(
     "DescribeExecutionOutputTypeDef",
     {
         "executionArn": str,
         "stateMachineArn": str,
         "name": str,
         "status": ExecutionStatusType,
@@ -1253,15 +1159,59 @@
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "mapRunArn": str,
         "error": str,
         "cause": str,
         "stateMachineVersionArn": str,
         "stateMachineAliasArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetActivityTaskOutputTypeDef = TypedDict(
+    "GetActivityTaskOutputTypeDef",
+    {
+        "taskToken": str,
+        "input": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListActivitiesOutputTypeDef = TypedDict(
+    "ListActivitiesOutputTypeDef",
+    {
+        "activities": List[ActivityListItemTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PublishStateMachineVersionOutputTypeDef = TypedDict(
+    "PublishStateMachineVersionOutputTypeDef",
+    {
+        "creationDate": datetime,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartExecutionOutputTypeDef = TypedDict(
+    "StartExecutionOutputTypeDef",
+    {
+        "executionArn": str,
+        "startDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSyncExecutionOutputTypeDef = TypedDict(
     "StartSyncExecutionOutputTypeDef",
     {
         "executionArn": str,
@@ -1274,58 +1224,41 @@
         "cause": str,
         "input": str,
         "inputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "output": str,
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "billingDetails": BillingDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LogDestinationTypeDef = TypedDict(
-    "LogDestinationTypeDef",
-    {
-        "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateActivityInputRequestTypeDef = TypedDict(
-    "_RequiredCreateActivityInputRequestTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalCreateActivityInputRequestTypeDef = TypedDict(
-    "_OptionalCreateActivityInputRequestTypeDef",
+StopExecutionOutputTypeDef = TypedDict(
+    "StopExecutionOutputTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "stopDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateActivityInputRequestTypeDef(
-    _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
-):
-    pass
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+UpdateStateMachineAliasOutputTypeDef = TypedDict(
+    "UpdateStateMachineAliasOutputTypeDef",
     {
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "updateDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+UpdateStateMachineOutputTypeDef = TypedDict(
+    "UpdateStateMachineOutputTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
+        "updateDate": datetime,
+        "revisionId": str,
+        "stateMachineVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateStateMachineAliasInputRequestTypeDef = TypedDict(
     "_RequiredCreateStateMachineAliasInputRequestTypeDef",
     {
         "name": str,
@@ -1351,15 +1284,15 @@
     {
         "stateMachineAliasArn": str,
         "name": str,
         "description": str,
         "routingConfiguration": List[RoutingConfigurationListItemTypeDef],
         "creationDate": datetime,
         "updateDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineAliasInputRequestTypeDef",
     {
         "stateMachineAliasArn": str,
@@ -1389,27 +1322,96 @@
         "startDate": datetime,
         "stopDate": datetime,
         "maxConcurrency": int,
         "toleratedFailurePercentage": float,
         "toleratedFailureCount": int,
         "itemCounts": MapRunItemCountsTypeDef,
         "executionCounts": MapRunExecutionCountsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExecutionsOutputTypeDef = TypedDict(
     "ListExecutionsOutputTypeDef",
     {
         "executions": List[ExecutionListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    {
+        "executionArn": str,
+    },
+)
+_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
+    {
+        "reverseOrder": bool,
+        "includeExecutionData": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
+    _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+):
+    pass
+
+ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
+    "ListActivitiesInputListActivitiesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListExecutionsInputListExecutionsPaginateTypeDef = TypedDict(
+    "ListExecutionsInputListExecutionsPaginateTypeDef",
+    {
+        "stateMachineArn": str,
+        "statusFilter": ExecutionStatusType,
+        "mapRunArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
+    "_RequiredListMapRunsInputListMapRunsPaginateTypeDef",
+    {
+        "executionArn": str,
+    },
+)
+_OptionalListMapRunsInputListMapRunsPaginateTypeDef = TypedDict(
+    "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMapRunsInputListMapRunsPaginateTypeDef(
+    _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
+    _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
+):
+    pass
+
+ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
+    "ListStateMachinesInputListStateMachinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredLambdaFunctionScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredLambdaFunctionScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
 )
 _OptionalLambdaFunctionScheduledEventDetailsTypeDef = TypedDict(
@@ -1454,45 +1456,55 @@
     pass
 
 ListMapRunsOutputTypeDef = TypedDict(
     "ListMapRunsOutputTypeDef",
     {
         "mapRuns": List[MapRunListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStateMachineAliasesOutputTypeDef = TypedDict(
     "ListStateMachineAliasesOutputTypeDef",
     {
         "stateMachineAliases": List[StateMachineAliasListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStateMachineVersionsOutputTypeDef = TypedDict(
     "ListStateMachineVersionsOutputTypeDef",
     {
         "stateMachineVersions": List[StateMachineVersionListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStateMachinesOutputTypeDef = TypedDict(
     "ListStateMachinesOutputTypeDef",
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingConfigurationOutputTypeDef = TypedDict(
+    "LoggingConfigurationOutputTypeDef",
+    {
+        "level": LogLevelType,
+        "includeExecutionData": bool,
+        "destinations": List[LogDestinationTypeDef],
+    },
+    total=False,
+)
+
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "level": LogLevelType,
         "includeExecutionData": bool,
         "destinations": Sequence[LogDestinationTypeDef],
     },
@@ -1548,76 +1560,79 @@
     },
     total=False,
 )
 
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
-_RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
-    "_RequiredCreateStateMachineInputRequestTypeDef",
-    {
-        "name": str,
-        "definition": str,
-        "roleArn": str,
-    },
-)
-_OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
-    "_OptionalCreateStateMachineInputRequestTypeDef",
-    {
-        "type": StateMachineTypeType,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
-        "tags": Sequence[TagTypeDef],
-        "tracingConfiguration": TracingConfigurationTypeDef,
-        "publish": bool,
-        "versionDescription": str,
-    },
-    total=False,
-)
-
-class CreateStateMachineInputRequestTypeDef(
-    _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
-):
-    pass
-
 DescribeStateMachineForExecutionOutputTypeDef = TypedDict(
     "DescribeStateMachineForExecutionOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "mapRunArn": str,
         "label": str,
         "revisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStateMachineOutputTypeDef = TypedDict(
     "DescribeStateMachineOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "status": StateMachineStatusType,
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "label": str,
         "revisionId": str,
         "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
+    "_RequiredCreateStateMachineInputRequestTypeDef",
+    {
+        "name": str,
+        "definition": str,
+        "roleArn": str,
+    },
+)
+_OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
+    "_OptionalCreateStateMachineInputRequestTypeDef",
+    {
+        "type": StateMachineTypeType,
+        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "tracingConfiguration": TracingConfigurationTypeDef,
+        "publish": bool,
+        "versionDescription": str,
     },
+    total=False,
 )
 
+class CreateStateMachineInputRequestTypeDef(
+    _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
+):
+    pass
+
+LoggingConfigurationUnionTypeDef = Union[
+    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
+]
 _RequiredUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalUpdateStateMachineInputRequestTypeDef = TypedDict(
@@ -1639,10 +1654,10 @@
     pass
 
 GetExecutionHistoryOutputTypeDef = TypedDict(
     "GetExecutionHistoryOutputTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions.egg-info/PKG-INFO` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-stepfunctions
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SFN 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SFN 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore stepfunctions type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore stepfunctions type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-stepfunctions"></a>
 
 # types-aiobotocore-stepfunctions
 
 [![PyPI - types-aiobotocore-stepfunctions](https://img.shields.io/pypi/v/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-stepfunctions?color=blue)](https://pypistats.org/packages/types-aiobotocore-stepfunctions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-stepfunctions)](https://pepy.tech/project/types-aiobotocore-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SFN 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [types-aiobotocore-stepfunctions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/).
 
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
@@ -329,58 +328,54 @@
 )
 
 
 def check_value(value: ExecutionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_stepfunctions.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_stepfunctions.type_defs import (
     ActivityFailedEventDetailsTypeDef,
     ActivityListItemTypeDef,
     ActivityScheduleFailedEventDetailsTypeDef,
     HistoryEventExecutionDataDetailsTypeDef,
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
-    CreateActivityOutputTypeDef,
+    ResponseMetadataTypeDef,
     RoutingConfigurationListItemTypeDef,
-    CreateStateMachineAliasOutputTypeDef,
     TracingConfigurationTypeDef,
-    CreateStateMachineOutputTypeDef,
     DeleteActivityInputRequestTypeDef,
     DeleteStateMachineAliasInputRequestTypeDef,
     DeleteStateMachineInputRequestTypeDef,
     DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
-    DescribeActivityOutputTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
     DescribeStateMachineAliasInputRequestTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
-    GetActivityTaskOutputTypeDef,
-    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetExecutionHistoryInputRequestTypeDef,
     LambdaFunctionFailedEventDetailsTypeDef,
     LambdaFunctionScheduleFailedEventDetailsTypeDef,
     LambdaFunctionStartFailedEventDetailsTypeDef,
     LambdaFunctionTimedOutEventDetailsTypeDef,
     MapIterationEventDetailsTypeDef,
     MapRunFailedEventDetailsTypeDef,
@@ -388,83 +383,89 @@
     MapStateStartedEventDetailsTypeDef,
     TaskFailedEventDetailsTypeDef,
     TaskStartFailedEventDetailsTypeDef,
     TaskStartedEventDetailsTypeDef,
     TaskSubmitFailedEventDetailsTypeDef,
     TaskTimedOutEventDetailsTypeDef,
     TaskCredentialsTypeDef,
-    ListActivitiesInputListActivitiesPaginateTypeDef,
     ListActivitiesInputRequestTypeDef,
-    ListExecutionsInputListExecutionsPaginateTypeDef,
     ListExecutionsInputRequestTypeDef,
-    ListMapRunsInputListMapRunsPaginateTypeDef,
     ListMapRunsInputRequestTypeDef,
     MapRunListItemTypeDef,
     ListStateMachineAliasesInputRequestTypeDef,
     StateMachineAliasListItemTypeDef,
     ListStateMachineVersionsInputRequestTypeDef,
     StateMachineVersionListItemTypeDef,
-    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PublishStateMachineVersionInputRequestTypeDef,
-    PublishStateMachineVersionOutputTypeDef,
-    ResponseMetadataTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
-    StartExecutionOutputTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
-    StopExecutionOutputTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateMapRunInputRequestTypeDef,
-    UpdateStateMachineAliasOutputTypeDef,
-    UpdateStateMachineOutputTypeDef,
-    ListActivitiesOutputTypeDef,
     ActivityScheduledEventDetailsTypeDef,
     ActivitySucceededEventDetailsTypeDef,
     ExecutionStartedEventDetailsTypeDef,
     ExecutionSucceededEventDetailsTypeDef,
     LambdaFunctionSucceededEventDetailsTypeDef,
     StateEnteredEventDetailsTypeDef,
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
-    DescribeExecutionOutputTypeDef,
-    StartSyncExecutionOutputTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateActivityOutputTypeDef,
+    CreateStateMachineAliasOutputTypeDef,
+    CreateStateMachineOutputTypeDef,
+    DescribeActivityOutputTypeDef,
+    DescribeExecutionOutputTypeDef,
+    GetActivityTaskOutputTypeDef,
+    ListActivitiesOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PublishStateMachineVersionOutputTypeDef,
+    StartExecutionOutputTypeDef,
+    StartSyncExecutionOutputTypeDef,
+    StopExecutionOutputTypeDef,
+    UpdateStateMachineAliasOutputTypeDef,
+    UpdateStateMachineOutputTypeDef,
     CreateStateMachineAliasInputRequestTypeDef,
     DescribeStateMachineAliasOutputTypeDef,
     UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
     ListExecutionsOutputTypeDef,
+    GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
+    ListActivitiesInputListActivitiesPaginateTypeDef,
+    ListExecutionsInputListExecutionsPaginateTypeDef,
+    ListMapRunsInputListMapRunsPaginateTypeDef,
+    ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
+    LoggingConfigurationOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
-    CreateStateMachineInputRequestTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
+    CreateStateMachineInputRequestTypeDef,
+    LoggingConfigurationUnionTypeDef,
     UpdateStateMachineInputRequestTypeDef,
     GetExecutionHistoryOutputTypeDef,
 )
 
 
-def get_structure() -> ActivityFailedEventDetailsTypeDef:
+def get_value() -> ActivityFailedEventDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt` & `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-swf-2.5.2.tar.gz` & `tmp/types-aiobotocore-swf-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-swf-2.5.2.tar", last modified: Sat Jul  8 01:44:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-swf-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:06 2023, max compression
```

## Comparing `types-aiobotocore-swf-2.5.2.tar` & `types-aiobotocore-swf-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:24.914988 types-aiobotocore-swf-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:51.000000 types-aiobotocore-swf-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21854 2023-07-08 01:44:24.914988 types-aiobotocore-swf-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20305 2023-07-08 01:41:51.000000 types-aiobotocore-swf-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:24.914988 types-aiobotocore-swf-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:41:51.000000 types-aiobotocore-swf-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:24.914988 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-08 01:41:51.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-08 01:41:51.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:41:51.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32985 2023-07-08 01:41:52.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32932 2023-07-08 01:41:52.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16003 2023-07-08 01:41:52.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-07-08 01:41:52.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-08 01:41:52.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-08 01:41:52.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:51.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    83956 2023-07-08 01:41:53.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    83799 2023-07-08 01:41:53.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:51.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:24.914988 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21854 2023-07-08 01:44:24.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:44:24.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:24.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:24.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:24.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:24.000000 types-aiobotocore-swf-2.5.2/types_aiobotocore_swf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.649440 types-aiobotocore-swf-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21812 2023-08-02 14:53:06.645440 types-aiobotocore-swf-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20310 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:06.649440 types-aiobotocore-swf-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.637440 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32985 2023-08-02 14:50:30.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32932 2023-08-02 14:50:30.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16003 2023-08-02 14:50:30.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-08-02 14:50:30.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-08-02 14:50:30.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-08-02 14:50:30.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    83962 2023-08-02 14:50:31.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83805 2023-08-02 14:50:31.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.645440 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21812 2023-08-02 14:53:06.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:53:06.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:06.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-swf-2.5.2/LICENSE` & `types-aiobotocore-swf-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2/PKG-INFO` & `types-aiobotocore-swf-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-swf
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SWF 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SWF 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore swf type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore swf type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-swf"></a>
 
 # types-aiobotocore-swf
 
 [![PyPI - types-aiobotocore-swf](https://img.shields.io/pypi/v/types-aiobotocore-swf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-swf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-swf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-swf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-swf?color=blue)](https://pypistats.org/packages/types-aiobotocore-swf)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-swf)](https://pepy.tech/project/types-aiobotocore-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SWF 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [types-aiobotocore-swf docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/).
 
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
@@ -361,43 +360,42 @@
 )
 
 
 def check_value(value: ActivityTaskTimeoutTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_swf.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_swf.type_defs import (
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
     ActivityTypeTypeDef,
     TaskListTypeDef,
     ActivityTaskStartedEventAttributesTypeDef,
-    ActivityTaskStatusTypeDef,
+    ResponseMetadataTypeDef,
     ActivityTaskTimedOutEventAttributesTypeDef,
     WorkflowExecutionTypeDef,
     CancelTimerDecisionAttributesTypeDef,
     CancelTimerFailedEventAttributesTypeDef,
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowTypeTypeDef,
     CloseStatusFilterTypeDef,
     CompleteWorkflowExecutionDecisionAttributesTypeDef,
     CompleteWorkflowExecutionFailedEventAttributesTypeDef,
     ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
-    ExecutionTimeFilterTypeDef,
     TagFilterTypeDef,
     WorkflowExecutionFilterTypeDef,
     WorkflowTypeFilterTypeDef,
     DecisionTaskCompletedEventAttributesTypeDef,
     DecisionTaskStartedEventAttributesTypeDef,
     DecisionTaskTimedOutEventAttributesTypeDef,
     FailWorkflowExecutionDecisionAttributesTypeDef,
@@ -407,16 +405,17 @@
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
     DescribeDomainInputRequestTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
+    PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
     LambdaFunctionStartedEventAttributesTypeDef,
     LambdaFunctionTimedOutEventAttributesTypeDef,
     MarkerRecordedEventAttributesTypeDef,
     RecordMarkerFailedEventAttributesTypeDef,
@@ -432,61 +431,56 @@
     TimerFiredEventAttributesTypeDef,
     TimerStartedEventAttributesTypeDef,
     WorkflowExecutionCanceledEventAttributesTypeDef,
     WorkflowExecutionCompletedEventAttributesTypeDef,
     WorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowExecutionTerminatedEventAttributesTypeDef,
     WorkflowExecutionTimedOutEventAttributesTypeDef,
-    ListActivityTypesInputListActivityTypesPaginateTypeDef,
     ListActivityTypesInputRequestTypeDef,
-    ListDomainsInputListDomainsPaginateTypeDef,
     ListDomainsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ResourceTagTypeDef,
-    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     ListWorkflowTypesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    PendingTaskCountTypeDef,
     RecordActivityTaskHeartbeatInputRequestTypeDef,
     RequestCancelWorkflowExecutionInputRequestTypeDef,
     RespondActivityTaskCanceledInputRequestTypeDef,
     RespondActivityTaskCompletedInputRequestTypeDef,
     RespondActivityTaskFailedInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RunTypeDef,
     SignalWorkflowExecutionInputRequestTypeDef,
     TerminateWorkflowExecutionInputRequestTypeDef,
     UndeprecateDomainInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    WorkflowExecutionCountTypeDef,
     WorkflowExecutionOpenCountsTypeDef,
     ActivityTypeInfoTypeDef,
     DeprecateActivityTypeInputRequestTypeDef,
     DescribeActivityTypeInputRequestTypeDef,
     ScheduleActivityTaskFailedEventAttributesTypeDef,
     UndeprecateActivityTypeInputRequestTypeDef,
     ActivityTaskScheduledEventAttributesTypeDef,
     ActivityTypeConfigurationTypeDef,
     ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
     CountPendingActivityTasksInputRequestTypeDef,
     CountPendingDecisionTasksInputRequestTypeDef,
     DecisionTaskScheduledEventAttributesTypeDef,
     PollForActivityTaskInputRequestTypeDef,
-    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     PollForDecisionTaskInputRequestTypeDef,
     RegisterActivityTypeInputRequestTypeDef,
     RegisterWorkflowTypeInputRequestTypeDef,
     ScheduleActivityTaskDecisionAttributesTypeDef,
     WorkflowExecutionConfigurationTypeDef,
     WorkflowTypeConfigurationTypeDef,
+    ActivityTaskStatusTypeDef,
+    EmptyResponseMetadataTypeDef,
+    PendingTaskCountTypeDef,
+    RunTypeDef,
+    WorkflowExecutionCountTypeDef,
     ActivityTaskTypeDef,
     DescribeWorkflowExecutionInputRequestTypeDef,
     ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
     ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
-    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     GetWorkflowExecutionHistoryInputRequestTypeDef,
     WorkflowExecutionCancelRequestedEventAttributesTypeDef,
     WorkflowExecutionSignaledEventAttributesTypeDef,
     ChildWorkflowExecutionCanceledEventAttributesTypeDef,
     ChildWorkflowExecutionCompletedEventAttributesTypeDef,
     ChildWorkflowExecutionFailedEventAttributesTypeDef,
     ChildWorkflowExecutionStartedEventAttributesTypeDef,
@@ -499,40 +493,46 @@
     StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
     StartWorkflowExecutionInputRequestTypeDef,
     UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
-    CountClosedWorkflowExecutionsInputRequestTypeDef,
-    CountOpenWorkflowExecutionsInputRequestTypeDef,
-    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-    ListClosedWorkflowExecutionsInputRequestTypeDef,
-    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
-    ListOpenWorkflowExecutionsInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
+    ExecutionTimeFilterTypeDef,
+    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+    ListActivityTypesInputListActivityTypesPaginateTypeDef,
+    ListDomainsInputListDomainsPaginateTypeDef,
+    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
     DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
     WorkflowExecutionInfosTypeDef,
     HistoryEventTypeDef,
     WorkflowTypeDetailTypeDef,
     WorkflowTypeInfosTypeDef,
+    CountClosedWorkflowExecutionsInputRequestTypeDef,
+    CountOpenWorkflowExecutionsInputRequestTypeDef,
+    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    ListClosedWorkflowExecutionsInputRequestTypeDef,
+    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    ListOpenWorkflowExecutionsInputRequestTypeDef,
     RespondDecisionTaskCompletedInputRequestTypeDef,
     DecisionTaskTypeDef,
     HistoryTypeDef,
 )
 
 
-def get_structure() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
+def get_value() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-swf-2.5.2/README.md` & `types-aiobotocore-swf-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-swf"></a>
 
 # types-aiobotocore-swf
 
 [![PyPI - types-aiobotocore-swf](https://img.shields.io/pypi/v/types-aiobotocore-swf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-swf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-swf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-swf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-swf?color=blue)](https://pypistats.org/packages/types-aiobotocore-swf)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-swf)](https://pepy.tech/project/types-aiobotocore-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SWF 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [types-aiobotocore-swf docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/).
 
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
@@ -328,43 +328,42 @@
 )
 
 
 def check_value(value: ActivityTaskTimeoutTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_swf.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_swf.type_defs import (
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
     ActivityTypeTypeDef,
     TaskListTypeDef,
     ActivityTaskStartedEventAttributesTypeDef,
-    ActivityTaskStatusTypeDef,
+    ResponseMetadataTypeDef,
     ActivityTaskTimedOutEventAttributesTypeDef,
     WorkflowExecutionTypeDef,
     CancelTimerDecisionAttributesTypeDef,
     CancelTimerFailedEventAttributesTypeDef,
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowTypeTypeDef,
     CloseStatusFilterTypeDef,
     CompleteWorkflowExecutionDecisionAttributesTypeDef,
     CompleteWorkflowExecutionFailedEventAttributesTypeDef,
     ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
-    ExecutionTimeFilterTypeDef,
     TagFilterTypeDef,
     WorkflowExecutionFilterTypeDef,
     WorkflowTypeFilterTypeDef,
     DecisionTaskCompletedEventAttributesTypeDef,
     DecisionTaskStartedEventAttributesTypeDef,
     DecisionTaskTimedOutEventAttributesTypeDef,
     FailWorkflowExecutionDecisionAttributesTypeDef,
@@ -374,16 +373,17 @@
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
     DescribeDomainInputRequestTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
+    PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
     LambdaFunctionStartedEventAttributesTypeDef,
     LambdaFunctionTimedOutEventAttributesTypeDef,
     MarkerRecordedEventAttributesTypeDef,
     RecordMarkerFailedEventAttributesTypeDef,
@@ -399,61 +399,56 @@
     TimerFiredEventAttributesTypeDef,
     TimerStartedEventAttributesTypeDef,
     WorkflowExecutionCanceledEventAttributesTypeDef,
     WorkflowExecutionCompletedEventAttributesTypeDef,
     WorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowExecutionTerminatedEventAttributesTypeDef,
     WorkflowExecutionTimedOutEventAttributesTypeDef,
-    ListActivityTypesInputListActivityTypesPaginateTypeDef,
     ListActivityTypesInputRequestTypeDef,
-    ListDomainsInputListDomainsPaginateTypeDef,
     ListDomainsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ResourceTagTypeDef,
-    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     ListWorkflowTypesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    PendingTaskCountTypeDef,
     RecordActivityTaskHeartbeatInputRequestTypeDef,
     RequestCancelWorkflowExecutionInputRequestTypeDef,
     RespondActivityTaskCanceledInputRequestTypeDef,
     RespondActivityTaskCompletedInputRequestTypeDef,
     RespondActivityTaskFailedInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RunTypeDef,
     SignalWorkflowExecutionInputRequestTypeDef,
     TerminateWorkflowExecutionInputRequestTypeDef,
     UndeprecateDomainInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    WorkflowExecutionCountTypeDef,
     WorkflowExecutionOpenCountsTypeDef,
     ActivityTypeInfoTypeDef,
     DeprecateActivityTypeInputRequestTypeDef,
     DescribeActivityTypeInputRequestTypeDef,
     ScheduleActivityTaskFailedEventAttributesTypeDef,
     UndeprecateActivityTypeInputRequestTypeDef,
     ActivityTaskScheduledEventAttributesTypeDef,
     ActivityTypeConfigurationTypeDef,
     ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
     CountPendingActivityTasksInputRequestTypeDef,
     CountPendingDecisionTasksInputRequestTypeDef,
     DecisionTaskScheduledEventAttributesTypeDef,
     PollForActivityTaskInputRequestTypeDef,
-    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     PollForDecisionTaskInputRequestTypeDef,
     RegisterActivityTypeInputRequestTypeDef,
     RegisterWorkflowTypeInputRequestTypeDef,
     ScheduleActivityTaskDecisionAttributesTypeDef,
     WorkflowExecutionConfigurationTypeDef,
     WorkflowTypeConfigurationTypeDef,
+    ActivityTaskStatusTypeDef,
+    EmptyResponseMetadataTypeDef,
+    PendingTaskCountTypeDef,
+    RunTypeDef,
+    WorkflowExecutionCountTypeDef,
     ActivityTaskTypeDef,
     DescribeWorkflowExecutionInputRequestTypeDef,
     ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
     ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
-    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     GetWorkflowExecutionHistoryInputRequestTypeDef,
     WorkflowExecutionCancelRequestedEventAttributesTypeDef,
     WorkflowExecutionSignaledEventAttributesTypeDef,
     ChildWorkflowExecutionCanceledEventAttributesTypeDef,
     ChildWorkflowExecutionCompletedEventAttributesTypeDef,
     ChildWorkflowExecutionFailedEventAttributesTypeDef,
     ChildWorkflowExecutionStartedEventAttributesTypeDef,
@@ -466,40 +461,46 @@
     StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
     StartWorkflowExecutionInputRequestTypeDef,
     UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
-    CountClosedWorkflowExecutionsInputRequestTypeDef,
-    CountOpenWorkflowExecutionsInputRequestTypeDef,
-    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-    ListClosedWorkflowExecutionsInputRequestTypeDef,
-    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
-    ListOpenWorkflowExecutionsInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
+    ExecutionTimeFilterTypeDef,
+    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+    ListActivityTypesInputListActivityTypesPaginateTypeDef,
+    ListDomainsInputListDomainsPaginateTypeDef,
+    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
     DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
     WorkflowExecutionInfosTypeDef,
     HistoryEventTypeDef,
     WorkflowTypeDetailTypeDef,
     WorkflowTypeInfosTypeDef,
+    CountClosedWorkflowExecutionsInputRequestTypeDef,
+    CountOpenWorkflowExecutionsInputRequestTypeDef,
+    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    ListClosedWorkflowExecutionsInputRequestTypeDef,
+    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    ListOpenWorkflowExecutionsInputRequestTypeDef,
     RespondDecisionTaskCompletedInputRequestTypeDef,
     DecisionTaskTypeDef,
     HistoryTypeDef,
 )
 
 
-def get_structure() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
+def get_value() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-swf-2.5.2/setup.py` & `types-aiobotocore-swf-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-swf",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_swf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SWF 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore swf type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore swf type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_swf": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/__init__.py` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/__init__.pyi` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/__main__.py` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SWF 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SWF 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF\nOther"
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

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/client.py` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/client.pyi` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/literals.py` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/literals.pyi` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/paginator.py` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
     def paginate(
         self,
         *,
         domain: str,
         execution: WorkflowExecutionTypeDef,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[HistoryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.GetWorkflowExecutionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#getworkflowexecutionhistorypaginator)
         """
 
 
@@ -105,15 +105,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ActivityTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListActivityTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listactivitytypespaginator)
         """
 
 
@@ -130,15 +130,15 @@
         startTimeFilter: ExecutionTimeFilterTypeDef = ...,
         closeTimeFilter: ExecutionTimeFilterTypeDef = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
         closeStatusFilter: CloseStatusFilterTypeDef = ...,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListClosedWorkflowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listclosedworkflowexecutionspaginator)
         """
 
 
@@ -149,15 +149,15 @@
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DomainInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listdomainspaginator)
         """
 
 
@@ -172,15 +172,15 @@
         *,
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListOpenWorkflowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listopenworkflowexecutionspaginator)
         """
 
 
@@ -193,15 +193,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[WorkflowTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListWorkflowTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listworkflowtypespaginator)
         """
 
 
@@ -215,13 +215,13 @@
         self,
         *,
         domain: str,
         taskList: TaskListTypeDef,
         identity: str = ...,
         reverseOrder: bool = ...,
         startAtPreviousStartedEvent: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DecisionTaskTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.PollForDecisionTask.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#pollfordecisiontaskpaginator)
         """
```

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/paginator.pyi` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     def paginate(
         self,
         *,
         domain: str,
         execution: WorkflowExecutionTypeDef,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[HistoryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.GetWorkflowExecutionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#getworkflowexecutionhistorypaginator)
         """
 
 class ListActivityTypesPaginator(AioPaginator):
@@ -101,15 +101,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ActivityTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListActivityTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listactivitytypespaginator)
         """
 
 class ListClosedWorkflowExecutionsPaginator(AioPaginator):
@@ -125,15 +125,15 @@
         startTimeFilter: ExecutionTimeFilterTypeDef = ...,
         closeTimeFilter: ExecutionTimeFilterTypeDef = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
         closeStatusFilter: CloseStatusFilterTypeDef = ...,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListClosedWorkflowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listclosedworkflowexecutionspaginator)
         """
 
 class ListDomainsPaginator(AioPaginator):
@@ -143,15 +143,15 @@
     """
 
     def paginate(
         self,
         *,
         registrationStatus: RegistrationStatusType,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DomainInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listdomainspaginator)
         """
 
 class ListOpenWorkflowExecutionsPaginator(AioPaginator):
@@ -165,15 +165,15 @@
         *,
         domain: str,
         startTimeFilter: ExecutionTimeFilterTypeDef,
         typeFilter: WorkflowTypeFilterTypeDef = ...,
         tagFilter: TagFilterTypeDef = ...,
         reverseOrder: bool = ...,
         executionFilter: WorkflowExecutionFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[WorkflowExecutionInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListOpenWorkflowExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listopenworkflowexecutionspaginator)
         """
 
 class ListWorkflowTypesPaginator(AioPaginator):
@@ -185,15 +185,15 @@
     def paginate(
         self,
         *,
         domain: str,
         registrationStatus: RegistrationStatusType,
         name: str = ...,
         reverseOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[WorkflowTypeInfosTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListWorkflowTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#listworkflowtypespaginator)
         """
 
 class PollForDecisionTaskPaginator(AioPaginator):
@@ -206,13 +206,13 @@
         self,
         *,
         domain: str,
         taskList: TaskListTypeDef,
         identity: str = ...,
         reverseOrder: bool = ...,
         startAtPreviousStartedEvent: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DecisionTaskTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.PollForDecisionTask.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/paginators/#pollfordecisiontaskpaginator)
         """
```

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/type_defs.py` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_swf.type_defs import ActivityTaskCancelRequestedEventAttributesTypeDef
 
-    data: ActivityTaskCancelRequestedEventAttributesTypeDef = {...}
+    data: ActivityTaskCancelRequestedEventAttributesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -52,27 +52,26 @@
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     "ActivityTaskCanceledEventAttributesTypeDef",
     "ActivityTaskCompletedEventAttributesTypeDef",
     "ActivityTaskFailedEventAttributesTypeDef",
     "ActivityTypeTypeDef",
     "TaskListTypeDef",
     "ActivityTaskStartedEventAttributesTypeDef",
-    "ActivityTaskStatusTypeDef",
+    "ResponseMetadataTypeDef",
     "ActivityTaskTimedOutEventAttributesTypeDef",
     "WorkflowExecutionTypeDef",
     "CancelTimerDecisionAttributesTypeDef",
     "CancelTimerFailedEventAttributesTypeDef",
     "CancelWorkflowExecutionDecisionAttributesTypeDef",
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowTypeTypeDef",
     "CloseStatusFilterTypeDef",
     "CompleteWorkflowExecutionDecisionAttributesTypeDef",
     "CompleteWorkflowExecutionFailedEventAttributesTypeDef",
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
-    "ExecutionTimeFilterTypeDef",
     "TagFilterTypeDef",
     "WorkflowExecutionFilterTypeDef",
     "WorkflowTypeFilterTypeDef",
     "DecisionTaskCompletedEventAttributesTypeDef",
     "DecisionTaskStartedEventAttributesTypeDef",
     "DecisionTaskTimedOutEventAttributesTypeDef",
     "FailWorkflowExecutionDecisionAttributesTypeDef",
@@ -82,16 +81,17 @@
     "ScheduleLambdaFunctionDecisionAttributesTypeDef",
     "SignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     "StartTimerDecisionAttributesTypeDef",
     "DeprecateDomainInputRequestTypeDef",
     "DescribeDomainInputRequestTypeDef",
     "DomainConfigurationTypeDef",
     "DomainInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
+    "PaginatorConfigTypeDef",
     "LambdaFunctionCompletedEventAttributesTypeDef",
     "LambdaFunctionFailedEventAttributesTypeDef",
     "LambdaFunctionScheduledEventAttributesTypeDef",
     "LambdaFunctionStartedEventAttributesTypeDef",
     "LambdaFunctionTimedOutEventAttributesTypeDef",
     "MarkerRecordedEventAttributesTypeDef",
     "RecordMarkerFailedEventAttributesTypeDef",
@@ -107,61 +107,56 @@
     "TimerFiredEventAttributesTypeDef",
     "TimerStartedEventAttributesTypeDef",
     "WorkflowExecutionCanceledEventAttributesTypeDef",
     "WorkflowExecutionCompletedEventAttributesTypeDef",
     "WorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowExecutionTerminatedEventAttributesTypeDef",
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
-    "ListActivityTypesInputListActivityTypesPaginateTypeDef",
     "ListActivityTypesInputRequestTypeDef",
-    "ListDomainsInputListDomainsPaginateTypeDef",
     "ListDomainsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ResourceTagTypeDef",
-    "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     "ListWorkflowTypesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "PendingTaskCountTypeDef",
     "RecordActivityTaskHeartbeatInputRequestTypeDef",
     "RequestCancelWorkflowExecutionInputRequestTypeDef",
     "RespondActivityTaskCanceledInputRequestTypeDef",
     "RespondActivityTaskCompletedInputRequestTypeDef",
     "RespondActivityTaskFailedInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "RunTypeDef",
     "SignalWorkflowExecutionInputRequestTypeDef",
     "TerminateWorkflowExecutionInputRequestTypeDef",
     "UndeprecateDomainInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "WorkflowExecutionCountTypeDef",
     "WorkflowExecutionOpenCountsTypeDef",
     "ActivityTypeInfoTypeDef",
     "DeprecateActivityTypeInputRequestTypeDef",
     "DescribeActivityTypeInputRequestTypeDef",
     "ScheduleActivityTaskFailedEventAttributesTypeDef",
     "UndeprecateActivityTypeInputRequestTypeDef",
     "ActivityTaskScheduledEventAttributesTypeDef",
     "ActivityTypeConfigurationTypeDef",
     "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
     "CountPendingActivityTasksInputRequestTypeDef",
     "CountPendingDecisionTasksInputRequestTypeDef",
     "DecisionTaskScheduledEventAttributesTypeDef",
     "PollForActivityTaskInputRequestTypeDef",
-    "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "PollForDecisionTaskInputRequestTypeDef",
     "RegisterActivityTypeInputRequestTypeDef",
     "RegisterWorkflowTypeInputRequestTypeDef",
     "ScheduleActivityTaskDecisionAttributesTypeDef",
     "WorkflowExecutionConfigurationTypeDef",
     "WorkflowTypeConfigurationTypeDef",
+    "ActivityTaskStatusTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "PendingTaskCountTypeDef",
+    "RunTypeDef",
+    "WorkflowExecutionCountTypeDef",
     "ActivityTaskTypeDef",
     "DescribeWorkflowExecutionInputRequestTypeDef",
     "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
-    "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     "GetWorkflowExecutionHistoryInputRequestTypeDef",
     "WorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "WorkflowExecutionSignaledEventAttributesTypeDef",
     "ChildWorkflowExecutionCanceledEventAttributesTypeDef",
     "ChildWorkflowExecutionCompletedEventAttributesTypeDef",
     "ChildWorkflowExecutionFailedEventAttributesTypeDef",
     "ChildWorkflowExecutionStartedEventAttributesTypeDef",
@@ -174,33 +169,39 @@
     "StartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
     "StartWorkflowExecutionInputRequestTypeDef",
     "UndeprecateWorkflowTypeInputRequestTypeDef",
     "WorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     "WorkflowExecutionInfoTypeDef",
     "WorkflowExecutionStartedEventAttributesTypeDef",
     "WorkflowTypeInfoTypeDef",
-    "CountClosedWorkflowExecutionsInputRequestTypeDef",
-    "CountOpenWorkflowExecutionsInputRequestTypeDef",
-    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
-    "ListClosedWorkflowExecutionsInputRequestTypeDef",
-    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
-    "ListOpenWorkflowExecutionsInputRequestTypeDef",
     "DomainDetailTypeDef",
     "DomainInfosTypeDef",
+    "ExecutionTimeFilterTypeDef",
+    "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+    "ListActivityTypesInputListActivityTypesPaginateTypeDef",
+    "ListDomainsInputListDomainsPaginateTypeDef",
+    "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+    "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "RegisterDomainInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ActivityTypeInfosTypeDef",
     "ActivityTypeDetailTypeDef",
     "DecisionTypeDef",
     "WorkflowExecutionDetailTypeDef",
     "WorkflowExecutionInfosTypeDef",
     "HistoryEventTypeDef",
     "WorkflowTypeDetailTypeDef",
     "WorkflowTypeInfosTypeDef",
+    "CountClosedWorkflowExecutionsInputRequestTypeDef",
+    "CountOpenWorkflowExecutionsInputRequestTypeDef",
+    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    "ListClosedWorkflowExecutionsInputRequestTypeDef",
+    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    "ListOpenWorkflowExecutionsInputRequestTypeDef",
     "RespondDecisionTaskCompletedInputRequestTypeDef",
     "DecisionTaskTypeDef",
     "HistoryTypeDef",
 )
 
 ActivityTaskCancelRequestedEventAttributesTypeDef = TypedDict(
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
@@ -314,19 +315,22 @@
 class ActivityTaskStartedEventAttributesTypeDef(
     _RequiredActivityTaskStartedEventAttributesTypeDef,
     _OptionalActivityTaskStartedEventAttributesTypeDef,
 ):
     pass
 
 
-ActivityTaskStatusTypeDef = TypedDict(
-    "ActivityTaskStatusTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "cancelRequested": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredActivityTaskTimedOutEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskTimedOutEventAttributesTypeDef",
     {
         "timeoutType": ActivityTaskTimeoutTypeType,
@@ -425,35 +429,14 @@
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": ContinueAsNewWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
-_RequiredExecutionTimeFilterTypeDef = TypedDict(
-    "_RequiredExecutionTimeFilterTypeDef",
-    {
-        "oldestDate": Union[datetime, str],
-    },
-)
-_OptionalExecutionTimeFilterTypeDef = TypedDict(
-    "_OptionalExecutionTimeFilterTypeDef",
-    {
-        "latestDate": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class ExecutionTimeFilterTypeDef(
-    _RequiredExecutionTimeFilterTypeDef, _OptionalExecutionTimeFilterTypeDef
-):
-    pass
-
-
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "tag": str,
     },
 )
 
@@ -709,29 +692,33 @@
 )
 
 
 class DomainInfoTypeDef(_RequiredDomainInfoTypeDef, _OptionalDomainInfoTypeDef):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 FailWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": FailWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
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
 _RequiredLambdaFunctionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -1137,39 +1124,14 @@
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
         "childPolicy": ChildPolicyType,
     },
 )
 
-_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
-    "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
-    {
-        "domain": str,
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
-    "_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef",
-    {
-        "name": str,
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListActivityTypesInputListActivityTypesPaginateTypeDef(
-    _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
-    _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListActivityTypesInputRequestTypeDef = TypedDict(
     "_RequiredListActivityTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1187,37 +1149,14 @@
 
 class ListActivityTypesInputRequestTypeDef(
     _RequiredListActivityTypesInputRequestTypeDef, _OptionalListActivityTypesInputRequestTypeDef
 ):
     pass
 
 
-_RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
-    "_RequiredListDomainsInputListDomainsPaginateTypeDef",
-    {
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
-    "_OptionalListDomainsInputListDomainsPaginateTypeDef",
-    {
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDomainsInputListDomainsPaginateTypeDef(
-    _RequiredListDomainsInputListDomainsPaginateTypeDef,
-    _OptionalListDomainsInputListDomainsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDomainsInputRequestTypeDef = TypedDict(
     "_RequiredListDomainsInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
     },
 )
 _OptionalListDomainsInputRequestTypeDef = TypedDict(
@@ -1259,39 +1198,14 @@
 )
 
 
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
 
-_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
-    {
-        "domain": str,
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
-    {
-        "name": str,
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
-    _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
-    _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListWorkflowTypesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkflowTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1309,33 +1223,14 @@
 
 class ListWorkflowTypesInputRequestTypeDef(
     _RequiredListWorkflowTypesInputRequestTypeDef, _OptionalListWorkflowTypesInputRequestTypeDef
 ):
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
-PendingTaskCountTypeDef = TypedDict(
-    "PendingTaskCountTypeDef",
-    {
-        "count": int,
-        "truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
     "_RequiredRecordActivityTaskHeartbeatInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
@@ -1440,33 +1335,14 @@
 class RespondActivityTaskFailedInputRequestTypeDef(
     _RequiredRespondActivityTaskFailedInputRequestTypeDef,
     _OptionalRespondActivityTaskFailedInputRequestTypeDef,
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
-RunTypeDef = TypedDict(
-    "RunTypeDef",
-    {
-        "runId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSignalWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredSignalWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
         "signalName": str,
     },
@@ -1525,23 +1401,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-WorkflowExecutionCountTypeDef = TypedDict(
-    "WorkflowExecutionCountTypeDef",
-    {
-        "count": int,
-        "truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredWorkflowExecutionOpenCountsTypeDef = TypedDict(
     "_RequiredWorkflowExecutionOpenCountsTypeDef",
     {
         "openActivityTasks": int,
         "openDecisionTasks": int,
         "openTimers": int,
         "openChildWorkflowExecutions": int,
@@ -1735,40 +1602,14 @@
 
 class PollForActivityTaskInputRequestTypeDef(
     _RequiredPollForActivityTaskInputRequestTypeDef, _OptionalPollForActivityTaskInputRequestTypeDef
 ):
     pass
 
 
-_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
-    "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
-    "_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
-    {
-        "identity": str,
-        "reverseOrder": bool,
-        "startAtPreviousStartedEvent": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
-    _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-    _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-):
-    pass
-
-
 _RequiredPollForDecisionTaskInputRequestTypeDef = TypedDict(
     "_RequiredPollForDecisionTaskInputRequestTypeDef",
     {
         "domain": str,
         "taskList": TaskListTypeDef,
     },
 )
@@ -1915,24 +1756,65 @@
         "defaultTaskPriority": str,
         "defaultChildPolicy": ChildPolicyType,
         "defaultLambdaRole": str,
     },
     total=False,
 )
 
+ActivityTaskStatusTypeDef = TypedDict(
+    "ActivityTaskStatusTypeDef",
+    {
+        "cancelRequested": bool,
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
+PendingTaskCountTypeDef = TypedDict(
+    "PendingTaskCountTypeDef",
+    {
+        "count": int,
+        "truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RunTypeDef = TypedDict(
+    "RunTypeDef",
+    {
+        "runId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+WorkflowExecutionCountTypeDef = TypedDict(
+    "WorkflowExecutionCountTypeDef",
+    {
+        "count": int,
+        "truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ActivityTaskTypeDef = TypedDict(
     "ActivityTaskTypeDef",
     {
         "taskToken": str,
         "activityId": str,
         "startedEventId": int,
         "workflowExecution": WorkflowExecutionTypeDef,
         "activityType": ActivityTypeTypeDef,
         "input": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkflowExecutionInputRequestTypeDef = TypedDict(
     "DescribeWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
@@ -1952,38 +1834,14 @@
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
     {
         "workflowExecution": WorkflowExecutionTypeDef,
         "initiatedEventId": int,
     },
 )
 
-_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
-    },
-)
-_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    {
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
-    _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-    _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef",
     {
         "domain": str,
         "execution": WorkflowExecutionTypeDef,
     },
 )
@@ -2398,203 +2256,181 @@
 )
 
 
 class WorkflowTypeInfoTypeDef(_RequiredWorkflowTypeInfoTypeDef, _OptionalWorkflowTypeInfoTypeDef):
     pass
 
 
-_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef",
+DomainDetailTypeDef = TypedDict(
+    "DomainDetailTypeDef",
     {
-        "domain": str,
+        "domainInfo": DomainInfoTypeDef,
+        "configuration": DomainConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef",
+
+DomainInfosTypeDef = TypedDict(
+    "DomainInfosTypeDef",
     {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
+        "domainInfos": List[DomainInfoTypeDef],
+        "nextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CountClosedWorkflowExecutionsInputRequestTypeDef(
-    _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef,
-    _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef",
+_RequiredExecutionTimeFilterTypeDef = TypedDict(
+    "_RequiredExecutionTimeFilterTypeDef",
     {
-        "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "oldestDate": TimestampTypeDef,
     },
 )
-_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef",
+_OptionalExecutionTimeFilterTypeDef = TypedDict(
+    "_OptionalExecutionTimeFilterTypeDef",
     {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "latestDate": TimestampTypeDef,
     },
     total=False,
 )
 
 
-class CountOpenWorkflowExecutionsInputRequestTypeDef(
-    _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
-    _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
+class ExecutionTimeFilterTypeDef(
+    _RequiredExecutionTimeFilterTypeDef, _OptionalExecutionTimeFilterTypeDef
 ):
     pass
 
 
-_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     {
         "domain": str,
+        "execution": WorkflowExecutionTypeDef,
     },
 )
-_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
         "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
+    _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+    _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
+_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
+    "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
     {
         "domain": str,
+        "registrationStatus": RegistrationStatusType,
     },
 )
-_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
+_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
+    "_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef",
     {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
+        "name": str,
         "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListClosedWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
+class ListActivityTypesInputListActivityTypesPaginateTypeDef(
+    _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
+    _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+_RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
+    "_RequiredListDomainsInputListDomainsPaginateTypeDef",
     {
-        "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "registrationStatus": RegistrationStatusType,
     },
 )
-_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+_OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
+    "_OptionalListDomainsInputListDomainsPaginateTypeDef",
     {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
         "reverseOrder": bool,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
-    _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
-    _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+class ListDomainsInputListDomainsPaginateTypeDef(
+    _RequiredListDomainsInputListDomainsPaginateTypeDef,
+    _OptionalListDomainsInputListDomainsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
+_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     {
         "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "registrationStatus": RegistrationStatusType,
     },
 )
-_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
+_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
+        "name": str,
         "reverseOrder": bool,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListOpenWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
+class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
+    _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
 ):
     pass
 
 
-DomainDetailTypeDef = TypedDict(
-    "DomainDetailTypeDef",
+_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
+    "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     {
-        "domainInfo": DomainInfoTypeDef,
-        "configuration": DomainConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "domain": str,
+        "taskList": TaskListTypeDef,
     },
 )
-
-DomainInfosTypeDef = TypedDict(
-    "DomainInfosTypeDef",
+_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
+    "_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     {
-        "domainInfos": List[DomainInfoTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "identity": str,
+        "reverseOrder": bool,
+        "startAtPreviousStartedEvent": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
+    _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
+    _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
+):
+    pass
+
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterDomainInputRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainInputRequestTypeDef",
     {
         "name": str,
@@ -2626,24 +2462,24 @@
 )
 
 ActivityTypeInfosTypeDef = TypedDict(
     "ActivityTypeInfosTypeDef",
     {
         "typeInfos": List[ActivityTypeInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActivityTypeDetailTypeDef = TypedDict(
     "ActivityTypeDetailTypeDef",
     {
         "typeInfo": ActivityTypeInfoTypeDef,
         "configuration": ActivityTypeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDecisionTypeDef = TypedDict(
     "_RequiredDecisionTypeDef",
     {
         "decisionType": DecisionTypeType,
@@ -2692,24 +2528,24 @@
     "WorkflowExecutionDetailTypeDef",
     {
         "executionInfo": WorkflowExecutionInfoTypeDef,
         "executionConfiguration": WorkflowExecutionConfigurationTypeDef,
         "openCounts": WorkflowExecutionOpenCountsTypeDef,
         "latestActivityTaskTimestamp": datetime,
         "latestExecutionContext": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkflowExecutionInfosTypeDef = TypedDict(
     "WorkflowExecutionInfosTypeDef",
     {
         "executionInfos": List[WorkflowExecutionInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHistoryEventTypeDef = TypedDict(
     "_RequiredHistoryEventTypeDef",
     {
         "eventTimestamp": datetime,
@@ -2836,27 +2672,193 @@
 
 
 WorkflowTypeDetailTypeDef = TypedDict(
     "WorkflowTypeDetailTypeDef",
     {
         "typeInfo": WorkflowTypeInfoTypeDef,
         "configuration": WorkflowTypeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkflowTypeInfosTypeDef = TypedDict(
     "WorkflowTypeInfosTypeDef",
     {
         "typeInfos": List[WorkflowTypeInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class CountClosedWorkflowExecutionsInputRequestTypeDef(
+    _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef,
+    _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class CountOpenWorkflowExecutionsInputRequestTypeDef(
+    _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
+    _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+    },
+    total=False,
+)
+
+
+class ListClosedWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "reverseOrder": bool,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
+    _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class ListOpenWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+
 _RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
     "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
@@ -2882,19 +2884,19 @@
         "taskToken": str,
         "startedEventId": int,
         "workflowExecution": WorkflowExecutionTypeDef,
         "workflowType": WorkflowTypeTypeDef,
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
         "previousStartedEventId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HistoryTypeDef = TypedDict(
     "HistoryTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf/type_defs.pyi` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_swf.type_defs import ActivityTaskCancelRequestedEventAttributesTypeDef
 
-    data: ActivityTaskCancelRequestedEventAttributesTypeDef = {...}
+    data: ActivityTaskCancelRequestedEventAttributesTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -51,27 +51,26 @@
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
     "ActivityTaskCanceledEventAttributesTypeDef",
     "ActivityTaskCompletedEventAttributesTypeDef",
     "ActivityTaskFailedEventAttributesTypeDef",
     "ActivityTypeTypeDef",
     "TaskListTypeDef",
     "ActivityTaskStartedEventAttributesTypeDef",
-    "ActivityTaskStatusTypeDef",
+    "ResponseMetadataTypeDef",
     "ActivityTaskTimedOutEventAttributesTypeDef",
     "WorkflowExecutionTypeDef",
     "CancelTimerDecisionAttributesTypeDef",
     "CancelTimerFailedEventAttributesTypeDef",
     "CancelWorkflowExecutionDecisionAttributesTypeDef",
     "CancelWorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowTypeTypeDef",
     "CloseStatusFilterTypeDef",
     "CompleteWorkflowExecutionDecisionAttributesTypeDef",
     "CompleteWorkflowExecutionFailedEventAttributesTypeDef",
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
-    "ExecutionTimeFilterTypeDef",
     "TagFilterTypeDef",
     "WorkflowExecutionFilterTypeDef",
     "WorkflowTypeFilterTypeDef",
     "DecisionTaskCompletedEventAttributesTypeDef",
     "DecisionTaskStartedEventAttributesTypeDef",
     "DecisionTaskTimedOutEventAttributesTypeDef",
     "FailWorkflowExecutionDecisionAttributesTypeDef",
@@ -81,16 +80,17 @@
     "ScheduleLambdaFunctionDecisionAttributesTypeDef",
     "SignalExternalWorkflowExecutionDecisionAttributesTypeDef",
     "StartTimerDecisionAttributesTypeDef",
     "DeprecateDomainInputRequestTypeDef",
     "DescribeDomainInputRequestTypeDef",
     "DomainConfigurationTypeDef",
     "DomainInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
+    "PaginatorConfigTypeDef",
     "LambdaFunctionCompletedEventAttributesTypeDef",
     "LambdaFunctionFailedEventAttributesTypeDef",
     "LambdaFunctionScheduledEventAttributesTypeDef",
     "LambdaFunctionStartedEventAttributesTypeDef",
     "LambdaFunctionTimedOutEventAttributesTypeDef",
     "MarkerRecordedEventAttributesTypeDef",
     "RecordMarkerFailedEventAttributesTypeDef",
@@ -106,61 +106,56 @@
     "TimerFiredEventAttributesTypeDef",
     "TimerStartedEventAttributesTypeDef",
     "WorkflowExecutionCanceledEventAttributesTypeDef",
     "WorkflowExecutionCompletedEventAttributesTypeDef",
     "WorkflowExecutionFailedEventAttributesTypeDef",
     "WorkflowExecutionTerminatedEventAttributesTypeDef",
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
-    "ListActivityTypesInputListActivityTypesPaginateTypeDef",
     "ListActivityTypesInputRequestTypeDef",
-    "ListDomainsInputListDomainsPaginateTypeDef",
     "ListDomainsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ResourceTagTypeDef",
-    "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     "ListWorkflowTypesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "PendingTaskCountTypeDef",
     "RecordActivityTaskHeartbeatInputRequestTypeDef",
     "RequestCancelWorkflowExecutionInputRequestTypeDef",
     "RespondActivityTaskCanceledInputRequestTypeDef",
     "RespondActivityTaskCompletedInputRequestTypeDef",
     "RespondActivityTaskFailedInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "RunTypeDef",
     "SignalWorkflowExecutionInputRequestTypeDef",
     "TerminateWorkflowExecutionInputRequestTypeDef",
     "UndeprecateDomainInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "WorkflowExecutionCountTypeDef",
     "WorkflowExecutionOpenCountsTypeDef",
     "ActivityTypeInfoTypeDef",
     "DeprecateActivityTypeInputRequestTypeDef",
     "DescribeActivityTypeInputRequestTypeDef",
     "ScheduleActivityTaskFailedEventAttributesTypeDef",
     "UndeprecateActivityTypeInputRequestTypeDef",
     "ActivityTaskScheduledEventAttributesTypeDef",
     "ActivityTypeConfigurationTypeDef",
     "ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef",
     "CountPendingActivityTasksInputRequestTypeDef",
     "CountPendingDecisionTasksInputRequestTypeDef",
     "DecisionTaskScheduledEventAttributesTypeDef",
     "PollForActivityTaskInputRequestTypeDef",
-    "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "PollForDecisionTaskInputRequestTypeDef",
     "RegisterActivityTypeInputRequestTypeDef",
     "RegisterWorkflowTypeInputRequestTypeDef",
     "ScheduleActivityTaskDecisionAttributesTypeDef",
     "WorkflowExecutionConfigurationTypeDef",
     "WorkflowTypeConfigurationTypeDef",
+    "ActivityTaskStatusTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "PendingTaskCountTypeDef",
+    "RunTypeDef",
+    "WorkflowExecutionCountTypeDef",
     "ActivityTaskTypeDef",
     "DescribeWorkflowExecutionInputRequestTypeDef",
     "ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
-    "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     "GetWorkflowExecutionHistoryInputRequestTypeDef",
     "WorkflowExecutionCancelRequestedEventAttributesTypeDef",
     "WorkflowExecutionSignaledEventAttributesTypeDef",
     "ChildWorkflowExecutionCanceledEventAttributesTypeDef",
     "ChildWorkflowExecutionCompletedEventAttributesTypeDef",
     "ChildWorkflowExecutionFailedEventAttributesTypeDef",
     "ChildWorkflowExecutionStartedEventAttributesTypeDef",
@@ -173,33 +168,39 @@
     "StartChildWorkflowExecutionInitiatedEventAttributesTypeDef",
     "StartWorkflowExecutionInputRequestTypeDef",
     "UndeprecateWorkflowTypeInputRequestTypeDef",
     "WorkflowExecutionContinuedAsNewEventAttributesTypeDef",
     "WorkflowExecutionInfoTypeDef",
     "WorkflowExecutionStartedEventAttributesTypeDef",
     "WorkflowTypeInfoTypeDef",
-    "CountClosedWorkflowExecutionsInputRequestTypeDef",
-    "CountOpenWorkflowExecutionsInputRequestTypeDef",
-    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
-    "ListClosedWorkflowExecutionsInputRequestTypeDef",
-    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
-    "ListOpenWorkflowExecutionsInputRequestTypeDef",
     "DomainDetailTypeDef",
     "DomainInfosTypeDef",
+    "ExecutionTimeFilterTypeDef",
+    "GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
+    "ListActivityTypesInputListActivityTypesPaginateTypeDef",
+    "ListDomainsInputListDomainsPaginateTypeDef",
+    "ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
+    "PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "RegisterDomainInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ActivityTypeInfosTypeDef",
     "ActivityTypeDetailTypeDef",
     "DecisionTypeDef",
     "WorkflowExecutionDetailTypeDef",
     "WorkflowExecutionInfosTypeDef",
     "HistoryEventTypeDef",
     "WorkflowTypeDetailTypeDef",
     "WorkflowTypeInfosTypeDef",
+    "CountClosedWorkflowExecutionsInputRequestTypeDef",
+    "CountOpenWorkflowExecutionsInputRequestTypeDef",
+    "ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    "ListClosedWorkflowExecutionsInputRequestTypeDef",
+    "ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    "ListOpenWorkflowExecutionsInputRequestTypeDef",
     "RespondDecisionTaskCompletedInputRequestTypeDef",
     "DecisionTaskTypeDef",
     "HistoryTypeDef",
 )
 
 ActivityTaskCancelRequestedEventAttributesTypeDef = TypedDict(
     "ActivityTaskCancelRequestedEventAttributesTypeDef",
@@ -305,19 +306,22 @@
 
 class ActivityTaskStartedEventAttributesTypeDef(
     _RequiredActivityTaskStartedEventAttributesTypeDef,
     _OptionalActivityTaskStartedEventAttributesTypeDef,
 ):
     pass
 
-ActivityTaskStatusTypeDef = TypedDict(
-    "ActivityTaskStatusTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "cancelRequested": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredActivityTaskTimedOutEventAttributesTypeDef = TypedDict(
     "_RequiredActivityTaskTimedOutEventAttributesTypeDef",
     {
         "timeoutType": ActivityTaskTimeoutTypeType,
@@ -414,33 +418,14 @@
     "ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": ContinueAsNewWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
 )
 
-_RequiredExecutionTimeFilterTypeDef = TypedDict(
-    "_RequiredExecutionTimeFilterTypeDef",
-    {
-        "oldestDate": Union[datetime, str],
-    },
-)
-_OptionalExecutionTimeFilterTypeDef = TypedDict(
-    "_OptionalExecutionTimeFilterTypeDef",
-    {
-        "latestDate": Union[datetime, str],
-    },
-    total=False,
-)
-
-class ExecutionTimeFilterTypeDef(
-    _RequiredExecutionTimeFilterTypeDef, _OptionalExecutionTimeFilterTypeDef
-):
-    pass
-
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "tag": str,
     },
 )
 
@@ -678,29 +663,33 @@
     },
     total=False,
 )
 
 class DomainInfoTypeDef(_RequiredDomainInfoTypeDef, _OptionalDomainInfoTypeDef):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 FailWorkflowExecutionFailedEventAttributesTypeDef = TypedDict(
     "FailWorkflowExecutionFailedEventAttributesTypeDef",
     {
         "cause": FailWorkflowExecutionFailedCauseType,
         "decisionTaskCompletedEventId": int,
     },
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
 _RequiredLambdaFunctionCompletedEventAttributesTypeDef = TypedDict(
     "_RequiredLambdaFunctionCompletedEventAttributesTypeDef",
     {
         "scheduledEventId": int,
         "startedEventId": int,
     },
 )
@@ -1078,37 +1067,14 @@
     "WorkflowExecutionTimedOutEventAttributesTypeDef",
     {
         "timeoutType": Literal["START_TO_CLOSE"],
         "childPolicy": ChildPolicyType,
     },
 )
 
-_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
-    "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
-    {
-        "domain": str,
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
-    "_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef",
-    {
-        "name": str,
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListActivityTypesInputListActivityTypesPaginateTypeDef(
-    _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
-    _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
-):
-    pass
-
 _RequiredListActivityTypesInputRequestTypeDef = TypedDict(
     "_RequiredListActivityTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1124,35 +1090,14 @@
 )
 
 class ListActivityTypesInputRequestTypeDef(
     _RequiredListActivityTypesInputRequestTypeDef, _OptionalListActivityTypesInputRequestTypeDef
 ):
     pass
 
-_RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
-    "_RequiredListDomainsInputListDomainsPaginateTypeDef",
-    {
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
-    "_OptionalListDomainsInputListDomainsPaginateTypeDef",
-    {
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDomainsInputListDomainsPaginateTypeDef(
-    _RequiredListDomainsInputListDomainsPaginateTypeDef,
-    _OptionalListDomainsInputListDomainsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDomainsInputRequestTypeDef = TypedDict(
     "_RequiredListDomainsInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
     },
 )
 _OptionalListDomainsInputRequestTypeDef = TypedDict(
@@ -1190,37 +1135,14 @@
     },
     total=False,
 )
 
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
-_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
-    "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
-    {
-        "domain": str,
-        "registrationStatus": RegistrationStatusType,
-    },
-)
-_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
-    "_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
-    {
-        "name": str,
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
-    _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
-    _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
-):
-    pass
-
 _RequiredListWorkflowTypesInputRequestTypeDef = TypedDict(
     "_RequiredListWorkflowTypesInputRequestTypeDef",
     {
         "domain": str,
         "registrationStatus": RegistrationStatusType,
     },
 )
@@ -1236,33 +1158,14 @@
 )
 
 class ListWorkflowTypesInputRequestTypeDef(
     _RequiredListWorkflowTypesInputRequestTypeDef, _OptionalListWorkflowTypesInputRequestTypeDef
 ):
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
-PendingTaskCountTypeDef = TypedDict(
-    "PendingTaskCountTypeDef",
-    {
-        "count": int,
-        "truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
     "_RequiredRecordActivityTaskHeartbeatInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRecordActivityTaskHeartbeatInputRequestTypeDef = TypedDict(
@@ -1357,33 +1260,14 @@
 
 class RespondActivityTaskFailedInputRequestTypeDef(
     _RequiredRespondActivityTaskFailedInputRequestTypeDef,
     _OptionalRespondActivityTaskFailedInputRequestTypeDef,
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
-RunTypeDef = TypedDict(
-    "RunTypeDef",
-    {
-        "runId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSignalWorkflowExecutionInputRequestTypeDef = TypedDict(
     "_RequiredSignalWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
         "workflowId": str,
         "signalName": str,
     },
@@ -1438,23 +1322,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-WorkflowExecutionCountTypeDef = TypedDict(
-    "WorkflowExecutionCountTypeDef",
-    {
-        "count": int,
-        "truncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredWorkflowExecutionOpenCountsTypeDef = TypedDict(
     "_RequiredWorkflowExecutionOpenCountsTypeDef",
     {
         "openActivityTasks": int,
         "openDecisionTasks": int,
         "openTimers": int,
         "openChildWorkflowExecutions": int,
@@ -1638,38 +1513,14 @@
 )
 
 class PollForActivityTaskInputRequestTypeDef(
     _RequiredPollForActivityTaskInputRequestTypeDef, _OptionalPollForActivityTaskInputRequestTypeDef
 ):
     pass
 
-_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
-    "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
-    {
-        "domain": str,
-        "taskList": TaskListTypeDef,
-    },
-)
-_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
-    "_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
-    {
-        "identity": str,
-        "reverseOrder": bool,
-        "startAtPreviousStartedEvent": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
-    _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-    _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
-):
-    pass
-
 _RequiredPollForDecisionTaskInputRequestTypeDef = TypedDict(
     "_RequiredPollForDecisionTaskInputRequestTypeDef",
     {
         "domain": str,
         "taskList": TaskListTypeDef,
     },
 )
@@ -1806,24 +1657,65 @@
         "defaultTaskPriority": str,
         "defaultChildPolicy": ChildPolicyType,
         "defaultLambdaRole": str,
     },
     total=False,
 )
 
+ActivityTaskStatusTypeDef = TypedDict(
+    "ActivityTaskStatusTypeDef",
+    {
+        "cancelRequested": bool,
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
+PendingTaskCountTypeDef = TypedDict(
+    "PendingTaskCountTypeDef",
+    {
+        "count": int,
+        "truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RunTypeDef = TypedDict(
+    "RunTypeDef",
+    {
+        "runId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+WorkflowExecutionCountTypeDef = TypedDict(
+    "WorkflowExecutionCountTypeDef",
+    {
+        "count": int,
+        "truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ActivityTaskTypeDef = TypedDict(
     "ActivityTaskTypeDef",
     {
         "taskToken": str,
         "activityId": str,
         "startedEventId": int,
         "workflowExecution": WorkflowExecutionTypeDef,
         "activityType": ActivityTypeTypeDef,
         "input": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWorkflowExecutionInputRequestTypeDef = TypedDict(
     "DescribeWorkflowExecutionInputRequestTypeDef",
     {
         "domain": str,
@@ -1843,36 +1735,14 @@
     "ExternalWorkflowExecutionSignaledEventAttributesTypeDef",
     {
         "workflowExecution": WorkflowExecutionTypeDef,
         "initiatedEventId": int,
     },
 )
 
-_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    {
-        "domain": str,
-        "execution": WorkflowExecutionTypeDef,
-    },
-)
-_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
-    {
-        "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
-    _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-    _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
-):
-    pass
-
 _RequiredGetWorkflowExecutionHistoryInputRequestTypeDef = TypedDict(
     "_RequiredGetWorkflowExecutionHistoryInputRequestTypeDef",
     {
         "domain": str,
         "execution": WorkflowExecutionTypeDef,
     },
 )
@@ -2261,191 +2131,169 @@
     },
     total=False,
 )
 
 class WorkflowTypeInfoTypeDef(_RequiredWorkflowTypeInfoTypeDef, _OptionalWorkflowTypeInfoTypeDef):
     pass
 
-_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef",
+DomainDetailTypeDef = TypedDict(
+    "DomainDetailTypeDef",
     {
-        "domain": str,
+        "domainInfo": DomainInfoTypeDef,
+        "configuration": DomainConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef",
+
+DomainInfosTypeDef = TypedDict(
+    "DomainInfosTypeDef",
     {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
+        "domainInfos": List[DomainInfoTypeDef],
+        "nextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CountClosedWorkflowExecutionsInputRequestTypeDef(
-    _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef,
-    _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef,
-):
-    pass
-
-_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef",
+_RequiredExecutionTimeFilterTypeDef = TypedDict(
+    "_RequiredExecutionTimeFilterTypeDef",
     {
-        "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "oldestDate": TimestampTypeDef,
     },
 )
-_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef",
+_OptionalExecutionTimeFilterTypeDef = TypedDict(
+    "_OptionalExecutionTimeFilterTypeDef",
     {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "latestDate": TimestampTypeDef,
     },
     total=False,
 )
 
-class CountOpenWorkflowExecutionsInputRequestTypeDef(
-    _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
-    _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
+class ExecutionTimeFilterTypeDef(
+    _RequiredExecutionTimeFilterTypeDef, _OptionalExecutionTimeFilterTypeDef
 ):
     pass
 
-_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     {
         "domain": str,
+        "execution": WorkflowExecutionTypeDef,
     },
 )
-_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef",
     {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
         "reverseOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+class GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef(
+    _RequiredGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+    _OptionalGetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
 ):
     pass
 
-_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
+_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
+    "_RequiredListActivityTypesInputListActivityTypesPaginateTypeDef",
     {
         "domain": str,
+        "registrationStatus": RegistrationStatusType,
     },
 )
-_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
+_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef = TypedDict(
+    "_OptionalListActivityTypesInputListActivityTypesPaginateTypeDef",
     {
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
-        "closeTimeFilter": ExecutionTimeFilterTypeDef,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "closeStatusFilter": CloseStatusFilterTypeDef,
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
+        "name": str,
         "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListClosedWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
+class ListActivityTypesInputListActivityTypesPaginateTypeDef(
+    _RequiredListActivityTypesInputListActivityTypesPaginateTypeDef,
+    _OptionalListActivityTypesInputListActivityTypesPaginateTypeDef,
 ):
     pass
 
-_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+_RequiredListDomainsInputListDomainsPaginateTypeDef = TypedDict(
+    "_RequiredListDomainsInputListDomainsPaginateTypeDef",
     {
-        "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "registrationStatus": RegistrationStatusType,
     },
 )
-_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+_OptionalListDomainsInputListDomainsPaginateTypeDef = TypedDict(
+    "_OptionalListDomainsInputListDomainsPaginateTypeDef",
     {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
         "reverseOrder": bool,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
-    _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
-    _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+class ListDomainsInputListDomainsPaginateTypeDef(
+    _RequiredListDomainsInputListDomainsPaginateTypeDef,
+    _OptionalListDomainsInputListDomainsPaginateTypeDef,
 ):
     pass
 
-_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
+_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
+    "_RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     {
         "domain": str,
-        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "registrationStatus": RegistrationStatusType,
     },
 )
-_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
-    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
+_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = TypedDict(
+    "_OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef",
     {
-        "typeFilter": WorkflowTypeFilterTypeDef,
-        "tagFilter": TagFilterTypeDef,
-        "nextPageToken": str,
-        "maximumPageSize": int,
+        "name": str,
         "reverseOrder": bool,
-        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListOpenWorkflowExecutionsInputRequestTypeDef(
-    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
-    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
+class ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef(
+    _RequiredListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    _OptionalListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
 ):
     pass
 
-DomainDetailTypeDef = TypedDict(
-    "DomainDetailTypeDef",
+_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
+    "_RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     {
-        "domainInfo": DomainInfoTypeDef,
-        "configuration": DomainConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "domain": str,
+        "taskList": TaskListTypeDef,
     },
 )
-
-DomainInfosTypeDef = TypedDict(
-    "DomainInfosTypeDef",
+_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = TypedDict(
+    "_OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef",
     {
-        "domainInfos": List[DomainInfoTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "identity": str,
+        "reverseOrder": bool,
+        "startAtPreviousStartedEvent": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef(
+    _RequiredPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
+    _OptionalPollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
+):
+    pass
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRegisterDomainInputRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainInputRequestTypeDef",
     {
         "name": str,
@@ -2475,24 +2323,24 @@
 )
 
 ActivityTypeInfosTypeDef = TypedDict(
     "ActivityTypeInfosTypeDef",
     {
         "typeInfos": List[ActivityTypeInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActivityTypeDetailTypeDef = TypedDict(
     "ActivityTypeDetailTypeDef",
     {
         "typeInfo": ActivityTypeInfoTypeDef,
         "configuration": ActivityTypeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDecisionTypeDef = TypedDict(
     "_RequiredDecisionTypeDef",
     {
         "decisionType": DecisionTypeType,
@@ -2539,24 +2387,24 @@
     "WorkflowExecutionDetailTypeDef",
     {
         "executionInfo": WorkflowExecutionInfoTypeDef,
         "executionConfiguration": WorkflowExecutionConfigurationTypeDef,
         "openCounts": WorkflowExecutionOpenCountsTypeDef,
         "latestActivityTaskTimestamp": datetime,
         "latestExecutionContext": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkflowExecutionInfosTypeDef = TypedDict(
     "WorkflowExecutionInfosTypeDef",
     {
         "executionInfos": List[WorkflowExecutionInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHistoryEventTypeDef = TypedDict(
     "_RequiredHistoryEventTypeDef",
     {
         "eventTimestamp": datetime,
@@ -2681,27 +2529,181 @@
     pass
 
 WorkflowTypeDetailTypeDef = TypedDict(
     "WorkflowTypeDetailTypeDef",
     {
         "typeInfo": WorkflowTypeInfoTypeDef,
         "configuration": WorkflowTypeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkflowTypeInfosTypeDef = TypedDict(
     "WorkflowTypeInfosTypeDef",
     {
         "typeInfos": List[WorkflowTypeInfoTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredCountClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalCountClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+    },
+    total=False,
+)
+
+class CountClosedWorkflowExecutionsInputRequestTypeDef(
+    _RequiredCountClosedWorkflowExecutionsInputRequestTypeDef,
+    _OptionalCountClosedWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredCountOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalCountOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+    },
+    total=False,
+)
+
+class CountOpenWorkflowExecutionsInputRequestTypeDef(
+    _RequiredCountOpenWorkflowExecutionsInputRequestTypeDef,
+    _OptionalCountOpenWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef",
+    {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "reverseOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+    },
+)
+_OptionalListClosedWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListClosedWorkflowExecutionsInputRequestTypeDef",
+    {
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+        "closeTimeFilter": ExecutionTimeFilterTypeDef,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "closeStatusFilter": CloseStatusFilterTypeDef,
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+    },
+    total=False,
+)
+
+class ListClosedWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListClosedWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListClosedWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
+_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "reverseOrder": bool,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef(
+    _RequiredListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    _OptionalListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_RequiredListOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "domain": str,
+        "startTimeFilter": ExecutionTimeFilterTypeDef,
+    },
+)
+_OptionalListOpenWorkflowExecutionsInputRequestTypeDef = TypedDict(
+    "_OptionalListOpenWorkflowExecutionsInputRequestTypeDef",
+    {
+        "typeFilter": WorkflowTypeFilterTypeDef,
+        "tagFilter": TagFilterTypeDef,
+        "nextPageToken": str,
+        "maximumPageSize": int,
+        "reverseOrder": bool,
+        "executionFilter": WorkflowExecutionFilterTypeDef,
+    },
+    total=False,
+)
+
+class ListOpenWorkflowExecutionsInputRequestTypeDef(
+    _RequiredListOpenWorkflowExecutionsInputRequestTypeDef,
+    _OptionalListOpenWorkflowExecutionsInputRequestTypeDef,
+):
+    pass
+
 _RequiredRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
     "_RequiredRespondDecisionTaskCompletedInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalRespondDecisionTaskCompletedInputRequestTypeDef = TypedDict(
@@ -2725,19 +2727,19 @@
         "taskToken": str,
         "startedEventId": int,
         "workflowExecution": WorkflowExecutionTypeDef,
         "workflowType": WorkflowTypeTypeDef,
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
         "previousStartedEventId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HistoryTypeDef = TypedDict(
     "HistoryTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf.egg-info/PKG-INFO` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-swf
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SWF 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SWF 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore swf type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore swf type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-swf"></a>
 
 # types-aiobotocore-swf
 
 [![PyPI - types-aiobotocore-swf](https://img.shields.io/pypi/v/types-aiobotocore-swf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-swf)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-swf.svg?color=blue)](https://pypi.org/project/types-aiobotocore-swf)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-swf?color=blue)](https://pypistats.org/packages/types-aiobotocore-swf)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-swf)](https://pepy.tech/project/types-aiobotocore-swf)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SWF 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
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
 [types-aiobotocore-swf docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf/).
 
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
@@ -361,43 +360,42 @@
 )
 
 
 def check_value(value: ActivityTaskTimeoutTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_swf.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_swf.type_defs import (
     ActivityTaskCancelRequestedEventAttributesTypeDef,
     ActivityTaskCanceledEventAttributesTypeDef,
     ActivityTaskCompletedEventAttributesTypeDef,
     ActivityTaskFailedEventAttributesTypeDef,
     ActivityTypeTypeDef,
     TaskListTypeDef,
     ActivityTaskStartedEventAttributesTypeDef,
-    ActivityTaskStatusTypeDef,
+    ResponseMetadataTypeDef,
     ActivityTaskTimedOutEventAttributesTypeDef,
     WorkflowExecutionTypeDef,
     CancelTimerDecisionAttributesTypeDef,
     CancelTimerFailedEventAttributesTypeDef,
     CancelWorkflowExecutionDecisionAttributesTypeDef,
     CancelWorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowTypeTypeDef,
     CloseStatusFilterTypeDef,
     CompleteWorkflowExecutionDecisionAttributesTypeDef,
     CompleteWorkflowExecutionFailedEventAttributesTypeDef,
     ContinueAsNewWorkflowExecutionFailedEventAttributesTypeDef,
-    ExecutionTimeFilterTypeDef,
     TagFilterTypeDef,
     WorkflowExecutionFilterTypeDef,
     WorkflowTypeFilterTypeDef,
     DecisionTaskCompletedEventAttributesTypeDef,
     DecisionTaskStartedEventAttributesTypeDef,
     DecisionTaskTimedOutEventAttributesTypeDef,
     FailWorkflowExecutionDecisionAttributesTypeDef,
@@ -407,16 +405,17 @@
     ScheduleLambdaFunctionDecisionAttributesTypeDef,
     SignalExternalWorkflowExecutionDecisionAttributesTypeDef,
     StartTimerDecisionAttributesTypeDef,
     DeprecateDomainInputRequestTypeDef,
     DescribeDomainInputRequestTypeDef,
     DomainConfigurationTypeDef,
     DomainInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampTypeDef,
     FailWorkflowExecutionFailedEventAttributesTypeDef,
+    PaginatorConfigTypeDef,
     LambdaFunctionCompletedEventAttributesTypeDef,
     LambdaFunctionFailedEventAttributesTypeDef,
     LambdaFunctionScheduledEventAttributesTypeDef,
     LambdaFunctionStartedEventAttributesTypeDef,
     LambdaFunctionTimedOutEventAttributesTypeDef,
     MarkerRecordedEventAttributesTypeDef,
     RecordMarkerFailedEventAttributesTypeDef,
@@ -432,61 +431,56 @@
     TimerFiredEventAttributesTypeDef,
     TimerStartedEventAttributesTypeDef,
     WorkflowExecutionCanceledEventAttributesTypeDef,
     WorkflowExecutionCompletedEventAttributesTypeDef,
     WorkflowExecutionFailedEventAttributesTypeDef,
     WorkflowExecutionTerminatedEventAttributesTypeDef,
     WorkflowExecutionTimedOutEventAttributesTypeDef,
-    ListActivityTypesInputListActivityTypesPaginateTypeDef,
     ListActivityTypesInputRequestTypeDef,
-    ListDomainsInputListDomainsPaginateTypeDef,
     ListDomainsInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ResourceTagTypeDef,
-    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
     ListWorkflowTypesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    PendingTaskCountTypeDef,
     RecordActivityTaskHeartbeatInputRequestTypeDef,
     RequestCancelWorkflowExecutionInputRequestTypeDef,
     RespondActivityTaskCanceledInputRequestTypeDef,
     RespondActivityTaskCompletedInputRequestTypeDef,
     RespondActivityTaskFailedInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RunTypeDef,
     SignalWorkflowExecutionInputRequestTypeDef,
     TerminateWorkflowExecutionInputRequestTypeDef,
     UndeprecateDomainInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    WorkflowExecutionCountTypeDef,
     WorkflowExecutionOpenCountsTypeDef,
     ActivityTypeInfoTypeDef,
     DeprecateActivityTypeInputRequestTypeDef,
     DescribeActivityTypeInputRequestTypeDef,
     ScheduleActivityTaskFailedEventAttributesTypeDef,
     UndeprecateActivityTypeInputRequestTypeDef,
     ActivityTaskScheduledEventAttributesTypeDef,
     ActivityTypeConfigurationTypeDef,
     ContinueAsNewWorkflowExecutionDecisionAttributesTypeDef,
     CountPendingActivityTasksInputRequestTypeDef,
     CountPendingDecisionTasksInputRequestTypeDef,
     DecisionTaskScheduledEventAttributesTypeDef,
     PollForActivityTaskInputRequestTypeDef,
-    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     PollForDecisionTaskInputRequestTypeDef,
     RegisterActivityTypeInputRequestTypeDef,
     RegisterWorkflowTypeInputRequestTypeDef,
     ScheduleActivityTaskDecisionAttributesTypeDef,
     WorkflowExecutionConfigurationTypeDef,
     WorkflowTypeConfigurationTypeDef,
+    ActivityTaskStatusTypeDef,
+    EmptyResponseMetadataTypeDef,
+    PendingTaskCountTypeDef,
+    RunTypeDef,
+    WorkflowExecutionCountTypeDef,
     ActivityTaskTypeDef,
     DescribeWorkflowExecutionInputRequestTypeDef,
     ExternalWorkflowExecutionCancelRequestedEventAttributesTypeDef,
     ExternalWorkflowExecutionSignaledEventAttributesTypeDef,
-    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
     GetWorkflowExecutionHistoryInputRequestTypeDef,
     WorkflowExecutionCancelRequestedEventAttributesTypeDef,
     WorkflowExecutionSignaledEventAttributesTypeDef,
     ChildWorkflowExecutionCanceledEventAttributesTypeDef,
     ChildWorkflowExecutionCompletedEventAttributesTypeDef,
     ChildWorkflowExecutionFailedEventAttributesTypeDef,
     ChildWorkflowExecutionStartedEventAttributesTypeDef,
@@ -499,40 +493,46 @@
     StartChildWorkflowExecutionInitiatedEventAttributesTypeDef,
     StartWorkflowExecutionInputRequestTypeDef,
     UndeprecateWorkflowTypeInputRequestTypeDef,
     WorkflowExecutionContinuedAsNewEventAttributesTypeDef,
     WorkflowExecutionInfoTypeDef,
     WorkflowExecutionStartedEventAttributesTypeDef,
     WorkflowTypeInfoTypeDef,
-    CountClosedWorkflowExecutionsInputRequestTypeDef,
-    CountOpenWorkflowExecutionsInputRequestTypeDef,
-    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
-    ListClosedWorkflowExecutionsInputRequestTypeDef,
-    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
-    ListOpenWorkflowExecutionsInputRequestTypeDef,
     DomainDetailTypeDef,
     DomainInfosTypeDef,
+    ExecutionTimeFilterTypeDef,
+    GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef,
+    ListActivityTypesInputListActivityTypesPaginateTypeDef,
+    ListDomainsInputListDomainsPaginateTypeDef,
+    ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef,
+    PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef,
     ListTagsForResourceOutputTypeDef,
     RegisterDomainInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ActivityTypeInfosTypeDef,
     ActivityTypeDetailTypeDef,
     DecisionTypeDef,
     WorkflowExecutionDetailTypeDef,
     WorkflowExecutionInfosTypeDef,
     HistoryEventTypeDef,
     WorkflowTypeDetailTypeDef,
     WorkflowTypeInfosTypeDef,
+    CountClosedWorkflowExecutionsInputRequestTypeDef,
+    CountOpenWorkflowExecutionsInputRequestTypeDef,
+    ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef,
+    ListClosedWorkflowExecutionsInputRequestTypeDef,
+    ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef,
+    ListOpenWorkflowExecutionsInputRequestTypeDef,
     RespondDecisionTaskCompletedInputRequestTypeDef,
     DecisionTaskTypeDef,
     HistoryTypeDef,
 )
 
 
-def get_structure() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
+def get_value() -> ActivityTaskCancelRequestedEventAttributesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-swf-2.5.2/types_aiobotocore_swf.egg-info/SOURCES.txt` & `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/SOURCES.txt`

 * *Files identical despite different names*


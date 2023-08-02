# Comparing `tmp/types-aiobotocore-iotevents-2.5.2.tar.gz` & `tmp/types-aiobotocore-iotevents-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotevents-2.5.2.tar", last modified: Sat Jul  8 01:43:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotevents-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
```

## Comparing `types-aiobotocore-iotevents-2.5.2.tar` & `types-aiobotocore-iotevents-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.722303 types-aiobotocore-iotevents-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-07-08 01:43:46.722303 types-aiobotocore-iotevents-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14575 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:46.722303 types-aiobotocore-iotevents-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.722303 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20395 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20361 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37414 2023-07-08 01:32:44.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    37349 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:43.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.722303 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-07-08 01:43:46.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-08 01:43:46.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:46.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:46.000000 types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.629562 types-aiobotocore-iotevents-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-08-02 14:52:26.629562 types-aiobotocore-iotevents-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.629562 types-aiobotocore-iotevents-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.625563 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20470 2023-08-02 14:40:45.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-08-02 14:40:45.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-08-02 14:40:45.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    43431 2023-08-02 14:40:47.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43352 2023-08-02 14:40:45.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.629562 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotevents-2.5.2/LICENSE` & `types-aiobotocore-iotevents-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.2/PKG-INFO` & `types-aiobotocore-iotevents-2.5.2.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotevents
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTEvents 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTEvents 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotevents type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotevents type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotevents"></a>
 
 # types-aiobotocore-iotevents
 
 [![PyPI - types-aiobotocore-iotevents](https://img.shields.io/pypi/v/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotevents?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotevents)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotevents)](https://pepy.tech/project/types-aiobotocore-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTEvents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [types-aiobotocore-iotevents docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -289,20 +288,20 @@
 )
 
 
 def check_value(value: AlarmModelVersionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotevents.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotevents.type_defs import (
     AcknowledgeFlowTypeDef,
     ClearTimerActionTypeDef,
     ResetTimerActionTypeDef,
     SetTimerActionTypeDef,
@@ -312,60 +311,62 @@
     AlarmModelVersionSummaryTypeDef,
     SimpleRuleTypeDef,
     AnalysisResultLocationTypeDef,
     AssetPropertyTimestampTypeDef,
     AssetPropertyVariantTypeDef,
     AttributeTypeDef,
     TagTypeDef,
-    CreateAlarmModelResponseTypeDef,
+    ResponseMetadataTypeDef,
     DetectorModelConfigurationTypeDef,
     InputConfigurationTypeDef,
     DeleteAlarmModelRequestRequestTypeDef,
     DeleteDetectorModelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DescribeAlarmModelRequestRequestTypeDef,
     DescribeDetectorModelAnalysisRequestRequestTypeDef,
-    DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelRequestRequestTypeDef,
     DescribeInputRequestRequestTypeDef,
     DetectorDebugOptionTypeDef,
     DetectorModelSummaryTypeDef,
     DetectorModelVersionSummaryTypeDef,
     PayloadTypeDef,
     EmailContentTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsRequestRequestTypeDef,
     IotEventsInputIdentifierTypeDef,
     InputSummaryTypeDef,
     IotSiteWiseAssetModelPropertyIdentifierTypeDef,
     ListAlarmModelVersionsRequestRequestTypeDef,
     ListAlarmModelsRequestRequestTypeDef,
     ListDetectorModelVersionsRequestRequestTypeDef,
     ListDetectorModelsRequestRequestTypeDef,
     RoutedResourceTypeDef,
     ListInputsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     SSOIdentityTypeDef,
-    ResponseMetadataTypeDef,
-    StartDetectorModelAnalysisResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAlarmModelResponseTypeDef,
     AlarmCapabilitiesTypeDef,
-    ListAlarmModelsResponseTypeDef,
-    ListAlarmModelVersionsResponseTypeDef,
     AlarmRuleTypeDef,
     AnalysisResultTypeDef,
     AssetPropertyValueTypeDef,
+    InputDefinitionOutputTypeDef,
     InputDefinitionTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateAlarmModelResponseTypeDef,
+    DescribeDetectorModelAnalysisResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAlarmModelVersionsResponseTypeDef,
+    ListAlarmModelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDetectorModelAnalysisResponseTypeDef,
+    UpdateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     UpdateInputResponseTypeDef,
+    LoggingOptionsOutputTypeDef,
     LoggingOptionsTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
     DynamoDBActionTypeDef,
     DynamoDBv2ActionTypeDef,
     FirehoseActionTypeDef,
     IotEventsActionTypeDef,
@@ -375,50 +376,68 @@
     SqsActionTypeDef,
     ListInputsResponseTypeDef,
     IotSiteWiseInputIdentifierTypeDef,
     ListInputRoutingsResponseTypeDef,
     RecipientDetailTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
     IotSiteWiseActionTypeDef,
-    CreateInputRequestRequestTypeDef,
     InputTypeDef,
+    CreateInputRequestRequestTypeDef,
+    InputDefinitionUnionTypeDef,
     UpdateInputRequestRequestTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
+    LoggingOptionsUnionTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     NotificationTargetActionsTypeDef,
     InputIdentifierTypeDef,
+    EmailRecipientsOutputTypeDef,
     EmailRecipientsTypeDef,
+    SMSConfigurationOutputTypeDef,
     SMSConfigurationTypeDef,
     ActionTypeDef,
     AlarmActionTypeDef,
     DescribeInputResponseTypeDef,
     ListInputRoutingsRequestRequestTypeDef,
+    EmailConfigurationOutputTypeDef,
     EmailConfigurationTypeDef,
+    EventOutputTypeDef,
     EventTypeDef,
+    TransitionEventOutputTypeDef,
     TransitionEventTypeDef,
+    AlarmEventActionsOutputTypeDef,
     AlarmEventActionsTypeDef,
+    NotificationActionOutputTypeDef,
     NotificationActionTypeDef,
+    OnEnterLifecycleOutputTypeDef,
+    OnExitLifecycleOutputTypeDef,
     OnEnterLifecycleTypeDef,
     OnExitLifecycleTypeDef,
+    OnInputLifecycleOutputTypeDef,
     OnInputLifecycleTypeDef,
+    AlarmEventActionsUnionTypeDef,
+    AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
+    StateOutputTypeDef,
     StateTypeDef,
-    CreateAlarmModelRequestRequestTypeDef,
     DescribeAlarmModelResponseTypeDef,
+    AlarmNotificationUnionTypeDef,
+    CreateAlarmModelRequestRequestTypeDef,
     UpdateAlarmModelRequestRequestTypeDef,
+    DetectorModelDefinitionOutputTypeDef,
     DetectorModelDefinitionTypeDef,
-    CreateDetectorModelRequestRequestTypeDef,
     DetectorModelTypeDef,
+    CreateDetectorModelRequestRequestTypeDef,
+    DetectorModelDefinitionUnionTypeDef,
     StartDetectorModelAnalysisRequestRequestTypeDef,
     UpdateDetectorModelRequestRequestTypeDef,
     DescribeDetectorModelResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeFlowTypeDef:
+def get_value() -> AcknowledgeFlowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotevents-2.5.2/README.md` & `types-aiobotocore-iotevents-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iotevents"></a>
 
 # types-aiobotocore-iotevents
 
 [![PyPI - types-aiobotocore-iotevents](https://img.shields.io/pypi/v/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotevents?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotevents)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotevents)](https://pepy.tech/project/types-aiobotocore-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTEvents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [types-aiobotocore-iotevents docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,15 +40,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -256,20 +256,20 @@
 )
 
 
 def check_value(value: AlarmModelVersionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotevents.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotevents.type_defs import (
     AcknowledgeFlowTypeDef,
     ClearTimerActionTypeDef,
     ResetTimerActionTypeDef,
     SetTimerActionTypeDef,
@@ -279,60 +279,62 @@
     AlarmModelVersionSummaryTypeDef,
     SimpleRuleTypeDef,
     AnalysisResultLocationTypeDef,
     AssetPropertyTimestampTypeDef,
     AssetPropertyVariantTypeDef,
     AttributeTypeDef,
     TagTypeDef,
-    CreateAlarmModelResponseTypeDef,
+    ResponseMetadataTypeDef,
     DetectorModelConfigurationTypeDef,
     InputConfigurationTypeDef,
     DeleteAlarmModelRequestRequestTypeDef,
     DeleteDetectorModelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DescribeAlarmModelRequestRequestTypeDef,
     DescribeDetectorModelAnalysisRequestRequestTypeDef,
-    DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelRequestRequestTypeDef,
     DescribeInputRequestRequestTypeDef,
     DetectorDebugOptionTypeDef,
     DetectorModelSummaryTypeDef,
     DetectorModelVersionSummaryTypeDef,
     PayloadTypeDef,
     EmailContentTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsRequestRequestTypeDef,
     IotEventsInputIdentifierTypeDef,
     InputSummaryTypeDef,
     IotSiteWiseAssetModelPropertyIdentifierTypeDef,
     ListAlarmModelVersionsRequestRequestTypeDef,
     ListAlarmModelsRequestRequestTypeDef,
     ListDetectorModelVersionsRequestRequestTypeDef,
     ListDetectorModelsRequestRequestTypeDef,
     RoutedResourceTypeDef,
     ListInputsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     SSOIdentityTypeDef,
-    ResponseMetadataTypeDef,
-    StartDetectorModelAnalysisResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAlarmModelResponseTypeDef,
     AlarmCapabilitiesTypeDef,
-    ListAlarmModelsResponseTypeDef,
-    ListAlarmModelVersionsResponseTypeDef,
     AlarmRuleTypeDef,
     AnalysisResultTypeDef,
     AssetPropertyValueTypeDef,
+    InputDefinitionOutputTypeDef,
     InputDefinitionTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateAlarmModelResponseTypeDef,
+    DescribeDetectorModelAnalysisResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAlarmModelVersionsResponseTypeDef,
+    ListAlarmModelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDetectorModelAnalysisResponseTypeDef,
+    UpdateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     UpdateInputResponseTypeDef,
+    LoggingOptionsOutputTypeDef,
     LoggingOptionsTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
     DynamoDBActionTypeDef,
     DynamoDBv2ActionTypeDef,
     FirehoseActionTypeDef,
     IotEventsActionTypeDef,
@@ -342,50 +344,68 @@
     SqsActionTypeDef,
     ListInputsResponseTypeDef,
     IotSiteWiseInputIdentifierTypeDef,
     ListInputRoutingsResponseTypeDef,
     RecipientDetailTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
     IotSiteWiseActionTypeDef,
-    CreateInputRequestRequestTypeDef,
     InputTypeDef,
+    CreateInputRequestRequestTypeDef,
+    InputDefinitionUnionTypeDef,
     UpdateInputRequestRequestTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
+    LoggingOptionsUnionTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     NotificationTargetActionsTypeDef,
     InputIdentifierTypeDef,
+    EmailRecipientsOutputTypeDef,
     EmailRecipientsTypeDef,
+    SMSConfigurationOutputTypeDef,
     SMSConfigurationTypeDef,
     ActionTypeDef,
     AlarmActionTypeDef,
     DescribeInputResponseTypeDef,
     ListInputRoutingsRequestRequestTypeDef,
+    EmailConfigurationOutputTypeDef,
     EmailConfigurationTypeDef,
+    EventOutputTypeDef,
     EventTypeDef,
+    TransitionEventOutputTypeDef,
     TransitionEventTypeDef,
+    AlarmEventActionsOutputTypeDef,
     AlarmEventActionsTypeDef,
+    NotificationActionOutputTypeDef,
     NotificationActionTypeDef,
+    OnEnterLifecycleOutputTypeDef,
+    OnExitLifecycleOutputTypeDef,
     OnEnterLifecycleTypeDef,
     OnExitLifecycleTypeDef,
+    OnInputLifecycleOutputTypeDef,
     OnInputLifecycleTypeDef,
+    AlarmEventActionsUnionTypeDef,
+    AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
+    StateOutputTypeDef,
     StateTypeDef,
-    CreateAlarmModelRequestRequestTypeDef,
     DescribeAlarmModelResponseTypeDef,
+    AlarmNotificationUnionTypeDef,
+    CreateAlarmModelRequestRequestTypeDef,
     UpdateAlarmModelRequestRequestTypeDef,
+    DetectorModelDefinitionOutputTypeDef,
     DetectorModelDefinitionTypeDef,
-    CreateDetectorModelRequestRequestTypeDef,
     DetectorModelTypeDef,
+    CreateDetectorModelRequestRequestTypeDef,
+    DetectorModelDefinitionUnionTypeDef,
     StartDetectorModelAnalysisRequestRequestTypeDef,
     UpdateDetectorModelRequestRequestTypeDef,
     DescribeDetectorModelResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeFlowTypeDef:
+def get_value() -> AcknowledgeFlowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotevents-2.5.2/setup.py` & `types-aiobotocore-iotevents-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotevents",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iotevents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTEvents 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore iotevents type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore iotevents type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotevents": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/"
```

### Comparing `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/__main__.py` & `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTEvents 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IoTEvents 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents\nOther"
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

### Comparing `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/client.py` & `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,69 +18,66 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import EvaluationMethodType
 from .type_defs import (
     AlarmCapabilitiesTypeDef,
-    AlarmEventActionsTypeDef,
-    AlarmNotificationTypeDef,
+    AlarmEventActionsUnionTypeDef,
+    AlarmNotificationUnionTypeDef,
     AlarmRuleTypeDef,
     CreateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     DescribeAlarmModelResponseTypeDef,
     DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelResponseTypeDef,
     DescribeInputResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    DetectorModelDefinitionTypeDef,
+    DetectorModelDefinitionUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
-    InputDefinitionTypeDef,
+    InputDefinitionUnionTypeDef,
     InputIdentifierTypeDef,
     ListAlarmModelsResponseTypeDef,
     ListAlarmModelVersionsResponseTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
     ListInputRoutingsResponseTypeDef,
     ListInputsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    LoggingOptionsTypeDef,
+    LoggingOptionsUnionTypeDef,
     StartDetectorModelAnalysisResponseTypeDef,
     TagTypeDef,
     UpdateAlarmModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     UpdateInputResponseTypeDef,
 )
 
 __all__ = ("IoTEventsClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
-
 class IoTEventsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/)
     """
 
     meta: ClientMeta
@@ -89,342 +86,311 @@
     def exceptions(self) -> Exceptions:
         """
         IoTEventsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#close)
         """
-
     async def create_alarm_model(
         self,
         *,
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         key: str = ...,
         severity: int = ...,
-        alarmNotification: AlarmNotificationTypeDef = ...,
-        alarmEventActions: AlarmEventActionsTypeDef = ...,
+        alarmNotification: AlarmNotificationUnionTypeDef = ...,
+        alarmEventActions: AlarmEventActionsUnionTypeDef = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> CreateAlarmModelResponseTypeDef:
         """
         Creates an alarm model to monitor an AWS IoT Events input attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_alarm_model)
         """
-
     async def create_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: DetectorModelDefinitionTypeDef,
+        detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         key: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> CreateDetectorModelResponseTypeDef:
         """
         Creates a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_detector_model)
         """
-
     async def create_input(
         self,
         *,
         inputName: str,
-        inputDefinition: InputDefinitionTypeDef,
+        inputDefinition: InputDefinitionUnionTypeDef,
         inputDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateInputResponseTypeDef:
         """
         Creates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_input)
         """
-
     async def delete_alarm_model(self, *, alarmModelName: str) -> Dict[str, Any]:
         """
         Deletes an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.delete_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#delete_alarm_model)
         """
-
     async def delete_detector_model(self, *, detectorModelName: str) -> Dict[str, Any]:
         """
         Deletes a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.delete_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#delete_detector_model)
         """
-
     async def delete_input(self, *, inputName: str) -> Dict[str, Any]:
         """
         Deletes an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.delete_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#delete_input)
         """
-
     async def describe_alarm_model(
         self, *, alarmModelName: str, alarmModelVersion: str = ...
     ) -> DescribeAlarmModelResponseTypeDef:
         """
         Retrieves information about an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.describe_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#describe_alarm_model)
         """
-
     async def describe_detector_model(
         self, *, detectorModelName: str, detectorModelVersion: str = ...
     ) -> DescribeDetectorModelResponseTypeDef:
         """
         Describes a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.describe_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#describe_detector_model)
         """
-
     async def describe_detector_model_analysis(
         self, *, analysisId: str
     ) -> DescribeDetectorModelAnalysisResponseTypeDef:
         """
         Retrieves runtime information about a detector model analysis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.describe_detector_model_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#describe_detector_model_analysis)
         """
-
     async def describe_input(self, *, inputName: str) -> DescribeInputResponseTypeDef:
         """
         Describes an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.describe_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#describe_input)
         """
-
     async def describe_logging_options(self) -> DescribeLoggingOptionsResponseTypeDef:
         """
         Retrieves the current settings of the AWS IoT Events logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.describe_logging_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#describe_logging_options)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#generate_presigned_url)
         """
-
     async def get_detector_model_analysis_results(
         self, *, analysisId: str, nextToken: str = ..., maxResults: int = ...
     ) -> GetDetectorModelAnalysisResultsResponseTypeDef:
         """
         Retrieves one or more analysis results of the detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.get_detector_model_analysis_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#get_detector_model_analysis_results)
         """
-
     async def list_alarm_model_versions(
         self, *, alarmModelName: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListAlarmModelVersionsResponseTypeDef:
         """
         Lists all the versions of an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_alarm_model_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_alarm_model_versions)
         """
-
     async def list_alarm_models(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListAlarmModelsResponseTypeDef:
         """
         Lists the alarm models that you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_alarm_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_alarm_models)
         """
-
     async def list_detector_model_versions(
         self, *, detectorModelName: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListDetectorModelVersionsResponseTypeDef:
         """
         Lists all the versions of a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_detector_model_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_detector_model_versions)
         """
-
     async def list_detector_models(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListDetectorModelsResponseTypeDef:
         """
         Lists the detector models you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_detector_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_detector_models)
         """
-
     async def list_input_routings(
         self,
         *,
         inputIdentifier: InputIdentifierTypeDef,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListInputRoutingsResponseTypeDef:
         """
         Lists one or more input routings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_input_routings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_input_routings)
         """
-
     async def list_inputs(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListInputsResponseTypeDef:
         """
         Lists the inputs you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_inputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_inputs)
         """
-
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags (metadata) you have assigned to the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_tags_for_resource)
         """
-
     async def put_logging_options(
-        self, *, loggingOptions: LoggingOptionsTypeDef
+        self, *, loggingOptions: LoggingOptionsUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets or updates the AWS IoT Events logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.put_logging_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#put_logging_options)
         """
-
     async def start_detector_model_analysis(
-        self, *, detectorModelDefinition: DetectorModelDefinitionTypeDef
+        self, *, detectorModelDefinition: DetectorModelDefinitionUnionTypeDef
     ) -> StartDetectorModelAnalysisResponseTypeDef:
         """
         Performs an analysis of your detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.start_detector_model_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#start_detector_model_analysis)
         """
-
     async def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds to or modifies the tags of the given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#tag_resource)
         """
-
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the given tags (metadata) from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#untag_resource)
         """
-
     async def update_alarm_model(
         self,
         *,
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         severity: int = ...,
-        alarmNotification: AlarmNotificationTypeDef = ...,
-        alarmEventActions: AlarmEventActionsTypeDef = ...,
+        alarmNotification: AlarmNotificationUnionTypeDef = ...,
+        alarmEventActions: AlarmEventActionsUnionTypeDef = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> UpdateAlarmModelResponseTypeDef:
         """
         Updates an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_alarm_model)
         """
-
     async def update_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: DetectorModelDefinitionTypeDef,
+        detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> UpdateDetectorModelResponseTypeDef:
         """
         Updates a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_detector_model)
         """
-
     async def update_input(
         self,
         *,
         inputName: str,
-        inputDefinition: InputDefinitionTypeDef,
+        inputDefinition: InputDefinitionUnionTypeDef,
         inputDescription: str = ...
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_input)
         """
-
     async def __aenter__(self) -> "IoTEventsClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/)
         """
```

### Comparing `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/client.pyi` & `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,66 +18,69 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import EvaluationMethodType
 from .type_defs import (
     AlarmCapabilitiesTypeDef,
-    AlarmEventActionsTypeDef,
-    AlarmNotificationTypeDef,
+    AlarmEventActionsUnionTypeDef,
+    AlarmNotificationUnionTypeDef,
     AlarmRuleTypeDef,
     CreateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     DescribeAlarmModelResponseTypeDef,
     DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelResponseTypeDef,
     DescribeInputResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    DetectorModelDefinitionTypeDef,
+    DetectorModelDefinitionUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
-    InputDefinitionTypeDef,
+    InputDefinitionUnionTypeDef,
     InputIdentifierTypeDef,
     ListAlarmModelsResponseTypeDef,
     ListAlarmModelVersionsResponseTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
     ListInputRoutingsResponseTypeDef,
     ListInputsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    LoggingOptionsTypeDef,
+    LoggingOptionsUnionTypeDef,
     StartDetectorModelAnalysisResponseTypeDef,
     TagTypeDef,
     UpdateAlarmModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     UpdateInputResponseTypeDef,
 )
 
 __all__ = ("IoTEventsClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
+
 class IoTEventsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/)
     """
 
     meta: ClientMeta
@@ -86,311 +89,342 @@
     def exceptions(self) -> Exceptions:
         """
         IoTEventsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#close)
         """
+
     async def create_alarm_model(
         self,
         *,
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         key: str = ...,
         severity: int = ...,
-        alarmNotification: AlarmNotificationTypeDef = ...,
-        alarmEventActions: AlarmEventActionsTypeDef = ...,
+        alarmNotification: AlarmNotificationUnionTypeDef = ...,
+        alarmEventActions: AlarmEventActionsUnionTypeDef = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> CreateAlarmModelResponseTypeDef:
         """
         Creates an alarm model to monitor an AWS IoT Events input attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_alarm_model)
         """
+
     async def create_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: DetectorModelDefinitionTypeDef,
+        detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         key: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> CreateDetectorModelResponseTypeDef:
         """
         Creates a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_detector_model)
         """
+
     async def create_input(
         self,
         *,
         inputName: str,
-        inputDefinition: InputDefinitionTypeDef,
+        inputDefinition: InputDefinitionUnionTypeDef,
         inputDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateInputResponseTypeDef:
         """
         Creates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_input)
         """
+
     async def delete_alarm_model(self, *, alarmModelName: str) -> Dict[str, Any]:
         """
         Deletes an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.delete_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#delete_alarm_model)
         """
+
     async def delete_detector_model(self, *, detectorModelName: str) -> Dict[str, Any]:
         """
         Deletes a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.delete_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#delete_detector_model)
         """
+
     async def delete_input(self, *, inputName: str) -> Dict[str, Any]:
         """
         Deletes an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.delete_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#delete_input)
         """
+
     async def describe_alarm_model(
         self, *, alarmModelName: str, alarmModelVersion: str = ...
     ) -> DescribeAlarmModelResponseTypeDef:
         """
         Retrieves information about an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.describe_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#describe_alarm_model)
         """
+
     async def describe_detector_model(
         self, *, detectorModelName: str, detectorModelVersion: str = ...
     ) -> DescribeDetectorModelResponseTypeDef:
         """
         Describes a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.describe_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#describe_detector_model)
         """
+
     async def describe_detector_model_analysis(
         self, *, analysisId: str
     ) -> DescribeDetectorModelAnalysisResponseTypeDef:
         """
         Retrieves runtime information about a detector model analysis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.describe_detector_model_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#describe_detector_model_analysis)
         """
+
     async def describe_input(self, *, inputName: str) -> DescribeInputResponseTypeDef:
         """
         Describes an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.describe_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#describe_input)
         """
+
     async def describe_logging_options(self) -> DescribeLoggingOptionsResponseTypeDef:
         """
         Retrieves the current settings of the AWS IoT Events logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.describe_logging_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#describe_logging_options)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#generate_presigned_url)
         """
+
     async def get_detector_model_analysis_results(
         self, *, analysisId: str, nextToken: str = ..., maxResults: int = ...
     ) -> GetDetectorModelAnalysisResultsResponseTypeDef:
         """
         Retrieves one or more analysis results of the detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.get_detector_model_analysis_results)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#get_detector_model_analysis_results)
         """
+
     async def list_alarm_model_versions(
         self, *, alarmModelName: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListAlarmModelVersionsResponseTypeDef:
         """
         Lists all the versions of an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_alarm_model_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_alarm_model_versions)
         """
+
     async def list_alarm_models(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListAlarmModelsResponseTypeDef:
         """
         Lists the alarm models that you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_alarm_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_alarm_models)
         """
+
     async def list_detector_model_versions(
         self, *, detectorModelName: str, nextToken: str = ..., maxResults: int = ...
     ) -> ListDetectorModelVersionsResponseTypeDef:
         """
         Lists all the versions of a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_detector_model_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_detector_model_versions)
         """
+
     async def list_detector_models(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListDetectorModelsResponseTypeDef:
         """
         Lists the detector models you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_detector_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_detector_models)
         """
+
     async def list_input_routings(
         self,
         *,
         inputIdentifier: InputIdentifierTypeDef,
         maxResults: int = ...,
         nextToken: str = ...
     ) -> ListInputRoutingsResponseTypeDef:
         """
         Lists one or more input routings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_input_routings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_input_routings)
         """
+
     async def list_inputs(
         self, *, nextToken: str = ..., maxResults: int = ...
     ) -> ListInputsResponseTypeDef:
         """
         Lists the inputs you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_inputs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_inputs)
         """
+
     async def list_tags_for_resource(
         self, *, resourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags (metadata) you have assigned to the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_tags_for_resource)
         """
+
     async def put_logging_options(
-        self, *, loggingOptions: LoggingOptionsTypeDef
+        self, *, loggingOptions: LoggingOptionsUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets or updates the AWS IoT Events logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.put_logging_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#put_logging_options)
         """
+
     async def start_detector_model_analysis(
-        self, *, detectorModelDefinition: DetectorModelDefinitionTypeDef
+        self, *, detectorModelDefinition: DetectorModelDefinitionUnionTypeDef
     ) -> StartDetectorModelAnalysisResponseTypeDef:
         """
         Performs an analysis of your detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.start_detector_model_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#start_detector_model_analysis)
         """
+
     async def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds to or modifies the tags of the given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#tag_resource)
         """
+
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the given tags (metadata) from the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#untag_resource)
         """
+
     async def update_alarm_model(
         self,
         *,
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         severity: int = ...,
-        alarmNotification: AlarmNotificationTypeDef = ...,
-        alarmEventActions: AlarmEventActionsTypeDef = ...,
+        alarmNotification: AlarmNotificationUnionTypeDef = ...,
+        alarmEventActions: AlarmEventActionsUnionTypeDef = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> UpdateAlarmModelResponseTypeDef:
         """
         Updates an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_alarm_model)
         """
+
     async def update_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: DetectorModelDefinitionTypeDef,
+        detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> UpdateDetectorModelResponseTypeDef:
         """
         Updates a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_detector_model)
         """
+
     async def update_input(
         self,
         *,
         inputName: str,
-        inputDefinition: InputDefinitionTypeDef,
+        inputDefinition: InputDefinitionUnionTypeDef,
         inputDescription: str = ...
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_input)
         """
+
     async def __aenter__(self) -> "IoTEventsClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/)
         """
```

### Comparing `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/literals.py` & `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/literals.pyi` & `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/type_defs.py` & `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iotevents.type_defs import AcknowledgeFlowTypeDef
 
-    data: AcknowledgeFlowTypeDef = {...}
+    data: AcknowledgeFlowTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AlarmModelVersionStatusType,
     AnalysisResultLevelType,
     AnalysisStatusType,
     ComparisonOperatorType,
     DetectorModelVersionStatusType,
@@ -44,60 +44,62 @@
     "AlarmModelVersionSummaryTypeDef",
     "SimpleRuleTypeDef",
     "AnalysisResultLocationTypeDef",
     "AssetPropertyTimestampTypeDef",
     "AssetPropertyVariantTypeDef",
     "AttributeTypeDef",
     "TagTypeDef",
-    "CreateAlarmModelResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DetectorModelConfigurationTypeDef",
     "InputConfigurationTypeDef",
     "DeleteAlarmModelRequestRequestTypeDef",
     "DeleteDetectorModelRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DescribeAlarmModelRequestRequestTypeDef",
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
-    "DescribeDetectorModelAnalysisResponseTypeDef",
     "DescribeDetectorModelRequestRequestTypeDef",
     "DescribeInputRequestRequestTypeDef",
     "DetectorDebugOptionTypeDef",
     "DetectorModelSummaryTypeDef",
     "DetectorModelVersionSummaryTypeDef",
     "PayloadTypeDef",
     "EmailContentTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetDetectorModelAnalysisResultsRequestRequestTypeDef",
     "IotEventsInputIdentifierTypeDef",
     "InputSummaryTypeDef",
     "IotSiteWiseAssetModelPropertyIdentifierTypeDef",
     "ListAlarmModelVersionsRequestRequestTypeDef",
     "ListAlarmModelsRequestRequestTypeDef",
     "ListDetectorModelVersionsRequestRequestTypeDef",
     "ListDetectorModelsRequestRequestTypeDef",
     "RoutedResourceTypeDef",
     "ListInputsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "SSOIdentityTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartDetectorModelAnalysisResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAlarmModelResponseTypeDef",
     "AlarmCapabilitiesTypeDef",
-    "ListAlarmModelsResponseTypeDef",
-    "ListAlarmModelVersionsResponseTypeDef",
     "AlarmRuleTypeDef",
     "AnalysisResultTypeDef",
     "AssetPropertyValueTypeDef",
+    "InputDefinitionOutputTypeDef",
     "InputDefinitionTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateAlarmModelResponseTypeDef",
+    "DescribeDetectorModelAnalysisResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListAlarmModelVersionsResponseTypeDef",
+    "ListAlarmModelsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartDetectorModelAnalysisResponseTypeDef",
+    "UpdateAlarmModelResponseTypeDef",
     "CreateDetectorModelResponseTypeDef",
     "UpdateDetectorModelResponseTypeDef",
     "CreateInputResponseTypeDef",
     "UpdateInputResponseTypeDef",
+    "LoggingOptionsOutputTypeDef",
     "LoggingOptionsTypeDef",
     "ListDetectorModelsResponseTypeDef",
     "ListDetectorModelVersionsResponseTypeDef",
     "DynamoDBActionTypeDef",
     "DynamoDBv2ActionTypeDef",
     "FirehoseActionTypeDef",
     "IotEventsActionTypeDef",
@@ -107,43 +109,61 @@
     "SqsActionTypeDef",
     "ListInputsResponseTypeDef",
     "IotSiteWiseInputIdentifierTypeDef",
     "ListInputRoutingsResponseTypeDef",
     "RecipientDetailTypeDef",
     "GetDetectorModelAnalysisResultsResponseTypeDef",
     "IotSiteWiseActionTypeDef",
-    "CreateInputRequestRequestTypeDef",
     "InputTypeDef",
+    "CreateInputRequestRequestTypeDef",
+    "InputDefinitionUnionTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
+    "LoggingOptionsUnionTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "NotificationTargetActionsTypeDef",
     "InputIdentifierTypeDef",
+    "EmailRecipientsOutputTypeDef",
     "EmailRecipientsTypeDef",
+    "SMSConfigurationOutputTypeDef",
     "SMSConfigurationTypeDef",
     "ActionTypeDef",
     "AlarmActionTypeDef",
     "DescribeInputResponseTypeDef",
     "ListInputRoutingsRequestRequestTypeDef",
+    "EmailConfigurationOutputTypeDef",
     "EmailConfigurationTypeDef",
+    "EventOutputTypeDef",
     "EventTypeDef",
+    "TransitionEventOutputTypeDef",
     "TransitionEventTypeDef",
+    "AlarmEventActionsOutputTypeDef",
     "AlarmEventActionsTypeDef",
+    "NotificationActionOutputTypeDef",
     "NotificationActionTypeDef",
+    "OnEnterLifecycleOutputTypeDef",
+    "OnExitLifecycleOutputTypeDef",
     "OnEnterLifecycleTypeDef",
     "OnExitLifecycleTypeDef",
+    "OnInputLifecycleOutputTypeDef",
     "OnInputLifecycleTypeDef",
+    "AlarmEventActionsUnionTypeDef",
+    "AlarmNotificationOutputTypeDef",
     "AlarmNotificationTypeDef",
+    "StateOutputTypeDef",
     "StateTypeDef",
-    "CreateAlarmModelRequestRequestTypeDef",
     "DescribeAlarmModelResponseTypeDef",
+    "AlarmNotificationUnionTypeDef",
+    "CreateAlarmModelRequestRequestTypeDef",
     "UpdateAlarmModelRequestRequestTypeDef",
+    "DetectorModelDefinitionOutputTypeDef",
     "DetectorModelDefinitionTypeDef",
-    "CreateDetectorModelRequestRequestTypeDef",
     "DetectorModelTypeDef",
+    "CreateDetectorModelRequestRequestTypeDef",
+    "DetectorModelDefinitionUnionTypeDef",
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     "UpdateDetectorModelRequestRequestTypeDef",
     "DescribeDetectorModelResponseTypeDef",
 )
 
 AcknowledgeFlowTypeDef = TypedDict(
     "AcknowledgeFlowTypeDef",
@@ -286,23 +306,22 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-CreateAlarmModelResponseTypeDef = TypedDict(
-    "CreateAlarmModelResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DetectorModelConfigurationTypeDef = TypedDict(
     "DetectorModelConfigurationTypeDef",
     {
         "detectorModelName": str,
@@ -390,22 +409,14 @@
 DescribeDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 
-DescribeDetectorModelAnalysisResponseTypeDef = TypedDict(
-    "DescribeDetectorModelAnalysisResponseTypeDef",
-    {
-        "status": AnalysisStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeDetectorModelRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDetectorModelRequestRequestTypeDef",
     {
         "detectorModelName": str,
     },
 )
 _OptionalDescribeDetectorModelRequestRequestTypeDef = TypedDict(
@@ -490,21 +501,14 @@
     {
         "subject": str,
         "additionalMessage": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 _OptionalGetDetectorModelAnalysisResultsRequestRequestTypeDef = TypedDict(
@@ -656,80 +660,31 @@
 )
 
 
 class SSOIdentityTypeDef(_RequiredSSOIdentityTypeDef, _OptionalSSOIdentityTypeDef):
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
-StartDetectorModelAnalysisResponseTypeDef = TypedDict(
-    "StartDetectorModelAnalysisResponseTypeDef",
-    {
-        "analysisId": str,
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
 
-UpdateAlarmModelResponseTypeDef = TypedDict(
-    "UpdateAlarmModelResponseTypeDef",
-    {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AlarmCapabilitiesTypeDef = TypedDict(
     "AlarmCapabilitiesTypeDef",
     {
         "initializationConfiguration": InitializationConfigurationTypeDef,
         "acknowledgeFlow": AcknowledgeFlowTypeDef,
     },
     total=False,
 )
 
-ListAlarmModelsResponseTypeDef = TypedDict(
-    "ListAlarmModelsResponseTypeDef",
-    {
-        "alarmModelSummaries": List[AlarmModelSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAlarmModelVersionsResponseTypeDef = TypedDict(
-    "ListAlarmModelVersionsResponseTypeDef",
-    {
-        "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AlarmRuleTypeDef = TypedDict(
     "AlarmRuleTypeDef",
     {
         "simpleRule": SimpleRuleTypeDef,
     },
     total=False,
 )
@@ -751,105 +706,200 @@
         "value": AssetPropertyVariantTypeDef,
         "timestamp": AssetPropertyTimestampTypeDef,
         "quality": str,
     },
     total=False,
 )
 
+InputDefinitionOutputTypeDef = TypedDict(
+    "InputDefinitionOutputTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+    },
+)
+
 InputDefinitionTypeDef = TypedDict(
     "InputDefinitionTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateAlarmModelResponseTypeDef = TypedDict(
+    "CreateAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDetectorModelAnalysisResponseTypeDef = TypedDict(
+    "DescribeDetectorModelAnalysisResponseTypeDef",
+    {
+        "status": AnalysisStatusType,
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
+ListAlarmModelVersionsResponseTypeDef = TypedDict(
+    "ListAlarmModelVersionsResponseTypeDef",
+    {
+        "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAlarmModelsResponseTypeDef = TypedDict(
+    "ListAlarmModelsResponseTypeDef",
+    {
+        "alarmModelSummaries": List[AlarmModelSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+StartDetectorModelAnalysisResponseTypeDef = TypedDict(
+    "StartDetectorModelAnalysisResponseTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
+        "analysisId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAlarmModelResponseTypeDef = TypedDict(
+    "UpdateAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDetectorModelResponseTypeDef = TypedDict(
     "CreateDetectorModelResponseTypeDef",
     {
         "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDetectorModelResponseTypeDef = TypedDict(
     "UpdateDetectorModelResponseTypeDef",
     {
         "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInputResponseTypeDef = TypedDict(
     "CreateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredLoggingOptionsOutputTypeDef = TypedDict(
+    "_RequiredLoggingOptionsOutputTypeDef",
+    {
+        "roleArn": str,
+        "level": LoggingLevelType,
+        "enabled": bool,
+    },
+)
+_OptionalLoggingOptionsOutputTypeDef = TypedDict(
+    "_OptionalLoggingOptionsOutputTypeDef",
+    {
+        "detectorDebugOptions": List[DetectorDebugOptionTypeDef],
+    },
+    total=False,
+)
+
+
+class LoggingOptionsOutputTypeDef(
+    _RequiredLoggingOptionsOutputTypeDef, _OptionalLoggingOptionsOutputTypeDef
+):
+    pass
+
+
 _RequiredLoggingOptionsTypeDef = TypedDict(
     "_RequiredLoggingOptionsTypeDef",
     {
         "roleArn": str,
         "level": LoggingLevelType,
         "enabled": bool,
     },
 )
 _OptionalLoggingOptionsTypeDef = TypedDict(
     "_OptionalLoggingOptionsTypeDef",
     {
-        "detectorDebugOptions": List[DetectorDebugOptionTypeDef],
+        "detectorDebugOptions": Sequence[DetectorDebugOptionTypeDef],
     },
     total=False,
 )
 
 
 class LoggingOptionsTypeDef(_RequiredLoggingOptionsTypeDef, _OptionalLoggingOptionsTypeDef):
     pass
 
 
 ListDetectorModelsResponseTypeDef = TypedDict(
     "ListDetectorModelsResponseTypeDef",
     {
         "detectorModelSummaries": List[DetectorModelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDetectorModelVersionsResponseTypeDef = TypedDict(
     "ListDetectorModelVersionsResponseTypeDef",
     {
         "detectorModelVersionSummaries": List[DetectorModelVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDynamoDBActionTypeDef = TypedDict(
     "_RequiredDynamoDBActionTypeDef",
     {
         "hashKeyField": str,
@@ -1016,15 +1066,15 @@
 
 
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "inputSummaries": List[InputSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IotSiteWiseInputIdentifierTypeDef = TypedDict(
     "IotSiteWiseInputIdentifierTypeDef",
     {
         "iotSiteWiseAssetModelPropertyIdentifier": IotSiteWiseAssetModelPropertyIdentifierTypeDef,
@@ -1033,15 +1083,15 @@
 )
 
 ListInputRoutingsResponseTypeDef = TypedDict(
     "ListInputRoutingsResponseTypeDef",
     {
         "routedResources": List[RoutedResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecipientDetailTypeDef = TypedDict(
     "RecipientDetailTypeDef",
     {
         "ssoIdentity": SSOIdentityTypeDef,
@@ -1050,15 +1100,15 @@
 )
 
 GetDetectorModelAnalysisResultsResponseTypeDef = TypedDict(
     "GetDetectorModelAnalysisResultsResponseTypeDef",
     {
         "analysisResults": List[AnalysisResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "entryId": str,
@@ -1066,14 +1116,23 @@
         "propertyId": str,
         "propertyAlias": str,
         "propertyValue": AssetPropertyValueTypeDef,
     },
     total=False,
 )
 
+InputTypeDef = TypedDict(
+    "InputTypeDef",
+    {
+        "inputConfiguration": InputConfigurationTypeDef,
+        "inputDefinition": InputDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateInputRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInputRequestRequestTypeDef",
     {
         "inputName": str,
         "inputDefinition": InputDefinitionTypeDef,
     },
 )
@@ -1089,23 +1148,15 @@
 
 class CreateInputRequestRequestTypeDef(
     _RequiredCreateInputRequestRequestTypeDef, _OptionalCreateInputRequestRequestTypeDef
 ):
     pass
 
 
-InputTypeDef = TypedDict(
-    "InputTypeDef",
-    {
-        "inputConfiguration": InputConfigurationTypeDef,
-        "inputDefinition": InputDefinitionTypeDef,
-    },
-    total=False,
-)
-
+InputDefinitionUnionTypeDef = Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef]
 _RequiredUpdateInputRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInputRequestRequestTypeDef",
     {
         "inputName": str,
         "inputDefinition": InputDefinitionTypeDef,
     },
 )
@@ -1123,19 +1174,20 @@
 ):
     pass
 
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
-        "loggingOptions": LoggingOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "loggingOptions": LoggingOptionsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingOptionsUnionTypeDef = Union[LoggingOptionsTypeDef, LoggingOptionsOutputTypeDef]
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
     },
 )
 
@@ -1152,22 +1204,52 @@
     {
         "iotEventsInputIdentifier": IotEventsInputIdentifierTypeDef,
         "iotSiteWiseInputIdentifier": IotSiteWiseInputIdentifierTypeDef,
     },
     total=False,
 )
 
+EmailRecipientsOutputTypeDef = TypedDict(
+    "EmailRecipientsOutputTypeDef",
+    {
+        "to": List[RecipientDetailTypeDef],
+    },
+    total=False,
+)
+
 EmailRecipientsTypeDef = TypedDict(
     "EmailRecipientsTypeDef",
     {
         "to": Sequence[RecipientDetailTypeDef],
     },
     total=False,
 )
 
+_RequiredSMSConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSMSConfigurationOutputTypeDef",
+    {
+        "recipients": List[RecipientDetailTypeDef],
+    },
+)
+_OptionalSMSConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSMSConfigurationOutputTypeDef",
+    {
+        "senderId": str,
+        "additionalMessage": str,
+    },
+    total=False,
+)
+
+
+class SMSConfigurationOutputTypeDef(
+    _RequiredSMSConfigurationOutputTypeDef, _OptionalSMSConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredSMSConfigurationTypeDef = TypedDict(
     "_RequiredSMSConfigurationTypeDef",
     {
         "recipients": Sequence[RecipientDetailTypeDef],
     },
 )
 _OptionalSMSConfigurationTypeDef = TypedDict(
@@ -1220,15 +1302,15 @@
     total=False,
 )
 
 DescribeInputResponseTypeDef = TypedDict(
     "DescribeInputResponseTypeDef",
     {
         "input": InputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListInputRoutingsRequestRequestTypeDef = TypedDict(
     "_RequiredListInputRoutingsRequestRequestTypeDef",
     {
         "inputIdentifier": InputIdentifierTypeDef,
@@ -1246,14 +1328,36 @@
 
 class ListInputRoutingsRequestRequestTypeDef(
     _RequiredListInputRoutingsRequestRequestTypeDef, _OptionalListInputRoutingsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredEmailConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEmailConfigurationOutputTypeDef",
+    {
+        "from": str,
+        "recipients": EmailRecipientsOutputTypeDef,
+    },
+)
+_OptionalEmailConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEmailConfigurationOutputTypeDef",
+    {
+        "content": EmailContentTypeDef,
+    },
+    total=False,
+)
+
+
+class EmailConfigurationOutputTypeDef(
+    _RequiredEmailConfigurationOutputTypeDef, _OptionalEmailConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredEmailConfigurationTypeDef = TypedDict(
     "_RequiredEmailConfigurationTypeDef",
     {
         "from": str,
         "recipients": EmailRecipientsTypeDef,
     },
 )
@@ -1268,14 +1372,34 @@
 
 class EmailConfigurationTypeDef(
     _RequiredEmailConfigurationTypeDef, _OptionalEmailConfigurationTypeDef
 ):
     pass
 
 
+_RequiredEventOutputTypeDef = TypedDict(
+    "_RequiredEventOutputTypeDef",
+    {
+        "eventName": str,
+    },
+)
+_OptionalEventOutputTypeDef = TypedDict(
+    "_OptionalEventOutputTypeDef",
+    {
+        "condition": str,
+        "actions": List[ActionTypeDef],
+    },
+    total=False,
+)
+
+
+class EventOutputTypeDef(_RequiredEventOutputTypeDef, _OptionalEventOutputTypeDef):
+    pass
+
+
 _RequiredEventTypeDef = TypedDict(
     "_RequiredEventTypeDef",
     {
         "eventName": str,
     },
 )
 _OptionalEventTypeDef = TypedDict(
@@ -1288,14 +1412,37 @@
 )
 
 
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
 
+_RequiredTransitionEventOutputTypeDef = TypedDict(
+    "_RequiredTransitionEventOutputTypeDef",
+    {
+        "eventName": str,
+        "condition": str,
+        "nextState": str,
+    },
+)
+_OptionalTransitionEventOutputTypeDef = TypedDict(
+    "_OptionalTransitionEventOutputTypeDef",
+    {
+        "actions": List[ActionTypeDef],
+    },
+    total=False,
+)
+
+
+class TransitionEventOutputTypeDef(
+    _RequiredTransitionEventOutputTypeDef, _OptionalTransitionEventOutputTypeDef
+):
+    pass
+
+
 _RequiredTransitionEventTypeDef = TypedDict(
     "_RequiredTransitionEventTypeDef",
     {
         "eventName": str,
         "condition": str,
         "nextState": str,
     },
@@ -1309,22 +1456,52 @@
 )
 
 
 class TransitionEventTypeDef(_RequiredTransitionEventTypeDef, _OptionalTransitionEventTypeDef):
     pass
 
 
+AlarmEventActionsOutputTypeDef = TypedDict(
+    "AlarmEventActionsOutputTypeDef",
+    {
+        "alarmActions": List[AlarmActionTypeDef],
+    },
+    total=False,
+)
+
 AlarmEventActionsTypeDef = TypedDict(
     "AlarmEventActionsTypeDef",
     {
         "alarmActions": Sequence[AlarmActionTypeDef],
     },
     total=False,
 )
 
+_RequiredNotificationActionOutputTypeDef = TypedDict(
+    "_RequiredNotificationActionOutputTypeDef",
+    {
+        "action": NotificationTargetActionsTypeDef,
+    },
+)
+_OptionalNotificationActionOutputTypeDef = TypedDict(
+    "_OptionalNotificationActionOutputTypeDef",
+    {
+        "smsConfigurations": List[SMSConfigurationOutputTypeDef],
+        "emailConfigurations": List[EmailConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class NotificationActionOutputTypeDef(
+    _RequiredNotificationActionOutputTypeDef, _OptionalNotificationActionOutputTypeDef
+):
+    pass
+
+
 _RequiredNotificationActionTypeDef = TypedDict(
     "_RequiredNotificationActionTypeDef",
     {
         "action": NotificationTargetActionsTypeDef,
     },
 )
 _OptionalNotificationActionTypeDef = TypedDict(
@@ -1339,14 +1516,30 @@
 
 class NotificationActionTypeDef(
     _RequiredNotificationActionTypeDef, _OptionalNotificationActionTypeDef
 ):
     pass
 
 
+OnEnterLifecycleOutputTypeDef = TypedDict(
+    "OnEnterLifecycleOutputTypeDef",
+    {
+        "events": List[EventOutputTypeDef],
+    },
+    total=False,
+)
+
+OnExitLifecycleOutputTypeDef = TypedDict(
+    "OnExitLifecycleOutputTypeDef",
+    {
+        "events": List[EventOutputTypeDef],
+    },
+    total=False,
+)
+
 OnEnterLifecycleTypeDef = TypedDict(
     "OnEnterLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
 )
@@ -1355,31 +1548,70 @@
     "OnExitLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
 )
 
+OnInputLifecycleOutputTypeDef = TypedDict(
+    "OnInputLifecycleOutputTypeDef",
+    {
+        "events": List[EventOutputTypeDef],
+        "transitionEvents": List[TransitionEventOutputTypeDef],
+    },
+    total=False,
+)
+
 OnInputLifecycleTypeDef = TypedDict(
     "OnInputLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
         "transitionEvents": Sequence[TransitionEventTypeDef],
     },
     total=False,
 )
 
+AlarmEventActionsUnionTypeDef = Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef]
+AlarmNotificationOutputTypeDef = TypedDict(
+    "AlarmNotificationOutputTypeDef",
+    {
+        "notificationActions": List[NotificationActionOutputTypeDef],
+    },
+    total=False,
+)
+
 AlarmNotificationTypeDef = TypedDict(
     "AlarmNotificationTypeDef",
     {
         "notificationActions": Sequence[NotificationActionTypeDef],
     },
     total=False,
 )
 
+_RequiredStateOutputTypeDef = TypedDict(
+    "_RequiredStateOutputTypeDef",
+    {
+        "stateName": str,
+    },
+)
+_OptionalStateOutputTypeDef = TypedDict(
+    "_OptionalStateOutputTypeDef",
+    {
+        "onInput": OnInputLifecycleOutputTypeDef,
+        "onEnter": OnEnterLifecycleOutputTypeDef,
+        "onExit": OnExitLifecycleOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class StateOutputTypeDef(_RequiredStateOutputTypeDef, _OptionalStateOutputTypeDef):
+    pass
+
+
 _RequiredStateTypeDef = TypedDict(
     "_RequiredStateTypeDef",
     {
         "stateName": str,
     },
 )
 _OptionalStateTypeDef = TypedDict(
@@ -1393,14 +1625,37 @@
 )
 
 
 class StateTypeDef(_RequiredStateTypeDef, _OptionalStateTypeDef):
     pass
 
 
+DescribeAlarmModelResponseTypeDef = TypedDict(
+    "DescribeAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "statusMessage": str,
+        "alarmModelName": str,
+        "alarmModelDescription": str,
+        "roleArn": str,
+        "key": str,
+        "severity": int,
+        "alarmRule": AlarmRuleTypeDef,
+        "alarmNotification": AlarmNotificationOutputTypeDef,
+        "alarmEventActions": AlarmEventActionsOutputTypeDef,
+        "alarmCapabilities": AlarmCapabilitiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AlarmNotificationUnionTypeDef = Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef]
 _RequiredCreateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
         "roleArn": str,
         "alarmRule": AlarmRuleTypeDef,
     },
@@ -1422,36 +1677,14 @@
 
 class CreateAlarmModelRequestRequestTypeDef(
     _RequiredCreateAlarmModelRequestRequestTypeDef, _OptionalCreateAlarmModelRequestRequestTypeDef
 ):
     pass
 
 
-DescribeAlarmModelResponseTypeDef = TypedDict(
-    "DescribeAlarmModelResponseTypeDef",
-    {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "statusMessage": str,
-        "alarmModelName": str,
-        "alarmModelDescription": str,
-        "roleArn": str,
-        "key": str,
-        "severity": int,
-        "alarmRule": AlarmRuleTypeDef,
-        "alarmNotification": AlarmNotificationTypeDef,
-        "alarmEventActions": AlarmEventActionsTypeDef,
-        "alarmCapabilities": AlarmCapabilitiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
         "roleArn": str,
         "alarmRule": AlarmRuleTypeDef,
     },
@@ -1471,22 +1704,39 @@
 
 class UpdateAlarmModelRequestRequestTypeDef(
     _RequiredUpdateAlarmModelRequestRequestTypeDef, _OptionalUpdateAlarmModelRequestRequestTypeDef
 ):
     pass
 
 
+DetectorModelDefinitionOutputTypeDef = TypedDict(
+    "DetectorModelDefinitionOutputTypeDef",
+    {
+        "states": List[StateOutputTypeDef],
+        "initialStateName": str,
+    },
+)
+
 DetectorModelDefinitionTypeDef = TypedDict(
     "DetectorModelDefinitionTypeDef",
     {
         "states": Sequence[StateTypeDef],
         "initialStateName": str,
     },
 )
 
+DetectorModelTypeDef = TypedDict(
+    "DetectorModelTypeDef",
+    {
+        "detectorModelDefinition": DetectorModelDefinitionOutputTypeDef,
+        "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateDetectorModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDetectorModelRequestRequestTypeDef",
     {
         "detectorModelName": str,
         "detectorModelDefinition": DetectorModelDefinitionTypeDef,
         "roleArn": str,
     },
@@ -1506,23 +1756,17 @@
 class CreateDetectorModelRequestRequestTypeDef(
     _RequiredCreateDetectorModelRequestRequestTypeDef,
     _OptionalCreateDetectorModelRequestRequestTypeDef,
 ):
     pass
 
 
-DetectorModelTypeDef = TypedDict(
-    "DetectorModelTypeDef",
-    {
-        "detectorModelDefinition": DetectorModelDefinitionTypeDef,
-        "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-    },
-    total=False,
-)
-
+DetectorModelDefinitionUnionTypeDef = Union[
+    DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
+]
 StartDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     {
         "detectorModelDefinition": DetectorModelDefinitionTypeDef,
     },
 )
 
@@ -1551,10 +1795,10 @@
     pass
 
 
 DescribeDetectorModelResponseTypeDef = TypedDict(
     "DescribeDetectorModelResponseTypeDef",
     {
         "detectorModel": DetectorModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents/type_defs.pyi` & `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/type_defs.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iotevents.type_defs import AcknowledgeFlowTypeDef
 
-    data: AcknowledgeFlowTypeDef = {...}
+    data: AcknowledgeFlowTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AlarmModelVersionStatusType,
     AnalysisResultLevelType,
     AnalysisStatusType,
     ComparisonOperatorType,
     DetectorModelVersionStatusType,
@@ -43,60 +43,62 @@
     "AlarmModelVersionSummaryTypeDef",
     "SimpleRuleTypeDef",
     "AnalysisResultLocationTypeDef",
     "AssetPropertyTimestampTypeDef",
     "AssetPropertyVariantTypeDef",
     "AttributeTypeDef",
     "TagTypeDef",
-    "CreateAlarmModelResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DetectorModelConfigurationTypeDef",
     "InputConfigurationTypeDef",
     "DeleteAlarmModelRequestRequestTypeDef",
     "DeleteDetectorModelRequestRequestTypeDef",
     "DeleteInputRequestRequestTypeDef",
     "DescribeAlarmModelRequestRequestTypeDef",
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
-    "DescribeDetectorModelAnalysisResponseTypeDef",
     "DescribeDetectorModelRequestRequestTypeDef",
     "DescribeInputRequestRequestTypeDef",
     "DetectorDebugOptionTypeDef",
     "DetectorModelSummaryTypeDef",
     "DetectorModelVersionSummaryTypeDef",
     "PayloadTypeDef",
     "EmailContentTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetDetectorModelAnalysisResultsRequestRequestTypeDef",
     "IotEventsInputIdentifierTypeDef",
     "InputSummaryTypeDef",
     "IotSiteWiseAssetModelPropertyIdentifierTypeDef",
     "ListAlarmModelVersionsRequestRequestTypeDef",
     "ListAlarmModelsRequestRequestTypeDef",
     "ListDetectorModelVersionsRequestRequestTypeDef",
     "ListDetectorModelsRequestRequestTypeDef",
     "RoutedResourceTypeDef",
     "ListInputsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "SSOIdentityTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartDetectorModelAnalysisResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAlarmModelResponseTypeDef",
     "AlarmCapabilitiesTypeDef",
-    "ListAlarmModelsResponseTypeDef",
-    "ListAlarmModelVersionsResponseTypeDef",
     "AlarmRuleTypeDef",
     "AnalysisResultTypeDef",
     "AssetPropertyValueTypeDef",
+    "InputDefinitionOutputTypeDef",
     "InputDefinitionTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateAlarmModelResponseTypeDef",
+    "DescribeDetectorModelAnalysisResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListAlarmModelVersionsResponseTypeDef",
+    "ListAlarmModelsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartDetectorModelAnalysisResponseTypeDef",
+    "UpdateAlarmModelResponseTypeDef",
     "CreateDetectorModelResponseTypeDef",
     "UpdateDetectorModelResponseTypeDef",
     "CreateInputResponseTypeDef",
     "UpdateInputResponseTypeDef",
+    "LoggingOptionsOutputTypeDef",
     "LoggingOptionsTypeDef",
     "ListDetectorModelsResponseTypeDef",
     "ListDetectorModelVersionsResponseTypeDef",
     "DynamoDBActionTypeDef",
     "DynamoDBv2ActionTypeDef",
     "FirehoseActionTypeDef",
     "IotEventsActionTypeDef",
@@ -106,43 +108,61 @@
     "SqsActionTypeDef",
     "ListInputsResponseTypeDef",
     "IotSiteWiseInputIdentifierTypeDef",
     "ListInputRoutingsResponseTypeDef",
     "RecipientDetailTypeDef",
     "GetDetectorModelAnalysisResultsResponseTypeDef",
     "IotSiteWiseActionTypeDef",
-    "CreateInputRequestRequestTypeDef",
     "InputTypeDef",
+    "CreateInputRequestRequestTypeDef",
+    "InputDefinitionUnionTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
+    "LoggingOptionsUnionTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "NotificationTargetActionsTypeDef",
     "InputIdentifierTypeDef",
+    "EmailRecipientsOutputTypeDef",
     "EmailRecipientsTypeDef",
+    "SMSConfigurationOutputTypeDef",
     "SMSConfigurationTypeDef",
     "ActionTypeDef",
     "AlarmActionTypeDef",
     "DescribeInputResponseTypeDef",
     "ListInputRoutingsRequestRequestTypeDef",
+    "EmailConfigurationOutputTypeDef",
     "EmailConfigurationTypeDef",
+    "EventOutputTypeDef",
     "EventTypeDef",
+    "TransitionEventOutputTypeDef",
     "TransitionEventTypeDef",
+    "AlarmEventActionsOutputTypeDef",
     "AlarmEventActionsTypeDef",
+    "NotificationActionOutputTypeDef",
     "NotificationActionTypeDef",
+    "OnEnterLifecycleOutputTypeDef",
+    "OnExitLifecycleOutputTypeDef",
     "OnEnterLifecycleTypeDef",
     "OnExitLifecycleTypeDef",
+    "OnInputLifecycleOutputTypeDef",
     "OnInputLifecycleTypeDef",
+    "AlarmEventActionsUnionTypeDef",
+    "AlarmNotificationOutputTypeDef",
     "AlarmNotificationTypeDef",
+    "StateOutputTypeDef",
     "StateTypeDef",
-    "CreateAlarmModelRequestRequestTypeDef",
     "DescribeAlarmModelResponseTypeDef",
+    "AlarmNotificationUnionTypeDef",
+    "CreateAlarmModelRequestRequestTypeDef",
     "UpdateAlarmModelRequestRequestTypeDef",
+    "DetectorModelDefinitionOutputTypeDef",
     "DetectorModelDefinitionTypeDef",
-    "CreateDetectorModelRequestRequestTypeDef",
     "DetectorModelTypeDef",
+    "CreateDetectorModelRequestRequestTypeDef",
+    "DetectorModelDefinitionUnionTypeDef",
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     "UpdateDetectorModelRequestRequestTypeDef",
     "DescribeDetectorModelResponseTypeDef",
 )
 
 AcknowledgeFlowTypeDef = TypedDict(
     "AcknowledgeFlowTypeDef",
@@ -281,23 +301,22 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-CreateAlarmModelResponseTypeDef = TypedDict(
-    "CreateAlarmModelResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DetectorModelConfigurationTypeDef = TypedDict(
     "DetectorModelConfigurationTypeDef",
     {
         "detectorModelName": str,
@@ -381,22 +400,14 @@
 DescribeDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 
-DescribeDetectorModelAnalysisResponseTypeDef = TypedDict(
-    "DescribeDetectorModelAnalysisResponseTypeDef",
-    {
-        "status": AnalysisStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeDetectorModelRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeDetectorModelRequestRequestTypeDef",
     {
         "detectorModelName": str,
     },
 )
 _OptionalDescribeDetectorModelRequestRequestTypeDef = TypedDict(
@@ -477,21 +488,14 @@
     {
         "subject": str,
         "additionalMessage": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 _OptionalGetDetectorModelAnalysisResultsRequestRequestTypeDef = TypedDict(
@@ -635,80 +639,31 @@
     },
     total=False,
 )
 
 class SSOIdentityTypeDef(_RequiredSSOIdentityTypeDef, _OptionalSSOIdentityTypeDef):
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
-StartDetectorModelAnalysisResponseTypeDef = TypedDict(
-    "StartDetectorModelAnalysisResponseTypeDef",
-    {
-        "analysisId": str,
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
 
-UpdateAlarmModelResponseTypeDef = TypedDict(
-    "UpdateAlarmModelResponseTypeDef",
-    {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AlarmCapabilitiesTypeDef = TypedDict(
     "AlarmCapabilitiesTypeDef",
     {
         "initializationConfiguration": InitializationConfigurationTypeDef,
         "acknowledgeFlow": AcknowledgeFlowTypeDef,
     },
     total=False,
 )
 
-ListAlarmModelsResponseTypeDef = TypedDict(
-    "ListAlarmModelsResponseTypeDef",
-    {
-        "alarmModelSummaries": List[AlarmModelSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAlarmModelVersionsResponseTypeDef = TypedDict(
-    "ListAlarmModelVersionsResponseTypeDef",
-    {
-        "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AlarmRuleTypeDef = TypedDict(
     "AlarmRuleTypeDef",
     {
         "simpleRule": SimpleRuleTypeDef,
     },
     total=False,
 )
@@ -730,103 +685,196 @@
         "value": AssetPropertyVariantTypeDef,
         "timestamp": AssetPropertyTimestampTypeDef,
         "quality": str,
     },
     total=False,
 )
 
+InputDefinitionOutputTypeDef = TypedDict(
+    "InputDefinitionOutputTypeDef",
+    {
+        "attributes": List[AttributeTypeDef],
+    },
+)
+
 InputDefinitionTypeDef = TypedDict(
     "InputDefinitionTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+
+CreateAlarmModelResponseTypeDef = TypedDict(
+    "CreateAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDetectorModelAnalysisResponseTypeDef = TypedDict(
+    "DescribeDetectorModelAnalysisResponseTypeDef",
+    {
+        "status": AnalysisStatusType,
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
+ListAlarmModelVersionsResponseTypeDef = TypedDict(
+    "ListAlarmModelVersionsResponseTypeDef",
+    {
+        "alarmModelVersionSummaries": List[AlarmModelVersionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAlarmModelsResponseTypeDef = TypedDict(
+    "ListAlarmModelsResponseTypeDef",
+    {
+        "alarmModelSummaries": List[AlarmModelSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+StartDetectorModelAnalysisResponseTypeDef = TypedDict(
+    "StartDetectorModelAnalysisResponseTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagTypeDef],
+        "analysisId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAlarmModelResponseTypeDef = TypedDict(
+    "UpdateAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDetectorModelResponseTypeDef = TypedDict(
     "CreateDetectorModelResponseTypeDef",
     {
         "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDetectorModelResponseTypeDef = TypedDict(
     "UpdateDetectorModelResponseTypeDef",
     {
         "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInputResponseTypeDef = TypedDict(
     "CreateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInputResponseTypeDef = TypedDict(
     "UpdateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredLoggingOptionsOutputTypeDef = TypedDict(
+    "_RequiredLoggingOptionsOutputTypeDef",
+    {
+        "roleArn": str,
+        "level": LoggingLevelType,
+        "enabled": bool,
+    },
+)
+_OptionalLoggingOptionsOutputTypeDef = TypedDict(
+    "_OptionalLoggingOptionsOutputTypeDef",
+    {
+        "detectorDebugOptions": List[DetectorDebugOptionTypeDef],
+    },
+    total=False,
+)
+
+class LoggingOptionsOutputTypeDef(
+    _RequiredLoggingOptionsOutputTypeDef, _OptionalLoggingOptionsOutputTypeDef
+):
+    pass
+
 _RequiredLoggingOptionsTypeDef = TypedDict(
     "_RequiredLoggingOptionsTypeDef",
     {
         "roleArn": str,
         "level": LoggingLevelType,
         "enabled": bool,
     },
 )
 _OptionalLoggingOptionsTypeDef = TypedDict(
     "_OptionalLoggingOptionsTypeDef",
     {
-        "detectorDebugOptions": List[DetectorDebugOptionTypeDef],
+        "detectorDebugOptions": Sequence[DetectorDebugOptionTypeDef],
     },
     total=False,
 )
 
 class LoggingOptionsTypeDef(_RequiredLoggingOptionsTypeDef, _OptionalLoggingOptionsTypeDef):
     pass
 
 ListDetectorModelsResponseTypeDef = TypedDict(
     "ListDetectorModelsResponseTypeDef",
     {
         "detectorModelSummaries": List[DetectorModelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDetectorModelVersionsResponseTypeDef = TypedDict(
     "ListDetectorModelVersionsResponseTypeDef",
     {
         "detectorModelVersionSummaries": List[DetectorModelVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDynamoDBActionTypeDef = TypedDict(
     "_RequiredDynamoDBActionTypeDef",
     {
         "hashKeyField": str,
@@ -977,15 +1025,15 @@
     pass
 
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "inputSummaries": List[InputSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IotSiteWiseInputIdentifierTypeDef = TypedDict(
     "IotSiteWiseInputIdentifierTypeDef",
     {
         "iotSiteWiseAssetModelPropertyIdentifier": IotSiteWiseAssetModelPropertyIdentifierTypeDef,
@@ -994,15 +1042,15 @@
 )
 
 ListInputRoutingsResponseTypeDef = TypedDict(
     "ListInputRoutingsResponseTypeDef",
     {
         "routedResources": List[RoutedResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecipientDetailTypeDef = TypedDict(
     "RecipientDetailTypeDef",
     {
         "ssoIdentity": SSOIdentityTypeDef,
@@ -1011,15 +1059,15 @@
 )
 
 GetDetectorModelAnalysisResultsResponseTypeDef = TypedDict(
     "GetDetectorModelAnalysisResultsResponseTypeDef",
     {
         "analysisResults": List[AnalysisResultTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IotSiteWiseActionTypeDef = TypedDict(
     "IotSiteWiseActionTypeDef",
     {
         "entryId": str,
@@ -1027,14 +1075,23 @@
         "propertyId": str,
         "propertyAlias": str,
         "propertyValue": AssetPropertyValueTypeDef,
     },
     total=False,
 )
 
+InputTypeDef = TypedDict(
+    "InputTypeDef",
+    {
+        "inputConfiguration": InputConfigurationTypeDef,
+        "inputDefinition": InputDefinitionOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateInputRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInputRequestRequestTypeDef",
     {
         "inputName": str,
         "inputDefinition": InputDefinitionTypeDef,
     },
 )
@@ -1048,23 +1105,15 @@
 )
 
 class CreateInputRequestRequestTypeDef(
     _RequiredCreateInputRequestRequestTypeDef, _OptionalCreateInputRequestRequestTypeDef
 ):
     pass
 
-InputTypeDef = TypedDict(
-    "InputTypeDef",
-    {
-        "inputConfiguration": InputConfigurationTypeDef,
-        "inputDefinition": InputDefinitionTypeDef,
-    },
-    total=False,
-)
-
+InputDefinitionUnionTypeDef = Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef]
 _RequiredUpdateInputRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInputRequestRequestTypeDef",
     {
         "inputName": str,
         "inputDefinition": InputDefinitionTypeDef,
     },
 )
@@ -1080,19 +1129,20 @@
     _RequiredUpdateInputRequestRequestTypeDef, _OptionalUpdateInputRequestRequestTypeDef
 ):
     pass
 
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
-        "loggingOptions": LoggingOptionsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "loggingOptions": LoggingOptionsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LoggingOptionsUnionTypeDef = Union[LoggingOptionsTypeDef, LoggingOptionsOutputTypeDef]
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
     },
 )
 
@@ -1109,22 +1159,50 @@
     {
         "iotEventsInputIdentifier": IotEventsInputIdentifierTypeDef,
         "iotSiteWiseInputIdentifier": IotSiteWiseInputIdentifierTypeDef,
     },
     total=False,
 )
 
+EmailRecipientsOutputTypeDef = TypedDict(
+    "EmailRecipientsOutputTypeDef",
+    {
+        "to": List[RecipientDetailTypeDef],
+    },
+    total=False,
+)
+
 EmailRecipientsTypeDef = TypedDict(
     "EmailRecipientsTypeDef",
     {
         "to": Sequence[RecipientDetailTypeDef],
     },
     total=False,
 )
 
+_RequiredSMSConfigurationOutputTypeDef = TypedDict(
+    "_RequiredSMSConfigurationOutputTypeDef",
+    {
+        "recipients": List[RecipientDetailTypeDef],
+    },
+)
+_OptionalSMSConfigurationOutputTypeDef = TypedDict(
+    "_OptionalSMSConfigurationOutputTypeDef",
+    {
+        "senderId": str,
+        "additionalMessage": str,
+    },
+    total=False,
+)
+
+class SMSConfigurationOutputTypeDef(
+    _RequiredSMSConfigurationOutputTypeDef, _OptionalSMSConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredSMSConfigurationTypeDef = TypedDict(
     "_RequiredSMSConfigurationTypeDef",
     {
         "recipients": Sequence[RecipientDetailTypeDef],
     },
 )
 _OptionalSMSConfigurationTypeDef = TypedDict(
@@ -1175,15 +1253,15 @@
     total=False,
 )
 
 DescribeInputResponseTypeDef = TypedDict(
     "DescribeInputResponseTypeDef",
     {
         "input": InputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListInputRoutingsRequestRequestTypeDef = TypedDict(
     "_RequiredListInputRoutingsRequestRequestTypeDef",
     {
         "inputIdentifier": InputIdentifierTypeDef,
@@ -1199,14 +1277,34 @@
 )
 
 class ListInputRoutingsRequestRequestTypeDef(
     _RequiredListInputRoutingsRequestRequestTypeDef, _OptionalListInputRoutingsRequestRequestTypeDef
 ):
     pass
 
+_RequiredEmailConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEmailConfigurationOutputTypeDef",
+    {
+        "from": str,
+        "recipients": EmailRecipientsOutputTypeDef,
+    },
+)
+_OptionalEmailConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEmailConfigurationOutputTypeDef",
+    {
+        "content": EmailContentTypeDef,
+    },
+    total=False,
+)
+
+class EmailConfigurationOutputTypeDef(
+    _RequiredEmailConfigurationOutputTypeDef, _OptionalEmailConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredEmailConfigurationTypeDef = TypedDict(
     "_RequiredEmailConfigurationTypeDef",
     {
         "from": str,
         "recipients": EmailRecipientsTypeDef,
     },
 )
@@ -1219,14 +1317,32 @@
 )
 
 class EmailConfigurationTypeDef(
     _RequiredEmailConfigurationTypeDef, _OptionalEmailConfigurationTypeDef
 ):
     pass
 
+_RequiredEventOutputTypeDef = TypedDict(
+    "_RequiredEventOutputTypeDef",
+    {
+        "eventName": str,
+    },
+)
+_OptionalEventOutputTypeDef = TypedDict(
+    "_OptionalEventOutputTypeDef",
+    {
+        "condition": str,
+        "actions": List[ActionTypeDef],
+    },
+    total=False,
+)
+
+class EventOutputTypeDef(_RequiredEventOutputTypeDef, _OptionalEventOutputTypeDef):
+    pass
+
 _RequiredEventTypeDef = TypedDict(
     "_RequiredEventTypeDef",
     {
         "eventName": str,
     },
 )
 _OptionalEventTypeDef = TypedDict(
@@ -1237,14 +1353,35 @@
     },
     total=False,
 )
 
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
+_RequiredTransitionEventOutputTypeDef = TypedDict(
+    "_RequiredTransitionEventOutputTypeDef",
+    {
+        "eventName": str,
+        "condition": str,
+        "nextState": str,
+    },
+)
+_OptionalTransitionEventOutputTypeDef = TypedDict(
+    "_OptionalTransitionEventOutputTypeDef",
+    {
+        "actions": List[ActionTypeDef],
+    },
+    total=False,
+)
+
+class TransitionEventOutputTypeDef(
+    _RequiredTransitionEventOutputTypeDef, _OptionalTransitionEventOutputTypeDef
+):
+    pass
+
 _RequiredTransitionEventTypeDef = TypedDict(
     "_RequiredTransitionEventTypeDef",
     {
         "eventName": str,
         "condition": str,
         "nextState": str,
     },
@@ -1256,22 +1393,50 @@
     },
     total=False,
 )
 
 class TransitionEventTypeDef(_RequiredTransitionEventTypeDef, _OptionalTransitionEventTypeDef):
     pass
 
+AlarmEventActionsOutputTypeDef = TypedDict(
+    "AlarmEventActionsOutputTypeDef",
+    {
+        "alarmActions": List[AlarmActionTypeDef],
+    },
+    total=False,
+)
+
 AlarmEventActionsTypeDef = TypedDict(
     "AlarmEventActionsTypeDef",
     {
         "alarmActions": Sequence[AlarmActionTypeDef],
     },
     total=False,
 )
 
+_RequiredNotificationActionOutputTypeDef = TypedDict(
+    "_RequiredNotificationActionOutputTypeDef",
+    {
+        "action": NotificationTargetActionsTypeDef,
+    },
+)
+_OptionalNotificationActionOutputTypeDef = TypedDict(
+    "_OptionalNotificationActionOutputTypeDef",
+    {
+        "smsConfigurations": List[SMSConfigurationOutputTypeDef],
+        "emailConfigurations": List[EmailConfigurationOutputTypeDef],
+    },
+    total=False,
+)
+
+class NotificationActionOutputTypeDef(
+    _RequiredNotificationActionOutputTypeDef, _OptionalNotificationActionOutputTypeDef
+):
+    pass
+
 _RequiredNotificationActionTypeDef = TypedDict(
     "_RequiredNotificationActionTypeDef",
     {
         "action": NotificationTargetActionsTypeDef,
     },
 )
 _OptionalNotificationActionTypeDef = TypedDict(
@@ -1284,14 +1449,30 @@
 )
 
 class NotificationActionTypeDef(
     _RequiredNotificationActionTypeDef, _OptionalNotificationActionTypeDef
 ):
     pass
 
+OnEnterLifecycleOutputTypeDef = TypedDict(
+    "OnEnterLifecycleOutputTypeDef",
+    {
+        "events": List[EventOutputTypeDef],
+    },
+    total=False,
+)
+
+OnExitLifecycleOutputTypeDef = TypedDict(
+    "OnExitLifecycleOutputTypeDef",
+    {
+        "events": List[EventOutputTypeDef],
+    },
+    total=False,
+)
+
 OnEnterLifecycleTypeDef = TypedDict(
     "OnEnterLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
 )
@@ -1300,31 +1481,68 @@
     "OnExitLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
 )
 
+OnInputLifecycleOutputTypeDef = TypedDict(
+    "OnInputLifecycleOutputTypeDef",
+    {
+        "events": List[EventOutputTypeDef],
+        "transitionEvents": List[TransitionEventOutputTypeDef],
+    },
+    total=False,
+)
+
 OnInputLifecycleTypeDef = TypedDict(
     "OnInputLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
         "transitionEvents": Sequence[TransitionEventTypeDef],
     },
     total=False,
 )
 
+AlarmEventActionsUnionTypeDef = Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef]
+AlarmNotificationOutputTypeDef = TypedDict(
+    "AlarmNotificationOutputTypeDef",
+    {
+        "notificationActions": List[NotificationActionOutputTypeDef],
+    },
+    total=False,
+)
+
 AlarmNotificationTypeDef = TypedDict(
     "AlarmNotificationTypeDef",
     {
         "notificationActions": Sequence[NotificationActionTypeDef],
     },
     total=False,
 )
 
+_RequiredStateOutputTypeDef = TypedDict(
+    "_RequiredStateOutputTypeDef",
+    {
+        "stateName": str,
+    },
+)
+_OptionalStateOutputTypeDef = TypedDict(
+    "_OptionalStateOutputTypeDef",
+    {
+        "onInput": OnInputLifecycleOutputTypeDef,
+        "onEnter": OnEnterLifecycleOutputTypeDef,
+        "onExit": OnExitLifecycleOutputTypeDef,
+    },
+    total=False,
+)
+
+class StateOutputTypeDef(_RequiredStateOutputTypeDef, _OptionalStateOutputTypeDef):
+    pass
+
 _RequiredStateTypeDef = TypedDict(
     "_RequiredStateTypeDef",
     {
         "stateName": str,
     },
 )
 _OptionalStateTypeDef = TypedDict(
@@ -1336,14 +1554,37 @@
     },
     total=False,
 )
 
 class StateTypeDef(_RequiredStateTypeDef, _OptionalStateTypeDef):
     pass
 
+DescribeAlarmModelResponseTypeDef = TypedDict(
+    "DescribeAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "statusMessage": str,
+        "alarmModelName": str,
+        "alarmModelDescription": str,
+        "roleArn": str,
+        "key": str,
+        "severity": int,
+        "alarmRule": AlarmRuleTypeDef,
+        "alarmNotification": AlarmNotificationOutputTypeDef,
+        "alarmEventActions": AlarmEventActionsOutputTypeDef,
+        "alarmCapabilities": AlarmCapabilitiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AlarmNotificationUnionTypeDef = Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef]
 _RequiredCreateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
         "roleArn": str,
         "alarmRule": AlarmRuleTypeDef,
     },
@@ -1363,36 +1604,14 @@
 )
 
 class CreateAlarmModelRequestRequestTypeDef(
     _RequiredCreateAlarmModelRequestRequestTypeDef, _OptionalCreateAlarmModelRequestRequestTypeDef
 ):
     pass
 
-DescribeAlarmModelResponseTypeDef = TypedDict(
-    "DescribeAlarmModelResponseTypeDef",
-    {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "statusMessage": str,
-        "alarmModelName": str,
-        "alarmModelDescription": str,
-        "roleArn": str,
-        "key": str,
-        "severity": int,
-        "alarmRule": AlarmRuleTypeDef,
-        "alarmNotification": AlarmNotificationTypeDef,
-        "alarmEventActions": AlarmEventActionsTypeDef,
-        "alarmCapabilities": AlarmCapabilitiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
         "roleArn": str,
         "alarmRule": AlarmRuleTypeDef,
     },
@@ -1410,22 +1629,39 @@
 )
 
 class UpdateAlarmModelRequestRequestTypeDef(
     _RequiredUpdateAlarmModelRequestRequestTypeDef, _OptionalUpdateAlarmModelRequestRequestTypeDef
 ):
     pass
 
+DetectorModelDefinitionOutputTypeDef = TypedDict(
+    "DetectorModelDefinitionOutputTypeDef",
+    {
+        "states": List[StateOutputTypeDef],
+        "initialStateName": str,
+    },
+)
+
 DetectorModelDefinitionTypeDef = TypedDict(
     "DetectorModelDefinitionTypeDef",
     {
         "states": Sequence[StateTypeDef],
         "initialStateName": str,
     },
 )
 
+DetectorModelTypeDef = TypedDict(
+    "DetectorModelTypeDef",
+    {
+        "detectorModelDefinition": DetectorModelDefinitionOutputTypeDef,
+        "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreateDetectorModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDetectorModelRequestRequestTypeDef",
     {
         "detectorModelName": str,
         "detectorModelDefinition": DetectorModelDefinitionTypeDef,
         "roleArn": str,
     },
@@ -1443,23 +1679,17 @@
 
 class CreateDetectorModelRequestRequestTypeDef(
     _RequiredCreateDetectorModelRequestRequestTypeDef,
     _OptionalCreateDetectorModelRequestRequestTypeDef,
 ):
     pass
 
-DetectorModelTypeDef = TypedDict(
-    "DetectorModelTypeDef",
-    {
-        "detectorModelDefinition": DetectorModelDefinitionTypeDef,
-        "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-    },
-    total=False,
-)
-
+DetectorModelDefinitionUnionTypeDef = Union[
+    DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
+]
 StartDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     {
         "detectorModelDefinition": DetectorModelDefinitionTypeDef,
     },
 )
 
@@ -1486,10 +1716,10 @@
 ):
     pass
 
 DescribeDetectorModelResponseTypeDef = TypedDict(
     "DescribeDetectorModelResponseTypeDef",
     {
         "detectorModel": DetectorModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/PKG-INFO` & `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotevents
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTEvents 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTEvents 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotevents type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotevents type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotevents"></a>
 
 # types-aiobotocore-iotevents
 
 [![PyPI - types-aiobotocore-iotevents](https://img.shields.io/pypi/v/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotevents?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotevents)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotevents)](https://pepy.tech/project/types-aiobotocore-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTEvents 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [types-aiobotocore-iotevents docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -289,20 +288,20 @@
 )
 
 
 def check_value(value: AlarmModelVersionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotevents.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotevents.type_defs import (
     AcknowledgeFlowTypeDef,
     ClearTimerActionTypeDef,
     ResetTimerActionTypeDef,
     SetTimerActionTypeDef,
@@ -312,60 +311,62 @@
     AlarmModelVersionSummaryTypeDef,
     SimpleRuleTypeDef,
     AnalysisResultLocationTypeDef,
     AssetPropertyTimestampTypeDef,
     AssetPropertyVariantTypeDef,
     AttributeTypeDef,
     TagTypeDef,
-    CreateAlarmModelResponseTypeDef,
+    ResponseMetadataTypeDef,
     DetectorModelConfigurationTypeDef,
     InputConfigurationTypeDef,
     DeleteAlarmModelRequestRequestTypeDef,
     DeleteDetectorModelRequestRequestTypeDef,
     DeleteInputRequestRequestTypeDef,
     DescribeAlarmModelRequestRequestTypeDef,
     DescribeDetectorModelAnalysisRequestRequestTypeDef,
-    DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelRequestRequestTypeDef,
     DescribeInputRequestRequestTypeDef,
     DetectorDebugOptionTypeDef,
     DetectorModelSummaryTypeDef,
     DetectorModelVersionSummaryTypeDef,
     PayloadTypeDef,
     EmailContentTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsRequestRequestTypeDef,
     IotEventsInputIdentifierTypeDef,
     InputSummaryTypeDef,
     IotSiteWiseAssetModelPropertyIdentifierTypeDef,
     ListAlarmModelVersionsRequestRequestTypeDef,
     ListAlarmModelsRequestRequestTypeDef,
     ListDetectorModelVersionsRequestRequestTypeDef,
     ListDetectorModelsRequestRequestTypeDef,
     RoutedResourceTypeDef,
     ListInputsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     SSOIdentityTypeDef,
-    ResponseMetadataTypeDef,
-    StartDetectorModelAnalysisResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAlarmModelResponseTypeDef,
     AlarmCapabilitiesTypeDef,
-    ListAlarmModelsResponseTypeDef,
-    ListAlarmModelVersionsResponseTypeDef,
     AlarmRuleTypeDef,
     AnalysisResultTypeDef,
     AssetPropertyValueTypeDef,
+    InputDefinitionOutputTypeDef,
     InputDefinitionTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateAlarmModelResponseTypeDef,
+    DescribeDetectorModelAnalysisResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListAlarmModelVersionsResponseTypeDef,
+    ListAlarmModelsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartDetectorModelAnalysisResponseTypeDef,
+    UpdateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     UpdateInputResponseTypeDef,
+    LoggingOptionsOutputTypeDef,
     LoggingOptionsTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
     DynamoDBActionTypeDef,
     DynamoDBv2ActionTypeDef,
     FirehoseActionTypeDef,
     IotEventsActionTypeDef,
@@ -375,50 +376,68 @@
     SqsActionTypeDef,
     ListInputsResponseTypeDef,
     IotSiteWiseInputIdentifierTypeDef,
     ListInputRoutingsResponseTypeDef,
     RecipientDetailTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
     IotSiteWiseActionTypeDef,
-    CreateInputRequestRequestTypeDef,
     InputTypeDef,
+    CreateInputRequestRequestTypeDef,
+    InputDefinitionUnionTypeDef,
     UpdateInputRequestRequestTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
+    LoggingOptionsUnionTypeDef,
     PutLoggingOptionsRequestRequestTypeDef,
     NotificationTargetActionsTypeDef,
     InputIdentifierTypeDef,
+    EmailRecipientsOutputTypeDef,
     EmailRecipientsTypeDef,
+    SMSConfigurationOutputTypeDef,
     SMSConfigurationTypeDef,
     ActionTypeDef,
     AlarmActionTypeDef,
     DescribeInputResponseTypeDef,
     ListInputRoutingsRequestRequestTypeDef,
+    EmailConfigurationOutputTypeDef,
     EmailConfigurationTypeDef,
+    EventOutputTypeDef,
     EventTypeDef,
+    TransitionEventOutputTypeDef,
     TransitionEventTypeDef,
+    AlarmEventActionsOutputTypeDef,
     AlarmEventActionsTypeDef,
+    NotificationActionOutputTypeDef,
     NotificationActionTypeDef,
+    OnEnterLifecycleOutputTypeDef,
+    OnExitLifecycleOutputTypeDef,
     OnEnterLifecycleTypeDef,
     OnExitLifecycleTypeDef,
+    OnInputLifecycleOutputTypeDef,
     OnInputLifecycleTypeDef,
+    AlarmEventActionsUnionTypeDef,
+    AlarmNotificationOutputTypeDef,
     AlarmNotificationTypeDef,
+    StateOutputTypeDef,
     StateTypeDef,
-    CreateAlarmModelRequestRequestTypeDef,
     DescribeAlarmModelResponseTypeDef,
+    AlarmNotificationUnionTypeDef,
+    CreateAlarmModelRequestRequestTypeDef,
     UpdateAlarmModelRequestRequestTypeDef,
+    DetectorModelDefinitionOutputTypeDef,
     DetectorModelDefinitionTypeDef,
-    CreateDetectorModelRequestRequestTypeDef,
     DetectorModelTypeDef,
+    CreateDetectorModelRequestRequestTypeDef,
+    DetectorModelDefinitionUnionTypeDef,
     StartDetectorModelAnalysisRequestRequestTypeDef,
     UpdateDetectorModelRequestRequestTypeDef,
     DescribeDetectorModelResponseTypeDef,
 )
 
 
-def get_structure() -> AcknowledgeFlowTypeDef:
+def get_value() -> AcknowledgeFlowTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotevents-2.5.2/types_aiobotocore_iotevents.egg-info/SOURCES.txt` & `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-chime-sdk-messaging-2.5.2.tar.gz` & `tmp/types-aiobotocore-chime-sdk-messaging-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-messaging-2.5.2.tar", last modified: Sat Jul  8 01:43:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-messaging-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
```

## Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.tar` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.261782 types-aiobotocore-chime-sdk-messaging-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:42.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18550 2023-07-08 01:43:19.261782 types-aiobotocore-chime-sdk-messaging-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16939 2023-07-08 01:26:42.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:19.261782 types-aiobotocore-chime-sdk-messaging-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-08 01:26:42.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.249782 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-08 01:26:42.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-08 01:26:42.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 01:26:42.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40511 2023-07-08 01:26:42.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40452 2023-07-08 01:26:42.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-07-08 01:26:42.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-07-08 01:26:42.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:42.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47661 2023-07-08 01:26:43.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47604 2023-07-08 01:26:43.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:42.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.261782 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18550 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.801642 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-08-02 14:51:57.801642 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.801642 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.793642 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40498 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40439 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48005 2023-08-02 14:34:12.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47948 2023-08-02 14:34:12.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.801642 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/LICENSE` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/PKG-INFO` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-messaging
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore chime-sdk-messaging type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore chime-sdk-messaging type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime-sdk-messaging"></a>
 
 # types-aiobotocore-chime-sdk-messaging
 
 [![PyPI - types-aiobotocore-chime-sdk-messaging](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime-sdk-messaging?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime-sdk-messaging)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-messaging)](https://pepy.tech/project/types-aiobotocore-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ChimeSDKMessaging 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [types-aiobotocore-chime-sdk-messaging docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/).
 
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
@@ -296,44 +295,44 @@
 )
 
 
 def check_value(value: AllowNotificationsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime_sdk_messaging.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_chime_sdk_messaging.type_defs import (
     AppInstanceUserMembershipSummaryTypeDef,
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ChannelAssociatedWithFlowSummaryTypeDef,
-    ChannelFlowCallbackResponseTypeDef,
     ChannelSummaryTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
+    MessageAttributeValueOutputTypeDef,
     TargetTypeDef,
     ElasticChannelConfigurationTypeDef,
     ExpirationSettingsTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
-    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
-    CreateChannelResponseTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
     DeleteChannelMessageRequestRequestTypeDef,
     DeleteChannelModeratorRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteMessagingStreamingConfigurationsRequestRequestTypeDef,
@@ -341,79 +340,82 @@
     DescribeChannelFlowRequestRequestTypeDef,
     DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef,
     DescribeChannelMembershipRequestRequestTypeDef,
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociateChannelFlowRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelMembershipPreferencesRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetChannelMessageStatusRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
     StreamingConfigurationTypeDef,
     LambdaConfigurationTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelFlowsRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
-    ListChannelMessagesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
-    RedactChannelMessageResponseTypeDef,
-    ResponseMetadataTypeDef,
     SearchFieldTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    UpdateChannelResponseTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
+    ChannelFlowCallbackResponseTypeDef,
     CreateChannelBanResponseTypeDef,
+    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    UpdateChannelFlowResponseTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ChannelMembershipForAppInstanceUserSummaryTypeDef,
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
+    MessageAttributeValueUnionTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
     PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
     PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     ProcessorConfigurationTypeDef,
+    ListChannelMessagesRequestRequestTypeDef,
     ListSubChannelsResponseTypeDef,
     SearchChannelsRequestRequestTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
@@ -423,28 +425,29 @@
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
     PutChannelMembershipPreferencesRequestRequestTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     ChannelFlowCallbackRequestRequestTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ProcessorTypeDef,
     ChannelFlowSummaryTypeDef,
     ChannelFlowTypeDef,
     CreateChannelFlowRequestRequestTypeDef,
     UpdateChannelFlowRequestRequestTypeDef,
     ListChannelFlowsResponseTypeDef,
     DescribeChannelFlowResponseTypeDef,
 )
 
 
-def get_structure() -> AppInstanceUserMembershipSummaryTypeDef:
+def get_value() -> AppInstanceUserMembershipSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/README.md` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-chime-sdk-messaging"></a>
 
 # types-aiobotocore-chime-sdk-messaging
 
 [![PyPI - types-aiobotocore-chime-sdk-messaging](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime-sdk-messaging?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime-sdk-messaging)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-messaging)](https://pepy.tech/project/types-aiobotocore-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ChimeSDKMessaging 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [types-aiobotocore-chime-sdk-messaging docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/).
 
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
@@ -263,44 +263,44 @@
 )
 
 
 def check_value(value: AllowNotificationsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime_sdk_messaging.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_chime_sdk_messaging.type_defs import (
     AppInstanceUserMembershipSummaryTypeDef,
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ChannelAssociatedWithFlowSummaryTypeDef,
-    ChannelFlowCallbackResponseTypeDef,
     ChannelSummaryTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
+    MessageAttributeValueOutputTypeDef,
     TargetTypeDef,
     ElasticChannelConfigurationTypeDef,
     ExpirationSettingsTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
-    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
-    CreateChannelResponseTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
     DeleteChannelMessageRequestRequestTypeDef,
     DeleteChannelModeratorRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteMessagingStreamingConfigurationsRequestRequestTypeDef,
@@ -308,79 +308,82 @@
     DescribeChannelFlowRequestRequestTypeDef,
     DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef,
     DescribeChannelMembershipRequestRequestTypeDef,
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociateChannelFlowRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelMembershipPreferencesRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetChannelMessageStatusRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
     StreamingConfigurationTypeDef,
     LambdaConfigurationTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelFlowsRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
-    ListChannelMessagesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
-    RedactChannelMessageResponseTypeDef,
-    ResponseMetadataTypeDef,
     SearchFieldTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    UpdateChannelResponseTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
+    ChannelFlowCallbackResponseTypeDef,
     CreateChannelBanResponseTypeDef,
+    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    UpdateChannelFlowResponseTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ChannelMembershipForAppInstanceUserSummaryTypeDef,
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
+    MessageAttributeValueUnionTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
     PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
     PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     ProcessorConfigurationTypeDef,
+    ListChannelMessagesRequestRequestTypeDef,
     ListSubChannelsResponseTypeDef,
     SearchChannelsRequestRequestTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
@@ -390,28 +393,29 @@
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
     PutChannelMembershipPreferencesRequestRequestTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     ChannelFlowCallbackRequestRequestTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ProcessorTypeDef,
     ChannelFlowSummaryTypeDef,
     ChannelFlowTypeDef,
     CreateChannelFlowRequestRequestTypeDef,
     UpdateChannelFlowRequestRequestTypeDef,
     ListChannelFlowsResponseTypeDef,
     DescribeChannelFlowResponseTypeDef,
 )
 
 
-def get_structure() -> AppInstanceUserMembershipSummaryTypeDef:
+def get_value() -> AppInstanceUserMembershipSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/setup.py` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-messaging",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_chime_sdk_messaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2 service generated with"
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
-        "aiobotocore chime-sdk-messaging type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore chime-sdk-messaging type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_chime_sdk_messaging": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/__init__.py` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/__init__.pyi` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/__main__.py` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging\nOther"
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

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/client.py` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from types_aiobotocore_chime_sdk_messaging.client import ChimeSDKMessagingClient
 
     session = get_session()
     async with session.create_client("chime-sdk-messaging") as client:
         client: ChimeSDKMessagingClient
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     ChannelMembershipTypeType,
     ChannelMessagePersistenceTypeType,
@@ -60,27 +59,28 @@
     ListChannelMessagesResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsResponseTypeDef,
     ListSubChannelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MessageAttributeValueTypeDef,
+    MessageAttributeValueUnionTypeDef,
     ProcessorTypeDef,
     PushNotificationConfigurationTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     RedactChannelMessageResponseTypeDef,
     SearchChannelsResponseTypeDef,
     SearchFieldTypeDef,
     SendChannelMessageResponseTypeDef,
     StreamingConfigurationTypeDef,
     TagTypeDef,
     TargetTypeDef,
+    TimestampTypeDef,
     UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 __all__ = ("ChimeSDKMessagingClient",)
@@ -525,16 +525,16 @@
 
     async def list_channel_messages(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         SortOrder: SortOrderType = ...,
-        NotBefore: Union[datetime, str] = ...,
-        NotAfter: Union[datetime, str] = ...,
+        NotBefore: TimestampTypeDef = ...,
+        NotAfter: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SubChannelId: str = ...
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
@@ -688,15 +688,15 @@
         Content: str,
         Type: ChannelMessageTypeType,
         Persistence: ChannelMessagePersistenceTypeType,
         ClientRequestToken: str,
         ChimeBearer: str,
         Metadata: str = ...,
         PushNotification: PushNotificationConfigurationTypeDef = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,
         SubChannelId: str = ...,
         ContentType: str = ...,
         Target: Sequence[TargetTypeDef] = ...
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/client.pyi` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from types_aiobotocore_chime_sdk_messaging.client import ChimeSDKMessagingClient
 
     session = get_session()
     async with session.create_client("chime-sdk-messaging") as client:
         client: ChimeSDKMessagingClient
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     ChannelMembershipTypeType,
     ChannelMessagePersistenceTypeType,
@@ -60,27 +59,28 @@
     ListChannelMessagesResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsResponseTypeDef,
     ListSubChannelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MessageAttributeValueTypeDef,
+    MessageAttributeValueUnionTypeDef,
     ProcessorTypeDef,
     PushNotificationConfigurationTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     RedactChannelMessageResponseTypeDef,
     SearchChannelsResponseTypeDef,
     SearchFieldTypeDef,
     SendChannelMessageResponseTypeDef,
     StreamingConfigurationTypeDef,
     TagTypeDef,
     TargetTypeDef,
+    TimestampTypeDef,
     UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelResponseTypeDef,
 )
 
 __all__ = ("ChimeSDKMessagingClient",)
@@ -486,16 +486,16 @@
         """
     async def list_channel_messages(
         self,
         *,
         ChannelArn: str,
         ChimeBearer: str,
         SortOrder: SortOrderType = ...,
-        NotBefore: Union[datetime, str] = ...,
-        NotAfter: Union[datetime, str] = ...,
+        NotBefore: TimestampTypeDef = ...,
+        NotAfter: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SubChannelId: str = ...
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
@@ -637,15 +637,15 @@
         Content: str,
         Type: ChannelMessageTypeType,
         Persistence: ChannelMessagePersistenceTypeType,
         ClientRequestToken: str,
         ChimeBearer: str,
         Metadata: str = ...,
         PushNotification: PushNotificationConfigurationTypeDef = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,
         SubChannelId: str = ...,
         ContentType: str = ...,
         Target: Sequence[TargetTypeDef] = ...
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/literals.py` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/literals.pyi` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/type_defs.py` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_chime_sdk_messaging.type_defs import AppInstanceUserMembershipSummaryTypeDef
 
-    data: AppInstanceUserMembershipSummaryTypeDef = {...}
+    data: AppInstanceUserMembershipSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -44,30 +44,29 @@
 
 __all__ = (
     "AppInstanceUserMembershipSummaryTypeDef",
     "AssociateChannelFlowRequestRequestTypeDef",
     "IdentityTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ChannelAssociatedWithFlowSummaryTypeDef",
-    "ChannelFlowCallbackResponseTypeDef",
     "ChannelSummaryTypeDef",
     "PushNotificationPreferencesTypeDef",
     "MessageAttributeValueTypeDef",
     "PushNotificationConfigurationTypeDef",
     "ChannelMessageStatusStructureTypeDef",
+    "MessageAttributeValueOutputTypeDef",
     "TargetTypeDef",
     "ElasticChannelConfigurationTypeDef",
     "ExpirationSettingsTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "TagTypeDef",
-    "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
-    "CreateChannelResponseTypeDef",
     "DeleteChannelBanRequestRequestTypeDef",
     "DeleteChannelFlowRequestRequestTypeDef",
     "DeleteChannelMembershipRequestRequestTypeDef",
     "DeleteChannelMessageRequestRequestTypeDef",
     "DeleteChannelModeratorRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteMessagingStreamingConfigurationsRequestRequestTypeDef",
@@ -75,79 +74,82 @@
     "DescribeChannelFlowRequestRequestTypeDef",
     "DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelMembershipRequestRequestTypeDef",
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelModeratorRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DisassociateChannelFlowRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     "GetChannelMessageRequestRequestTypeDef",
     "GetChannelMessageStatusRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
     "StreamingConfigurationTypeDef",
     "LambdaConfigurationTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelFlowsRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
-    "ListChannelMessagesRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
     "ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListSubChannelsRequestRequestTypeDef",
     "SubChannelSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
-    "RedactChannelMessageResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchFieldTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateChannelFlowResponseTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
-    "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "UpdateChannelResponseTypeDef",
     "BatchChannelMembershipsTypeDef",
     "ChannelBanSummaryTypeDef",
     "ChannelBanTypeDef",
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
+    "ChannelFlowCallbackResponseTypeDef",
     "CreateChannelBanResponseTypeDef",
+    "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipResponseTypeDef",
     "CreateChannelModeratorResponseTypeDef",
+    "CreateChannelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "RedactChannelMessageResponseTypeDef",
+    "UpdateChannelFlowResponseTypeDef",
+    "UpdateChannelReadMarkerResponseTypeDef",
+    "UpdateChannelResponseTypeDef",
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     "ChannelModeratedByAppInstanceUserSummaryTypeDef",
     "ListChannelsResponseTypeDef",
     "SearchChannelsResponseTypeDef",
     "ChannelMembershipPreferencesTypeDef",
     "ChannelMessageCallbackTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
+    "MessageAttributeValueUnionTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
-    "SendChannelMessageRequestRequestTypeDef",
     "ChannelTypeDef",
     "PutChannelExpirationSettingsRequestRequestTypeDef",
     "PutChannelExpirationSettingsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "PutMessagingStreamingConfigurationsResponseTypeDef",
     "ProcessorConfigurationTypeDef",
+    "ListChannelMessagesRequestRequestTypeDef",
     "ListSubChannelsResponseTypeDef",
     "SearchChannelsRequestRequestTypeDef",
     "BatchCreateChannelMembershipResponseTypeDef",
     "ListChannelBansResponseTypeDef",
     "DescribeChannelBanResponseTypeDef",
     "ListChannelMembershipsResponseTypeDef",
     "DescribeChannelMembershipResponseTypeDef",
@@ -157,14 +159,15 @@
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "GetChannelMembershipPreferencesResponseTypeDef",
     "PutChannelMembershipPreferencesRequestRequestTypeDef",
     "PutChannelMembershipPreferencesResponseTypeDef",
     "ChannelFlowCallbackRequestRequestTypeDef",
+    "SendChannelMessageRequestRequestTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "ProcessorTypeDef",
     "ChannelFlowSummaryTypeDef",
     "ChannelFlowTypeDef",
     "CreateChannelFlowRequestRequestTypeDef",
@@ -232,35 +235,37 @@
 class BatchCreateChannelMembershipRequestRequestTypeDef(
     _RequiredBatchCreateChannelMembershipRequestRequestTypeDef,
     _OptionalBatchCreateChannelMembershipRequestRequestTypeDef,
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
 ChannelAssociatedWithFlowSummaryTypeDef = TypedDict(
     "ChannelAssociatedWithFlowSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
     },
     total=False,
 )
 
-ChannelFlowCallbackResponseTypeDef = TypedDict(
-    "ChannelFlowCallbackResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "CallbackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -314,14 +319,22 @@
     {
         "Value": ChannelMessageStatusType,
         "Detail": str,
     },
     total=False,
 )
 
+MessageAttributeValueOutputTypeDef = TypedDict(
+    "MessageAttributeValueOutputTypeDef",
+    {
+        "StringValues": List[str],
+    },
+    total=False,
+)
+
 TargetTypeDef = TypedDict(
     "TargetTypeDef",
     {
         "MemberArn": str,
     },
     total=False,
 )
@@ -356,22 +369,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateChannelFlowResponseTypeDef = TypedDict(
-    "CreateChannelFlowResponseTypeDef",
-    {
-        "ChannelFlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateChannelMembershipRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelMembershipRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "Type": ChannelMembershipTypeType,
         "ChimeBearer": str,
@@ -398,22 +403,14 @@
     {
         "ChannelArn": str,
         "ChannelModeratorArn": str,
         "ChimeBearer": str,
     },
 )
 
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteChannelBanRequestRequestTypeDef = TypedDict(
     "DeleteChannelBanRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -578,21 +575,14 @@
     {
         "ChannelArn": str,
         "ChannelFlowArn": str,
         "ChimeBearer": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -767,42 +757,15 @@
 class ListChannelMembershipsRequestRequestTypeDef(
     _RequiredListChannelMembershipsRequestRequestTypeDef,
     _OptionalListChannelMembershipsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
-    "_RequiredListChannelMessagesRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "ChimeBearer": str,
-    },
-)
-_OptionalListChannelMessagesRequestRequestTypeDef = TypedDict(
-    "_OptionalListChannelMessagesRequestRequestTypeDef",
-    {
-        "SortOrder": SortOrderType,
-        "NotBefore": Union[datetime, str],
-        "NotAfter": Union[datetime, str],
-        "MaxResults": int,
-        "NextToken": str,
-        "SubChannelId": str,
-    },
-    total=False,
-)
-
-
-class ListChannelMessagesRequestRequestTypeDef(
-    _RequiredListChannelMessagesRequestRequestTypeDef,
-    _OptionalListChannelMessagesRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListChannelModeratorsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelModeratorsRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -953,35 +916,14 @@
 class RedactChannelMessageRequestRequestTypeDef(
     _RequiredRedactChannelMessageRequestRequestTypeDef,
     _OptionalRedactChannelMessageRequestRequestTypeDef,
 ):
     pass
 
 
-RedactChannelMessageResponseTypeDef = TypedDict(
-    "RedactChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "SubChannelId": str,
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
 SearchFieldTypeDef = TypedDict(
     "SearchFieldTypeDef",
     {
         "Key": Literal["MEMBERS"],
         "Values": Sequence[str],
         "Operator": SearchFieldOperatorType,
     },
@@ -991,22 +933,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateChannelFlowResponseTypeDef = TypedDict(
-    "UpdateChannelFlowResponseTypeDef",
-    {
-        "ChannelFlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Content": str,
         "ChimeBearer": str,
@@ -1034,22 +968,14 @@
     "UpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
 
-UpdateChannelReadMarkerResponseTypeDef = TypedDict(
-    "UpdateChannelReadMarkerResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -1066,22 +992,14 @@
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
 
-UpdateChannelResponseTypeDef = TypedDict(
-    "UpdateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchChannelMembershipsTypeDef = TypedDict(
     "BatchChannelMembershipsTypeDef",
     {
         "InvitedBy": IdentityTypeDef,
         "Type": ChannelMembershipTypeType,
         "Members": List[IdentityTypeDef],
         "ChannelArn": str,
@@ -1146,48 +1064,114 @@
         "ChannelArn": str,
         "CreatedTimestamp": datetime,
         "CreatedBy": IdentityTypeDef,
     },
     total=False,
 )
 
+ChannelFlowCallbackResponseTypeDef = TypedDict(
+    "ChannelFlowCallbackResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "CallbackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateChannelBanResponseTypeDef = TypedDict(
     "CreateChannelBanResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChannelFlowResponseTypeDef = TypedDict(
+    "CreateChannelFlowResponseTypeDef",
+    {
+        "ChannelFlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelMembershipResponseTypeDef = TypedDict(
     "CreateChannelMembershipResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "SubChannelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelModeratorResponseTypeDef = TypedDict(
     "CreateChannelModeratorResponseTypeDef",
     {
         "ChannelArn": str,
         "ChannelModerator": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
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
+RedactChannelMessageResponseTypeDef = TypedDict(
+    "RedactChannelMessageResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "MessageId": str,
+        "SubChannelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChannelFlowResponseTypeDef = TypedDict(
+    "UpdateChannelFlowResponseTypeDef",
+    {
+        "ChannelFlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChannelReadMarkerResponseTypeDef = TypedDict(
+    "UpdateChannelReadMarkerResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChannelResponseTypeDef = TypedDict(
+    "UpdateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsAssociatedWithChannelFlowResponseTypeDef = TypedDict(
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     {
         "Channels": List[ChannelAssociatedWithFlowSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChannelMembershipForAppInstanceUserSummaryTypeDef = TypedDict(
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     {
         "ChannelSummary": ChannelSummaryTypeDef,
@@ -1205,24 +1189,24 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchChannelsResponseTypeDef = TypedDict(
     "SearchChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChannelMembershipPreferencesTypeDef = TypedDict(
     "ChannelMembershipPreferencesTypeDef",
     {
         "PushNotifications": PushNotificationPreferencesTypeDef,
@@ -1256,54 +1240,57 @@
     pass
 
 
 GetChannelMessageStatusResponseTypeDef = TypedDict(
     "GetChannelMessageStatusResponseTypeDef",
     {
         "Status": ChannelMessageStatusStructureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendChannelMessageResponseTypeDef = TypedDict(
     "SendChannelMessageResponseTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelMessageResponseTypeDef = TypedDict(
     "UpdateChannelMessageResponseTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MessageAttributeValueUnionTypeDef = Union[
+    MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef
+]
 ChannelMessageSummaryTypeDef = TypedDict(
     "ChannelMessageSummaryTypeDef",
     {
         "MessageId": str,
         "Content": str,
         "Metadata": str,
         "Type": ChannelMessageTypeType,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Status": ChannelMessageStatusStructureTypeDef,
-        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
         "ContentType": str,
         "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
 ChannelMessageTypeDef = TypedDict(
@@ -1317,54 +1304,22 @@
         "CreatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Persistence": ChannelMessagePersistenceTypeType,
         "Status": ChannelMessageStatusStructureTypeDef,
-        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
         "SubChannelId": str,
         "ContentType": str,
         "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
-_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_RequiredSendChannelMessageRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "Content": str,
-        "Type": ChannelMessageTypeType,
-        "Persistence": ChannelMessagePersistenceTypeType,
-        "ClientRequestToken": str,
-        "ChimeBearer": str,
-    },
-)
-_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_OptionalSendChannelMessageRequestRequestTypeDef",
-    {
-        "Metadata": str,
-        "PushNotification": PushNotificationConfigurationTypeDef,
-        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
-        "SubChannelId": str,
-        "ContentType": str,
-        "Target": Sequence[TargetTypeDef],
-    },
-    total=False,
-)
-
-
-class SendChannelMessageRequestRequestTypeDef(
-    _RequiredSendChannelMessageRequestRequestTypeDef,
-    _OptionalSendChannelMessageRequestRequestTypeDef,
-):
-    pass
-
-
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -1404,15 +1359,15 @@
 
 
 PutChannelExpirationSettingsResponseTypeDef = TypedDict(
     "PutChannelExpirationSettingsResponseTypeDef",
     {
         "ChannelArn": str,
         "ExpirationSettings": ExpirationSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -1444,15 +1399,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1460,23 +1415,23 @@
     },
 )
 
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     {
         "StreamingConfigurations": List[StreamingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
     "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -1484,32 +1439,60 @@
     },
 )
 
 PutMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
     "PutMessagingStreamingConfigurationsResponseTypeDef",
     {
         "StreamingConfigurations": List[StreamingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProcessorConfigurationTypeDef = TypedDict(
     "ProcessorConfigurationTypeDef",
     {
         "Lambda": LambdaConfigurationTypeDef,
     },
 )
 
+_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_RequiredListChannelMessagesRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "ChimeBearer": str,
+    },
+)
+_OptionalListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_OptionalListChannelMessagesRequestRequestTypeDef",
+    {
+        "SortOrder": SortOrderType,
+        "NotBefore": TimestampTypeDef,
+        "NotAfter": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "SubChannelId": str,
+    },
+    total=False,
+)
+
+
+class ListChannelMessagesRequestRequestTypeDef(
+    _RequiredListChannelMessagesRequestRequestTypeDef,
+    _OptionalListChannelMessagesRequestRequestTypeDef,
+):
+    pass
+
+
 ListSubChannelsResponseTypeDef = TypedDict(
     "ListSubChannelsResponseTypeDef",
     {
         "ChannelArn": str,
         "SubChannels": List[SubChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchChannelsRequestRequestTypeDef",
     {
         "Fields": Sequence[SearchFieldTypeDef],
@@ -1533,113 +1516,113 @@
 
 
 BatchCreateChannelMembershipResponseTypeDef = TypedDict(
     "BatchCreateChannelMembershipResponseTypeDef",
     {
         "BatchChannelMemberships": BatchChannelMembershipsTypeDef,
         "Errors": List[BatchCreateChannelMembershipErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelBansResponseTypeDef = TypedDict(
     "ListChannelBansResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelBans": List[ChannelBanSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelBanResponseTypeDef = TypedDict(
     "DescribeChannelBanResponseTypeDef",
     {
         "ChannelBan": ChannelBanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelMembershipsResponseTypeDef = TypedDict(
     "ListChannelMembershipsResponseTypeDef",
     {
         "ChannelArn": str,
         "ChannelMemberships": List[ChannelMembershipSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelMembershipResponseTypeDef = TypedDict(
     "DescribeChannelMembershipResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelModeratorsResponseTypeDef = TypedDict(
     "ListChannelModeratorsResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelModerators": List[ChannelModeratorSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelModeratorResponseTypeDef = TypedDict(
     "DescribeChannelModeratorResponseTypeDef",
     {
         "ChannelModerator": ChannelModeratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelMembershipForAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipForAppInstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelMembershipsForAppInstanceUserResponseTypeDef = TypedDict(
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     {
         "ChannelMemberships": List[ChannelMembershipForAppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelModeratedByAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     {
         "Channel": ChannelModeratedByAppInstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsModeratedByAppInstanceUserResponseTypeDef = TypedDict(
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     {
         "Channels": List[ChannelModeratedByAppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelMembershipPreferencesResponseTypeDef = TypedDict(
     "GetChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "Preferences": ChannelMembershipPreferencesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
     "PutChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
@@ -1651,15 +1634,15 @@
 
 PutChannelMembershipPreferencesResponseTypeDef = TypedDict(
     "PutChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "Preferences": ChannelMembershipPreferencesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredChannelFlowCallbackRequestRequestTypeDef = TypedDict(
     "_RequiredChannelFlowCallbackRequestRequestTypeDef",
     {
         "CallbackId": str,
@@ -1679,38 +1662,70 @@
 class ChannelFlowCallbackRequestRequestTypeDef(
     _RequiredChannelFlowCallbackRequestRequestTypeDef,
     _OptionalChannelFlowCallbackRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_RequiredSendChannelMessageRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "Content": str,
+        "Type": ChannelMessageTypeType,
+        "Persistence": ChannelMessagePersistenceTypeType,
+        "ClientRequestToken": str,
+        "ChimeBearer": str,
+    },
+)
+_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_OptionalSendChannelMessageRequestRequestTypeDef",
+    {
+        "Metadata": str,
+        "PushNotification": PushNotificationConfigurationTypeDef,
+        "MessageAttributes": Mapping[str, MessageAttributeValueUnionTypeDef],
+        "SubChannelId": str,
+        "ContentType": str,
+        "Target": Sequence[TargetTypeDef],
+    },
+    total=False,
+)
+
+
+class SendChannelMessageRequestRequestTypeDef(
+    _RequiredSendChannelMessageRequestRequestTypeDef,
+    _OptionalSendChannelMessageRequestRequestTypeDef,
+):
+    pass
+
+
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
         "SubChannelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelMessageResponseTypeDef = TypedDict(
     "GetChannelMessageResponseTypeDef",
     {
         "ChannelMessage": ChannelMessageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProcessorTypeDef = TypedDict(
     "ProcessorTypeDef",
     {
         "Name": str,
@@ -1776,18 +1791,18 @@
 )
 
 ListChannelFlowsResponseTypeDef = TypedDict(
     "ListChannelFlowsResponseTypeDef",
     {
         "ChannelFlows": List[ChannelFlowSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelFlowResponseTypeDef = TypedDict(
     "DescribeChannelFlowResponseTypeDef",
     {
         "ChannelFlow": ChannelFlowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging/type_defs.pyi` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_chime_sdk_messaging.type_defs import AppInstanceUserMembershipSummaryTypeDef
 
-    data: AppInstanceUserMembershipSummaryTypeDef = {...}
+    data: AppInstanceUserMembershipSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -43,30 +43,29 @@
 
 __all__ = (
     "AppInstanceUserMembershipSummaryTypeDef",
     "AssociateChannelFlowRequestRequestTypeDef",
     "IdentityTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ChannelAssociatedWithFlowSummaryTypeDef",
-    "ChannelFlowCallbackResponseTypeDef",
     "ChannelSummaryTypeDef",
     "PushNotificationPreferencesTypeDef",
     "MessageAttributeValueTypeDef",
     "PushNotificationConfigurationTypeDef",
     "ChannelMessageStatusStructureTypeDef",
+    "MessageAttributeValueOutputTypeDef",
     "TargetTypeDef",
     "ElasticChannelConfigurationTypeDef",
     "ExpirationSettingsTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "TagTypeDef",
-    "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
-    "CreateChannelResponseTypeDef",
     "DeleteChannelBanRequestRequestTypeDef",
     "DeleteChannelFlowRequestRequestTypeDef",
     "DeleteChannelMembershipRequestRequestTypeDef",
     "DeleteChannelMessageRequestRequestTypeDef",
     "DeleteChannelModeratorRequestRequestTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteMessagingStreamingConfigurationsRequestRequestTypeDef",
@@ -74,79 +73,82 @@
     "DescribeChannelFlowRequestRequestTypeDef",
     "DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelMembershipRequestRequestTypeDef",
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelModeratorRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DisassociateChannelFlowRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     "GetChannelMessageRequestRequestTypeDef",
     "GetChannelMessageStatusRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetMessagingStreamingConfigurationsRequestRequestTypeDef",
     "StreamingConfigurationTypeDef",
     "LambdaConfigurationTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelFlowsRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
-    "ListChannelMessagesRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
     "ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListSubChannelsRequestRequestTypeDef",
     "SubChannelSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
-    "RedactChannelMessageResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchFieldTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateChannelFlowResponseTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
-    "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "UpdateChannelResponseTypeDef",
     "BatchChannelMembershipsTypeDef",
     "ChannelBanSummaryTypeDef",
     "ChannelBanTypeDef",
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
+    "ChannelFlowCallbackResponseTypeDef",
     "CreateChannelBanResponseTypeDef",
+    "CreateChannelFlowResponseTypeDef",
     "CreateChannelMembershipResponseTypeDef",
     "CreateChannelModeratorResponseTypeDef",
+    "CreateChannelResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "RedactChannelMessageResponseTypeDef",
+    "UpdateChannelFlowResponseTypeDef",
+    "UpdateChannelReadMarkerResponseTypeDef",
+    "UpdateChannelResponseTypeDef",
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     "ChannelModeratedByAppInstanceUserSummaryTypeDef",
     "ListChannelsResponseTypeDef",
     "SearchChannelsResponseTypeDef",
     "ChannelMembershipPreferencesTypeDef",
     "ChannelMessageCallbackTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
+    "MessageAttributeValueUnionTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
-    "SendChannelMessageRequestRequestTypeDef",
     "ChannelTypeDef",
     "PutChannelExpirationSettingsRequestRequestTypeDef",
     "PutChannelExpirationSettingsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "PutMessagingStreamingConfigurationsResponseTypeDef",
     "ProcessorConfigurationTypeDef",
+    "ListChannelMessagesRequestRequestTypeDef",
     "ListSubChannelsResponseTypeDef",
     "SearchChannelsRequestRequestTypeDef",
     "BatchCreateChannelMembershipResponseTypeDef",
     "ListChannelBansResponseTypeDef",
     "DescribeChannelBanResponseTypeDef",
     "ListChannelMembershipsResponseTypeDef",
     "DescribeChannelMembershipResponseTypeDef",
@@ -156,14 +158,15 @@
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "GetChannelMembershipPreferencesResponseTypeDef",
     "PutChannelMembershipPreferencesRequestRequestTypeDef",
     "PutChannelMembershipPreferencesResponseTypeDef",
     "ChannelFlowCallbackRequestRequestTypeDef",
+    "SendChannelMessageRequestRequestTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "ProcessorTypeDef",
     "ChannelFlowSummaryTypeDef",
     "ChannelFlowTypeDef",
     "CreateChannelFlowRequestRequestTypeDef",
@@ -229,35 +232,37 @@
 
 class BatchCreateChannelMembershipRequestRequestTypeDef(
     _RequiredBatchCreateChannelMembershipRequestRequestTypeDef,
     _OptionalBatchCreateChannelMembershipRequestRequestTypeDef,
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
 ChannelAssociatedWithFlowSummaryTypeDef = TypedDict(
     "ChannelAssociatedWithFlowSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
     },
     total=False,
 )
 
-ChannelFlowCallbackResponseTypeDef = TypedDict(
-    "ChannelFlowCallbackResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "CallbackId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ChannelSummaryTypeDef = TypedDict(
     "ChannelSummaryTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -309,14 +314,22 @@
     {
         "Value": ChannelMessageStatusType,
         "Detail": str,
     },
     total=False,
 )
 
+MessageAttributeValueOutputTypeDef = TypedDict(
+    "MessageAttributeValueOutputTypeDef",
+    {
+        "StringValues": List[str],
+    },
+    total=False,
+)
+
 TargetTypeDef = TypedDict(
     "TargetTypeDef",
     {
         "MemberArn": str,
     },
     total=False,
 )
@@ -351,22 +364,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateChannelFlowResponseTypeDef = TypedDict(
-    "CreateChannelFlowResponseTypeDef",
-    {
-        "ChannelFlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateChannelMembershipRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelMembershipRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "Type": ChannelMembershipTypeType,
         "ChimeBearer": str,
@@ -391,22 +396,14 @@
     {
         "ChannelArn": str,
         "ChannelModeratorArn": str,
         "ChimeBearer": str,
     },
 )
 
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteChannelBanRequestRequestTypeDef = TypedDict(
     "DeleteChannelBanRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -565,21 +562,14 @@
     {
         "ChannelArn": str,
         "ChannelFlowArn": str,
         "ChimeBearer": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
     "GetChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -742,40 +732,15 @@
 
 class ListChannelMembershipsRequestRequestTypeDef(
     _RequiredListChannelMembershipsRequestRequestTypeDef,
     _OptionalListChannelMembershipsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
-    "_RequiredListChannelMessagesRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "ChimeBearer": str,
-    },
-)
-_OptionalListChannelMessagesRequestRequestTypeDef = TypedDict(
-    "_OptionalListChannelMessagesRequestRequestTypeDef",
-    {
-        "SortOrder": SortOrderType,
-        "NotBefore": Union[datetime, str],
-        "NotAfter": Union[datetime, str],
-        "MaxResults": int,
-        "NextToken": str,
-        "SubChannelId": str,
-    },
-    total=False,
-)
-
-class ListChannelMessagesRequestRequestTypeDef(
-    _RequiredListChannelMessagesRequestRequestTypeDef,
-    _OptionalListChannelMessagesRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListChannelModeratorsRequestRequestTypeDef = TypedDict(
     "_RequiredListChannelModeratorsRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -914,35 +879,14 @@
 
 class RedactChannelMessageRequestRequestTypeDef(
     _RequiredRedactChannelMessageRequestRequestTypeDef,
     _OptionalRedactChannelMessageRequestRequestTypeDef,
 ):
     pass
 
-RedactChannelMessageResponseTypeDef = TypedDict(
-    "RedactChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "SubChannelId": str,
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
 SearchFieldTypeDef = TypedDict(
     "SearchFieldTypeDef",
     {
         "Key": Literal["MEMBERS"],
         "Values": Sequence[str],
         "Operator": SearchFieldOperatorType,
     },
@@ -952,22 +896,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateChannelFlowResponseTypeDef = TypedDict(
-    "UpdateChannelFlowResponseTypeDef",
-    {
-        "ChannelFlowArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Content": str,
         "ChimeBearer": str,
@@ -993,22 +929,14 @@
     "UpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
 
-UpdateChannelReadMarkerResponseTypeDef = TypedDict(
-    "UpdateChannelReadMarkerResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "ChimeBearer": str,
     },
 )
@@ -1023,22 +951,14 @@
 )
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-UpdateChannelResponseTypeDef = TypedDict(
-    "UpdateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchChannelMembershipsTypeDef = TypedDict(
     "BatchChannelMembershipsTypeDef",
     {
         "InvitedBy": IdentityTypeDef,
         "Type": ChannelMembershipTypeType,
         "Members": List[IdentityTypeDef],
         "ChannelArn": str,
@@ -1103,48 +1023,114 @@
         "ChannelArn": str,
         "CreatedTimestamp": datetime,
         "CreatedBy": IdentityTypeDef,
     },
     total=False,
 )
 
+ChannelFlowCallbackResponseTypeDef = TypedDict(
+    "ChannelFlowCallbackResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "CallbackId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateChannelBanResponseTypeDef = TypedDict(
     "CreateChannelBanResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChannelFlowResponseTypeDef = TypedDict(
+    "CreateChannelFlowResponseTypeDef",
+    {
+        "ChannelFlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelMembershipResponseTypeDef = TypedDict(
     "CreateChannelMembershipResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "SubChannelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelModeratorResponseTypeDef = TypedDict(
     "CreateChannelModeratorResponseTypeDef",
     {
         "ChannelArn": str,
         "ChannelModerator": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
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
+RedactChannelMessageResponseTypeDef = TypedDict(
+    "RedactChannelMessageResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "MessageId": str,
+        "SubChannelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChannelFlowResponseTypeDef = TypedDict(
+    "UpdateChannelFlowResponseTypeDef",
+    {
+        "ChannelFlowArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChannelReadMarkerResponseTypeDef = TypedDict(
+    "UpdateChannelReadMarkerResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChannelResponseTypeDef = TypedDict(
+    "UpdateChannelResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsAssociatedWithChannelFlowResponseTypeDef = TypedDict(
     "ListChannelsAssociatedWithChannelFlowResponseTypeDef",
     {
         "Channels": List[ChannelAssociatedWithFlowSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChannelMembershipForAppInstanceUserSummaryTypeDef = TypedDict(
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     {
         "ChannelSummary": ChannelSummaryTypeDef,
@@ -1162,24 +1148,24 @@
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchChannelsResponseTypeDef = TypedDict(
     "SearchChannelsResponseTypeDef",
     {
         "Channels": List[ChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChannelMembershipPreferencesTypeDef = TypedDict(
     "ChannelMembershipPreferencesTypeDef",
     {
         "PushNotifications": PushNotificationPreferencesTypeDef,
@@ -1211,54 +1197,57 @@
 ):
     pass
 
 GetChannelMessageStatusResponseTypeDef = TypedDict(
     "GetChannelMessageStatusResponseTypeDef",
     {
         "Status": ChannelMessageStatusStructureTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendChannelMessageResponseTypeDef = TypedDict(
     "SendChannelMessageResponseTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateChannelMessageResponseTypeDef = TypedDict(
     "UpdateChannelMessageResponseTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
         "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+MessageAttributeValueUnionTypeDef = Union[
+    MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef
+]
 ChannelMessageSummaryTypeDef = TypedDict(
     "ChannelMessageSummaryTypeDef",
     {
         "MessageId": str,
         "Content": str,
         "Metadata": str,
         "Type": ChannelMessageTypeType,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Status": ChannelMessageStatusStructureTypeDef,
-        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
         "ContentType": str,
         "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
 ChannelMessageTypeDef = TypedDict(
@@ -1272,52 +1261,22 @@
         "CreatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Persistence": ChannelMessagePersistenceTypeType,
         "Status": ChannelMessageStatusStructureTypeDef,
-        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
         "SubChannelId": str,
         "ContentType": str,
         "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
-_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_RequiredSendChannelMessageRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "Content": str,
-        "Type": ChannelMessageTypeType,
-        "Persistence": ChannelMessagePersistenceTypeType,
-        "ClientRequestToken": str,
-        "ChimeBearer": str,
-    },
-)
-_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_OptionalSendChannelMessageRequestRequestTypeDef",
-    {
-        "Metadata": str,
-        "PushNotification": PushNotificationConfigurationTypeDef,
-        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
-        "SubChannelId": str,
-        "ContentType": str,
-        "Target": Sequence[TargetTypeDef],
-    },
-    total=False,
-)
-
-class SendChannelMessageRequestRequestTypeDef(
-    _RequiredSendChannelMessageRequestRequestTypeDef,
-    _OptionalSendChannelMessageRequestRequestTypeDef,
-):
-    pass
-
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -1355,15 +1314,15 @@
     pass
 
 PutChannelExpirationSettingsResponseTypeDef = TypedDict(
     "PutChannelExpirationSettingsResponseTypeDef",
     {
         "ChannelArn": str,
         "ExpirationSettings": ExpirationSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -1393,15 +1352,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1409,23 +1368,23 @@
     },
 )
 
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     {
         "StreamingConfigurations": List[StreamingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutMessagingStreamingConfigurationsRequestRequestTypeDef = TypedDict(
     "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -1433,32 +1392,58 @@
     },
 )
 
 PutMessagingStreamingConfigurationsResponseTypeDef = TypedDict(
     "PutMessagingStreamingConfigurationsResponseTypeDef",
     {
         "StreamingConfigurations": List[StreamingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProcessorConfigurationTypeDef = TypedDict(
     "ProcessorConfigurationTypeDef",
     {
         "Lambda": LambdaConfigurationTypeDef,
     },
 )
 
+_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_RequiredListChannelMessagesRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "ChimeBearer": str,
+    },
+)
+_OptionalListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_OptionalListChannelMessagesRequestRequestTypeDef",
+    {
+        "SortOrder": SortOrderType,
+        "NotBefore": TimestampTypeDef,
+        "NotAfter": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "SubChannelId": str,
+    },
+    total=False,
+)
+
+class ListChannelMessagesRequestRequestTypeDef(
+    _RequiredListChannelMessagesRequestRequestTypeDef,
+    _OptionalListChannelMessagesRequestRequestTypeDef,
+):
+    pass
+
 ListSubChannelsResponseTypeDef = TypedDict(
     "ListSubChannelsResponseTypeDef",
     {
         "ChannelArn": str,
         "SubChannels": List[SubChannelSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchChannelsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchChannelsRequestRequestTypeDef",
     {
         "Fields": Sequence[SearchFieldTypeDef],
@@ -1480,113 +1465,113 @@
     pass
 
 BatchCreateChannelMembershipResponseTypeDef = TypedDict(
     "BatchCreateChannelMembershipResponseTypeDef",
     {
         "BatchChannelMemberships": BatchChannelMembershipsTypeDef,
         "Errors": List[BatchCreateChannelMembershipErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelBansResponseTypeDef = TypedDict(
     "ListChannelBansResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelBans": List[ChannelBanSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelBanResponseTypeDef = TypedDict(
     "DescribeChannelBanResponseTypeDef",
     {
         "ChannelBan": ChannelBanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelMembershipsResponseTypeDef = TypedDict(
     "ListChannelMembershipsResponseTypeDef",
     {
         "ChannelArn": str,
         "ChannelMemberships": List[ChannelMembershipSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelMembershipResponseTypeDef = TypedDict(
     "DescribeChannelMembershipResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelModeratorsResponseTypeDef = TypedDict(
     "ListChannelModeratorsResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelModerators": List[ChannelModeratorSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelModeratorResponseTypeDef = TypedDict(
     "DescribeChannelModeratorResponseTypeDef",
     {
         "ChannelModerator": ChannelModeratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelMembershipForAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelMembershipForAppInstanceUserResponseTypeDef",
     {
         "ChannelMembership": ChannelMembershipForAppInstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelMembershipsForAppInstanceUserResponseTypeDef = TypedDict(
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     {
         "ChannelMemberships": List[ChannelMembershipForAppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelModeratedByAppInstanceUserResponseTypeDef = TypedDict(
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     {
         "Channel": ChannelModeratedByAppInstanceUserSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsModeratedByAppInstanceUserResponseTypeDef = TypedDict(
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     {
         "Channels": List[ChannelModeratedByAppInstanceUserSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelMembershipPreferencesResponseTypeDef = TypedDict(
     "GetChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "Preferences": ChannelMembershipPreferencesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutChannelMembershipPreferencesRequestRequestTypeDef = TypedDict(
     "PutChannelMembershipPreferencesRequestRequestTypeDef",
     {
         "ChannelArn": str,
@@ -1598,15 +1583,15 @@
 
 PutChannelMembershipPreferencesResponseTypeDef = TypedDict(
     "PutChannelMembershipPreferencesResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
         "Preferences": ChannelMembershipPreferencesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredChannelFlowCallbackRequestRequestTypeDef = TypedDict(
     "_RequiredChannelFlowCallbackRequestRequestTypeDef",
     {
         "CallbackId": str,
@@ -1624,38 +1609,68 @@
 
 class ChannelFlowCallbackRequestRequestTypeDef(
     _RequiredChannelFlowCallbackRequestRequestTypeDef,
     _OptionalChannelFlowCallbackRequestRequestTypeDef,
 ):
     pass
 
+_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_RequiredSendChannelMessageRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "Content": str,
+        "Type": ChannelMessageTypeType,
+        "Persistence": ChannelMessagePersistenceTypeType,
+        "ClientRequestToken": str,
+        "ChimeBearer": str,
+    },
+)
+_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_OptionalSendChannelMessageRequestRequestTypeDef",
+    {
+        "Metadata": str,
+        "PushNotification": PushNotificationConfigurationTypeDef,
+        "MessageAttributes": Mapping[str, MessageAttributeValueUnionTypeDef],
+        "SubChannelId": str,
+        "ContentType": str,
+        "Target": Sequence[TargetTypeDef],
+    },
+    total=False,
+)
+
+class SendChannelMessageRequestRequestTypeDef(
+    _RequiredSendChannelMessageRequestRequestTypeDef,
+    _OptionalSendChannelMessageRequestRequestTypeDef,
+):
+    pass
+
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
         "SubChannelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChannelMessageResponseTypeDef = TypedDict(
     "GetChannelMessageResponseTypeDef",
     {
         "ChannelMessage": ChannelMessageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProcessorTypeDef = TypedDict(
     "ProcessorTypeDef",
     {
         "Name": str,
@@ -1719,18 +1734,18 @@
 )
 
 ListChannelFlowsResponseTypeDef = TypedDict(
     "ListChannelFlowsResponseTypeDef",
     {
         "ChannelFlows": List[ChannelFlowSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChannelFlowResponseTypeDef = TypedDict(
     "DescribeChannelFlowResponseTypeDef",
     {
         "ChannelFlow": ChannelFlowTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-messaging
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore chime-sdk-messaging type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore chime-sdk-messaging type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime-sdk-messaging"></a>
 
 # types-aiobotocore-chime-sdk-messaging
 
 [![PyPI - types-aiobotocore-chime-sdk-messaging](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime-sdk-messaging?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime-sdk-messaging)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-messaging)](https://pepy.tech/project/types-aiobotocore-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ChimeSDKMessaging 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
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
 [types-aiobotocore-chime-sdk-messaging docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging/).
 
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
@@ -296,44 +295,44 @@
 )
 
 
 def check_value(value: AllowNotificationsType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime_sdk_messaging.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_chime_sdk_messaging.type_defs import (
     AppInstanceUserMembershipSummaryTypeDef,
     AssociateChannelFlowRequestRequestTypeDef,
     IdentityTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ChannelAssociatedWithFlowSummaryTypeDef,
-    ChannelFlowCallbackResponseTypeDef,
     ChannelSummaryTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
+    MessageAttributeValueOutputTypeDef,
     TargetTypeDef,
     ElasticChannelConfigurationTypeDef,
     ExpirationSettingsTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
-    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
-    CreateChannelResponseTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
     DeleteChannelMessageRequestRequestTypeDef,
     DeleteChannelModeratorRequestRequestTypeDef,
     DeleteChannelRequestRequestTypeDef,
     DeleteMessagingStreamingConfigurationsRequestRequestTypeDef,
@@ -341,79 +340,82 @@
     DescribeChannelFlowRequestRequestTypeDef,
     DescribeChannelMembershipForAppInstanceUserRequestRequestTypeDef,
     DescribeChannelMembershipRequestRequestTypeDef,
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociateChannelFlowRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetChannelMembershipPreferencesRequestRequestTypeDef,
     GetChannelMessageRequestRequestTypeDef,
     GetChannelMessageStatusRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetMessagingStreamingConfigurationsRequestRequestTypeDef,
     StreamingConfigurationTypeDef,
     LambdaConfigurationTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelFlowsRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
-    ListChannelMessagesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsAssociatedWithChannelFlowRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListSubChannelsRequestRequestTypeDef,
     SubChannelSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
-    RedactChannelMessageResponseTypeDef,
-    ResponseMetadataTypeDef,
     SearchFieldTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateChannelFlowResponseTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    UpdateChannelResponseTypeDef,
     BatchChannelMembershipsTypeDef,
     ChannelBanSummaryTypeDef,
     ChannelBanTypeDef,
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
+    ChannelFlowCallbackResponseTypeDef,
     CreateChannelBanResponseTypeDef,
+    CreateChannelFlowResponseTypeDef,
     CreateChannelMembershipResponseTypeDef,
     CreateChannelModeratorResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    UpdateChannelFlowResponseTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ChannelMembershipForAppInstanceUserSummaryTypeDef,
     ChannelModeratedByAppInstanceUserSummaryTypeDef,
     ListChannelsResponseTypeDef,
     SearchChannelsResponseTypeDef,
     ChannelMembershipPreferencesTypeDef,
     ChannelMessageCallbackTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
+    MessageAttributeValueUnionTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
-    SendChannelMessageRequestRequestTypeDef,
     ChannelTypeDef,
     PutChannelExpirationSettingsRequestRequestTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
     PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     ProcessorConfigurationTypeDef,
+    ListChannelMessagesRequestRequestTypeDef,
     ListSubChannelsResponseTypeDef,
     SearchChannelsRequestRequestTypeDef,
     BatchCreateChannelMembershipResponseTypeDef,
     ListChannelBansResponseTypeDef,
     DescribeChannelBanResponseTypeDef,
     ListChannelMembershipsResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
@@ -423,28 +425,29 @@
     ListChannelMembershipsForAppInstanceUserResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
     PutChannelMembershipPreferencesRequestRequestTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     ChannelFlowCallbackRequestRequestTypeDef,
+    SendChannelMessageRequestRequestTypeDef,
     ListChannelMessagesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ProcessorTypeDef,
     ChannelFlowSummaryTypeDef,
     ChannelFlowTypeDef,
     CreateChannelFlowRequestRequestTypeDef,
     UpdateChannelFlowRequestRequestTypeDef,
     ListChannelFlowsResponseTypeDef,
     DescribeChannelFlowResponseTypeDef,
 )
 
 
-def get_structure() -> AppInstanceUserMembershipSummaryTypeDef:
+def get_value() -> AppInstanceUserMembershipSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*


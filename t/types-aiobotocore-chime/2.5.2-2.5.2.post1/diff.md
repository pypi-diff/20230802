# Comparing `tmp/types-aiobotocore-chime-2.5.2.tar.gz` & `tmp/types-aiobotocore-chime-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-2.5.2.tar", last modified: Sat Jul  8 01:43:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
```

## Comparing `types-aiobotocore-chime-2.5.2.tar` & `types-aiobotocore-chime-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.161780 types-aiobotocore-chime-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:32.000000 types-aiobotocore-chime-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32880 2023-07-08 01:43:19.153780 types-aiobotocore-chime-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31323 2023-07-08 01:26:32.000000 types-aiobotocore-chime-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:19.161780 types-aiobotocore-chime-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-08 01:26:32.000000 types-aiobotocore-chime-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.149780 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-08 01:26:32.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-08 01:26:32.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-08 01:26:32.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   127528 2023-07-08 01:26:33.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   127326 2023-07-08 01:26:33.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-07-08 01:26:33.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-08 01:26:33.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-08 01:26:33.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-08 01:26:33.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:32.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   144748 2023-07-08 01:26:37.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   144589 2023-07-08 01:26:35.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:32.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.153780 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32880 2023-07-08 01:43:18.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-08 01:43:19.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:18.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 01:43:18.000000 types-aiobotocore-chime-2.5.2/types_aiobotocore_chime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.553643 types-aiobotocore-chime-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    33302 2023-08-02 14:51:57.549643 types-aiobotocore-chime-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31792 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.553643 types-aiobotocore-chime-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.545642 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127555 2023-08-02 14:34:01.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127353 2023-08-02 14:34:01.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-08-02 14:34:01.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-08-02 14:34:01.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-02 14:34:01.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-08-02 14:34:01.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   147475 2023-08-02 14:34:05.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147314 2023-08-02 14:34:03.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.549643 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33302 2023-08-02 14:51:57.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 14:51:57.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:51:57.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-2.5.2/LICENSE` & `types-aiobotocore-chime-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2/PKG-INFO` & `types-aiobotocore-chime-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Chime 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Chime 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore chime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore chime type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime"></a>
 
 # types-aiobotocore-chime
 
 [![PyPI - types-aiobotocore-chime](https://img.shields.io/pypi/v/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime)](https://pepy.tech/project/types-aiobotocore-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Chime 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [types-aiobotocore-chime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/).
 
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
@@ -355,20 +354,20 @@
 )
 
 
 def check_value(value: AccountStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_chime.type_defs import (
     AccountSettingsTypeDef,
     SigninDelegateGroupTypeDef,
     AddressTypeDef,
     AlexaForBusinessMetadataTypeDef,
@@ -382,14 +381,15 @@
     AppInstanceUserTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     AssociatePhoneNumberWithUserRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
+    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeErrorTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     MembershipItemTypeDef,
     MemberErrorTypeDef,
@@ -402,23 +402,19 @@
     BusinessCallingSettingsTypeDef,
     CandidateAddressTypeDef,
     ChannelSummaryTypeDef,
     ConversationRetentionSettingsTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     TagTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
     CreateBotRequestRequestTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
-    CreateChannelResponseTypeDef,
     CreateMeetingDialOutRequestRequestTypeDef,
-    CreateMeetingDialOutResponseTypeDef,
     MeetingNotificationConfigurationTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateRoomMembershipRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     RoomTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
@@ -468,15 +464,14 @@
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociatePhoneNumberFromUserRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     EventsConfigurationTypeDef,
     GetAccountRequestRequestTypeDef,
     GetAccountSettingsRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     GetAppInstanceStreamingConfigurationsRequestRequestTypeDef,
@@ -486,15 +481,14 @@
     GetEventsConfigurationRequestRequestTypeDef,
     VoiceConnectorSettingsTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetRetentionSettingsRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
@@ -508,29 +502,29 @@
     GetVoiceConnectorProxyRequestRequestTypeDef,
     ProxyTypeDef,
     GetVoiceConnectorRequestRequestTypeDef,
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
-    TerminationTypeDef,
+    TerminationOutputTypeDef,
     InviteTypeDef,
     InviteUsersRequestRequestTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
-    ListChannelMessagesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     ListMeetingTagsRequestRequestTypeDef,
     ListMeetingsRequestRequestTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
@@ -539,72 +533,61 @@
     ListRoomMembershipsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     LogoutUserRequestRequestTypeDef,
     MediaPlacementTypeDef,
     MemberTypeDef,
     OrderedPhoneNumberTypeDef,
     OriginationRouteTypeDef,
-    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutEventsConfigurationRequestRequestTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
+    TerminationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
-    RedactChannelMessageResponseTypeDef,
     RedactConversationMessageRequestRequestTypeDef,
     RedactRoomMessageRequestRequestTypeDef,
     RegenerateSecurityTokenRequestRequestTypeDef,
     ResetPersonalPINRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     RoomRetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
+    SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     SendChannelMessageRequestRequestTypeDef,
-    SendChannelMessageResponseTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     StreamingNotificationTargetTypeDef,
     TelephonySettingsTypeDef,
     UntagAttendeeRequestRequestTypeDef,
     UntagMeetingRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
-    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
     UpdateBotRequestRequestTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
-    UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    UpdateChannelResponseTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateRoomMembershipRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
-    GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsRequestRequestTypeDef,
     AccountTypeDef,
     AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
     UpdateUserRequestItemTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserTypeDef,
     AppInstanceAdminSummaryTypeDef,
@@ -615,33 +598,49 @@
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
     ChannelTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateChannelBanResponseTypeDef,
-    CreateChannelMembershipResponseTypeDef,
-    CreateChannelModeratorResponseTypeDef,
     AppInstanceRetentionSettingsTypeDef,
-    GetAppInstanceStreamingConfigurationsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
-    PutAppInstanceStreamingConfigurationsResponseTypeDef,
-    ListAppInstancesResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    DescribeAppInstanceUserResponseTypeDef,
     ArtifactsConfigurationTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
+    CreateChannelBanResponseTypeDef,
+    CreateChannelMembershipResponseTypeDef,
+    CreateChannelModeratorResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    CreateMeetingDialOutResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
+    DescribeAppInstanceUserResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccountSettingsResponseTypeDef,
+    GetAppInstanceStreamingConfigurationsResponseTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
+    ListAppInstancesResponseTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
+    PutAppInstanceStreamingConfigurationsResponseTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
+    SendChannelMessageResponseTypeDef,
+    UpdateAppInstanceResponseTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
+    UpdateChannelMessageResponseTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     BatchCreateRoomMembershipRequestRequestTypeDef,
     BatchCreateRoomMembershipResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
@@ -686,14 +685,15 @@
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
     VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     TranscriptionConfigurationTypeDef,
     GetEventsConfigurationResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     GetGlobalSettingsResponseTypeDef,
     UpdateGlobalSettingsRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
@@ -703,26 +703,33 @@
     GetVoiceConnectorLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
-    PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     InviteUsersResponseTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListChannelMessagesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
+    PutVoiceConnectorTerminationRequestRequestTypeDef,
+    TerminationUnionTypeDef,
     RetentionSettingsTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
     UserSettingsTypeDef,
     CreateAccountResponseTypeDef,
     GetAccountResponseTypeDef,
     ListAccountsResponseTypeDef,
     UpdateAccountResponseTypeDef,
     BatchUpdateUserRequestRequestTypeDef,
@@ -761,56 +768,61 @@
     ListSipRulesResponseTypeDef,
     UpdateSipRuleResponseTypeDef,
     CreateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorGroupResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
-    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
+    EmergencyCallingConfigurationUnionTypeDef,
+    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
     ListMeetingsResponseTypeDef,
     CreateRoomMembershipResponseTypeDef,
     ListRoomMembershipsResponseTypeDef,
     UpdateRoomMembershipResponseTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
-    PutVoiceConnectorOriginationRequestRequestTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
+    OriginationUnionTypeDef,
+    PutVoiceConnectorOriginationRequestRequestTypeDef,
     CreateProxySessionResponseTypeDef,
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     GetRetentionSettingsResponseTypeDef,
     PutRetentionSettingsRequestRequestTypeDef,
     PutRetentionSettingsResponseTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
-    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
+    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
+    StreamingConfigurationUnionTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
-    CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaCapturePipelineTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
+    CreateMediaCapturePipelineRequestRequestTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-2.5.2/README.md` & `types-aiobotocore-chime-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-chime"></a>
 
 # types-aiobotocore-chime
 
 [![PyPI - types-aiobotocore-chime](https://img.shields.io/pypi/v/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime)](https://pepy.tech/project/types-aiobotocore-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Chime 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [types-aiobotocore-chime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/).
 
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
@@ -322,20 +322,20 @@
 )
 
 
 def check_value(value: AccountStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_chime.type_defs import (
     AccountSettingsTypeDef,
     SigninDelegateGroupTypeDef,
     AddressTypeDef,
     AlexaForBusinessMetadataTypeDef,
@@ -349,14 +349,15 @@
     AppInstanceUserTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     AssociatePhoneNumberWithUserRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
+    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeErrorTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     MembershipItemTypeDef,
     MemberErrorTypeDef,
@@ -369,23 +370,19 @@
     BusinessCallingSettingsTypeDef,
     CandidateAddressTypeDef,
     ChannelSummaryTypeDef,
     ConversationRetentionSettingsTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     TagTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
     CreateBotRequestRequestTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
-    CreateChannelResponseTypeDef,
     CreateMeetingDialOutRequestRequestTypeDef,
-    CreateMeetingDialOutResponseTypeDef,
     MeetingNotificationConfigurationTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateRoomMembershipRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     RoomTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
@@ -435,15 +432,14 @@
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociatePhoneNumberFromUserRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     EventsConfigurationTypeDef,
     GetAccountRequestRequestTypeDef,
     GetAccountSettingsRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     GetAppInstanceStreamingConfigurationsRequestRequestTypeDef,
@@ -453,15 +449,14 @@
     GetEventsConfigurationRequestRequestTypeDef,
     VoiceConnectorSettingsTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetRetentionSettingsRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
@@ -475,29 +470,29 @@
     GetVoiceConnectorProxyRequestRequestTypeDef,
     ProxyTypeDef,
     GetVoiceConnectorRequestRequestTypeDef,
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
-    TerminationTypeDef,
+    TerminationOutputTypeDef,
     InviteTypeDef,
     InviteUsersRequestRequestTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
-    ListChannelMessagesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     ListMeetingTagsRequestRequestTypeDef,
     ListMeetingsRequestRequestTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
@@ -506,72 +501,61 @@
     ListRoomMembershipsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     LogoutUserRequestRequestTypeDef,
     MediaPlacementTypeDef,
     MemberTypeDef,
     OrderedPhoneNumberTypeDef,
     OriginationRouteTypeDef,
-    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutEventsConfigurationRequestRequestTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
+    TerminationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
-    RedactChannelMessageResponseTypeDef,
     RedactConversationMessageRequestRequestTypeDef,
     RedactRoomMessageRequestRequestTypeDef,
     RegenerateSecurityTokenRequestRequestTypeDef,
     ResetPersonalPINRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     RoomRetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
+    SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     SendChannelMessageRequestRequestTypeDef,
-    SendChannelMessageResponseTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     StreamingNotificationTargetTypeDef,
     TelephonySettingsTypeDef,
     UntagAttendeeRequestRequestTypeDef,
     UntagMeetingRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
-    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
     UpdateBotRequestRequestTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
-    UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    UpdateChannelResponseTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateRoomMembershipRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
-    GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsRequestRequestTypeDef,
     AccountTypeDef,
     AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
     UpdateUserRequestItemTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserTypeDef,
     AppInstanceAdminSummaryTypeDef,
@@ -582,33 +566,49 @@
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
     ChannelTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateChannelBanResponseTypeDef,
-    CreateChannelMembershipResponseTypeDef,
-    CreateChannelModeratorResponseTypeDef,
     AppInstanceRetentionSettingsTypeDef,
-    GetAppInstanceStreamingConfigurationsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
-    PutAppInstanceStreamingConfigurationsResponseTypeDef,
-    ListAppInstancesResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    DescribeAppInstanceUserResponseTypeDef,
     ArtifactsConfigurationTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
+    CreateChannelBanResponseTypeDef,
+    CreateChannelMembershipResponseTypeDef,
+    CreateChannelModeratorResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    CreateMeetingDialOutResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
+    DescribeAppInstanceUserResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccountSettingsResponseTypeDef,
+    GetAppInstanceStreamingConfigurationsResponseTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
+    ListAppInstancesResponseTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
+    PutAppInstanceStreamingConfigurationsResponseTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
+    SendChannelMessageResponseTypeDef,
+    UpdateAppInstanceResponseTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
+    UpdateChannelMessageResponseTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     BatchCreateRoomMembershipRequestRequestTypeDef,
     BatchCreateRoomMembershipResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
@@ -653,14 +653,15 @@
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
     VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     TranscriptionConfigurationTypeDef,
     GetEventsConfigurationResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     GetGlobalSettingsResponseTypeDef,
     UpdateGlobalSettingsRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
@@ -670,26 +671,33 @@
     GetVoiceConnectorLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
-    PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     InviteUsersResponseTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListChannelMessagesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
+    PutVoiceConnectorTerminationRequestRequestTypeDef,
+    TerminationUnionTypeDef,
     RetentionSettingsTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
     UserSettingsTypeDef,
     CreateAccountResponseTypeDef,
     GetAccountResponseTypeDef,
     ListAccountsResponseTypeDef,
     UpdateAccountResponseTypeDef,
     BatchUpdateUserRequestRequestTypeDef,
@@ -728,56 +736,61 @@
     ListSipRulesResponseTypeDef,
     UpdateSipRuleResponseTypeDef,
     CreateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorGroupResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
-    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
+    EmergencyCallingConfigurationUnionTypeDef,
+    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
     ListMeetingsResponseTypeDef,
     CreateRoomMembershipResponseTypeDef,
     ListRoomMembershipsResponseTypeDef,
     UpdateRoomMembershipResponseTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
-    PutVoiceConnectorOriginationRequestRequestTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
+    OriginationUnionTypeDef,
+    PutVoiceConnectorOriginationRequestRequestTypeDef,
     CreateProxySessionResponseTypeDef,
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     GetRetentionSettingsResponseTypeDef,
     PutRetentionSettingsRequestRequestTypeDef,
     PutRetentionSettingsResponseTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
-    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
+    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
+    StreamingConfigurationUnionTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
-    CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaCapturePipelineTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
+    CreateMediaCapturePipelineRequestRequestTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-2.5.2/setup.py` & `types-aiobotocore-chime-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_chime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Chime 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore chime type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore chime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_chime": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/"
```

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/__init__.py` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/__init__.pyi` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/__main__.py` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Chime 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Chime 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime\nOther"
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

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/client.py` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("chime") as client:
         client: ChimeClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     CapabilityType,
     ChannelMembershipTypeType,
@@ -55,15 +54,15 @@
     BatchCreateRoomMembershipResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
     BatchUnsuspendUserResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     BatchUpdateUserResponseTypeDef,
     BusinessCallingSettingsTypeDef,
-    ChimeSdkMeetingConfigurationTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     CreateAccountResponseTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeResponseTypeDef,
     CreateBotResponseTypeDef,
@@ -93,15 +92,15 @@
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmergencyCallingConfigurationTypeDef,
+    EmergencyCallingConfigurationUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetAccountResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     GetAppInstanceStreamingConfigurationsResponseTypeDef,
     GetAttendeeResponseTypeDef,
@@ -162,15 +161,15 @@
     ListUsersResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     LoggingConfigurationTypeDef,
     MeetingNotificationConfigurationTypeDef,
     MembershipItemTypeDef,
-    OriginationTypeDef,
+    OriginationUnionTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     PutRetentionSettingsResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
@@ -185,17 +184,18 @@
     RetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     SigninDelegateGroupTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
-    StreamingConfigurationTypeDef,
+    StreamingConfigurationUnionTypeDef,
     TagTypeDef,
-    TerminationTypeDef,
+    TerminationUnionTypeDef,
+    TimestampTypeDef,
     TranscriptionConfigurationTypeDef,
     UpdateAccountResponseTypeDef,
     UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserResponseTypeDef,
     UpdateBotResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
@@ -543,15 +543,15 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media capture pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_media_capture_pipeline)
         """
@@ -1604,16 +1604,16 @@
         """
 
     async def list_channel_messages(
         self,
         *,
         ChannelArn: str,
         SortOrder: SortOrderType = ...,
-        NotBefore: Union[datetime, str] = ...,
-        NotAfter: Union[datetime, str] = ...,
+        NotBefore: TimestampTypeDef = ...,
+        NotAfter: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         ChimeBearer: str = ...
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
@@ -1920,15 +1920,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_sip_media_application_logging_configuration)
         """
 
     async def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
-        EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef
+        EmergencyCallingConfiguration: EmergencyCallingConfigurationUnionTypeDef
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
         Puts emergency calling configuration details to the specified Amazon Chime Voice
         Connector, such as emergency phone numbers and calling countries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_emergency_calling_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_emergency_calling_configuration)
@@ -1941,15 +1941,15 @@
         Adds a logging configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_logging_configuration)
         """
 
     async def put_voice_connector_origination(
-        self, *, VoiceConnectorId: str, Origination: OriginationTypeDef
+        self, *, VoiceConnectorId: str, Origination: OriginationUnionTypeDef
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
         Adds origination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_origination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_origination)
         """
@@ -1968,25 +1968,25 @@
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_proxy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_proxy)
         """
 
     async def put_voice_connector_streaming_configuration(
-        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationTypeDef
+        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationUnionTypeDef
     ) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
         Adds a streaming configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_streaming_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_streaming_configuration)
         """
 
     async def put_voice_connector_termination(
-        self, *, VoiceConnectorId: str, Termination: TerminationTypeDef
+        self, *, VoiceConnectorId: str, Termination: TerminationUnionTypeDef
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
         Adds termination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_termination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_termination)
         """
```

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/client.pyi` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("chime") as client:
         client: ChimeClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     CapabilityType,
     ChannelMembershipTypeType,
@@ -55,15 +54,15 @@
     BatchCreateRoomMembershipResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
     BatchUnsuspendUserResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     BatchUpdateUserResponseTypeDef,
     BusinessCallingSettingsTypeDef,
-    ChimeSdkMeetingConfigurationTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
     CreateAccountResponseTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeResponseTypeDef,
     CreateBotResponseTypeDef,
@@ -93,15 +92,15 @@
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmergencyCallingConfigurationTypeDef,
+    EmergencyCallingConfigurationUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetAccountResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     GetAppInstanceStreamingConfigurationsResponseTypeDef,
     GetAttendeeResponseTypeDef,
@@ -162,15 +161,15 @@
     ListUsersResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     LoggingConfigurationTypeDef,
     MeetingNotificationConfigurationTypeDef,
     MembershipItemTypeDef,
-    OriginationTypeDef,
+    OriginationUnionTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     PutRetentionSettingsResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
@@ -185,17 +184,18 @@
     RetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     SigninDelegateGroupTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
-    StreamingConfigurationTypeDef,
+    StreamingConfigurationUnionTypeDef,
     TagTypeDef,
-    TerminationTypeDef,
+    TerminationUnionTypeDef,
+    TimestampTypeDef,
     TranscriptionConfigurationTypeDef,
     UpdateAccountResponseTypeDef,
     UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserResponseTypeDef,
     UpdateBotResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerResponseTypeDef,
@@ -514,15 +514,15 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media capture pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_media_capture_pipeline)
         """
@@ -1476,16 +1476,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#list_channel_memberships_for_app_instance_user)
         """
     async def list_channel_messages(
         self,
         *,
         ChannelArn: str,
         SortOrder: SortOrderType = ...,
-        NotBefore: Union[datetime, str] = ...,
-        NotAfter: Union[datetime, str] = ...,
+        NotBefore: TimestampTypeDef = ...,
+        NotAfter: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         ChimeBearer: str = ...
     ) -> ListChannelMessagesResponseTypeDef:
         """
         List all the messages in a channel.
 
@@ -1766,15 +1766,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_sip_media_application_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_sip_media_application_logging_configuration)
         """
     async def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
-        EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef
+        EmergencyCallingConfiguration: EmergencyCallingConfigurationUnionTypeDef
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
         Puts emergency calling configuration details to the specified Amazon Chime Voice
         Connector, such as emergency phone numbers and calling countries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_emergency_calling_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_emergency_calling_configuration)
@@ -1785,15 +1785,15 @@
         """
         Adds a logging configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_logging_configuration)
         """
     async def put_voice_connector_origination(
-        self, *, VoiceConnectorId: str, Origination: OriginationTypeDef
+        self, *, VoiceConnectorId: str, Origination: OriginationUnionTypeDef
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
         Adds origination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_origination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_origination)
         """
@@ -1810,24 +1810,24 @@
         Puts the specified proxy configuration to the specified Amazon Chime Voice
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_proxy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_proxy)
         """
     async def put_voice_connector_streaming_configuration(
-        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationTypeDef
+        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationUnionTypeDef
     ) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
         Adds a streaming configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_streaming_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_streaming_configuration)
         """
     async def put_voice_connector_termination(
-        self, *, VoiceConnectorId: str, Termination: TerminationTypeDef
+        self, *, VoiceConnectorId: str, Termination: TerminationUnionTypeDef
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
         Adds termination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_termination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_termination)
         """
```

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/literals.py` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/literals.pyi` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/paginator.py` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str = ...,
         UserEmail: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/paginators/#listaccountspaginator)
         """
 
 
@@ -70,13 +70,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         UserEmail: str = ...,
         UserType: UserTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/paginators/#listuserspaginator)
         """
```

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/paginator.pyi` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     """
 
     def paginate(
         self,
         *,
         Name: str = ...,
         UserEmail: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/paginators/#listaccountspaginator)
         """
 
 class ListUsersPaginator(AioPaginator):
@@ -66,13 +66,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         UserEmail: str = ...,
         UserType: UserTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Paginator.ListUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/paginators/#listuserspaginator)
         """
```

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/type_defs.py` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_chime.type_defs import AccountSettingsTypeDef
 
-    data: AccountSettingsTypeDef = {...}
+    data: AccountSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -85,14 +85,15 @@
     "AppInstanceUserTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "AssociatePhoneNumberWithUserRequestRequestTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeErrorTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
     "MembershipItemTypeDef",
     "MemberErrorTypeDef",
@@ -105,23 +106,19 @@
     "BusinessCallingSettingsTypeDef",
     "CandidateAddressTypeDef",
     "ChannelSummaryTypeDef",
     "ConversationRetentionSettingsTypeDef",
     "CreateAccountRequestRequestTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
     "TagTypeDef",
-    "CreateAppInstanceResponseTypeDef",
-    "CreateAppInstanceUserResponseTypeDef",
     "CreateBotRequestRequestTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
-    "CreateChannelResponseTypeDef",
     "CreateMeetingDialOutRequestRequestTypeDef",
-    "CreateMeetingDialOutResponseTypeDef",
     "MeetingNotificationConfigurationTypeDef",
     "CreatePhoneNumberOrderRequestRequestTypeDef",
     "GeoMatchParamsTypeDef",
     "CreateRoomMembershipRequestRequestTypeDef",
     "CreateRoomRequestRequestTypeDef",
     "RoomTypeDef",
     "CreateSipMediaApplicationCallRequestRequestTypeDef",
@@ -171,15 +168,14 @@
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelModeratorRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DisassociatePhoneNumberFromUserRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "EventsConfigurationTypeDef",
     "GetAccountRequestRequestTypeDef",
     "GetAccountSettingsRequestRequestTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     "GetAppInstanceStreamingConfigurationsRequestRequestTypeDef",
@@ -189,15 +185,14 @@
     "GetEventsConfigurationRequestRequestTypeDef",
     "VoiceConnectorSettingsTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
-    "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetRetentionSettingsRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
@@ -211,29 +206,29 @@
     "GetVoiceConnectorProxyRequestRequestTypeDef",
     "ProxyTypeDef",
     "GetVoiceConnectorRequestRequestTypeDef",
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
-    "TerminationTypeDef",
+    "TerminationOutputTypeDef",
     "InviteTypeDef",
     "InviteUsersRequestRequestTypeDef",
-    "ListAccountsRequestListAccountsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListAttendeeTagsRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListBotsRequestRequestTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
-    "ListChannelMessagesRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "ListMeetingTagsRequestRequestTypeDef",
     "ListMeetingsRequestRequestTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
@@ -242,72 +237,61 @@
     "ListRoomMembershipsRequestRequestTypeDef",
     "ListRoomsRequestRequestTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
     "LogoutUserRequestRequestTypeDef",
     "MediaPlacementTypeDef",
     "MemberTypeDef",
     "OrderedPhoneNumberTypeDef",
     "OriginationRouteTypeDef",
-    "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutEventsConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
+    "TerminationTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
-    "RedactChannelMessageResponseTypeDef",
     "RedactConversationMessageRequestRequestTypeDef",
     "RedactRoomMessageRequestRequestTypeDef",
     "RegenerateSecurityTokenRequestRequestTypeDef",
     "ResetPersonalPINRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "RoomRetentionSettingsTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
-    "SearchAvailablePhoneNumbersResponseTypeDef",
+    "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "SendChannelMessageRequestRequestTypeDef",
-    "SendChannelMessageResponseTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "StreamingNotificationTargetTypeDef",
     "TelephonySettingsTypeDef",
     "UntagAttendeeRequestRequestTypeDef",
     "UntagMeetingRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccountRequestRequestTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
-    "UpdateAppInstanceResponseTypeDef",
     "UpdateAppInstanceUserRequestRequestTypeDef",
-    "UpdateAppInstanceUserResponseTypeDef",
     "UpdateBotRequestRequestTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
-    "UpdateChannelMessageResponseTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
-    "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "UpdateChannelResponseTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateRoomMembershipRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
-    "GetAccountSettingsResponseTypeDef",
     "UpdateAccountSettingsRequestRequestTypeDef",
     "AccountTypeDef",
     "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
     "UpdateUserRequestItemTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UserTypeDef",
     "AppInstanceAdminSummaryTypeDef",
@@ -318,33 +302,49 @@
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
     "ChannelTypeDef",
-    "CreateAppInstanceAdminResponseTypeDef",
-    "CreateChannelBanResponseTypeDef",
-    "CreateChannelMembershipResponseTypeDef",
-    "CreateChannelModeratorResponseTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
-    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
     "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
-    "ListAppInstancesResponseTypeDef",
-    "DescribeAppInstanceResponseTypeDef",
-    "ListAppInstanceUsersResponseTypeDef",
-    "DescribeAppInstanceUserResponseTypeDef",
     "ArtifactsConfigurationTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
+    "CreateAppInstanceAdminResponseTypeDef",
+    "CreateAppInstanceResponseTypeDef",
+    "CreateAppInstanceUserResponseTypeDef",
+    "CreateChannelBanResponseTypeDef",
+    "CreateChannelMembershipResponseTypeDef",
+    "CreateChannelModeratorResponseTypeDef",
+    "CreateChannelResponseTypeDef",
+    "CreateMeetingDialOutResponseTypeDef",
+    "DescribeAppInstanceResponseTypeDef",
+    "DescribeAppInstanceUserResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAccountSettingsResponseTypeDef",
+    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
+    "GetPhoneNumberSettingsResponseTypeDef",
+    "ListAppInstanceUsersResponseTypeDef",
+    "ListAppInstancesResponseTypeDef",
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+    "RedactChannelMessageResponseTypeDef",
+    "SearchAvailablePhoneNumbersResponseTypeDef",
+    "SendChannelMessageResponseTypeDef",
+    "UpdateAppInstanceResponseTypeDef",
+    "UpdateAppInstanceUserResponseTypeDef",
+    "UpdateChannelMessageResponseTypeDef",
+    "UpdateChannelReadMarkerResponseTypeDef",
+    "UpdateChannelResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     "BatchCreateRoomMembershipResponseTypeDef",
     "BatchSuspendUserResponseTypeDef",
@@ -389,14 +389,15 @@
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
     "VoiceConnectorGroupTypeDef",
     "CreateVoiceConnectorResponseTypeDef",
     "GetVoiceConnectorResponseTypeDef",
     "ListVoiceConnectorsResponseTypeDef",
     "UpdateVoiceConnectorResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
+    "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "TranscriptionConfigurationTypeDef",
     "GetEventsConfigurationResponseTypeDef",
     "PutEventsConfigurationResponseTypeDef",
     "GetGlobalSettingsResponseTypeDef",
     "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
@@ -406,26 +407,33 @@
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "InviteUsersResponseTypeDef",
+    "ListAccountsRequestListAccountsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
+    "ListChannelMessagesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     "MeetingTypeDef",
     "RoomMembershipTypeDef",
     "PhoneNumberOrderTypeDef",
+    "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    "TerminationUnionTypeDef",
     "RetentionSettingsTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
+    "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
     "UserSettingsTypeDef",
     "CreateAccountResponseTypeDef",
     "GetAccountResponseTypeDef",
     "ListAccountsResponseTypeDef",
     "UpdateAccountResponseTypeDef",
     "BatchUpdateUserRequestRequestTypeDef",
@@ -464,49 +472,54 @@
     "ListSipRulesResponseTypeDef",
     "UpdateSipRuleResponseTypeDef",
     "CreateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorGroupResponseTypeDef",
     "ListVoiceConnectorGroupsResponseTypeDef",
     "UpdateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+    "EmergencyCallingConfigurationUnionTypeDef",
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
     "ListMeetingsResponseTypeDef",
     "CreateRoomMembershipResponseTypeDef",
     "ListRoomMembershipsResponseTypeDef",
     "UpdateRoomMembershipResponseTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "PutVoiceConnectorOriginationResponseTypeDef",
+    "OriginationUnionTypeDef",
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "CreateProxySessionResponseTypeDef",
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
     "GetRetentionSettingsResponseTypeDef",
     "PutRetentionSettingsRequestRequestTypeDef",
     "PutRetentionSettingsResponseTypeDef",
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+    "StreamingConfigurationUnionTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
-    "CreateMediaCapturePipelineRequestRequestTypeDef",
     "MediaCapturePipelineTypeDef",
+    "ChimeSdkMeetingConfigurationUnionTypeDef",
+    "CreateMediaCapturePipelineRequestRequestTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
@@ -716,14 +729,25 @@
         "PhoneNumberId": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
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
 _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "E164PhoneNumbers": Sequence[str],
     },
 )
@@ -949,30 +973,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAppInstanceResponseTypeDef = TypedDict(
-    "CreateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAppInstanceUserResponseTypeDef = TypedDict(
-    "CreateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateBotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotRequestRequestTypeDef",
     {
         "AccountId": str,
         "DisplayName": str,
     },
 )
@@ -1056,40 +1064,24 @@
 class CreateChannelModeratorRequestRequestTypeDef(
     _RequiredCreateChannelModeratorRequestRequestTypeDef,
     _OptionalCreateChannelModeratorRequestRequestTypeDef,
 ):
     pass
 
 
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMeetingDialOutRequestRequestTypeDef = TypedDict(
     "CreateMeetingDialOutRequestRequestTypeDef",
     {
         "MeetingId": str,
         "FromPhoneNumber": str,
         "ToPhoneNumber": str,
         "JoinToken": str,
     },
 )
 
-CreateMeetingDialOutResponseTypeDef = TypedDict(
-    "CreateMeetingDialOutResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MeetingNotificationConfigurationTypeDef = TypedDict(
     "MeetingNotificationConfigurationTypeDef",
     {
         "SnsTopicArn": str,
         "SqsQueueArn": str,
     },
     total=False,
@@ -1788,21 +1780,14 @@
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
     {
         "AccountId": str,
         "GroupNames": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEngineTranscribeMedicalSettingsTypeDef = TypedDict(
     "_RequiredEngineTranscribeMedicalSettingsTypeDef",
     {
         "LanguageCode": Literal["en-US"],
         "Specialty": TranscribeMedicalSpecialtyType,
         "Type": TranscribeMedicalTypeType,
     },
@@ -1971,23 +1956,14 @@
 GetPhoneNumberRequestRequestTypeDef = TypedDict(
     "GetPhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
-GetPhoneNumberSettingsResponseTypeDef = TypedDict(
-    "GetPhoneNumberSettingsResponseTypeDef",
-    {
-        "CallingName": str,
-        "CallingNameUpdatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetProxySessionRequestRequestTypeDef = TypedDict(
     "GetProxySessionRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "ProxySessionId": str,
     },
 )
@@ -2140,16 +2116,16 @@
 GetVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-TerminationTypeDef = TypedDict(
-    "TerminationTypeDef",
+TerminationOutputTypeDef = TypedDict(
+    "TerminationOutputTypeDef",
     {
         "CpsLimit": int,
         "DefaultPhoneNumber": str,
         "CallingRegions": List[str],
         "CidrAllowedList": List[str],
         "Disabled": bool,
     },
@@ -2185,20 +2161,20 @@
 
 class InviteUsersRequestRequestTypeDef(
     _RequiredInviteUsersRequestRequestTypeDef, _OptionalInviteUsersRequestRequestTypeDef
 ):
     pass
 
 
-ListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "ListAccountsRequestListAccountsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Name": str,
-        "UserEmail": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccountsRequestRequestTypeDef = TypedDict(
     "ListAccountsRequestRequestTypeDef",
     {
@@ -2372,41 +2348,15 @@
 class ListChannelMembershipsRequestRequestTypeDef(
     _RequiredListChannelMembershipsRequestRequestTypeDef,
     _OptionalListChannelMembershipsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
-    "_RequiredListChannelMessagesRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
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
-        "ChimeBearer": str,
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
     },
 )
 _OptionalListChannelModeratorsRequestRequestTypeDef = TypedDict(
@@ -2617,38 +2567,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "UserEmail": str,
-        "UserType": UserTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -2681,22 +2607,14 @@
 ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
-    {
-        "Usernames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListVoiceConnectorsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -2754,24 +2672,14 @@
         "Protocol": OriginationRouteProtocolType,
         "Priority": int,
         "Weight": int,
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
 ParticipantTypeDef = TypedDict(
     "ParticipantTypeDef",
     {
         "PhoneNumber": str,
         "ProxyPhoneNumber": str,
     },
     total=False,
@@ -2845,14 +2753,26 @@
 class PutVoiceConnectorProxyRequestRequestTypeDef(
     _RequiredPutVoiceConnectorProxyRequestRequestTypeDef,
     _OptionalPutVoiceConnectorProxyRequestRequestTypeDef,
 ):
     pass
 
 
+TerminationTypeDef = TypedDict(
+    "TerminationTypeDef",
+    {
+        "CpsLimit": int,
+        "DefaultPhoneNumber": str,
+        "CallingRegions": Sequence[str],
+        "CidrAllowedList": Sequence[str],
+        "Disabled": bool,
+    },
+    total=False,
+)
+
 _RequiredRedactChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredRedactChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
     },
 )
@@ -2868,23 +2788,14 @@
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
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RedactConversationMessageRequestRequestTypeDef = TypedDict(
     "RedactConversationMessageRequestRequestTypeDef",
     {
         "AccountId": str,
         "ConversationId": str,
         "MessageId": str,
     },
@@ -2911,25 +2822,14 @@
     "ResetPersonalPINRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
     },
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
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
@@ -2952,21 +2852,21 @@
         "PhoneNumberType": PhoneNumberTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
-    "SearchAvailablePhoneNumbersResponseTypeDef",
+SelectedVideoStreamsOutputTypeDef = TypedDict(
+    "SelectedVideoStreamsOutputTypeDef",
     {
-        "E164PhoneNumbers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AttendeeIds": List[str],
+        "ExternalUserIds": List[str],
     },
+    total=False,
 )
 
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
@@ -2997,23 +2897,14 @@
 class SendChannelMessageRequestRequestTypeDef(
     _RequiredSendChannelMessageRequestRequestTypeDef,
     _OptionalSendChannelMessageRequestRequestTypeDef,
 ):
     pass
 
 
-SendChannelMessageResponseTypeDef = TypedDict(
-    "SendChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
@@ -3098,22 +2989,14 @@
 
 class UpdateAppInstanceRequestRequestTypeDef(
     _RequiredUpdateAppInstanceRequestRequestTypeDef, _OptionalUpdateAppInstanceRequestRequestTypeDef
 ):
     pass
 
 
-UpdateAppInstanceResponseTypeDef = TypedDict(
-    "UpdateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAppInstanceUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
     },
 )
@@ -3129,22 +3012,14 @@
 class UpdateAppInstanceUserRequestRequestTypeDef(
     _RequiredUpdateAppInstanceUserRequestRequestTypeDef,
     _OptionalUpdateAppInstanceUserRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateAppInstanceUserResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateBotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotRequestRequestTypeDef",
     {
         "AccountId": str,
         "BotId": str,
     },
 )
@@ -3184,23 +3059,14 @@
 class UpdateChannelMessageRequestRequestTypeDef(
     _RequiredUpdateChannelMessageRequestRequestTypeDef,
     _OptionalUpdateChannelMessageRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateChannelMessageResponseTypeDef = TypedDict(
-    "UpdateChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
     },
 )
 _OptionalUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
@@ -3215,22 +3081,14 @@
 class UpdateChannelReadMarkerRequestRequestTypeDef(
     _RequiredUpdateChannelReadMarkerRequestRequestTypeDef,
     _OptionalUpdateChannelReadMarkerRequestRequestTypeDef,
 ):
     pass
 
 
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
         "Name": str,
         "Mode": ChannelModeType,
     },
@@ -3247,22 +3105,14 @@
 
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
 _RequiredUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 _OptionalUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
@@ -3385,22 +3235,14 @@
         "City": str,
         "State": str,
         "Country": str,
         "PostalCode": str,
     },
 )
 
-GetAccountSettingsResponseTypeDef = TypedDict(
-    "GetAccountSettingsResponseTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
     "UpdateAccountSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "AccountSettings": AccountSettingsTypeDef,
     },
 )
@@ -3650,205 +3492,337 @@
         "CreatedTimestamp": datetime,
         "LastMessageTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+AppInstanceRetentionSettingsTypeDef = TypedDict(
+    "AppInstanceRetentionSettingsTypeDef",
+    {
+        "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
+    },
+    total=False,
+)
+
+PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
+    {
+        "AppInstanceArn": str,
+        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
+    },
+)
+
+ArtifactsConfigurationTypeDef = TypedDict(
+    "ArtifactsConfigurationTypeDef",
+    {
+        "Audio": AudioArtifactsConfigurationTypeDef,
+        "Video": VideoArtifactsConfigurationTypeDef,
+        "Content": ContentArtifactsConfigurationTypeDef,
+    },
+)
+
+AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
+    "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchDeletePhoneNumberResponseTypeDef = TypedDict(
+    "BatchDeletePhoneNumberResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
+    "BatchUpdatePhoneNumberResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateAppInstanceAdminResponseTypeDef = TypedDict(
     "CreateAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": IdentityTypeDef,
         "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceResponseTypeDef = TypedDict(
+    "CreateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceUserResponseTypeDef = TypedDict(
+    "CreateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelBanResponseTypeDef = TypedDict(
     "CreateChannelBanResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelMembershipResponseTypeDef = TypedDict(
     "CreateChannelMembershipResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
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
     },
 )
 
-AppInstanceRetentionSettingsTypeDef = TypedDict(
-    "AppInstanceRetentionSettingsTypeDef",
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
     {
-        "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMeetingDialOutResponseTypeDef = TypedDict(
+    "CreateMeetingDialOutResponseTypeDef",
+    {
+        "TransactionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppInstanceResponseTypeDef = TypedDict(
+    "DescribeAppInstanceResponseTypeDef",
+    {
+        "AppInstance": AppInstanceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppInstanceUserResponseTypeDef = TypedDict(
+    "DescribeAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUser": AppInstanceUserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
+    "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
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
+GetAccountSettingsResponseTypeDef = TypedDict(
+    "GetAccountSettingsResponseTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetAppInstanceStreamingConfigurationsResponseTypeDef",
     {
         "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
+GetPhoneNumberSettingsResponseTypeDef = TypedDict(
+    "GetPhoneNumberSettingsResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
+        "CallingName": str,
+        "CallingNameUpdatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+ListAppInstanceUsersResponseTypeDef = TypedDict(
+    "ListAppInstanceUsersResponseTypeDef",
     {
-        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceArn": str,
+        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppInstancesResponseTypeDef = TypedDict(
     "ListAppInstancesResponseTypeDef",
     {
         "AppInstances": List[AppInstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAppInstanceResponseTypeDef = TypedDict(
-    "DescribeAppInstanceResponseTypeDef",
+ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     {
-        "AppInstance": AppInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Usernames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAppInstanceUsersResponseTypeDef = TypedDict(
-    "ListAppInstanceUsersResponseTypeDef",
+PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAppInstanceUserResponseTypeDef = TypedDict(
-    "DescribeAppInstanceUserResponseTypeDef",
+RedactChannelMessageResponseTypeDef = TypedDict(
+    "RedactChannelMessageResponseTypeDef",
     {
-        "AppInstanceUser": AppInstanceUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ArtifactsConfigurationTypeDef = TypedDict(
-    "ArtifactsConfigurationTypeDef",
+SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     {
-        "Audio": AudioArtifactsConfigurationTypeDef,
-        "Video": VideoArtifactsConfigurationTypeDef,
-        "Content": ContentArtifactsConfigurationTypeDef,
+        "E164PhoneNumbers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
+SendChannelMessageResponseTypeDef = TypedDict(
+    "SendChannelMessageResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
-    "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
+UpdateAppInstanceResponseTypeDef = TypedDict(
+    "UpdateAppInstanceResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDeletePhoneNumberResponseTypeDef = TypedDict(
-    "BatchDeletePhoneNumberResponseTypeDef",
+UpdateAppInstanceUserResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
-    "BatchUpdatePhoneNumberResponseTypeDef",
+UpdateChannelMessageResponseTypeDef = TypedDict(
+    "UpdateChannelMessageResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
+UpdateChannelReadMarkerResponseTypeDef = TypedDict(
+    "UpdateChannelReadMarkerResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
-    "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
+UpdateChannelResponseTypeDef = TypedDict(
+    "UpdateChannelResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAttendeeResponseTypeDef = TypedDict(
     "CreateAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAttendeeResponseTypeDef = TypedDict(
     "GetAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttendeesResponseTypeDef = TypedDict(
     "ListAttendeesResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateAttendeeResponseTypeDef = TypedDict(
     "BatchCreateAttendeeResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateRoomMembershipRequestRequestTypeDef = TypedDict(
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -3857,98 +3831,98 @@
     },
 )
 
 BatchCreateRoomMembershipResponseTypeDef = TypedDict(
     "BatchCreateRoomMembershipResponseTypeDef",
     {
         "Errors": List[MemberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchSuspendUserResponseTypeDef = TypedDict(
     "BatchSuspendUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUnsuspendUserResponseTypeDef = TypedDict(
     "BatchUnsuspendUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateUserResponseTypeDef = TypedDict(
     "BatchUpdateUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
     },
 )
 
 CreateBotResponseTypeDef = TypedDict(
     "CreateBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBotsResponseTypeDef = TypedDict(
     "ListBotsResponseTypeDef",
     {
         "Bots": List[BotTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegenerateSecurityTokenResponseTypeDef = TypedDict(
     "RegenerateSecurityTokenResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotResponseTypeDef = TypedDict(
     "UpdateBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidateE911AddressResponseTypeDef = TypedDict(
     "ValidateE911AddressResponseTypeDef",
     {
         "ValidationResult": int,
         "AddressExternalId": str,
         "Address": AddressTypeDef,
         "CandidateAddressList": List[CandidateAddressTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChannelMembershipForAppInstanceUserSummaryTypeDef = TypedDict(
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     {
         "ChannelSummary": ChannelSummaryTypeDef,
@@ -3966,15 +3940,15 @@
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
 
 _RequiredCreateAppInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppInstanceRequestRequestTypeDef",
     {
         "Name": str,
@@ -4093,31 +4067,31 @@
     pass
 
 
 ListAttendeeTagsResponseTypeDef = TypedDict(
     "ListAttendeeTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMeetingTagsResponseTypeDef = TypedDict(
     "ListMeetingTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagAttendeeRequestRequestTypeDef = TypedDict(
     "TagAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -4195,56 +4169,56 @@
     pass
 
 
 CreateRoomResponseTypeDef = TypedDict(
     "CreateRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoomResponseTypeDef = TypedDict(
     "GetRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoomsResponseTypeDef = TypedDict(
     "ListRoomsResponseTypeDef",
     {
         "Rooms": List[RoomTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRoomResponseTypeDef = TypedDict(
     "UpdateRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSipMediaApplicationCallResponseTypeDef = TypedDict(
     "CreateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSipMediaApplicationCallResponseTypeDef = TypedDict(
     "UpdateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "CreateSipMediaApplicationRequestRequestTypeDef",
     {
         "AwsRegion": str,
@@ -4395,40 +4369,40 @@
     total=False,
 )
 
 CreateVoiceConnectorResponseTypeDef = TypedDict(
     "CreateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorResponseTypeDef = TypedDict(
     "GetVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVoiceConnectorsResponseTypeDef = TypedDict(
     "ListVoiceConnectorsResponseTypeDef",
     {
         "VoiceConnectors": List[VoiceConnectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceConnectorResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -4446,18 +4420,26 @@
 class PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef(
     _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
 ):
     pass
 
 
+EmergencyCallingConfigurationOutputTypeDef = TypedDict(
+    "EmergencyCallingConfigurationOutputTypeDef",
+    {
+        "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
+    },
+    total=False,
+)
+
 EmergencyCallingConfigurationTypeDef = TypedDict(
     "EmergencyCallingConfigurationTypeDef",
     {
-        "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
+        "DNIS": Sequence[DNISEmergencyCallingConfigurationTypeDef],
     },
     total=False,
 )
 
 TranscriptionConfigurationTypeDef = TypedDict(
     "TranscriptionConfigurationTypeDef",
     {
@@ -4467,32 +4449,32 @@
     total=False,
 )
 
 GetEventsConfigurationResponseTypeDef = TypedDict(
     "GetEventsConfigurationResponseTypeDef",
     {
         "EventsConfiguration": EventsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEventsConfigurationResponseTypeDef = TypedDict(
     "PutEventsConfigurationResponseTypeDef",
     {
         "EventsConfiguration": EventsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
         "BusinessCalling": BusinessCallingSettingsTypeDef,
         "VoiceConnector": VoiceConnectorSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsRequestRequestTypeDef",
     {
         "BusinessCalling": BusinessCallingSettingsTypeDef,
@@ -4501,23 +4483,23 @@
     total=False,
 )
 
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
         "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
@@ -4539,23 +4521,23 @@
     pass
 
 
 PutSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
         "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -4563,79 +4545,132 @@
     },
 )
 
 PutVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorProxyResponseTypeDef = TypedDict(
     "GetVoiceConnectorProxyResponseTypeDef",
     {
         "Proxy": ProxyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorProxyResponseTypeDef = TypedDict(
     "PutVoiceConnectorProxyResponseTypeDef",
     {
         "Proxy": ProxyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorTerminationHealthResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     {
         "TerminationHealth": TerminationHealthTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "Termination": TerminationTypeDef,
+        "Termination": TerminationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "PutVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Termination": TerminationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InviteUsersResponseTypeDef = TypedDict(
     "InviteUsersResponseTypeDef",
     {
         "Invites": List[InviteTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "ListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "Name": str,
+        "UserEmail": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "UserEmail": str,
+        "UserType": UserTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_RequiredListChannelMessagesRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
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
+        "ChimeBearer": str,
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
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MeetingTypeDef = TypedDict(
     "MeetingTypeDef",
     {
         "MeetingId": str,
@@ -4667,18 +4702,27 @@
         "OrderedPhoneNumbers": List[OrderedPhoneNumberTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+OriginationOutputTypeDef = TypedDict(
+    "OriginationOutputTypeDef",
+    {
+        "Routes": List[OriginationRouteTypeDef],
+        "Disabled": bool,
+    },
+    total=False,
+)
+
 OriginationTypeDef = TypedDict(
     "OriginationTypeDef",
     {
-        "Routes": List[OriginationRouteTypeDef],
+        "Routes": Sequence[OriginationRouteTypeDef],
         "Disabled": bool,
     },
     total=False,
 )
 
 ProxySessionTypeDef = TypedDict(
     "ProxySessionTypeDef",
@@ -4716,42 +4760,81 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "DeletionTimestamp": datetime,
     },
     total=False,
 )
 
+PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "Termination": TerminationTypeDef,
+    },
+)
+
+TerminationUnionTypeDef = Union[TerminationTypeDef, TerminationOutputTypeDef]
 RetentionSettingsTypeDef = TypedDict(
     "RetentionSettingsTypeDef",
     {
         "RoomRetentionSettings": RoomRetentionSettingsTypeDef,
         "ConversationRetentionSettings": ConversationRetentionSettingsTypeDef,
     },
     total=False,
 )
 
+SourceConfigurationOutputTypeDef = TypedDict(
+    "SourceConfigurationOutputTypeDef",
+    {
+        "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
+_RequiredStreamingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredStreamingConfigurationOutputTypeDef",
+    {
+        "DataRetentionInHours": int,
+    },
+)
+_OptionalStreamingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalStreamingConfigurationOutputTypeDef",
+    {
+        "Disabled": bool,
+        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
+    },
+    total=False,
+)
+
+
+class StreamingConfigurationOutputTypeDef(
+    _RequiredStreamingConfigurationOutputTypeDef, _OptionalStreamingConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredStreamingConfigurationTypeDef = TypedDict(
     "_RequiredStreamingConfigurationTypeDef",
     {
         "DataRetentionInHours": int,
     },
 )
 _OptionalStreamingConfigurationTypeDef = TypedDict(
     "_OptionalStreamingConfigurationTypeDef",
     {
         "Disabled": bool,
-        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
+        "StreamingNotificationTargets": Sequence[StreamingNotificationTargetTypeDef],
     },
     total=False,
 )
 
 
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
@@ -4766,40 +4849,40 @@
     },
 )
 
 CreateAccountResponseTypeDef = TypedDict(
     "CreateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountsResponseTypeDef = TypedDict(
     "ListAccountsResponseTypeDef",
     {
         "Accounts": List[AccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountResponseTypeDef = TypedDict(
     "UpdateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateUserRequestRequestTypeDef = TypedDict(
     "BatchUpdateUserRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -4807,164 +4890,164 @@
     },
 )
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserResponseTypeDef = TypedDict(
     "GetUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetPersonalPINResponseTypeDef = TypedDict(
     "ResetPersonalPINResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppInstanceAdminsResponseTypeDef = TypedDict(
     "ListAppInstanceAdminsResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceAdmins": List[AppInstanceAdminSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppInstanceAdminResponseTypeDef = TypedDict(
     "DescribeAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": AppInstanceAdminTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
 
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
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
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     {
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
     "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -4973,49 +5056,49 @@
 )
 
 PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "PutAppInstanceRetentionSettingsResponseTypeDef",
     {
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
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
 
 BatchCreateAttendeeRequestRequestTypeDef = TypedDict(
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -5050,130 +5133,133 @@
     pass
 
 
 CreateSipMediaApplicationResponseTypeDef = TypedDict(
     "CreateSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSipMediaApplicationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSipMediaApplicationsResponseTypeDef = TypedDict(
     "ListSipMediaApplicationsResponseTypeDef",
     {
         "SipMediaApplications": List[SipMediaApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSipMediaApplicationResponseTypeDef = TypedDict(
     "UpdateSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSipRuleResponseTypeDef = TypedDict(
     "CreateSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSipRuleResponseTypeDef = TypedDict(
     "GetSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSipRulesResponseTypeDef = TypedDict(
     "ListSipRulesResponseTypeDef",
     {
         "SipRules": List[SipRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSipRuleResponseTypeDef = TypedDict(
     "UpdateSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
     "CreateVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorGroupResponseTypeDef = TypedDict(
     "GetVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
     "ListVoiceConnectorGroupsResponseTypeDef",
     {
         "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
+PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+EmergencyCallingConfigurationUnionTypeDef = Union[
+    EmergencyCallingConfigurationTypeDef, EmergencyCallingConfigurationOutputTypeDef
+]
+PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StartMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -5181,191 +5267,192 @@
     },
 )
 
 CreateMeetingResponseTypeDef = TypedDict(
     "CreateMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMeetingWithAttendeesResponseTypeDef = TypedDict(
     "CreateMeetingWithAttendeesResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMeetingResponseTypeDef = TypedDict(
     "GetMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMeetingsResponseTypeDef = TypedDict(
     "ListMeetingsResponseTypeDef",
     {
         "Meetings": List[MeetingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRoomMembershipResponseTypeDef = TypedDict(
     "CreateRoomMembershipResponseTypeDef",
     {
         "RoomMembership": RoomMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoomMembershipsResponseTypeDef = TypedDict(
     "ListRoomMembershipsResponseTypeDef",
     {
         "RoomMemberships": List[RoomMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRoomMembershipResponseTypeDef = TypedDict(
     "UpdateRoomMembershipResponseTypeDef",
     {
         "RoomMembership": RoomMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePhoneNumberOrderResponseTypeDef = TypedDict(
     "CreatePhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPhoneNumberOrderResponseTypeDef = TypedDict(
     "GetPhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPhoneNumberOrdersResponseTypeDef = TypedDict(
     "ListPhoneNumberOrdersResponseTypeDef",
     {
         "PhoneNumberOrders": List[PhoneNumberOrderTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "GetVoiceConnectorOriginationResponseTypeDef",
     {
-        "Origination": OriginationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Origination": OriginationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
+PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "Origination": OriginationTypeDef,
+        "Origination": OriginationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationResponseTypeDef",
+OriginationUnionTypeDef = Union[OriginationTypeDef, OriginationOutputTypeDef]
+PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "Origination": OriginationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProxySessionResponseTypeDef = TypedDict(
     "CreateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProxySessionResponseTypeDef = TypedDict(
     "GetProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProxySessionsResponseTypeDef = TypedDict(
     "ListProxySessionsResponseTypeDef",
     {
         "ProxySessions": List[ProxySessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProxySessionResponseTypeDef = TypedDict(
     "UpdateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPhoneNumberResponseTypeDef = TypedDict(
     "GetPhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPhoneNumbersResponseTypeDef = TypedDict(
     "ListPhoneNumbersResponseTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestorePhoneNumberResponseTypeDef = TypedDict(
     "RestorePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePhoneNumberResponseTypeDef = TypedDict(
     "UpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRetentionSettingsResponseTypeDef = TypedDict(
     "GetRetentionSettingsResponseTypeDef",
     {
         "RetentionSettings": RetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRetentionSettingsRequestRequestTypeDef = TypedDict(
     "PutRetentionSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -5374,68 +5461,99 @@
 )
 
 PutRetentionSettingsResponseTypeDef = TypedDict(
     "PutRetentionSettingsResponseTypeDef",
     {
         "RetentionSettings": RetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
+    {
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
+    total=False,
 )
 
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "StreamingConfiguration": StreamingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StreamingConfigurationUnionTypeDef = Union[
+    StreamingConfigurationTypeDef, StreamingConfigurationOutputTypeDef
+]
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "UserSettings": UserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserSettingsRequestRequestTypeDef = TypedDict(
     "UpdateUserSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
         "UserSettings": UserSettingsTypeDef,
     },
 )
 
+MediaCapturePipelineTypeDef = TypedDict(
+    "MediaCapturePipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "SourceArn": str,
+        "Status": MediaPipelineStatusType,
+        "SinkType": Literal["S3Bucket"],
+        "SinkArn": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+ChimeSdkMeetingConfigurationUnionTypeDef = Union[
+    ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
+]
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
@@ -5454,47 +5572,31 @@
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
 
-MediaCapturePipelineTypeDef = TypedDict(
-    "MediaCapturePipelineTypeDef",
-    {
-        "MediaPipelineId": str,
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "SourceArn": str,
-        "Status": MediaPipelineStatusType,
-        "SinkType": Literal["S3Bucket"],
-        "SinkArn": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
-    },
-    total=False,
-)
-
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime/type_defs.pyi` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_chime.type_defs import AccountSettingsTypeDef
 
-    data: AccountSettingsTypeDef = {...}
+    data: AccountSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -84,14 +84,15 @@
     "AppInstanceUserTypeDef",
     "AudioArtifactsConfigurationTypeDef",
     "ContentArtifactsConfigurationTypeDef",
     "VideoArtifactsConfigurationTypeDef",
     "AssociatePhoneNumberWithUserRequestRequestTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef",
     "PhoneNumberErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeErrorTypeDef",
     "BatchCreateChannelMembershipErrorTypeDef",
     "BatchCreateChannelMembershipRequestRequestTypeDef",
     "MembershipItemTypeDef",
     "MemberErrorTypeDef",
@@ -104,23 +105,19 @@
     "BusinessCallingSettingsTypeDef",
     "CandidateAddressTypeDef",
     "ChannelSummaryTypeDef",
     "ConversationRetentionSettingsTypeDef",
     "CreateAccountRequestRequestTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
     "TagTypeDef",
-    "CreateAppInstanceResponseTypeDef",
-    "CreateAppInstanceUserResponseTypeDef",
     "CreateBotRequestRequestTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
-    "CreateChannelResponseTypeDef",
     "CreateMeetingDialOutRequestRequestTypeDef",
-    "CreateMeetingDialOutResponseTypeDef",
     "MeetingNotificationConfigurationTypeDef",
     "CreatePhoneNumberOrderRequestRequestTypeDef",
     "GeoMatchParamsTypeDef",
     "CreateRoomMembershipRequestRequestTypeDef",
     "CreateRoomRequestRequestTypeDef",
     "RoomTypeDef",
     "CreateSipMediaApplicationCallRequestRequestTypeDef",
@@ -170,15 +167,14 @@
     "DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef",
     "DescribeChannelModeratorRequestRequestTypeDef",
     "DescribeChannelRequestRequestTypeDef",
     "DisassociatePhoneNumberFromUserRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef",
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "EventsConfigurationTypeDef",
     "GetAccountRequestRequestTypeDef",
     "GetAccountSettingsRequestRequestTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     "GetAppInstanceStreamingConfigurationsRequestRequestTypeDef",
@@ -188,15 +184,14 @@
     "GetEventsConfigurationRequestRequestTypeDef",
     "VoiceConnectorSettingsTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "MessagingSessionEndpointTypeDef",
     "GetPhoneNumberOrderRequestRequestTypeDef",
     "GetPhoneNumberRequestRequestTypeDef",
-    "GetPhoneNumberSettingsResponseTypeDef",
     "GetProxySessionRequestRequestTypeDef",
     "GetRetentionSettingsRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     "SipMediaApplicationLoggingConfigurationTypeDef",
     "GetSipMediaApplicationRequestRequestTypeDef",
     "GetSipRuleRequestRequestTypeDef",
@@ -210,29 +205,29 @@
     "GetVoiceConnectorProxyRequestRequestTypeDef",
     "ProxyTypeDef",
     "GetVoiceConnectorRequestRequestTypeDef",
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
-    "TerminationTypeDef",
+    "TerminationOutputTypeDef",
     "InviteTypeDef",
     "InviteUsersRequestRequestTypeDef",
-    "ListAccountsRequestListAccountsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListAttendeeTagsRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListBotsRequestRequestTypeDef",
     "ListChannelBansRequestRequestTypeDef",
     "ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef",
     "ListChannelMembershipsRequestRequestTypeDef",
-    "ListChannelMessagesRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListChannelModeratorsRequestRequestTypeDef",
     "ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef",
     "ListChannelsRequestRequestTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "ListMeetingTagsRequestRequestTypeDef",
     "ListMeetingsRequestRequestTypeDef",
     "ListPhoneNumberOrdersRequestRequestTypeDef",
@@ -241,72 +236,61 @@
     "ListRoomMembershipsRequestRequestTypeDef",
     "ListRoomsRequestRequestTypeDef",
     "ListSipMediaApplicationsRequestRequestTypeDef",
     "ListSipRulesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesRequestRequestTypeDef",
     "PhoneNumberCountryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVoiceConnectorGroupsRequestRequestTypeDef",
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     "ListVoiceConnectorsRequestRequestTypeDef",
     "LogoutUserRequestRequestTypeDef",
     "MediaPlacementTypeDef",
     "MemberTypeDef",
     "OrderedPhoneNumberTypeDef",
     "OriginationRouteTypeDef",
-    "PaginatorConfigTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutEventsConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
+    "TerminationTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
-    "RedactChannelMessageResponseTypeDef",
     "RedactConversationMessageRequestRequestTypeDef",
     "RedactRoomMessageRequestRequestTypeDef",
     "RegenerateSecurityTokenRequestRequestTypeDef",
     "ResetPersonalPINRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "RoomRetentionSettingsTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
-    "SearchAvailablePhoneNumbersResponseTypeDef",
+    "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "SendChannelMessageRequestRequestTypeDef",
-    "SendChannelMessageResponseTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "StreamingNotificationTargetTypeDef",
     "TelephonySettingsTypeDef",
     "UntagAttendeeRequestRequestTypeDef",
     "UntagMeetingRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccountRequestRequestTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
-    "UpdateAppInstanceResponseTypeDef",
     "UpdateAppInstanceUserRequestRequestTypeDef",
-    "UpdateAppInstanceUserResponseTypeDef",
     "UpdateBotRequestRequestTypeDef",
     "UpdateChannelMessageRequestRequestTypeDef",
-    "UpdateChannelMessageResponseTypeDef",
     "UpdateChannelReadMarkerRequestRequestTypeDef",
-    "UpdateChannelReadMarkerResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "UpdateChannelResponseTypeDef",
     "UpdatePhoneNumberRequestRequestTypeDef",
     "UpdatePhoneNumberSettingsRequestRequestTypeDef",
     "UpdateProxySessionRequestRequestTypeDef",
     "UpdateRoomMembershipRequestRequestTypeDef",
     "UpdateRoomRequestRequestTypeDef",
     "UpdateSipMediaApplicationCallRequestRequestTypeDef",
     "UpdateVoiceConnectorRequestRequestTypeDef",
     "ValidateE911AddressRequestRequestTypeDef",
-    "GetAccountSettingsResponseTypeDef",
     "UpdateAccountSettingsRequestRequestTypeDef",
     "AccountTypeDef",
     "AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef",
     "UpdateUserRequestItemTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UserTypeDef",
     "AppInstanceAdminSummaryTypeDef",
@@ -317,33 +301,49 @@
     "ChannelMembershipSummaryTypeDef",
     "ChannelMembershipTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
     "ChannelModeratorSummaryTypeDef",
     "ChannelModeratorTypeDef",
     "ChannelTypeDef",
-    "CreateAppInstanceAdminResponseTypeDef",
-    "CreateChannelBanResponseTypeDef",
-    "CreateChannelMembershipResponseTypeDef",
-    "CreateChannelModeratorResponseTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
-    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
     "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
-    "ListAppInstancesResponseTypeDef",
-    "DescribeAppInstanceResponseTypeDef",
-    "ListAppInstanceUsersResponseTypeDef",
-    "DescribeAppInstanceUserResponseTypeDef",
     "ArtifactsConfigurationTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
     "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
     "BatchDeletePhoneNumberResponseTypeDef",
     "BatchUpdatePhoneNumberResponseTypeDef",
+    "CreateAppInstanceAdminResponseTypeDef",
+    "CreateAppInstanceResponseTypeDef",
+    "CreateAppInstanceUserResponseTypeDef",
+    "CreateChannelBanResponseTypeDef",
+    "CreateChannelMembershipResponseTypeDef",
+    "CreateChannelModeratorResponseTypeDef",
+    "CreateChannelResponseTypeDef",
+    "CreateMeetingDialOutResponseTypeDef",
+    "DescribeAppInstanceResponseTypeDef",
+    "DescribeAppInstanceUserResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
     "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAccountSettingsResponseTypeDef",
+    "GetAppInstanceStreamingConfigurationsResponseTypeDef",
+    "GetPhoneNumberSettingsResponseTypeDef",
+    "ListAppInstanceUsersResponseTypeDef",
+    "ListAppInstancesResponseTypeDef",
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+    "RedactChannelMessageResponseTypeDef",
+    "SearchAvailablePhoneNumbersResponseTypeDef",
+    "SendChannelMessageResponseTypeDef",
+    "UpdateAppInstanceResponseTypeDef",
+    "UpdateAppInstanceUserResponseTypeDef",
+    "UpdateChannelMessageResponseTypeDef",
+    "UpdateChannelReadMarkerResponseTypeDef",
+    "UpdateChannelResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     "BatchCreateRoomMembershipResponseTypeDef",
     "BatchSuspendUserResponseTypeDef",
@@ -388,14 +388,15 @@
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
     "VoiceConnectorGroupTypeDef",
     "CreateVoiceConnectorResponseTypeDef",
     "GetVoiceConnectorResponseTypeDef",
     "ListVoiceConnectorsResponseTypeDef",
     "UpdateVoiceConnectorResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
+    "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "TranscriptionConfigurationTypeDef",
     "GetEventsConfigurationResponseTypeDef",
     "PutEventsConfigurationResponseTypeDef",
     "GetGlobalSettingsResponseTypeDef",
     "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
@@ -405,26 +406,33 @@
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "InviteUsersResponseTypeDef",
+    "ListAccountsRequestListAccountsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
+    "ListChannelMessagesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     "MeetingTypeDef",
     "RoomMembershipTypeDef",
     "PhoneNumberOrderTypeDef",
+    "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    "TerminationUnionTypeDef",
     "RetentionSettingsTypeDef",
+    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
+    "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
     "UserSettingsTypeDef",
     "CreateAccountResponseTypeDef",
     "GetAccountResponseTypeDef",
     "ListAccountsResponseTypeDef",
     "UpdateAccountResponseTypeDef",
     "BatchUpdateUserRequestRequestTypeDef",
@@ -463,49 +471,54 @@
     "ListSipRulesResponseTypeDef",
     "UpdateSipRuleResponseTypeDef",
     "CreateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorGroupResponseTypeDef",
     "ListVoiceConnectorGroupsResponseTypeDef",
     "UpdateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+    "EmergencyCallingConfigurationUnionTypeDef",
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
     "ListMeetingsResponseTypeDef",
     "CreateRoomMembershipResponseTypeDef",
     "ListRoomMembershipsResponseTypeDef",
     "UpdateRoomMembershipResponseTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "PutVoiceConnectorOriginationResponseTypeDef",
+    "OriginationUnionTypeDef",
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     "CreateProxySessionResponseTypeDef",
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
     "GetRetentionSettingsResponseTypeDef",
     "PutRetentionSettingsRequestRequestTypeDef",
     "PutRetentionSettingsResponseTypeDef",
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+    "StreamingConfigurationUnionTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
-    "CreateMediaCapturePipelineRequestRequestTypeDef",
     "MediaCapturePipelineTypeDef",
+    "ChimeSdkMeetingConfigurationUnionTypeDef",
+    "CreateMediaCapturePipelineRequestRequestTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
@@ -709,14 +722,25 @@
         "PhoneNumberId": str,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
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
 _RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef = TypedDict(
     "_RequiredAssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "E164PhoneNumbers": Sequence[str],
     },
 )
@@ -936,30 +960,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAppInstanceResponseTypeDef = TypedDict(
-    "CreateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAppInstanceUserResponseTypeDef = TypedDict(
-    "CreateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateBotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBotRequestRequestTypeDef",
     {
         "AccountId": str,
         "DisplayName": str,
     },
 )
@@ -1035,40 +1043,24 @@
 
 class CreateChannelModeratorRequestRequestTypeDef(
     _RequiredCreateChannelModeratorRequestRequestTypeDef,
     _OptionalCreateChannelModeratorRequestRequestTypeDef,
 ):
     pass
 
-CreateChannelResponseTypeDef = TypedDict(
-    "CreateChannelResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateMeetingDialOutRequestRequestTypeDef = TypedDict(
     "CreateMeetingDialOutRequestRequestTypeDef",
     {
         "MeetingId": str,
         "FromPhoneNumber": str,
         "ToPhoneNumber": str,
         "JoinToken": str,
     },
 )
 
-CreateMeetingDialOutResponseTypeDef = TypedDict(
-    "CreateMeetingDialOutResponseTypeDef",
-    {
-        "TransactionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MeetingNotificationConfigurationTypeDef = TypedDict(
     "MeetingNotificationConfigurationTypeDef",
     {
         "SnsTopicArn": str,
         "SqsQueueArn": str,
     },
     total=False,
@@ -1733,21 +1725,14 @@
     "DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef",
     {
         "AccountId": str,
         "GroupNames": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEngineTranscribeMedicalSettingsTypeDef = TypedDict(
     "_RequiredEngineTranscribeMedicalSettingsTypeDef",
     {
         "LanguageCode": Literal["en-US"],
         "Specialty": TranscribeMedicalSpecialtyType,
         "Type": TranscribeMedicalTypeType,
     },
@@ -1912,23 +1897,14 @@
 GetPhoneNumberRequestRequestTypeDef = TypedDict(
     "GetPhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
-GetPhoneNumberSettingsResponseTypeDef = TypedDict(
-    "GetPhoneNumberSettingsResponseTypeDef",
-    {
-        "CallingName": str,
-        "CallingNameUpdatedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetProxySessionRequestRequestTypeDef = TypedDict(
     "GetProxySessionRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
         "ProxySessionId": str,
     },
 )
@@ -2081,16 +2057,16 @@
 GetVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-TerminationTypeDef = TypedDict(
-    "TerminationTypeDef",
+TerminationOutputTypeDef = TypedDict(
+    "TerminationOutputTypeDef",
     {
         "CpsLimit": int,
         "DefaultPhoneNumber": str,
         "CallingRegions": List[str],
         "CidrAllowedList": List[str],
         "Disabled": bool,
     },
@@ -2124,20 +2100,20 @@
 )
 
 class InviteUsersRequestRequestTypeDef(
     _RequiredInviteUsersRequestRequestTypeDef, _OptionalInviteUsersRequestRequestTypeDef
 ):
     pass
 
-ListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "ListAccountsRequestListAccountsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Name": str,
-        "UserEmail": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccountsRequestRequestTypeDef = TypedDict(
     "ListAccountsRequestRequestTypeDef",
     {
@@ -2299,39 +2275,15 @@
 
 class ListChannelMembershipsRequestRequestTypeDef(
     _RequiredListChannelMembershipsRequestRequestTypeDef,
     _OptionalListChannelMembershipsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
-    "_RequiredListChannelMessagesRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
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
-        "ChimeBearer": str,
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
     },
 )
 _OptionalListChannelModeratorsRequestRequestTypeDef = TypedDict(
@@ -2532,36 +2484,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "AccountId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "UserEmail": str,
-        "UserType": UserTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "AccountId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -2592,22 +2522,14 @@
 ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
-    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
-    {
-        "Usernames": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListVoiceConnectorsRequestRequestTypeDef = TypedDict(
     "ListVoiceConnectorsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -2665,24 +2587,14 @@
         "Protocol": OriginationRouteProtocolType,
         "Priority": int,
         "Weight": int,
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
 ParticipantTypeDef = TypedDict(
     "ParticipantTypeDef",
     {
         "PhoneNumber": str,
         "ProxyPhoneNumber": str,
     },
     total=False,
@@ -2752,14 +2664,26 @@
 
 class PutVoiceConnectorProxyRequestRequestTypeDef(
     _RequiredPutVoiceConnectorProxyRequestRequestTypeDef,
     _OptionalPutVoiceConnectorProxyRequestRequestTypeDef,
 ):
     pass
 
+TerminationTypeDef = TypedDict(
+    "TerminationTypeDef",
+    {
+        "CpsLimit": int,
+        "DefaultPhoneNumber": str,
+        "CallingRegions": Sequence[str],
+        "CidrAllowedList": Sequence[str],
+        "Disabled": bool,
+    },
+    total=False,
+)
+
 _RequiredRedactChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredRedactChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
     },
 )
@@ -2773,23 +2697,14 @@
 
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
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RedactConversationMessageRequestRequestTypeDef = TypedDict(
     "RedactConversationMessageRequestRequestTypeDef",
     {
         "AccountId": str,
         "ConversationId": str,
         "MessageId": str,
     },
@@ -2816,25 +2731,14 @@
     "ResetPersonalPINRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
     },
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
 RestorePhoneNumberRequestRequestTypeDef = TypedDict(
     "RestorePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 
@@ -2857,21 +2761,21 @@
         "PhoneNumberType": PhoneNumberTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
-    "SearchAvailablePhoneNumbersResponseTypeDef",
+SelectedVideoStreamsOutputTypeDef = TypedDict(
+    "SelectedVideoStreamsOutputTypeDef",
     {
-        "E164PhoneNumbers": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AttendeeIds": List[str],
+        "ExternalUserIds": List[str],
     },
+    total=False,
 )
 
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
@@ -2900,23 +2804,14 @@
 
 class SendChannelMessageRequestRequestTypeDef(
     _RequiredSendChannelMessageRequestRequestTypeDef,
     _OptionalSendChannelMessageRequestRequestTypeDef,
 ):
     pass
 
-SendChannelMessageResponseTypeDef = TypedDict(
-    "SendChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
@@ -2997,22 +2892,14 @@
 )
 
 class UpdateAppInstanceRequestRequestTypeDef(
     _RequiredUpdateAppInstanceRequestRequestTypeDef, _OptionalUpdateAppInstanceRequestRequestTypeDef
 ):
     pass
 
-UpdateAppInstanceResponseTypeDef = TypedDict(
-    "UpdateAppInstanceResponseTypeDef",
-    {
-        "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateAppInstanceUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppInstanceUserRequestRequestTypeDef",
     {
         "AppInstanceUserArn": str,
         "Name": str,
     },
 )
@@ -3026,22 +2913,14 @@
 
 class UpdateAppInstanceUserRequestRequestTypeDef(
     _RequiredUpdateAppInstanceUserRequestRequestTypeDef,
     _OptionalUpdateAppInstanceUserRequestRequestTypeDef,
 ):
     pass
 
-UpdateAppInstanceUserResponseTypeDef = TypedDict(
-    "UpdateAppInstanceUserResponseTypeDef",
-    {
-        "AppInstanceUserArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateBotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBotRequestRequestTypeDef",
     {
         "AccountId": str,
         "BotId": str,
     },
 )
@@ -3077,23 +2956,14 @@
 
 class UpdateChannelMessageRequestRequestTypeDef(
     _RequiredUpdateChannelMessageRequestRequestTypeDef,
     _OptionalUpdateChannelMessageRequestRequestTypeDef,
 ):
     pass
 
-UpdateChannelMessageResponseTypeDef = TypedDict(
-    "UpdateChannelMessageResponseTypeDef",
-    {
-        "ChannelArn": str,
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelReadMarkerRequestRequestTypeDef",
     {
         "ChannelArn": str,
     },
 )
 _OptionalUpdateChannelReadMarkerRequestRequestTypeDef = TypedDict(
@@ -3106,22 +2976,14 @@
 
 class UpdateChannelReadMarkerRequestRequestTypeDef(
     _RequiredUpdateChannelReadMarkerRequestRequestTypeDef,
     _OptionalUpdateChannelReadMarkerRequestRequestTypeDef,
 ):
     pass
 
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
         "Name": str,
         "Mode": ChannelModeType,
     },
@@ -3136,22 +2998,14 @@
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
 _RequiredUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePhoneNumberRequestRequestTypeDef",
     {
         "PhoneNumberId": str,
     },
 )
 _OptionalUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
@@ -3266,22 +3120,14 @@
         "City": str,
         "State": str,
         "Country": str,
         "PostalCode": str,
     },
 )
 
-GetAccountSettingsResponseTypeDef = TypedDict(
-    "GetAccountSettingsResponseTypeDef",
-    {
-        "AccountSettings": AccountSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAccountSettingsRequestRequestTypeDef = TypedDict(
     "UpdateAccountSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "AccountSettings": AccountSettingsTypeDef,
     },
 )
@@ -3523,205 +3369,337 @@
         "CreatedTimestamp": datetime,
         "LastMessageTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+AppInstanceRetentionSettingsTypeDef = TypedDict(
+    "AppInstanceRetentionSettingsTypeDef",
+    {
+        "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
+    },
+    total=False,
+)
+
+PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
+    {
+        "AppInstanceArn": str,
+        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
+    },
+)
+
+ArtifactsConfigurationTypeDef = TypedDict(
+    "ArtifactsConfigurationTypeDef",
+    {
+        "Audio": AudioArtifactsConfigurationTypeDef,
+        "Video": VideoArtifactsConfigurationTypeDef,
+        "Content": ContentArtifactsConfigurationTypeDef,
+    },
+)
+
+AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
+    "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchDeletePhoneNumberResponseTypeDef = TypedDict(
+    "BatchDeletePhoneNumberResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
+    "BatchUpdatePhoneNumberResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateAppInstanceAdminResponseTypeDef = TypedDict(
     "CreateAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": IdentityTypeDef,
         "AppInstanceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceResponseTypeDef = TypedDict(
+    "CreateAppInstanceResponseTypeDef",
+    {
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAppInstanceUserResponseTypeDef = TypedDict(
+    "CreateAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelBanResponseTypeDef = TypedDict(
     "CreateChannelBanResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateChannelMembershipResponseTypeDef = TypedDict(
     "CreateChannelMembershipResponseTypeDef",
     {
         "ChannelArn": str,
         "Member": IdentityTypeDef,
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
     },
 )
 
-AppInstanceRetentionSettingsTypeDef = TypedDict(
-    "AppInstanceRetentionSettingsTypeDef",
+CreateChannelResponseTypeDef = TypedDict(
+    "CreateChannelResponseTypeDef",
     {
-        "ChannelRetentionSettings": ChannelRetentionSettingsTypeDef,
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMeetingDialOutResponseTypeDef = TypedDict(
+    "CreateMeetingDialOutResponseTypeDef",
+    {
+        "TransactionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppInstanceResponseTypeDef = TypedDict(
+    "DescribeAppInstanceResponseTypeDef",
+    {
+        "AppInstance": AppInstanceTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAppInstanceUserResponseTypeDef = TypedDict(
+    "DescribeAppInstanceUserResponseTypeDef",
+    {
+        "AppInstanceUser": AppInstanceUserTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
+    "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
+    "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
+    {
+        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
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
+GetAccountSettingsResponseTypeDef = TypedDict(
+    "GetAccountSettingsResponseTypeDef",
+    {
+        "AccountSettings": AccountSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
     "GetAppInstanceStreamingConfigurationsResponseTypeDef",
     {
         "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppInstanceStreamingConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsRequestRequestTypeDef",
+GetPhoneNumberSettingsResponseTypeDef = TypedDict(
+    "GetPhoneNumberSettingsResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "AppInstanceStreamingConfigurations": Sequence[AppInstanceStreamingConfigurationTypeDef],
+        "CallingName": str,
+        "CallingNameUpdatedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
-    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
+ListAppInstanceUsersResponseTypeDef = TypedDict(
+    "ListAppInstanceUsersResponseTypeDef",
     {
-        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceArn": str,
+        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppInstancesResponseTypeDef = TypedDict(
     "ListAppInstancesResponseTypeDef",
     {
         "AppInstances": List[AppInstanceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAppInstanceResponseTypeDef = TypedDict(
-    "DescribeAppInstanceResponseTypeDef",
+ListVoiceConnectorTerminationCredentialsResponseTypeDef = TypedDict(
+    "ListVoiceConnectorTerminationCredentialsResponseTypeDef",
     {
-        "AppInstance": AppInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Usernames": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListAppInstanceUsersResponseTypeDef = TypedDict(
-    "ListAppInstanceUsersResponseTypeDef",
+PutAppInstanceStreamingConfigurationsResponseTypeDef = TypedDict(
+    "PutAppInstanceStreamingConfigurationsResponseTypeDef",
     {
-        "AppInstanceArn": str,
-        "AppInstanceUsers": List[AppInstanceUserSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceStreamingConfigurations": List[AppInstanceStreamingConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAppInstanceUserResponseTypeDef = TypedDict(
-    "DescribeAppInstanceUserResponseTypeDef",
+RedactChannelMessageResponseTypeDef = TypedDict(
+    "RedactChannelMessageResponseTypeDef",
     {
-        "AppInstanceUser": AppInstanceUserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ArtifactsConfigurationTypeDef = TypedDict(
-    "ArtifactsConfigurationTypeDef",
+SearchAvailablePhoneNumbersResponseTypeDef = TypedDict(
+    "SearchAvailablePhoneNumbersResponseTypeDef",
     {
-        "Audio": AudioArtifactsConfigurationTypeDef,
-        "Video": VideoArtifactsConfigurationTypeDef,
-        "Content": ContentArtifactsConfigurationTypeDef,
+        "E164PhoneNumbers": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef",
+SendChannelMessageResponseTypeDef = TypedDict(
+    "SendChannelMessageResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = TypedDict(
-    "AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef",
+UpdateAppInstanceResponseTypeDef = TypedDict(
+    "UpdateAppInstanceResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchDeletePhoneNumberResponseTypeDef = TypedDict(
-    "BatchDeletePhoneNumberResponseTypeDef",
+UpdateAppInstanceUserResponseTypeDef = TypedDict(
+    "UpdateAppInstanceUserResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppInstanceUserArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchUpdatePhoneNumberResponseTypeDef = TypedDict(
-    "BatchUpdatePhoneNumberResponseTypeDef",
+UpdateChannelMessageResponseTypeDef = TypedDict(
+    "UpdateChannelMessageResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef = TypedDict(
-    "DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef",
+UpdateChannelReadMarkerResponseTypeDef = TypedDict(
+    "UpdateChannelReadMarkerResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef = TypedDict(
-    "DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef",
+UpdateChannelResponseTypeDef = TypedDict(
+    "UpdateChannelResponseTypeDef",
     {
-        "PhoneNumberErrors": List[PhoneNumberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ChannelArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAttendeeResponseTypeDef = TypedDict(
     "CreateAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAttendeeResponseTypeDef = TypedDict(
     "GetAttendeeResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttendeesResponseTypeDef = TypedDict(
     "ListAttendeesResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateAttendeeResponseTypeDef = TypedDict(
     "BatchCreateAttendeeResponseTypeDef",
     {
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateRoomMembershipRequestRequestTypeDef = TypedDict(
     "BatchCreateRoomMembershipRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -3730,98 +3708,98 @@
     },
 )
 
 BatchCreateRoomMembershipResponseTypeDef = TypedDict(
     "BatchCreateRoomMembershipResponseTypeDef",
     {
         "Errors": List[MemberErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchSuspendUserResponseTypeDef = TypedDict(
     "BatchSuspendUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUnsuspendUserResponseTypeDef = TypedDict(
     "BatchUnsuspendUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateUserResponseTypeDef = TypedDict(
     "BatchUpdateUserResponseTypeDef",
     {
         "UserErrors": List[UserErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdatePhoneNumberRequestRequestTypeDef = TypedDict(
     "BatchUpdatePhoneNumberRequestRequestTypeDef",
     {
         "UpdatePhoneNumberRequestItems": Sequence[UpdatePhoneNumberRequestItemTypeDef],
     },
 )
 
 CreateBotResponseTypeDef = TypedDict(
     "CreateBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBotResponseTypeDef = TypedDict(
     "GetBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBotsResponseTypeDef = TypedDict(
     "ListBotsResponseTypeDef",
     {
         "Bots": List[BotTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegenerateSecurityTokenResponseTypeDef = TypedDict(
     "RegenerateSecurityTokenResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBotResponseTypeDef = TypedDict(
     "UpdateBotResponseTypeDef",
     {
         "Bot": BotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidateE911AddressResponseTypeDef = TypedDict(
     "ValidateE911AddressResponseTypeDef",
     {
         "ValidationResult": int,
         "AddressExternalId": str,
         "Address": AddressTypeDef,
         "CandidateAddressList": List[CandidateAddressTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChannelMembershipForAppInstanceUserSummaryTypeDef = TypedDict(
     "ChannelMembershipForAppInstanceUserSummaryTypeDef",
     {
         "ChannelSummary": ChannelSummaryTypeDef,
@@ -3839,15 +3817,15 @@
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
 
 _RequiredCreateAppInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppInstanceRequestRequestTypeDef",
     {
         "Name": str,
@@ -3956,31 +3934,31 @@
 ):
     pass
 
 ListAttendeeTagsResponseTypeDef = TypedDict(
     "ListAttendeeTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMeetingTagsResponseTypeDef = TypedDict(
     "ListMeetingTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagAttendeeRequestRequestTypeDef = TypedDict(
     "TagAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -4054,56 +4032,56 @@
 ):
     pass
 
 CreateRoomResponseTypeDef = TypedDict(
     "CreateRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoomResponseTypeDef = TypedDict(
     "GetRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoomsResponseTypeDef = TypedDict(
     "ListRoomsResponseTypeDef",
     {
         "Rooms": List[RoomTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRoomResponseTypeDef = TypedDict(
     "UpdateRoomResponseTypeDef",
     {
         "Room": RoomTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSipMediaApplicationCallResponseTypeDef = TypedDict(
     "CreateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSipMediaApplicationCallResponseTypeDef = TypedDict(
     "UpdateSipMediaApplicationCallResponseTypeDef",
     {
         "SipMediaApplicationCall": SipMediaApplicationCallTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSipMediaApplicationRequestRequestTypeDef = TypedDict(
     "CreateSipMediaApplicationRequestRequestTypeDef",
     {
         "AwsRegion": str,
@@ -4246,40 +4224,40 @@
     total=False,
 )
 
 CreateVoiceConnectorResponseTypeDef = TypedDict(
     "CreateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorResponseTypeDef = TypedDict(
     "GetVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVoiceConnectorsResponseTypeDef = TypedDict(
     "ListVoiceConnectorsResponseTypeDef",
     {
         "VoiceConnectors": List[VoiceConnectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceConnectorResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorResponseTypeDef",
     {
         "VoiceConnector": VoiceConnectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = TypedDict(
     "_RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -4295,18 +4273,26 @@
 
 class PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef(
     _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
 ):
     pass
 
+EmergencyCallingConfigurationOutputTypeDef = TypedDict(
+    "EmergencyCallingConfigurationOutputTypeDef",
+    {
+        "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
+    },
+    total=False,
+)
+
 EmergencyCallingConfigurationTypeDef = TypedDict(
     "EmergencyCallingConfigurationTypeDef",
     {
-        "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
+        "DNIS": Sequence[DNISEmergencyCallingConfigurationTypeDef],
     },
     total=False,
 )
 
 TranscriptionConfigurationTypeDef = TypedDict(
     "TranscriptionConfigurationTypeDef",
     {
@@ -4316,32 +4302,32 @@
     total=False,
 )
 
 GetEventsConfigurationResponseTypeDef = TypedDict(
     "GetEventsConfigurationResponseTypeDef",
     {
         "EventsConfiguration": EventsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEventsConfigurationResponseTypeDef = TypedDict(
     "PutEventsConfigurationResponseTypeDef",
     {
         "EventsConfiguration": EventsConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGlobalSettingsResponseTypeDef = TypedDict(
     "GetGlobalSettingsResponseTypeDef",
     {
         "BusinessCalling": BusinessCallingSettingsTypeDef,
         "VoiceConnector": VoiceConnectorSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalSettingsRequestRequestTypeDef = TypedDict(
     "UpdateGlobalSettingsRequestRequestTypeDef",
     {
         "BusinessCalling": BusinessCallingSettingsTypeDef,
@@ -4350,23 +4336,23 @@
     total=False,
 )
 
 GetMessagingSessionEndpointResponseTypeDef = TypedDict(
     "GetMessagingSessionEndpointResponseTypeDef",
     {
         "Endpoint": MessagingSessionEndpointTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
         "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredPutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef",
     {
         "SipMediaApplicationId": str,
@@ -4386,23 +4372,23 @@
 ):
     pass
 
 PutSipMediaApplicationLoggingConfigurationResponseTypeDef = TypedDict(
     "PutSipMediaApplicationLoggingConfigurationResponseTypeDef",
     {
         "SipMediaApplicationLoggingConfiguration": SipMediaApplicationLoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
@@ -4410,79 +4396,128 @@
     },
 )
 
 PutVoiceConnectorLoggingConfigurationResponseTypeDef = TypedDict(
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     {
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorProxyResponseTypeDef = TypedDict(
     "GetVoiceConnectorProxyResponseTypeDef",
     {
         "Proxy": ProxyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorProxyResponseTypeDef = TypedDict(
     "PutVoiceConnectorProxyResponseTypeDef",
     {
         "Proxy": ProxyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorTerminationHealthResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     {
         "TerminationHealth": TerminationHealthTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "Termination": TerminationTypeDef,
+        "Termination": TerminationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "PutVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Termination": TerminationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InviteUsersResponseTypeDef = TypedDict(
     "InviteUsersResponseTypeDef",
     {
         "Invites": List[InviteTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "ListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "Name": str,
+        "UserEmail": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "AccountId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "UserEmail": str,
+        "UserType": UserTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+_RequiredListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_RequiredListChannelMessagesRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
     },
 )
+_OptionalListChannelMessagesRequestRequestTypeDef = TypedDict(
+    "_OptionalListChannelMessagesRequestRequestTypeDef",
+    {
+        "SortOrder": SortOrderType,
+        "NotBefore": TimestampTypeDef,
+        "NotAfter": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "ChimeBearer": str,
+    },
+    total=False,
+)
+
+class ListChannelMessagesRequestRequestTypeDef(
+    _RequiredListChannelMessagesRequestRequestTypeDef,
+    _OptionalListChannelMessagesRequestRequestTypeDef,
+):
+    pass
 
 ListSupportedPhoneNumberCountriesResponseTypeDef = TypedDict(
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     {
         "PhoneNumberCountries": List[PhoneNumberCountryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MeetingTypeDef = TypedDict(
     "MeetingTypeDef",
     {
         "MeetingId": str,
@@ -4514,18 +4549,27 @@
         "OrderedPhoneNumbers": List[OrderedPhoneNumberTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
+OriginationOutputTypeDef = TypedDict(
+    "OriginationOutputTypeDef",
+    {
+        "Routes": List[OriginationRouteTypeDef],
+        "Disabled": bool,
+    },
+    total=False,
+)
+
 OriginationTypeDef = TypedDict(
     "OriginationTypeDef",
     {
-        "Routes": List[OriginationRouteTypeDef],
+        "Routes": Sequence[OriginationRouteTypeDef],
         "Disabled": bool,
     },
     total=False,
 )
 
 ProxySessionTypeDef = TypedDict(
     "ProxySessionTypeDef",
@@ -4563,42 +4607,79 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "DeletionTimestamp": datetime,
     },
     total=False,
 )
 
+PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "Termination": TerminationTypeDef,
+    },
+)
+
+TerminationUnionTypeDef = Union[TerminationTypeDef, TerminationOutputTypeDef]
 RetentionSettingsTypeDef = TypedDict(
     "RetentionSettingsTypeDef",
     {
         "RoomRetentionSettings": RoomRetentionSettingsTypeDef,
         "ConversationRetentionSettings": ConversationRetentionSettingsTypeDef,
     },
     total=False,
 )
 
+SourceConfigurationOutputTypeDef = TypedDict(
+    "SourceConfigurationOutputTypeDef",
+    {
+        "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
+_RequiredStreamingConfigurationOutputTypeDef = TypedDict(
+    "_RequiredStreamingConfigurationOutputTypeDef",
+    {
+        "DataRetentionInHours": int,
+    },
+)
+_OptionalStreamingConfigurationOutputTypeDef = TypedDict(
+    "_OptionalStreamingConfigurationOutputTypeDef",
+    {
+        "Disabled": bool,
+        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
+    },
+    total=False,
+)
+
+class StreamingConfigurationOutputTypeDef(
+    _RequiredStreamingConfigurationOutputTypeDef, _OptionalStreamingConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredStreamingConfigurationTypeDef = TypedDict(
     "_RequiredStreamingConfigurationTypeDef",
     {
         "DataRetentionInHours": int,
     },
 )
 _OptionalStreamingConfigurationTypeDef = TypedDict(
     "_OptionalStreamingConfigurationTypeDef",
     {
         "Disabled": bool,
-        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
+        "StreamingNotificationTargets": Sequence[StreamingNotificationTargetTypeDef],
     },
     total=False,
 )
 
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
 ):
@@ -4611,40 +4692,40 @@
     },
 )
 
 CreateAccountResponseTypeDef = TypedDict(
     "CreateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccountsResponseTypeDef = TypedDict(
     "ListAccountsResponseTypeDef",
     {
         "Accounts": List[AccountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountResponseTypeDef = TypedDict(
     "UpdateAccountResponseTypeDef",
     {
         "Account": AccountTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateUserRequestRequestTypeDef = TypedDict(
     "BatchUpdateUserRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -4652,164 +4733,164 @@
     },
 )
 
 CreateUserResponseTypeDef = TypedDict(
     "CreateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserResponseTypeDef = TypedDict(
     "GetUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetPersonalPINResponseTypeDef = TypedDict(
     "ResetPersonalPINResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "User": UserTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppInstanceAdminsResponseTypeDef = TypedDict(
     "ListAppInstanceAdminsResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceAdmins": List[AppInstanceAdminSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAppInstanceAdminResponseTypeDef = TypedDict(
     "DescribeAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": AppInstanceAdminTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
 
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
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
 
 DescribeChannelResponseTypeDef = TypedDict(
     "DescribeChannelResponseTypeDef",
     {
         "Channel": ChannelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     {
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
     "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
@@ -4818,49 +4899,49 @@
 )
 
 PutAppInstanceRetentionSettingsResponseTypeDef = TypedDict(
     "PutAppInstanceRetentionSettingsResponseTypeDef",
     {
         "AppInstanceRetentionSettings": AppInstanceRetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
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
 
 BatchCreateAttendeeRequestRequestTypeDef = TypedDict(
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -4893,130 +4974,133 @@
 ):
     pass
 
 CreateSipMediaApplicationResponseTypeDef = TypedDict(
     "CreateSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSipMediaApplicationResponseTypeDef = TypedDict(
     "GetSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSipMediaApplicationsResponseTypeDef = TypedDict(
     "ListSipMediaApplicationsResponseTypeDef",
     {
         "SipMediaApplications": List[SipMediaApplicationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSipMediaApplicationResponseTypeDef = TypedDict(
     "UpdateSipMediaApplicationResponseTypeDef",
     {
         "SipMediaApplication": SipMediaApplicationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSipRuleResponseTypeDef = TypedDict(
     "CreateSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSipRuleResponseTypeDef = TypedDict(
     "GetSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSipRulesResponseTypeDef = TypedDict(
     "ListSipRulesResponseTypeDef",
     {
         "SipRules": List[SipRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSipRuleResponseTypeDef = TypedDict(
     "UpdateSipRuleResponseTypeDef",
     {
         "SipRule": SipRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVoiceConnectorGroupResponseTypeDef = TypedDict(
     "CreateVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorGroupResponseTypeDef = TypedDict(
     "GetVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVoiceConnectorGroupsResponseTypeDef = TypedDict(
     "ListVoiceConnectorGroupsResponseTypeDef",
     {
         "VoiceConnectorGroups": List[VoiceConnectorGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVoiceConnectorGroupResponseTypeDef = TypedDict(
     "UpdateVoiceConnectorGroupResponseTypeDef",
     {
         "VoiceConnectorGroup": VoiceConnectorGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
+PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+EmergencyCallingConfigurationUnionTypeDef = Union[
+    EmergencyCallingConfigurationTypeDef, EmergencyCallingConfigurationOutputTypeDef
+]
+PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 StartMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StartMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -5024,191 +5108,192 @@
     },
 )
 
 CreateMeetingResponseTypeDef = TypedDict(
     "CreateMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMeetingWithAttendeesResponseTypeDef = TypedDict(
     "CreateMeetingWithAttendeesResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
         "Attendees": List[AttendeeTypeDef],
         "Errors": List[CreateAttendeeErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMeetingResponseTypeDef = TypedDict(
     "GetMeetingResponseTypeDef",
     {
         "Meeting": MeetingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMeetingsResponseTypeDef = TypedDict(
     "ListMeetingsResponseTypeDef",
     {
         "Meetings": List[MeetingTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRoomMembershipResponseTypeDef = TypedDict(
     "CreateRoomMembershipResponseTypeDef",
     {
         "RoomMembership": RoomMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoomMembershipsResponseTypeDef = TypedDict(
     "ListRoomMembershipsResponseTypeDef",
     {
         "RoomMemberships": List[RoomMembershipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRoomMembershipResponseTypeDef = TypedDict(
     "UpdateRoomMembershipResponseTypeDef",
     {
         "RoomMembership": RoomMembershipTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePhoneNumberOrderResponseTypeDef = TypedDict(
     "CreatePhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPhoneNumberOrderResponseTypeDef = TypedDict(
     "GetPhoneNumberOrderResponseTypeDef",
     {
         "PhoneNumberOrder": PhoneNumberOrderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPhoneNumberOrdersResponseTypeDef = TypedDict(
     "ListPhoneNumberOrdersResponseTypeDef",
     {
         "PhoneNumberOrders": List[PhoneNumberOrderTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "GetVoiceConnectorOriginationResponseTypeDef",
     {
-        "Origination": OriginationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Origination": OriginationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
+PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "Origination": OriginationTypeDef,
+        "Origination": OriginationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationResponseTypeDef",
+OriginationUnionTypeDef = Union[OriginationTypeDef, OriginationOutputTypeDef]
+PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "Origination": OriginationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CreateProxySessionResponseTypeDef = TypedDict(
     "CreateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetProxySessionResponseTypeDef = TypedDict(
     "GetProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProxySessionsResponseTypeDef = TypedDict(
     "ListProxySessionsResponseTypeDef",
     {
         "ProxySessions": List[ProxySessionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProxySessionResponseTypeDef = TypedDict(
     "UpdateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPhoneNumberResponseTypeDef = TypedDict(
     "GetPhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPhoneNumbersResponseTypeDef = TypedDict(
     "ListPhoneNumbersResponseTypeDef",
     {
         "PhoneNumbers": List[PhoneNumberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestorePhoneNumberResponseTypeDef = TypedDict(
     "RestorePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePhoneNumberResponseTypeDef = TypedDict(
     "UpdatePhoneNumberResponseTypeDef",
     {
         "PhoneNumber": PhoneNumberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRetentionSettingsResponseTypeDef = TypedDict(
     "GetRetentionSettingsResponseTypeDef",
     {
         "RetentionSettings": RetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRetentionSettingsRequestRequestTypeDef = TypedDict(
     "PutRetentionSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
@@ -5217,68 +5302,99 @@
 )
 
 PutRetentionSettingsResponseTypeDef = TypedDict(
     "PutRetentionSettingsResponseTypeDef",
     {
         "RetentionSettings": RetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
+    "ChimeSdkMeetingConfigurationOutputTypeDef",
+    {
+        "SourceConfiguration": SourceConfigurationOutputTypeDef,
+        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
+    total=False,
 )
 
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
-        "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
+        "VoiceConnectorId": str,
         "StreamingConfiguration": StreamingConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+StreamingConfigurationUnionTypeDef = Union[
+    StreamingConfigurationTypeDef, StreamingConfigurationOutputTypeDef
+]
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "UserSettings": UserSettingsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserSettingsRequestRequestTypeDef = TypedDict(
     "UpdateUserSettingsRequestRequestTypeDef",
     {
         "AccountId": str,
         "UserId": str,
         "UserSettings": UserSettingsTypeDef,
     },
 )
 
+MediaCapturePipelineTypeDef = TypedDict(
+    "MediaCapturePipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "SourceArn": str,
+        "Status": MediaPipelineStatusType,
+        "SinkType": Literal["S3Bucket"],
+        "SinkArn": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+ChimeSdkMeetingConfigurationUnionTypeDef = Union[
+    ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
+]
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
@@ -5295,47 +5411,31 @@
 
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
-MediaCapturePipelineTypeDef = TypedDict(
-    "MediaCapturePipelineTypeDef",
-    {
-        "MediaPipelineId": str,
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "SourceArn": str,
-        "Status": MediaPipelineStatusType,
-        "SinkType": Literal["S3Bucket"],
-        "SinkArn": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
-    },
-    total=False,
-)
-
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMediaCapturePipelineResponseTypeDef = TypedDict(
     "GetMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMediaCapturePipelinesResponseTypeDef = TypedDict(
     "ListMediaCapturePipelinesResponseTypeDef",
     {
         "MediaCapturePipelines": List[MediaCapturePipelineTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime.egg-info/PKG-INFO` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Chime 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Chime 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore chime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore chime type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime"></a>
 
 # types-aiobotocore-chime
 
 [![PyPI - types-aiobotocore-chime](https://img.shields.io/pypi/v/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime)](https://pepy.tech/project/types-aiobotocore-chime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Chime 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime)
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
 [types-aiobotocore-chime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/).
 
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
@@ -355,20 +354,20 @@
 )
 
 
 def check_value(value: AccountStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_chime.type_defs import (
     AccountSettingsTypeDef,
     SigninDelegateGroupTypeDef,
     AddressTypeDef,
     AlexaForBusinessMetadataTypeDef,
@@ -382,14 +381,15 @@
     AppInstanceUserTypeDef,
     AudioArtifactsConfigurationTypeDef,
     ContentArtifactsConfigurationTypeDef,
     VideoArtifactsConfigurationTypeDef,
     AssociatePhoneNumberWithUserRequestRequestTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef,
     PhoneNumberErrorTypeDef,
+    ResponseMetadataTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeErrorTypeDef,
     BatchCreateChannelMembershipErrorTypeDef,
     BatchCreateChannelMembershipRequestRequestTypeDef,
     MembershipItemTypeDef,
     MemberErrorTypeDef,
@@ -402,23 +402,19 @@
     BusinessCallingSettingsTypeDef,
     CandidateAddressTypeDef,
     ChannelSummaryTypeDef,
     ConversationRetentionSettingsTypeDef,
     CreateAccountRequestRequestTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     TagTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
     CreateBotRequestRequestTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
-    CreateChannelResponseTypeDef,
     CreateMeetingDialOutRequestRequestTypeDef,
-    CreateMeetingDialOutResponseTypeDef,
     MeetingNotificationConfigurationTypeDef,
     CreatePhoneNumberOrderRequestRequestTypeDef,
     GeoMatchParamsTypeDef,
     CreateRoomMembershipRequestRequestTypeDef,
     CreateRoomRequestRequestTypeDef,
     RoomTypeDef,
     CreateSipMediaApplicationCallRequestRequestTypeDef,
@@ -468,15 +464,14 @@
     DescribeChannelModeratedByAppInstanceUserRequestRequestTypeDef,
     DescribeChannelModeratorRequestRequestTypeDef,
     DescribeChannelRequestRequestTypeDef,
     DisassociatePhoneNumberFromUserRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef,
     DisassociateSigninDelegateGroupsFromAccountRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     EventsConfigurationTypeDef,
     GetAccountRequestRequestTypeDef,
     GetAccountSettingsRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
     GetAppInstanceStreamingConfigurationsRequestRequestTypeDef,
@@ -486,15 +481,14 @@
     GetEventsConfigurationRequestRequestTypeDef,
     VoiceConnectorSettingsTypeDef,
     GetMediaCapturePipelineRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     MessagingSessionEndpointTypeDef,
     GetPhoneNumberOrderRequestRequestTypeDef,
     GetPhoneNumberRequestRequestTypeDef,
-    GetPhoneNumberSettingsResponseTypeDef,
     GetProxySessionRequestRequestTypeDef,
     GetRetentionSettingsRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     GetSipMediaApplicationRequestRequestTypeDef,
     GetSipRuleRequestRequestTypeDef,
@@ -508,29 +502,29 @@
     GetVoiceConnectorProxyRequestRequestTypeDef,
     ProxyTypeDef,
     GetVoiceConnectorRequestRequestTypeDef,
     GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     GetVoiceConnectorTerminationHealthRequestRequestTypeDef,
     TerminationHealthTypeDef,
     GetVoiceConnectorTerminationRequestRequestTypeDef,
-    TerminationTypeDef,
+    TerminationOutputTypeDef,
     InviteTypeDef,
     InviteUsersRequestRequestTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountsRequestRequestTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListAttendeeTagsRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListBotsRequestRequestTypeDef,
     ListChannelBansRequestRequestTypeDef,
     ListChannelMembershipsForAppInstanceUserRequestRequestTypeDef,
     ListChannelMembershipsRequestRequestTypeDef,
-    ListChannelMessagesRequestRequestTypeDef,
+    TimestampTypeDef,
     ListChannelModeratorsRequestRequestTypeDef,
     ListChannelsModeratedByAppInstanceUserRequestRequestTypeDef,
     ListChannelsRequestRequestTypeDef,
     ListMediaCapturePipelinesRequestRequestTypeDef,
     ListMeetingTagsRequestRequestTypeDef,
     ListMeetingsRequestRequestTypeDef,
     ListPhoneNumberOrdersRequestRequestTypeDef,
@@ -539,72 +533,61 @@
     ListRoomMembershipsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListSipMediaApplicationsRequestRequestTypeDef,
     ListSipRulesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesRequestRequestTypeDef,
     PhoneNumberCountryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVoiceConnectorGroupsRequestRequestTypeDef,
     ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
-    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     ListVoiceConnectorsRequestRequestTypeDef,
     LogoutUserRequestRequestTypeDef,
     MediaPlacementTypeDef,
     MemberTypeDef,
     OrderedPhoneNumberTypeDef,
     OriginationRouteTypeDef,
-    PaginatorConfigTypeDef,
     ParticipantTypeDef,
     PhoneNumberAssociationTypeDef,
     PhoneNumberCapabilitiesTypeDef,
     PutEventsConfigurationRequestRequestTypeDef,
     PutVoiceConnectorProxyRequestRequestTypeDef,
+    TerminationTypeDef,
     RedactChannelMessageRequestRequestTypeDef,
-    RedactChannelMessageResponseTypeDef,
     RedactConversationMessageRequestRequestTypeDef,
     RedactRoomMessageRequestRequestTypeDef,
     RegenerateSecurityTokenRequestRequestTypeDef,
     ResetPersonalPINRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestorePhoneNumberRequestRequestTypeDef,
     RoomRetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersRequestRequestTypeDef,
-    SearchAvailablePhoneNumbersResponseTypeDef,
+    SelectedVideoStreamsOutputTypeDef,
     SelectedVideoStreamsTypeDef,
     SendChannelMessageRequestRequestTypeDef,
-    SendChannelMessageResponseTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     StreamingNotificationTargetTypeDef,
     TelephonySettingsTypeDef,
     UntagAttendeeRequestRequestTypeDef,
     UntagMeetingRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccountRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
-    UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
     UpdateBotRequestRequestTypeDef,
     UpdateChannelMessageRequestRequestTypeDef,
-    UpdateChannelMessageResponseTypeDef,
     UpdateChannelReadMarkerRequestRequestTypeDef,
-    UpdateChannelReadMarkerResponseTypeDef,
     UpdateChannelRequestRequestTypeDef,
-    UpdateChannelResponseTypeDef,
     UpdatePhoneNumberRequestRequestTypeDef,
     UpdatePhoneNumberSettingsRequestRequestTypeDef,
     UpdateProxySessionRequestRequestTypeDef,
     UpdateRoomMembershipRequestRequestTypeDef,
     UpdateRoomRequestRequestTypeDef,
     UpdateSipMediaApplicationCallRequestRequestTypeDef,
     UpdateVoiceConnectorRequestRequestTypeDef,
     ValidateE911AddressRequestRequestTypeDef,
-    GetAccountSettingsResponseTypeDef,
     UpdateAccountSettingsRequestRequestTypeDef,
     AccountTypeDef,
     AssociateSigninDelegateGroupsWithAccountRequestRequestTypeDef,
     UpdateUserRequestItemTypeDef,
     UpdateUserRequestRequestTypeDef,
     UserTypeDef,
     AppInstanceAdminSummaryTypeDef,
@@ -615,33 +598,49 @@
     ChannelMembershipSummaryTypeDef,
     ChannelMembershipTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
     ChannelModeratorSummaryTypeDef,
     ChannelModeratorTypeDef,
     ChannelTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateChannelBanResponseTypeDef,
-    CreateChannelMembershipResponseTypeDef,
-    CreateChannelModeratorResponseTypeDef,
     AppInstanceRetentionSettingsTypeDef,
-    GetAppInstanceStreamingConfigurationsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsRequestRequestTypeDef,
-    PutAppInstanceStreamingConfigurationsResponseTypeDef,
-    ListAppInstancesResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    DescribeAppInstanceUserResponseTypeDef,
     ArtifactsConfigurationTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef,
     AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
+    CreateAppInstanceAdminResponseTypeDef,
+    CreateAppInstanceResponseTypeDef,
+    CreateAppInstanceUserResponseTypeDef,
+    CreateChannelBanResponseTypeDef,
+    CreateChannelMembershipResponseTypeDef,
+    CreateChannelModeratorResponseTypeDef,
+    CreateChannelResponseTypeDef,
+    CreateMeetingDialOutResponseTypeDef,
+    DescribeAppInstanceResponseTypeDef,
+    DescribeAppInstanceUserResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAccountSettingsResponseTypeDef,
+    GetAppInstanceStreamingConfigurationsResponseTypeDef,
+    GetPhoneNumberSettingsResponseTypeDef,
+    ListAppInstanceUsersResponseTypeDef,
+    ListAppInstancesResponseTypeDef,
+    ListVoiceConnectorTerminationCredentialsResponseTypeDef,
+    PutAppInstanceStreamingConfigurationsResponseTypeDef,
+    RedactChannelMessageResponseTypeDef,
+    SearchAvailablePhoneNumbersResponseTypeDef,
+    SendChannelMessageResponseTypeDef,
+    UpdateAppInstanceResponseTypeDef,
+    UpdateAppInstanceUserResponseTypeDef,
+    UpdateChannelMessageResponseTypeDef,
+    UpdateChannelReadMarkerResponseTypeDef,
+    UpdateChannelResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     BatchCreateRoomMembershipRequestRequestTypeDef,
     BatchCreateRoomMembershipResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
@@ -686,14 +685,15 @@
     UpdateVoiceConnectorGroupRequestRequestTypeDef,
     VoiceConnectorGroupTypeDef,
     CreateVoiceConnectorResponseTypeDef,
     GetVoiceConnectorResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     UpdateVoiceConnectorResponseTypeDef,
     PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
+    EmergencyCallingConfigurationOutputTypeDef,
     EmergencyCallingConfigurationTypeDef,
     TranscriptionConfigurationTypeDef,
     GetEventsConfigurationResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     GetGlobalSettingsResponseTypeDef,
     UpdateGlobalSettingsRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
@@ -703,26 +703,33 @@
     GetVoiceConnectorLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
     GetVoiceConnectorProxyResponseTypeDef,
     PutVoiceConnectorProxyResponseTypeDef,
     GetVoiceConnectorTerminationHealthResponseTypeDef,
     GetVoiceConnectorTerminationResponseTypeDef,
-    PutVoiceConnectorTerminationRequestRequestTypeDef,
     PutVoiceConnectorTerminationResponseTypeDef,
     InviteUsersResponseTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
+    ListChannelMessagesRequestRequestTypeDef,
     ListSupportedPhoneNumberCountriesResponseTypeDef,
     MeetingTypeDef,
     RoomMembershipTypeDef,
     PhoneNumberOrderTypeDef,
+    OriginationOutputTypeDef,
     OriginationTypeDef,
     ProxySessionTypeDef,
     PhoneNumberTypeDef,
+    PutVoiceConnectorTerminationRequestRequestTypeDef,
+    TerminationUnionTypeDef,
     RetentionSettingsTypeDef,
+    SourceConfigurationOutputTypeDef,
     SourceConfigurationTypeDef,
+    StreamingConfigurationOutputTypeDef,
     StreamingConfigurationTypeDef,
     UserSettingsTypeDef,
     CreateAccountResponseTypeDef,
     GetAccountResponseTypeDef,
     ListAccountsResponseTypeDef,
     UpdateAccountResponseTypeDef,
     BatchUpdateUserRequestRequestTypeDef,
@@ -761,56 +768,61 @@
     ListSipRulesResponseTypeDef,
     UpdateSipRuleResponseTypeDef,
     CreateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorGroupResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     UpdateVoiceConnectorGroupResponseTypeDef,
     GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
-    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
+    EmergencyCallingConfigurationUnionTypeDef,
+    PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef,
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
     ListMeetingsResponseTypeDef,
     CreateRoomMembershipResponseTypeDef,
     ListRoomMembershipsResponseTypeDef,
     UpdateRoomMembershipResponseTypeDef,
     CreatePhoneNumberOrderResponseTypeDef,
     GetPhoneNumberOrderResponseTypeDef,
     ListPhoneNumberOrdersResponseTypeDef,
     GetVoiceConnectorOriginationResponseTypeDef,
-    PutVoiceConnectorOriginationRequestRequestTypeDef,
     PutVoiceConnectorOriginationResponseTypeDef,
+    OriginationUnionTypeDef,
+    PutVoiceConnectorOriginationRequestRequestTypeDef,
     CreateProxySessionResponseTypeDef,
     GetProxySessionResponseTypeDef,
     ListProxySessionsResponseTypeDef,
     UpdateProxySessionResponseTypeDef,
     GetPhoneNumberResponseTypeDef,
     ListPhoneNumbersResponseTypeDef,
     RestorePhoneNumberResponseTypeDef,
     UpdatePhoneNumberResponseTypeDef,
     GetRetentionSettingsResponseTypeDef,
     PutRetentionSettingsRequestRequestTypeDef,
     PutRetentionSettingsResponseTypeDef,
+    ChimeSdkMeetingConfigurationOutputTypeDef,
     ChimeSdkMeetingConfigurationTypeDef,
     GetVoiceConnectorStreamingConfigurationResponseTypeDef,
-    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
     PutVoiceConnectorStreamingConfigurationResponseTypeDef,
+    PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef,
+    StreamingConfigurationUnionTypeDef,
     GetUserSettingsResponseTypeDef,
     UpdateUserSettingsRequestRequestTypeDef,
-    CreateMediaCapturePipelineRequestRequestTypeDef,
     MediaCapturePipelineTypeDef,
+    ChimeSdkMeetingConfigurationUnionTypeDef,
+    CreateMediaCapturePipelineRequestRequestTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountSettingsTypeDef:
+def get_value() -> AccountSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-2.5.2/types_aiobotocore_chime.egg-info/SOURCES.txt` & `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/SOURCES.txt`

 * *Files identical despite different names*


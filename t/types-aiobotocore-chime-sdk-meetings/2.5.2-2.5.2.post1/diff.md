# Comparing `tmp/types-aiobotocore-chime-sdk-meetings-2.5.2.tar.gz` & `tmp/types-aiobotocore-chime-sdk-meetings-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-meetings-2.5.2.tar", last modified: Sat Jul  8 01:43:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-meetings-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
```

## Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2.tar` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.181781 types-aiobotocore-chime-sdk-meetings-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-08 01:43:19.181781 types-aiobotocore-chime-sdk-meetings-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:19.181781 types-aiobotocore-chime-sdk-meetings-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.181781 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-07-08 01:26:41.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14282 2023-07-08 01:26:41.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14269 2023-07-08 01:26:41.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:40.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:19.181781 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 01:43:19.000000 types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.697642 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-08-02 14:51:57.689642 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.697642 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.689642 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15479 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-08-02 14:34:10.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-08-02 14:34:10.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2023-08-02 14:34:10.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:09.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.689642 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/LICENSE` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/PKG-INFO` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-meetings
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ChimeSDKMeetings 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ChimeSDKMeetings 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore chime-sdk-meetings type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore chime-sdk-meetings type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime-sdk-meetings"></a>
 
 # types-aiobotocore-chime-sdk-meetings
 
 [![PyPI - types-aiobotocore-chime-sdk-meetings](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime-sdk-meetings?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime-sdk-meetings)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-meetings)](https://pepy.tech/project/types-aiobotocore-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ChimeSDKMeetings 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
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
 [types-aiobotocore-chime-sdk-meetings docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/).
 
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
@@ -293,48 +292,48 @@
 )
 
 
 def check_value(value: MediaCapabilitiesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime_sdk_meetings.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_chime_sdk_meetings.type_defs import (
     AttendeeCapabilitiesTypeDef,
     AttendeeIdItemTypeDef,
     AudioFeaturesTypeDef,
     CreateAttendeeErrorTypeDef,
+    ResponseMetadataTypeDef,
     NotificationsConfigurationTypeDef,
     TagTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
     DeleteMeetingRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MediaPlacementTypeDef,
-    ResponseMetadataTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     UpdateAttendeeCapabilitiesRequestRequestTypeDef,
     BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
     MeetingFeaturesConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TranscriptionConfigurationTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
@@ -346,15 +345,15 @@
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
 )
 
 
-def get_structure() -> AttendeeCapabilitiesTypeDef:
+def get_value() -> AttendeeCapabilitiesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/README.md` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-chime-sdk-meetings"></a>
 
 # types-aiobotocore-chime-sdk-meetings
 
 [![PyPI - types-aiobotocore-chime-sdk-meetings](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime-sdk-meetings?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime-sdk-meetings)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-meetings)](https://pepy.tech/project/types-aiobotocore-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ChimeSDKMeetings 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
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
 [types-aiobotocore-chime-sdk-meetings docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/).
 
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
@@ -260,48 +260,48 @@
 )
 
 
 def check_value(value: MediaCapabilitiesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime_sdk_meetings.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_chime_sdk_meetings.type_defs import (
     AttendeeCapabilitiesTypeDef,
     AttendeeIdItemTypeDef,
     AudioFeaturesTypeDef,
     CreateAttendeeErrorTypeDef,
+    ResponseMetadataTypeDef,
     NotificationsConfigurationTypeDef,
     TagTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
     DeleteMeetingRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MediaPlacementTypeDef,
-    ResponseMetadataTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     UpdateAttendeeCapabilitiesRequestRequestTypeDef,
     BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
     MeetingFeaturesConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TranscriptionConfigurationTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
@@ -313,15 +313,15 @@
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
 )
 
 
-def get_structure() -> AttendeeCapabilitiesTypeDef:
+def get_value() -> AttendeeCapabilitiesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/setup.py` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-meetings",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_chime_sdk_meetings"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ChimeSDKMeetings 2.5.2 service generated with"
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
-        "aiobotocore chime-sdk-meetings type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore chime-sdk-meetings type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_chime_sdk_meetings": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/"
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/__init__.py` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/__init__.pyi` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/__main__.py` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ChimeSDKMeetings 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ChimeSDKMeetings 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings\nOther"
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

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/client.py` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/client.pyi` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/literals.py` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/literals.pyi` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/type_defs.py` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_chime_sdk_meetings.type_defs import AttendeeCapabilitiesTypeDef
 
-    data: AttendeeCapabilitiesTypeDef = {...}
+    data: AttendeeCapabilitiesTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import (
     MediaCapabilitiesType,
@@ -37,35 +37,35 @@
 
 
 __all__ = (
     "AttendeeCapabilitiesTypeDef",
     "AttendeeIdItemTypeDef",
     "AudioFeaturesTypeDef",
     "CreateAttendeeErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "NotificationsConfigurationTypeDef",
     "TagTypeDef",
     "DeleteAttendeeRequestRequestTypeDef",
     "DeleteMeetingRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "GetAttendeeRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MediaPlacementTypeDef",
-    "ResponseMetadataTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeRequestItemTypeDef",
     "CreateAttendeeRequestRequestTypeDef",
     "UpdateAttendeeCapabilitiesRequestRequestTypeDef",
     "BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef",
     "MeetingFeaturesConfigurationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TranscriptionConfigurationTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
@@ -110,14 +110,25 @@
         "ExternalUserId": str,
         "ErrorCode": str,
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
 NotificationsConfigurationTypeDef = TypedDict(
     "NotificationsConfigurationTypeDef",
     {
         "LambdaFunctionArn": str,
         "SnsTopicArn": str,
         "SqsQueueArn": str,
     },
@@ -143,21 +154,14 @@
 DeleteMeetingRequestRequestTypeDef = TypedDict(
     "DeleteMeetingRequestRequestTypeDef",
     {
         "MeetingId": str,
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
@@ -257,25 +261,14 @@
         "ScreenViewingUrl": str,
         "ScreenSharingUrl": str,
         "EventIngestionUrl": str,
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
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
@@ -363,19 +356,26 @@
     "MeetingFeaturesConfigurationTypeDef",
     {
         "Audio": AudioFeaturesTypeDef,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
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
@@ -393,48 +393,48 @@
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
 
 UpdateAttendeeCapabilitiesResponseTypeDef = TypedDict(
     "UpdateAttendeeCapabilitiesResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateAttendeeRequestRequestTypeDef = TypedDict(
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -524,28 +524,28 @@
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
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings/type_defs.pyi` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_chime_sdk_meetings.type_defs import AttendeeCapabilitiesTypeDef
 
-    data: AttendeeCapabilitiesTypeDef = {...}
+    data: AttendeeCapabilitiesTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import (
     MediaCapabilitiesType,
@@ -36,35 +36,35 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttendeeCapabilitiesTypeDef",
     "AttendeeIdItemTypeDef",
     "AudioFeaturesTypeDef",
     "CreateAttendeeErrorTypeDef",
+    "ResponseMetadataTypeDef",
     "NotificationsConfigurationTypeDef",
     "TagTypeDef",
     "DeleteAttendeeRequestRequestTypeDef",
     "DeleteMeetingRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EngineTranscribeMedicalSettingsTypeDef",
     "EngineTranscribeSettingsTypeDef",
     "GetAttendeeRequestRequestTypeDef",
     "GetMeetingRequestRequestTypeDef",
     "ListAttendeesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MediaPlacementTypeDef",
-    "ResponseMetadataTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AttendeeTypeDef",
     "CreateAttendeeRequestItemTypeDef",
     "CreateAttendeeRequestRequestTypeDef",
     "UpdateAttendeeCapabilitiesRequestRequestTypeDef",
     "BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef",
     "MeetingFeaturesConfigurationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TranscriptionConfigurationTypeDef",
     "BatchCreateAttendeeResponseTypeDef",
     "CreateAttendeeResponseTypeDef",
     "GetAttendeeResponseTypeDef",
     "ListAttendeesResponseTypeDef",
@@ -109,14 +109,25 @@
         "ExternalUserId": str,
         "ErrorCode": str,
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
 NotificationsConfigurationTypeDef = TypedDict(
     "NotificationsConfigurationTypeDef",
     {
         "LambdaFunctionArn": str,
         "SnsTopicArn": str,
         "SqsQueueArn": str,
     },
@@ -142,21 +153,14 @@
 DeleteMeetingRequestRequestTypeDef = TypedDict(
     "DeleteMeetingRequestRequestTypeDef",
     {
         "MeetingId": str,
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
@@ -252,25 +256,14 @@
         "ScreenViewingUrl": str,
         "ScreenSharingUrl": str,
         "EventIngestionUrl": str,
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
 StopMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StopMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
     },
 )
 
@@ -354,19 +347,26 @@
     "MeetingFeaturesConfigurationTypeDef",
     {
         "Audio": AudioFeaturesTypeDef,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
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
@@ -384,48 +384,48 @@
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
 
 UpdateAttendeeCapabilitiesResponseTypeDef = TypedDict(
     "UpdateAttendeeCapabilitiesResponseTypeDef",
     {
         "Attendee": AttendeeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchCreateAttendeeRequestRequestTypeDef = TypedDict(
     "BatchCreateAttendeeRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -511,28 +511,28 @@
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
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings.egg-info/PKG-INFO` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chime-sdk-meetings
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ChimeSDKMeetings 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ChimeSDKMeetings 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore chime-sdk-meetings type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore chime-sdk-meetings type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime-sdk-meetings"></a>
 
 # types-aiobotocore-chime-sdk-meetings
 
 [![PyPI - types-aiobotocore-chime-sdk-meetings](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-meetings.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-meetings)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-chime-sdk-meetings?color=blue)](https://pypistats.org/packages/types-aiobotocore-chime-sdk-meetings)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chime-sdk-meetings)](https://pepy.tech/project/types-aiobotocore-chime-sdk-meetings)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ChimeSDKMeetings 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#ChimeSDKMeetings)
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
 [types-aiobotocore-chime-sdk-meetings docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_meetings/).
 
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
@@ -293,48 +292,48 @@
 )
 
 
 def check_value(value: MediaCapabilitiesType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_chime_sdk_meetings.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_chime_sdk_meetings.type_defs import (
     AttendeeCapabilitiesTypeDef,
     AttendeeIdItemTypeDef,
     AudioFeaturesTypeDef,
     CreateAttendeeErrorTypeDef,
+    ResponseMetadataTypeDef,
     NotificationsConfigurationTypeDef,
     TagTypeDef,
     DeleteAttendeeRequestRequestTypeDef,
     DeleteMeetingRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EngineTranscribeMedicalSettingsTypeDef,
     EngineTranscribeSettingsTypeDef,
     GetAttendeeRequestRequestTypeDef,
     GetMeetingRequestRequestTypeDef,
     ListAttendeesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MediaPlacementTypeDef,
-    ResponseMetadataTypeDef,
     StopMeetingTranscriptionRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AttendeeTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeRequestRequestTypeDef,
     UpdateAttendeeCapabilitiesRequestRequestTypeDef,
     BatchUpdateAttendeeCapabilitiesExceptRequestRequestTypeDef,
     MeetingFeaturesConfigurationTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     TranscriptionConfigurationTypeDef,
     BatchCreateAttendeeResponseTypeDef,
     CreateAttendeeResponseTypeDef,
     GetAttendeeResponseTypeDef,
     ListAttendeesResponseTypeDef,
@@ -346,15 +345,15 @@
     StartMeetingTranscriptionRequestRequestTypeDef,
     CreateMeetingResponseTypeDef,
     CreateMeetingWithAttendeesResponseTypeDef,
     GetMeetingResponseTypeDef,
 )
 
 
-def get_structure() -> AttendeeCapabilitiesTypeDef:
+def get_value() -> AttendeeCapabilitiesTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-chime-sdk-meetings-2.5.2/types_aiobotocore_chime_sdk_meetings.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-meetings-2.5.2.post1/types_aiobotocore_chime_sdk_meetings.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-sms-voice-2.5.2.tar.gz` & `tmp/types-aiobotocore-sms-voice-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sms-voice-2.5.2.tar", last modified: Sat Jul  8 01:44:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-sms-voice-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:02 2023, max compression
```

## Comparing `types-aiobotocore-sms-voice-2.5.2.tar` & `types-aiobotocore-sms-voice-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.730912 types-aiobotocore-sms-voice-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:12.000000 types-aiobotocore-sms-voice-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13098 2023-07-08 01:44:20.730912 types-aiobotocore-sms-voice-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-07-08 01:41:12.000000 types-aiobotocore-sms-voice-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:20.730912 types-aiobotocore-sms-voice-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:41:12.000000 types-aiobotocore-sms-voice-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.730912 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-08 01:41:12.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-08 01:41:12.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-08 01:41:12.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-08 01:41:12.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-07-08 01:41:12.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-07-08 01:41:13.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-08 01:41:12.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:12.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-07-08 01:41:13.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-07-08 01:41:13.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:12.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:20.730912 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13098 2023-07-08 01:44:20.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-08 01:44:20.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:20.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:20.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:20.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:44:20.000000 types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.249454 types-aiobotocore-sms-voice-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-08-02 14:53:02.241454 types-aiobotocore-sms-voice-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:02.249454 types-aiobotocore-sms-voice-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.233454 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.241454 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-08-02 14:53:02.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 14:53:02.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:02.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:02.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:02.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:53:02.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sms-voice-2.5.2/LICENSE` & `types-aiobotocore-sms-voice-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-voice-2.5.2/PKG-INFO` & `types-aiobotocore-sms-voice-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sms-voice
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.PinpointSMSVoice 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.PinpointSMSVoice 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sms-voice type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sms-voice type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sms-voice"></a>
 
 # types-aiobotocore-sms-voice
 
 [![PyPI - types-aiobotocore-sms-voice](https://img.shields.io/pypi/v/types-aiobotocore-sms-voice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sms-voice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms-voice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sms-voice?color=blue)](https://pypistats.org/packages/types-aiobotocore-sms-voice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sms-voice)](https://pepy.tech/project/types-aiobotocore-sms-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.PinpointSMSVoice 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice)
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
 [types-aiobotocore-sms-voice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/).
 
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
@@ -280,48 +279,48 @@
 )
 
 
 def check_value(value: EventTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sms_voice.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sms_voice.type_defs import (
     CallInstructionsMessageTypeTypeDef,
     CloudWatchLogsDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     PlainTextMessageTypeTypeDef,
-    ResponseMetadataTypeDef,
     SSMLMessageTypeTypeDef,
-    SendVoiceMessageResponseTypeDef,
     EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    SendVoiceMessageResponseTypeDef,
     VoiceMessageContentTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     SendVoiceMessageRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CallInstructionsMessageTypeTypeDef:
+def get_value() -> CallInstructionsMessageTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sms-voice-2.5.2/README.md` & `types-aiobotocore-sms-voice-2.5.2.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-sms-voice"></a>
 
 # types-aiobotocore-sms-voice
 
 [![PyPI - types-aiobotocore-sms-voice](https://img.shields.io/pypi/v/types-aiobotocore-sms-voice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sms-voice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms-voice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sms-voice?color=blue)](https://pypistats.org/packages/types-aiobotocore-sms-voice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sms-voice)](https://pepy.tech/project/types-aiobotocore-sms-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.PinpointSMSVoice 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice)
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
 [types-aiobotocore-sms-voice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/).
 
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
@@ -247,48 +247,48 @@
 )
 
 
 def check_value(value: EventTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sms_voice.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sms_voice.type_defs import (
     CallInstructionsMessageTypeTypeDef,
     CloudWatchLogsDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     PlainTextMessageTypeTypeDef,
-    ResponseMetadataTypeDef,
     SSMLMessageTypeTypeDef,
-    SendVoiceMessageResponseTypeDef,
     EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    SendVoiceMessageResponseTypeDef,
     VoiceMessageContentTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     SendVoiceMessageRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CallInstructionsMessageTypeTypeDef:
+def get_value() -> CallInstructionsMessageTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sms-voice-2.5.2/setup.py` & `types-aiobotocore-sms-voice-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sms-voice",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_sms_voice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.PinpointSMSVoice 2.5.2 service generated with"
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
-    keywords="aiobotocore sms-voice type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore sms-voice type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sms_voice": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/"
```

### Comparing `types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/__main__.py` & `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PinpointSMSVoice 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.PinpointSMSVoice 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice\nOther"
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

### Comparing `types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/client.py` & `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/client.pyi` & `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/literals.py` & `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/literals.pyi` & `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/type_defs.py` & `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sms_voice.type_defs import CallInstructionsMessageTypeTypeDef
 
-    data: CallInstructionsMessageTypeTypeDef = {...}
+    data: CallInstructionsMessageTypeTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import EventTypeType
 
@@ -27,22 +27,22 @@
     "CloudWatchLogsDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SnsDestinationTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
     "PlainTextMessageTypeTypeDef",
-    "ResponseMetadataTypeDef",
     "SSMLMessageTypeTypeDef",
-    "SendVoiceMessageResponseTypeDef",
     "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "SendVoiceMessageResponseTypeDef",
     "VoiceMessageContentTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     "SendVoiceMessageRequestRequestTypeDef",
 )
 
@@ -106,71 +106,54 @@
 GetConfigurationSetEventDestinationsRequestRequestTypeDef = TypedDict(
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
-ListConfigurationSetsRequestRequestTypeDef = TypedDict(
-    "ListConfigurationSetsRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "NextToken": str,
-        "PageSize": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
+ListConfigurationSetsRequestRequestTypeDef = TypedDict(
+    "ListConfigurationSetsRequestRequestTypeDef",
     {
-        "ConfigurationSets": List[str],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PageSize": str,
     },
+    total=False,
 )
 
 PlainTextMessageTypeTypeDef = TypedDict(
     "PlainTextMessageTypeTypeDef",
     {
         "LanguageCode": str,
         "Text": str,
         "VoiceId": str,
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
 SSMLMessageTypeTypeDef = TypedDict(
     "SSMLMessageTypeTypeDef",
     {
         "LanguageCode": str,
         "Text": str,
         "VoiceId": str,
     },
     total=False,
 )
 
-SendVoiceMessageResponseTypeDef = TypedDict(
-    "SendVoiceMessageResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventDestinationDefinitionTypeDef = TypedDict(
     "EventDestinationDefinitionTypeDef",
     {
         "CloudWatchLogsDestination": CloudWatchLogsDestinationTypeDef,
         "Enabled": bool,
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "MatchingEventTypes": Sequence[EventTypeType],
@@ -188,14 +171,31 @@
         "MatchingEventTypes": List[EventTypeType],
         "Name": str,
         "SnsDestination": SnsDestinationTypeDef,
     },
     total=False,
 )
 
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendVoiceMessageResponseTypeDef = TypedDict(
+    "SendVoiceMessageResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VoiceMessageContentTypeDef = TypedDict(
     "VoiceMessageContentTypeDef",
     {
         "CallInstructionsMessage": CallInstructionsMessageTypeTypeDef,
         "PlainTextMessage": PlainTextMessageTypeTypeDef,
         "SSMLMessage": SSMLMessageTypeTypeDef,
     },
@@ -248,15 +248,15 @@
     pass
 
 
 GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     {
         "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendVoiceMessageRequestRequestTypeDef = TypedDict(
     "SendVoiceMessageRequestRequestTypeDef",
     {
         "CallerId": str,
```

### Comparing `types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice/type_defs.pyi` & `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sms_voice.type_defs import CallInstructionsMessageTypeTypeDef
 
-    data: CallInstructionsMessageTypeTypeDef = {...}
+    data: CallInstructionsMessageTypeTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import EventTypeType
 
@@ -26,22 +26,22 @@
     "CloudWatchLogsDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "SnsDestinationTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
-    "ListConfigurationSetsResponseTypeDef",
     "PlainTextMessageTypeTypeDef",
-    "ResponseMetadataTypeDef",
     "SSMLMessageTypeTypeDef",
-    "SendVoiceMessageResponseTypeDef",
     "EventDestinationDefinitionTypeDef",
     "EventDestinationTypeDef",
+    "ListConfigurationSetsResponseTypeDef",
+    "SendVoiceMessageResponseTypeDef",
     "VoiceMessageContentTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     "SendVoiceMessageRequestRequestTypeDef",
 )
 
@@ -105,71 +105,54 @@
 GetConfigurationSetEventDestinationsRequestRequestTypeDef = TypedDict(
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
-ListConfigurationSetsRequestRequestTypeDef = TypedDict(
-    "ListConfigurationSetsRequestRequestTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "NextToken": str,
-        "PageSize": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-ListConfigurationSetsResponseTypeDef = TypedDict(
-    "ListConfigurationSetsResponseTypeDef",
+ListConfigurationSetsRequestRequestTypeDef = TypedDict(
+    "ListConfigurationSetsRequestRequestTypeDef",
     {
-        "ConfigurationSets": List[str],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PageSize": str,
     },
+    total=False,
 )
 
 PlainTextMessageTypeTypeDef = TypedDict(
     "PlainTextMessageTypeTypeDef",
     {
         "LanguageCode": str,
         "Text": str,
         "VoiceId": str,
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
 SSMLMessageTypeTypeDef = TypedDict(
     "SSMLMessageTypeTypeDef",
     {
         "LanguageCode": str,
         "Text": str,
         "VoiceId": str,
     },
     total=False,
 )
 
-SendVoiceMessageResponseTypeDef = TypedDict(
-    "SendVoiceMessageResponseTypeDef",
-    {
-        "MessageId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EventDestinationDefinitionTypeDef = TypedDict(
     "EventDestinationDefinitionTypeDef",
     {
         "CloudWatchLogsDestination": CloudWatchLogsDestinationTypeDef,
         "Enabled": bool,
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "MatchingEventTypes": Sequence[EventTypeType],
@@ -187,14 +170,31 @@
         "MatchingEventTypes": List[EventTypeType],
         "Name": str,
         "SnsDestination": SnsDestinationTypeDef,
     },
     total=False,
 )
 
+ListConfigurationSetsResponseTypeDef = TypedDict(
+    "ListConfigurationSetsResponseTypeDef",
+    {
+        "ConfigurationSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendVoiceMessageResponseTypeDef = TypedDict(
+    "SendVoiceMessageResponseTypeDef",
+    {
+        "MessageId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 VoiceMessageContentTypeDef = TypedDict(
     "VoiceMessageContentTypeDef",
     {
         "CallInstructionsMessage": CallInstructionsMessageTypeTypeDef,
         "PlainTextMessage": PlainTextMessageTypeTypeDef,
         "SSMLMessage": SSMLMessageTypeTypeDef,
     },
@@ -243,15 +243,15 @@
 ):
     pass
 
 GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
     "GetConfigurationSetEventDestinationsResponseTypeDef",
     {
         "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendVoiceMessageRequestRequestTypeDef = TypedDict(
     "SendVoiceMessageRequestRequestTypeDef",
     {
         "CallerId": str,
```

### Comparing `types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice.egg-info/PKG-INFO` & `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sms-voice
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.PinpointSMSVoice 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.PinpointSMSVoice 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sms-voice type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sms-voice type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sms-voice"></a>
 
 # types-aiobotocore-sms-voice
 
 [![PyPI - types-aiobotocore-sms-voice](https://img.shields.io/pypi/v/types-aiobotocore-sms-voice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms-voice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sms-voice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sms-voice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sms-voice?color=blue)](https://pypistats.org/packages/types-aiobotocore-sms-voice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sms-voice)](https://pepy.tech/project/types-aiobotocore-sms-voice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.PinpointSMSVoice 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice)
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
 [types-aiobotocore-sms-voice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/).
 
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
@@ -280,48 +279,48 @@
 )
 
 
 def check_value(value: EventTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sms_voice.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sms_voice.type_defs import (
     CallInstructionsMessageTypeTypeDef,
     CloudWatchLogsDestinationTypeDef,
     CreateConfigurationSetRequestRequestTypeDef,
     DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
     DeleteConfigurationSetRequestRequestTypeDef,
     KinesisFirehoseDestinationTypeDef,
     SnsDestinationTypeDef,
     GetConfigurationSetEventDestinationsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ListConfigurationSetsRequestRequestTypeDef,
-    ListConfigurationSetsResponseTypeDef,
     PlainTextMessageTypeTypeDef,
-    ResponseMetadataTypeDef,
     SSMLMessageTypeTypeDef,
-    SendVoiceMessageResponseTypeDef,
     EventDestinationDefinitionTypeDef,
     EventDestinationTypeDef,
+    ListConfigurationSetsResponseTypeDef,
+    SendVoiceMessageResponseTypeDef,
     VoiceMessageContentTypeDef,
     CreateConfigurationSetEventDestinationRequestRequestTypeDef,
     UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     SendVoiceMessageRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CallInstructionsMessageTypeTypeDef:
+def get_value() -> CallInstructionsMessageTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sms-voice-2.5.2/types_aiobotocore_sms_voice.egg-info/SOURCES.txt` & `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-voice-id-2.5.2.tar.gz` & `tmp/types-aiobotocore-voice-id-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-voice-id-2.5.2.tar", last modified: Sat Jul  8 01:44:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-voice-id-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:09 2023, max compression
```

## Comparing `types-aiobotocore-voice-id-2.5.2.tar` & `types-aiobotocore-voice-id-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.211030 types-aiobotocore-voice-id-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-07-08 01:44:27.211030 types-aiobotocore-voice-id-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16206 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:27.211030 types-aiobotocore-voice-id-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.211030 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25008 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32507 2023-07-08 01:42:13.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32470 2023-07-08 01:42:13.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:12.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.211030 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17774 2023-07-08 01:44:27.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-08 01:44:27.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:27.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:27.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:27.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:27.000000 types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.097431 types-aiobotocore-voice-id-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-08-02 14:53:09.093431 types-aiobotocore-voice-id-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:09.097431 types-aiobotocore-voice-id-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-02 14:50:47.000000 types-aiobotocore-voice-id-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.093431 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25028 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24984 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33666 2023-08-02 14:50:49.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33629 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:48.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.093431 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17904 2023-08-02 14:53:08.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:53:08.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:08.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:08.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:08.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:08.000000 types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-voice-id-2.5.2/LICENSE` & `types-aiobotocore-voice-id-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2/PKG-INFO` & `types-aiobotocore-voice-id-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-voice-id
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.VoiceID 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.VoiceID 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore voice-id type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore voice-id type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-voice-id"></a>
 
 # types-aiobotocore-voice-id
 
 [![PyPI - types-aiobotocore-voice-id](https://img.shields.io/pypi/v/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-voice-id?color=blue)](https://pypistats.org/packages/types-aiobotocore-voice-id)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-voice-id)](https://pepy.tech/project/types-aiobotocore-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.VoiceID 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [types-aiobotocore-voice-id docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/).
 
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
@@ -337,25 +336,26 @@
 )
 
 
 def check_value(value: AuthenticationDecisionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_voice_id.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_voice_id.type_defs import (
     AssociateFraudsterRequestRequestTypeDef,
     FraudsterTypeDef,
+    ResponseMetadataTypeDef,
     AuthenticationConfigurationTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TagTypeDef,
     CreateWatchlistRequestRequestTypeDef,
     WatchlistTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteFraudsterRequestRequestTypeDef,
@@ -367,88 +367,92 @@
     DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
     DescribeSpeakerRequestRequestTypeDef,
     SpeakerTypeDef,
     DescribeWatchlistRequestRequestTypeDef,
     DisassociateFraudsterRequestRequestTypeDef,
     ServerSideEncryptionUpdateDetailsTypeDef,
     WatchlistDetailsTypeDef,
-    EmptyResponseMetadataTypeDef,
+    EnrollmentJobFraudDetectionConfigOutputTypeDef,
     EnrollmentJobFraudDetectionConfigTypeDef,
     EvaluateSessionRequestRequestTypeDef,
     FailureDetailsTypeDef,
     FraudDetectionConfigurationTypeDef,
     KnownFraudsterRiskTypeDef,
     VoiceSpoofingRiskTypeDef,
     JobProgressTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
-    RegistrationConfigTypeDef,
+    RegistrationConfigOutputTypeDef,
     FraudsterSummaryTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudsterRegistrationJobsRequestRequestTypeDef,
-    ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListFraudstersRequestRequestTypeDef,
-    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestRequestTypeDef,
-    ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListSpeakersRequestRequestTypeDef,
     SpeakerSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListWatchlistsRequestRequestTypeDef,
     WatchlistSummaryTypeDef,
     OptOutSpeakerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    RegistrationConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWatchlistRequestRequestTypeDef,
     AssociateFraudsterResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     AuthenticationResultTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateWatchlistResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     DomainSummaryTypeDef,
     DomainTypeDef,
+    EnrollmentConfigOutputTypeDef,
     EnrollmentConfigTypeDef,
     FraudRiskDetailsTypeDef,
     FraudsterRegistrationJobSummaryTypeDef,
     SpeakerEnrollmentJobSummaryTypeDef,
     FraudsterRegistrationJobTypeDef,
-    StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListFraudstersResponseTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+    ListFraudstersRequestListFraudstersPaginateTypeDef,
+    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+    ListSpeakersRequestListSpeakersPaginateTypeDef,
+    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
     ListWatchlistsResponseTypeDef,
+    RegistrationConfigUnionTypeDef,
+    StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
+    EnrollmentConfigUnionTypeDef,
     StartSpeakerEnrollmentJobRequestRequestTypeDef,
     FraudDetectionResultTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     DescribeFraudsterRegistrationJobResponseTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     EvaluateSessionResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateFraudsterRequestRequestTypeDef:
+def get_value() -> AssociateFraudsterRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-voice-id-2.5.2/README.md` & `types-aiobotocore-voice-id-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-voice-id"></a>
 
 # types-aiobotocore-voice-id
 
 [![PyPI - types-aiobotocore-voice-id](https://img.shields.io/pypi/v/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-voice-id?color=blue)](https://pypistats.org/packages/types-aiobotocore-voice-id)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-voice-id)](https://pepy.tech/project/types-aiobotocore-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.VoiceID 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [types-aiobotocore-voice-id docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/).
 
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
@@ -304,25 +304,26 @@
 )
 
 
 def check_value(value: AuthenticationDecisionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_voice_id.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_voice_id.type_defs import (
     AssociateFraudsterRequestRequestTypeDef,
     FraudsterTypeDef,
+    ResponseMetadataTypeDef,
     AuthenticationConfigurationTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TagTypeDef,
     CreateWatchlistRequestRequestTypeDef,
     WatchlistTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteFraudsterRequestRequestTypeDef,
@@ -334,88 +335,92 @@
     DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
     DescribeSpeakerRequestRequestTypeDef,
     SpeakerTypeDef,
     DescribeWatchlistRequestRequestTypeDef,
     DisassociateFraudsterRequestRequestTypeDef,
     ServerSideEncryptionUpdateDetailsTypeDef,
     WatchlistDetailsTypeDef,
-    EmptyResponseMetadataTypeDef,
+    EnrollmentJobFraudDetectionConfigOutputTypeDef,
     EnrollmentJobFraudDetectionConfigTypeDef,
     EvaluateSessionRequestRequestTypeDef,
     FailureDetailsTypeDef,
     FraudDetectionConfigurationTypeDef,
     KnownFraudsterRiskTypeDef,
     VoiceSpoofingRiskTypeDef,
     JobProgressTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
-    RegistrationConfigTypeDef,
+    RegistrationConfigOutputTypeDef,
     FraudsterSummaryTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudsterRegistrationJobsRequestRequestTypeDef,
-    ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListFraudstersRequestRequestTypeDef,
-    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestRequestTypeDef,
-    ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListSpeakersRequestRequestTypeDef,
     SpeakerSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListWatchlistsRequestRequestTypeDef,
     WatchlistSummaryTypeDef,
     OptOutSpeakerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    RegistrationConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWatchlistRequestRequestTypeDef,
     AssociateFraudsterResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     AuthenticationResultTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateWatchlistResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     DomainSummaryTypeDef,
     DomainTypeDef,
+    EnrollmentConfigOutputTypeDef,
     EnrollmentConfigTypeDef,
     FraudRiskDetailsTypeDef,
     FraudsterRegistrationJobSummaryTypeDef,
     SpeakerEnrollmentJobSummaryTypeDef,
     FraudsterRegistrationJobTypeDef,
-    StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListFraudstersResponseTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+    ListFraudstersRequestListFraudstersPaginateTypeDef,
+    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+    ListSpeakersRequestListSpeakersPaginateTypeDef,
+    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
     ListWatchlistsResponseTypeDef,
+    RegistrationConfigUnionTypeDef,
+    StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
+    EnrollmentConfigUnionTypeDef,
     StartSpeakerEnrollmentJobRequestRequestTypeDef,
     FraudDetectionResultTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     DescribeFraudsterRegistrationJobResponseTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     EvaluateSessionResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateFraudsterRequestRequestTypeDef:
+def get_value() -> AssociateFraudsterRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-voice-id-2.5.2/setup.py` & `types-aiobotocore-voice-id-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-voice-id",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_voice_id"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.VoiceID 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore voice-id type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore voice-id type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_voice_id": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/"
```

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/__init__.py` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/__init__.pyi` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/__main__.py` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.VoiceID 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.VoiceID 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID\nOther"
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

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/client.py` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,27 +37,27 @@
     DescribeFraudsterRegistrationJobResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnrollmentConfigTypeDef,
+    EnrollmentConfigUnionTypeDef,
     EvaluateSessionResponseTypeDef,
     InputDataConfigTypeDef,
     ListDomainsResponseTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListFraudstersResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     ListSpeakersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     OutputDataConfigTypeDef,
-    RegistrationConfigTypeDef,
+    RegistrationConfigUnionTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     TagTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
 )
@@ -388,15 +388,15 @@
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
         JobName: str = ...,
-        RegistrationConfig: RegistrationConfigTypeDef = ...
+        RegistrationConfig: RegistrationConfigUnionTypeDef = ...
     ) -> StartFraudsterRegistrationJobResponseTypeDef:
         """
         Starts a new batch fraudster registration job using provided details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_fraudster_registration_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#start_fraudster_registration_job)
         """
@@ -405,15 +405,15 @@
         self,
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
-        EnrollmentConfig: EnrollmentConfigTypeDef = ...,
+        EnrollmentConfig: EnrollmentConfigUnionTypeDef = ...,
         JobName: str = ...
     ) -> StartSpeakerEnrollmentJobResponseTypeDef:
         """
         Starts a new batch speaker enrollment job using specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_speaker_enrollment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#start_speaker_enrollment_job)
```

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/client.pyi` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,27 +37,27 @@
     DescribeFraudsterRegistrationJobResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EnrollmentConfigTypeDef,
+    EnrollmentConfigUnionTypeDef,
     EvaluateSessionResponseTypeDef,
     InputDataConfigTypeDef,
     ListDomainsResponseTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListFraudstersResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     ListSpeakersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWatchlistsResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     OutputDataConfigTypeDef,
-    RegistrationConfigTypeDef,
+    RegistrationConfigUnionTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     TagTypeDef,
     UpdateDomainResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
 )
@@ -357,15 +357,15 @@
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
         JobName: str = ...,
-        RegistrationConfig: RegistrationConfigTypeDef = ...
+        RegistrationConfig: RegistrationConfigUnionTypeDef = ...
     ) -> StartFraudsterRegistrationJobResponseTypeDef:
         """
         Starts a new batch fraudster registration job using provided details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_fraudster_registration_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#start_fraudster_registration_job)
         """
@@ -373,15 +373,15 @@
         self,
         *,
         DataAccessRoleArn: str,
         DomainId: str,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         ClientToken: str = ...,
-        EnrollmentConfig: EnrollmentConfigTypeDef = ...,
+        EnrollmentConfig: EnrollmentConfigUnionTypeDef = ...,
         JobName: str = ...
     ) -> StartSpeakerEnrollmentJobResponseTypeDef:
         """
         Starts a new batch speaker enrollment job using specified details.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Client.start_speaker_enrollment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/client/#start_speaker_enrollment_job)
```

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/literals.py` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/literals.pyi` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/paginator.py` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 class ListDomainsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListDomains)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listdomainspaginator)
         """
 
 
@@ -88,15 +88,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: FraudsterRegistrationJobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFraudsterRegistrationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsterRegistrationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listfraudsterregistrationjobspaginator)
         """
 
 
@@ -107,15 +107,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         WatchlistId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFraudstersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listfraudsterspaginator)
         """
 
 
@@ -126,43 +126,43 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: SpeakerEnrollmentJobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSpeakerEnrollmentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakerEnrollmentJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listspeakerenrollmentjobspaginator)
         """
 
 
 class ListSpeakersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listspeakerspaginator)
     """
 
     def paginate(
-        self, *, DomainId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSpeakersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listspeakerspaginator)
         """
 
 
 class ListWatchlistsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListWatchlists)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listwatchlistspaginator)
     """
 
     def paginate(
-        self, *, DomainId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWatchlistsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListWatchlists.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listwatchlistspaginator)
         """
```

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/paginator.pyi` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 class ListDomainsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListDomains)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listdomainspaginator)
         """
 
 class ListFraudsterRegistrationJobsPaginator(AioPaginator):
@@ -84,15 +84,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: FraudsterRegistrationJobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFraudsterRegistrationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsterRegistrationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listfraudsterregistrationjobspaginator)
         """
 
 class ListFraudstersPaginator(AioPaginator):
@@ -102,15 +102,15 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         WatchlistId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFraudstersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListFraudsters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listfraudsterspaginator)
         """
 
 class ListSpeakerEnrollmentJobsPaginator(AioPaginator):
@@ -120,41 +120,41 @@
     """
 
     def paginate(
         self,
         *,
         DomainId: str,
         JobStatus: SpeakerEnrollmentJobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSpeakerEnrollmentJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakerEnrollmentJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listspeakerenrollmentjobspaginator)
         """
 
 class ListSpeakersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listspeakerspaginator)
     """
 
     def paginate(
-        self, *, DomainId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSpeakersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListSpeakers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listspeakerspaginator)
         """
 
 class ListWatchlistsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListWatchlists)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listwatchlistspaginator)
     """
 
     def paginate(
-        self, *, DomainId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DomainId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWatchlistsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID.Paginator.ListWatchlists.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/paginators/#listwatchlistspaginator)
         """
```

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/type_defs.py` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_voice_id.type_defs import AssociateFraudsterRequestRequestTypeDef
 
-    data: AssociateFraudsterRequestRequestTypeDef = {...}
+    data: AssociateFraudsterRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AuthenticationDecisionType,
     DomainStatusType,
     DuplicateRegistrationActionType,
     ExistingEnrollmentActionType,
     FraudDetectionActionType,
@@ -35,14 +35,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateFraudsterRequestRequestTypeDef",
     "FraudsterTypeDef",
+    "ResponseMetadataTypeDef",
     "AuthenticationConfigurationTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "TagTypeDef",
     "CreateWatchlistRequestRequestTypeDef",
     "WatchlistTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteFraudsterRequestRequestTypeDef",
@@ -54,75 +55,79 @@
     "DescribeSpeakerEnrollmentJobRequestRequestTypeDef",
     "DescribeSpeakerRequestRequestTypeDef",
     "SpeakerTypeDef",
     "DescribeWatchlistRequestRequestTypeDef",
     "DisassociateFraudsterRequestRequestTypeDef",
     "ServerSideEncryptionUpdateDetailsTypeDef",
     "WatchlistDetailsTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "EnrollmentJobFraudDetectionConfigOutputTypeDef",
     "EnrollmentJobFraudDetectionConfigTypeDef",
     "EvaluateSessionRequestRequestTypeDef",
     "FailureDetailsTypeDef",
     "FraudDetectionConfigurationTypeDef",
     "KnownFraudsterRiskTypeDef",
     "VoiceSpoofingRiskTypeDef",
     "JobProgressTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
-    "RegistrationConfigTypeDef",
+    "RegistrationConfigOutputTypeDef",
     "FraudsterSummaryTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
     "ListFraudsterRegistrationJobsRequestRequestTypeDef",
-    "ListFraudstersRequestListFraudstersPaginateTypeDef",
     "ListFraudstersRequestRequestTypeDef",
-    "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     "ListSpeakerEnrollmentJobsRequestRequestTypeDef",
-    "ListSpeakersRequestListSpeakersPaginateTypeDef",
     "ListSpeakersRequestRequestTypeDef",
     "SpeakerSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListWatchlistsRequestRequestTypeDef",
     "WatchlistSummaryTypeDef",
     "OptOutSpeakerRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "RegistrationConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWatchlistRequestRequestTypeDef",
     "AssociateFraudsterResponseTypeDef",
     "DescribeFraudsterResponseTypeDef",
     "DisassociateFraudsterResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "AuthenticationResultTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateWatchlistResponseTypeDef",
     "DescribeWatchlistResponseTypeDef",
     "UpdateWatchlistResponseTypeDef",
     "DescribeSpeakerResponseTypeDef",
     "OptOutSpeakerResponseTypeDef",
     "DomainSummaryTypeDef",
     "DomainTypeDef",
+    "EnrollmentConfigOutputTypeDef",
     "EnrollmentConfigTypeDef",
     "FraudRiskDetailsTypeDef",
     "FraudsterRegistrationJobSummaryTypeDef",
     "SpeakerEnrollmentJobSummaryTypeDef",
     "FraudsterRegistrationJobTypeDef",
-    "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListFraudstersResponseTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+    "ListFraudstersRequestListFraudstersPaginateTypeDef",
+    "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
+    "ListSpeakersRequestListSpeakersPaginateTypeDef",
+    "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListSpeakersResponseTypeDef",
     "ListWatchlistsResponseTypeDef",
+    "RegistrationConfigUnionTypeDef",
+    "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "SpeakerEnrollmentJobTypeDef",
+    "EnrollmentConfigUnionTypeDef",
     "StartSpeakerEnrollmentJobRequestRequestTypeDef",
     "FraudDetectionResultTypeDef",
     "ListFraudsterRegistrationJobsResponseTypeDef",
     "ListSpeakerEnrollmentJobsResponseTypeDef",
     "DescribeFraudsterRegistrationJobResponseTypeDef",
     "StartFraudsterRegistrationJobResponseTypeDef",
     "DescribeSpeakerEnrollmentJobResponseTypeDef",
@@ -146,14 +151,25 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
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
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "AcceptanceThreshold": int,
     },
 )
 
@@ -323,27 +339,30 @@
 WatchlistDetailsTypeDef = TypedDict(
     "WatchlistDetailsTypeDef",
     {
         "DefaultWatchlistId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+EnrollmentJobFraudDetectionConfigOutputTypeDef = TypedDict(
+    "EnrollmentJobFraudDetectionConfigOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FraudDetectionAction": FraudDetectionActionType,
+        "RiskThreshold": int,
+        "WatchlistIds": List[str],
     },
+    total=False,
 )
 
 EnrollmentJobFraudDetectionConfigTypeDef = TypedDict(
     "EnrollmentJobFraudDetectionConfigTypeDef",
     {
         "FraudDetectionAction": FraudDetectionActionType,
         "RiskThreshold": int,
-        "WatchlistIds": List[str],
+        "WatchlistIds": Sequence[str],
     },
     total=False,
 )
 
 EvaluateSessionRequestRequestTypeDef = TypedDict(
     "EvaluateSessionRequestRequestTypeDef",
     {
@@ -428,16 +447,16 @@
 )
 
 
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
 
-RegistrationConfigTypeDef = TypedDict(
-    "RegistrationConfigTypeDef",
+RegistrationConfigOutputTypeDef = TypedDict(
+    "RegistrationConfigOutputTypeDef",
     {
         "DuplicateRegistrationAction": DuplicateRegistrationActionType,
         "FraudsterSimilarityThreshold": int,
         "WatchlistIds": List[str],
     },
     total=False,
 )
@@ -449,58 +468,33 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
     },
     total=False,
 )
 
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
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
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-        {
-            "DomainId": str,
-        },
-    )
-)
-_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-        {
-            "JobStatus": FraudsterRegistrationJobStatusType,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(
-    _RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-    _OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFraudsterRegistrationJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListFraudsterRegistrationJobsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListFraudsterRegistrationJobsRequestRequestTypeDef = TypedDict(
@@ -517,37 +511,14 @@
 class ListFraudsterRegistrationJobsRequestRequestTypeDef(
     _RequiredListFraudsterRegistrationJobsRequestRequestTypeDef,
     _OptionalListFraudsterRegistrationJobsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
-    "_RequiredListFraudstersRequestListFraudstersPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
-    "_OptionalListFraudstersRequestListFraudstersPaginateTypeDef",
-    {
-        "WatchlistId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFraudstersRequestListFraudstersPaginateTypeDef(
-    _RequiredListFraudstersRequestListFraudstersPaginateTypeDef,
-    _OptionalListFraudstersRequestListFraudstersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFraudstersRequestRequestTypeDef = TypedDict(
     "_RequiredListFraudstersRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListFraudstersRequestRequestTypeDef = TypedDict(
@@ -563,37 +534,14 @@
 
 class ListFraudstersRequestRequestTypeDef(
     _RequiredListFraudstersRequestRequestTypeDef, _OptionalListFraudstersRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
-    "_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
-    "_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    {
-        "JobStatus": SpeakerEnrollmentJobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(
-    _RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-    _OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListSpeakerEnrollmentJobsRequestRequestTypeDef = TypedDict(
@@ -610,36 +558,14 @@
 class ListSpeakerEnrollmentJobsRequestRequestTypeDef(
     _RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef,
     _OptionalListSpeakerEnrollmentJobsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
-    "_RequiredListSpeakersRequestListSpeakersPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
-    "_OptionalListSpeakersRequestListSpeakersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSpeakersRequestListSpeakersPaginateTypeDef(
-    _RequiredListSpeakersRequestListSpeakersPaginateTypeDef,
-    _OptionalListSpeakersRequestListSpeakersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSpeakersRequestRequestTypeDef = TypedDict(
     "_RequiredListSpeakersRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListSpeakersRequestRequestTypeDef = TypedDict(
@@ -675,36 +601,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
-    "_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
-    "_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListWatchlistsRequestListWatchlistsPaginateTypeDef(
-    _RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef,
-    _OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListWatchlistsRequestRequestTypeDef = TypedDict(
     "_RequiredListWatchlistsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListWatchlistsRequestRequestTypeDef = TypedDict(
@@ -741,35 +645,24 @@
     "OptOutSpeakerRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpeakerId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+RegistrationConfigTypeDef = TypedDict(
+    "RegistrationConfigTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DuplicateRegistrationAction": DuplicateRegistrationActionType,
+        "FraudsterSimilarityThreshold": int,
+        "WatchlistIds": Sequence[str],
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -797,31 +690,38 @@
     pass
 
 
 AssociateFraudsterResponseTypeDef = TypedDict(
     "AssociateFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFraudsterResponseTypeDef = TypedDict(
     "DescribeFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateFraudsterResponseTypeDef = TypedDict(
     "DisassociateFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthenticationResultTypeDef = TypedDict(
     "AuthenticationResultTypeDef",
     {
         "AudioAggregationEndedAt": datetime,
@@ -883,15 +783,15 @@
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
         "ResourceArn": str,
@@ -899,47 +799,47 @@
     },
 )
 
 CreateWatchlistResponseTypeDef = TypedDict(
     "CreateWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWatchlistResponseTypeDef = TypedDict(
     "DescribeWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWatchlistResponseTypeDef = TypedDict(
     "UpdateWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSpeakerResponseTypeDef = TypedDict(
     "DescribeSpeakerResponseTypeDef",
     {
         "Speaker": SpeakerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OptOutSpeakerResponseTypeDef = TypedDict(
     "OptOutSpeakerResponseTypeDef",
     {
         "Speaker": SpeakerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "Arn": str,
@@ -969,14 +869,23 @@
         "ServerSideEncryptionUpdateDetails": ServerSideEncryptionUpdateDetailsTypeDef,
         "UpdatedAt": datetime,
         "WatchlistDetails": WatchlistDetailsTypeDef,
     },
     total=False,
 )
 
+EnrollmentConfigOutputTypeDef = TypedDict(
+    "EnrollmentConfigOutputTypeDef",
+    {
+        "ExistingEnrollmentAction": ExistingEnrollmentActionType,
+        "FraudDetectionConfig": EnrollmentJobFraudDetectionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 EnrollmentConfigTypeDef = TypedDict(
     "EnrollmentConfigTypeDef",
     {
         "ExistingEnrollmentAction": ExistingEnrollmentActionType,
         "FraudDetectionConfig": EnrollmentJobFraudDetectionConfigTypeDef,
     },
     total=False,
@@ -1030,125 +939,252 @@
         "FailureDetails": FailureDetailsTypeDef,
         "InputDataConfig": InputDataConfigTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": FraudsterRegistrationJobStatusType,
         "OutputDataConfig": OutputDataConfigTypeDef,
-        "RegistrationConfig": RegistrationConfigTypeDef,
+        "RegistrationConfig": RegistrationConfigOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
+ListFraudstersResponseTypeDef = TypedDict(
+    "ListFraudstersResponseTypeDef",
+    {
+        "FraudsterSummaries": List[FraudsterSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+        {
+            "DomainId": str,
+        },
+    )
+)
+_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+        {
+            "JobStatus": FraudsterRegistrationJobStatusType,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(
+    _RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+    _OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
+    "_RequiredListFraudstersRequestListFraudstersPaginateTypeDef",
     {
-        "DataAccessRoleArn": str,
         "DomainId": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
     },
 )
-_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef",
+_OptionalListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
+    "_OptionalListFraudstersRequestListFraudstersPaginateTypeDef",
     {
-        "ClientToken": str,
-        "JobName": str,
-        "RegistrationConfig": RegistrationConfigTypeDef,
+        "WatchlistId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class StartFraudsterRegistrationJobRequestRequestTypeDef(
-    _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef,
-    _OptionalStartFraudsterRegistrationJobRequestRequestTypeDef,
+class ListFraudstersRequestListFraudstersPaginateTypeDef(
+    _RequiredListFraudstersRequestListFraudstersPaginateTypeDef,
+    _OptionalListFraudstersRequestListFraudstersPaginateTypeDef,
 ):
     pass
 
 
-ListFraudstersResponseTypeDef = TypedDict(
-    "ListFraudstersResponseTypeDef",
+_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
+    "_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     {
-        "FraudsterSummaries": List[FraudsterSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DomainId": str,
+    },
+)
+_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
+    "_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
+    {
+        "JobStatus": SpeakerEnrollmentJobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(
+    _RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+    _OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
+    "_RequiredListSpeakersRequestListSpeakersPaginateTypeDef",
+    {
+        "DomainId": str,
     },
 )
+_OptionalListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
+    "_OptionalListSpeakersRequestListSpeakersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSpeakersRequestListSpeakersPaginateTypeDef(
+    _RequiredListSpeakersRequestListSpeakersPaginateTypeDef,
+    _OptionalListSpeakersRequestListSpeakersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
+    "_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
+    "_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListWatchlistsRequestListWatchlistsPaginateTypeDef(
+    _RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef,
+    _OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef,
+):
+    pass
+
 
 ListSpeakersResponseTypeDef = TypedDict(
     "ListSpeakersResponseTypeDef",
     {
         "NextToken": str,
         "SpeakerSummaries": List[SpeakerSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWatchlistsResponseTypeDef = TypedDict(
     "ListWatchlistsResponseTypeDef",
     {
         "NextToken": str,
         "WatchlistSummaries": List[WatchlistSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RegistrationConfigUnionTypeDef = Union[RegistrationConfigTypeDef, RegistrationConfigOutputTypeDef]
+_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
+    {
+        "DataAccessRoleArn": str,
+        "DomainId": str,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+    },
+)
+_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "JobName": str,
+        "RegistrationConfig": RegistrationConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class StartFraudsterRegistrationJobRequestRequestTypeDef(
+    _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef,
+    _OptionalStartFraudsterRegistrationJobRequestRequestTypeDef,
+):
+    pass
+
+
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "DomainSummaries": List[DomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainResponseTypeDef = TypedDict(
     "UpdateDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SpeakerEnrollmentJobTypeDef = TypedDict(
     "SpeakerEnrollmentJobTypeDef",
     {
         "CreatedAt": datetime,
         "DataAccessRoleArn": str,
         "DomainId": str,
         "EndedAt": datetime,
-        "EnrollmentConfig": EnrollmentConfigTypeDef,
+        "EnrollmentConfig": EnrollmentConfigOutputTypeDef,
         "FailureDetails": FailureDetailsTypeDef,
         "InputDataConfig": InputDataConfigTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": SpeakerEnrollmentJobStatusType,
         "OutputDataConfig": OutputDataConfigTypeDef,
     },
     total=False,
 )
 
+EnrollmentConfigUnionTypeDef = Union[EnrollmentConfigTypeDef, EnrollmentConfigOutputTypeDef]
 _RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef",
     {
         "DataAccessRoleArn": str,
         "DomainId": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
@@ -1187,64 +1223,64 @@
 )
 
 ListFraudsterRegistrationJobsResponseTypeDef = TypedDict(
     "ListFraudsterRegistrationJobsResponseTypeDef",
     {
         "JobSummaries": List[FraudsterRegistrationJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpeakerEnrollmentJobsResponseTypeDef = TypedDict(
     "ListSpeakerEnrollmentJobsResponseTypeDef",
     {
         "JobSummaries": List[SpeakerEnrollmentJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFraudsterRegistrationJobResponseTypeDef = TypedDict(
     "DescribeFraudsterRegistrationJobResponseTypeDef",
     {
         "Job": FraudsterRegistrationJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFraudsterRegistrationJobResponseTypeDef = TypedDict(
     "StartFraudsterRegistrationJobResponseTypeDef",
     {
         "Job": FraudsterRegistrationJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSpeakerEnrollmentJobResponseTypeDef = TypedDict(
     "DescribeSpeakerEnrollmentJobResponseTypeDef",
     {
         "Job": SpeakerEnrollmentJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSpeakerEnrollmentJobResponseTypeDef = TypedDict(
     "StartSpeakerEnrollmentJobResponseTypeDef",
     {
         "Job": SpeakerEnrollmentJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EvaluateSessionResponseTypeDef = TypedDict(
     "EvaluateSessionResponseTypeDef",
     {
         "AuthenticationResult": AuthenticationResultTypeDef,
         "DomainId": str,
         "FraudDetectionResult": FraudDetectionResultTypeDef,
         "SessionId": str,
         "SessionName": str,
         "StreamingStatus": StreamingStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id/type_defs.pyi` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_voice_id.type_defs import AssociateFraudsterRequestRequestTypeDef
 
-    data: AssociateFraudsterRequestRequestTypeDef = {...}
+    data: AssociateFraudsterRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AuthenticationDecisionType,
     DomainStatusType,
     DuplicateRegistrationActionType,
     ExistingEnrollmentActionType,
     FraudDetectionActionType,
@@ -34,14 +34,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateFraudsterRequestRequestTypeDef",
     "FraudsterTypeDef",
+    "ResponseMetadataTypeDef",
     "AuthenticationConfigurationTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "TagTypeDef",
     "CreateWatchlistRequestRequestTypeDef",
     "WatchlistTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeleteFraudsterRequestRequestTypeDef",
@@ -53,75 +54,79 @@
     "DescribeSpeakerEnrollmentJobRequestRequestTypeDef",
     "DescribeSpeakerRequestRequestTypeDef",
     "SpeakerTypeDef",
     "DescribeWatchlistRequestRequestTypeDef",
     "DisassociateFraudsterRequestRequestTypeDef",
     "ServerSideEncryptionUpdateDetailsTypeDef",
     "WatchlistDetailsTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "EnrollmentJobFraudDetectionConfigOutputTypeDef",
     "EnrollmentJobFraudDetectionConfigTypeDef",
     "EvaluateSessionRequestRequestTypeDef",
     "FailureDetailsTypeDef",
     "FraudDetectionConfigurationTypeDef",
     "KnownFraudsterRiskTypeDef",
     "VoiceSpoofingRiskTypeDef",
     "JobProgressTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
-    "RegistrationConfigTypeDef",
+    "RegistrationConfigOutputTypeDef",
     "FraudsterSummaryTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDomainsRequestRequestTypeDef",
-    "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
     "ListFraudsterRegistrationJobsRequestRequestTypeDef",
-    "ListFraudstersRequestListFraudstersPaginateTypeDef",
     "ListFraudstersRequestRequestTypeDef",
-    "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     "ListSpeakerEnrollmentJobsRequestRequestTypeDef",
-    "ListSpeakersRequestListSpeakersPaginateTypeDef",
     "ListSpeakersRequestRequestTypeDef",
     "SpeakerSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListWatchlistsRequestRequestTypeDef",
     "WatchlistSummaryTypeDef",
     "OptOutSpeakerRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "RegistrationConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWatchlistRequestRequestTypeDef",
     "AssociateFraudsterResponseTypeDef",
     "DescribeFraudsterResponseTypeDef",
     "DisassociateFraudsterResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "AuthenticationResultTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateWatchlistResponseTypeDef",
     "DescribeWatchlistResponseTypeDef",
     "UpdateWatchlistResponseTypeDef",
     "DescribeSpeakerResponseTypeDef",
     "OptOutSpeakerResponseTypeDef",
     "DomainSummaryTypeDef",
     "DomainTypeDef",
+    "EnrollmentConfigOutputTypeDef",
     "EnrollmentConfigTypeDef",
     "FraudRiskDetailsTypeDef",
     "FraudsterRegistrationJobSummaryTypeDef",
     "SpeakerEnrollmentJobSummaryTypeDef",
     "FraudsterRegistrationJobTypeDef",
-    "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListFraudstersResponseTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+    "ListFraudstersRequestListFraudstersPaginateTypeDef",
+    "ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
+    "ListSpeakersRequestListSpeakersPaginateTypeDef",
+    "ListWatchlistsRequestListWatchlistsPaginateTypeDef",
     "ListSpeakersResponseTypeDef",
     "ListWatchlistsResponseTypeDef",
+    "RegistrationConfigUnionTypeDef",
+    "StartFraudsterRegistrationJobRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
     "CreateDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
     "SpeakerEnrollmentJobTypeDef",
+    "EnrollmentConfigUnionTypeDef",
     "StartSpeakerEnrollmentJobRequestRequestTypeDef",
     "FraudDetectionResultTypeDef",
     "ListFraudsterRegistrationJobsResponseTypeDef",
     "ListSpeakerEnrollmentJobsResponseTypeDef",
     "DescribeFraudsterRegistrationJobResponseTypeDef",
     "StartFraudsterRegistrationJobResponseTypeDef",
     "DescribeSpeakerEnrollmentJobResponseTypeDef",
@@ -145,14 +150,25 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
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
 AuthenticationConfigurationTypeDef = TypedDict(
     "AuthenticationConfigurationTypeDef",
     {
         "AcceptanceThreshold": int,
     },
 )
 
@@ -320,27 +336,30 @@
 WatchlistDetailsTypeDef = TypedDict(
     "WatchlistDetailsTypeDef",
     {
         "DefaultWatchlistId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+EnrollmentJobFraudDetectionConfigOutputTypeDef = TypedDict(
+    "EnrollmentJobFraudDetectionConfigOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FraudDetectionAction": FraudDetectionActionType,
+        "RiskThreshold": int,
+        "WatchlistIds": List[str],
     },
+    total=False,
 )
 
 EnrollmentJobFraudDetectionConfigTypeDef = TypedDict(
     "EnrollmentJobFraudDetectionConfigTypeDef",
     {
         "FraudDetectionAction": FraudDetectionActionType,
         "RiskThreshold": int,
-        "WatchlistIds": List[str],
+        "WatchlistIds": Sequence[str],
     },
     total=False,
 )
 
 EvaluateSessionRequestRequestTypeDef = TypedDict(
     "EvaluateSessionRequestRequestTypeDef",
     {
@@ -421,16 +440,16 @@
     },
     total=False,
 )
 
 class OutputDataConfigTypeDef(_RequiredOutputDataConfigTypeDef, _OptionalOutputDataConfigTypeDef):
     pass
 
-RegistrationConfigTypeDef = TypedDict(
-    "RegistrationConfigTypeDef",
+RegistrationConfigOutputTypeDef = TypedDict(
+    "RegistrationConfigOutputTypeDef",
     {
         "DuplicateRegistrationAction": DuplicateRegistrationActionType,
         "FraudsterSimilarityThreshold": int,
         "WatchlistIds": List[str],
     },
     total=False,
 )
@@ -442,56 +461,33 @@
         "DomainId": str,
         "GeneratedFraudsterId": str,
         "WatchlistIds": List[str],
     },
     total=False,
 )
 
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
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
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-        {
-            "DomainId": str,
-        },
-    )
-)
-_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
-        {
-            "JobStatus": FraudsterRegistrationJobStatusType,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(
-    _RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-    _OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
-):
-    pass
-
 _RequiredListFraudsterRegistrationJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListFraudsterRegistrationJobsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListFraudsterRegistrationJobsRequestRequestTypeDef = TypedDict(
@@ -506,35 +502,14 @@
 
 class ListFraudsterRegistrationJobsRequestRequestTypeDef(
     _RequiredListFraudsterRegistrationJobsRequestRequestTypeDef,
     _OptionalListFraudsterRegistrationJobsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
-    "_RequiredListFraudstersRequestListFraudstersPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
-    "_OptionalListFraudstersRequestListFraudstersPaginateTypeDef",
-    {
-        "WatchlistId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFraudstersRequestListFraudstersPaginateTypeDef(
-    _RequiredListFraudstersRequestListFraudstersPaginateTypeDef,
-    _OptionalListFraudstersRequestListFraudstersPaginateTypeDef,
-):
-    pass
-
 _RequiredListFraudstersRequestRequestTypeDef = TypedDict(
     "_RequiredListFraudstersRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListFraudstersRequestRequestTypeDef = TypedDict(
@@ -548,35 +523,14 @@
 )
 
 class ListFraudstersRequestRequestTypeDef(
     _RequiredListFraudstersRequestRequestTypeDef, _OptionalListFraudstersRequestRequestTypeDef
 ):
     pass
 
-_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
-    "_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
-    "_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
-    {
-        "JobStatus": SpeakerEnrollmentJobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(
-    _RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-    _OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
-):
-    pass
-
 _RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListSpeakerEnrollmentJobsRequestRequestTypeDef = TypedDict(
@@ -591,34 +545,14 @@
 
 class ListSpeakerEnrollmentJobsRequestRequestTypeDef(
     _RequiredListSpeakerEnrollmentJobsRequestRequestTypeDef,
     _OptionalListSpeakerEnrollmentJobsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
-    "_RequiredListSpeakersRequestListSpeakersPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
-    "_OptionalListSpeakersRequestListSpeakersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSpeakersRequestListSpeakersPaginateTypeDef(
-    _RequiredListSpeakersRequestListSpeakersPaginateTypeDef,
-    _OptionalListSpeakersRequestListSpeakersPaginateTypeDef,
-):
-    pass
-
 _RequiredListSpeakersRequestRequestTypeDef = TypedDict(
     "_RequiredListSpeakersRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListSpeakersRequestRequestTypeDef = TypedDict(
@@ -652,34 +586,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
-    "_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef",
-    {
-        "DomainId": str,
-    },
-)
-_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
-    "_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListWatchlistsRequestListWatchlistsPaginateTypeDef(
-    _RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef,
-    _OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef,
-):
-    pass
-
 _RequiredListWatchlistsRequestRequestTypeDef = TypedDict(
     "_RequiredListWatchlistsRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalListWatchlistsRequestRequestTypeDef = TypedDict(
@@ -714,35 +628,24 @@
     "OptOutSpeakerRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpeakerId": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+RegistrationConfigTypeDef = TypedDict(
+    "RegistrationConfigTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "DuplicateRegistrationAction": DuplicateRegistrationActionType,
+        "FraudsterSimilarityThreshold": int,
+        "WatchlistIds": Sequence[str],
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -768,31 +671,38 @@
 ):
     pass
 
 AssociateFraudsterResponseTypeDef = TypedDict(
     "AssociateFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFraudsterResponseTypeDef = TypedDict(
     "DescribeFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateFraudsterResponseTypeDef = TypedDict(
     "DisassociateFraudsterResponseTypeDef",
     {
         "Fraudster": FraudsterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthenticationResultTypeDef = TypedDict(
     "AuthenticationResultTypeDef",
     {
         "AudioAggregationEndedAt": datetime,
@@ -850,15 +760,15 @@
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
         "ResourceArn": str,
@@ -866,47 +776,47 @@
     },
 )
 
 CreateWatchlistResponseTypeDef = TypedDict(
     "CreateWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWatchlistResponseTypeDef = TypedDict(
     "DescribeWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateWatchlistResponseTypeDef = TypedDict(
     "UpdateWatchlistResponseTypeDef",
     {
         "Watchlist": WatchlistTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSpeakerResponseTypeDef = TypedDict(
     "DescribeSpeakerResponseTypeDef",
     {
         "Speaker": SpeakerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OptOutSpeakerResponseTypeDef = TypedDict(
     "OptOutSpeakerResponseTypeDef",
     {
         "Speaker": SpeakerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainSummaryTypeDef = TypedDict(
     "DomainSummaryTypeDef",
     {
         "Arn": str,
@@ -936,14 +846,23 @@
         "ServerSideEncryptionUpdateDetails": ServerSideEncryptionUpdateDetailsTypeDef,
         "UpdatedAt": datetime,
         "WatchlistDetails": WatchlistDetailsTypeDef,
     },
     total=False,
 )
 
+EnrollmentConfigOutputTypeDef = TypedDict(
+    "EnrollmentConfigOutputTypeDef",
+    {
+        "ExistingEnrollmentAction": ExistingEnrollmentActionType,
+        "FraudDetectionConfig": EnrollmentJobFraudDetectionConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 EnrollmentConfigTypeDef = TypedDict(
     "EnrollmentConfigTypeDef",
     {
         "ExistingEnrollmentAction": ExistingEnrollmentActionType,
         "FraudDetectionConfig": EnrollmentJobFraudDetectionConfigTypeDef,
     },
     total=False,
@@ -997,123 +916,240 @@
         "FailureDetails": FailureDetailsTypeDef,
         "InputDataConfig": InputDataConfigTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": FraudsterRegistrationJobStatusType,
         "OutputDataConfig": OutputDataConfigTypeDef,
-        "RegistrationConfig": RegistrationConfigTypeDef,
+        "RegistrationConfig": RegistrationConfigOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
+ListFraudstersResponseTypeDef = TypedDict(
+    "ListFraudstersResponseTypeDef",
+    {
+        "FraudsterSummaries": List[FraudsterSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+        {
+            "DomainId": str,
+        },
+    )
+)
+_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef",
+        {
+            "JobStatus": FraudsterRegistrationJobStatusType,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(
+    _RequiredListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+    _OptionalListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
+    "_RequiredListFraudstersRequestListFraudstersPaginateTypeDef",
     {
-        "DataAccessRoleArn": str,
         "DomainId": str,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
     },
 )
-_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef",
+_OptionalListFraudstersRequestListFraudstersPaginateTypeDef = TypedDict(
+    "_OptionalListFraudstersRequestListFraudstersPaginateTypeDef",
     {
-        "ClientToken": str,
-        "JobName": str,
-        "RegistrationConfig": RegistrationConfigTypeDef,
+        "WatchlistId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class StartFraudsterRegistrationJobRequestRequestTypeDef(
-    _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef,
-    _OptionalStartFraudsterRegistrationJobRequestRequestTypeDef,
+class ListFraudstersRequestListFraudstersPaginateTypeDef(
+    _RequiredListFraudstersRequestListFraudstersPaginateTypeDef,
+    _OptionalListFraudstersRequestListFraudstersPaginateTypeDef,
 ):
     pass
 
-ListFraudstersResponseTypeDef = TypedDict(
-    "ListFraudstersResponseTypeDef",
+_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
+    "_RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
     {
-        "FraudsterSummaries": List[FraudsterSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DomainId": str,
+    },
+)
+_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef = TypedDict(
+    "_OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef",
+    {
+        "JobStatus": SpeakerEnrollmentJobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(
+    _RequiredListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+    _OptionalListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
+    "_RequiredListSpeakersRequestListSpeakersPaginateTypeDef",
+    {
+        "DomainId": str,
+    },
+)
+_OptionalListSpeakersRequestListSpeakersPaginateTypeDef = TypedDict(
+    "_OptionalListSpeakersRequestListSpeakersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSpeakersRequestListSpeakersPaginateTypeDef(
+    _RequiredListSpeakersRequestListSpeakersPaginateTypeDef,
+    _OptionalListSpeakersRequestListSpeakersPaginateTypeDef,
+):
+    pass
+
+_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
+    "_RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    {
+        "DomainId": str,
     },
 )
+_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef = TypedDict(
+    "_OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListWatchlistsRequestListWatchlistsPaginateTypeDef(
+    _RequiredListWatchlistsRequestListWatchlistsPaginateTypeDef,
+    _OptionalListWatchlistsRequestListWatchlistsPaginateTypeDef,
+):
+    pass
 
 ListSpeakersResponseTypeDef = TypedDict(
     "ListSpeakersResponseTypeDef",
     {
         "NextToken": str,
         "SpeakerSummaries": List[SpeakerSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWatchlistsResponseTypeDef = TypedDict(
     "ListWatchlistsResponseTypeDef",
     {
         "NextToken": str,
         "WatchlistSummaries": List[WatchlistSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RegistrationConfigUnionTypeDef = Union[RegistrationConfigTypeDef, RegistrationConfigOutputTypeDef]
+_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFraudsterRegistrationJobRequestRequestTypeDef",
+    {
+        "DataAccessRoleArn": str,
+        "DomainId": str,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+    },
+)
+_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFraudsterRegistrationJobRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "JobName": str,
+        "RegistrationConfig": RegistrationConfigTypeDef,
+    },
+    total=False,
+)
+
+class StartFraudsterRegistrationJobRequestRequestTypeDef(
+    _RequiredStartFraudsterRegistrationJobRequestRequestTypeDef,
+    _OptionalStartFraudsterRegistrationJobRequestRequestTypeDef,
+):
+    pass
+
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "DomainSummaries": List[DomainSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDomainResponseTypeDef = TypedDict(
     "CreateDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDomainResponseTypeDef = TypedDict(
     "DescribeDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainResponseTypeDef = TypedDict(
     "UpdateDomainResponseTypeDef",
     {
         "Domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SpeakerEnrollmentJobTypeDef = TypedDict(
     "SpeakerEnrollmentJobTypeDef",
     {
         "CreatedAt": datetime,
         "DataAccessRoleArn": str,
         "DomainId": str,
         "EndedAt": datetime,
-        "EnrollmentConfig": EnrollmentConfigTypeDef,
+        "EnrollmentConfig": EnrollmentConfigOutputTypeDef,
         "FailureDetails": FailureDetailsTypeDef,
         "InputDataConfig": InputDataConfigTypeDef,
         "JobId": str,
         "JobName": str,
         "JobProgress": JobProgressTypeDef,
         "JobStatus": SpeakerEnrollmentJobStatusType,
         "OutputDataConfig": OutputDataConfigTypeDef,
     },
     total=False,
 )
 
+EnrollmentConfigUnionTypeDef = Union[EnrollmentConfigTypeDef, EnrollmentConfigOutputTypeDef]
 _RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartSpeakerEnrollmentJobRequestRequestTypeDef",
     {
         "DataAccessRoleArn": str,
         "DomainId": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
@@ -1150,64 +1186,64 @@
 )
 
 ListFraudsterRegistrationJobsResponseTypeDef = TypedDict(
     "ListFraudsterRegistrationJobsResponseTypeDef",
     {
         "JobSummaries": List[FraudsterRegistrationJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpeakerEnrollmentJobsResponseTypeDef = TypedDict(
     "ListSpeakerEnrollmentJobsResponseTypeDef",
     {
         "JobSummaries": List[SpeakerEnrollmentJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFraudsterRegistrationJobResponseTypeDef = TypedDict(
     "DescribeFraudsterRegistrationJobResponseTypeDef",
     {
         "Job": FraudsterRegistrationJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartFraudsterRegistrationJobResponseTypeDef = TypedDict(
     "StartFraudsterRegistrationJobResponseTypeDef",
     {
         "Job": FraudsterRegistrationJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSpeakerEnrollmentJobResponseTypeDef = TypedDict(
     "DescribeSpeakerEnrollmentJobResponseTypeDef",
     {
         "Job": SpeakerEnrollmentJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSpeakerEnrollmentJobResponseTypeDef = TypedDict(
     "StartSpeakerEnrollmentJobResponseTypeDef",
     {
         "Job": SpeakerEnrollmentJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EvaluateSessionResponseTypeDef = TypedDict(
     "EvaluateSessionResponseTypeDef",
     {
         "AuthenticationResult": AuthenticationResultTypeDef,
         "DomainId": str,
         "FraudDetectionResult": FraudDetectionResultTypeDef,
         "SessionId": str,
         "SessionName": str,
         "StreamingStatus": StreamingStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id.egg-info/PKG-INFO` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-voice-id
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.VoiceID 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.VoiceID 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore voice-id type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore voice-id type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-voice-id"></a>
 
 # types-aiobotocore-voice-id
 
 [![PyPI - types-aiobotocore-voice-id](https://img.shields.io/pypi/v/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-voice-id.svg?color=blue)](https://pypi.org/project/types-aiobotocore-voice-id)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-voice-id?color=blue)](https://pypistats.org/packages/types-aiobotocore-voice-id)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-voice-id)](https://pepy.tech/project/types-aiobotocore-voice-id)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.VoiceID 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
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
 [types-aiobotocore-voice-id docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_voice_id/).
 
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
@@ -337,25 +336,26 @@
 )
 
 
 def check_value(value: AuthenticationDecisionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_voice_id.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_voice_id.type_defs import (
     AssociateFraudsterRequestRequestTypeDef,
     FraudsterTypeDef,
+    ResponseMetadataTypeDef,
     AuthenticationConfigurationTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
     TagTypeDef,
     CreateWatchlistRequestRequestTypeDef,
     WatchlistTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DeleteFraudsterRequestRequestTypeDef,
@@ -367,88 +367,92 @@
     DescribeSpeakerEnrollmentJobRequestRequestTypeDef,
     DescribeSpeakerRequestRequestTypeDef,
     SpeakerTypeDef,
     DescribeWatchlistRequestRequestTypeDef,
     DisassociateFraudsterRequestRequestTypeDef,
     ServerSideEncryptionUpdateDetailsTypeDef,
     WatchlistDetailsTypeDef,
-    EmptyResponseMetadataTypeDef,
+    EnrollmentJobFraudDetectionConfigOutputTypeDef,
     EnrollmentJobFraudDetectionConfigTypeDef,
     EvaluateSessionRequestRequestTypeDef,
     FailureDetailsTypeDef,
     FraudDetectionConfigurationTypeDef,
     KnownFraudsterRiskTypeDef,
     VoiceSpoofingRiskTypeDef,
     JobProgressTypeDef,
     InputDataConfigTypeDef,
     OutputDataConfigTypeDef,
-    RegistrationConfigTypeDef,
+    RegistrationConfigOutputTypeDef,
     FraudsterSummaryTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDomainsRequestRequestTypeDef,
-    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
     ListFraudsterRegistrationJobsRequestRequestTypeDef,
-    ListFraudstersRequestListFraudstersPaginateTypeDef,
     ListFraudstersRequestRequestTypeDef,
-    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
     ListSpeakerEnrollmentJobsRequestRequestTypeDef,
-    ListSpeakersRequestListSpeakersPaginateTypeDef,
     ListSpeakersRequestRequestTypeDef,
     SpeakerSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListWatchlistsRequestRequestTypeDef,
     WatchlistSummaryTypeDef,
     OptOutSpeakerRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    RegistrationConfigTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateWatchlistRequestRequestTypeDef,
     AssociateFraudsterResponseTypeDef,
     DescribeFraudsterResponseTypeDef,
     DisassociateFraudsterResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     AuthenticationResultTypeDef,
     UpdateDomainRequestRequestTypeDef,
     CreateDomainRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateWatchlistResponseTypeDef,
     DescribeWatchlistResponseTypeDef,
     UpdateWatchlistResponseTypeDef,
     DescribeSpeakerResponseTypeDef,
     OptOutSpeakerResponseTypeDef,
     DomainSummaryTypeDef,
     DomainTypeDef,
+    EnrollmentConfigOutputTypeDef,
     EnrollmentConfigTypeDef,
     FraudRiskDetailsTypeDef,
     FraudsterRegistrationJobSummaryTypeDef,
     SpeakerEnrollmentJobSummaryTypeDef,
     FraudsterRegistrationJobTypeDef,
-    StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListFraudstersResponseTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef,
+    ListFraudstersRequestListFraudstersPaginateTypeDef,
+    ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef,
+    ListSpeakersRequestListSpeakersPaginateTypeDef,
+    ListWatchlistsRequestListWatchlistsPaginateTypeDef,
     ListSpeakersResponseTypeDef,
     ListWatchlistsResponseTypeDef,
+    RegistrationConfigUnionTypeDef,
+    StartFraudsterRegistrationJobRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
     CreateDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     UpdateDomainResponseTypeDef,
     SpeakerEnrollmentJobTypeDef,
+    EnrollmentConfigUnionTypeDef,
     StartSpeakerEnrollmentJobRequestRequestTypeDef,
     FraudDetectionResultTypeDef,
     ListFraudsterRegistrationJobsResponseTypeDef,
     ListSpeakerEnrollmentJobsResponseTypeDef,
     DescribeFraudsterRegistrationJobResponseTypeDef,
     StartFraudsterRegistrationJobResponseTypeDef,
     DescribeSpeakerEnrollmentJobResponseTypeDef,
     StartSpeakerEnrollmentJobResponseTypeDef,
     EvaluateSessionResponseTypeDef,
 )
 
 
-def get_structure() -> AssociateFraudsterRequestRequestTypeDef:
+def get_value() -> AssociateFraudsterRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-voice-id-2.5.2/types_aiobotocore_voice_id.egg-info/SOURCES.txt` & `types-aiobotocore-voice-id-2.5.2.post1/types_aiobotocore_voice_id.egg-info/SOURCES.txt`

 * *Files identical despite different names*


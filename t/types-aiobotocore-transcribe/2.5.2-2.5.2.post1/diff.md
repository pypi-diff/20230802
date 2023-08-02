# Comparing `tmp/types-aiobotocore-transcribe-2.5.2.tar.gz` & `tmp/types-aiobotocore-transcribe-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-transcribe-2.5.2.tar", last modified: Sat Jul  8 01:44:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-transcribe-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:08 2023, max compression
```

## Comparing `types-aiobotocore-transcribe-2.5.2.tar` & `types-aiobotocore-transcribe-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:26.147010 types-aiobotocore-transcribe-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:03.000000 types-aiobotocore-transcribe-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-07-08 01:44:26.135010 types-aiobotocore-transcribe-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-07-08 01:42:03.000000 types-aiobotocore-transcribe-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:26.147010 types-aiobotocore-transcribe-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-08 01:42:03.000000 types-aiobotocore-transcribe-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:26.135010 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-08 01:42:03.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-08 01:42:03.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-08 01:42:03.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31721 2023-07-08 01:42:03.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31673 2023-07-08 01:42:03.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-07-08 01:42:03.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-07-08 01:42:03.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:03.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39213 2023-07-08 01:42:04.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39182 2023-07-08 01:42:04.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:03.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:26.135010 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16882 2023-07-08 01:44:25.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-08 01:44:25.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:25.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:25.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:25.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:44:25.000000 types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.081435 types-aiobotocore-transcribe-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-08-02 14:53:08.081435 types-aiobotocore-transcribe-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:08.081435 types-aiobotocore-transcribe-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.081435 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31820 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31772 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10452 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42322 2023-08-02 14:50:42.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42286 2023-08-02 14:50:42.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:41.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.081435 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-08-02 14:53:07.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 14:53:07.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:07.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:07.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:07.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:53:07.000000 types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-transcribe-2.5.2/LICENSE` & `types-aiobotocore-transcribe-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.5.2/PKG-INFO` & `types-aiobotocore-transcribe-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-transcribe
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.TranscribeService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.TranscribeService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore transcribe type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore transcribe type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-transcribe"></a>
 
 # types-aiobotocore-transcribe
 
 [![PyPI - types-aiobotocore-transcribe](https://img.shields.io/pypi/v/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-transcribe?color=blue)](https://pypistats.org/packages/types-aiobotocore-transcribe)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transcribe)](https://pepy.tech/project/types-aiobotocore-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.TranscribeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [types-aiobotocore-transcribe docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/).
 
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
@@ -301,55 +300,50 @@
 )
 
 
 def check_value(value: BaseModelNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_transcribe.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_transcribe.type_defs import (
     AbsoluteTimeRangeTypeDef,
-    ContentRedactionTypeDef,
+    ContentRedactionOutputTypeDef,
     LanguageIdSettingsTypeDef,
+    ContentRedactionTypeDef,
     CallAnalyticsJobSummaryTypeDef,
     ChannelDefinitionTypeDef,
     MediaTypeDef,
     TranscriptTypeDef,
+    ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
-    CreateMedicalVocabularyResponseTypeDef,
-    CreateVocabularyFilterResponseTypeDef,
-    CreateVocabularyResponseTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
     DescribeLanguageModelRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
-    GetMedicalVocabularyResponseTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
-    GetVocabularyFilterResponseTypeDef,
     GetVocabularyRequestRequestTypeDef,
-    GetVocabularyResponseTypeDef,
     RelativeTimeRangeTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
@@ -360,71 +354,84 @@
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
     MedicalTranscriptTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
-    ResponseMetadataTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
     SubtitlesOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
-    UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterRequestRequestTypeDef,
-    UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyRequestRequestTypeDef,
-    UpdateVocabularyResponseTypeDef,
+    CallAnalyticsJobSettingsOutputTypeDef,
     CallAnalyticsJobSettingsTypeDef,
+    ContentRedactionUnionTypeDef,
+    CreateMedicalVocabularyResponseTypeDef,
+    CreateVocabularyFilterResponseTypeDef,
+    CreateVocabularyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetMedicalVocabularyResponseTypeDef,
+    GetVocabularyFilterResponseTypeDef,
+    GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
+    UpdateMedicalVocabularyResponseTypeDef,
+    UpdateVocabularyFilterResponseTypeDef,
+    UpdateVocabularyResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     LanguageModelTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     InterruptionFilterTypeDef,
     NonTalkTimeFilterTypeDef,
+    SentimentFilterOutputTypeDef,
     SentimentFilterTypeDef,
+    TranscriptFilterOutputTypeDef,
     TranscriptFilterTypeDef,
     ListMedicalTranscriptionJobsResponseTypeDef,
     ListMedicalVocabulariesResponseTypeDef,
     ListVocabulariesResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MedicalTranscriptionJobTypeDef,
     StartMedicalTranscriptionJobRequestRequestTypeDef,
     TranscriptionJobSummaryTypeDef,
     StartTranscriptionJobRequestRequestTypeDef,
     TranscriptionJobTypeDef,
     CallAnalyticsJobTypeDef,
+    CallAnalyticsJobSettingsUnionTypeDef,
     StartCallAnalyticsJobRequestRequestTypeDef,
     DescribeLanguageModelResponseTypeDef,
     ListLanguageModelsResponseTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     GetMedicalTranscriptionJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     ListTranscriptionJobsResponseTypeDef,
     GetTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     GetCallAnalyticsJobResponseTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     CategoryPropertiesTypeDef,
-    CreateCallAnalyticsCategoryRequestRequestTypeDef,
-    UpdateCallAnalyticsCategoryRequestRequestTypeDef,
+    RuleUnionTypeDef,
     CreateCallAnalyticsCategoryResponseTypeDef,
     GetCallAnalyticsCategoryResponseTypeDef,
     ListCallAnalyticsCategoriesResponseTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
+    CreateCallAnalyticsCategoryRequestRequestTypeDef,
+    UpdateCallAnalyticsCategoryRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbsoluteTimeRangeTypeDef:
+def get_value() -> AbsoluteTimeRangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-transcribe-2.5.2/README.md` & `types-aiobotocore-transcribe-2.5.2.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-transcribe"></a>
 
 # types-aiobotocore-transcribe
 
 [![PyPI - types-aiobotocore-transcribe](https://img.shields.io/pypi/v/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-transcribe?color=blue)](https://pypistats.org/packages/types-aiobotocore-transcribe)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transcribe)](https://pepy.tech/project/types-aiobotocore-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.TranscribeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [types-aiobotocore-transcribe docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/).
 
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
@@ -268,55 +268,50 @@
 )
 
 
 def check_value(value: BaseModelNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_transcribe.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_transcribe.type_defs import (
     AbsoluteTimeRangeTypeDef,
-    ContentRedactionTypeDef,
+    ContentRedactionOutputTypeDef,
     LanguageIdSettingsTypeDef,
+    ContentRedactionTypeDef,
     CallAnalyticsJobSummaryTypeDef,
     ChannelDefinitionTypeDef,
     MediaTypeDef,
     TranscriptTypeDef,
+    ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
-    CreateMedicalVocabularyResponseTypeDef,
-    CreateVocabularyFilterResponseTypeDef,
-    CreateVocabularyResponseTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
     DescribeLanguageModelRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
-    GetMedicalVocabularyResponseTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
-    GetVocabularyFilterResponseTypeDef,
     GetVocabularyRequestRequestTypeDef,
-    GetVocabularyResponseTypeDef,
     RelativeTimeRangeTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
@@ -327,71 +322,84 @@
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
     MedicalTranscriptTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
-    ResponseMetadataTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
     SubtitlesOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
-    UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterRequestRequestTypeDef,
-    UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyRequestRequestTypeDef,
-    UpdateVocabularyResponseTypeDef,
+    CallAnalyticsJobSettingsOutputTypeDef,
     CallAnalyticsJobSettingsTypeDef,
+    ContentRedactionUnionTypeDef,
+    CreateMedicalVocabularyResponseTypeDef,
+    CreateVocabularyFilterResponseTypeDef,
+    CreateVocabularyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetMedicalVocabularyResponseTypeDef,
+    GetVocabularyFilterResponseTypeDef,
+    GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
+    UpdateMedicalVocabularyResponseTypeDef,
+    UpdateVocabularyFilterResponseTypeDef,
+    UpdateVocabularyResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     LanguageModelTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     InterruptionFilterTypeDef,
     NonTalkTimeFilterTypeDef,
+    SentimentFilterOutputTypeDef,
     SentimentFilterTypeDef,
+    TranscriptFilterOutputTypeDef,
     TranscriptFilterTypeDef,
     ListMedicalTranscriptionJobsResponseTypeDef,
     ListMedicalVocabulariesResponseTypeDef,
     ListVocabulariesResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MedicalTranscriptionJobTypeDef,
     StartMedicalTranscriptionJobRequestRequestTypeDef,
     TranscriptionJobSummaryTypeDef,
     StartTranscriptionJobRequestRequestTypeDef,
     TranscriptionJobTypeDef,
     CallAnalyticsJobTypeDef,
+    CallAnalyticsJobSettingsUnionTypeDef,
     StartCallAnalyticsJobRequestRequestTypeDef,
     DescribeLanguageModelResponseTypeDef,
     ListLanguageModelsResponseTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     GetMedicalTranscriptionJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     ListTranscriptionJobsResponseTypeDef,
     GetTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     GetCallAnalyticsJobResponseTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     CategoryPropertiesTypeDef,
-    CreateCallAnalyticsCategoryRequestRequestTypeDef,
-    UpdateCallAnalyticsCategoryRequestRequestTypeDef,
+    RuleUnionTypeDef,
     CreateCallAnalyticsCategoryResponseTypeDef,
     GetCallAnalyticsCategoryResponseTypeDef,
     ListCallAnalyticsCategoriesResponseTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
+    CreateCallAnalyticsCategoryRequestRequestTypeDef,
+    UpdateCallAnalyticsCategoryRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbsoluteTimeRangeTypeDef:
+def get_value() -> AbsoluteTimeRangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-transcribe-2.5.2/setup.py` & `types-aiobotocore-transcribe-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-transcribe",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_transcribe"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.TranscribeService 2.5.2 service generated with"
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
-    keywords="aiobotocore transcribe type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore transcribe type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_transcribe": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/"
```

### Comparing `types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/__main__.py` & `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.TranscribeService 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.TranscribeService 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService\nOther"
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

### Comparing `types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/client.py` & `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     MediaFormatType,
     ModelStatusType,
     TranscriptionJobStatusType,
     TypeType,
     VocabularyStateType,
 )
 from .type_defs import (
-    CallAnalyticsJobSettingsTypeDef,
+    CallAnalyticsJobSettingsUnionTypeDef,
     ChannelDefinitionTypeDef,
-    ContentRedactionTypeDef,
+    ContentRedactionUnionTypeDef,
     CreateCallAnalyticsCategoryResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     CreateMedicalVocabularyResponseTypeDef,
     CreateVocabularyFilterResponseTypeDef,
     CreateVocabularyResponseTypeDef,
     DescribeLanguageModelResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -61,15 +61,15 @@
     ListTagsForResourceResponseTypeDef,
     ListTranscriptionJobsResponseTypeDef,
     ListVocabulariesResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MediaTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
-    RuleTypeDef,
+    RuleUnionTypeDef,
     SettingsTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     SubtitlesTypeDef,
     TagTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
@@ -134,15 +134,19 @@
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#close)
         """
 
     async def create_call_analytics_category(
-        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
+        self,
+        *,
+        CategoryName: str,
+        Rules: Sequence[RuleUnionTypeDef],
+        InputType: InputTypeType = ...
     ) -> CreateCallAnalyticsCategoryResponseTypeDef:
         """
         Creates a new Call Analytics category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_call_analytics_category)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#create_call_analytics_category)
         """
@@ -503,15 +507,15 @@
         self,
         *,
         CallAnalyticsJobName: str,
         Media: MediaTypeDef,
         OutputLocation: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         DataAccessRoleArn: str = ...,
-        Settings: CallAnalyticsJobSettingsTypeDef = ...,
+        Settings: CallAnalyticsJobSettingsUnionTypeDef = ...,
         ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...
     ) -> StartCallAnalyticsJobResponseTypeDef:
         """
         Transcribes the audio from a customer service call and applies any additional
         Request Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_call_analytics_job)
@@ -555,15 +559,15 @@
         OutputBucketName: str = ...,
         OutputKey: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         Settings: SettingsTypeDef = ...,
         ModelSettings: ModelSettingsTypeDef = ...,
         JobExecutionSettings: JobExecutionSettingsTypeDef = ...,
-        ContentRedaction: ContentRedactionTypeDef = ...,
+        ContentRedaction: ContentRedactionUnionTypeDef = ...,
         IdentifyLanguage: bool = ...,
         IdentifyMultipleLanguages: bool = ...,
         LanguageOptions: Sequence[LanguageCodeType] = ...,
         Subtitles: SubtitlesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...
     ) -> StartTranscriptionJobResponseTypeDef:
@@ -589,15 +593,19 @@
         Removes the specified tags from the specified Amazon Transcribe resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#untag_resource)
         """
 
     async def update_call_analytics_category(
-        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
+        self,
+        *,
+        CategoryName: str,
+        Rules: Sequence[RuleUnionTypeDef],
+        InputType: InputTypeType = ...
     ) -> UpdateCallAnalyticsCategoryResponseTypeDef:
         """
         Updates the specified Call Analytics category with new rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_call_analytics_category)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#update_call_analytics_category)
         """
```

### Comparing `types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/client.pyi` & `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
     MediaFormatType,
     ModelStatusType,
     TranscriptionJobStatusType,
     TypeType,
     VocabularyStateType,
 )
 from .type_defs import (
-    CallAnalyticsJobSettingsTypeDef,
+    CallAnalyticsJobSettingsUnionTypeDef,
     ChannelDefinitionTypeDef,
-    ContentRedactionTypeDef,
+    ContentRedactionUnionTypeDef,
     CreateCallAnalyticsCategoryResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     CreateMedicalVocabularyResponseTypeDef,
     CreateVocabularyFilterResponseTypeDef,
     CreateVocabularyResponseTypeDef,
     DescribeLanguageModelResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -61,15 +61,15 @@
     ListTagsForResourceResponseTypeDef,
     ListTranscriptionJobsResponseTypeDef,
     ListVocabulariesResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MediaTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
-    RuleTypeDef,
+    RuleUnionTypeDef,
     SettingsTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     SubtitlesTypeDef,
     TagTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
@@ -127,15 +127,19 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#close)
         """
     async def create_call_analytics_category(
-        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
+        self,
+        *,
+        CategoryName: str,
+        Rules: Sequence[RuleUnionTypeDef],
+        InputType: InputTypeType = ...
     ) -> CreateCallAnalyticsCategoryResponseTypeDef:
         """
         Creates a new Call Analytics category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_call_analytics_category)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#create_call_analytics_category)
         """
@@ -465,15 +469,15 @@
         self,
         *,
         CallAnalyticsJobName: str,
         Media: MediaTypeDef,
         OutputLocation: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         DataAccessRoleArn: str = ...,
-        Settings: CallAnalyticsJobSettingsTypeDef = ...,
+        Settings: CallAnalyticsJobSettingsUnionTypeDef = ...,
         ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...
     ) -> StartCallAnalyticsJobResponseTypeDef:
         """
         Transcribes the audio from a customer service call and applies any additional
         Request Parameters you choose to include in your request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_call_analytics_job)
@@ -515,15 +519,15 @@
         OutputBucketName: str = ...,
         OutputKey: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         Settings: SettingsTypeDef = ...,
         ModelSettings: ModelSettingsTypeDef = ...,
         JobExecutionSettings: JobExecutionSettingsTypeDef = ...,
-        ContentRedaction: ContentRedactionTypeDef = ...,
+        ContentRedaction: ContentRedactionUnionTypeDef = ...,
         IdentifyLanguage: bool = ...,
         IdentifyMultipleLanguages: bool = ...,
         LanguageOptions: Sequence[LanguageCodeType] = ...,
         Subtitles: SubtitlesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...
     ) -> StartTranscriptionJobResponseTypeDef:
@@ -546,15 +550,19 @@
         """
         Removes the specified tags from the specified Amazon Transcribe resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#untag_resource)
         """
     async def update_call_analytics_category(
-        self, *, CategoryName: str, Rules: Sequence[RuleTypeDef], InputType: InputTypeType = ...
+        self,
+        *,
+        CategoryName: str,
+        Rules: Sequence[RuleUnionTypeDef],
+        InputType: InputTypeType = ...
     ) -> UpdateCallAnalyticsCategoryResponseTypeDef:
         """
         Updates the specified Call Analytics category with new rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_call_analytics_category)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#update_call_analytics_category)
         """
```

### Comparing `types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/literals.py` & `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/literals.pyi` & `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/type_defs.py` & `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_transcribe.type_defs import AbsoluteTimeRangeTypeDef
 
-    data: AbsoluteTimeRangeTypeDef = {...}
+    data: AbsoluteTimeRangeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BaseModelNameType,
     CallAnalyticsJobStatusType,
     CLMLanguageCodeType,
     InputTypeType,
     LanguageCodeType,
@@ -40,48 +40,42 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbsoluteTimeRangeTypeDef",
-    "ContentRedactionTypeDef",
+    "ContentRedactionOutputTypeDef",
     "LanguageIdSettingsTypeDef",
+    "ContentRedactionTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
     "ChannelDefinitionTypeDef",
     "MediaTypeDef",
     "TranscriptTypeDef",
+    "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
-    "CreateMedicalVocabularyResponseTypeDef",
-    "CreateVocabularyFilterResponseTypeDef",
-    "CreateVocabularyResponseTypeDef",
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     "DeleteCallAnalyticsJobRequestRequestTypeDef",
     "DeleteLanguageModelRequestRequestTypeDef",
     "DeleteMedicalTranscriptionJobRequestRequestTypeDef",
     "DeleteMedicalVocabularyRequestRequestTypeDef",
     "DeleteTranscriptionJobRequestRequestTypeDef",
     "DeleteVocabularyFilterRequestRequestTypeDef",
     "DeleteVocabularyRequestRequestTypeDef",
     "DescribeLanguageModelRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     "GetCallAnalyticsJobRequestRequestTypeDef",
     "GetMedicalTranscriptionJobRequestRequestTypeDef",
     "GetMedicalVocabularyRequestRequestTypeDef",
-    "GetMedicalVocabularyResponseTypeDef",
     "GetTranscriptionJobRequestRequestTypeDef",
     "GetVocabularyFilterRequestRequestTypeDef",
-    "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyRequestRequestTypeDef",
-    "GetVocabularyResponseTypeDef",
     "RelativeTimeRangeTypeDef",
     "JobExecutionSettingsTypeDef",
     "LanguageCodeItemTypeDef",
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     "ListCallAnalyticsJobsRequestRequestTypeDef",
     "ListLanguageModelsRequestRequestTypeDef",
     "ListMedicalTranscriptionJobsRequestRequestTypeDef",
@@ -92,110 +86,141 @@
     "ListTranscriptionJobsRequestRequestTypeDef",
     "ListVocabulariesRequestRequestTypeDef",
     "ListVocabularyFiltersRequestRequestTypeDef",
     "VocabularyFilterInfoTypeDef",
     "MedicalTranscriptTypeDef",
     "MedicalTranscriptionSettingTypeDef",
     "ModelSettingsTypeDef",
-    "ResponseMetadataTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
     "SubtitlesOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
-    "UpdateMedicalVocabularyResponseTypeDef",
     "UpdateVocabularyFilterRequestRequestTypeDef",
-    "UpdateVocabularyFilterResponseTypeDef",
     "UpdateVocabularyRequestRequestTypeDef",
-    "UpdateVocabularyResponseTypeDef",
+    "CallAnalyticsJobSettingsOutputTypeDef",
     "CallAnalyticsJobSettingsTypeDef",
+    "ContentRedactionUnionTypeDef",
+    "CreateMedicalVocabularyResponseTypeDef",
+    "CreateVocabularyFilterResponseTypeDef",
+    "CreateVocabularyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetMedicalVocabularyResponseTypeDef",
+    "GetVocabularyFilterResponseTypeDef",
+    "GetVocabularyResponseTypeDef",
     "ListCallAnalyticsJobsResponseTypeDef",
+    "UpdateMedicalVocabularyResponseTypeDef",
+    "UpdateVocabularyFilterResponseTypeDef",
+    "UpdateVocabularyResponseTypeDef",
     "CreateLanguageModelResponseTypeDef",
     "LanguageModelTypeDef",
     "CreateLanguageModelRequestRequestTypeDef",
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "InterruptionFilterTypeDef",
     "NonTalkTimeFilterTypeDef",
+    "SentimentFilterOutputTypeDef",
     "SentimentFilterTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "TranscriptFilterTypeDef",
     "ListMedicalTranscriptionJobsResponseTypeDef",
     "ListMedicalVocabulariesResponseTypeDef",
     "ListVocabulariesResponseTypeDef",
     "ListVocabularyFiltersResponseTypeDef",
     "MedicalTranscriptionJobTypeDef",
     "StartMedicalTranscriptionJobRequestRequestTypeDef",
     "TranscriptionJobSummaryTypeDef",
     "StartTranscriptionJobRequestRequestTypeDef",
     "TranscriptionJobTypeDef",
     "CallAnalyticsJobTypeDef",
+    "CallAnalyticsJobSettingsUnionTypeDef",
     "StartCallAnalyticsJobRequestRequestTypeDef",
     "DescribeLanguageModelResponseTypeDef",
     "ListLanguageModelsResponseTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
     "GetMedicalTranscriptionJobResponseTypeDef",
     "StartMedicalTranscriptionJobResponseTypeDef",
     "ListTranscriptionJobsResponseTypeDef",
     "GetTranscriptionJobResponseTypeDef",
     "StartTranscriptionJobResponseTypeDef",
     "GetCallAnalyticsJobResponseTypeDef",
     "StartCallAnalyticsJobResponseTypeDef",
     "CategoryPropertiesTypeDef",
-    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
-    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
+    "RuleUnionTypeDef",
     "CreateCallAnalyticsCategoryResponseTypeDef",
     "GetCallAnalyticsCategoryResponseTypeDef",
     "ListCallAnalyticsCategoriesResponseTypeDef",
     "UpdateCallAnalyticsCategoryResponseTypeDef",
+    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
+    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
 )
 
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
-_RequiredContentRedactionTypeDef = TypedDict(
-    "_RequiredContentRedactionTypeDef",
+_RequiredContentRedactionOutputTypeDef = TypedDict(
+    "_RequiredContentRedactionOutputTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
     },
 )
-_OptionalContentRedactionTypeDef = TypedDict(
-    "_OptionalContentRedactionTypeDef",
+_OptionalContentRedactionOutputTypeDef = TypedDict(
+    "_OptionalContentRedactionOutputTypeDef",
     {
         "PiiEntityTypes": List[PiiEntityTypeType],
     },
     total=False,
 )
 
-
-class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
+class ContentRedactionOutputTypeDef(
+    _RequiredContentRedactionOutputTypeDef, _OptionalContentRedactionOutputTypeDef
+):
     pass
 
-
 LanguageIdSettingsTypeDef = TypedDict(
     "LanguageIdSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "LanguageModelName": str,
     },
     total=False,
 )
 
+_RequiredContentRedactionTypeDef = TypedDict(
+    "_RequiredContentRedactionTypeDef",
+    {
+        "RedactionType": Literal["PII"],
+        "RedactionOutput": RedactionOutputType,
+    },
+)
+_OptionalContentRedactionTypeDef = TypedDict(
+    "_OptionalContentRedactionTypeDef",
+    {
+        "PiiEntityTypes": Sequence[PiiEntityTypeType],
+    },
+    total=False,
+)
+
+class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
+    pass
+
 CallAnalyticsJobSummaryTypeDef = TypedDict(
     "CallAnalyticsJobSummaryTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
@@ -229,14 +254,25 @@
     {
         "TranscriptFileUri": str,
         "RedactedTranscriptFileUri": str,
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
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "S3Uri": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -244,61 +280,25 @@
     "_OptionalInputDataConfigTypeDef",
     {
         "TuningDataS3Uri": str,
     },
     total=False,
 )
 
-
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateMedicalVocabularyResponseTypeDef = TypedDict(
-    "CreateMedicalVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVocabularyFilterResponseTypeDef = TypedDict(
-    "CreateVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVocabularyResponseTypeDef = TypedDict(
-    "CreateVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -354,21 +354,14 @@
 DescribeLanguageModelRequestRequestTypeDef = TypedDict(
     "DescribeLanguageModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -389,72 +382,35 @@
 GetMedicalVocabularyRequestRequestTypeDef = TypedDict(
     "GetMedicalVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
-GetMedicalVocabularyResponseTypeDef = TypedDict(
-    "GetMedicalVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "DownloadUri": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTranscriptionJobRequestRequestTypeDef = TypedDict(
     "GetTranscriptionJobRequestRequestTypeDef",
     {
         "TranscriptionJobName": str,
     },
 )
 
 GetVocabularyFilterRequestRequestTypeDef = TypedDict(
     "GetVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
     },
 )
 
-GetVocabularyFilterResponseTypeDef = TypedDict(
-    "GetVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "DownloadUri": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVocabularyRequestRequestTypeDef = TypedDict(
     "GetVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
-GetVocabularyResponseTypeDef = TypedDict(
-    "GetVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "DownloadUri": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RelativeTimeRangeTypeDef = TypedDict(
     "RelativeTimeRangeTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
         "First": int,
         "Last": int,
@@ -636,25 +592,14 @@
     "ModelSettingsTypeDef",
     {
         "LanguageModelName": str,
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
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "VocabularyName": str,
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
         "ChannelIdentification": bool,
@@ -698,25 +643,14 @@
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "VocabularyFileUri": str,
     },
 )
 
-UpdateMedicalVocabularyResponseTypeDef = TypedDict(
-    "UpdateMedicalVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "VocabularyState": VocabularyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVocabularyFilterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
     },
 )
 _OptionalUpdateVocabularyFilterRequestRequestTypeDef = TypedDict(
@@ -725,32 +659,20 @@
         "Words": Sequence[str],
         "VocabularyFilterFileUri": str,
         "DataAccessRoleArn": str,
     },
     total=False,
 )
 
-
 class UpdateVocabularyFilterRequestRequestTypeDef(
     _RequiredUpdateVocabularyFilterRequestRequestTypeDef,
     _OptionalUpdateVocabularyFilterRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateVocabularyFilterResponseTypeDef = TypedDict(
-    "UpdateVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -760,65 +682,177 @@
         "Phrases": Sequence[str],
         "VocabularyFileUri": str,
         "DataAccessRoleArn": str,
     },
     total=False,
 )
 
-
 class UpdateVocabularyRequestRequestTypeDef(
     _RequiredUpdateVocabularyRequestRequestTypeDef, _OptionalUpdateVocabularyRequestRequestTypeDef
 ):
     pass
 
-
-UpdateVocabularyResponseTypeDef = TypedDict(
-    "UpdateVocabularyResponseTypeDef",
+CallAnalyticsJobSettingsOutputTypeDef = TypedDict(
+    "CallAnalyticsJobSettingsOutputTypeDef",
     {
         "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "VocabularyState": VocabularyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+        "LanguageModelName": str,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
+        "LanguageOptions": List[LanguageCodeType],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
     },
+    total=False,
 )
 
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "ContentRedaction": ContentRedactionTypeDef,
-        "LanguageOptions": List[LanguageCodeType],
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageOptions": Sequence[LanguageCodeType],
+        "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
     },
     total=False,
 )
 
+ContentRedactionUnionTypeDef = Union[ContentRedactionTypeDef, ContentRedactionOutputTypeDef]
+CreateMedicalVocabularyResponseTypeDef = TypedDict(
+    "CreateMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVocabularyFilterResponseTypeDef = TypedDict(
+    "CreateVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVocabularyResponseTypeDef = TypedDict(
+    "CreateVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
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
+GetMedicalVocabularyResponseTypeDef = TypedDict(
+    "GetMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "DownloadUri": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVocabularyFilterResponseTypeDef = TypedDict(
+    "GetVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "DownloadUri": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVocabularyResponseTypeDef = TypedDict(
+    "GetVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "DownloadUri": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCallAnalyticsJobsResponseTypeDef = TypedDict(
     "ListCallAnalyticsJobsResponseTypeDef",
     {
         "Status": CallAnalyticsJobStatusType,
         "NextToken": str,
         "CallAnalyticsJobSummaries": List[CallAnalyticsJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMedicalVocabularyResponseTypeDef = TypedDict(
+    "UpdateMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "VocabularyState": VocabularyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVocabularyFilterResponseTypeDef = TypedDict(
+    "UpdateVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVocabularyResponseTypeDef = TypedDict(
+    "UpdateVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "VocabularyState": VocabularyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLanguageModelResponseTypeDef = TypedDict(
     "CreateLanguageModelResponseTypeDef",
     {
         "LanguageCode": CLMLanguageCodeType,
         "BaseModelName": BaseModelNameType,
         "ModelName": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "ModelStatus": ModelStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LanguageModelTypeDef = TypedDict(
     "LanguageModelTypeDef",
     {
         "ModelName": str,
@@ -847,22 +881,20 @@
     "_OptionalCreateLanguageModelRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateLanguageModelRequestRequestTypeDef(
     _RequiredCreateLanguageModelRequestRequestTypeDef,
     _OptionalCreateLanguageModelRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateMedicalVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMedicalVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "VocabularyFileUri": str,
     },
@@ -871,22 +903,20 @@
     "_OptionalCreateMedicalVocabularyRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateMedicalVocabularyRequestRequestTypeDef(
     _RequiredCreateMedicalVocabularyRequestRequestTypeDef,
     _OptionalCreateMedicalVocabularyRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateVocabularyFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -897,22 +927,20 @@
         "VocabularyFilterFileUri": str,
         "Tags": Sequence[TagTypeDef],
         "DataAccessRoleArn": str,
     },
     total=False,
 )
 
-
 class CreateVocabularyFilterRequestRequestTypeDef(
     _RequiredCreateVocabularyFilterRequestRequestTypeDef,
     _OptionalCreateVocabularyFilterRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -923,27 +951,25 @@
         "VocabularyFileUri": str,
         "Tags": Sequence[TagTypeDef],
         "DataAccessRoleArn": str,
     },
     total=False,
 )
 
-
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -970,14 +996,36 @@
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
         "Negate": bool,
     },
     total=False,
 )
 
+_RequiredSentimentFilterOutputTypeDef = TypedDict(
+    "_RequiredSentimentFilterOutputTypeDef",
+    {
+        "Sentiments": List[SentimentValueType],
+    },
+)
+_OptionalSentimentFilterOutputTypeDef = TypedDict(
+    "_OptionalSentimentFilterOutputTypeDef",
+    {
+        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "ParticipantRole": ParticipantRoleType,
+        "Negate": bool,
+    },
+    total=False,
+)
+
+class SentimentFilterOutputTypeDef(
+    _RequiredSentimentFilterOutputTypeDef, _OptionalSentimentFilterOutputTypeDef
+):
+    pass
+
 _RequiredSentimentFilterTypeDef = TypedDict(
     "_RequiredSentimentFilterTypeDef",
     {
         "Sentiments": Sequence[SentimentValueType],
     },
 )
 _OptionalSentimentFilterTypeDef = TypedDict(
@@ -987,18 +1035,39 @@
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
     total=False,
 )
 
-
 class SentimentFilterTypeDef(_RequiredSentimentFilterTypeDef, _OptionalSentimentFilterTypeDef):
     pass
 
+_RequiredTranscriptFilterOutputTypeDef = TypedDict(
+    "_RequiredTranscriptFilterOutputTypeDef",
+    {
+        "TranscriptFilterType": Literal["EXACT"],
+        "Targets": List[str],
+    },
+)
+_OptionalTranscriptFilterOutputTypeDef = TypedDict(
+    "_OptionalTranscriptFilterOutputTypeDef",
+    {
+        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "ParticipantRole": ParticipantRoleType,
+        "Negate": bool,
+    },
+    total=False,
+)
+
+class TranscriptFilterOutputTypeDef(
+    _RequiredTranscriptFilterOutputTypeDef, _OptionalTranscriptFilterOutputTypeDef
+):
+    pass
 
 _RequiredTranscriptFilterTypeDef = TypedDict(
     "_RequiredTranscriptFilterTypeDef",
     {
         "TranscriptFilterType": Literal["EXACT"],
         "Targets": Sequence[str],
     },
@@ -1010,55 +1079,53 @@
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
     total=False,
 )
 
-
 class TranscriptFilterTypeDef(_RequiredTranscriptFilterTypeDef, _OptionalTranscriptFilterTypeDef):
     pass
 
-
 ListMedicalTranscriptionJobsResponseTypeDef = TypedDict(
     "ListMedicalTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "NextToken": str,
         "MedicalTranscriptionJobSummaries": List[MedicalTranscriptionJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMedicalVocabulariesResponseTypeDef = TypedDict(
     "ListMedicalVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVocabulariesResponseTypeDef = TypedDict(
     "ListVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVocabularyFiltersResponseTypeDef = TypedDict(
     "ListVocabularyFiltersResponseTypeDef",
     {
         "NextToken": str,
         "VocabularyFilters": List[VocabularyFilterInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MedicalTranscriptionJobTypeDef = TypedDict(
     "MedicalTranscriptionJobTypeDef",
     {
         "MedicalTranscriptionJobName": str,
@@ -1103,34 +1170,32 @@
         "Settings": MedicalTranscriptionSettingTypeDef,
         "ContentIdentificationType": Literal["PHI"],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartMedicalTranscriptionJobRequestRequestTypeDef(
     _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef,
     _OptionalStartMedicalTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
-
 TranscriptionJobSummaryTypeDef = TypedDict(
     "TranscriptionJobSummaryTypeDef",
     {
         "TranscriptionJobName": str,
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
         "LanguageCode": LanguageCodeType,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "FailureReason": str,
         "OutputLocationType": OutputLocationTypeType,
-        "ContentRedaction": ContentRedactionTypeDef,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
         "ModelSettings": ModelSettingsTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
     },
     total=False,
@@ -1163,22 +1228,20 @@
         "Subtitles": SubtitlesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
     },
     total=False,
 )
 
-
 class StartTranscriptionJobRequestRequestTypeDef(
     _RequiredStartTranscriptionJobRequestRequestTypeDef,
     _OptionalStartTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
-
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
@@ -1188,15 +1251,15 @@
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "Settings": SettingsTypeDef,
         "ModelSettings": ModelSettingsTypeDef,
         "JobExecutionSettings": JobExecutionSettingsTypeDef,
-        "ContentRedaction": ContentRedactionTypeDef,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": List[LanguageCodeType],
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
         "Tags": List[TagTypeDef],
         "Subtitles": SubtitlesOutputTypeDef,
@@ -1217,20 +1280,23 @@
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "DataAccessRoleArn": str,
         "IdentifiedLanguageScore": float,
-        "Settings": CallAnalyticsJobSettingsTypeDef,
+        "Settings": CallAnalyticsJobSettingsOutputTypeDef,
         "ChannelDefinitions": List[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
+CallAnalyticsJobSettingsUnionTypeDef = Union[
+    CallAnalyticsJobSettingsTypeDef, CallAnalyticsJobSettingsOutputTypeDef
+]
 _RequiredStartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
     },
 )
@@ -1242,39 +1308,48 @@
         "DataAccessRoleArn": str,
         "Settings": CallAnalyticsJobSettingsTypeDef,
         "ChannelDefinitions": Sequence[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
-
 class StartCallAnalyticsJobRequestRequestTypeDef(
     _RequiredStartCallAnalyticsJobRequestRequestTypeDef,
     _OptionalStartCallAnalyticsJobRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeLanguageModelResponseTypeDef = TypedDict(
     "DescribeLanguageModelResponseTypeDef",
     {
         "LanguageModel": LanguageModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLanguageModelsResponseTypeDef = TypedDict(
     "ListLanguageModelsResponseTypeDef",
     {
         "NextToken": str,
         "Models": List[LanguageModelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
+        "InterruptionFilter": InterruptionFilterTypeDef,
+        "TranscriptFilter": TranscriptFilterOutputTypeDef,
+        "SentimentFilter": SentimentFilterOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
         "InterruptionFilter": InterruptionFilterTypeDef,
         "TranscriptFilter": TranscriptFilterTypeDef,
         "SentimentFilter": SentimentFilterTypeDef,
@@ -1282,151 +1357,148 @@
     total=False,
 )
 
 GetMedicalTranscriptionJobResponseTypeDef = TypedDict(
     "GetMedicalTranscriptionJobResponseTypeDef",
     {
         "MedicalTranscriptionJob": MedicalTranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMedicalTranscriptionJobResponseTypeDef = TypedDict(
     "StartMedicalTranscriptionJobResponseTypeDef",
     {
         "MedicalTranscriptionJob": MedicalTranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTranscriptionJobsResponseTypeDef = TypedDict(
     "ListTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "NextToken": str,
         "TranscriptionJobSummaries": List[TranscriptionJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTranscriptionJobResponseTypeDef = TypedDict(
     "GetTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTranscriptionJobResponseTypeDef = TypedDict(
     "StartTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCallAnalyticsJobResponseTypeDef = TypedDict(
     "GetCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartCallAnalyticsJobResponseTypeDef = TypedDict(
     "StartCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CategoryPropertiesTypeDef = TypedDict(
     "CategoryPropertiesTypeDef",
     {
         "CategoryName": str,
-        "Rules": List[RuleTypeDef],
+        "Rules": List[RuleOutputTypeDef],
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "InputType": InputTypeType,
     },
     total=False,
 )
 
+RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
+CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
+    "CreateCallAnalyticsCategoryResponseTypeDef",
+    {
+        "CategoryProperties": CategoryPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCallAnalyticsCategoryResponseTypeDef = TypedDict(
+    "GetCallAnalyticsCategoryResponseTypeDef",
+    {
+        "CategoryProperties": CategoryPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
+    "ListCallAnalyticsCategoriesResponseTypeDef",
+    {
+        "NextToken": str,
+        "Categories": List[CategoryPropertiesTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
+    "UpdateCallAnalyticsCategoryResponseTypeDef",
+    {
+        "CategoryProperties": CategoryPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
     },
 )
 _OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "InputType": InputTypeType,
     },
     total=False,
 )
 
-
 class CreateCallAnalyticsCategoryRequestRequestTypeDef(
     _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef,
     _OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
     },
 )
 _OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "InputType": InputTypeType,
     },
     total=False,
 )
 
-
 class UpdateCallAnalyticsCategoryRequestRequestTypeDef(
     _RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef,
     _OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef,
 ):
     pass
-
-
-CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
-    "CreateCallAnalyticsCategoryResponseTypeDef",
-    {
-        "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetCallAnalyticsCategoryResponseTypeDef = TypedDict(
-    "GetCallAnalyticsCategoryResponseTypeDef",
-    {
-        "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
-    "ListCallAnalyticsCategoriesResponseTypeDef",
-    {
-        "NextToken": str,
-        "Categories": List[CategoryPropertiesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
-    "UpdateCallAnalyticsCategoryResponseTypeDef",
-    {
-        "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe/type_defs.pyi` & `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_transcribe.type_defs import AbsoluteTimeRangeTypeDef
 
-    data: AbsoluteTimeRangeTypeDef = {...}
+    data: AbsoluteTimeRangeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     BaseModelNameType,
     CallAnalyticsJobStatusType,
     CLMLanguageCodeType,
     InputTypeType,
     LanguageCodeType,
@@ -40,47 +40,43 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AbsoluteTimeRangeTypeDef",
-    "ContentRedactionTypeDef",
+    "ContentRedactionOutputTypeDef",
     "LanguageIdSettingsTypeDef",
+    "ContentRedactionTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
     "ChannelDefinitionTypeDef",
     "MediaTypeDef",
     "TranscriptTypeDef",
+    "ResponseMetadataTypeDef",
     "InputDataConfigTypeDef",
     "TagTypeDef",
-    "CreateMedicalVocabularyResponseTypeDef",
-    "CreateVocabularyFilterResponseTypeDef",
-    "CreateVocabularyResponseTypeDef",
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     "DeleteCallAnalyticsJobRequestRequestTypeDef",
     "DeleteLanguageModelRequestRequestTypeDef",
     "DeleteMedicalTranscriptionJobRequestRequestTypeDef",
     "DeleteMedicalVocabularyRequestRequestTypeDef",
     "DeleteTranscriptionJobRequestRequestTypeDef",
     "DeleteVocabularyFilterRequestRequestTypeDef",
     "DeleteVocabularyRequestRequestTypeDef",
     "DescribeLanguageModelRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     "GetCallAnalyticsJobRequestRequestTypeDef",
     "GetMedicalTranscriptionJobRequestRequestTypeDef",
     "GetMedicalVocabularyRequestRequestTypeDef",
-    "GetMedicalVocabularyResponseTypeDef",
     "GetTranscriptionJobRequestRequestTypeDef",
     "GetVocabularyFilterRequestRequestTypeDef",
-    "GetVocabularyFilterResponseTypeDef",
     "GetVocabularyRequestRequestTypeDef",
-    "GetVocabularyResponseTypeDef",
     "RelativeTimeRangeTypeDef",
     "JobExecutionSettingsTypeDef",
     "LanguageCodeItemTypeDef",
     "ListCallAnalyticsCategoriesRequestRequestTypeDef",
     "ListCallAnalyticsJobsRequestRequestTypeDef",
     "ListLanguageModelsRequestRequestTypeDef",
     "ListMedicalTranscriptionJobsRequestRequestTypeDef",
@@ -91,108 +87,145 @@
     "ListTranscriptionJobsRequestRequestTypeDef",
     "ListVocabulariesRequestRequestTypeDef",
     "ListVocabularyFiltersRequestRequestTypeDef",
     "VocabularyFilterInfoTypeDef",
     "MedicalTranscriptTypeDef",
     "MedicalTranscriptionSettingTypeDef",
     "ModelSettingsTypeDef",
-    "ResponseMetadataTypeDef",
     "SettingsTypeDef",
     "SubtitlesTypeDef",
     "SubtitlesOutputTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMedicalVocabularyRequestRequestTypeDef",
-    "UpdateMedicalVocabularyResponseTypeDef",
     "UpdateVocabularyFilterRequestRequestTypeDef",
-    "UpdateVocabularyFilterResponseTypeDef",
     "UpdateVocabularyRequestRequestTypeDef",
-    "UpdateVocabularyResponseTypeDef",
+    "CallAnalyticsJobSettingsOutputTypeDef",
     "CallAnalyticsJobSettingsTypeDef",
+    "ContentRedactionUnionTypeDef",
+    "CreateMedicalVocabularyResponseTypeDef",
+    "CreateVocabularyFilterResponseTypeDef",
+    "CreateVocabularyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetMedicalVocabularyResponseTypeDef",
+    "GetVocabularyFilterResponseTypeDef",
+    "GetVocabularyResponseTypeDef",
     "ListCallAnalyticsJobsResponseTypeDef",
+    "UpdateMedicalVocabularyResponseTypeDef",
+    "UpdateVocabularyFilterResponseTypeDef",
+    "UpdateVocabularyResponseTypeDef",
     "CreateLanguageModelResponseTypeDef",
     "LanguageModelTypeDef",
     "CreateLanguageModelRequestRequestTypeDef",
     "CreateMedicalVocabularyRequestRequestTypeDef",
     "CreateVocabularyFilterRequestRequestTypeDef",
     "CreateVocabularyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "InterruptionFilterTypeDef",
     "NonTalkTimeFilterTypeDef",
+    "SentimentFilterOutputTypeDef",
     "SentimentFilterTypeDef",
+    "TranscriptFilterOutputTypeDef",
     "TranscriptFilterTypeDef",
     "ListMedicalTranscriptionJobsResponseTypeDef",
     "ListMedicalVocabulariesResponseTypeDef",
     "ListVocabulariesResponseTypeDef",
     "ListVocabularyFiltersResponseTypeDef",
     "MedicalTranscriptionJobTypeDef",
     "StartMedicalTranscriptionJobRequestRequestTypeDef",
     "TranscriptionJobSummaryTypeDef",
     "StartTranscriptionJobRequestRequestTypeDef",
     "TranscriptionJobTypeDef",
     "CallAnalyticsJobTypeDef",
+    "CallAnalyticsJobSettingsUnionTypeDef",
     "StartCallAnalyticsJobRequestRequestTypeDef",
     "DescribeLanguageModelResponseTypeDef",
     "ListLanguageModelsResponseTypeDef",
+    "RuleOutputTypeDef",
     "RuleTypeDef",
     "GetMedicalTranscriptionJobResponseTypeDef",
     "StartMedicalTranscriptionJobResponseTypeDef",
     "ListTranscriptionJobsResponseTypeDef",
     "GetTranscriptionJobResponseTypeDef",
     "StartTranscriptionJobResponseTypeDef",
     "GetCallAnalyticsJobResponseTypeDef",
     "StartCallAnalyticsJobResponseTypeDef",
     "CategoryPropertiesTypeDef",
-    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
-    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
+    "RuleUnionTypeDef",
     "CreateCallAnalyticsCategoryResponseTypeDef",
     "GetCallAnalyticsCategoryResponseTypeDef",
     "ListCallAnalyticsCategoriesResponseTypeDef",
     "UpdateCallAnalyticsCategoryResponseTypeDef",
+    "CreateCallAnalyticsCategoryRequestRequestTypeDef",
+    "UpdateCallAnalyticsCategoryRequestRequestTypeDef",
 )
 
 AbsoluteTimeRangeTypeDef = TypedDict(
     "AbsoluteTimeRangeTypeDef",
     {
         "StartTime": int,
         "EndTime": int,
         "First": int,
         "Last": int,
     },
     total=False,
 )
 
-_RequiredContentRedactionTypeDef = TypedDict(
-    "_RequiredContentRedactionTypeDef",
+_RequiredContentRedactionOutputTypeDef = TypedDict(
+    "_RequiredContentRedactionOutputTypeDef",
     {
         "RedactionType": Literal["PII"],
         "RedactionOutput": RedactionOutputType,
     },
 )
-_OptionalContentRedactionTypeDef = TypedDict(
-    "_OptionalContentRedactionTypeDef",
+_OptionalContentRedactionOutputTypeDef = TypedDict(
+    "_OptionalContentRedactionOutputTypeDef",
     {
         "PiiEntityTypes": List[PiiEntityTypeType],
     },
     total=False,
 )
 
-class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
+
+class ContentRedactionOutputTypeDef(
+    _RequiredContentRedactionOutputTypeDef, _OptionalContentRedactionOutputTypeDef
+):
     pass
 
+
 LanguageIdSettingsTypeDef = TypedDict(
     "LanguageIdSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "LanguageModelName": str,
     },
     total=False,
 )
 
+_RequiredContentRedactionTypeDef = TypedDict(
+    "_RequiredContentRedactionTypeDef",
+    {
+        "RedactionType": Literal["PII"],
+        "RedactionOutput": RedactionOutputType,
+    },
+)
+_OptionalContentRedactionTypeDef = TypedDict(
+    "_OptionalContentRedactionTypeDef",
+    {
+        "PiiEntityTypes": Sequence[PiiEntityTypeType],
+    },
+    total=False,
+)
+
+
+class ContentRedactionTypeDef(_RequiredContentRedactionTypeDef, _OptionalContentRedactionTypeDef):
+    pass
+
+
 CallAnalyticsJobSummaryTypeDef = TypedDict(
     "CallAnalyticsJobSummaryTypeDef",
     {
         "CallAnalyticsJobName": str,
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
@@ -226,14 +259,25 @@
     {
         "TranscriptFileUri": str,
         "RedactedTranscriptFileUri": str,
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
 _RequiredInputDataConfigTypeDef = TypedDict(
     "_RequiredInputDataConfigTypeDef",
     {
         "S3Uri": str,
         "DataAccessRoleArn": str,
     },
 )
@@ -241,59 +285,27 @@
     "_OptionalInputDataConfigTypeDef",
     {
         "TuningDataS3Uri": str,
     },
     total=False,
 )
 
+
 class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateMedicalVocabularyResponseTypeDef = TypedDict(
-    "CreateMedicalVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVocabularyFilterResponseTypeDef = TypedDict(
-    "CreateVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateVocabularyResponseTypeDef = TypedDict(
-    "CreateVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "DeleteCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -349,21 +361,14 @@
 DescribeLanguageModelRequestRequestTypeDef = TypedDict(
     "DescribeLanguageModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "GetCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
     },
 )
 
@@ -384,72 +389,35 @@
 GetMedicalVocabularyRequestRequestTypeDef = TypedDict(
     "GetMedicalVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
-GetMedicalVocabularyResponseTypeDef = TypedDict(
-    "GetMedicalVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "DownloadUri": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTranscriptionJobRequestRequestTypeDef = TypedDict(
     "GetTranscriptionJobRequestRequestTypeDef",
     {
         "TranscriptionJobName": str,
     },
 )
 
 GetVocabularyFilterRequestRequestTypeDef = TypedDict(
     "GetVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
     },
 )
 
-GetVocabularyFilterResponseTypeDef = TypedDict(
-    "GetVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "DownloadUri": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVocabularyRequestRequestTypeDef = TypedDict(
     "GetVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
     },
 )
 
-GetVocabularyResponseTypeDef = TypedDict(
-    "GetVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "VocabularyState": VocabularyStateType,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "DownloadUri": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RelativeTimeRangeTypeDef = TypedDict(
     "RelativeTimeRangeTypeDef",
     {
         "StartPercentage": int,
         "EndPercentage": int,
         "First": int,
         "Last": int,
@@ -631,25 +599,14 @@
     "ModelSettingsTypeDef",
     {
         "LanguageModelName": str,
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
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "VocabularyName": str,
         "ShowSpeakerLabels": bool,
         "MaxSpeakerLabels": int,
         "ChannelIdentification": bool,
@@ -693,25 +650,14 @@
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "VocabularyFileUri": str,
     },
 )
 
-UpdateMedicalVocabularyResponseTypeDef = TypedDict(
-    "UpdateMedicalVocabularyResponseTypeDef",
-    {
-        "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "VocabularyState": VocabularyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVocabularyFilterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
     },
 )
 _OptionalUpdateVocabularyFilterRequestRequestTypeDef = TypedDict(
@@ -720,29 +666,21 @@
         "Words": Sequence[str],
         "VocabularyFilterFileUri": str,
         "DataAccessRoleArn": str,
     },
     total=False,
 )
 
+
 class UpdateVocabularyFilterRequestRequestTypeDef(
     _RequiredUpdateVocabularyFilterRequestRequestTypeDef,
     _OptionalUpdateVocabularyFilterRequestRequestTypeDef,
 ):
     pass
 
-UpdateVocabularyFilterResponseTypeDef = TypedDict(
-    "UpdateVocabularyFilterResponseTypeDef",
-    {
-        "VocabularyFilterName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
     },
@@ -753,63 +691,179 @@
         "Phrases": Sequence[str],
         "VocabularyFileUri": str,
         "DataAccessRoleArn": str,
     },
     total=False,
 )
 
+
 class UpdateVocabularyRequestRequestTypeDef(
     _RequiredUpdateVocabularyRequestRequestTypeDef, _OptionalUpdateVocabularyRequestRequestTypeDef
 ):
     pass
 
-UpdateVocabularyResponseTypeDef = TypedDict(
-    "UpdateVocabularyResponseTypeDef",
+
+CallAnalyticsJobSettingsOutputTypeDef = TypedDict(
+    "CallAnalyticsJobSettingsOutputTypeDef",
     {
         "VocabularyName": str,
-        "LanguageCode": LanguageCodeType,
-        "LastModifiedTime": datetime,
-        "VocabularyState": VocabularyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VocabularyFilterName": str,
+        "VocabularyFilterMethod": VocabularyFilterMethodType,
+        "LanguageModelName": str,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
+        "LanguageOptions": List[LanguageCodeType],
+        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
     },
+    total=False,
 )
 
 CallAnalyticsJobSettingsTypeDef = TypedDict(
     "CallAnalyticsJobSettingsTypeDef",
     {
         "VocabularyName": str,
         "VocabularyFilterName": str,
         "VocabularyFilterMethod": VocabularyFilterMethodType,
         "LanguageModelName": str,
         "ContentRedaction": ContentRedactionTypeDef,
-        "LanguageOptions": List[LanguageCodeType],
-        "LanguageIdSettings": Dict[LanguageCodeType, LanguageIdSettingsTypeDef],
+        "LanguageOptions": Sequence[LanguageCodeType],
+        "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
     },
     total=False,
 )
 
+ContentRedactionUnionTypeDef = Union[ContentRedactionTypeDef, ContentRedactionOutputTypeDef]
+CreateMedicalVocabularyResponseTypeDef = TypedDict(
+    "CreateMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVocabularyFilterResponseTypeDef = TypedDict(
+    "CreateVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVocabularyResponseTypeDef = TypedDict(
+    "CreateVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
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
+GetMedicalVocabularyResponseTypeDef = TypedDict(
+    "GetMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "DownloadUri": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVocabularyFilterResponseTypeDef = TypedDict(
+    "GetVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "DownloadUri": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVocabularyResponseTypeDef = TypedDict(
+    "GetVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "VocabularyState": VocabularyStateType,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "DownloadUri": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListCallAnalyticsJobsResponseTypeDef = TypedDict(
     "ListCallAnalyticsJobsResponseTypeDef",
     {
         "Status": CallAnalyticsJobStatusType,
         "NextToken": str,
         "CallAnalyticsJobSummaries": List[CallAnalyticsJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMedicalVocabularyResponseTypeDef = TypedDict(
+    "UpdateMedicalVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "VocabularyState": VocabularyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVocabularyFilterResponseTypeDef = TypedDict(
+    "UpdateVocabularyFilterResponseTypeDef",
+    {
+        "VocabularyFilterName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVocabularyResponseTypeDef = TypedDict(
+    "UpdateVocabularyResponseTypeDef",
+    {
+        "VocabularyName": str,
+        "LanguageCode": LanguageCodeType,
+        "LastModifiedTime": datetime,
+        "VocabularyState": VocabularyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLanguageModelResponseTypeDef = TypedDict(
     "CreateLanguageModelResponseTypeDef",
     {
         "LanguageCode": CLMLanguageCodeType,
         "BaseModelName": BaseModelNameType,
         "ModelName": str,
         "InputDataConfig": InputDataConfigTypeDef,
         "ModelStatus": ModelStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LanguageModelTypeDef = TypedDict(
     "LanguageModelTypeDef",
     {
         "ModelName": str,
@@ -838,20 +892,22 @@
     "_OptionalCreateLanguageModelRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateLanguageModelRequestRequestTypeDef(
     _RequiredCreateLanguageModelRequestRequestTypeDef,
     _OptionalCreateLanguageModelRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateMedicalVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMedicalVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
         "VocabularyFileUri": str,
     },
@@ -860,20 +916,22 @@
     "_OptionalCreateMedicalVocabularyRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateMedicalVocabularyRequestRequestTypeDef(
     _RequiredCreateMedicalVocabularyRequestRequestTypeDef,
     _OptionalCreateMedicalVocabularyRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateVocabularyFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVocabularyFilterRequestRequestTypeDef",
     {
         "VocabularyFilterName": str,
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -884,20 +942,22 @@
         "VocabularyFilterFileUri": str,
         "Tags": Sequence[TagTypeDef],
         "DataAccessRoleArn": str,
     },
     total=False,
 )
 
+
 class CreateVocabularyFilterRequestRequestTypeDef(
     _RequiredCreateVocabularyFilterRequestRequestTypeDef,
     _OptionalCreateVocabularyFilterRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateVocabularyRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVocabularyRequestRequestTypeDef",
     {
         "VocabularyName": str,
         "LanguageCode": LanguageCodeType,
     },
 )
@@ -908,25 +968,27 @@
         "VocabularyFileUri": str,
         "Tags": Sequence[TagTypeDef],
         "DataAccessRoleArn": str,
     },
     total=False,
 )
 
+
 class CreateVocabularyRequestRequestTypeDef(
     _RequiredCreateVocabularyRequestRequestTypeDef, _OptionalCreateVocabularyRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -953,14 +1015,38 @@
         "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
         "Negate": bool,
     },
     total=False,
 )
 
+_RequiredSentimentFilterOutputTypeDef = TypedDict(
+    "_RequiredSentimentFilterOutputTypeDef",
+    {
+        "Sentiments": List[SentimentValueType],
+    },
+)
+_OptionalSentimentFilterOutputTypeDef = TypedDict(
+    "_OptionalSentimentFilterOutputTypeDef",
+    {
+        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "ParticipantRole": ParticipantRoleType,
+        "Negate": bool,
+    },
+    total=False,
+)
+
+
+class SentimentFilterOutputTypeDef(
+    _RequiredSentimentFilterOutputTypeDef, _OptionalSentimentFilterOutputTypeDef
+):
+    pass
+
+
 _RequiredSentimentFilterTypeDef = TypedDict(
     "_RequiredSentimentFilterTypeDef",
     {
         "Sentiments": Sequence[SentimentValueType],
     },
 )
 _OptionalSentimentFilterTypeDef = TypedDict(
@@ -970,17 +1056,44 @@
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
     total=False,
 )
 
+
 class SentimentFilterTypeDef(_RequiredSentimentFilterTypeDef, _OptionalSentimentFilterTypeDef):
     pass
 
+
+_RequiredTranscriptFilterOutputTypeDef = TypedDict(
+    "_RequiredTranscriptFilterOutputTypeDef",
+    {
+        "TranscriptFilterType": Literal["EXACT"],
+        "Targets": List[str],
+    },
+)
+_OptionalTranscriptFilterOutputTypeDef = TypedDict(
+    "_OptionalTranscriptFilterOutputTypeDef",
+    {
+        "AbsoluteTimeRange": AbsoluteTimeRangeTypeDef,
+        "RelativeTimeRange": RelativeTimeRangeTypeDef,
+        "ParticipantRole": ParticipantRoleType,
+        "Negate": bool,
+    },
+    total=False,
+)
+
+
+class TranscriptFilterOutputTypeDef(
+    _RequiredTranscriptFilterOutputTypeDef, _OptionalTranscriptFilterOutputTypeDef
+):
+    pass
+
+
 _RequiredTranscriptFilterTypeDef = TypedDict(
     "_RequiredTranscriptFilterTypeDef",
     {
         "TranscriptFilterType": Literal["EXACT"],
         "Targets": Sequence[str],
     },
 )
@@ -991,53 +1104,55 @@
         "RelativeTimeRange": RelativeTimeRangeTypeDef,
         "ParticipantRole": ParticipantRoleType,
         "Negate": bool,
     },
     total=False,
 )
 
+
 class TranscriptFilterTypeDef(_RequiredTranscriptFilterTypeDef, _OptionalTranscriptFilterTypeDef):
     pass
 
+
 ListMedicalTranscriptionJobsResponseTypeDef = TypedDict(
     "ListMedicalTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "NextToken": str,
         "MedicalTranscriptionJobSummaries": List[MedicalTranscriptionJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMedicalVocabulariesResponseTypeDef = TypedDict(
     "ListMedicalVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVocabulariesResponseTypeDef = TypedDict(
     "ListVocabulariesResponseTypeDef",
     {
         "Status": VocabularyStateType,
         "NextToken": str,
         "Vocabularies": List[VocabularyInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVocabularyFiltersResponseTypeDef = TypedDict(
     "ListVocabularyFiltersResponseTypeDef",
     {
         "NextToken": str,
         "VocabularyFilters": List[VocabularyFilterInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MedicalTranscriptionJobTypeDef = TypedDict(
     "MedicalTranscriptionJobTypeDef",
     {
         "MedicalTranscriptionJobName": str,
@@ -1082,32 +1197,34 @@
         "Settings": MedicalTranscriptionSettingTypeDef,
         "ContentIdentificationType": Literal["PHI"],
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartMedicalTranscriptionJobRequestRequestTypeDef(
     _RequiredStartMedicalTranscriptionJobRequestRequestTypeDef,
     _OptionalStartMedicalTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
+
 TranscriptionJobSummaryTypeDef = TypedDict(
     "TranscriptionJobSummaryTypeDef",
     {
         "TranscriptionJobName": str,
         "CreationTime": datetime,
         "StartTime": datetime,
         "CompletionTime": datetime,
         "LanguageCode": LanguageCodeType,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "FailureReason": str,
         "OutputLocationType": OutputLocationTypeType,
-        "ContentRedaction": ContentRedactionTypeDef,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
         "ModelSettings": ModelSettingsTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
     },
     total=False,
@@ -1140,20 +1257,22 @@
         "Subtitles": SubtitlesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "LanguageIdSettings": Mapping[LanguageCodeType, LanguageIdSettingsTypeDef],
     },
     total=False,
 )
 
+
 class StartTranscriptionJobRequestRequestTypeDef(
     _RequiredStartTranscriptionJobRequestRequestTypeDef,
     _OptionalStartTranscriptionJobRequestRequestTypeDef,
 ):
     pass
 
+
 TranscriptionJobTypeDef = TypedDict(
     "TranscriptionJobTypeDef",
     {
         "TranscriptionJobName": str,
         "TranscriptionJobStatus": TranscriptionJobStatusType,
         "LanguageCode": LanguageCodeType,
         "MediaSampleRateHertz": int,
@@ -1163,15 +1282,15 @@
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "Settings": SettingsTypeDef,
         "ModelSettings": ModelSettingsTypeDef,
         "JobExecutionSettings": JobExecutionSettingsTypeDef,
-        "ContentRedaction": ContentRedactionTypeDef,
+        "ContentRedaction": ContentRedactionOutputTypeDef,
         "IdentifyLanguage": bool,
         "IdentifyMultipleLanguages": bool,
         "LanguageOptions": List[LanguageCodeType],
         "IdentifiedLanguageScore": float,
         "LanguageCodes": List[LanguageCodeItemTypeDef],
         "Tags": List[TagTypeDef],
         "Subtitles": SubtitlesOutputTypeDef,
@@ -1192,20 +1311,23 @@
         "Transcript": TranscriptTypeDef,
         "StartTime": datetime,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "FailureReason": str,
         "DataAccessRoleArn": str,
         "IdentifiedLanguageScore": float,
-        "Settings": CallAnalyticsJobSettingsTypeDef,
+        "Settings": CallAnalyticsJobSettingsOutputTypeDef,
         "ChannelDefinitions": List[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
+CallAnalyticsJobSettingsUnionTypeDef = Union[
+    CallAnalyticsJobSettingsTypeDef, CallAnalyticsJobSettingsOutputTypeDef
+]
 _RequiredStartCallAnalyticsJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartCallAnalyticsJobRequestRequestTypeDef",
     {
         "CallAnalyticsJobName": str,
         "Media": MediaTypeDef,
     },
 )
@@ -1217,37 +1339,50 @@
         "DataAccessRoleArn": str,
         "Settings": CallAnalyticsJobSettingsTypeDef,
         "ChannelDefinitions": Sequence[ChannelDefinitionTypeDef],
     },
     total=False,
 )
 
+
 class StartCallAnalyticsJobRequestRequestTypeDef(
     _RequiredStartCallAnalyticsJobRequestRequestTypeDef,
     _OptionalStartCallAnalyticsJobRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeLanguageModelResponseTypeDef = TypedDict(
     "DescribeLanguageModelResponseTypeDef",
     {
         "LanguageModel": LanguageModelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLanguageModelsResponseTypeDef = TypedDict(
     "ListLanguageModelsResponseTypeDef",
     {
         "NextToken": str,
         "Models": List[LanguageModelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RuleOutputTypeDef = TypedDict(
+    "RuleOutputTypeDef",
+    {
+        "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
+        "InterruptionFilter": InterruptionFilterTypeDef,
+        "TranscriptFilter": TranscriptFilterOutputTypeDef,
+        "SentimentFilter": SentimentFilterOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleTypeDef = TypedDict(
     "RuleTypeDef",
     {
         "NonTalkTimeFilter": NonTalkTimeFilterTypeDef,
         "InterruptionFilter": InterruptionFilterTypeDef,
         "TranscriptFilter": TranscriptFilterTypeDef,
         "SentimentFilter": SentimentFilterTypeDef,
@@ -1255,147 +1390,151 @@
     total=False,
 )
 
 GetMedicalTranscriptionJobResponseTypeDef = TypedDict(
     "GetMedicalTranscriptionJobResponseTypeDef",
     {
         "MedicalTranscriptionJob": MedicalTranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMedicalTranscriptionJobResponseTypeDef = TypedDict(
     "StartMedicalTranscriptionJobResponseTypeDef",
     {
         "MedicalTranscriptionJob": MedicalTranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTranscriptionJobsResponseTypeDef = TypedDict(
     "ListTranscriptionJobsResponseTypeDef",
     {
         "Status": TranscriptionJobStatusType,
         "NextToken": str,
         "TranscriptionJobSummaries": List[TranscriptionJobSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTranscriptionJobResponseTypeDef = TypedDict(
     "GetTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartTranscriptionJobResponseTypeDef = TypedDict(
     "StartTranscriptionJobResponseTypeDef",
     {
         "TranscriptionJob": TranscriptionJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCallAnalyticsJobResponseTypeDef = TypedDict(
     "GetCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartCallAnalyticsJobResponseTypeDef = TypedDict(
     "StartCallAnalyticsJobResponseTypeDef",
     {
         "CallAnalyticsJob": CallAnalyticsJobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CategoryPropertiesTypeDef = TypedDict(
     "CategoryPropertiesTypeDef",
     {
         "CategoryName": str,
-        "Rules": List[RuleTypeDef],
+        "Rules": List[RuleOutputTypeDef],
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "InputType": InputTypeType,
     },
     total=False,
 )
 
+RuleUnionTypeDef = Union[RuleTypeDef, RuleOutputTypeDef]
+CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
+    "CreateCallAnalyticsCategoryResponseTypeDef",
+    {
+        "CategoryProperties": CategoryPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCallAnalyticsCategoryResponseTypeDef = TypedDict(
+    "GetCallAnalyticsCategoryResponseTypeDef",
+    {
+        "CategoryProperties": CategoryPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
+    "ListCallAnalyticsCategoriesResponseTypeDef",
+    {
+        "NextToken": str,
+        "Categories": List[CategoryPropertiesTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
+    "UpdateCallAnalyticsCategoryResponseTypeDef",
+    {
+        "CategoryProperties": CategoryPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
     },
 )
 _OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "InputType": InputTypeType,
     },
     total=False,
 )
 
+
 class CreateCallAnalyticsCategoryRequestRequestTypeDef(
     _RequiredCreateCallAnalyticsCategoryRequestRequestTypeDef,
     _OptionalCreateCallAnalyticsCategoryRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "CategoryName": str,
-        "Rules": Sequence[RuleTypeDef],
+        "Rules": Sequence[RuleUnionTypeDef],
     },
 )
 _OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef",
     {
         "InputType": InputTypeType,
     },
     total=False,
 )
 
+
 class UpdateCallAnalyticsCategoryRequestRequestTypeDef(
     _RequiredUpdateCallAnalyticsCategoryRequestRequestTypeDef,
     _OptionalUpdateCallAnalyticsCategoryRequestRequestTypeDef,
 ):
     pass
-
-CreateCallAnalyticsCategoryResponseTypeDef = TypedDict(
-    "CreateCallAnalyticsCategoryResponseTypeDef",
-    {
-        "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetCallAnalyticsCategoryResponseTypeDef = TypedDict(
-    "GetCallAnalyticsCategoryResponseTypeDef",
-    {
-        "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCallAnalyticsCategoriesResponseTypeDef = TypedDict(
-    "ListCallAnalyticsCategoriesResponseTypeDef",
-    {
-        "NextToken": str,
-        "Categories": List[CategoryPropertiesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateCallAnalyticsCategoryResponseTypeDef = TypedDict(
-    "UpdateCallAnalyticsCategoryResponseTypeDef",
-    {
-        "CategoryProperties": CategoryPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe.egg-info/PKG-INFO` & `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-transcribe
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.TranscribeService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.TranscribeService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore transcribe type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore transcribe type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-transcribe"></a>
 
 # types-aiobotocore-transcribe
 
 [![PyPI - types-aiobotocore-transcribe](https://img.shields.io/pypi/v/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-transcribe?color=blue)](https://pypistats.org/packages/types-aiobotocore-transcribe)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transcribe)](https://pepy.tech/project/types-aiobotocore-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.TranscribeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [types-aiobotocore-transcribe docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/).
 
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
@@ -301,55 +300,50 @@
 )
 
 
 def check_value(value: BaseModelNameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_transcribe.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_transcribe.type_defs import (
     AbsoluteTimeRangeTypeDef,
-    ContentRedactionTypeDef,
+    ContentRedactionOutputTypeDef,
     LanguageIdSettingsTypeDef,
+    ContentRedactionTypeDef,
     CallAnalyticsJobSummaryTypeDef,
     ChannelDefinitionTypeDef,
     MediaTypeDef,
     TranscriptTypeDef,
+    ResponseMetadataTypeDef,
     InputDataConfigTypeDef,
     TagTypeDef,
-    CreateMedicalVocabularyResponseTypeDef,
-    CreateVocabularyFilterResponseTypeDef,
-    CreateVocabularyResponseTypeDef,
     DeleteCallAnalyticsCategoryRequestRequestTypeDef,
     DeleteCallAnalyticsJobRequestRequestTypeDef,
     DeleteLanguageModelRequestRequestTypeDef,
     DeleteMedicalTranscriptionJobRequestRequestTypeDef,
     DeleteMedicalVocabularyRequestRequestTypeDef,
     DeleteTranscriptionJobRequestRequestTypeDef,
     DeleteVocabularyFilterRequestRequestTypeDef,
     DeleteVocabularyRequestRequestTypeDef,
     DescribeLanguageModelRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetCallAnalyticsCategoryRequestRequestTypeDef,
     GetCallAnalyticsJobRequestRequestTypeDef,
     GetMedicalTranscriptionJobRequestRequestTypeDef,
     GetMedicalVocabularyRequestRequestTypeDef,
-    GetMedicalVocabularyResponseTypeDef,
     GetTranscriptionJobRequestRequestTypeDef,
     GetVocabularyFilterRequestRequestTypeDef,
-    GetVocabularyFilterResponseTypeDef,
     GetVocabularyRequestRequestTypeDef,
-    GetVocabularyResponseTypeDef,
     RelativeTimeRangeTypeDef,
     JobExecutionSettingsTypeDef,
     LanguageCodeItemTypeDef,
     ListCallAnalyticsCategoriesRequestRequestTypeDef,
     ListCallAnalyticsJobsRequestRequestTypeDef,
     ListLanguageModelsRequestRequestTypeDef,
     ListMedicalTranscriptionJobsRequestRequestTypeDef,
@@ -360,71 +354,84 @@
     ListTranscriptionJobsRequestRequestTypeDef,
     ListVocabulariesRequestRequestTypeDef,
     ListVocabularyFiltersRequestRequestTypeDef,
     VocabularyFilterInfoTypeDef,
     MedicalTranscriptTypeDef,
     MedicalTranscriptionSettingTypeDef,
     ModelSettingsTypeDef,
-    ResponseMetadataTypeDef,
     SettingsTypeDef,
     SubtitlesTypeDef,
     SubtitlesOutputTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateMedicalVocabularyRequestRequestTypeDef,
-    UpdateMedicalVocabularyResponseTypeDef,
     UpdateVocabularyFilterRequestRequestTypeDef,
-    UpdateVocabularyFilterResponseTypeDef,
     UpdateVocabularyRequestRequestTypeDef,
-    UpdateVocabularyResponseTypeDef,
+    CallAnalyticsJobSettingsOutputTypeDef,
     CallAnalyticsJobSettingsTypeDef,
+    ContentRedactionUnionTypeDef,
+    CreateMedicalVocabularyResponseTypeDef,
+    CreateVocabularyFilterResponseTypeDef,
+    CreateVocabularyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetMedicalVocabularyResponseTypeDef,
+    GetVocabularyFilterResponseTypeDef,
+    GetVocabularyResponseTypeDef,
     ListCallAnalyticsJobsResponseTypeDef,
+    UpdateMedicalVocabularyResponseTypeDef,
+    UpdateVocabularyFilterResponseTypeDef,
+    UpdateVocabularyResponseTypeDef,
     CreateLanguageModelResponseTypeDef,
     LanguageModelTypeDef,
     CreateLanguageModelRequestRequestTypeDef,
     CreateMedicalVocabularyRequestRequestTypeDef,
     CreateVocabularyFilterRequestRequestTypeDef,
     CreateVocabularyRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     InterruptionFilterTypeDef,
     NonTalkTimeFilterTypeDef,
+    SentimentFilterOutputTypeDef,
     SentimentFilterTypeDef,
+    TranscriptFilterOutputTypeDef,
     TranscriptFilterTypeDef,
     ListMedicalTranscriptionJobsResponseTypeDef,
     ListMedicalVocabulariesResponseTypeDef,
     ListVocabulariesResponseTypeDef,
     ListVocabularyFiltersResponseTypeDef,
     MedicalTranscriptionJobTypeDef,
     StartMedicalTranscriptionJobRequestRequestTypeDef,
     TranscriptionJobSummaryTypeDef,
     StartTranscriptionJobRequestRequestTypeDef,
     TranscriptionJobTypeDef,
     CallAnalyticsJobTypeDef,
+    CallAnalyticsJobSettingsUnionTypeDef,
     StartCallAnalyticsJobRequestRequestTypeDef,
     DescribeLanguageModelResponseTypeDef,
     ListLanguageModelsResponseTypeDef,
+    RuleOutputTypeDef,
     RuleTypeDef,
     GetMedicalTranscriptionJobResponseTypeDef,
     StartMedicalTranscriptionJobResponseTypeDef,
     ListTranscriptionJobsResponseTypeDef,
     GetTranscriptionJobResponseTypeDef,
     StartTranscriptionJobResponseTypeDef,
     GetCallAnalyticsJobResponseTypeDef,
     StartCallAnalyticsJobResponseTypeDef,
     CategoryPropertiesTypeDef,
-    CreateCallAnalyticsCategoryRequestRequestTypeDef,
-    UpdateCallAnalyticsCategoryRequestRequestTypeDef,
+    RuleUnionTypeDef,
     CreateCallAnalyticsCategoryResponseTypeDef,
     GetCallAnalyticsCategoryResponseTypeDef,
     ListCallAnalyticsCategoriesResponseTypeDef,
     UpdateCallAnalyticsCategoryResponseTypeDef,
+    CreateCallAnalyticsCategoryRequestRequestTypeDef,
+    UpdateCallAnalyticsCategoryRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AbsoluteTimeRangeTypeDef:
+def get_value() -> AbsoluteTimeRangeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-transcribe-2.5.2/types_aiobotocore_transcribe.egg-info/SOURCES.txt` & `types-aiobotocore-transcribe-2.5.2.post1/types_aiobotocore_transcribe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

